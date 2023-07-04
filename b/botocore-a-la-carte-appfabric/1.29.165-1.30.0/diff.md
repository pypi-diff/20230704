# Comparing `tmp/botocore-a-la-carte-appfabric-1.29.165.tar.gz` & `tmp/botocore-a-la-carte-appfabric-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-appfabric-1.29.165.tar", last modified: Sat Jul  1 01:49:37 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-appfabric-1.30.0.tar", last modified: Tue Jul  4 01:44:12 2023, max compression
```

## Comparing `botocore-a-la-carte-appfabric-1.29.165.tar` & `botocore-a-la-carte-appfabric-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:37.014724 botocore-a-la-carte-appfabric-1.29.165/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-01 01:49:36.000000 botocore-a-la-carte-appfabric-1.29.165/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-01 01:49:37.014724 botocore-a-la-carte-appfabric-1.29.165/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:37.010724 botocore-a-la-carte-appfabric-1.29.165/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:37.010724 botocore-a-la-carte-appfabric-1.29.165/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:37.010724 botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:37.010724 botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/2023-05-19/
--rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-07-01 01:49:29.000000 botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/2023-05-19/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-01 01:49:29.000000 botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/2023-05-19/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    86773 2023-07-01 01:49:29.000000 botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/2023-05-19/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-01 01:49:29.000000 botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/2023-05-19/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:37.014724 botocore-a-la-carte-appfabric-1.29.165/botocore_a_la_carte_appfabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-01 01:49:36.000000 botocore-a-la-carte-appfabric-1.29.165/botocore_a_la_carte_appfabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-01 01:49:36.000000 botocore-a-la-carte-appfabric-1.29.165/botocore_a_la_carte_appfabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 01:49:36.000000 botocore-a-la-carte-appfabric-1.29.165/botocore_a_la_carte_appfabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 01:49:36.000000 botocore-a-la-carte-appfabric-1.29.165/botocore_a_la_carte_appfabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 01:49:37.014724 botocore-a-la-carte-appfabric-1.29.165/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-01 01:49:36.000000 botocore-a-la-carte-appfabric-1.29.165/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:12.802374 botocore-a-la-carte-appfabric-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:12.000000 botocore-a-la-carte-appfabric-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-04 01:44:12.802374 botocore-a-la-carte-appfabric-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:12.802374 botocore-a-la-carte-appfabric-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:12.802374 botocore-a-la-carte-appfabric-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:12.802374 botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:12.802374 botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/2023-05-19/
+-rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-07-04 01:44:02.000000 botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/2023-05-19/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-04 01:44:02.000000 botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/2023-05-19/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    86773 2023-07-04 01:44:02.000000 botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/2023-05-19/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 01:44:02.000000 botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/2023-05-19/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:12.802374 botocore-a-la-carte-appfabric-1.30.0/botocore_a_la_carte_appfabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-04 01:44:12.000000 botocore-a-la-carte-appfabric-1.30.0/botocore_a_la_carte_appfabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 01:44:12.000000 botocore-a-la-carte-appfabric-1.30.0/botocore_a_la_carte_appfabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:12.000000 botocore-a-la-carte-appfabric-1.30.0/botocore_a_la_carte_appfabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:12.000000 botocore-a-la-carte-appfabric-1.30.0/botocore_a_la_carte_appfabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:12.802374 botocore-a-la-carte-appfabric-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-04 01:44:12.000000 botocore-a-la-carte-appfabric-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-appfabric-1.29.165/LICENSE.txt` & `botocore-a-la-carte-appfabric-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appfabric-1.29.165/PKG-INFO` & `botocore-a-la-carte-appfabric-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-appfabric
-Version: 1.29.165
+Version: 1.30.0
 Summary: appfabric data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/2023-05-19/endpoint-rule-set-1.json` & `botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/2023-05-19/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/2023-05-19/paginators-1.json` & `botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/2023-05-19/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appfabric-1.29.165/botocore/data/appfabric/2023-05-19/service-2.json` & `botocore-a-la-carte-appfabric-1.30.0/botocore/data/appfabric/2023-05-19/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appfabric-1.29.165/botocore_a_la_carte_appfabric.egg-info/PKG-INFO` & `botocore-a-la-carte-appfabric-1.30.0/botocore_a_la_carte_appfabric.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-appfabric
-Version: 1.29.165
+Version: 1.30.0
 Summary: appfabric data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-appfabric-1.29.165/setup.py` & `botocore-a-la-carte-appfabric-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-appfabric',
-    version="1.29.165",
+    version="1.30.0",
     description='appfabric data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/appfabric/*/*.json'],
```

