# Comparing `tmp/botocore-a-la-carte-codeguru-reviewer-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-codeguru-reviewer-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-codeguru-reviewer-1.29.99.tar", last modified: Sat Mar 25 01:22:24 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-codeguru-reviewer-1.30.0.tar", last modified: Tue Jul  4 01:44:14 2023, max compression
```

## Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99.tar` & `botocore-a-la-carte-codeguru-reviewer-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:24.114393 botocore-a-la-carte-codeguru-reviewer-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:23.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-25 01:22:24.114393 botocore-a-la-carte-codeguru-reviewer-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:24.110393 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:24.110393 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:24.110393 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:24.114393 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-03-25 01:22:12.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-25 01:22:12.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    90782 2023-03-25 01:22:12.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-25 01:22:12.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:24.114393 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore_a_la_carte_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-25 01:22:24.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore_a_la_carte_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-25 01:22:24.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore_a_la_carte_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:24.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore_a_la_carte_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:24.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore_a_la_carte_codeguru_reviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:24.114393 botocore-a-la-carte-codeguru-reviewer-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-25 01:22:23.000000 botocore-a-la-carte-codeguru-reviewer-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.478388 botocore-a-la-carte-codeguru-reviewer-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:14.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 01:44:14.478388 botocore-a-la-carte-codeguru-reviewer-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.478388 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.478388 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.478388 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.478388 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-07-04 01:44:02.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 01:44:02.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90782 2023-07-04 01:44:02.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-04 01:44:02.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.478388 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore_a_la_carte_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 01:44:14.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore_a_la_carte_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-04 01:44:14.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore_a_la_carte_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:14.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore_a_la_carte_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:14.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore_a_la_carte_codeguru_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:14.482389 botocore-a-la-carte-codeguru-reviewer-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-04 01:44:14.000000 botocore-a-la-carte-codeguru-reviewer-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99/LICENSE.txt` & `botocore-a-la-carte-codeguru-reviewer-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99/PKG-INFO` & `botocore-a-la-carte-codeguru-reviewer-1.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codeguru-reviewer
-Version: 1.29.99
+Version: 1.30.0
 Summary: codeguru-reviewer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/endpoint-rule-set-1.json` & `botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/service-2.json` & `botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore/data/codeguru-reviewer/2019-09-19/waiters-2.json` & `botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore/data/codeguru-reviewer/2019-09-19/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore_a_la_carte_codeguru_reviewer.egg-info/PKG-INFO` & `botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore_a_la_carte_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codeguru-reviewer
-Version: 1.29.99
+Version: 1.30.0
 Summary: codeguru-reviewer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99/botocore_a_la_carte_codeguru_reviewer.egg-info/SOURCES.txt` & `botocore-a-la-carte-codeguru-reviewer-1.30.0/botocore_a_la_carte_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-reviewer-1.29.99/setup.py` & `botocore-a-la-carte-codeguru-reviewer-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-codeguru-reviewer',
-    version="1.29.99",
+    version="1.30.0",
     description='codeguru-reviewer data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/codeguru-reviewer/*/*.json'],
```

