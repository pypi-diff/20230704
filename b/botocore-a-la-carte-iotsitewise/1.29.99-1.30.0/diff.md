# Comparing `tmp/botocore-a-la-carte-iotsitewise-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-iotsitewise-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-iotsitewise-1.29.99.tar", last modified: Sat Mar 25 01:22:44 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-iotsitewise-1.30.0.tar", last modified: Tue Jul  4 01:44:35 2023, max compression
```

## Comparing `botocore-a-la-carte-iotsitewise-1.29.99.tar` & `botocore-a-la-carte-iotsitewise-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:44.207671 botocore-a-la-carte-iotsitewise-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:43.000000 botocore-a-la-carte-iotsitewise-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-25 01:22:44.207671 botocore-a-la-carte-iotsitewise-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:44.207671 botocore-a-la-carte-iotsitewise-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:44.207671 botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:44.207671 botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:44.207671 botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/
--rw-r--r--   0 runner    (1001) docker     (123)    17644 2023-03-25 01:22:12.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-25 01:22:12.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   317171 2023-03-25 01:22:12.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-25 01:22:12.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:44.207671 botocore-a-la-carte-iotsitewise-1.29.99/botocore_a_la_carte_iotsitewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-25 01:22:44.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore_a_la_carte_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-25 01:22:44.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore_a_la_carte_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:44.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore_a_la_carte_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:44.000000 botocore-a-la-carte-iotsitewise-1.29.99/botocore_a_la_carte_iotsitewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:44.207671 botocore-a-la-carte-iotsitewise-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-25 01:22:43.000000 botocore-a-la-carte-iotsitewise-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:35.062595 botocore-a-la-carte-iotsitewise-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:34.000000 botocore-a-la-carte-iotsitewise-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-04 01:44:35.062595 botocore-a-la-carte-iotsitewise-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:35.058595 botocore-a-la-carte-iotsitewise-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:35.058595 botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:35.058595 botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:35.058595 botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/
+-rw-r--r--   0 runner    (1001) docker     (123)    17644 2023-07-04 01:44:02.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-04 01:44:02.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   317992 2023-07-04 01:44:02.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-04 01:44:02.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:35.062595 botocore-a-la-carte-iotsitewise-1.30.0/botocore_a_la_carte_iotsitewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-04 01:44:35.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore_a_la_carte_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-04 01:44:35.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore_a_la_carte_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:35.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore_a_la_carte_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:35.000000 botocore-a-la-carte-iotsitewise-1.30.0/botocore_a_la_carte_iotsitewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:35.062595 botocore-a-la-carte-iotsitewise-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 01:44:34.000000 botocore-a-la-carte-iotsitewise-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/LICENSE.txt` & `botocore-a-la-carte-iotsitewise-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/PKG-INFO` & `botocore-a-la-carte-iotsitewise-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotsitewise
-Version: 1.29.99
+Version: 1.30.0
 Summary: iotsitewise data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/paginators-1.json` & `botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/service-2.json` & `botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994689981280466%*

 * *Differences: {"'shapes'": "{'BatchGetAssetPropertyAggregatesRequest': {'members': {'maxResults': "*

 * *             "{'documentation': '<p>The maximum number of results to return for each paginated "*

 * *             'request. A result set is returned in the two cases, whichever occurs first.</p> <ul> '*

 * *             '<li> <p>The size of the result set is equal to 1 MB.</p> </li> <li> <p>The number of '*

 * *             'data points in the result set is equal to the value of <code>maxResults</code>. The '*

 * *             "maximum value […]*

```diff
@@ -3591,15 +3591,15 @@
         "BatchGetAssetPropertyAggregatesRequest": {
             "members": {
                 "entries": {
                     "documentation": "<p>The list of asset property aggregate entries for the batch get request. You can specify up to 16 entries per request.</p>",
                     "shape": "BatchGetAssetPropertyAggregatesEntries"
                 },
                 "maxResults": {
-                    "documentation": "<p>The maximum number of results to return for each paginated request. A result set is returned in the two cases, whichever occurs first.</p> <ul> <li> <p>The size of the result set is less than 1 MB.</p> </li> <li> <p>The number of data points in the result set is less than the value of <code>maxResults</code>. The maximum value of <code>maxResults</code> is 4000.</p> </li> </ul>",
+                    "documentation": "<p>The maximum number of results to return for each paginated request. A result set is returned in the two cases, whichever occurs first.</p> <ul> <li> <p>The size of the result set is equal to 1 MB.</p> </li> <li> <p>The number of data points in the result set is equal to the value of <code>maxResults</code>. The maximum value of <code>maxResults</code> is 4000.</p> </li> </ul>",
                     "shape": "BatchGetAssetPropertyAggregatesMaxResults"
                 },
                 "nextToken": {
                     "documentation": "<p>The token to be used for the next set of paginated results.</p>",
                     "shape": "NextToken"
                 }
             },
@@ -3881,15 +3881,15 @@
         "BatchGetAssetPropertyValueHistoryRequest": {
             "members": {
                 "entries": {
                     "documentation": "<p>The list of asset property historical value entries for the batch get request. You can specify up to 16 entries per request.</p>",
                     "shape": "BatchGetAssetPropertyValueHistoryEntries"
                 },
                 "maxResults": {
-                    "documentation": "<p>The maximum number of results to return for each paginated request. A result set is returned in the two cases, whichever occurs first.</p> <ul> <li> <p>The size of the result set is less than 1 MB.</p> </li> <li> <p>The number of data points in the result set is less than the value of <code>maxResults</code>. The maximum value of <code>maxResults</code> is 4000.</p> </li> </ul>",
+                    "documentation": "<p>The maximum number of results to return for each paginated request. A result set is returned in the two cases, whichever occurs first.</p> <ul> <li> <p>The size of the result set is equal to 4 MB.</p> </li> <li> <p>The number of data points in the result set is equal to the value of <code>maxResults</code>. The maximum value of <code>maxResults</code> is 20000.</p> </li> </ul>",
                     "shape": "BatchGetAssetPropertyValueHistoryMaxResults"
                 },
                 "nextToken": {
                     "documentation": "<p>The token to be used for the next set of paginated results.</p>",
                     "shape": "NextToken"
                 }
             },
@@ -6193,18 +6193,18 @@
                 "endDate": {
                     "documentation": "<p>The inclusive end of the range from which to query historical data, expressed in seconds in Unix epoch time.</p>",
                     "location": "querystring",
                     "locationName": "endDate",
                     "shape": "Timestamp"
                 },
                 "maxResults": {
-                    "documentation": "<p>The maximum number of results to return for each paginated request.</p> <p>Default: 100</p>",
+                    "documentation": "<p>The maximum number of results to return for each paginated request. A result set is returned in the two cases, whichever occurs first.</p> <ul> <li> <p>The size of the result set is equal to 1 MB.</p> </li> <li> <p>The number of data points in the result set is equal to the value of <code>maxResults</code>. The maximum value of <code>maxResults</code> is 250.</p> </li> </ul>",
                     "location": "querystring",
                     "locationName": "maxResults",
-                    "shape": "MaxResults"
+                    "shape": "GetAssetPropertyValueAggregatesMaxResults"
                 },
                 "nextToken": {
                     "documentation": "<p>The token to be used for the next set of paginated results.</p>",
                     "location": "querystring",
                     "locationName": "nextToken",
                     "shape": "NextToken"
                 },
@@ -6265,14 +6265,22 @@
                 }
             },
             "required": [
                 "aggregatedValues"
             ],
             "type": "structure"
         },
+        "GetAssetPropertyValueAggregatesMaxResults": {
+            "min": 1,
+            "type": "integer"
+        },
+        "GetAssetPropertyValueHistoryMaxResults": {
+            "min": 1,
+            "type": "integer"
+        },
         "GetAssetPropertyValueHistoryRequest": {
             "members": {
                 "assetId": {
                     "documentation": "<p>The ID of the asset.</p>",
                     "location": "querystring",
                     "locationName": "assetId",
                     "shape": "ID"
@@ -6280,18 +6288,18 @@
                 "endDate": {
                     "documentation": "<p>The inclusive end of the range from which to query historical data, expressed in seconds in Unix epoch time.</p>",
                     "location": "querystring",
                     "locationName": "endDate",
                     "shape": "Timestamp"
                 },
                 "maxResults": {
-                    "documentation": "<p>The maximum number of results to return for each paginated request.</p> <p>Default: 100</p>",
+                    "documentation": "<p>The maximum number of results to return for each paginated request. A result set is returned in the two cases, whichever occurs first.</p> <ul> <li> <p>The size of the result set is equal to 4 MB.</p> </li> <li> <p>The number of data points in the result set is equal to the value of <code>maxResults</code>. The maximum value of <code>maxResults</code> is 20000.</p> </li> </ul>",
                     "location": "querystring",
                     "locationName": "maxResults",
-                    "shape": "MaxResults"
+                    "shape": "GetAssetPropertyValueHistoryMaxResults"
                 },
                 "nextToken": {
                     "documentation": "<p>The token to be used for the next set of paginated results.</p>",
                     "location": "querystring",
                     "locationName": "nextToken",
                     "shape": "NextToken"
                 },
@@ -8086,17 +8094,17 @@
                 "GOOD",
                 "BAD",
                 "UNCERTAIN"
             ],
             "type": "string"
         },
         "Resolution": {
-            "max": 2,
+            "max": 3,
             "min": 2,
-            "pattern": "1m|1h|1d",
+            "pattern": "1m|15m|1h|1d",
             "type": "string"
         },
         "Resource": {
             "documentation": "<p>Contains an IoT SiteWise Monitor resource ID for a portal or project.</p>",
             "members": {
                 "portal": {
                     "documentation": "<p>A portal resource.</p>",
```

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/botocore/data/iotsitewise/2019-12-02/waiters-2.json` & `botocore-a-la-carte-iotsitewise-1.30.0/botocore/data/iotsitewise/2019-12-02/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/botocore_a_la_carte_iotsitewise.egg-info/PKG-INFO` & `botocore-a-la-carte-iotsitewise-1.30.0/botocore_a_la_carte_iotsitewise.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotsitewise
-Version: 1.29.99
+Version: 1.30.0
 Summary: iotsitewise data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/botocore_a_la_carte_iotsitewise.egg-info/SOURCES.txt` & `botocore-a-la-carte-iotsitewise-1.30.0/botocore_a_la_carte_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotsitewise-1.29.99/setup.py` & `botocore-a-la-carte-iotsitewise-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-iotsitewise',
-    version="1.29.99",
+    version="1.30.0",
     description='iotsitewise data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/iotsitewise/*/*.json'],
```

