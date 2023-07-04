# Comparing `tmp/botocore-a-la-carte-comprehendmedical-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-comprehendmedical-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-comprehendmedical-1.29.99.tar", last modified: Sat Mar 25 01:22:27 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-comprehendmedical-1.30.0.tar", last modified: Tue Jul  4 01:44:18 2023, max compression
```

## Comparing `botocore-a-la-carte-comprehendmedical-1.29.99.tar` & `botocore-a-la-carte-comprehendmedical-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.498616 botocore-a-la-carte-comprehendmedical-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:27.000000 botocore-a-la-carte-comprehendmedical-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-25 01:22:27.498616 botocore-a-la-carte-comprehendmedical-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.498616 botocore-a-la-carte-comprehendmedical-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.498616 botocore-a-la-carte-comprehendmedical-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.498616 botocore-a-la-carte-comprehendmedical-1.29.99/botocore/data/comprehendmedical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.498616 botocore-a-la-carte-comprehendmedical-1.29.99/botocore/data/comprehendmedical/2018-10-30/
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-03-25 01:22:12.000000 botocore-a-la-carte-comprehendmedical-1.29.99/botocore/data/comprehendmedical/2018-10-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-comprehendmedical-1.29.99/botocore/data/comprehendmedical/2018-10-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-25 01:22:12.000000 botocore-a-la-carte-comprehendmedical-1.29.99/botocore/data/comprehendmedical/2018-10-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    92480 2023-03-25 01:22:12.000000 botocore-a-la-carte-comprehendmedical-1.29.99/botocore/data/comprehendmedical/2018-10-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.498616 botocore-a-la-carte-comprehendmedical-1.29.99/botocore_a_la_carte_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-25 01:22:27.000000 botocore-a-la-carte-comprehendmedical-1.29.99/botocore_a_la_carte_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-25 01:22:27.000000 botocore-a-la-carte-comprehendmedical-1.29.99/botocore_a_la_carte_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:27.000000 botocore-a-la-carte-comprehendmedical-1.29.99/botocore_a_la_carte_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:27.000000 botocore-a-la-carte-comprehendmedical-1.29.99/botocore_a_la_carte_comprehendmedical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:27.498616 botocore-a-la-carte-comprehendmedical-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-25 01:22:27.000000 botocore-a-la-carte-comprehendmedical-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.310422 botocore-a-la-carte-comprehendmedical-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:18.000000 botocore-a-la-carte-comprehendmedical-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 01:44:18.310422 botocore-a-la-carte-comprehendmedical-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.310422 botocore-a-la-carte-comprehendmedical-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.310422 botocore-a-la-carte-comprehendmedical-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.310422 botocore-a-la-carte-comprehendmedical-1.30.0/botocore/data/comprehendmedical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.310422 botocore-a-la-carte-comprehendmedical-1.30.0/botocore/data/comprehendmedical/2018-10-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-07-04 01:44:02.000000 botocore-a-la-carte-comprehendmedical-1.30.0/botocore/data/comprehendmedical/2018-10-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-comprehendmedical-1.30.0/botocore/data/comprehendmedical/2018-10-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-comprehendmedical-1.30.0/botocore/data/comprehendmedical/2018-10-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    92596 2023-07-04 01:44:02.000000 botocore-a-la-carte-comprehendmedical-1.30.0/botocore/data/comprehendmedical/2018-10-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.310422 botocore-a-la-carte-comprehendmedical-1.30.0/botocore_a_la_carte_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 01:44:18.000000 botocore-a-la-carte-comprehendmedical-1.30.0/botocore_a_la_carte_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-04 01:44:18.000000 botocore-a-la-carte-comprehendmedical-1.30.0/botocore_a_la_carte_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:18.000000 botocore-a-la-carte-comprehendmedical-1.30.0/botocore_a_la_carte_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:18.000000 botocore-a-la-carte-comprehendmedical-1.30.0/botocore_a_la_carte_comprehendmedical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:18.310422 botocore-a-la-carte-comprehendmedical-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-04 01:44:18.000000 botocore-a-la-carte-comprehendmedical-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-comprehendmedical-1.29.99/LICENSE.txt` & `botocore-a-la-carte-comprehendmedical-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-comprehendmedical-1.29.99/PKG-INFO` & `botocore-a-la-carte-comprehendmedical-1.30.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-comprehendmedical
-Version: 1.29.99
+Version: 1.30.0
 Summary: comprehendmedical data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-comprehendmedical-1.29.99/botocore/data/comprehendmedical/2018-10-30/service-2.json` & `botocore-a-la-carte-comprehendmedical-1.30.0/botocore/data/comprehendmedical/2018-10-30/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999901920995671%*

 * *Differences: {"'shapes'": "{'ICD10CMRelationshipType': {'enum': {insert: [(2, 'QUALITY')]}}, "*

 * *             "'RelationshipType': {'enum': {insert: [(20, 'USAGE'), (21, 'QUALITY')]}}, "*

 * *             "'RxNormTraitName': {'enum': {insert: [(1, 'PAST_HISTORY')]}}, "*

 * *             "'SNOMEDCTRelationshipType': {'enum': {insert: [(6, 'TEST_UNIT')]}}}"}*

```diff
@@ -1426,15 +1426,16 @@
                 "TIME_EXPRESSION"
             ],
             "type": "string"
         },
         "ICD10CMRelationshipType": {
             "enum": [
                 "OVERLAP",
-                "SYSTEM_ORGAN_SITE"
+                "SYSTEM_ORGAN_SITE",
+                "QUALITY"
             ],
             "type": "string"
         },
         "ICD10CMTrait": {
             "documentation": "<p>Contextual information for the entity. The traits recognized by InferICD10CM are <code>DIAGNOSIS</code>, <code>SIGN</code>, <code>SYMPTOM</code>, and <code>NEGATION</code>.</p>",
             "members": {
                 "Name": {
@@ -1864,15 +1865,17 @@
                 "RATE",
                 "ACUITY",
                 "TEST_VALUE",
                 "TEST_UNITS",
                 "TEST_UNIT",
                 "DIRECTION",
                 "SYSTEM_ORGAN_SITE",
-                "AMOUNT"
+                "AMOUNT",
+                "USAGE",
+                "QUALITY"
             ],
             "type": "string"
         },
         "ResourceNotFoundException": {
             "documentation": "<p>The resource identified by the specified Amazon Resource Name (ARN) was not found. Check the ARN and try your request again.</p>",
             "exception": true,
             "members": {
@@ -2045,15 +2048,16 @@
             "member": {
                 "shape": "RxNormTrait"
             },
             "type": "list"
         },
         "RxNormTraitName": {
             "enum": [
-                "NEGATION"
+                "NEGATION",
+                "PAST_HISTORY"
             ],
             "type": "string"
         },
         "S3Bucket": {
             "max": 63,
             "min": 3,
             "pattern": "^[0-9a-z\\.\\-_]*(?!\\.)$",
@@ -2245,15 +2249,16 @@
         "SNOMEDCTRelationshipType": {
             "enum": [
                 "ACUITY",
                 "QUALITY",
                 "TEST_VALUE",
                 "TEST_UNITS",
                 "DIRECTION",
-                "SYSTEM_ORGAN_SITE"
+                "SYSTEM_ORGAN_SITE",
+                "TEST_UNIT"
             ],
             "type": "string"
         },
         "SNOMEDCTTrait": {
             "documentation": "<p> Contextual information for an entity. </p>",
             "members": {
                 "Name": {
```

### Comparing `botocore-a-la-carte-comprehendmedical-1.29.99/botocore_a_la_carte_comprehendmedical.egg-info/PKG-INFO` & `botocore-a-la-carte-comprehendmedical-1.30.0/botocore_a_la_carte_comprehendmedical.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-comprehendmedical
-Version: 1.29.99
+Version: 1.30.0
 Summary: comprehendmedical data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-comprehendmedical-1.29.99/setup.py` & `botocore-a-la-carte-comprehendmedical-1.30.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-comprehendmedical',
-    version="1.29.99",
+    version="1.30.0",
     description='comprehendmedical data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/comprehendmedical/*/*.json'],
```

