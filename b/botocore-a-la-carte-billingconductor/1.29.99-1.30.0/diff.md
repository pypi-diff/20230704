# Comparing `tmp/botocore-a-la-carte-billingconductor-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-billingconductor-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-billingconductor-1.29.99.tar", last modified: Sat Mar 25 01:22:28 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-billingconductor-1.30.0.tar", last modified: Tue Jul  4 01:44:19 2023, max compression
```

## Comparing `botocore-a-la-carte-billingconductor-1.29.99.tar` & `botocore-a-la-carte-billingconductor-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:28.894714 botocore-a-la-carte-billingconductor-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:28.000000 botocore-a-la-carte-billingconductor-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-25 01:22:28.894714 botocore-a-la-carte-billingconductor-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:28.890714 botocore-a-la-carte-billingconductor-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:28.890714 botocore-a-la-carte-billingconductor-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:28.890714 botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:28.894714 botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/
--rw-r--r--   0 runner    (1001) docker     (123)    33698 2023-03-25 01:22:12.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-25 01:22:12.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   116718 2023-03-25 01:22:12.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-25 01:22:12.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:28.894714 botocore-a-la-carte-billingconductor-1.29.99/botocore_a_la_carte_billingconductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-25 01:22:28.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore_a_la_carte_billingconductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-25 01:22:28.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore_a_la_carte_billingconductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:28.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore_a_la_carte_billingconductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:28.000000 botocore-a-la-carte-billingconductor-1.29.99/botocore_a_la_carte_billingconductor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:28.894714 botocore-a-la-carte-billingconductor-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-25 01:22:28.000000 botocore-a-la-carte-billingconductor-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:19.486433 botocore-a-la-carte-billingconductor-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:19.000000 botocore-a-la-carte-billingconductor-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-04 01:44:19.486433 botocore-a-la-carte-billingconductor-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:19.482433 botocore-a-la-carte-billingconductor-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:19.482433 botocore-a-la-carte-billingconductor-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:19.482433 botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:19.486433 botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    33698 2023-07-04 01:44:02.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-04 01:44:02.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   116718 2023-07-04 01:44:02.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 01:44:02.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:19.486433 botocore-a-la-carte-billingconductor-1.30.0/botocore_a_la_carte_billingconductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-04 01:44:19.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore_a_la_carte_billingconductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-04 01:44:19.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore_a_la_carte_billingconductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:19.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore_a_la_carte_billingconductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:19.000000 botocore-a-la-carte-billingconductor-1.30.0/botocore_a_la_carte_billingconductor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:19.486433 botocore-a-la-carte-billingconductor-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-04 01:44:19.000000 botocore-a-la-carte-billingconductor-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-billingconductor-1.29.99/LICENSE.txt` & `botocore-a-la-carte-billingconductor-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-billingconductor-1.29.99/PKG-INFO` & `botocore-a-la-carte-billingconductor-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-billingconductor
-Version: 1.29.99
+Version: 1.30.0
 Summary: billingconductor data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/paginators-1.json` & `botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-billingconductor-1.29.99/botocore/data/billingconductor/2021-07-30/service-2.json` & `botocore-a-la-carte-billingconductor-1.30.0/botocore/data/billingconductor/2021-07-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-billingconductor-1.29.99/botocore_a_la_carte_billingconductor.egg-info/PKG-INFO` & `botocore-a-la-carte-billingconductor-1.30.0/botocore_a_la_carte_billingconductor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-billingconductor
-Version: 1.29.99
+Version: 1.30.0
 Summary: billingconductor data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-billingconductor-1.29.99/botocore_a_la_carte_billingconductor.egg-info/SOURCES.txt` & `botocore-a-la-carte-billingconductor-1.30.0/botocore_a_la_carte_billingconductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-billingconductor-1.29.99/setup.py` & `botocore-a-la-carte-billingconductor-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-billingconductor',
-    version="1.29.99",
+    version="1.30.0",
     description='billingconductor data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/billingconductor/*/*.json'],
```

