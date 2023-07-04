# Comparing `tmp/botocore-a-la-carte-dynamodbstreams-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-dynamodbstreams-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-dynamodbstreams-1.29.99.tar", last modified: Sat Mar 25 01:22:36 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-dynamodbstreams-1.30.0.tar", last modified: Tue Jul  4 01:44:27 2023, max compression
```

## Comparing `botocore-a-la-carte-dynamodbstreams-1.29.99.tar` & `botocore-a-la-carte-dynamodbstreams-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.979195 botocore-a-la-carte-dynamodbstreams-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-25 01:22:36.979195 botocore-a-la-carte-dynamodbstreams-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.979195 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.979195 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.979195 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/dynamodbstreams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.979195 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/dynamodbstreams/2012-08-10/
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/dynamodbstreams/2012-08-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/dynamodbstreams/2012-08-10/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/dynamodbstreams/2012-08-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    32632 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/dynamodbstreams/2012-08-10/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.979195 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore_a_la_carte_dynamodbstreams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore_a_la_carte_dynamodbstreams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore_a_la_carte_dynamodbstreams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore_a_la_carte_dynamodbstreams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/botocore_a_la_carte_dynamodbstreams.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:36.979195 botocore-a-la-carte-dynamodbstreams-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodbstreams-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.686524 botocore-a-la-carte-dynamodbstreams-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 01:44:27.686524 botocore-a-la-carte-dynamodbstreams-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.682523 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.682523 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.682523 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/dynamodbstreams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.682523 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/dynamodbstreams/2012-08-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/dynamodbstreams/2012-08-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/dynamodbstreams/2012-08-10/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/dynamodbstreams/2012-08-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/dynamodbstreams/2012-08-10/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.686524 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore_a_la_carte_dynamodbstreams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore_a_la_carte_dynamodbstreams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore_a_la_carte_dynamodbstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore_a_la_carte_dynamodbstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/botocore_a_la_carte_dynamodbstreams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:27.686524 botocore-a-la-carte-dynamodbstreams-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodbstreams-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-dynamodbstreams-1.29.99/LICENSE.txt` & `botocore-a-la-carte-dynamodbstreams-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodbstreams-1.29.99/PKG-INFO` & `botocore-a-la-carte-dynamodbstreams-1.30.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-dynamodbstreams
-Version: 1.29.99
+Version: 1.30.0
 Summary: dynamodbstreams data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/dynamodbstreams/2012-08-10/examples-1.json` & `botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/dynamodbstreams/2012-08-10/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodbstreams-1.29.99/botocore/data/dynamodbstreams/2012-08-10/service-2.json` & `botocore-a-la-carte-dynamodbstreams-1.30.0/botocore/data/dynamodbstreams/2012-08-10/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998701744072115%*

 * *Differences: {"'shapes'": "{'LimitExceededException': {'documentation': '<p>There is no limit to the number of "*

 * *             'daily on-demand backups that can be taken. </p> <p>For most purposes, up to 500 '*

 * *             'simultaneous table operations are allowed per account. These operations include '*

 * *             '<code>CreateTable</code>, <code>UpdateTable</code>, '*

 * *             '<code>DeleteTable</code>,<code>UpdateTimeToLive</code>, '*

 * *             '<code>RestoreTableFromBackup</code>, and <code>RestoreTableToPoint […]*

```diff
@@ -363,15 +363,15 @@
             "enum": [
                 "HASH",
                 "RANGE"
             ],
             "type": "string"
         },
         "LimitExceededException": {
-            "documentation": "<p>There is no limit to the number of daily on-demand backups that can be taken. </p> <p>For most purposes, up to 500 simultaneous table operations are allowed per account. These operations include <code>CreateTable</code>, <code>UpdateTable</code>, <code>DeleteTable</code>,<code>UpdateTimeToLive</code>, <code>RestoreTableFromBackup</code>, and <code>RestoreTableToPointInTime</code>. </p> <p>When you are creating a table with one or more secondary indexes, you can have up to 250 such requests running at a time. However, if the table or index specifications are complex, then DynamoDB might temporarily reduce the number of concurrent operations.</p> <p>When importing into DynamoDB, up to 50 simultaneous import table operations are allowed per account.</p> <p>There is a soft account quota of 2,500 tables.</p>",
+            "documentation": "<p>There is no limit to the number of daily on-demand backups that can be taken. </p> <p>For most purposes, up to 500 simultaneous table operations are allowed per account. These operations include <code>CreateTable</code>, <code>UpdateTable</code>, <code>DeleteTable</code>,<code>UpdateTimeToLive</code>, <code>RestoreTableFromBackup</code>, and <code>RestoreTableToPointInTime</code>. </p> <p>When you are creating a table with one or more secondary indexes, you can have up to 250 such requests running at a time. However, if the table or index specifications are complex, then DynamoDB might temporarily reduce the number of concurrent operations.</p> <p>When importing into DynamoDB, up to 50 simultaneous import table operations are allowed per account.</p> <p>There is a soft account quota of 2,500 tables.</p> <p>GetRecords was called with a value of more than 1000 for the limit request parameter.</p> <p>More than 2 processes are reading from the same streams shard at the same time. Exceeding this limit may result in request throttling.</p>",
             "exception": true,
             "members": {
                 "message": {
                     "documentation": "<p>Too many operations for a given subscriber.</p>",
                     "shape": "ErrorMessage"
                 }
             },
@@ -468,15 +468,15 @@
                     "shape": "String"
                 },
                 "eventName": {
                     "documentation": "<p>The type of data modification that was performed on the DynamoDB table:</p> <ul> <li> <p> <code>INSERT</code> - a new item was added to the table.</p> </li> <li> <p> <code>MODIFY</code> - one or more of an existing item's attributes were modified.</p> </li> <li> <p> <code>REMOVE</code> - the item was deleted from the table</p> </li> </ul>",
                     "shape": "OperationType"
                 },
                 "eventSource": {
-                    "documentation": "<p>The AWS service from which the stream record originated. For DynamoDB Streams, this is <code>aws:dynamodb</code>.</p>",
+                    "documentation": "<p>The Amazon Web Services service from which the stream record originated. For DynamoDB Streams, this is <code>aws:dynamodb</code>.</p>",
                     "shape": "String"
                 },
                 "eventVersion": {
                     "documentation": "<p>The version number of the stream record format. This number is updated whenever the structure of <code>Record</code> is modified.</p> <p>Client applications must not assume that <code>eventVersion</code> will remain at a particular value, as this number is subject to change at any time. In general, <code>eventVersion</code> will only increase as the low-level DynamoDB Streams API evolves.</p>",
                     "shape": "String"
                 },
                 "userIdentity": {
@@ -569,15 +569,15 @@
             "documentation": "<p>Represents all of the data describing a particular stream.</p>",
             "members": {
                 "StreamArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the stream.</p>",
                     "shape": "StreamArn"
                 },
                 "StreamLabel": {
-                    "documentation": "<p>A timestamp, in ISO 8601 format, for this stream.</p> <p>Note that <code>LatestStreamLabel</code> is not a unique identifier for the stream, because it is possible that a stream from another table might have the same timestamp. However, the combination of the following three elements is guaranteed to be unique:</p> <ul> <li> <p>the AWS customer ID.</p> </li> <li> <p>the table name</p> </li> <li> <p>the <code>StreamLabel</code> </p> </li> </ul>",
+                    "documentation": "<p>A timestamp, in ISO 8601 format, for this stream.</p> <p>Note that <code>LatestStreamLabel</code> is not a unique identifier for the stream, because it is possible that a stream from another table might have the same timestamp. However, the combination of the following three elements is guaranteed to be unique:</p> <ul> <li> <p>the Amazon Web Services customer ID.</p> </li> <li> <p>the table name</p> </li> <li> <p>the <code>StreamLabel</code> </p> </li> </ul>",
                     "shape": "String"
                 },
                 "TableName": {
                     "documentation": "<p>The DynamoDB table with which the stream is associated.</p>",
                     "shape": "TableName"
                 }
             },
@@ -608,15 +608,15 @@
                     "shape": "ShardDescriptionList"
                 },
                 "StreamArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the stream.</p>",
                     "shape": "StreamArn"
                 },
                 "StreamLabel": {
-                    "documentation": "<p>A timestamp, in ISO 8601 format, for this stream.</p> <p>Note that <code>LatestStreamLabel</code> is not a unique identifier for the stream, because it is possible that a stream from another table might have the same timestamp. However, the combination of the following three elements is guaranteed to be unique:</p> <ul> <li> <p>the AWS customer ID.</p> </li> <li> <p>the table name</p> </li> <li> <p>the <code>StreamLabel</code> </p> </li> </ul>",
+                    "documentation": "<p>A timestamp, in ISO 8601 format, for this stream.</p> <p>Note that <code>LatestStreamLabel</code> is not a unique identifier for the stream, because it is possible that a stream from another table might have the same timestamp. However, the combination of the following three elements is guaranteed to be unique:</p> <ul> <li> <p>the Amazon Web Services customer ID.</p> </li> <li> <p>the table name</p> </li> <li> <p>the <code>StreamLabel</code> </p> </li> </ul>",
                     "shape": "String"
                 },
                 "StreamStatus": {
                     "documentation": "<p>Indicates the current status of the stream:</p> <ul> <li> <p> <code>ENABLING</code> - Streams is currently being enabled on the DynamoDB table.</p> </li> <li> <p> <code>ENABLED</code> - the stream is enabled.</p> </li> <li> <p> <code>DISABLING</code> - Streams is currently being disabled on the DynamoDB table.</p> </li> <li> <p> <code>DISABLED</code> - the stream is disabled.</p> </li> </ul>",
                     "shape": "StreamStatus"
                 },
                 "StreamViewType": {
@@ -636,15 +636,15 @@
             },
             "type": "list"
         },
         "StreamRecord": {
             "documentation": "<p>A description of a single data modification that was performed on an item in a DynamoDB table.</p>",
             "members": {
                 "ApproximateCreationDateTime": {
-                    "documentation": "<p>The approximate date and time when the stream record was created, in <a href=\"http://www.epochconverter.com/\">UNIX epoch time</a> format.</p>",
+                    "documentation": "<p>The approximate date and time when the stream record was created, in <a href=\"http://www.epochconverter.com/\">UNIX epoch time</a> format and rounded down to the closest second.</p>",
                     "shape": "Date"
                 },
                 "Keys": {
                     "documentation": "<p>The primary key attribute(s) for the DynamoDB item that was modified.</p>",
                     "shape": "AttributeMap"
                 },
                 "NewImage": {
```

### Comparing `botocore-a-la-carte-dynamodbstreams-1.29.99/botocore_a_la_carte_dynamodbstreams.egg-info/PKG-INFO` & `botocore-a-la-carte-dynamodbstreams-1.30.0/botocore_a_la_carte_dynamodbstreams.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-dynamodbstreams
-Version: 1.29.99
+Version: 1.30.0
 Summary: dynamodbstreams data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-dynamodbstreams-1.29.99/setup.py` & `botocore-a-la-carte-dynamodbstreams-1.30.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-dynamodbstreams',
-    version="1.29.99",
+    version="1.30.0",
     description='dynamodbstreams data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/dynamodbstreams/*/*.json'],
```

