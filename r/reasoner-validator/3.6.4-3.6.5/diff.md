# Comparing `tmp/reasoner_validator-3.6.4.tar.gz` & `tmp/reasoner_validator-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.6.4.tar", max compression
+gzip compressed data, was "reasoner_validator-3.6.5.tar", max compression
```

## Comparing `reasoner_validator-3.6.4.tar` & `reasoner_validator-3.6.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/LICENSE
--rw-r--r--   0        0        0    12620 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/README.md
--rw-r--r--   0        0        0      131 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/conf.py
--rw-r--r--   0        0        0    19640 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/make.bat
--rw-r--r--   0        0        0      136 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    35958 2023-07-01 19:53:22.994430 reasoner_validator-3.6.4/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2092 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/pyproject.toml
--rw-r--r--   0        0        0    38373 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    63014 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39199 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    28625 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4592 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     9721 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14009 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    10707 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      398 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/conftest.py
--rw-r--r--   0        0        0   114356 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62095 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml
--rw-r--r--   0        0        0    34174 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_response_validator.py
--rw-r--r--   0        0        0     5508 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_semver.py
--rw-r--r--   0        0        0     1886 2023-07-01 19:53:22.998430 reasoner_validator-3.6.4/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26525 2023-07-01 19:53:23.002430 reasoner_validator-3.6.4/tests/test_validate.py
--rw-r--r--   0        0        0    20333 2023-07-01 19:53:23.002430 reasoner_validator-3.6.4/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-07-01 19:53:23.002430 reasoner_validator-3.6.4/tests/test_workflows.py
--rw-r--r--   0        0        0    14658 1970-01-01 00:00:00.000000 reasoner_validator-3.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/LICENSE
+-rw-r--r--   0        0        0    12620 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/README.md
+-rw-r--r--   0        0        0      131 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/conf.py
+-rw-r--r--   0        0        0    19640 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    35958 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2092 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/pyproject.toml
+-rw-r--r--   0        0        0    38413 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    63014 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39199 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    28625 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4592 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    10750 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14019 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    10707 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      410 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/tests/conftest.py
+-rw-r--r--   0        0        0   114356 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62106 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    38591 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_response_validator.py
+-rw-r--r--   0        0        0     5528 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_semver.py
+-rw-r--r--   0        0        0     1913 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26525 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_validate.py
+-rw-r--r--   0        0        0    20333 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_workflows.py
+-rw-r--r--   0        0        0    14658 1970-01-01 00:00:00.000000 reasoner_validator-3.6.5/PKG-INFO
```

### Comparing `reasoner_validator-3.6.4/LICENSE` & `reasoner_validator-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/README.md` & `reasoner_validator-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/docs/Makefile` & `reasoner_validator-3.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/docs/conf.py` & `reasoner_validator-3.6.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/docs/index.rst` & `reasoner_validator-3.6.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/docs/make.bat` & `reasoner_validator-3.6.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/docs/validation_codes_dictionary.md` & `reasoner_validator-3.6.5/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/pyproject.toml` & `reasoner_validator-3.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.6.4"
+version = "3.6.5"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.6.4/reasoner_validator/__init__.py` & `reasoner_validator-3.6.5/reasoner_validator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,17 @@
                     continue
                 for source in edge['sources']:
                     if 'source_record_urls' not in source or source['source_record_urls'] is None:
                         source['source_record_urls'] = list()
                     if 'upstream_resource_ids' not in source or source['upstream_resource_ids'] is None:
                         source['upstream_resource_ids'] = list()
 
-        # 'auxiliary_graphs' (from TRAPI 1.4.0-beta3 onwards)
-        # ought to be nullable, however... not specified that way (yet)
-        if current_version >= self.TRAPI_1_4_0_BETA3 and \
+        # 'auxiliary_graphs' (introduced the TRAPI 1.4.0-beta3 pre-releases,
+        # full updated in the full 1.4.0 release) ought to be nullable
+        if self.TRAPI_1_4_0_BETA4 >= current_version >= self.TRAPI_1_4_0_BETA3 and \
                 ('auxiliary_graphs' not in response['message'] or response['message']['auxiliary_graphs'] is None):
             response['message']['auxiliary_graphs'] = dict()
 
         if 'workflow' in response and response['workflow']:
             # a 'workflow' is a list of steps, which are JSON object specifications
             workflow_steps: List[Dict] = response['workflow']
             for step in workflow_steps:
```

### Comparing `reasoner_validator-3.6.4/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.6.5/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/reasoner_validator/codes.yaml` & `reasoner_validator-3.6.5/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/reasoner_validator/report.py` & `reasoner_validator-3.6.5/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/reasoner_validator/sri/util.py` & `reasoner_validator-3.6.5/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.6.5/reasoner_validator/trapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TRAPI Validation Functions."""
 from json import dumps
-from typing import Optional, Dict
+from typing import Optional, Dict, List
 from os.path import isfile
 import copy
 from functools import lru_cache
 
 import jsonschema
 import requests
 
@@ -145,44 +145,72 @@
             key: schema.pop(key)
             for key in list(schema.keys())
         },
         {"type": "null"},
     ]
 
 
-def openapi_to_jsonschema(schema, version: str) -> None:
-    """
-    Convert OpenAPI schema to JSON schema.
-    :param schema: Dict, in-memory representation of the OpenAPI schema to be validated.
-    :param version: str, TRAPI version against which the schema is currently being validated.
-    :return:
-    """
+TRAPI_1_4_0_BETA = SemVer.from_string("1.4.0-beta")
+TRAPI_1_4_0_BETA3 = SemVer.from_string("1.4.0-beta3")
+TRAPI_1_4_0_BETA4 = SemVer.from_string("1.4.0-beta4")
+TRAPI_1_4_0 = SemVer.from_string("1.4.0")
+
 
+def map_semver(version: str):
     mapped_semver: Optional[SemVer]
     try:
         mapped_semver = SemVer.from_string(version)
     except SemVerError as sve:
         # if we cannot map the version, then it may simply
         # be a non-versioned branch of the schemata
         logger.error(str(sve))
         mapped_semver = None
+    return mapped_semver
+
+
+def patch_schema(tag: str, schema: Dict, version: str):
+    # temporary patch for small TRAPI schema bugs
+    # TODO: fix TRAPI schemata to eliminate these
+    mapped_semver: Optional[SemVer] = map_semver(version)
+    if (
+            mapped_semver and
+            (TRAPI_1_4_0 >= mapped_semver >= TRAPI_1_4_0_BETA3)
+    ):
+        if tag == "auxiliary_graphs" and "oneOf" in schema:
+            # TODO: very short term workaround for problematics 'auxiliary_graphs' value schema
+            schema["type"] = "object"
+            value_types: List[str] = schema.pop("oneOf")
+            schema["additionalProperties"] = value_types[0]
+
+
+def openapi_to_jsonschema(schema, version: str) -> None:
+    """
+    Convert OpenAPI schema to JSON schema.
+    :param schema: Dict, in-memory representation of the OpenAPI schema to be validated.
+    :param version: str, TRAPI version against which the schema is currently being validated.
+    :return:
+    """
+    mapped_semver: Optional[SemVer] = map_semver(version)
 
     # we'll only tweak mapped schemata and
     # such releases that are prior to TRAPI 1.4.0-beta
-    if (mapped_semver and not (mapped_semver >= SemVer.from_string("1.4.0-beta"))) \
-            and "allOf" in schema:
+    if (
+            mapped_semver and
+            not (TRAPI_1_4_0_BETA4 >= mapped_semver >= TRAPI_1_4_0_BETA)
+    ) and "allOf" in schema:
         # September 1, 2022 hacky patch to rewrite 'allOf'
         # tagged schemata, in TRAPI 1.3.0 or earlier, to 'oneOf'
         schema["oneOf"] = schema.pop("allOf")
 
     if schema.get("type", None) == "object":
         for tag, prop in schema.get("properties", dict()).items():
+            patch_schema(tag, prop, version)
             openapi_to_jsonschema(prop, version=version)
 
-    if schema.get("type", None) == "array":
+    elif schema.get("type", None) == "array":
         openapi_to_jsonschema(schema.get("items", dict()), version=version)
 
     if schema.pop("nullable", False):
         fix_nullable(schema)
 
 
 class TRAPISchemaValidator(ValidationReporter):
```

### Comparing `reasoner_validator-3.6.4/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.6.5/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/reasoner_validator/validation_codes.py` & `reasoner_validator-3.6.5/reasoner_validator/validation_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 logger = logging.getLogger(__name__)
 
 DEFAULT_CODES_DOCUMENTATION_FILE = abspath(join(dirname(__file__), "..", "docs", "validation_codes_dictionary.md"))
 
 
 class CodeDictionary:
 
-    CODE_DICTIONARY: str = abspath(join(dirname(__file__), "codes.yaml"))
+    CODE_DICTIONARY_FILE: str = abspath(join(dirname(__file__), "codes.yaml"))
 
     MESSAGE = "$message"
     CONTEXT = "$context"
     DESCRIPTION = "$description"
 
     code_dictionary: Optional[Dict] = None
 
     @classmethod
     def _get_code_dictionary(cls) -> Dict:
         if not cls.code_dictionary:
             # Open the file and load the file
-            with open(cls.CODE_DICTIONARY, mode='r') as f:
+            with open(cls.CODE_DICTIONARY_FILE, mode='r') as f:
                 cls.code_dictionary = load(f, Loader=BaseLoader)
         return cls.code_dictionary
 
     @classmethod
     def filter_copy_by_facet(cls, tree: Dict, facet: str) -> Dict:
         """
         Copy subtree, filtering out leaf data by specified facet. Leaves are simply identified by
```

### Comparing `reasoner_validator-3.6.4/reasoner_validator/versioning.py` & `reasoner_validator-3.6.5/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.6.5/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml` & `reasoner_validator-3.6.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -504,14 +504,15 @@
           type: object
           description: >-
             Dictionary of AuxiliaryGraph instances that are used by Knowledge
             Graph Edges and Result Analyses. These are referenced elsewhere by
             the dictionary key.
           additionalProperties:
             $ref: '#components/schemas/AuxiliaryGraph'
+          nullable: true
       additionalProperties: false
     LogEntry:
       description: >-
         The LogEntry object contains information useful for tracing
         and debugging across Translator components.  Although an
         individual component (for example, an ARA or KP) may have its
         own logging and debugging infrastructure, this internal
@@ -561,16 +562,15 @@
         - DEBUG
     Result:
       type: object
       description: >-
         A Result object specifies the nodes and edges in the knowledge graph
         that satisfy the structure or conditions of a user-submitted query
         graph. It must contain a NodeBindings object (list of query graph node
-        to knowledge graph node mappings) and an EdgeBindings object (list of
-        query graph edge to knowledge graph edge mappings).
+        to knowledge graph node mappings) and a list of Analysis objects.
       properties:
         node_bindings:
           type: object
           description: >-
             The dictionary of Input Query Graph to Result Knowledge Graph node
             bindings where the dictionary keys are the key identifiers of the
             Query Graph nodes and the associated values of those keys are
@@ -1486,28 +1486,30 @@
           description: >-
             The role played by the InformationResource in serving as a
             source for an Edge. Note that a given Edge should have one
             and only one 'primary' source, and may have any number of
             'aggregator' or 'supporting data' sources.
         upstream_resource_ids:
           type: array
+          nullable: true
           items:
             $ref: '#/components/schemas/CURIE'
           description: >-
             An upstream InformationResource from which the resource
             being described directly retrieved a record of the knowledge
             expressed in the Edge, or data used to generate this knowledge.
             This is an array because there are cases where a merged Edge
             holds knowledge that was retrieved from multiple sources. e.g.
             an Edge provided by the ARAGORN ARA can expressing knowledge it
             retrieved from both the automat-mychem-info and molepro KPs,
             which both provided it with records of this single fact.
           example: [infores:automat-mychem-info, infores:molepro]
         source_record_urls:
           type: array
+          nullable: true
           items:
             type: string
           description: >-
             A URL linking to a specific web page or document provided by the 
             source, that contains a record of the knowledge expressed in the 
             Edge. If the knowledge is contained in more than one web page on 
             an Information Resource's site, urls MAY be provided for each.
```

### Comparing `reasoner_validator-3.6.4/tests/test_response_validator.py` & `reasoner_validator-3.6.5/tests/test_response_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 from typing import Tuple,  Dict
 from sys import stderr
 
 import logging
 
 from json import dump
 
+from copy import deepcopy
+
 import pytest
 
 from reasoner_validator import TRAPIResponseValidator
+
+from tests import PATCHED_140_SCHEMA_FILEPATH
 from tests.test_validation_report import check_messages
 
+
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
 PRE_TRAPI_1_4_0 = "1.3.0"
+TRAPI_1_4_0 = "1.4.0"
 
 _TEST_QG_1 = {
     "nodes": {
         "type-2 diabetes": {"ids": ["MONDO:0005148"]},
         "drug": {
             "categories": ["biolink:Drug"]
         }
@@ -93,15 +99,15 @@
     'edges': _TEST_EDGES_1
 }
 
 _TEST_RESULTS_1 = [
         {
             "node_bindings": {
                 "type-2 diabetes": [{"id": "MONDO:0005148"}],
-                "drug": [{"id": "CHEBI:6801"}]
+                "drug": [{"id": "ncats.drug:9100L32L2N"}]
             },
             "edge_bindings": {
                 "treats": [{"id": "df87ff82"}]
             }
         }
     ]
 
@@ -221,14 +227,79 @@
 
 
 _TEST_KG_4 = {
     'nodes': _TEST_NODES_1,
     'edges': _TEST_EDGES_4
 }
 
+# From Implementation Guidlines circa June 2023
+_TEST_TRAPI_1_4_0_FULL_SAMPLE = {
+    "message": {
+        "query_graph": {
+            "nodes": {
+                "type-2 diabetes": {"ids": ["MONDO:0005148"]},
+                "drug": {"categories": ["biolink:Drug"]}
+            },
+            "edges": {
+                "treats": {"subject": "drug", "predicates": ["biolink:treats"],
+                           "object": "type-2 diabetes"}
+            }
+        },
+        "knowledge_graph": {
+            "nodes": {
+                "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
+                "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
+            },
+            "edges": {
+                "df87ff82": {"subject": "ncats.drug:9100L32L2N", "predicate": "biolink:treats",
+                             "object": "MONDO:0005148", "sources": [
+                        {"resource_id": "infores:molepro",
+                         "resource_role": "primary_knowledge_source"}]}
+            }
+        },
+        "auxiliary_graphs": {
+            "a0": {
+                "edges": [
+                    "e02",
+                    "e12"
+                ]
+            },
+            "a1": {
+                "edges": [
+                    "extra_edge0"
+                ]
+            },
+            "a2": {
+                "edges": [
+                    "extra_edge1"
+                ]
+            }
+        },
+        "results": [
+            {
+                "node_bindings": {
+                    "type-2 diabetes": [{"id": "MONDO:0005148"}],
+                    "drug": [{"id": "ncats.drug:9100L32L2N"}]
+                },
+                "analyses": [
+                    {
+                        "resource_id": "infores:ara0",
+                        "edge_bindings": {"treats": [{"id": "df87ff82"}]},
+                        "support_graphs": [],
+                        "score": 0.7
+                    }
+                ]
+            }
+        ]
+    }
+}
+
+_TEST_TRAPI_1_4_0_FULL_SAMPLE_WITHOUT_AUX_GRAPH = deepcopy(_TEST_TRAPI_1_4_0_FULL_SAMPLE)
+_TEST_TRAPI_1_4_0_FULL_SAMPLE_WITHOUT_AUX_GRAPH["message"].pop("auxiliary_graphs")
+
 
 @pytest.mark.parametrize(
     "query",
     [
         (   # Query 0 - No 'workflow' key in TRAPI Response
             {
                 'message': {}
@@ -897,14 +968,23 @@
                 ]
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             ""   # this filtered workflow spec should pass
+        ),
+        (   # Query 26 - We throw a full TRAPI JSON example here (taken directly from the
+            #            TRAPI implementation guidelines...) just for fun and profit
+            _TEST_TRAPI_1_4_0_FULL_SAMPLE,
+            TRAPI_1_4_0,
+            None,
+            None,
+            True,
+            ""   # this filtered workflow spec should pass
         )
     ]
 )
 def test_check_biolink_model_compliance_of_trapi_response(query: Tuple):
     validator: TRAPIResponseValidator = TRAPIResponseValidator(
         trapi_version=query[1],
         biolink_version=query[2],
@@ -1016,14 +1096,59 @@
                 }
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             False,
             ""
+        ),
+        (
+            # Query 7 - Full fake sample Response from TRAPI 1.4.0 implementation guidelines
+            _TEST_TRAPI_1_4_0_FULL_SAMPLE,
+            # 25 June 2023 1.4.0 trapi_version with
+            # defective auxiliary_graphs schema model
+            # now temporarily patched?
+            TRAPI_1_4_0,
+            None,
+            None,
+            False,
+            ""  # would be a "critical.trapi.validation" if the schema was unpatched
+        ),
+        (
+            # Query 8 - Full fake sample Response from TRAPI 1.4.0 implementation guidelines
+            _TEST_TRAPI_1_4_0_FULL_SAMPLE,
+            # patched 1.4.0 test schema - fixed critical
+            # TRAPI schema parsing error with auxiliary_graphs
+            PATCHED_140_SCHEMA_FILEPATH,
+            None,
+            None,
+            False,
+            ""
+        ),
+        (
+            # Query 9 - Sample Response from TRAPI 1.4.0 implementation guidelines without auxiliary_graph
+            _TEST_TRAPI_1_4_0_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
+            # 25 June 2023 1.4.0 trapi_version with
+            # defective auxiliary_graphs schema model
+            TRAPI_1_4_0,
+            None,
+            None,
+            False,
+            ""  # nullable: true allows this outcome
+        ),
+        (
+            # Query 10 - Sample Response from TRAPI 1.4.0 implementation guidelines without auxiliary_graph
+            _TEST_TRAPI_1_4_0_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
+            # patched 1.4.0 test schema - fixed critical
+            # TRAPI schema parsing error with auxiliary_graphs
+            PATCHED_140_SCHEMA_FILEPATH,
+            None,
+            None,
+            False,
+            ""  # should still work if nullable: true
         )
     ]
 )
 def test_check_biolink_model_compliance_of_trapi_response_suppressing_empty_data_warnings(
         response, trapi_version, biolink_version, sources, strict_validation, code
 ):
     validator: TRAPIResponseValidator = TRAPIResponseValidator(
```

### Comparing `reasoner_validator-3.6.4/tests/test_semver.py` & `reasoner_validator-3.6.5/tests/test_semver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test semantic version handling."""
 import pytest
 
-from tests import SAMPLE_SCHEMA_FILE, SAMPLE_SCHEMA_VERSION
+from tests import PATCHED_SCHEMA_VERSION, PATCHED_140_SCHEMA_FILEPATH
 from reasoner_validator.versioning import semver_pattern, SemVer, SemVerUnderspecified
 
 
 def test_regex_pattern():
     # test the semver pattern directly
     assert semver_pattern.fullmatch("1.2.3")
     assert semver_pattern.fullmatch("1.2")
@@ -143,15 +143,15 @@
     assert one_four_zero_beta_one != one_four_zero
     assert one_four_zero_beta_one != one_four_zero_beta_four
 
     # pruned SemVer comparisons
     assert not one_four_zero != one_four_one_beta_pruned
 
 
-sample_schema_version = SemVer.from_string(SAMPLE_SCHEMA_VERSION)
-sample_schema_file_semver = SemVer.from_string(SAMPLE_SCHEMA_FILE)
+sample_schema_version = SemVer.from_string(PATCHED_SCHEMA_VERSION)
+sample_schema_file_semver = SemVer.from_string(PATCHED_140_SCHEMA_FILEPATH)
 
 
 def test_schema_file_versioning():
 
     # Sample schema file has internal version type
     assert sample_schema_file_semver == sample_schema_version
```

### Comparing `reasoner_validator-3.6.4/tests/test_trapi_versioning.py` & `reasoner_validator-3.6.5/tests/test_trapi_versioning.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test TRAPI version handling."""
 from typing import Dict
 
 import pytest
 
 from reasoner_validator.versioning import get_latest_version
 from reasoner_validator.trapi import load_schema, TRAPIAccessError
-from tests import SAMPLE_SCHEMA_FILE, LATEST_TRAPI_VERSION
+from tests import PATCHED_140_SCHEMA_FILEPATH, LATEST_TRAPI_VERSION
 
 
 def test_semver_spec_trapi_version():
     trapi_version: str = get_latest_version(release_tag="1")
     assert trapi_version == LATEST_TRAPI_VERSION
 
 
@@ -25,15 +25,15 @@
 
 def test_semver_spec_trapi_version_without_prefix():
     trapi_version: str = get_latest_version(release_tag=LATEST_TRAPI_VERSION[1:])
     assert trapi_version == LATEST_TRAPI_VERSION
 
 
 def test_schema_spec_trapi_version():
-    trapi_version = get_latest_version(release_tag=SAMPLE_SCHEMA_FILE)
+    trapi_version = get_latest_version(release_tag=PATCHED_140_SCHEMA_FILEPATH)
     assert trapi_version is not None
     assert trapi_version.endswith(".yaml")
 
 
 def test_load_schema_with_semver_trapi_version():
     trapi_version: str = get_latest_version(release_tag="1")
     schema: Dict = load_schema(trapi_version)
@@ -45,13 +45,13 @@
     schema: Dict = load_schema(trapi_version)
     assert schema
     with pytest.raises(ValueError):
         load_schema(target="not-a-branch-name")
 
 
 def test_load_schema_with_schema_trapi_version():
-    trapi_version: str = get_latest_version(release_tag=SAMPLE_SCHEMA_FILE)
+    trapi_version: str = get_latest_version(release_tag=PATCHED_140_SCHEMA_FILEPATH)
     assert trapi_version is not None
     schema: Dict = load_schema(trapi_version)
     assert schema
     with pytest.raises(TRAPIAccessError):
         load_schema(target="not-a-trapi-schema.yaml")
```

### Comparing `reasoner_validator-3.6.4/tests/test_validate.py` & `reasoner_validator-3.6.5/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/tests/test_validation_report.py` & `reasoner_validator-3.6.5/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/tests/test_workflows.py` & `reasoner_validator-3.6.5/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.4/PKG-INFO` & `reasoner_validator-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.6.4
+Version: 3.6.5
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

