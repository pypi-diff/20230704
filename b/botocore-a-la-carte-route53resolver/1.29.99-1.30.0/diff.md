# Comparing `tmp/botocore-a-la-carte-route53resolver-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-route53resolver-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-route53resolver-1.29.99.tar", last modified: Sat Mar 25 01:23:08 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-route53resolver-1.30.0.tar", last modified: Tue Jul  4 01:45:00 2023, max compression
```

## Comparing `botocore-a-la-carte-route53resolver-1.29.99.tar` & `botocore-a-la-carte-route53resolver-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:08.437068 botocore-a-la-carte-route53resolver-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:08.000000 botocore-a-la-carte-route53resolver-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-25 01:23:08.437068 botocore-a-la-carte-route53resolver-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:08.433068 botocore-a-la-carte-route53resolver-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:08.433068 botocore-a-la-carte-route53resolver-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:08.433068 botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:08.433068 botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-03-25 01:22:12.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-25 01:22:12.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-25 01:22:12.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)   226948 2023-03-25 01:22:12.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:08.433068 botocore-a-la-carte-route53resolver-1.29.99/botocore_a_la_carte_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-25 01:23:08.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore_a_la_carte_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-25 01:23:08.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore_a_la_carte_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:08.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore_a_la_carte_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:08.000000 botocore-a-la-carte-route53resolver-1.29.99/botocore_a_la_carte_route53resolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:08.437068 botocore-a-la-carte-route53resolver-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-25 01:23:08.000000 botocore-a-la-carte-route53resolver-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:00.862835 botocore-a-la-carte-route53resolver-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:00.000000 botocore-a-la-carte-route53resolver-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 01:45:00.862835 botocore-a-la-carte-route53resolver-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:00.858835 botocore-a-la-carte-route53resolver-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:00.858835 botocore-a-la-carte-route53resolver-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:00.858835 botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:00.858835 botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-07-04 01:44:02.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-04 01:44:02.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-04 01:44:02.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)   226948 2023-07-04 01:44:02.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:00.862835 botocore-a-la-carte-route53resolver-1.30.0/botocore_a_la_carte_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 01:45:00.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore_a_la_carte_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-04 01:45:00.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore_a_la_carte_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:00.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore_a_la_carte_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:00.000000 botocore-a-la-carte-route53resolver-1.30.0/botocore_a_la_carte_route53resolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:00.862835 botocore-a-la-carte-route53resolver-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-04 01:45:00.000000 botocore-a-la-carte-route53resolver-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/LICENSE.txt` & `botocore-a-la-carte-route53resolver-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/PKG-INFO` & `botocore-a-la-carte-route53resolver-1.30.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53resolver
-Version: 1.29.99
+Version: 1.30.0
 Summary: route53resolver data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/endpoint-rule-set-1.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999255782274%*

 * *Differences: {"'rules'": "{1: {'rules': {0: {'rules': {0: {'rules': {1: {'rules': {0: {'rules': {0: {'rules': "*

 * *            "{insert: [(0, OrderedDict([('conditions', [OrderedDict([('fn', 'stringEquals'), "*

 * *            "('argv', [OrderedDict([('ref', 'Region')]), 'us-gov-east-1'])])]), ('endpoint', "*

 * *            "OrderedDict([('url', 'https://route53resolver.us-gov-east-1.amazonaws.com'), "*

 * *            "('properties', OrderedDict()), ('headers', OrderedDict())])), ('type', "*

 * *            "'endpoint')])), (1, OrderedDict( […]*

```diff
@@ -232,14 +232,52 @@
                                                 }
                                             ],
                                             "rules": [
                                                 {
                                                     "conditions": [],
                                                     "rules": [
                                                         {
+                                                            "conditions": [
+                                                                {
+                                                                    "argv": [
+                                                                        {
+                                                                            "ref": "Region"
+                                                                        },
+                                                                        "us-gov-east-1"
+                                                                    ],
+                                                                    "fn": "stringEquals"
+                                                                }
+                                                            ],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://route53resolver.us-gov-east-1.amazonaws.com"
+                                                            },
+                                                            "type": "endpoint"
+                                                        },
+                                                        {
+                                                            "conditions": [
+                                                                {
+                                                                    "argv": [
+                                                                        {
+                                                                            "ref": "Region"
+                                                                        },
+                                                                        "us-gov-west-1"
+                                                                    ],
+                                                                    "fn": "stringEquals"
+                                                                }
+                                                            ],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://route53resolver.us-gov-west-1.amazonaws.com"
+                                                            },
+                                                            "type": "endpoint"
+                                                        },
+                                                        {
                                                             "conditions": [],
                                                             "endpoint": {
                                                                 "headers": {},
                                                                 "properties": {},
                                                                 "url": "https://route53resolver-fips.{Region}.{PartitionResult#dnsSuffix}"
                                                             },
                                                             "type": "endpoint"
```

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/paginators-1.json` & `botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/paginators-1.sdk-extras.json` & `botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/paginators-1.sdk-extras.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/botocore/data/route53resolver/2018-04-01/service-2.json` & `botocore-a-la-carte-route53resolver-1.30.0/botocore/data/route53resolver/2018-04-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/botocore_a_la_carte_route53resolver.egg-info/PKG-INFO` & `botocore-a-la-carte-route53resolver-1.30.0/botocore_a_la_carte_route53resolver.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53resolver
-Version: 1.29.99
+Version: 1.30.0
 Summary: route53resolver data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/botocore_a_la_carte_route53resolver.egg-info/SOURCES.txt` & `botocore-a-la-carte-route53resolver-1.30.0/botocore_a_la_carte_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53resolver-1.29.99/setup.py` & `botocore-a-la-carte-route53resolver-1.30.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-route53resolver',
-    version="1.29.99",
+    version="1.30.0",
     description='route53resolver data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/route53resolver/*/*.json'],
```

