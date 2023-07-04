# Comparing `tmp/botocore-a-la-carte-keyspaces-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-keyspaces-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-keyspaces-1.29.99.tar", last modified: Sat Mar 25 01:22:48 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-keyspaces-1.30.0.tar", last modified: Tue Jul  4 01:44:39 2023, max compression
```

## Comparing `botocore-a-la-carte-keyspaces-1.29.99.tar` & `botocore-a-la-carte-keyspaces-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.323905 botocore-a-la-carte-keyspaces-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:48.000000 botocore-a-la-carte-keyspaces-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-25 01:22:48.323905 botocore-a-la-carte-keyspaces-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.323905 botocore-a-la-carte-keyspaces-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.323905 botocore-a-la-carte-keyspaces-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.323905 botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.323905 botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/
--rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-03-25 01:22:12.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-25 01:22:12.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    60014 2023-03-25 01:22:12.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:12.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.323905 botocore-a-la-carte-keyspaces-1.29.99/botocore_a_la_carte_keyspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-25 01:22:48.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore_a_la_carte_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-25 01:22:48.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore_a_la_carte_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:48.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore_a_la_carte_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:48.000000 botocore-a-la-carte-keyspaces-1.29.99/botocore_a_la_carte_keyspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:48.323905 botocore-a-la-carte-keyspaces-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-25 01:22:48.000000 botocore-a-la-carte-keyspaces-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:39.022636 botocore-a-la-carte-keyspaces-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:38.000000 botocore-a-la-carte-keyspaces-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-04 01:44:39.022636 botocore-a-la-carte-keyspaces-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:39.018636 botocore-a-la-carte-keyspaces-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:39.018636 botocore-a-la-carte-keyspaces-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:39.018636 botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:39.018636 botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-07-04 01:44:02.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-04 01:44:02.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63076 2023-07-04 01:44:02.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:02.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:39.022636 botocore-a-la-carte-keyspaces-1.30.0/botocore_a_la_carte_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-04 01:44:38.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore_a_la_carte_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-04 01:44:38.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore_a_la_carte_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:38.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore_a_la_carte_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:38.000000 botocore-a-la-carte-keyspaces-1.30.0/botocore_a_la_carte_keyspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:39.022636 botocore-a-la-carte-keyspaces-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-04 01:44:38.000000 botocore-a-la-carte-keyspaces-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-keyspaces-1.29.99/LICENSE.txt` & `botocore-a-la-carte-keyspaces-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-keyspaces-1.29.99/PKG-INFO` & `botocore-a-la-carte-keyspaces-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-keyspaces
-Version: 1.29.99
+Version: 1.30.0
 Summary: keyspaces data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/paginators-1.json` & `botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-keyspaces-1.29.99/botocore/data/keyspaces/2022-02-10/service-2.json` & `botocore-a-la-carte-keyspaces-1.30.0/botocore/data/keyspaces/2022-02-10/service-2.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942656774045224%*

 * *Differences: {"'operations'": "{'TagResource': {'documentation': '<p>Associates a set of tags with a Amazon "*

 * *                 'Keyspaces resource. You can then activate these user-defined tags so that they '*

 * *                 'appear on the Cost Management Console for cost allocation tracking. For more '*

 * *                 'information, see <a '*

 * *                 'href="https://docs.aws.amazon.com/keyspaces/latest/devguide/tagging-keyspaces.html">Adding '*

 * *                 'tags and labels to Amazon Keyspaces resources</a>  […]*

```diff
@@ -332,15 +332,15 @@
             },
             "name": "RestoreTable",
             "output": {
                 "shape": "RestoreTableResponse"
             }
         },
         "TagResource": {
-            "documentation": "<p>Associates a set of tags with a Amazon Keyspaces resource. You can then activate these user-defined tags so that they appear on the Cost Management Console for cost allocation tracking. For more information, see <a href=\"https://docs.aws.amazon.com/keyspaces/latest/devguide/tagging-keyspaces.html\">Adding tags and labels to Amazon Keyspaces resources</a> in the <i>Amazon Keyspaces Developer Guide</i>.</p> <p>For IAM policy examples that show how to control access to Amazon Keyspaces resources based on tags, see <a href=\"https://docs.aws.amazon.com/keyspaces/latest/devguide/security_iam_id-based-policy-examples-tags\">Amazon Keyspaces resource access based on tags</a> in the <i>Amazon Keyspaces Developer Guide</i>.</p>",
+            "documentation": "<p>Associates a set of tags with a Amazon Keyspaces resource. You can then activate these user-defined tags so that they appear on the Cost Management Console for cost allocation tracking. For more information, see <a href=\"https://docs.aws.amazon.com/keyspaces/latest/devguide/tagging-keyspaces.html\">Adding tags and labels to Amazon Keyspaces resources</a> in the <i>Amazon Keyspaces Developer Guide</i>.</p> <p>For IAM policy examples that show how to control access to Amazon Keyspaces resources based on tags, see <a href=\"https://docs.aws.amazon.com/keyspaces/latest/devguide/security_iam_id-based-policy-examples.html#security_iam_id-based-policy-examples-tags\">Amazon Keyspaces resource access based on tags</a> in the <i>Amazon Keyspaces Developer Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "ServiceQuotaExceededException"
                 },
@@ -596,14 +596,18 @@
         },
         "CreateKeyspaceRequest": {
             "members": {
                 "keyspaceName": {
                     "documentation": "<p>The name of the keyspace to be created.</p>",
                     "shape": "KeyspaceName"
                 },
+                "replicationSpecification": {
+                    "documentation": "<p> The replication specification of the keyspace includes:</p> <ul> <li> <p> <code>replicationStrategy</code> - the required value is <code>SINGLE_REGION</code> or <code>MULTI_REGION</code>.</p> </li> <li> <p> <code>regionList</code> - if the <code>replicationStrategy</code> is <code>MULTI_REGION</code>, the <code>regionList</code> requires the current Region and at least one additional Amazon Web Services Region where the keyspace is going to be replicated in. The maximum number of supported replication Regions including the current Region is six.</p> </li> </ul>",
+                    "shape": "ReplicationSpecification"
+                },
                 "tags": {
                     "documentation": "<p>A list of key-value pair tags to be attached to the keyspace.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/keyspaces/latest/devguide/tagging-keyspaces.html\">Adding tags and labels to Amazon Keyspaces resources</a> in the <i>Amazon Keyspaces Developer Guide</i>.</p>",
                     "shape": "TagList"
                 }
             },
             "required": [
                 "keyspaceName"
@@ -772,22 +776,31 @@
         },
         "GetKeyspaceResponse": {
             "members": {
                 "keyspaceName": {
                     "documentation": "<p>The name of the keyspace.</p>",
                     "shape": "KeyspaceName"
                 },
+                "replicationRegions": {
+                    "documentation": "<p> If the <code>replicationStrategy</code> of the keyspace is <code>MULTI_REGION</code>, a list of replication Regions is returned. </p>",
+                    "shape": "RegionList"
+                },
+                "replicationStrategy": {
+                    "documentation": "<p> Returns the replication strategy of the keyspace. The options are <code>SINGLE_REGION</code> or <code>MULTI_REGION</code>. </p>",
+                    "shape": "rs"
+                },
                 "resourceArn": {
-                    "documentation": "<p>The ARN of the keyspace.</p>",
+                    "documentation": "<p>Returns the ARN of the keyspace.</p>",
                     "shape": "ARN"
                 }
             },
             "required": [
                 "keyspaceName",
-                "resourceArn"
+                "resourceArn",
+                "replicationStrategy"
             ],
             "type": "structure"
         },
         "GetTableRequest": {
             "members": {
                 "keyspaceName": {
                     "documentation": "<p>The name of the keyspace that the table is stored in.</p>",
@@ -876,32 +889,41 @@
                 }
             },
             "type": "structure"
         },
         "KeyspaceName": {
             "max": 48,
             "min": 1,
-            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_]{1,47}",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_]{0,47}",
             "type": "string"
         },
         "KeyspaceSummary": {
             "documentation": "<p>Represents the properties of a keyspace.</p>",
             "members": {
                 "keyspaceName": {
                     "documentation": "<p>The name of the keyspace.</p>",
                     "shape": "KeyspaceName"
                 },
+                "replicationRegions": {
+                    "documentation": "<p> If the <code>replicationStrategy</code> of the keyspace is <code>MULTI_REGION</code>, a list of replication Regions is returned. </p>",
+                    "shape": "RegionList"
+                },
+                "replicationStrategy": {
+                    "documentation": "<p> This property specifies if a keyspace is a single Region keyspace or a multi-Region keyspace. The available values are <code>SINGLE_REGION</code> or <code>MULTI_REGION</code>. </p>",
+                    "shape": "rs"
+                },
                 "resourceArn": {
                     "documentation": "<p>The unique identifier of the keyspace in the format of an Amazon Resource Name (ARN).</p>",
                     "shape": "ARN"
                 }
             },
             "required": [
                 "keyspaceName",
-                "resourceArn"
+                "resourceArn",
+                "replicationStrategy"
             ],
             "type": "structure"
         },
         "KeyspaceSummaryList": {
             "member": {
                 "shape": "KeyspaceSummary"
             },
@@ -1066,14 +1088,39 @@
                 }
             },
             "required": [
                 "status"
             ],
             "type": "structure"
         },
+        "RegionList": {
+            "max": 6,
+            "member": {
+                "shape": "region"
+            },
+            "min": 2,
+            "type": "list"
+        },
+        "ReplicationSpecification": {
+            "documentation": "<p> The replication specification of the keyspace includes:</p> <ul> <li> <p> <code>regionList</code> - up to six Amazon Web Services Regions where the keyspace is replicated in.</p> </li> <li> <p> <code>replicationStrategy</code> - the required value is <code>SINGLE_REGION</code> or <code>MULTI_REGION</code>.</p> </li> </ul>",
+            "members": {
+                "regionList": {
+                    "documentation": "<p> The <code>regionList</code> can contain up to six Amazon Web Services Regions where the keyspace is replicated in. </p>",
+                    "shape": "RegionList"
+                },
+                "replicationStrategy": {
+                    "documentation": "<p> The <code>replicationStrategy</code> of a keyspace, the required value is <code>SINGLE_REGION</code> or <code>MULTI_REGION</code>. </p>",
+                    "shape": "rs"
+                }
+            },
+            "required": [
+                "replicationStrategy"
+            ],
+            "type": "structure"
+        },
         "ResourceNotFoundException": {
             "documentation": "<p>The operation tried to access a keyspace or table that doesn't exist. The resource might not be specified correctly, or its status might not be <code>ACTIVE</code>.</p>",
             "exception": true,
             "members": {
                 "message": {
                     "shape": "String"
                 },
@@ -1207,15 +1254,15 @@
         },
         "String": {
             "type": "string"
         },
         "TableName": {
             "max": 48,
             "min": 1,
-            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_]{1,47}",
+            "pattern": "[a-zA-Z0-9][a-zA-Z0-9_]{0,47}",
             "type": "string"
         },
         "TableStatus": {
             "enum": [
                 "ACTIVE",
                 "CREATING",
                 "UPDATING",
@@ -1429,11 +1476,25 @@
             },
             "type": "structure"
         },
         "kmsKeyARN": {
             "max": 5096,
             "min": 1,
             "type": "string"
+        },
+        "region": {
+            "max": 25,
+            "min": 2,
+            "type": "string"
+        },
+        "rs": {
+            "enum": [
+                "SINGLE_REGION",
+                "MULTI_REGION"
+            ],
+            "max": 20,
+            "min": 1,
+            "type": "string"
         }
     },
     "version": "2.0"
 }
```

### Comparing `botocore-a-la-carte-keyspaces-1.29.99/botocore_a_la_carte_keyspaces.egg-info/PKG-INFO` & `botocore-a-la-carte-keyspaces-1.30.0/botocore_a_la_carte_keyspaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-keyspaces
-Version: 1.29.99
+Version: 1.30.0
 Summary: keyspaces data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-keyspaces-1.29.99/setup.py` & `botocore-a-la-carte-keyspaces-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-keyspaces',
-    version="1.29.99",
+    version="1.30.0",
     description='keyspaces data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/keyspaces/*/*.json'],
```

