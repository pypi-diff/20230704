# Comparing `tmp/botocore-a-la-carte-waf-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-waf-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-waf-1.29.99.tar", last modified: Sat Mar 25 01:23:13 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-waf-1.30.0.tar", last modified: Tue Jul  4 01:45:06 2023, max compression
```

## Comparing `botocore-a-la-carte-waf-1.29.99.tar` & `botocore-a-la-carte-waf-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:13.913257 botocore-a-la-carte-waf-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:13.000000 botocore-a-la-carte-waf-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:23:13.913257 botocore-a-la-carte-waf-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:13.913257 botocore-a-la-carte-waf-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:13.913257 botocore-a-la-carte-waf-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:13.913257 botocore-a-la-carte-waf-1.29.99/botocore/data/waf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:13.913257 botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/
--rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-03-25 01:22:12.000000 botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-03-25 01:22:12.000000 botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-25 01:22:12.000000 botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   401091 2023-03-25 01:22:12.000000 botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:13.913257 botocore-a-la-carte-waf-1.29.99/botocore_a_la_carte_waf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:23:13.000000 botocore-a-la-carte-waf-1.29.99/botocore_a_la_carte_waf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-25 01:23:13.000000 botocore-a-la-carte-waf-1.29.99/botocore_a_la_carte_waf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:13.000000 botocore-a-la-carte-waf-1.29.99/botocore_a_la_carte_waf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:13.000000 botocore-a-la-carte-waf-1.29.99/botocore_a_la_carte_waf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:13.913257 botocore-a-la-carte-waf-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-25 01:23:13.000000 botocore-a-la-carte-waf-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.566886 botocore-a-la-carte-waf-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:06.000000 botocore-a-la-carte-waf-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:45:06.566886 botocore-a-la-carte-waf-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.566886 botocore-a-la-carte-waf-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.566886 botocore-a-la-carte-waf-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.566886 botocore-a-la-carte-waf-1.30.0/botocore/data/waf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.566886 botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/
+-rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-07-04 01:44:02.000000 botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-07-04 01:44:02.000000 botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-04 01:44:02.000000 botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   401091 2023-07-04 01:44:02.000000 botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.566886 botocore-a-la-carte-waf-1.30.0/botocore_a_la_carte_waf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:45:06.000000 botocore-a-la-carte-waf-1.30.0/botocore_a_la_carte_waf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 01:45:06.000000 botocore-a-la-carte-waf-1.30.0/botocore_a_la_carte_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:06.000000 botocore-a-la-carte-waf-1.30.0/botocore_a_la_carte_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:06.000000 botocore-a-la-carte-waf-1.30.0/botocore_a_la_carte_waf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:06.566886 botocore-a-la-carte-waf-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-04 01:45:06.000000 botocore-a-la-carte-waf-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-waf-1.29.99/LICENSE.txt` & `botocore-a-la-carte-waf-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-waf-1.29.99/PKG-INFO` & `botocore-a-la-carte-waf-1.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-waf
-Version: 1.29.99
+Version: 1.30.0
 Summary: waf data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/endpoint-rule-set-1.json` & `botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/examples-1.json` & `botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/paginators-1.json` & `botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-waf-1.29.99/botocore/data/waf/2015-08-24/service-2.json` & `botocore-a-la-carte-waf-1.30.0/botocore/data/waf/2015-08-24/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-waf-1.29.99/botocore_a_la_carte_waf.egg-info/PKG-INFO` & `botocore-a-la-carte-waf-1.30.0/botocore_a_la_carte_waf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-waf
-Version: 1.29.99
+Version: 1.30.0
 Summary: waf data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-waf-1.29.99/setup.py` & `botocore-a-la-carte-waf-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-waf',
-    version="1.29.99",
+    version="1.30.0",
     description='waf data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/waf/*/*.json'],
```

