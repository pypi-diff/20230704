# Comparing `tmp/heimdallm-0.1.2.tar.gz` & `tmp/heimdallm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimdallm-0.1.2.tar", max compression
+gzip compressed data, was "heimdallm-0.1.3.tar", max compression
```

## Comparing `heimdallm-0.1.2.tar` & `heimdallm-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      750 2023-07-01 13:58:32.237701 heimdallm-0.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-07-01 13:58:32.237701 heimdallm-0.1.2/LICENSE
--rw-r--r--   0        0        0     6498 2023-07-01 13:58:32.237701 heimdallm-0.1.2/README.md
--rw-r--r--   0        0        0       81 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/__init__.py
--rw-r--r--   0        0        0     6301 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrost.py
--rw-r--r--   0        0        0        0 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/__init__.py
--rw-r--r--   0        0        0     4341 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/exc.py
--rw-r--r--   0        0        0        0 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/mysql/__init__.py
--rw-r--r--   0        0        0     3441 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/mysql/presets.py
--rw-r--r--   0        0        0        0 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/__init__.py
--rw-r--r--   0        0        0     3707 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/presets.py
--rw-r--r--   0        0        0        0 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/__init__.py
--rw-r--r--   0        0        0     4539 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
--rw-r--r--   0        0        0     4740 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/envelope.py
--rw-r--r--   0        0        0     1331 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2
--rw-r--r--   0        0        0     4756 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py
--rw-r--r--   0        0        0     6704 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark
--rw-r--r--   0        0        0     8817 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/validator.py
--rw-r--r--   0        0        0    16115 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/visitors.py
--rw-r--r--   0        0        0        0 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/__init__.py
--rw-r--r--   0        0        0      993 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/identifier.py
--rw-r--r--   0        0        0     2716 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/visitors.py
--rw-r--r--   0        0        0     4369 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/utils.py
--rw-r--r--   0        0        0      711 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/constraints.py
--rw-r--r--   0        0        0     1854 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/envelope.py
--rw-r--r--   0        0        0      156 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/llm.py
--rw-r--r--   0        0        0        0 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/llm_providers/__init__.py
--rw-r--r--   0        0        0      753 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/llm_providers/mock.py
--rw-r--r--   0        0        0     2388 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/llm_providers/openai.py
--rw-r--r--   0        0        0        0 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/support/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/support/github.py
--rw-r--r--   0        0        0     1547 2023-07-01 13:58:32.273700 heimdallm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7808 1970-01-01 00:00:00.000000 heimdallm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-07-04 17:56:21.955014 heimdallm-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-07-04 17:56:21.955014 heimdallm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6947 2023-07-04 17:56:21.955014 heimdallm-0.1.3/README.md
+-rw-r--r--   0        0        0       81 2023-07-04 17:56:21.955014 heimdallm-0.1.3/heimdallm/__init__.py
+-rw-r--r--   0        0        0     6288 2023-07-04 17:56:21.955014 heimdallm-0.1.3/heimdallm/bifrost.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/__init__.py
+-rw-r--r--   0        0        0     4341 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/mysql/__init__.py
+-rw-r--r--   0        0        0     3441 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/mysql/presets.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/__init__.py
+-rw-r--r--   0        0        0     3707 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/presets.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/__init__.py
+-rw-r--r--   0        0        0     4693 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
+-rw-r--r--   0        0        0     4740 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/envelope.py
+-rw-r--r--   0        0        0     1331 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2
+-rw-r--r--   0        0        0     4756 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py
+-rw-r--r--   0        0        0     6704 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark
+-rw-r--r--   0        0        0    10606 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/validator.py
+-rw-r--r--   0        0        0    16115 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/visitors.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/utils/__init__.py
+-rw-r--r--   0        0        0      993 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/utils/identifier.py
+-rw-r--r--   0        0        0     2716 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/utils/visitors.py
+-rw-r--r--   0        0        0     5684 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/bifrosts/sql/utils.py
+-rw-r--r--   0        0        0     1179 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/constraints.py
+-rw-r--r--   0        0        0     1643 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/envelope.py
+-rw-r--r--   0        0        0      734 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/llm.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/llm_providers/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/llm_providers/mock.py
+-rw-r--r--   0        0        0     2399 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/llm_providers/openai.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/support/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-04 17:56:21.959014 heimdallm-0.1.3/heimdallm/support/github.py
+-rw-r--r--   0        0        0     1564 2023-07-04 17:56:21.991015 heimdallm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 heimdallm-0.1.3/PKG-INFO
```

### Comparing `heimdallm-0.1.2/CONTRIBUTING.md` & `heimdallm-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/LICENSE` & `heimdallm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/README.md` & `heimdallm-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 # HeimdaLLM
 
 > Heimdall, the watchman of the gods, dwelt at its entrance, where he guarded Bifrost,
 > the shimmering path connecting the realms.
 
 [![Heimdall](https://raw.githubusercontent.com/amoffat/HeimdaLLM/main/docs/source/images/heimdall.png)](https://docs.heimdallm.ai)
 [![Build status](https://github.com/amoffat/HeimdaLLM/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/amoffat/HeimdaLLM/actions)
-[![Docs](https://img.shields.io/badge/Docs-purple.svg)](https://docs.heimdallm.ai)
+[![Docs](https://img.shields.io/badge/Documentation-purple.svg)](https://docs.heimdallm.ai)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/amoffat)](https://github.com/sponsors/amoffat)
 [![PyPI](https://img.shields.io/pypi/v/heimdallm)](https://pypi.org/project/heimdallm/)
 [![License: Commercial](https://img.shields.io/badge/License-Commercial-blue.svg)](https://forms.gle/frEPeeJx81Cmwva78)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Coverage Status](https://coveralls.io/repos/github/amoffat/HeimdaLLM/badge.svg?branch=dev)](https://coveralls.io/github/amoffat/HeimdaLLM?branch=dev)
 
 HeimdaLLM safely bridges the gap between untrusted human input and trusted
-machine-readable input by augmenting LLMs with a robust validation framework. It allows
-you to do things like construct trusted SQL queries from untrusted input, **using
-validation that you have full control over.**
+machine-readable input by augmenting LLMs with a robust validation framework. This
+allows you externalize LLM technology to your users, for example, to do things like
+construct trusted SQL queries from untrusted input, **using validation under your full
+control.**
 
 To accomplish this, HeimdaLLM introduces a new technology, the 🌈✨ Bifrost, composed of
 4 parts: an LLM prompt envelope, an LLM integration, a grammar, and a constraint
 validator. These 4 components operate as a single unit—a Bifrost—which is capable of
 translating untrusted human input into trusted machine input.
 
 ✨ **This allows you to perform magic** ✨
 
 Imagine giving your users natural language access to their data in your database,
 without having to worry about dangerous queries. This is an actual query on the [Sakila
 Sample
 Database](https://www.kaggle.com/datasets/atanaskanev/sqlite-sakila-sample-database):
 
 ```python
-traverse("Show me the 5 movies I rented the longest, and the number of days I had them for.")
+traverse("Show me the movies I rented the longest, and the number of days I had them for.")
 ```
 
-|     | Title           | Rental Date             | Return Date             | Rental Days |
-| --- | --------------- | ----------------------- | ----------------------- | ----------- |
-| 0   | OUTLAW HANKY    | 2005-08-19 05:48:12.000 | 2005-08-28 10:10:12.000 | 9.181944    |
-| 1   | BOULEVARD MOB   | 2005-08-19 07:06:51.000 | 2005-08-28 10:35:51.000 | 9.145139    |
-| 2   | MINDS TRUMAN    | 2005-08-02 17:42:49.000 | 2005-08-11 18:14:49.000 | 9.022222    |
-| 3   | AMERICAN CIRCUS | 2005-07-12 16:37:55.000 | 2005-07-21 16:04:55.000 | 8.977083    |
-| 4   | LADY STAGE      | 2005-07-28 10:07:04.000 | 2005-08-06 08:16:04.000 | 8.922917    |
+```
+✅ Resolving column and table aliases...
+✅ Allowlisting selectable columns...
+   ✅ Removing 4 forbidden columns...
+✅ Ensuring correct row LIMIT exists...
+   ✅ Lowering row LIMIT to 5...
+✅ Checking JOINed tables and conditions...
+✅ Checking required WHERE conditions...
+✅ Ensuring query is constrained to requester's identity...
+✅ Allowlisting SQL functions...
+```
+
+| Title           | Rental Date             | Return Date             | Rental Days |
+| --------------- | ----------------------- | ----------------------- | ----------- |
+| OUTLAW HANKY    | 2005-08-19 05:48:12.000 | 2005-08-28 10:10:12.000 | 9.181944    |
+| BOULEVARD MOB   | 2005-08-19 07:06:51.000 | 2005-08-28 10:35:51.000 | 9.145139    |
+| MINDS TRUMAN    | 2005-08-02 17:42:49.000 | 2005-08-11 18:14:49.000 | 9.022222    |
+| AMERICAN CIRCUS | 2005-07-12 16:37:55.000 | 2005-07-21 16:04:55.000 | 8.977083    |
+| LADY STAGE      | 2005-07-28 10:07:04.000 | 2005-08-06 08:16:04.000 | 8.922917    |
 
 You can safely run this example here:
 
-[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/amoffat/heimdallm/main)
+[![Open in GitHub Codespaces](https://img.shields.io/badge/Open%20in-Codespaces-purple.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=656570421)
 
 or [view the read-only notebook](./notebooks/demo.ipynb)
 
 # 📋 Explanation
 
 So, what is actually happening above?
 
@@ -59,32 +72,33 @@
 1. The LLM response is parsed by a strict grammar which defines only the SQL features
    that are allowed.
 1. If parsing succeeds, we know at the very least we're dealing with a valid SQL query
    albeit an untrusted one.
 1. Different features of the parsed query are extracted for validation.
 1. A soft validation pass is performed on the extracted features, and we potentially
    modify the query to be compliant, for example, to add a `LIMIT` clause, or to remove
-   disallowed columns. See [reconstruction](TODO).
+   disallowed columns.
 1. A hard validation pass is performed with your custom constraints to ensure that the
    query is only accessing allowed tables, columns, and functions, while containing
-   required conditions. See [validation](TODO).
+   required conditions.
 1. If validation succeeds, the resulting SQL query can then be sent to the database.
 1. If validation fails, you'll see a helpful exception explaining exactly why.
 
 # 🥽 Safety
 
 I am in the process of organizing an independent security audit of HeimdaLLM. Until this
 audit is complete, I do not recommend using HeimdaLLM against any production system
 without a careful risk assessment. These audits are self-funded, so if you will get
 value from the confidence that they bring, consider [sponsoring
 me](https://github.com/sponsors/amoffat) or [inquire about interest in a commercial
 license](https://forms.gle/frEPeeJx81Cmwva78).
 
-To understand some of the potential vulnerabilities, take a look at the [attack surface
-area](TODO) to see the risks and the mitigations.
+To understand some of the potential vulnerabilities, take a look at the [attack
+surface](https://docs.heimdallm.ai/en/latest/attack_surface.html) to see the risks and
+the mitigations.
 
 # 📚 Database support
 
 Currently, sqlite's flavor of SQL is supported. There is active development for the
 other top relational SQL databases. To help me prioritize, please vote on which database
 you would like to see supported:
```

### Comparing `heimdallm-0.1.2/heimdallm/bifrost.py` & `heimdallm-0.1.3/heimdallm/bifrost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Sequence
+from typing import Callable, Sequence
 
 import structlog
 from lark import Lark, ParseTree
 
 from heimdallm.constraints import ConstraintValidator
 from heimdallm.envelope import PromptEnvelope
 from heimdallm.llm import LLMIntegration
@@ -45,23 +45,23 @@
         self.tree_producer = tree_producer
         self.constraint_validators = constraint_validators
 
     def traverse(
         self,
         untrusted_human_input: str,
         autofix: bool = True,
-    ) -> Any:
+    ) -> str:
         """Run the full chain of the bifrost, from untrusted input to trusted
         input.
 
         :param untrusted_human_input: The untrusted input from the user.
-        :param autofix: Whether or not to attempt to reconstruct the input to satisfy
-            the constraint validator.
+        :param autofix: Whether or not to attempt to :doc:`reconstruct
+            </reconstruction>` the input to satisfy the constraint validator.
 
-        :return: The LLM output that has passed the constraint validator.
+        :return: The trusted LLM output.
         """
 
         log = LOG.bind(input=untrusted_human_input, autofix=autofix)
         log.info("Traversing untrusted input")
 
         # wrap the untrusted input in our prompt
         log.info("Wrapping input in prompt envelope")
```

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/exc.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/exc.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/mysql/presets.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/mysql/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/presets.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/bifrost.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/bifrost.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 from typing import Callable, Sequence, Union
 
 import lark
 from lark import Lark, ParseTree
 from lark.exceptions import VisitError
 
-from heimdallm.bifrost import Bifrost as _Bifrost
+from heimdallm.bifrost import Bifrost
 from heimdallm.bifrosts.sql import exc
-from heimdallm.envelope import PromptEnvelope as _PromptEnvelope
+from heimdallm.envelope import PromptEnvelope
 from heimdallm.llm import LLMIntegration
 from heimdallm.llm_providers.mock import EchoMockLLM
 
 from .envelope import TestSQLPromptEnvelope
 from .validator import SQLConstraintValidator
 from .visitors import AmbiguityResolver
 
@@ -65,16 +65,19 @@
     schema = []
     for line in conn.iterdump():
         if "CREATE TABLE" in line:
             schema.append(line)
     return "\n".join(schema)
 
 
-class SQLBifrost(_Bifrost):
-    """A Bifrost for traversing SQL ``SELECT`` queries."""
+class SQLBifrost(Bifrost):
+    """A Bifrost for traversing SQL ``SELECT`` queries.
+
+    :vartype value: str
+    """
 
     # for tests
     @classmethod
     def mocked(
         cls,
         constraint_validators: Union[
             SQLConstraintValidator, Sequence[SQLConstraintValidator]
@@ -82,14 +85,16 @@
     ):
         """A convenience method for our tests. This creates a Bifrost that assumes its
         untrusted input is a SQL query already, so it does not need to communicate with
         the LLM, only parse and validate it.
 
         :param constraint_validators: A constraint validator or sequence of constraint
             validators to run on the untrusted input.
+
+        :meta private:
         """
         if not isinstance(constraint_validators, Sequence):
             constraint_validators = [constraint_validators]
 
         llm = EchoMockLLM()
         return cls(
             llm=llm,
@@ -101,15 +106,15 @@
             ),
         )
 
     def __init__(
         self,
         *,
         llm: LLMIntegration,
-        prompt_envelope: _PromptEnvelope,
+        prompt_envelope: PromptEnvelope,
         constraint_validators: Sequence[SQLConstraintValidator],
     ):
         super().__init__(
             llm=llm,
             prompt_envelope=prompt_envelope,
             grammar=_build_grammar(),
             tree_producer=_build_tree_producer(),
@@ -118,14 +123,18 @@
 
     def parse(self, untrusted_llm_output: str) -> ParseTree:
         """Parse the unwrapped SQL query from the LLM's output. Raise a SQL-specific
         exception if the query is not valid.
 
         :param untrusted_llm_output: The output from the LLM, which should be a SQL
             query. If it isn't, then our :meth:`SQLPromptEnvelope.unwrap` method failed.
+        :raises InvalidQuery: If the query is not valid.
+        :return: The Lark parse tree for the query.
+
+        :meta private:
         """
         try:
             return super().parse(untrusted_llm_output)
         except lark.exceptions.UnexpectedEOF as e:
             raise exc.InvalidQuery(query=untrusted_llm_output) from e
         except lark.exceptions.UnexpectedCharacters as e:
             raise exc.InvalidQuery(query=untrusted_llm_output) from e
```

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/envelope.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/validator.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/validator.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,90 +13,137 @@
 from .. import presets
 from ..utils.visitors import AliasCollector
 from .visitors import FacetCollector, Facets
 
 
 class SQLConstraintValidator(_ConstraintValidator):
     """
-    Validate different aspects of a SQL query. You are intended to derive this class and
-    implement methods."""
+    This validator checks different of a SQL query. You are intended to derive this
+    class and implement its methods."""
 
     @abstractmethod
     def requester_identities(self) -> Sequence[RequiredConstraint]:
-        """Returns the identity of the requester, as represented in the
-        database. this is used to instruct the LLM how to constrain the query
-        that it generates. only one of these identities needs to match.
-
-        the reason that we return a sequence, and not a single identity, is that
-        sometimes an LLM will specify the constraint as part of a ``JOIN``
-        condition, and not a ``WHERE`` condition. in that case, the column in the
-        JOIN condition may not match the column you expect, for example,
+        """Returns the possible identities of the requester, as represented in the
+        database. This is used to instruct the LLM how to constrain the query that it
+        generates. Only one of these identities needs to match for the query to be
+        compliant.
+
+        The reason that we return a sequence, and not a single identity, is that
+        sometimes an LLM will specify the constraint as part of a ``JOIN`` condition,
+        and not a ``WHERE`` condition. In that case, the column in the JOIN condition
+        may not match the column you expect.
+
+        For example, consider selecting films for a customer, constrained by the
+        customer id. The LLM may give you a query like this:
+
+        .. code-block:: sql
+
+            SELECT f.title
+            FROM film f
+            JOIN inventory i ON f.film_id=i.film_id
+            JOIN rental r ON i.inventory_id=r.inventory_id
+            JOIN customer c ON r.customer_id=c.customer_id
+            WHERE c.customer_id=:customer_id
+
+        Or you may receive a query like this:
+
+        .. code-block:: sql
+
+            SELECT f.title
+            FROM film f
+            JOIN inventory i ON f.film_id=i.film_id
+            JOIN rental r
+                ON i.inventory_id=r.inventory_id
+                AND r.customer_id=:customer_id
+
+        Both ``rental.customer_id`` and ``customer.customer_id`` are valid requester
+        identities, so ou need to specify both of them by returning a
+        :class:`RequiredConstraint` for each of them.
 
-            Invoice.CustomerId vs Customer.CustomerId
-
-        although they represent the same identity, they are different tables and
-        columns, but constraining on one of them is sufficient.
+        :return: The sequence of possible requester identities.
         """
         raise NotImplementedError(
             "You must explicitly provide the requester identity, "
             "or an empty list for full access (dangerous)"
         )
 
     @abstractmethod
     def required_constraints(self) -> Sequence[RequiredConstraint]:
-        """Returns a sequence of secure constraints that must exist in the ``WHERE``
-        clause of the query"""
+        """Returns a sequence of secure constraints that must exist in either the
+        ``WHERE`` clause of the query or in a ``JOIN`` condition. It doesn't matter
+        where the constraint is, as long as it exists and is required (i.e. not part of
+        an optional condition).
+
+        :return: The sequence of required constraints.
+        """
         raise NotImplementedError(
             "You must explicitly provide a sequence of required constraints, "
             "or an empty list for no constraints"
         )
 
     @abstractmethod
     def select_column_allowed(self, column: FqColumn) -> bool:
-        """Ensures that the column is allowed to be selected in the ``SELECT`` clause"""
+        """Check that a fully-qualified column is allowed to be selected in the
+        ``SELECT`` clause. Use this to restrict the columns and tables that can be
+        selected.
+
+        This value is also used to inform :doc:`/reconstruction`. Columns that do not
+        pass this check will be removed from the query.
+
+        :param column: The fully-qualified column.
+        :return: Whether or not the column is allowed to be selected.
+        """
         return False
 
     @abstractmethod
     def allowed_joins(self) -> Sequence[JoinCondition]:
-        """Returns all of the tables allowed to be connected to the query,
-        either via a ``JOIN``, or via a ``FROM``. this encompasses both cases because
-        LLMs frequently produce queries that select unpredictable tables with
-        ``FROM``, even if that table is valid to be connected via ``JOIN``. so to
-        handle this, we consider a table selected with ``FROM`` as a ``JOIN`` with no
-        explicit conditions. in practice, if there are other joins in the query,
-        the selected table will have an explicit condition via the ON clause. if
-        there are no other joins, the selected table will have no join
-        conditions.
+        """Returns all of the tables allowed to be connected to the query via a
+        ``JOIN`` and the equi-join conditions that must be met for the join to be valid.
+
+        :return: The sequence of allowed joins.
         """
         return []
 
     @abstractmethod
     def max_limit(self) -> Optional[int]:
         """Return the maximum number of rows that can be returned by a query. if
-        None, there is no limit."""
+        None, there is no limit.
+
+        This value is also used to inform :doc:`/reconstruction`. If this function
+        provides a limit, but the query does not, or the query provides a higher limit,
+        the query will be reconstructed to include the correct limit.
+
+        :return: The maximum number of rows that can be returned by a query, or None if
+            unlimited.
+        """
         return None
 
     def can_use_function(self, function: str) -> bool:
-        """Ensures that the function is allowed to be used in the query
+        """Returns whether or not a SQL function is allowed to be used anywhere in the
+        query.
 
-        :param function: the name of the function
+        :param function: The *lowercase* name of the function.
+        :return: Whether or not the function is allowed.
         """
         return function in presets.safe_functions
 
     def condition_column_allowed(self, fq_column: FqColumn) -> bool:
         """Checks if a column is allowed in a ``WHERE``, ``JOIN``, ``HAVING``, or
         ``ORDER BY``"""
         # let's default to "if you can see it, you can use it"
         return self.select_column_allowed(fq_column)
 
     def fix(self, grammar: Lark, tree: ParseTree) -> str:
         """A parse tree may be valid SQL, but it may not be valid according to
         the validator's constraints. we may be able to make intelligent
         decisions about those constraints, and fix the parse tree though, for
-        example, by adding a limit to a query."""
+        example, by adding a limit to a query.
+
+        :meta private:
+        """
 
         # gets around a circular import issue
         from heimdallm.bifrosts.sql.sqlite.select import reconstruct
 
         transform = reconstruct.ReconstructTransformer(self)
         try:
             fixed_tree = transform.transform(tree)
@@ -108,15 +155,22 @@
         output = Reconstructor(grammar).reconstruct(
             fixed_tree,
             postproc=reconstruct.postproc,
         )
         return output
 
     def validate(self, untrusted_input: str, tree: ParseTree):
-        """Analyze the tree and validate it against our SQL constraints"""
+        """Analyze the parsed tree and validate it against our SQL constraints
+
+        :param untrusted_input: The original query string. This is passed in so that if
+            we need to raise an exception that references it, we can.
+        :param tree: The parsed tree from the original query string.
+
+        :meta private:
+        """
         try:
             alias_collector = AliasCollector()
             alias_collector.visit(tree)
 
             facets = Facets()
             facet_collector = FacetCollector(facets, alias_collector)
             facet_collector.visit(tree)
```

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/visitors.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/select/visitors.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/identifier.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/visitors.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/sqlite/utils/visitors.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.2/heimdallm/bifrosts/sql/utils.py` & `heimdallm-0.1.3/heimdallm/bifrosts/sql/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from typing import Any, Optional, Sequence
 
 from . import exc
 
 
 class RequiredConstraint:
-    """represents a constraint that must be applied to the query. in the query,
-    this comes in the form of "table.column=:placeholder". enforced by the
-    grammar, the comparison is always equality, the left hand side is always a
-    fully-qualified column, and the right hand side is always a placeholder.
-    this requirements ensure that the query is always constrained by a value
-    that the developer specifies at query execution time."""
+    """This represents a constraint that *must* be applied to the query.
+
+    In the query, this comes in the form of ``table.column=:placeholder``. enforced by
+    the grammar, the comparison is always equality, the left hand side is always a
+    fully-qualified column, and the right hand side is always a placeholder. this
+    requirements ensure that the query is always constrained by a value that the
+    developer specifies at query execution time.
+
+    :param column: The fully-qualified column name.
+    :param placeholder: The placeholder name for the value that your database expects to
+        be interpolated at execution time.
+    """
 
     def __init__(self, *, column: str, placeholder: str):
         self.fq_column = FqColumn.from_string(column)
         self.placeholder = placeholder
 
     def __eq__(self, other: Any) -> bool:
         return (
@@ -28,37 +34,52 @@
     def __str__(self):
         return f"{self.fq_column}=:{self.placeholder}"
 
     __repr__ = __str__
 
 
 class FqColumn:
-    """represents a fully-qualified column name. we require that LLM-produced
-    queries use fully-qualified columns in their SELECT and WHERE clauses,
-    otherwise we would need to infer which table owned the column, which
-    requires runtime database analysis. much easier to require the LLM give us
-    fully-qualified names"""
+    """This represents a fully-qualified column name.
+
+    We require that LLM-produced queries from SQL Bifrosts use fully-qualified columns
+    in their clauses, because if they didn't, we would need to infer which table owned
+    the column, which requires runtime schema analysis. We could do that, but maybe in
+    the future. It's much more straightforward to require the LLM give us
+    fully-qualified names.
+
+    :param table: The table name.
+    :param column: The column name.
+    """
 
     __slots__ = ("table", "column")
 
     @classmethod
-    def from_string(cls, s: str):
-        if "." not in s:
-            raise exc.UnqualifiedColumn(s)
-        table, column = s.split(".")
+    def from_string(cls, fq_column_name: str) -> "FqColumn":
+        """Parses a fully-qualified column name from a string, using the expected
+        format of ``table.column``
+
+        :param fq_column_name: The fully-qualified column name.
+        :raises UnqualifiedColumn: If the string does not contain a period."""
+        if "." not in fq_column_name:
+            raise exc.UnqualifiedColumn(fq_column_name)
+        table, column = fq_column_name.split(".")
         return cls(table=table, column=column)
 
     def __init__(self, *, table: str, column: str):
         self.table = table
         self.column = column
 
     def __str__(self):
         return f"{self.table}.{self.column}"
 
-    name = property(str)
+    @property
+    def name(self) -> str:
+        """A convenience property that returns the fully-qualified column name as a
+        string in the same format ``table.column``"""
+        return str(self)
 
     def __iter__(self):
         return iter((self.table, self.column))
 
     def __hash__(self):
         return hash((self.table, self.column))
 
@@ -66,33 +87,42 @@
         return self.table == other.table and self.column == other.column
 
     def __repr__(self):
         return f"{self.table}.{self.column}"
 
 
 class JoinCondition:
-    """represents an equi-join between two tables. for our hash and equality
-    functions, we don't care about the order of the join condition"""
+    """This represents an equi-join between two tables, on two columns. The order of
+    the fully-qualified columns does not matter; matching will work correctly in the
+    code.
+
+    :param first: The first fully-qualified column.
+    :param second: The second fully-qualified column.
+    :param identity: If the columns specified in this join condition can also be used as
+        a :meth:`requester identity
+        <heimdallm.bifrosts.sql.sqlite.select.validator.SQLConstraintValidator.requester_identities>`
+        for the query, then this should be set to the name of the placeholder where the
+        identity will be populated at runtime.
+    """
 
     __slots__ = ("first", "second", "identity_placeholder")
 
     def __init__(self, first: str, second: str, *, identity: Optional[str] = None):
-        """if identity is True, then either column in the join condition is a
-        valid requester identity. this means it can be used to constrain the
-        query in the same way SQLConstraintValidator.requester_identities
-        does."""
         self.first = FqColumn.from_string(first)
         self.second = FqColumn.from_string(second)
         self.identity_placeholder = identity
 
     @property
     def requester_identities(self) -> Sequence[RequiredConstraint]:
-        """if this join condition has been marked as an identity join,
-        construct the required constraints for both sides of the join. we'll use
-        those constraints when testing for the requester's identity"""
+        """If this join condition has been marked as an identity join,
+        construct the required constraints for both sides of the join. We'll use those
+        constraints when testing for the requester's identity.
+
+        :meta private:
+        """
         if self.identity_placeholder:
             return [
                 RequiredConstraint(
                     column=self.first.name,
                     placeholder=self.identity_placeholder,
                 ),
                 RequiredConstraint(
@@ -116,14 +146,16 @@
     def __str__(self) -> str:
         return f"{self.first}={self.second}"
 
     __repr__ = __str__
 
 
 class _AnyJoinCondition(JoinCondition):
-    """a convenience class for representing any valid join condition."""
+    """A convenience class for representing any valid join condition."""
 
     def __init__(self):
         super().__init__("*.*", "*.*")
 
 
+#: A convenience object that represents any valid join condition. Only use it for a
+#: validator that represents full admin access to your database.
 ANY_JOIN = _AnyJoinCondition()
```

### Comparing `heimdallm-0.1.2/heimdallm/constraints.py` & `heimdallm-0.1.3/heimdallm/constraints.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 
 from lark import Lark, ParseTree
 
 
 class ConstraintValidator(ABC):
     @abstractmethod
     def fix(self, Grammar: Lark, tree: ParseTree) -> str:
-        """if the tree does not pass the constraints, attempt to reconstruct it
-        to satisfy the constraints. if the tree cannot be reconstructed, throw a
-        bifrost-specific exception"""
-        pass
+        """If the tree fails validation in a soft-pass, attempt to reconstruct it
+        to satisfy the constraints. If the tree cannot be reconstructed, throw a
+        bifrost-specific exception
+
+        :param Grammar: The Lark grammar used to parse the untrusted input. This is
+            often used by :class:`lark.reconstruct.Reconstructor` to fix the parse tree.
+        :param tree: The resulting parse tree of the untrusted input.
+        """
+        raise NotImplementedError
 
     @abstractmethod
     def validate(self, untrusted_input: str, tree: ParseTree):
-        """throws a bifrost-specific exception if the tree does not pass the
-        constraints. the untrusted_input is provided for context if we need to raise
-        an exception that contains the original input."""
-        pass
+        """This performs the Bifrost-specific validation of the parse tree. It throws a
+        Bifrost-specific exception if the tree does not pass the constraints.
+
+        :param untrusted_input: The untrusted input, which can be used to provide extra
+            context if we need to raise an exception.
+        :param tree: The resulting parse tree of the untrusted input.
+        """
+        raise NotImplementedError
```

### Comparing `heimdallm-0.1.2/heimdallm/envelope.py` & `heimdallm-0.1.3/heimdallm/envelope.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from heimdallm.llm import LLMIntegration
 
 
 class PromptEnvelope(ABC):
     """
     The purpose of the prompt envelope is to guide the wrapped untrusted query to
-    produce the structured output. Itt is impossible to prevent prompt injection, so
+    produce the structured output. It is impossible to prevent prompt injection, so
     accept that up front. However, a malicious prompt will not produce a valid response,
     so our grammar will not parse it, and the validator will not validate it, so the
     malicious user will never see the result of their malicious output.
 
     :param llm: The LLM integration being sent the human input. This is passed in so
         that the envelope can change the way it wraps or unwraps data communicated with
         the LLM, based on different quirks of the LLM.
@@ -22,26 +22,18 @@
     @abstractmethod
     def wrap(self, untrusted_input: str) -> str:
         """Wrap the untrusted input with additional context to guide the LLM to produce
         the correct output.
 
         :param untrusted_input: The untrusted input from the user.
         :return: The wrapped input to send to the LLM."""
-        return untrusted_input
+        raise NotImplementedError
 
     @abstractmethod
     def unwrap(self, untrusted_llm_output: str) -> str:
         """Unwrap the LLM's output to produce the original untrusted input. This method
         should work closely with the wrap method to coordinate how to delimit the
         structured response.
 
         :param untrusted_llm_output: The untrusted output from the LLM.
         :return: The structured response, unwrapped from the LLM's output."""
-        return untrusted_llm_output
-
-
-class NoOpEnvelope(PromptEnvelope):
-    def wrap(self, untrusted_input: str) -> str:
-        return untrusted_input
-
-    def unwrap(self, untrusted_llm_output: str) -> str:
-        return untrusted_llm_output
+        raise NotImplementedError
```

### Comparing `heimdallm-0.1.2/heimdallm/llm_providers/mock.py` & `heimdallm-0.1.3/heimdallm/llm_providers/mock.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import hashlib
 from typing import Dict
 
 from ..llm import LLMIntegration
 
 
-class LookupMockLLM(LLMIntegration):
+class LookupMockLLM(LLMIntegration):  # pragma: no cover
     """a mock LLM integration that simply returns a canned response for the
     hash of some input"""
 
     def __init__(self) -> None:
         self.responses: Dict[str, str] = {}
 
     def complete(self, untrusted_user_input: str) -> str:
         hash_id = hashlib.md5(untrusted_user_input.encode("utf8")).hexdigest()
         return self.responses[hash_id]
 
 
-class EchoMockLLM(LLMIntegration):
+class EchoMockLLM(LLMIntegration):  # pragma: no cover
     """a mock LLM integration that simply returns the provided response. useful
     in our tests where we know the query that we want to attempt to parse +
     validate."""
 
     def complete(self, sql_output: str) -> str:
         return sql_output
```

### Comparing `heimdallm-0.1.2/heimdallm/llm_providers/openai.py` & `heimdallm-0.1.3/heimdallm/llm_providers/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         the prompt envelopes can make the LLM input quite long.
     :param method: The method to use to interact with the OpenAI API. I don't really
         know the difference in terms of quality, but the chat method has worked fine so
         far."""
 
     def __init__(
         self,
+        *,
         api_key: str,
         model: str = "gpt-3.5-turbo-16k",
         method: OpenAIMethod = OpenAIMethod.CHAT,
     ):
         self.api_key = api_key
         self.model = model
         self.method = method
```

### Comparing `heimdallm-0.1.2/heimdallm/support/github.py` & `heimdallm-0.1.3/heimdallm/support/github.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from urllib.parse import quote
 
 
 def _dict_to_qs(params):
     """Converts a dict to a query string, with values url-encoded"""
     qs = []
     for k, v in params.items():
-        if isinstance(v, list):
-            for i in v:
-                qs.append(f"{quote(k)}={quote(str(i))}")
-        else:
-            qs.append(f"{quote(k)}={quote(str(v))}")
+        qs.append(f"{quote(k)}={quote(str(v))}")
     return "&".join(qs)
 
 
 def make_issue_link(*, title: str, body: str, labels: list[str] = []) -> str:
     """Makes a generic GH issue"""
     url = "https://github.com/amoffat/HeimdaLLM/issues/new"
     params = {
```

### Comparing `heimdallm-0.1.2/pyproject.toml` & `heimdallm-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heimdallm"
-version = "0.1.2"
+version = "0.1.3"
 description = "Construct trusted SQL queries from untrusted input"
 homepage = "https://github.com/amoffat/HeimdaLLM"
 repository = "https://github.com/amoffat/HeimdaLLM"
 documentation = "https://heimdallm.readthedocs.io/en/latest/"
 authors = ["Andrew Moffat <arwmoffat@gmail.com>"]
 maintainers = ["Andrew Moffat <arwmoffat@gmail.com>"]
 keywords = ["sql", "llm", "ai"]
@@ -48,11 +48,12 @@
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 ipykernel = "^6.23.3"
 sphinx = ">=1.6,<7"
 sphinx-rtd-theme = "^1.2.2"
 toml = "^0.10.2"
 types-toml = "^0.10.8.6"
+munch = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `heimdallm-0.1.2/PKG-INFO` & `heimdallm-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heimdallm
-Version: 0.1.2
+Version: 0.1.3
 Summary: Construct trusted SQL queries from untrusted input
 Home-page: https://github.com/amoffat/HeimdaLLM
 License: AGPL-3.0
 Keywords: sql,llm,ai
 Author: Andrew Moffat
 Author-email: arwmoffat@gmail.com
 Maintainer: Andrew Moffat
@@ -32,53 +32,66 @@
 # HeimdaLLM
 
 > Heimdall, the watchman of the gods, dwelt at its entrance, where he guarded Bifrost,
 > the shimmering path connecting the realms.
 
 [![Heimdall](https://raw.githubusercontent.com/amoffat/HeimdaLLM/main/docs/source/images/heimdall.png)](https://docs.heimdallm.ai)
 [![Build status](https://github.com/amoffat/HeimdaLLM/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/amoffat/HeimdaLLM/actions)
-[![Docs](https://img.shields.io/badge/Docs-purple.svg)](https://docs.heimdallm.ai)
+[![Docs](https://img.shields.io/badge/Documentation-purple.svg)](https://docs.heimdallm.ai)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/amoffat)](https://github.com/sponsors/amoffat)
 [![PyPI](https://img.shields.io/pypi/v/heimdallm)](https://pypi.org/project/heimdallm/)
 [![License: Commercial](https://img.shields.io/badge/License-Commercial-blue.svg)](https://forms.gle/frEPeeJx81Cmwva78)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Coverage Status](https://coveralls.io/repos/github/amoffat/HeimdaLLM/badge.svg?branch=dev)](https://coveralls.io/github/amoffat/HeimdaLLM?branch=dev)
 
 HeimdaLLM safely bridges the gap between untrusted human input and trusted
-machine-readable input by augmenting LLMs with a robust validation framework. It allows
-you to do things like construct trusted SQL queries from untrusted input, **using
-validation that you have full control over.**
+machine-readable input by augmenting LLMs with a robust validation framework. This
+allows you externalize LLM technology to your users, for example, to do things like
+construct trusted SQL queries from untrusted input, **using validation under your full
+control.**
 
 To accomplish this, HeimdaLLM introduces a new technology, the 🌈✨ Bifrost, composed of
 4 parts: an LLM prompt envelope, an LLM integration, a grammar, and a constraint
 validator. These 4 components operate as a single unit—a Bifrost—which is capable of
 translating untrusted human input into trusted machine input.
 
 ✨ **This allows you to perform magic** ✨
 
 Imagine giving your users natural language access to their data in your database,
 without having to worry about dangerous queries. This is an actual query on the [Sakila
 Sample
 Database](https://www.kaggle.com/datasets/atanaskanev/sqlite-sakila-sample-database):
 
 ```python
-traverse("Show me the 5 movies I rented the longest, and the number of days I had them for.")
+traverse("Show me the movies I rented the longest, and the number of days I had them for.")
 ```
 
-|     | Title           | Rental Date             | Return Date             | Rental Days |
-| --- | --------------- | ----------------------- | ----------------------- | ----------- |
-| 0   | OUTLAW HANKY    | 2005-08-19 05:48:12.000 | 2005-08-28 10:10:12.000 | 9.181944    |
-| 1   | BOULEVARD MOB   | 2005-08-19 07:06:51.000 | 2005-08-28 10:35:51.000 | 9.145139    |
-| 2   | MINDS TRUMAN    | 2005-08-02 17:42:49.000 | 2005-08-11 18:14:49.000 | 9.022222    |
-| 3   | AMERICAN CIRCUS | 2005-07-12 16:37:55.000 | 2005-07-21 16:04:55.000 | 8.977083    |
-| 4   | LADY STAGE      | 2005-07-28 10:07:04.000 | 2005-08-06 08:16:04.000 | 8.922917    |
+```
+✅ Resolving column and table aliases...
+✅ Allowlisting selectable columns...
+   ✅ Removing 4 forbidden columns...
+✅ Ensuring correct row LIMIT exists...
+   ✅ Lowering row LIMIT to 5...
+✅ Checking JOINed tables and conditions...
+✅ Checking required WHERE conditions...
+✅ Ensuring query is constrained to requester's identity...
+✅ Allowlisting SQL functions...
+```
+
+| Title           | Rental Date             | Return Date             | Rental Days |
+| --------------- | ----------------------- | ----------------------- | ----------- |
+| OUTLAW HANKY    | 2005-08-19 05:48:12.000 | 2005-08-28 10:10:12.000 | 9.181944    |
+| BOULEVARD MOB   | 2005-08-19 07:06:51.000 | 2005-08-28 10:35:51.000 | 9.145139    |
+| MINDS TRUMAN    | 2005-08-02 17:42:49.000 | 2005-08-11 18:14:49.000 | 9.022222    |
+| AMERICAN CIRCUS | 2005-07-12 16:37:55.000 | 2005-07-21 16:04:55.000 | 8.977083    |
+| LADY STAGE      | 2005-07-28 10:07:04.000 | 2005-08-06 08:16:04.000 | 8.922917    |
 
 You can safely run this example here:
 
-[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/amoffat/heimdallm/main)
+[![Open in GitHub Codespaces](https://img.shields.io/badge/Open%20in-Codespaces-purple.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=656570421)
 
 or [view the read-only notebook](./notebooks/demo.ipynb)
 
 # 📋 Explanation
 
 So, what is actually happening above?
 
@@ -90,32 +103,33 @@
 1. The LLM response is parsed by a strict grammar which defines only the SQL features
    that are allowed.
 1. If parsing succeeds, we know at the very least we're dealing with a valid SQL query
    albeit an untrusted one.
 1. Different features of the parsed query are extracted for validation.
 1. A soft validation pass is performed on the extracted features, and we potentially
    modify the query to be compliant, for example, to add a `LIMIT` clause, or to remove
-   disallowed columns. See [reconstruction](TODO).
+   disallowed columns.
 1. A hard validation pass is performed with your custom constraints to ensure that the
    query is only accessing allowed tables, columns, and functions, while containing
-   required conditions. See [validation](TODO).
+   required conditions.
 1. If validation succeeds, the resulting SQL query can then be sent to the database.
 1. If validation fails, you'll see a helpful exception explaining exactly why.
 
 # 🥽 Safety
 
 I am in the process of organizing an independent security audit of HeimdaLLM. Until this
 audit is complete, I do not recommend using HeimdaLLM against any production system
 without a careful risk assessment. These audits are self-funded, so if you will get
 value from the confidence that they bring, consider [sponsoring
 me](https://github.com/sponsors/amoffat) or [inquire about interest in a commercial
 license](https://forms.gle/frEPeeJx81Cmwva78).
 
-To understand some of the potential vulnerabilities, take a look at the [attack surface
-area](TODO) to see the risks and the mitigations.
+To understand some of the potential vulnerabilities, take a look at the [attack
+surface](https://docs.heimdallm.ai/en/latest/attack_surface.html) to see the risks and
+the mitigations.
 
 # 📚 Database support
 
 Currently, sqlite's flavor of SQL is supported. There is active development for the
 other top relational SQL databases. To help me prioritize, please vote on which database
 you would like to see supported:
```

