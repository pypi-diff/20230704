# Comparing `tmp/botocore-a-la-carte-codestar-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-codestar-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-codestar-1.29.99.tar", last modified: Sat Mar 25 01:22:25 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-codestar-1.30.0.tar", last modified: Tue Jul  4 01:44:15 2023, max compression
```

## Comparing `botocore-a-la-carte-codestar-1.29.99.tar` & `botocore-a-la-carte-codestar-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:25.122449 botocore-a-la-carte-codestar-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:24.000000 botocore-a-la-carte-codestar-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:22:25.122449 botocore-a-la-carte-codestar-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:25.122449 botocore-a-la-carte-codestar-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:25.122449 botocore-a-la-carte-codestar-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:25.122449 botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:25.122449 botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/2017-04-19/
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-03-25 01:22:12.000000 botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/2017-04-19/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/2017-04-19/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-25 01:22:12.000000 botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/2017-04-19/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    55261 2023-03-25 01:22:12.000000 botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/2017-04-19/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:25.122449 botocore-a-la-carte-codestar-1.29.99/botocore_a_la_carte_codestar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:22:25.000000 botocore-a-la-carte-codestar-1.29.99/botocore_a_la_carte_codestar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-25 01:22:25.000000 botocore-a-la-carte-codestar-1.29.99/botocore_a_la_carte_codestar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:25.000000 botocore-a-la-carte-codestar-1.29.99/botocore_a_la_carte_codestar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:25.000000 botocore-a-la-carte-codestar-1.29.99/botocore_a_la_carte_codestar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:25.122449 botocore-a-la-carte-codestar-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-25 01:22:24.000000 botocore-a-la-carte-codestar-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:15.898401 botocore-a-la-carte-codestar-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:15.000000 botocore-a-la-carte-codestar-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:15.898401 botocore-a-la-carte-codestar-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:15.894401 botocore-a-la-carte-codestar-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:15.894401 botocore-a-la-carte-codestar-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:15.898401 botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:15.898401 botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/2017-04-19/
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-07-04 01:44:02.000000 botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/2017-04-19/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/2017-04-19/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-04 01:44:02.000000 botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/2017-04-19/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55261 2023-07-04 01:44:02.000000 botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/2017-04-19/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:15.898401 botocore-a-la-carte-codestar-1.30.0/botocore_a_la_carte_codestar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:15.000000 botocore-a-la-carte-codestar-1.30.0/botocore_a_la_carte_codestar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-04 01:44:15.000000 botocore-a-la-carte-codestar-1.30.0/botocore_a_la_carte_codestar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:15.000000 botocore-a-la-carte-codestar-1.30.0/botocore_a_la_carte_codestar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:15.000000 botocore-a-la-carte-codestar-1.30.0/botocore_a_la_carte_codestar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:15.898401 botocore-a-la-carte-codestar-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-04 01:44:15.000000 botocore-a-la-carte-codestar-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-codestar-1.29.99/LICENSE.txt` & `botocore-a-la-carte-codestar-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codestar-1.29.99/PKG-INFO` & `botocore-a-la-carte-codestar-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codestar
-Version: 1.29.99
+Version: 1.30.0
 Summary: codestar data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/2017-04-19/endpoint-rule-set-1.json` & `botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/2017-04-19/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/2017-04-19/paginators-1.json` & `botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/2017-04-19/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codestar-1.29.99/botocore/data/codestar/2017-04-19/service-2.json` & `botocore-a-la-carte-codestar-1.30.0/botocore/data/codestar/2017-04-19/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codestar-1.29.99/botocore_a_la_carte_codestar.egg-info/PKG-INFO` & `botocore-a-la-carte-codestar-1.30.0/botocore_a_la_carte_codestar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codestar
-Version: 1.29.99
+Version: 1.30.0
 Summary: codestar data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codestar-1.29.99/setup.py` & `botocore-a-la-carte-codestar-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-codestar',
-    version="1.29.99",
+    version="1.30.0",
     description='codestar data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/codestar/*/*.json'],
```

