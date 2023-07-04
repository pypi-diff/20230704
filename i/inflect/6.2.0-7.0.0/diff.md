# Comparing `tmp/inflect-6.2.0.tar.gz` & `tmp/inflect-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inflect-6.2.0.tar", last modified: Mon Jul  3 18:53:02 2023, max compression
+gzip compressed data, was "inflect-7.0.0.tar", last modified: Tue Jul  4 14:16:51 2023, max compression
```

## Comparing `inflect-6.2.0.tar` & `inflect-7.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.198320 inflect-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 18:52:38.000000 inflect-6.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 18:52:38.000000 inflect-6.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.190320 inflect-6.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 18:52:38.000000 inflect-6.2.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 18:52:38.000000 inflect-6.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.190320 inflect-6.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-03 18:52:38.000000 inflect-6.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 18:52:38.000000 inflect-6.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 18:52:38.000000 inflect-6.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 18:52:38.000000 inflect-6.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 18:52:38.000000 inflect-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-03 18:52:38.000000 inflect-6.2.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-03 18:53:02.198320 inflect-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-07-03 18:52:38.000000 inflect-6.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.190320 inflect-6.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 18:52:38.000000 inflect-6.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-03 18:52:38.000000 inflect-6.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 18:52:38.000000 inflect-6.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.190320 inflect-6.2.0/inflect/
--rw-r--r--   0 runner    (1001) docker     (123)   103758 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.198320 inflect-6.2.0/inflect/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/compat/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/compat/pydantic1.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.194320 inflect-6.2.0/inflect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 18:52:38.000000 inflect-6.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-03 18:52:38.000000 inflect-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 18:52:38.000000 inflect-6.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-03 18:53:02.198320 inflect-6.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.198320 inflect-6.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/inflections.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_an.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_ancient.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_herd.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_person.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_compounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_inflections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_numwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_pl_si.py
--rw-r--r--   0 runner    (1001) docker     (123)    46096 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_unicode.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 18:52:38.000000 inflect-6.2.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-03 18:52:38.000000 inflect-6.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:51.694981 inflect-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 14:16:29.000000 inflect-7.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 14:16:29.000000 inflect-7.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:51.678981 inflect-7.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 14:16:29.000000 inflect-7.0.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 14:16:29.000000 inflect-7.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:51.678981 inflect-7.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-04 14:16:29.000000 inflect-7.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-04 14:16:29.000000 inflect-7.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 14:16:29.000000 inflect-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 14:16:29.000000 inflect-7.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-04 14:16:29.000000 inflect-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-07-04 14:16:29.000000 inflect-7.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-04 14:16:51.694981 inflect-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-07-04 14:16:29.000000 inflect-7.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:51.678981 inflect-7.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-04 14:16:29.000000 inflect-7.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 14:16:29.000000 inflect-7.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 14:16:29.000000 inflect-7.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:51.682981 inflect-7.0.0/inflect/
+-rw-r--r--   0 runner    (1001) docker     (123)   102919 2023-07-04 14:16:29.000000 inflect-7.0.0/inflect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:51.686981 inflect-7.0.0/inflect/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:29.000000 inflect-7.0.0/inflect/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 14:16:29.000000 inflect-7.0.0/inflect/compat/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-04 14:16:29.000000 inflect-7.0.0/inflect/compat/pydantic1.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:29.000000 inflect-7.0.0/inflect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:51.682981 inflect-7.0.0/inflect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-04 14:16:51.000000 inflect-7.0.0/inflect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-04 14:16:51.000000 inflect-7.0.0/inflect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:16:51.000000 inflect-7.0.0/inflect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 14:16:51.000000 inflect-7.0.0/inflect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 14:16:51.000000 inflect-7.0.0/inflect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 14:16:29.000000 inflect-7.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-04 14:16:29.000000 inflect-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-04 14:16:29.000000 inflect-7.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-04 14:16:51.694981 inflect-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:16:51.694981 inflect-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/inflections.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_an.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_classical_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_classical_ancient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_classical_herd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_classical_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_classical_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_classical_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_compounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_inflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_numwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_pl_si.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42514 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-04 14:16:29.000000 inflect-7.0.0/tests/test_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 14:16:29.000000 inflect-7.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-04 14:16:29.000000 inflect-7.0.0/tox.ini
```

### Comparing `inflect-6.2.0/.github/workflows/main.yml` & `inflect-7.0.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/LICENSE` & `inflect-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/NEWS.rst` & `inflect-7.0.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v7.0.0
+======
+
+Features
+--------
+
+- Refine type hint for ``singular_noun`` to indicate a literal return type for ``False``. (#186)
+
+
+Deprecations and Removals
+-------------------------
+
+- Removed methods renamed in 0.2.0.
+
+
 v6.2.0
 ======
 
 Features
 --------
 
 - Project now supports Pydantic 2 while retaining support for Pydantic 1. (#187)
```

### Comparing `inflect-6.2.0/PKG-INFO` & `inflect-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 6.2.0
+Version: 7.0.0
 Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
 Home-page: https://github.com/jaraco/inflect
 Author: Paul Dyson
 Author-email: pwdyson@yahoo.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inflect-6.2.0/README.rst` & `inflect-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/docs/conf.py` & `inflect-7.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/inflect/__init__.py` & `inflect-7.0.0/inflect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """
 inflect: english language inflection
  - correctly generate plurals, ordinals, indefinite articles
  - convert numbers to words
 
-Copyright (C) 2010 Paul Dyson
-
 Based upon the Perl module
 `Lingua::EN::Inflect <https://metacpan.org/pod/Lingua::EN::Inflect>`_.
 
 methods:
     classical inflect
     plural plural_noun plural_verb plural_adj singular_noun no num a an
     compare compare_nouns compare_verbs compare_adjs
@@ -66,14 +64,15 @@
     Match,
     Tuple,
     Callable,
     Sequence,
     cast,
     Any,
 )
+from typing_extensions import Literal
 from numbers import Number
 
 
 from pydantic import Field
 from typing_extensions import Annotated
 
 
@@ -105,22 +104,14 @@
     pass
 
 
 class BadGenderError(Exception):
     pass
 
 
-STDOUT_ON = False
-
-
-def print3(txt: str) -> None:
-    if STDOUT_ON:
-        print(txt)
-
-
 def enclose(s: str) -> str:
     return f"(?:{s})"
 
 
 def joinstem(cutpoint: Optional[int] = 0, words: Optional[Iterable[str]] = None) -> str:
     """
     Join stem of each word in words into a string for regex.
@@ -2050,35 +2041,14 @@
     def _number_args(self):
         return cast(Dict[str, str], self.__number_args)
 
     @_number_args.setter
     def _number_args(self, val):
         self.__number_args = val
 
-    deprecated_methods = dict(
-        pl="plural",
-        plnoun="plural_noun",
-        plverb="plural_verb",
-        pladj="plural_adj",
-        sinoun="single_noun",
-        prespart="present_participle",
-        numwords="number_to_words",
-        plequal="compare",
-        plnounequal="compare_nouns",
-        plverbequal="compare_verbs",
-        pladjequal="compare_adjs",
-        wordlist="join",
-    )
-
-    def __getattr__(self, meth):
-        if meth in self.deprecated_methods:
-            print3(f"{meth}() deprecated, use {self.deprecated_methods[meth]}()")
-            raise DeprecationWarning
-        raise AttributeError
-
     @validate_call
     def defnoun(self, singular: Optional[Word], plural: Optional[Word]) -> int:
         """
         Set the noun plural of singular to plural.
 
         """
         self.checkpat(singular)
@@ -2148,16 +2118,15 @@
         check for errors in a regex pattern
         """
         if pattern is None:
             return
         try:
             re.match(pattern, "")
         except re.error:
-            print3(f"\nBad user-defined singular pattern:\n\t{pattern}\n")
-            raise BadUserDefinedPatternError
+            raise BadUserDefinedPatternError(pattern)
 
     def checkpatplural(self, pattern: Optional[Word]) -> None:
         """
         check for errors in a regex replace pattern
         """
         return
 
@@ -2549,15 +2518,15 @@
 
     @validate_call
     def singular_noun(
         self,
         text: Word,
         count: Optional[Union[int, str, Any]] = None,
         gender: Optional[str] = None,
-    ) -> Union[str, bool]:
+    ) -> Union[str, Literal[False]]:
         """
         Return the singular of text, where text is a plural noun.
 
         If count supplied, then return the singular if count is one of:
             1, a, an, one, each, every, this, that or if count is None
 
         otherwise return text unchanged.
@@ -3256,19 +3225,19 @@
         except KeyError:
             pass
 
         # HANDLE ISOLATED IRREGULAR PLURALS
 
         if words.last in si_sb_irregular_caps:
             llen = len(words.last)
-            return "{}{}".format(word[:-llen], si_sb_irregular_caps[words.last])
+            return f"{word[:-llen]}{si_sb_irregular_caps[words.last]}"
 
         if words.last.lower() in si_sb_irregular:
             llen = len(words.last.lower())
-            return "{}{}".format(word[:-llen], si_sb_irregular[words.last.lower()])
+            return f"{word[:-llen]}{si_sb_irregular[words.last.lower()]}"
 
         dash_split = words.lowered.split("-")
         if (" ".join(dash_split[-2:])).lower() in si_sb_irregular_compound:
             llen = len(
                 " ".join(dash_split[-2:])
             )  # TODO: what if 2 spaces between these words?
             return "{}{}".format(
@@ -3659,15 +3628,14 @@
                 rval = ordinal_suff.sub(post, str_num)
             else:
                 rval = f"{str_num}th"
             return rval
 
     def millfn(self, ind: int = 0) -> str:
         if ind > len(mill) - 1:
-            print3("number out of range")
             raise NumOutOfRangeError
         return mill[ind]
 
     def unitfn(self, units: int, mindex: int = 0) -> str:
         return f"{unit[units]}{self.millfn(mindex)}"
 
     def tenfn(self, tens, units, mindex=0) -> str:
```

### Comparing `inflect-6.2.0/inflect.egg-info/PKG-INFO` & `inflect-7.0.0/inflect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 6.2.0
+Version: 7.0.0
 Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
 Home-page: https://github.com/jaraco/inflect
 Author: Paul Dyson
 Author-email: pwdyson@yahoo.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inflect-6.2.0/inflect.egg-info/SOURCES.txt` & `inflect-7.0.0/inflect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/pytest.ini` & `inflect-7.0.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/setup.cfg` & `inflect-7.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/inflections.txt` & `inflect-7.0.0/tests/inflections.txt`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_an.py` & `inflect-7.0.0/tests/test_an.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_classical_ancient.py` & `inflect-7.0.0/tests/test_classical_ancient.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_classical_herd.py` & `inflect-7.0.0/tests/test_classical_herd.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_classical_names.py` & `inflect-7.0.0/tests/test_classical_names.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_classical_person.py` & `inflect-7.0.0/tests/test_classical_person.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_classical_zero.py` & `inflect-7.0.0/tests/test_classical_zero.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_compounds.py` & `inflect-7.0.0/tests/test_compounds.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_inflections.py` & `inflect-7.0.0/tests/test_inflections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import io
 
 import pytest
 
 import inflect
 
 
 def is_eq(p, a, b):
@@ -78,15 +77,15 @@
     assert mod_plural == mod_PL_val
     assert class_plural == class_PL_val
     assert is_eq(p, singular, mod_plural) in ("s:p", "p:s", "eq")
     assert is_eq(p, mod_plural, singular) in ("p:s", "s:p", "eq")
     assert is_eq(p, singular, class_plural) in ("s:p", "p:s", "eq")
     assert is_eq(p, class_plural, singular) in ("p:s", "s:p", "eq")
     assert singular != ""
-    expected = mod_PL_val if class_PL_val else "%s|%s" % (mod_PL_val, class_PL_val)
+    expected = mod_PL_val if class_PL_val else "{}|{}".format(mod_PL_val, class_PL_val)
     assert mod_PL_val == expected
 
     if is_nv != "_V":
         assert p.singular_noun(mod_plural, 1) == singular
 
         assert p.singular_noun(class_plural, 1) == singular
 
@@ -261,9 +260,9 @@
         p = inflect.engine()
         assert p.inflect("plural('two')") == "twoes"
         p.inflect("plural(two)")
 
 
 def get_data():
     filename = os.path.join(os.path.dirname(__file__), "inflections.txt")
-    with io.open(filename, encoding='utf-8') as strm:
+    with open(filename, encoding='utf-8') as strm:
         return list(map(str.strip, strm))
```

### Comparing `inflect-6.2.0/tests/test_join.py` & `inflect-7.0.0/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_numwords.py` & `inflect-7.0.0/tests/test_numwords.py`

 * *Files identical despite different names*

### Comparing `inflect-6.2.0/tests/test_pwd.py` & `inflect-7.0.0/tests/test_pwd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import unittest
-
 import pytest
 
 from inflect import (
     BadChunkingOptionError,
     NumOutOfRangeError,
     BadNumValueError,
     BadGenderError,
@@ -12,130 +10,116 @@
 import inflect
 from inflect.compat.pydantic import same_method
 
 
 missing = object()
 
 
-class test(unittest.TestCase):
-    def TODO(
-        self,
-        ans,
-        answer_wanted,
-        answer_gives_now=missing,
-    ):
-        """
-        make this test for future testing
-
-        so can easily rename these to assertEqual when code ready
-        """
-        if ans == answer_wanted:
-            print("test unexpectedly passed!: {} == {}".format(ans, answer_wanted))
-        if answer_gives_now is not missing:
-            self.assertEqual(ans, answer_gives_now)
-
+class Test:
     def test_enclose(self):
         # def enclose
-        self.assertEqual(inflect.enclose("test"), "(?:test)")
+        assert inflect.enclose("test") == "(?:test)"
 
     def test_joinstem(self):
         # def joinstem
-        self.assertEqual(
-            inflect.joinstem(-2, ["ephemeris", "iris", ".*itis"]), "(?:ephemer|ir|.*it)"
+        assert (
+            inflect.joinstem(-2, ["ephemeris", "iris", ".*itis"])
+            == "(?:ephemer|ir|.*it)"
         )
 
     def test_classical(self):
         # classical dicts
-        self.assertEqual(
-            set(inflect.def_classical.keys()), set(inflect.all_classical.keys())
-        )
-        self.assertEqual(
-            set(inflect.def_classical.keys()), set(inflect.no_classical.keys())
-        )
+        assert set(inflect.def_classical.keys()) == set(inflect.all_classical.keys())
+        assert set(inflect.def_classical.keys()) == set(inflect.no_classical.keys())
 
         # def classical
         p = inflect.engine()
-        self.assertEqual(p.classical_dict, inflect.def_classical)
+        assert p.classical_dict == inflect.def_classical
 
         p.classical()
-        self.assertEqual(p.classical_dict, inflect.all_classical)
+        assert p.classical_dict == inflect.all_classical
 
-        self.assertRaises(TypeError, p.classical, 0)
-        self.assertRaises(TypeError, p.classical, 1)
-        self.assertRaises(TypeError, p.classical, "names")
-        self.assertRaises(TypeError, p.classical, "names", "zero")
-        self.assertRaises(TypeError, p.classical, "all")
+        with pytest.raises(TypeError):
+            p.classical(0)
+        with pytest.raises(TypeError):
+            p.classical(1)
+        with pytest.raises(TypeError):
+            p.classical("names")
+        with pytest.raises(TypeError):
+            p.classical("names", "zero")
+        with pytest.raises(TypeError):
+            p.classical("all")
 
         p.classical(all=False)
-        self.assertEqual(p.classical_dict, inflect.no_classical)
+        assert p.classical_dict == inflect.no_classical
 
         p.classical(names=True, zero=True)
         mydict = inflect.def_classical.copy()
         mydict.update(dict(names=1, zero=1))
-        self.assertEqual(p.classical_dict, mydict)
+        assert p.classical_dict == mydict
 
         p.classical(all=True)
-        self.assertEqual(p.classical_dict, inflect.all_classical)
+        assert p.classical_dict == inflect.all_classical
 
         p.classical(all=False)
         p.classical(names=True, zero=True)
         mydict = inflect.def_classical.copy()
         mydict.update(dict(names=True, zero=True))
-        self.assertEqual(p.classical_dict, mydict)
+        assert p.classical_dict == mydict
 
         p.classical(all=False)
         p.classical(names=True, zero=False)
         mydict = inflect.def_classical.copy()
         mydict.update(dict(names=True, zero=False))
-        self.assertEqual(p.classical_dict, mydict)
+        assert p.classical_dict == mydict
 
-        self.assertRaises(UnknownClassicalModeError, p.classical, bogus=True)
+        with pytest.raises(UnknownClassicalModeError):
+            p.classical(bogus=True)
 
     def test_num(self):
         # def num
         p = inflect.engine()
-        self.assertTrue(p.persistent_count is None)
+        assert p.persistent_count is None
 
         p.num()
-        self.assertTrue(p.persistent_count is None)
+        assert p.persistent_count is None
 
         ret = p.num(3)
-        self.assertEqual(p.persistent_count, 3)
-        self.assertEqual(ret, "3")
+        assert p.persistent_count == 3
+        assert ret == "3"
 
         p.num()
         ret = p.num("3")
-        self.assertEqual(p.persistent_count, 3)
-        self.assertEqual(ret, "3")
+        assert p.persistent_count == 3
+        assert ret == "3"
 
         p.num()
         ret = p.num(count=3, show=1)
-        self.assertEqual(p.persistent_count, 3)
-        self.assertEqual(ret, "3")
+        assert p.persistent_count == 3
+        assert ret == "3"
 
         p.num()
         ret = p.num(count=3, show=0)
-        self.assertEqual(p.persistent_count, 3)
-        self.assertEqual(ret, "")
+        assert p.persistent_count == 3
+        assert ret == ""
 
-        self.assertRaises(BadNumValueError, p.num, "text")
+        with pytest.raises(BadNumValueError):
+            p.num("text")
 
     def test_inflect(self):
         p = inflect.engine()
         for txt, ans in (
             ("num(1)", "1"),
             ("num(1,0)", ""),
             ("num(1,1)", "1"),
             ("num(1)   ", "1   "),
             ("   num(1)   ", "   1   "),
             ("num(3) num(1)", "3 1"),
         ):
-            self.assertEqual(
-                p.inflect(txt), ans, msg='p.inflect("{}") != "{}"'.format(txt, ans)
-            )
+            assert p.inflect(txt) == ans, f'p.inflect("{txt}") != "{ans}"'
 
         for txt, ans in (
             ("plural('rock')", "rocks"),
             ("plural('rock')  plural('child')", "rocks  children"),
             ("num(2) plural('rock')  plural('child')", "2 rocks  children"),
             (
                 "plural('rock') plural_noun('rock') plural_verb('rocks') "
@@ -145,97 +129,99 @@
             (
                 "an('rock') no('cat') ordinal(3) number_to_words(1234) "
                 "present_participle('runs')",
                 "a rock no cats 3rd one thousand, two hundred and thirty-four running",
             ),
             ("a('cat',0) a('cat',1) a('cat',2) a('cat', 2)", "0 cat a cat 2 cat 2 cat"),
         ):
-            self.assertEqual(
-                p.inflect(txt), ans, msg='p.inflect("{}") != "{}"'.format(txt, ans)
-            )
+            assert p.inflect(txt) == ans, f'p.inflect("{txt}") != "{ans}"'
 
     def test_user_input_fns(self):
         p = inflect.engine()
 
-        self.assertEqual(p.pl_sb_user_defined, [])
+        assert p.pl_sb_user_defined == []
         p.defnoun("VAX", "VAXen")
-        self.assertEqual(p.plural("VAX"), "VAXEN")
-        self.assertEqual(p.pl_sb_user_defined, ["VAX", "VAXen"])
+        assert p.plural("VAX") == "VAXEN"
+        assert p.pl_sb_user_defined == ["VAX", "VAXen"]
 
-        self.assertTrue(p.ud_match("word", p.pl_sb_user_defined) is None)
-        self.assertEqual(p.ud_match("VAX", p.pl_sb_user_defined), "VAXen")
-        self.assertTrue(p.ud_match("VVAX", p.pl_sb_user_defined) is None)
+        assert p.ud_match("word", p.pl_sb_user_defined) is None
+        assert p.ud_match("VAX", p.pl_sb_user_defined) == "VAXen"
+        assert p.ud_match("VVAX", p.pl_sb_user_defined) is None
 
         p.defnoun("cow", "cows|kine")
-        self.assertEqual(p.plural("cow"), "cows")
+        assert p.plural("cow") == "cows"
         p.classical()
-        self.assertEqual(p.plural("cow"), "kine")
+        assert p.plural("cow") == "kine"
 
-        self.assertEqual(p.ud_match("cow", p.pl_sb_user_defined), "cows|kine")
+        assert p.ud_match("cow", p.pl_sb_user_defined) == "cows|kine"
 
         p.defnoun("(.+i)o", r"$1i")
-        self.assertEqual(p.plural("studio"), "studii")
-        self.assertEqual(p.ud_match("studio", p.pl_sb_user_defined), "studii")
+        assert p.plural("studio") == "studii"
+        assert p.ud_match("studio", p.pl_sb_user_defined) == "studii"
 
         p.defnoun("aviatrix", "aviatrices")
-        self.assertEqual(p.plural("aviatrix"), "aviatrices")
-        self.assertEqual(p.ud_match("aviatrix", p.pl_sb_user_defined), "aviatrices")
+        assert p.plural("aviatrix") == "aviatrices"
+        assert p.ud_match("aviatrix", p.pl_sb_user_defined) == "aviatrices"
         p.defnoun("aviatrix", "aviatrixes")
-        self.assertEqual(p.plural("aviatrix"), "aviatrixes")
-        self.assertEqual(p.ud_match("aviatrix", p.pl_sb_user_defined), "aviatrixes")
+        assert p.plural("aviatrix") == "aviatrixes"
+        assert p.ud_match("aviatrix", p.pl_sb_user_defined) == "aviatrixes"
         p.defnoun("aviatrix", None)
-        self.assertEqual(p.plural("aviatrix"), "aviatrices")
-        self.assertEqual(p.ud_match("aviatrix", p.pl_sb_user_defined), None)
+        assert p.plural("aviatrix") == "aviatrices"
+        assert p.ud_match("aviatrix", p.pl_sb_user_defined) is None
 
         p.defnoun("(cat)", r"$1s")
-        self.assertEqual(p.plural("cat"), "cats")
+        assert p.plural("cat") == "cats"
 
-        inflect.STDOUT_ON = False
-        self.assertRaises(inflect.BadUserDefinedPatternError, p.defnoun, "(??", None)
-        inflect.STDOUT_ON = True
+        with pytest.raises(inflect.BadUserDefinedPatternError):
+            p.defnoun("(??", None)
 
         p.defnoun(None, "any")  # check None doesn't crash it
 
-        # defverb
-        p.defverb("will", "shall", "will", "will", "will", "will")
-        self.assertEqual(p.ud_match("will", p.pl_v_user_defined), "will")
-        self.assertEqual(p.plural("will"), "will")
-        # TODO: will -> shall. Tests below fail
-        self.TODO(p.compare("will", "shall"), "s:p")
-        self.TODO(p.compare_verbs("will", "shall"), "s:p")
-
         # defadj
         p.defadj("hir", "their")
-        self.assertEqual(p.plural("hir"), "their")
-        self.assertEqual(p.ud_match("hir", p.pl_adj_user_defined), "their")
+        assert p.plural("hir") == "their"
+        assert p.ud_match("hir", p.pl_adj_user_defined) == "their"
 
         # defa defan
         p.defa("h")
-        self.assertEqual(p.a("h"), "a h")
-        self.assertEqual(p.ud_match("h", p.A_a_user_defined), "a")
+        assert p.a("h") == "a h"
+        assert p.ud_match("h", p.A_a_user_defined) == "a"
 
         p.defan("horrendous.*")
-        self.assertEqual(p.a("horrendously"), "an horrendously")
-        self.assertEqual(p.ud_match("horrendously", p.A_a_user_defined), "an")
+        assert p.a("horrendously") == "an horrendously"
+        assert p.ud_match("horrendously", p.A_a_user_defined) == "an"
+
+    def test_user_input_defverb(self):
+        p = inflect.engine()
+        p.defverb("will", "shall", "will", "will", "will", "will")
+        assert p.ud_match("will", p.pl_v_user_defined) == "will"
+        assert p.plural("will") == "will"
+
+    @pytest.mark.xfail(reason="todo")
+    def test_user_input_defverb_compare(self):
+        p = inflect.engine()
+        p.defverb("will", "shall", "will", "will", "will", "will")
+        assert p.compare("will", "shall") == "s:p"
+        assert p.compare_verbs("will", "shall") == "s:p"
 
     def test_postprocess(self):
         p = inflect.engine()
         for orig, infl, txt in (
             ("cow", "cows", "cows"),
             ("I", "we", "we"),
             ("COW", "cows", "COWS"),
             ("Cow", "cows", "Cows"),
             ("cow", "cows|kine", "cows"),
             ("Entry", "entries", "Entries"),
             ("can of Coke", "cans of coke", "cans of Coke"),
         ):
-            self.assertEqual(p.postprocess(orig, infl), txt)
+            assert p.postprocess(orig, infl) == txt
 
         p.classical()
-        self.assertEqual(p.postprocess("cow", "cows|kine"), "kine")
+        assert p.postprocess("cow", "cows|kine") == "kine"
 
     def test_partition_word(self):
         p = inflect.engine()
         for txt, part in (
             (" cow ", (" ", "cow", " ")),
             ("cow", ("", "cow", "")),
             ("   cow", ("   ", "cow", "")),
@@ -244,15 +230,15 @@
             ("", ("", "", "")),
             ("bottle of beer", ("", "bottle of beer", "")),
             # spaces give weird results
             # (' '),('', ' ', '')),
             # ('  '),(' ', ' ', '')),
             # ('   '),('  ', ' ', '')),
         ):
-            self.assertEqual(p.partition_word(txt), part)
+            assert p.partition_word(txt) == part
 
     def test_pl(self):
         p = inflect.engine()
         for fn, sing, plur in (
             (p.plural, "cow", "cows"),
             (p.plural, "thought", "thoughts"),
             (p.plural, "mouse", "mice"),
@@ -273,275 +259,278 @@
             (p.plural_adj, "a", "some"),
             (p.plural_adj, "this", "these"),
             (p.plural_adj, "that", "those"),
             (p.plural_adj, "my", "our"),
             (p.plural_adj, "cat's", "cats'"),
             (p.plural_adj, "child's", "children's"),
         ):
-            self.assertEqual(
-                fn(sing),
-                plur,
-                msg='{}("{}") == "{}" != "{}"'.format(
-                    fn.__name__, sing, fn(sing), plur
-                ),
+            assert fn(sing) == plur, '{}("{}") == "{}" != "{}"'.format(
+                fn.__name__, sing, fn(sing), plur
             )
 
         for sing, num, plur in (
             ("cow", 1, "cow"),
             ("cow", 2, "cows"),
             ("cow", "one", "cow"),
             ("cow", "each", "cow"),
             ("cow", "two", "cows"),
             ("cow", 0, "cows"),
             ("cow", "zero", "cows"),
             ("runs", 0, "run"),
             ("runs", 1, "runs"),
             ("am", 0, "are"),
         ):
-            self.assertEqual(p.plural(sing, num), plur)
+            assert p.plural(sing, num) == plur
 
         p.classical(zero=True)
-        self.assertEqual(p.plural("cow", 0), "cow")
-        self.assertEqual(p.plural("cow", "zero"), "cow")
-        self.assertEqual(p.plural("runs", 0), "runs")
-        self.assertEqual(p.plural("am", 0), "am")
-        self.assertEqual(p.plural_verb("runs", 1), "runs")
+        assert p.plural("cow", 0) == "cow"
+        assert p.plural("cow", "zero") == "cow"
+        assert p.plural("runs", 0) == "runs"
+        assert p.plural("am", 0) == "am"
+        assert p.plural_verb("runs", 1) == "runs"
 
-        self.assertEqual(p.plural("die"), "dice")
-        self.assertEqual(p.plural_noun("die"), "dice")
+        assert p.plural("die") == "dice"
+        assert p.plural_noun("die") == "dice"
 
         with pytest.raises(Exception):
             p.plural("")
             p.plural_noun("")
             p.plural_verb("")
             p.plural_adj("")
 
     def test_sinoun(self):
         p = inflect.engine()
         for sing, plur in (
             ("cat", "cats"),
             ("die", "dice"),
             ("goose", "geese"),
         ):
-            self.assertEqual(p.singular_noun(plur), sing)
-            self.assertEqual(p.inflect("singular_noun('%s')" % plur), sing)
+            assert p.singular_noun(plur) == sing
+            assert p.inflect("singular_noun('%s')" % plur) == sing
 
-        self.assertEqual(p.singular_noun("cats", count=2), "cats")
-        self.assertEqual(p.singular_noun("open valves", count=2), "open valves")
+        assert p.singular_noun("cats", count=2) == "cats"
+        assert p.singular_noun("open valves", count=2) == "open valves"
 
-        self.assertEqual(p.singular_noun("zombies"), "zombie")
+        assert p.singular_noun("zombies") == "zombie"
 
-        self.assertEqual(p.singular_noun("shoes"), "shoe")
-        self.assertEqual(p.singular_noun("dancing shoes"), "dancing shoe")
+        assert p.singular_noun("shoes") == "shoe"
+        assert p.singular_noun("dancing shoes") == "dancing shoe"
 
-        self.assertEqual(p.singular_noun("Matisses"), "Matisse")
-        self.assertEqual(p.singular_noun("bouillabaisses"), "bouillabaisse")
+        assert p.singular_noun("Matisses") == "Matisse"
+        assert p.singular_noun("bouillabaisses") == "bouillabaisse"
 
-        self.assertEqual(p.singular_noun("quartzes"), "quartz")
+        assert p.singular_noun("quartzes") == "quartz"
 
-        self.assertEqual(p.singular_noun("Nietzsches"), "Nietzsche")
-        self.assertEqual(p.singular_noun("aches"), "ache")
+        assert p.singular_noun("Nietzsches") == "Nietzsche"
+        assert p.singular_noun("aches") == "ache"
 
-        self.assertEqual(p.singular_noun("Clives"), "Clive")
-        self.assertEqual(p.singular_noun("weaves"), "weave")
+        assert p.singular_noun("Clives") == "Clive"
+        assert p.singular_noun("weaves") == "weave"
 
-        self.assertEqual(p.singular_noun("status"), False)
-        self.assertEqual(p.singular_noun("hiatus"), False)
+        assert p.singular_noun("status") is False
+        assert p.singular_noun("hiatus") is False
 
     def test_gender(self):
         p = inflect.engine()
         p.gender("feminine")
         for sing, plur in (
             ("she", "they"),
             ("herself", "themselves"),
             ("hers", "theirs"),
             ("to her", "to them"),
             ("to herself", "to themselves"),
         ):
-            self.assertEqual(
-                p.singular_noun(plur),
-                sing,
-                "singular_noun({}) == {} != {}".format(
-                    plur, p.singular_noun(plur), sing
-                ),
-            )
-            self.assertEqual(p.inflect("singular_noun('%s')" % plur), sing)
+            assert (
+                p.singular_noun(plur) == sing
+            ), f"singular_noun({plur}) == {p.singular_noun(plur)} != {sing}"
+            assert p.inflect("singular_noun('%s')" % plur) == sing
 
         p.gender("masculine")
         for sing, plur in (
             ("he", "they"),
             ("himself", "themselves"),
             ("his", "theirs"),
             ("to him", "to them"),
             ("to himself", "to themselves"),
         ):
-            self.assertEqual(
-                p.singular_noun(plur),
-                sing,
-                "singular_noun({}) == {} != {}".format(
-                    plur, p.singular_noun(plur), sing
-                ),
-            )
-            self.assertEqual(p.inflect("singular_noun('%s')" % plur), sing)
+            assert (
+                p.singular_noun(plur) == sing
+            ), f"singular_noun({plur}) == {p.singular_noun(plur)} != {sing}"
+            assert p.inflect("singular_noun('%s')" % plur) == sing
 
         p.gender("gender-neutral")
         for sing, plur in (
             ("they", "they"),
             ("themself", "themselves"),
             ("theirs", "theirs"),
             ("to them", "to them"),
             ("to themself", "to themselves"),
         ):
-            self.assertEqual(
-                p.singular_noun(plur),
-                sing,
-                "singular_noun({}) == {} != {}".format(
-                    plur, p.singular_noun(plur), sing
-                ),
-            )
-            self.assertEqual(p.inflect("singular_noun('%s')" % plur), sing)
+            assert (
+                p.singular_noun(plur) == sing
+            ), f"singular_noun({plur}) == {p.singular_noun(plur)} != {sing}"
+            assert p.inflect("singular_noun('%s')" % plur) == sing
 
         p.gender("neuter")
         for sing, plur in (
             ("it", "they"),
             ("itself", "themselves"),
             ("its", "theirs"),
             ("to it", "to them"),
             ("to itself", "to themselves"),
         ):
-            self.assertEqual(
-                p.singular_noun(plur),
-                sing,
-                "singular_noun({}) == {} != {}".format(
-                    plur, p.singular_noun(plur), sing
-                ),
-            )
-            self.assertEqual(p.inflect("singular_noun('%s')" % plur), sing)
+            assert (
+                p.singular_noun(plur) == sing
+            ), f"singular_noun({plur}) == {p.singular_noun(plur)} != {sing}"
+            assert p.inflect("singular_noun('%s')" % plur) == sing
 
-        self.assertRaises(BadGenderError, p.gender, "male")
+        with pytest.raises(BadGenderError):
+            p.gender("male")
 
         for sing, plur, gen in (
             ("it", "they", "neuter"),
             ("she", "they", "feminine"),
             ("he", "they", "masculine"),
             ("they", "they", "gender-neutral"),
             ("she or he", "they", "feminine or masculine"),
             ("he or she", "they", "masculine or feminine"),
         ):
-            self.assertEqual(p.singular_noun(plur, gender=gen), sing)
+            assert p.singular_noun(plur, gender=gen) == sing
 
-        with self.assertRaises(BadGenderError):
+        with pytest.raises(BadGenderError):
             p.singular_noun("cats", gender="unknown gender")
 
-    def test_plequal(self):
-        p = inflect.engine()
-        for fn, sing, plur, res in (
-            (p.compare, "index", "index", "eq"),
-            (p.compare, "index", "indexes", "s:p"),
-            (p.compare, "index", "indices", "s:p"),
-            (p.compare, "indexes", "index", "p:s"),
-            (p.compare, "indices", "index", "p:s"),
-            (p.compare, "indices", "indexes", "p:p"),
-            (p.compare, "indexes", "indices", "p:p"),
-            (p.compare, "indices", "indices", "eq"),
-            (p.compare, "inverted index", "inverted indices", "s:p"),
-            (p.compare, "inverted indices", "inverted index", "p:s"),
-            (p.compare, "inverted indexes", "inverted indices", "p:p"),
-            (p.compare, "opuses", "opera", "p:p"),
-            (p.compare, "opera", "opuses", "p:p"),
-            (p.compare, "brothers", "brethren", "p:p"),
-            (p.compare, "cats", "cats", "eq"),
-            (p.compare, "base", "basis", False),
-            (p.compare, "syrinx", "syringe", False),
-            (p.compare, "she", "he", False),
-            (p.compare, "opus", "operas", False),
-            (p.compare, "taxi", "taxes", False),
-            (p.compare, "time", "Times", False),
-            (p.compare, "time".lower(), "Times".lower(), "s:p"),
-            (p.compare, "courts martial", "court martial", "p:s"),
-            (p.compare, "my", "my", "eq"),
-            (p.compare, "my", "our", "s:p"),
-            (p.compare, "our", "our", "eq"),
-            (p.compare_nouns, "index", "index", "eq"),
-            (p.compare_nouns, "index", "indexes", "s:p"),
-            (p.compare_nouns, "index", "indices", "s:p"),
-            (p.compare_nouns, "indexes", "index", "p:s"),
-            (p.compare_nouns, "indices", "index", "p:s"),
-            (p.compare_nouns, "indices", "indexes", "p:p"),
-            (p.compare_nouns, "indexes", "indices", "p:p"),
-            (p.compare_nouns, "indices", "indices", "eq"),
-            (p.compare_nouns, "inverted index", "inverted indices", "s:p"),
-            (p.compare_nouns, "inverted indices", "inverted index", "p:s"),
-            (p.compare_nouns, "inverted indexes", "inverted indices", "p:p"),
-            (p.compare_verbs, "runs", "runs", "eq"),
-            (p.compare_verbs, "runs", "run", "s:p"),
-            (p.compare_verbs, "run", "run", "eq"),
-            (p.compare_adjs, "my", "my", "eq"),
-            (p.compare_adjs, "my", "our", "s:p"),
-            (p.compare_adjs, "our", "our", "eq"),
-        ):
-            self.assertEqual(fn(sing, plur), res)
-
-    def test_plequal_todos(self):
+    @pytest.mark.parametrize(
+        'sing,plur,res',
+        (
+            ("index", "index", "eq"),
+            ("index", "indexes", "s:p"),
+            ("index", "indices", "s:p"),
+            ("indexes", "index", "p:s"),
+            ("indices", "index", "p:s"),
+            ("indices", "indexes", "p:p"),
+            ("indexes", "indices", "p:p"),
+            ("indices", "indices", "eq"),
+            ("inverted index", "inverted indices", "s:p"),
+            ("inverted indices", "inverted index", "p:s"),
+            ("inverted indexes", "inverted indices", "p:p"),
+            ("opuses", "opera", "p:p"),
+            ("opera", "opuses", "p:p"),
+            ("brothers", "brethren", "p:p"),
+            ("cats", "cats", "eq"),
+            ("base", "basis", False),
+            ("syrinx", "syringe", False),
+            ("she", "he", False),
+            ("opus", "operas", False),
+            ("taxi", "taxes", False),
+            ("time", "Times", False),
+            ("time".lower(), "Times".lower(), "s:p"),
+            ("courts martial", "court martial", "p:s"),
+            ("my", "my", "eq"),
+            ("my", "our", "s:p"),
+            ("our", "our", "eq"),
+            pytest.param(
+                "dresses's", "dresses'", "p:p", marks=pytest.mark.xfail(reason="todo")
+            ),
+            pytest.param(
+                "dress's", "dress'", "s:s", marks=pytest.mark.xfail(reason='todo')
+            ),
+            pytest.param(
+                "Jess's", "Jess'", "s:s", marks=pytest.mark.xfail(reason='todo')
+            ),
+        ),
+    )
+    def test_compare_simple(self, sing, plur, res):
+        assert inflect.engine().compare(sing, plur) == res
+
+    @pytest.mark.parametrize(
+        'sing,plur,res',
+        (
+            ("index", "index", "eq"),
+            ("index", "indexes", "s:p"),
+            ("index", "indices", "s:p"),
+            ("indexes", "index", "p:s"),
+            ("indices", "index", "p:s"),
+            ("indices", "indexes", "p:p"),
+            ("indexes", "indices", "p:p"),
+            ("indices", "indices", "eq"),
+            ("inverted index", "inverted indices", "s:p"),
+            ("inverted indices", "inverted index", "p:s"),
+            ("inverted indexes", "inverted indices", "p:p"),
+        ),
+    )
+    def test_compare_nouns(self, sing, plur, res):
+        assert inflect.engine().compare_nouns(sing, plur) == res
+
+    @pytest.mark.parametrize(
+        'sing,plur,res',
+        (
+            ("runs", "runs", "eq"),
+            ("runs", "run", "s:p"),
+            ("run", "run", "eq"),
+        ),
+    )
+    def test_compare_verbs(self, sing, plur, res):
+        assert inflect.engine().compare_verbs(sing, plur) == res
+
+    @pytest.mark.parametrize(
+        'sing,plur,res',
+        (
+            ("my", "my", "eq"),
+            ("my", "our", "s:p"),
+            ("our", "our", "eq"),
+            pytest.param(
+                "dresses's", "dresses'", "p:p", marks=pytest.mark.xfail(reason="todo")
+            ),
+            pytest.param(
+                "dress's", "dress'", "s:s", marks=pytest.mark.xfail(reason='todo')
+            ),
+            pytest.param(
+                "Jess's", "Jess'", "s:s", marks=pytest.mark.xfail(reason='todo')
+            ),
+        ),
+    )
+    def test_compare_adjectives(self, sing, plur, res):
+        assert inflect.engine().compare_adjs(sing, plur) == res
+
+    @pytest.mark.xfail()
+    def test_compare_your_our(self):
+        # multiple adjective plurals not (yet) supported
         p = inflect.engine()
-        for fn, sing, plur, res, badres in (
-            (
-                p.compare,
-                "dresses's",
-                "dresses'",
-                "p:p",
-                "p:s",
-            ),  # TODO: should return p:p
-            (
-                p.compare_adjs,
-                "dresses's",
-                "dresses'",
-                "p:p",
-                False,
-            ),  # TODO: should return p:p
-            # TODO: future: support different singulars one day.
-            (p.compare, "dress's", "dress'", "s:s", "p:s"),
-            (p.compare_adjs, "dress's", "dress'", "s:s", False),
-            (p.compare, "Jess's", "Jess'", "s:s", "p:s"),
-            (p.compare_adjs, "Jess's", "Jess'", "s:s", False),
-        ):
-            self.TODO(fn(sing, plur), res, badres)
-
-        # TODO: pass upstream. multiple adjective plurals not supported
-        self.assertEqual(p.compare("your", "our"), False)
+        assert p.compare("your", "our") is False
         p.defadj("my", "our|your")  # what's ours is yours
-        self.TODO(p.compare("your", "our"), "p:p")
+        assert p.compare("your", "our") == "p:p"
 
     def test__pl_reg_plurals(self):
         p = inflect.engine()
         for pair, stems, end1, end2, ans in (
             ("indexes|indices", "dummy|ind", "exes", "ices", True),
             ("indexes|robots", "dummy|ind", "exes", "ices", False),
             ("beaus|beaux", ".*eau", "s", "x", True),
         ):
-            self.assertEqual(p._pl_reg_plurals(pair, stems, end1, end2), ans)
+            assert p._pl_reg_plurals(pair, stems, end1, end2) == ans
 
     def test__pl_check_plurals_N(self):
         p = inflect.engine()
-        self.assertEqual(p._pl_check_plurals_N("index", "indices"), False)
-        self.assertEqual(p._pl_check_plurals_N("indexes", "indices"), True)
-        self.assertEqual(p._pl_check_plurals_N("indices", "indexes"), True)
-        self.assertEqual(p._pl_check_plurals_N("stigmata", "stigmas"), True)
-        self.assertEqual(p._pl_check_plurals_N("phalanxes", "phalanges"), True)
+        assert p._pl_check_plurals_N("index", "indices") is False
+        assert p._pl_check_plurals_N("indexes", "indices") is True
+        assert p._pl_check_plurals_N("indices", "indexes") is True
+        assert p._pl_check_plurals_N("stigmata", "stigmas") is True
+        assert p._pl_check_plurals_N("phalanxes", "phalanges") is True
 
     def test__pl_check_plurals_adj(self):
         p = inflect.engine()
-        self.assertEqual(p._pl_check_plurals_adj("indexes's", "indices's"), True)
-        self.assertEqual(p._pl_check_plurals_adj("indices's", "indexes's"), True)
-        self.assertEqual(p._pl_check_plurals_adj("indexes'", "indices's"), True)
-        self.assertEqual(p._pl_check_plurals_adj("indexes's", "indices'"), True)
-        self.assertEqual(p._pl_check_plurals_adj("indexes's", "indexes's"), False)
-        self.assertEqual(p._pl_check_plurals_adj("dogmas's", "dogmata's"), True)
-        self.assertEqual(p._pl_check_plurals_adj("dogmas'", "dogmata'"), True)
-        self.assertEqual(p._pl_check_plurals_adj("indexes'", "indices'"), True)
+        assert p._pl_check_plurals_adj("indexes's", "indices's") is True
+        assert p._pl_check_plurals_adj("indices's", "indexes's") is True
+        assert p._pl_check_plurals_adj("indexes'", "indices's") is True
+        assert p._pl_check_plurals_adj("indexes's", "indices'") is True
+        assert p._pl_check_plurals_adj("indexes's", "indexes's") is False
+        assert p._pl_check_plurals_adj("dogmas's", "dogmata's") is True
+        assert p._pl_check_plurals_adj("dogmas'", "dogmata'") is True
+        assert p._pl_check_plurals_adj("indexes'", "indices'") is True
 
     def test_count(self):
         p = inflect.engine()
         for txt, num in (
             (1, 1),
             (2, 2),
             (0, 2),
@@ -558,19 +547,19 @@
             ("one", 1),
             ("each", 1),
             ("every", 1),
             ("this", 1),
             ("that", 1),
             ("dummy", 2),
         ):
-            self.assertEqual(p.get_count(txt), num)
+            assert p.get_count(txt) == num
 
-        self.assertEqual(p.get_count(), "")
+        assert p.get_count() == ""
         p.num(3)
-        self.assertEqual(p.get_count(), 2)
+        assert p.get_count() == 2
 
     def test__plnoun(self):
         p = inflect.engine()
         for sing, plur in (
             ("tuna", "tuna"),
             ("TUNA", "TUNA"),
             ("swordfish", "swordfish"),
@@ -617,59 +606,45 @@
             ("sally", "sallies"),
             ("ado", "ados"),
             ("auto", "autos"),
             ("alto", "altos"),
             ("zoo", "zoos"),
             ("tomato", "tomatoes"),
         ):
-            self.assertEqual(
-                p._plnoun(sing),
-                plur,
-                msg='p._plnoun("{}") == {} != "{}"'.format(sing, p._plnoun(sing), plur),
+            assert p._plnoun(sing) == plur, 'p._plnoun("{}") == {} != "{}"'.format(
+                sing, p._plnoun(sing), plur
             )
 
-            self.assertEqual(
-                p._sinoun(plur), sing, msg='p._sinoun("{}") != "{}"'.format(plur, sing)
-            )
+            assert p._sinoun(plur) == sing, f'p._sinoun("{plur}") != "{sing}"'
 
         # words where forming singular is ambiguous or not attempted
         for sing, plur in (
             ("son of a gun", "sons of guns"),
             ("son-of-a-gun", "sons-of-guns"),
             ("basis", "bases"),
             ("Jess", "Jesses"),
         ):
-            self.assertEqual(
-                p._plnoun(sing), plur, msg='p._plnoun("{}") != "{}"'.format(sing, plur)
-            )
-
-        for sing, plur in (
-            # TODO: does not keep case
-            ("about ME", "about US"),
-            # TODO: does not keep case
-            ("YOU", "YOU"),
-        ):
-            self.TODO(p._plnoun(sing), plur)
+            assert p._plnoun(sing) == plur, f'p._plnoun("{sing}") != "{plur}"'
 
         p.num(1)
-        self.assertEqual(p._plnoun("cat"), "cat")
+        assert p._plnoun("cat") == "cat"
         p.num(3)
 
         p.classical(herd=True)
-        self.assertEqual(p._plnoun("swine"), "swine")
+        assert p._plnoun("swine") == "swine"
         p.classical(herd=False)
-        self.assertEqual(p._plnoun("swine"), "swines")
+        assert p._plnoun("swine") == "swines"
         p.classical(persons=True)
-        self.assertEqual(p._plnoun("chairperson"), "chairpersons")
+        assert p._plnoun("chairperson") == "chairpersons"
         p.classical(persons=False)
-        self.assertEqual(p._plnoun("chairperson"), "chairpeople")
+        assert p._plnoun("chairperson") == "chairpeople"
         p.classical(ancient=True)
-        self.assertEqual(p._plnoun("formula"), "formulae")
+        assert p._plnoun("formula") == "formulae"
         p.classical(ancient=False)
-        self.assertEqual(p._plnoun("formula"), "formulas")
+        assert p._plnoun("formula") == "formulas"
 
         p.classical()
         for sing, plur in (
             ("matrix", "matrices"),
             ("gateau", "gateaux"),
             ("millieu", "millieux"),
             ("syrinx", "syringes"),
@@ -683,83 +658,117 @@
             ("soma", "somata"),
             ("iris", "irides"),
             ("solo", "soli"),
             ("oxymoron", "oxymora"),
             ("goy", "goyim"),
             ("afrit", "afriti"),
         ):
-            self.assertEqual(p._plnoun(sing), plur)
+            assert p._plnoun(sing) == plur
 
         # p.classical(0)
         # p.classical('names')
         # classical now back to the default mode
 
+    @pytest.mark.parametrize(
+        'sing, plur',
+        (
+            pytest.param(
+                'about ME',
+                'about US',
+                marks=pytest.mark.xfail(reason='does not keep case'),
+            ),
+            pytest.param(
+                'YOU',
+                'YOU',
+                marks=pytest.mark.xfail(reason='does not keep case'),
+            ),
+        ),
+    )
+    def test_plnoun_retains_case(self, sing, plur):
+        assert inflect.engine()._plnoun(sing) == plur
+
     def test_classical_pl(self):
         p = inflect.engine()
         p.classical()
         for sing, plur in (("brother", "brethren"), ("dogma", "dogmata")):
-            self.assertEqual(p.plural(sing), plur)
+            assert p.plural(sing) == plur
 
     def test__pl_special_verb(self):
         p = inflect.engine()
         with pytest.raises(Exception):
-            self.assertEqual(p._pl_special_verb(""), False)
-        self.assertEqual(p._pl_special_verb("am"), "are")
-        self.assertEqual(p._pl_special_verb("am", 0), "are")
-        self.assertEqual(p._pl_special_verb("runs", 0), "run")
+            assert p._pl_special_verb("") is False
+        assert p._pl_special_verb("am") == "are"
+        assert p._pl_special_verb("am", 0) == "are"
+        assert p._pl_special_verb("runs", 0) == "run"
         p.classical(zero=True)
-        self.assertEqual(p._pl_special_verb("am", 0), False)
-        self.assertEqual(p._pl_special_verb("am", 1), "am")
-        self.assertEqual(p._pl_special_verb("am", 2), "are")
-        self.assertEqual(p._pl_special_verb("runs", 0), False)
-        self.assertEqual(p._pl_special_verb("am going to"), "are going to")
-        self.assertEqual(p._pl_special_verb("did"), "did")
-        self.assertEqual(p._pl_special_verb("wasn't"), "weren't")
-        self.assertEqual(p._pl_special_verb("shouldn't"), "shouldn't")
-        self.assertEqual(p._pl_special_verb("bias"), False)
-        self.assertEqual(p._pl_special_verb("news"), False)
-        self.assertEqual(p._pl_special_verb("Jess"), False)
-        self.assertEqual(p._pl_special_verb(" "), False)
-        self.assertEqual(p._pl_special_verb("brushes"), "brush")
-        self.assertEqual(p._pl_special_verb("fixes"), "fix")
-        self.assertEqual(p._pl_special_verb("quizzes"), "quiz")
-        self.assertEqual(p._pl_special_verb("fizzes"), "fizz")
-        self.assertEqual(p._pl_special_verb("dresses"), "dress")
-        self.assertEqual(p._pl_special_verb("flies"), "fly")
-        self.assertEqual(p._pl_special_verb("canoes"), "canoe")
-        self.assertEqual(p._pl_special_verb("horseshoes"), "horseshoe")
-        self.assertEqual(p._pl_special_verb("does"), "do")
+        assert p._pl_special_verb("am", 0) is False
+        assert p._pl_special_verb("am", 1) == "am"
+        assert p._pl_special_verb("am", 2) == "are"
+        assert p._pl_special_verb("runs", 0) is False
+        assert p._pl_special_verb("am going to") == "are going to"
+        assert p._pl_special_verb("did") == "did"
+        assert p._pl_special_verb("wasn't") == "weren't"
+        assert p._pl_special_verb("shouldn't") == "shouldn't"
+        assert p._pl_special_verb("bias") is False
+        assert p._pl_special_verb("news") is False
+        assert p._pl_special_verb("Jess") is False
+        assert p._pl_special_verb(" ") is False
+        assert p._pl_special_verb("brushes") == "brush"
+        assert p._pl_special_verb("fixes") == "fix"
+        assert p._pl_special_verb("quizzes") == "quiz"
+        assert p._pl_special_verb("fizzes") == "fizz"
+        assert p._pl_special_verb("dresses") == "dress"
+        assert p._pl_special_verb("flies") == "fly"
+        assert p._pl_special_verb("canoes") == "canoe"
+        assert p._pl_special_verb("horseshoes") == "horseshoe"
+        assert p._pl_special_verb("does") == "do"
         # TODO: what's a real word to test this case?
-        self.assertEqual(p._pl_special_verb("zzzoes"), "zzzo")
-        self.assertEqual(p._pl_special_verb("runs"), "run")
+        assert p._pl_special_verb("zzzoes") == "zzzo"
+        assert p._pl_special_verb("runs") == "run"
 
     def test__pl_general_verb(self):
         p = inflect.engine()
-        self.assertEqual(p._pl_general_verb("acts"), "act")
-        self.assertEqual(p._pl_general_verb("act"), "act")
-        self.assertEqual(p._pl_general_verb("saw"), "saw")
-        self.assertEqual(p._pl_general_verb("runs", 1), "runs")
-
-    def test__pl_special_adjective(self):
-        p = inflect.engine()
-        self.assertEqual(p._pl_special_adjective("a"), "some")
-        self.assertEqual(p._pl_special_adjective("my"), "our")
-        self.assertEqual(p._pl_special_adjective("John's"), "Johns'")
-        # TODO: original can't handle this. should we handle it?
-        self.TODO(p._pl_special_adjective("JOHN's"), "JOHNS'")
-        # TODO: can't handle capitals
-        self.TODO(p._pl_special_adjective("JOHN'S"), "JOHNS'")
-        self.TODO(p._pl_special_adjective("TUNA'S"), "TUNA'S")
-        self.assertEqual(p._pl_special_adjective("tuna's"), "tuna's")
-        self.assertEqual(p._pl_special_adjective("TUNA's"), "TUNA's")
-        self.assertEqual(p._pl_special_adjective("bad"), False)
-
-    def test_a(self):
-        p = inflect.engine()
-        for sing, plur in (
+        assert p._pl_general_verb("acts") == "act"
+        assert p._pl_general_verb("act") == "act"
+        assert p._pl_general_verb("saw") == "saw"
+        assert p._pl_general_verb("runs", 1) == "runs"
+
+    @pytest.mark.parametrize(
+        'adj,plur',
+        (
+            ("a", "some"),
+            ("my", "our"),
+            ("John's", "Johns'"),
+            ("tuna's", "tuna's"),
+            ("TUNA's", "TUNA's"),
+            ("bad", False),
+            pytest.param(
+                "JOHN's",
+                "JOHNS'",
+                marks=pytest.mark.xfail(reason='should this be handled?'),
+            ),
+            pytest.param(
+                "JOHN'S",
+                "JOHNS'",
+                marks=pytest.mark.xfail(reason="can't handle capitals"),
+            ),
+            pytest.param(
+                "TUNA'S",
+                "TUNA'S",
+                marks=pytest.mark.xfail(reason="can't handle capitals"),
+            ),
+        ),
+    )
+    def test__pl_special_adjective(self, adj, plur):
+        p = inflect.engine()
+        assert p._pl_special_adjective(adj) == plur
+
+    @pytest.mark.parametrize(
+        'sing, plur',
+        (
             ("cat", "a cat"),
             ("euphemism", "a euphemism"),
             ("Euler number", "an Euler number"),
             ("hour", "an hour"),
             ("houri", "a houri"),
             ("nth", "an nth"),
             ("rth", "an rth"),
@@ -793,67 +802,74 @@
             ("UNESCO", "a UNESCO"),
             ("a", "an a"),
             ("an", "an an"),
             ("an ant", "an ant"),
             ("a cat", "a cat"),
             ("an cat", "a cat"),
             ("a ant", "an ant"),
-        ):
-            self.assertEqual(p.a(sing), plur)
+        ),
+    )
+    def test_a(self, sing, plur):
+        p = inflect.engine()
+        assert p.a(sing) == plur
 
-        self.assertEqual(p.a("cat", 1), "a cat")
-        self.assertEqual(p.a("cat", 2), "2 cat")
+    def test_a_alt(self):
+        p = inflect.engine()
+        assert p.a("cat", 1) == "a cat"
+        assert p.a("cat", 2) == "2 cat"
 
         with pytest.raises(Exception):
             p.a("")
 
     def test_a_and_an_same_method(self):
         assert same_method(inflect.engine.a, inflect.engine.an)
         p = inflect.engine()
         assert same_method(p.a, p.an)
 
     def test_no(self):
         p = inflect.engine()
-        self.assertEqual(p.no("cat"), "no cats")
-        self.assertEqual(p.no("cat", count=3), "3 cats")
-        self.assertEqual(p.no("cat", count="three"), "three cats")
-        self.assertEqual(p.no("cat", count=1), "1 cat")
-        self.assertEqual(p.no("cat", count="one"), "one cat")
-        self.assertEqual(p.no("mouse"), "no mice")
+        assert p.no("cat") == "no cats"
+        assert p.no("cat", count=3) == "3 cats"
+        assert p.no("cat", count="three") == "three cats"
+        assert p.no("cat", count=1) == "1 cat"
+        assert p.no("cat", count="one") == "one cat"
+        assert p.no("mouse") == "no mice"
         p.num(3)
-        self.assertEqual(p.no("cat"), "3 cats")
+        assert p.no("cat") == "3 cats"
 
-    def test_prespart(self):
-        p = inflect.engine()
-        for sing, plur in (
+    @pytest.mark.parametrize(
+        'sing, plur',
+        (
             ("runs", "running"),
             ("dies", "dying"),
             ("glues", "gluing"),
             ("eyes", "eying"),
             ("skis", "skiing"),
             ("names", "naming"),
             ("sees", "seeing"),
             ("hammers", "hammering"),
             ("bats", "batting"),
             ("eats", "eating"),
             ("loves", "loving"),
             ("spies", "spying"),
-        ):
-            self.assertEqual(p.present_participle(sing), plur)
-
-        self.assertEqual(p.present_participle("hoes"), "hoeing")
-        self.assertEqual(p.present_participle("alibis"), "alibiing")
-        self.assertEqual(p.present_participle("is"), "being")
-        self.assertEqual(p.present_participle("are"), "being")
-        self.assertEqual(p.present_participle("had"), "having")
-        self.assertEqual(p.present_participle("has"), "having")
-
-    def test_ordinal(self):
-        p = inflect.engine()
-        for num, numord in (
+            ("hoes", "hoeing"),
+            ("alibis", "alibiing"),
+            ("is", "being"),
+            ("are", "being"),
+            ("had", "having"),
+            ("has", "having"),
+        ),
+    )
+    def test_prespart(self, sing, plur):
+        p = inflect.engine()
+        assert p.present_participle(sing) == plur
+
+    @pytest.mark.parametrize(
+        'num, ord',
+        (
             ("1", "1st"),
             ("2", "2nd"),
             ("3", "3rd"),
             ("4", "4th"),
             ("10", "10th"),
             ("28", "28th"),
             ("100", "100th"),
@@ -865,103 +881,103 @@
             ("two", "second"),
             ("four", "fourth"),
             ("twenty", "twentieth"),
             ("one hundered", "one hunderedth"),
             ("one hundered and one", "one hundered and first"),
             ("zero", "zeroth"),
             ("n", "nth"),  # bonus!
-        ):
-            self.assertEqual(p.ordinal(num), numord)
+        ),
+    )
+    def test_ordinal(self, num, ord):
+        p = inflect.engine()
+        assert p.ordinal(num) == ord
 
     def test_millfn(self):
         p = inflect.engine()
         millfn = p.millfn
-        self.assertEqual(millfn(1), " thousand")
-        self.assertEqual(millfn(2), " million")
-        self.assertEqual(millfn(3), " billion")
-        self.assertEqual(millfn(0), " ")
-        self.assertEqual(millfn(11), " decillion")
-        inflect.STDOUT_ON = False
-        self.assertRaises(NumOutOfRangeError, millfn, 12)
-        inflect.STDOUT_ON = True
+        assert millfn(1) == " thousand"
+        assert millfn(2) == " million"
+        assert millfn(3) == " billion"
+        assert millfn(0) == " "
+        assert millfn(11) == " decillion"
+        with pytest.raises(NumOutOfRangeError):
+            millfn(12)
 
     def test_unitfn(self):
         p = inflect.engine()
         unitfn = p.unitfn
-        self.assertEqual(unitfn(1, 2), "one million")
-        self.assertEqual(unitfn(1, 3), "one billion")
-        self.assertEqual(unitfn(5, 3), "five billion")
-        self.assertEqual(unitfn(5, 0), "five ")
-        self.assertEqual(unitfn(0, 0), " ")
+        assert unitfn(1, 2) == "one million"
+        assert unitfn(1, 3) == "one billion"
+        assert unitfn(5, 3) == "five billion"
+        assert unitfn(5, 0) == "five "
+        assert unitfn(0, 0) == " "
 
     def test_tenfn(self):
         p = inflect.engine()
         tenfn = p.tenfn
-        self.assertEqual(tenfn(3, 1, 2), "thirty-one million")
-        self.assertEqual(tenfn(3, 0, 2), "thirty million")
-        self.assertEqual(tenfn(0, 1, 2), "one million")
-        self.assertEqual(tenfn(1, 1, 2), "eleven million")
-        self.assertEqual(tenfn(1, 0, 2), "ten million")
-        self.assertEqual(tenfn(1, 0, 0), "ten ")
-        self.assertEqual(tenfn(0, 0, 0), " ")
+        assert tenfn(3, 1, 2) == "thirty-one million"
+        assert tenfn(3, 0, 2) == "thirty million"
+        assert tenfn(0, 1, 2) == "one million"
+        assert tenfn(1, 1, 2) == "eleven million"
+        assert tenfn(1, 0, 2) == "ten million"
+        assert tenfn(1, 0, 0) == "ten "
+        assert tenfn(0, 0, 0) == " "
 
     def test_hundfn(self):
         p = inflect.engine()
         hundfn = p.hundfn
         p._number_args = dict(andword="and")
-        self.assertEqual(hundfn(4, 3, 1, 2), "four hundred and thirty-one  million, ")
-        self.assertEqual(hundfn(4, 0, 0, 2), "four hundred  million, ")
-        self.assertEqual(hundfn(4, 0, 5, 2), "four hundred and five  million, ")
-        self.assertEqual(hundfn(0, 3, 1, 2), "thirty-one  million, ")
-        self.assertEqual(hundfn(0, 0, 7, 2), "seven  million, ")
+        assert hundfn(4, 3, 1, 2) == "four hundred and thirty-one  million, "
+        assert hundfn(4, 0, 0, 2) == "four hundred  million, "
+        assert hundfn(4, 0, 5, 2) == "four hundred and five  million, "
+        assert hundfn(0, 3, 1, 2) == "thirty-one  million, "
+        assert hundfn(0, 0, 7, 2) == "seven  million, "
 
     def test_enword(self):
         p = inflect.engine()
         enword = p.enword
-        self.assertEqual(enword("5", 1), "five, ")
+        assert enword("5", 1) == "five, "
         p._number_args = dict(zero="zero", one="one", andword="and")
-        self.assertEqual(enword("0", 1), " zero, ")
-        self.assertEqual(enword("1", 1), " one, ")
-        self.assertEqual(enword("347", 1), "three, four, seven, ")
-
-        self.assertEqual(enword("34", 2), "thirty-four , ")
-        self.assertEqual(enword("347", 2), "thirty-four , seven, ")
-        self.assertEqual(enword("34768", 2), "thirty-four , seventy-six , eight, ")
-        self.assertEqual(enword("1", 2), "one, ")
-        p._number_args["one"] = "single"
-        self.TODO(
-            enword("1", 2), "single, ", "one, "
-        )  # TODO: doesn't use default word for 'one' here
-
-        p._number_args["one"] = "one"
-
-        self.assertEqual(enword("134", 3), " one thirty-four , ")
-
-        self.assertEqual(enword("0", -1), "zero")
-        self.assertEqual(enword("1", -1), "one")
-
-        self.assertEqual(enword("3", -1), "three , ")
-        self.assertEqual(enword("12", -1), "twelve , ")
-        self.assertEqual(enword("123", -1), "one hundred and twenty-three  , ")
-        self.assertEqual(
-            enword("1234", -1), "one thousand, two hundred and thirty-four  , "
-        )
-        self.assertEqual(
-            enword("12345", -1), "twelve thousand, three hundred and forty-five  , "
-        )
-        self.assertEqual(
-            enword("123456", -1),
-            "one hundred and twenty-three  thousand, four hundred and fifty-six  , ",
-        )
-        self.assertEqual(
-            enword("1234567", -1),
-            "one million, two hundred and thirty-four  thousand, "
-            "five hundred and sixty-seven  , ",
+        assert enword("0", 1) == " zero, "
+        assert enword("1", 1) == " one, "
+        assert enword("347", 1) == "three, four, seven, "
+
+        assert enword("34", 2) == "thirty-four , "
+        assert enword("347", 2) == "thirty-four , seven, "
+        assert enword("34768", 2) == "thirty-four , seventy-six , eight, "
+        assert enword("1", 2) == "one, "
+
+        assert enword("134", 3) == " one thirty-four , "
+
+        assert enword("0", -1) == "zero"
+        assert enword("1", -1) == "one"
+
+        assert enword("3", -1) == "three , "
+        assert enword("12", -1) == "twelve , "
+        assert enword("123", -1) == "one hundred and twenty-three  , "
+        assert enword("1234", -1) == "one thousand, two hundred and thirty-four  , "
+        assert (
+            enword("12345", -1) == "twelve thousand, three hundred and forty-five  , "
+        )
+        assert (
+            enword("123456", -1)
+            == "one hundred and twenty-three  thousand, four hundred and fifty-six  , "
+        )
+        assert (
+            enword("1234567", -1)
+            == "one million, two hundred and thirty-four  thousand, "
+            "five hundred and sixty-seven  , "
         )
 
+    @pytest.mark.xfail(reason="doesn't use indicated word for 'one'")
+    def test_enword_number_args_override(self):
+        p = inflect.engine()
+        p._number_args["one"] = "single"
+        p.enword("1", 2) == "single, "
+
     def test_numwords(self):
         p = inflect.engine()
         numwords = p.number_to_words
 
         for n, word in (
             ("1", "one"),
             ("10", "ten"),
@@ -972,271 +988,241 @@
             ("1000000", "one million"),
             ("10000000", "ten million"),
             ("+10", "plus ten"),
             ("-10", "minus ten"),
             ("10.", "ten point"),
             (".10", "point one zero"),
         ):
-            self.assertEqual(numwords(n), word)
+            assert numwords(n) == word
 
         for n, word, wrongword in (
             # TODO: should be one point two three
             ("1.23", "one point two three", "one point twenty-three"),
         ):
-            self.assertEqual(numwords(n), word)
+            assert numwords(n) == word
 
         for n, txt in (
             (3, "three bottles of beer on the wall"),
             (2, "two bottles of beer on the wall"),
             (1, "a solitary bottle of beer on the wall"),
             (0, "no more bottles of beer on the wall"),
         ):
-            self.assertEqual(
+            assert (
                 "{}{}".format(
                     numwords(n, one="a solitary", zero="no more"),
                     p.plural(" bottle of beer on the wall", n),
-                ),
-                txt,
+                )
+                == txt
             )
 
-        self.assertEqual(numwords(0, one="one", zero="zero"), "zero")
-
-        self.assertEqual(numwords("1234"), "one thousand, two hundred and thirty-four")
-        self.assertEqual(
-            numwords("1234", wantlist=True),
-            ["one thousand", "two hundred and thirty-four"],
-        )
-        self.assertEqual(
-            numwords("1234567", wantlist=True),
-            [
-                "one million",
-                "two hundred and thirty-four thousand",
-                "five hundred and sixty-seven",
-            ],
-        )
-        self.assertEqual(numwords("+10", wantlist=True), ["plus", "ten"])
-        self.assertEqual(
-            numwords("1234", andword=""), "one thousand, two hundred thirty-four"
-        )
-        self.assertEqual(
-            numwords("1234", andword="plus"),
-            "one thousand, two hundred plus thirty-four",
-        )
-        self.assertEqual(numwords(p.ordinal("21")), "twenty-first")
-        self.assertEqual(numwords("9", threshold=10), "nine")
-        self.assertEqual(numwords("10", threshold=10), "ten")
-        self.assertEqual(numwords("11", threshold=10), "11")
-        self.assertEqual(numwords("1000", threshold=10), "1,000")
-        self.assertEqual(numwords("123", threshold=10), "123")
-        self.assertEqual(numwords("1234", threshold=10), "1,234")
-        self.assertEqual(numwords("1234.5678", threshold=10), "1,234.5678")
-        self.assertEqual(numwords("1", decimal=None), "one")
-        self.assertEqual(
-            numwords("1234.5678", decimal=None),
-            "twelve million, three hundred and forty-five "
-            "thousand, six hundred and seventy-eight",
-        )
+        assert numwords(0, one="one", zero="zero") == "zero"
 
-    def test_numwords_group(self):
+        assert numwords("1234") == "one thousand, two hundred and thirty-four"
+        assert numwords("1234", wantlist=True) == [
+            "one thousand",
+            "two hundred and thirty-four",
+        ]
+        assert numwords("1234567", wantlist=True) == [
+            "one million",
+            "two hundred and thirty-four thousand",
+            "five hundred and sixty-seven",
+        ]
+        assert numwords("+10", wantlist=True) == ["plus", "ten"]
+        assert numwords("1234", andword="") == "one thousand, two hundred thirty-four"
+        assert (
+            numwords("1234", andword="plus")
+            == "one thousand, two hundred plus thirty-four"
+        )
+        assert numwords(p.ordinal("21")) == "twenty-first"
+        assert numwords("9", threshold=10) == "nine"
+        assert numwords("10", threshold=10) == "ten"
+        assert numwords("11", threshold=10) == "11"
+        assert numwords("1000", threshold=10) == "1,000"
+        assert numwords("123", threshold=10) == "123"
+        assert numwords("1234", threshold=10) == "1,234"
+        assert numwords("1234.5678", threshold=10) == "1,234.5678"
+        assert numwords("1", decimal=None) == "one"
+        assert (
+            numwords("1234.5678", decimal=None)
+            == "twelve million, three hundred and forty-five "
+            "thousand, six hundred and seventy-eight"
+        )
+
+    def test_numwords_group_chunking_error(self):
+        p = inflect.engine()
+        with pytest.raises(BadChunkingOptionError):
+            p.number_to_words("1234", group=4)
+
+    @pytest.mark.parametrize(
+        'input,kwargs,expect',
+        (
+            ("12345", dict(group=2), "twelve, thirty-four, five"),
+            ("123456", dict(group=3), "one twenty-three, four fifty-six"),
+            ("12345", dict(group=1), "one, two, three, four, five"),
+            (
+                "1234th",
+                dict(group=0, andword="and"),
+                "one thousand, two hundred and thirty-fourth",
+            ),
+            (
+                "1234th",
+                dict(group=0),
+                "one thousand, two hundred and thirty-fourth",
+            ),
+            ("120", dict(group=2), "twelve, zero"),
+            ("120", dict(group=2, zero="oh", one="unity"), "twelve, oh"),
+            (
+                "555_1202",
+                dict(group=1, zero="oh"),
+                "five, five, five, one, two, oh, two",
+            ),
+            (
+                "555_1202",
+                dict(group=1, one="unity"),
+                "five, five, five, unity, two, zero, two",
+            ),
+            (
+                "123.456",
+                dict(group=1, decimal="mark", one="one"),
+                "one, two, three, mark, four, five, six",
+            ),
+            pytest.param(
+                '12345',
+                dict(group=3),
+                'one hundred and twenty-three',
+                marks=pytest.mark.xfail(reason="'hundred and' missing"),
+            ),
+            pytest.param(
+                '101',
+                dict(group=2, zero="oh", one="unity"),
+                "ten, unity",
+                marks=pytest.mark.xfail(reason="ignoring 'one' param with group=2"),
+            ),
+        ),
+    )
+    def test_numwords_group(self, input, kwargs, expect):
         p = inflect.engine()
-        numwords = p.number_to_words
-        self.assertEqual(numwords("12345", group=2), "twelve, thirty-four, five")
-        # TODO: 'hundred and' missing
-        self.TODO(
-            numwords("12345", group=3),
-            "one hundred and twenty-three",
-            "one twenty-three, forty-five",
-        )
-        self.assertEqual(
-            numwords("123456", group=3), "one twenty-three, four fifty-six"
-        )
-        self.assertEqual(numwords("12345", group=1), "one, two, three, four, five")
-        self.assertEqual(
-            numwords("1234th", group=0, andword="and"),
-            "one thousand, two hundred and thirty-fourth",
-        )
-        self.assertEqual(
-            numwords(p.ordinal("1234"), group=0),
-            "one thousand, two hundred and thirty-fourth",
-        )
-        self.assertEqual(numwords("120", group=2), "twelve, zero")
-        self.assertEqual(numwords("120", group=2, zero="oh", one="unity"), "twelve, oh")
-        # TODO: ignoring 'one' param with group=2
-        self.TODO(
-            numwords("101", group=2, zero="oh", one="unity"), "ten, unity", "ten, one"
-        )
-        self.assertEqual(
-            numwords("555_1202", group=1, zero="oh"),
-            "five, five, five, one, two, oh, two",
-        )
-        self.assertEqual(
-            numwords("555_1202", group=1, one="unity"),
-            "five, five, five, unity, two, zero, two",
-        )
-        self.assertEqual(
-            numwords("123.456", group=1, decimal="mark", one="one"),
-            "one, two, three, mark, four, five, six",
-        )
-
-        inflect.STDOUT_ON = False
-        self.assertRaises(BadChunkingOptionError, numwords, "1234", group=4)
-        inflect.STDOUT_ON = True
+        assert p.number_to_words(input, **kwargs) == expect
 
     def test_wordlist(self):
         p = inflect.engine()
         wordlist = p.join
-        self.assertEqual(wordlist([]), "")
-        self.assertEqual(wordlist(("apple",)), "apple")
-        self.assertEqual(wordlist(("apple", "banana")), "apple and banana")
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot")), "apple, banana, and carrot"
-        )
-        self.assertEqual(
-            wordlist(("apple", "1,000", "carrot")), "apple; 1,000; and carrot"
-        )
-        self.assertEqual(
-            wordlist(("apple", "1,000", "carrot"), sep=","), "apple, 1,000, and carrot"
-        )
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot"), final_sep=""),
-            "apple, banana and carrot",
-        )
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot"), final_sep=";"),
-            "apple, banana; and carrot",
-        )
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot"), conj="or"),
-            "apple, banana, or carrot",
+        assert wordlist([]) == ""
+        assert wordlist(("apple",)) == "apple"
+        assert wordlist(("apple", "banana")) == "apple and banana"
+        assert wordlist(("apple", "banana", "carrot")) == "apple, banana, and carrot"
+        assert wordlist(("apple", "1,000", "carrot")) == "apple; 1,000; and carrot"
+        assert (
+            wordlist(("apple", "1,000", "carrot"), sep=",")
+            == "apple, 1,000, and carrot"
+        )
+        assert (
+            wordlist(("apple", "banana", "carrot"), final_sep="")
+            == "apple, banana and carrot"
+        )
+        assert (
+            wordlist(("apple", "banana", "carrot"), final_sep=";")
+            == "apple, banana; and carrot"
+        )
+        assert (
+            wordlist(("apple", "banana", "carrot"), conj="or")
+            == "apple, banana, or carrot"
+        )
+
+        assert wordlist(("apple", "banana"), conj=" or ") == "apple  or  banana"
+        assert wordlist(("apple", "banana"), conj="&") == "apple & banana"
+        assert (
+            wordlist(("apple", "banana"), conj="&", conj_spaced=False) == "apple&banana"
+        )
+        assert (
+            wordlist(("apple", "banana"), conj="& ", conj_spaced=False)
+            == "apple& banana"
+        )
+
+        assert (
+            wordlist(("apple", "banana", "carrot"), conj=" or ")
+            == "apple, banana,  or  carrot"
+        )
+        assert (
+            wordlist(("apple", "banana", "carrot"), conj="+")
+            == "apple, banana, + carrot"
+        )
+        assert (
+            wordlist(("apple", "banana", "carrot"), conj="&")
+            == "apple, banana, & carrot"
+        )
+        assert (
+            wordlist(("apple", "banana", "carrot"), conj="&", conj_spaced=False)
+            == "apple, banana,&carrot"
+        )
+        assert (
+            wordlist(("apple", "banana", "carrot"), conj=" &", conj_spaced=False)
+            == "apple, banana, &carrot"
         )
 
-        self.assertEqual(
-            wordlist(("apple", "banana"), conj=" or "), "apple  or  banana"
-        )
-        self.assertEqual(
-            wordlist(("apple", "banana"), conj="&"), "apple & banana"
-        )  # TODO: want spaces here. Done, report upstream
-        self.assertEqual(
-            wordlist(("apple", "banana"), conj="&", conj_spaced=False), "apple&banana"
-        )
-        self.assertEqual(
-            wordlist(("apple", "banana"), conj="& ", conj_spaced=False), "apple& banana"
-        )
-
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot"), conj=" or "),
-            "apple, banana,  or  carrot",
-        )
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot"), conj="+"), "apple, banana, + carrot"
-        )
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot"), conj="&"), "apple, banana, & carrot"
-        )  # TODO: want space here. Done, report upstream
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot"), conj="&", conj_spaced=False),
-            "apple, banana,&carrot",
-        )  # TODO: want space here. Done, report upstream
-        self.assertEqual(
-            wordlist(("apple", "banana", "carrot"), conj=" &", conj_spaced=False),
-            "apple, banana, &carrot",
-        )  # TODO: want space here. Done, report upstream
-
-    def test_print(self):
-        inflect.STDOUT_ON = True
-        inflect.print3("")  # make sure it doesn't crash
-        inflect.STDOUT_ON = False
-
     def test_doc_examples(self):
         p = inflect.engine()
-        self.assertEqual(p.plural_noun("I"), "we")
-        self.assertEqual(p.plural_verb("saw"), "saw")
-        self.assertEqual(p.plural_adj("my"), "our")
-        self.assertEqual(p.plural_noun("saw"), "saws")
-        self.assertEqual(p.plural("was"), "were")
-        self.assertEqual(p.plural("was", 1), "was")
-        self.assertEqual(p.plural_verb("was", 2), "were")
-        self.assertEqual(p.plural_verb("was"), "were")
-        self.assertEqual(p.plural_verb("was", 1), "was")
+        assert p.plural_noun("I") == "we"
+        assert p.plural_verb("saw") == "saw"
+        assert p.plural_adj("my") == "our"
+        assert p.plural_noun("saw") == "saws"
+        assert p.plural("was") == "were"
+        assert p.plural("was", 1) == "was"
+        assert p.plural_verb("was", 2) == "were"
+        assert p.plural_verb("was") == "were"
+        assert p.plural_verb("was", 1) == "was"
 
         for errors, txt in (
             (0, "There were no errors"),
             (1, "There was 1 error"),
             (2, "There were 2 errors"),
         ):
-            self.assertEqual(
+            assert (
                 "There {}{}".format(
                     p.plural_verb("was", errors), p.no(" error", errors)
-                ),
-                txt,
+                )
+                == txt
             )
 
-            self.assertEqual(
+            assert (
                 p.inflect(
                     "There plural_verb('was',%d) no('error',%d)" % (errors, errors)
-                ),
-                txt,
+                )
+                == txt
             )
 
         for num1, num2, txt in ((1, 2, "I saw 2 saws"), (2, 1, "we saw 1 saw")):
-            self.assertEqual(
+            assert (
                 "{}{}{} {}{}".format(
                     p.num(num1, ""),
                     p.plural("I"),
                     p.plural_verb(" saw"),
                     p.num(num2),
                     p.plural_noun(" saw"),
-                ),
-                txt,
+                )
+                == txt
             )
 
-            self.assertEqual(
+            assert (
                 p.inflect(
                     "num(%d, False)plural('I') plural_verb('saw') "
                     "num(%d) plural_noun('saw')" % (num1, num2)
-                ),
-                txt,
+                )
+                == txt
             )
 
-        self.assertEqual(p.a("a cat"), "a cat")
+        assert p.a("a cat") == "a cat"
 
         for word, txt in (
             ("cat", "a cat"),
             ("aardvark", "an aardvark"),
             ("ewe", "a ewe"),
             ("hour", "an hour"),
         ):
-            self.assertEqual(
-                p.a("{} {}".format(p.number_to_words(1, one="a"), word)), txt
-            )
+            assert p.a("{} {}".format(p.number_to_words(1, one="a"), word)) == txt
 
         p.num(2)
 
-    def test_deprecation(self):
-        p = inflect.engine()
-        for meth in (
-            "pl",
-            "plnoun",
-            "plverb",
-            "pladj",
-            "sinoun",
-            "prespart",
-            "numwords",
-            "plequal",
-            "plnounequal",
-            "plverbequal",
-            "pladjequal",
-            "wordlist",
-        ):
-            self.assertRaises(DeprecationWarning, getattr, p, meth)
-
     def test_unknown_method(self):
         p = inflect.engine()
-        with self.assertRaises(AttributeError):
+        with pytest.raises(AttributeError):
             p.unknown_method
-
-
-if __name__ == "__main__":
-    try:
-        unittest.main()
-    except SystemExit:
-        pass
```

### Comparing `inflect-6.2.0/tox.ini` & `inflect-7.0.0/tox.ini`

 * *Files identical despite different names*

