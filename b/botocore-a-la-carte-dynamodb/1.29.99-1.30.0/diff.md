# Comparing `tmp/botocore-a-la-carte-dynamodb-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-dynamodb-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-dynamodb-1.29.99.tar", last modified: Sat Mar 25 01:22:36 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-dynamodb-1.30.0.tar", last modified: Tue Jul  4 01:44:27 2023, max compression
```

## Comparing `botocore-a-la-carte-dynamodb-1.29.99.tar` & `botocore-a-la-carte-dynamodb-1.30.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.611170 botocore-a-la-carte-dynamodb-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodb-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:22:36.611170 botocore-a-la-carte-dynamodb-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.607170 botocore-a-la-carte-dynamodb-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.607170 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.607170 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.611170 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2011-12-05/
--rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2011-12-05/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2011-12-05/examples-1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.611170 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/
--rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   438122 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-25 01:22:12.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.611170 botocore-a-la-carte-dynamodb-1.29.99/botocore_a_la_carte_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore_a_la_carte_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore_a_la_carte_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore_a_la_carte_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodb-1.29.99/botocore_a_la_carte_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:36.611170 botocore-a-la-carte-dynamodb-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-25 01:22:36.000000 botocore-a-la-carte-dynamodb-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.290520 botocore-a-la-carte-dynamodb-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodb-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:27.290520 botocore-a-la-carte-dynamodb-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.286520 botocore-a-la-carte-dynamodb-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.286520 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.286520 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.286520 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2011-12-05/
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2011-12-05/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2011-12-05/examples-1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.286520 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   441538 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-04 01:44:02.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.286520 botocore-a-la-carte-dynamodb-1.30.0/botocore_a_la_carte_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore_a_la_carte_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore_a_la_carte_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore_a_la_carte_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodb-1.30.0/botocore_a_la_carte_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:27.290520 botocore-a-la-carte-dynamodb-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-04 01:44:27.000000 botocore-a-la-carte-dynamodb-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/LICENSE.txt` & `botocore-a-la-carte-dynamodb-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/PKG-INFO` & `botocore-a-la-carte-dynamodb-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-dynamodb
-Version: 1.29.99
+Version: 1.30.0
 Summary: dynamodb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2011-12-05/endpoint-rule-set-1.json` & `botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2011-12-05/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/examples-1.json` & `botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/paginators-1.json` & `botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/service-2.json` & `botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997431430942555%*

 * *Differences: {"'operations'": "{'BatchGetItem': {'documentation': '<p>The <code>BatchGetItem</code> operation "*

 * *                 'returns the attributes of one or more items from one or more tables. You '*

 * *                 'identify requested items by primary key.</p> <p>A single operation can retrieve '*

 * *                 'up to 16 MB of data, which can contain as many as 100 items. '*

 * *                 '<code>BatchGetItem</code> returns a partial result if the response size limit is '*

 * *                 "exceeded, the table\ […]*

```diff
@@ -32,15 +32,15 @@
             },
             "name": "BatchExecuteStatement",
             "output": {
                 "shape": "BatchExecuteStatementOutput"
             }
         },
         "BatchGetItem": {
-            "documentation": "<p>The <code>BatchGetItem</code> operation returns the attributes of one or more items from one or more tables. You identify requested items by primary key.</p> <p>A single operation can retrieve up to 16 MB of data, which can contain as many as 100 items. <code>BatchGetItem</code> returns a partial result if the response size limit is exceeded, the table's provisioned throughput is exceeded, or an internal processing failure occurs. If a partial result is returned, the operation returns a value for <code>UnprocessedKeys</code>. You can use this value to retry the operation starting with the next item to get.</p> <important> <p>If you request more than 100 items, <code>BatchGetItem</code> returns a <code>ValidationException</code> with the message \"Too many items requested for the BatchGetItem call.\"</p> </important> <p>For example, if you ask to retrieve 100 items, but each individual item is 300 KB in size, the system returns 52 items (so as not to exceed the 16 MB limit). It also returns an appropriate <code>UnprocessedKeys</code> value so you can get the next page of results. If desired, your application can include its own logic to assemble the pages of results into one dataset.</p> <p>If <i>none</i> of the items can be processed due to insufficient provisioned throughput on all of the tables in the request, then <code>BatchGetItem</code> returns a <code>ProvisionedThroughputExceededException</code>. If <i>at least one</i> of the items is successfully processed, then <code>BatchGetItem</code> completes successfully, while returning the keys of the unread items in <code>UnprocessedKeys</code>.</p> <important> <p>If DynamoDB returns any unprocessed items, you should retry the batch operation on those items. However, <i>we strongly recommend that you use an exponential backoff algorithm</i>. If you retry the batch operation immediately, the underlying read or write requests can still fail due to throttling on the individual tables. If you delay the batch operation using exponential backoff, the individual requests in the batch are much more likely to succeed.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/ErrorHandling.html#BatchOperations\">Batch Operations and Error Handling</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p> </important> <p>By default, <code>BatchGetItem</code> performs eventually consistent reads on every table in the request. If you want strongly consistent reads instead, you can set <code>ConsistentRead</code> to <code>true</code> for any or all tables.</p> <p>In order to minimize response latency, <code>BatchGetItem</code> retrieves items in parallel.</p> <p>When designing your application, keep in mind that DynamoDB does not return items in any particular order. To help parse the response by item, include the primary key values for the items in your request in the <code>ProjectionExpression</code> parameter.</p> <p>If a requested item does not exist, it is not returned in the result. Requests for nonexistent items consume the minimum read capacity units according to the type of read. For more information, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/WorkingWithTables.html#CapacityUnitCalculations\">Working with Tables</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p>",
+            "documentation": "<p>The <code>BatchGetItem</code> operation returns the attributes of one or more items from one or more tables. You identify requested items by primary key.</p> <p>A single operation can retrieve up to 16 MB of data, which can contain as many as 100 items. <code>BatchGetItem</code> returns a partial result if the response size limit is exceeded, the table's provisioned throughput is exceeded, more than 1MB per partition is requested, or an internal processing failure occurs. If a partial result is returned, the operation returns a value for <code>UnprocessedKeys</code>. You can use this value to retry the operation starting with the next item to get.</p> <important> <p>If you request more than 100 items, <code>BatchGetItem</code> returns a <code>ValidationException</code> with the message \"Too many items requested for the BatchGetItem call.\"</p> </important> <p>For example, if you ask to retrieve 100 items, but each individual item is 300 KB in size, the system returns 52 items (so as not to exceed the 16 MB limit). It also returns an appropriate <code>UnprocessedKeys</code> value so you can get the next page of results. If desired, your application can include its own logic to assemble the pages of results into one dataset.</p> <p>If <i>none</i> of the items can be processed due to insufficient provisioned throughput on all of the tables in the request, then <code>BatchGetItem</code> returns a <code>ProvisionedThroughputExceededException</code>. If <i>at least one</i> of the items is successfully processed, then <code>BatchGetItem</code> completes successfully, while returning the keys of the unread items in <code>UnprocessedKeys</code>.</p> <important> <p>If DynamoDB returns any unprocessed items, you should retry the batch operation on those items. However, <i>we strongly recommend that you use an exponential backoff algorithm</i>. If you retry the batch operation immediately, the underlying read or write requests can still fail due to throttling on the individual tables. If you delay the batch operation using exponential backoff, the individual requests in the batch are much more likely to succeed.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/ErrorHandling.html#BatchOperations\">Batch Operations and Error Handling</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p> </important> <p>By default, <code>BatchGetItem</code> performs eventually consistent reads on every table in the request. If you want strongly consistent reads instead, you can set <code>ConsistentRead</code> to <code>true</code> for any or all tables.</p> <p>In order to minimize response latency, <code>BatchGetItem</code> may retrieve items in parallel.</p> <p>When designing your application, keep in mind that DynamoDB does not return items in any particular order. To help parse the response by item, include the primary key values for the items in your request in the <code>ProjectionExpression</code> parameter.</p> <p>If a requested item does not exist, it is not returned in the result. Requests for nonexistent items consume the minimum read capacity units according to the type of read. For more information, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/WorkingWithTables.html#CapacityUnitCalculations\">Working with Tables</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p>",
             "endpointdiscovery": {},
             "errors": [
                 {
                     "shape": "ProvisionedThroughputExceededException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
@@ -347,15 +347,15 @@
             },
             "name": "DescribeContributorInsights",
             "output": {
                 "shape": "DescribeContributorInsightsOutput"
             }
         },
         "DescribeEndpoints": {
-            "documentation": "<p>Returns the regional endpoint information. This action must be included in your VPC endpoint policies, or access to the DescribeEndpoints API will be denied. For more information on policy permissions, please see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/inter-network-traffic-privacy.html#inter-network-traffic-DescribeEndpoints\">Internetwork traffic privacy</a>.</p>",
+            "documentation": "<p>Returns the regional endpoint information. For more information on policy permissions, please see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/inter-network-traffic-privacy.html#inter-network-traffic-DescribeEndpoints\">Internetwork traffic privacy</a>.</p>",
             "endpointoperation": true,
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DescribeEndpointsRequest"
@@ -999,15 +999,15 @@
             },
             "name": "Query",
             "output": {
                 "shape": "QueryOutput"
             }
         },
         "RestoreTableFromBackup": {
-            "documentation": "<p>Creates a new table from an existing backup. Any number of users can execute up to 4 concurrent restores (any type of restore) in a given account. </p> <p>You can call <code>RestoreTableFromBackup</code> at a maximum rate of 10 times per second.</p> <p>You must manually set up the following on the restored table:</p> <ul> <li> <p>Auto scaling policies</p> </li> <li> <p>IAM policies</p> </li> <li> <p>Amazon CloudWatch metrics and alarms</p> </li> <li> <p>Tags</p> </li> <li> <p>Stream settings</p> </li> <li> <p>Time to Live (TTL) settings</p> </li> </ul>",
+            "documentation": "<p>Creates a new table from an existing backup. Any number of users can execute up to 50 concurrent restores (any type of restore) in a given account. </p> <p>You can call <code>RestoreTableFromBackup</code> at a maximum rate of 10 times per second.</p> <p>You must manually set up the following on the restored table:</p> <ul> <li> <p>Auto scaling policies</p> </li> <li> <p>IAM policies</p> </li> <li> <p>Amazon CloudWatch metrics and alarms</p> </li> <li> <p>Tags</p> </li> <li> <p>Stream settings</p> </li> <li> <p>Time to Live (TTL) settings</p> </li> </ul>",
             "endpointdiscovery": {},
             "errors": [
                 {
                     "shape": "TableAlreadyExistsException"
                 },
                 {
                     "shape": "TableInUseException"
@@ -2033,14 +2033,18 @@
         "BatchStatementError": {
             "documentation": "<p> An error associated with a statement in a PartiQL batch that was run. </p>",
             "members": {
                 "Code": {
                     "documentation": "<p> The error code associated with the failed PartiQL batch statement. </p>",
                     "shape": "BatchStatementErrorCodeEnum"
                 },
+                "Item": {
+                    "documentation": "<p>The item which caused the condition check to fail. This will be set if ReturnValuesOnConditionCheckFailure is specified as <code>ALL_OLD</code>.</p>",
+                    "shape": "AttributeMap"
+                },
                 "Message": {
                     "documentation": "<p> The error message associated with the PartiQL batch response. </p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
@@ -2067,14 +2071,18 @@
                     "documentation": "<p> The read consistency of the PartiQL batch request. </p>",
                     "shape": "ConsistentRead"
                 },
                 "Parameters": {
                     "documentation": "<p> The parameters associated with a PartiQL statement in the batch request. </p>",
                     "shape": "PreparedStatementParameters"
                 },
+                "ReturnValuesOnConditionCheckFailure": {
+                    "documentation": "<p>An optional parameter that returns the item attributes for a PartiQL batch request operation that failed a condition check.</p> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p>",
+                    "shape": "ReturnValuesOnConditionCheckFailure"
+                },
                 "Statement": {
                     "documentation": "<p> A valid PartiQL statement. </p>",
                     "shape": "PartiQLStatement"
                 }
             },
             "required": [
                 "Statement"
@@ -2322,14 +2330,18 @@
         "ConditionExpression": {
             "type": "string"
         },
         "ConditionalCheckFailedException": {
             "documentation": "<p>A condition specified in the operation could not be evaluated.</p>",
             "exception": true,
             "members": {
+                "Item": {
+                    "documentation": "<p>Item which caused the <code>ConditionalCheckFailedException</code>.</p>",
+                    "shape": "AttributeMap"
+                },
                 "message": {
                     "documentation": "<p>The conditional request failed.</p>",
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
         },
@@ -2800,14 +2812,18 @@
                     "documentation": "<p>Determines whether item collection metrics are returned. If set to <code>SIZE</code>, the response includes statistics about item collections, if any, that were modified during the operation are returned in the response. If set to <code>NONE</code> (the default), no statistics are returned.</p>",
                     "shape": "ReturnItemCollectionMetrics"
                 },
                 "ReturnValues": {
                     "documentation": "<p>Use <code>ReturnValues</code> if you want to get the item attributes as they appeared before they were deleted. For <code>DeleteItem</code>, the valid values are:</p> <ul> <li> <p> <code>NONE</code> - If <code>ReturnValues</code> is not specified, or if its value is <code>NONE</code>, then nothing is returned. (This setting is the default for <code>ReturnValues</code>.)</p> </li> <li> <p> <code>ALL_OLD</code> - The content of the old item is returned.</p> </li> </ul> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p> <note> <p>The <code>ReturnValues</code> parameter is used by several DynamoDB operations; however, <code>DeleteItem</code> does not recognize any values other than <code>NONE</code> or <code>ALL_OLD</code>.</p> </note>",
                     "shape": "ReturnValue"
                 },
+                "ReturnValuesOnConditionCheckFailure": {
+                    "documentation": "<p>An optional parameter that returns the item attributes for a <code>DeleteItem</code> operation that failed a condition check.</p> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p>",
+                    "shape": "ReturnValuesOnConditionCheckFailure"
+                },
                 "TableName": {
                     "documentation": "<p>The name of the table from which to delete the item.</p>",
                     "shape": "TableName"
                 }
             },
             "required": [
                 "TableName",
@@ -3286,14 +3302,18 @@
                 "Parameters": {
                     "documentation": "<p>The parameters for the PartiQL statement, if any.</p>",
                     "shape": "PreparedStatementParameters"
                 },
                 "ReturnConsumedCapacity": {
                     "shape": "ReturnConsumedCapacity"
                 },
+                "ReturnValuesOnConditionCheckFailure": {
+                    "documentation": "<p>An optional parameter that returns the item attributes for an <code>ExecuteStatement</code> operation that failed a condition check.</p> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p>",
+                    "shape": "ReturnValuesOnConditionCheckFailure"
+                },
                 "Statement": {
                     "documentation": "<p>The PartiQL statement representing the operation to run.</p>",
                     "shape": "PartiQLStatement"
                 }
             },
             "required": [
                 "Statement"
@@ -4556,15 +4576,15 @@
             },
             "type": "structure"
         },
         "LastUpdateDateTime": {
             "type": "timestamp"
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
@@ -4953,14 +4973,18 @@
         "ParameterizedStatement": {
             "documentation": "<p> Represents a PartiQL statment that uses parameters. </p>",
             "members": {
                 "Parameters": {
                     "documentation": "<p> The parameter values. </p>",
                     "shape": "PreparedStatementParameters"
                 },
+                "ReturnValuesOnConditionCheckFailure": {
+                    "documentation": "<p>An optional parameter that returns the item attributes for a PartiQL <code>ParameterizedStatement</code> operation that failed a condition check.</p> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p>",
+                    "shape": "ReturnValuesOnConditionCheckFailure"
+                },
                 "Statement": {
                     "documentation": "<p> A PartiQL statment that uses parameters. </p>",
                     "shape": "PartiQLStatement"
                 }
             },
             "required": [
                 "Statement"
@@ -5091,19 +5115,19 @@
             ],
             "type": "string"
         },
         "ProvisionedThroughput": {
             "documentation": "<p>Represents the provisioned throughput settings for a specified table or index. The settings can be modified using the <code>UpdateTable</code> operation.</p> <p>For current minimum and maximum provisioned throughput values, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Limits.html\">Service, Account, and Table Quotas</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p>",
             "members": {
                 "ReadCapacityUnits": {
-                    "documentation": "<p>The maximum number of strongly consistent reads consumed per second before DynamoDB returns a <code>ThrottlingException</code>. For more information, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/WorkingWithTables.html#ProvisionedThroughput\">Specifying Read and Write Requirements</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p> <p>If read/write capacity mode is <code>PAY_PER_REQUEST</code> the value is set to 0.</p>",
+                    "documentation": "<p>The maximum number of strongly consistent reads consumed per second before DynamoDB returns a <code>ThrottlingException</code>. For more information, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/ProvisionedThroughput.html\">Specifying Read and Write Requirements</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p> <p>If read/write capacity mode is <code>PAY_PER_REQUEST</code> the value is set to 0.</p>",
                     "shape": "PositiveLongObject"
                 },
                 "WriteCapacityUnits": {
-                    "documentation": "<p>The maximum number of writes consumed per second before DynamoDB returns a <code>ThrottlingException</code>. For more information, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/WorkingWithTables.html#ProvisionedThroughput\">Specifying Read and Write Requirements</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p> <p>If read/write capacity mode is <code>PAY_PER_REQUEST</code> the value is set to 0.</p>",
+                    "documentation": "<p>The maximum number of writes consumed per second before DynamoDB returns a <code>ThrottlingException</code>. For more information, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/ProvisionedThroughput.html\">Specifying Read and Write Requirements</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p> <p>If read/write capacity mode is <code>PAY_PER_REQUEST</code> the value is set to 0.</p>",
                     "shape": "PositiveLongObject"
                 }
             },
             "required": [
                 "ReadCapacityUnits",
                 "WriteCapacityUnits"
             ],
@@ -5224,14 +5248,18 @@
                     "documentation": "<p>Determines whether item collection metrics are returned. If set to <code>SIZE</code>, the response includes statistics about item collections, if any, that were modified during the operation are returned in the response. If set to <code>NONE</code> (the default), no statistics are returned.</p>",
                     "shape": "ReturnItemCollectionMetrics"
                 },
                 "ReturnValues": {
                     "documentation": "<p>Use <code>ReturnValues</code> if you want to get the item attributes as they appeared before they were updated with the <code>PutItem</code> request. For <code>PutItem</code>, the valid values are:</p> <ul> <li> <p> <code>NONE</code> - If <code>ReturnValues</code> is not specified, or if its value is <code>NONE</code>, then nothing is returned. (This setting is the default for <code>ReturnValues</code>.)</p> </li> <li> <p> <code>ALL_OLD</code> - If <code>PutItem</code> overwrote an attribute name-value pair, then the content of the old item is returned.</p> </li> </ul> <p>The values returned are strongly consistent.</p> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p> <note> <p>The <code>ReturnValues</code> parameter is used by several DynamoDB operations; however, <code>PutItem</code> does not recognize any values other than <code>NONE</code> or <code>ALL_OLD</code>.</p> </note>",
                     "shape": "ReturnValue"
                 },
+                "ReturnValuesOnConditionCheckFailure": {
+                    "documentation": "<p>An optional parameter that returns the item attributes for a <code>PutItem</code> operation that failed a condition check.</p> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p>",
+                    "shape": "ReturnValuesOnConditionCheckFailure"
+                },
                 "TableName": {
                     "documentation": "<p>The name of the table to contain the item.</p>",
                     "shape": "TableName"
                 }
             },
             "required": [
                 "TableName",
@@ -7145,14 +7173,18 @@
                     "documentation": "<p>Determines whether item collection metrics are returned. If set to <code>SIZE</code>, the response includes statistics about item collections, if any, that were modified during the operation are returned in the response. If set to <code>NONE</code> (the default), no statistics are returned.</p>",
                     "shape": "ReturnItemCollectionMetrics"
                 },
                 "ReturnValues": {
                     "documentation": "<p>Use <code>ReturnValues</code> if you want to get the item attributes as they appear before or after they are successfully updated. For <code>UpdateItem</code>, the valid values are:</p> <ul> <li> <p> <code>NONE</code> - If <code>ReturnValues</code> is not specified, or if its value is <code>NONE</code>, then nothing is returned. (This setting is the default for <code>ReturnValues</code>.)</p> </li> <li> <p> <code>ALL_OLD</code> - Returns all of the attributes of the item, as they appeared before the UpdateItem operation.</p> </li> <li> <p> <code>UPDATED_OLD</code> - Returns only the updated attributes, as they appeared before the UpdateItem operation.</p> </li> <li> <p> <code>ALL_NEW</code> - Returns all of the attributes of the item, as they appear after the UpdateItem operation.</p> </li> <li> <p> <code>UPDATED_NEW</code> - Returns only the updated attributes, as they appear after the UpdateItem operation.</p> </li> </ul> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p> <p>The values returned are strongly consistent.</p>",
                     "shape": "ReturnValue"
                 },
+                "ReturnValuesOnConditionCheckFailure": {
+                    "documentation": "<p>An optional parameter that returns the item attributes for an <code>UpdateItem</code> operation that failed a condition check.</p> <p>There is no additional cost associated with requesting a return value aside from the small network and processing overhead of receiving a larger response. No read capacity units are consumed.</p>",
+                    "shape": "ReturnValuesOnConditionCheckFailure"
+                },
                 "TableName": {
                     "documentation": "<p>The name of the table containing the item to update.</p>",
                     "shape": "TableName"
                 },
                 "UpdateExpression": {
                     "documentation": "<p>An expression that defines one or more attributes to be updated, the action to be performed on them, and new values for them.</p> <p>The following action values are available for <code>UpdateExpression</code>.</p> <ul> <li> <p> <code>SET</code> - Adds one or more attributes and values to an item. If any of these attributes already exist, they are replaced by the new values. You can also use <code>SET</code> to add or subtract from an attribute that is of type Number. For example: <code>SET myNum = myNum + :val</code> </p> <p> <code>SET</code> supports the following functions:</p> <ul> <li> <p> <code>if_not_exists (path, operand)</code> - if the item does not contain an attribute at the specified path, then <code>if_not_exists</code> evaluates to operand; otherwise, it evaluates to path. You can use this function to avoid overwriting an attribute that may already be present in the item.</p> </li> <li> <p> <code>list_append (operand, operand)</code> - evaluates to a list with a new element added to it. You can append the new element to the start or the end of the list by reversing the order of the operands.</p> </li> </ul> <p>These function names are case-sensitive.</p> </li> <li> <p> <code>REMOVE</code> - Removes one or more attributes from an item.</p> </li> <li> <p> <code>ADD</code> - Adds the specified value to the item, if the attribute does not already exist. If the attribute does exist, then the behavior of <code>ADD</code> depends on the data type of the attribute:</p> <ul> <li> <p>If the existing attribute is a number, and if <code>Value</code> is also a number, then <code>Value</code> is mathematically added to the existing attribute. If <code>Value</code> is a negative number, then it is subtracted from the existing attribute.</p> <note> <p>If you use <code>ADD</code> to increment or decrement a number value for an item that doesn't exist before the update, DynamoDB uses <code>0</code> as the initial value.</p> <p>Similarly, if you use <code>ADD</code> for an existing item to increment or decrement an attribute value that doesn't exist before the update, DynamoDB uses <code>0</code> as the initial value. For example, suppose that the item you want to update doesn't have an attribute named <code>itemcount</code>, but you decide to <code>ADD</code> the number <code>3</code> to this attribute anyway. DynamoDB will create the <code>itemcount</code> attribute, set its initial value to <code>0</code>, and finally add <code>3</code> to it. The result will be a new <code>itemcount</code> attribute in the item, with a value of <code>3</code>.</p> </note> </li> <li> <p>If the existing data type is a set and if <code>Value</code> is also a set, then <code>Value</code> is added to the existing set. For example, if the attribute value is the set <code>[1,2]</code>, and the <code>ADD</code> action specified <code>[3]</code>, then the final attribute value is <code>[1,2,3]</code>. An error occurs if an <code>ADD</code> action is specified for a set attribute and the attribute type specified does not match the existing set type. </p> <p>Both sets must have the same primitive data type. For example, if the existing data type is a set of strings, the <code>Value</code> must also be a set of strings.</p> </li> </ul> <important> <p>The <code>ADD</code> action only supports Number and set data types. In addition, <code>ADD</code> can only be used on top-level attributes, not nested attributes.</p> </important> </li> <li> <p> <code>DELETE</code> - Deletes an element from a set.</p> <p>If a set of values is specified, then those values are subtracted from the old set. For example, if the attribute value was the set <code>[a,b,c]</code> and the <code>DELETE</code> action specifies <code>[a,c]</code>, then the final attribute value is <code>[b]</code>. Specifying an empty set is an error.</p> <important> <p>The <code>DELETE</code> action only supports set data types. In addition, <code>DELETE</code> can only be used on top-level attributes, not nested attributes.</p> </important> </li> </ul> <p>You can have many actions in a single expression, such as the following: <code>SET a=:value1, b=:value2 DELETE :value3, :value4, :value5</code> </p> <p>For more information on update expressions, see <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Expressions.Modifying.html\">Modifying Items and Attributes</a> in the <i>Amazon DynamoDB Developer Guide</i>.</p>",
                     "shape": "UpdateExpression"
```

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/botocore/data/dynamodb/2012-08-10/waiters-2.json` & `botocore-a-la-carte-dynamodb-1.30.0/botocore/data/dynamodb/2012-08-10/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/botocore_a_la_carte_dynamodb.egg-info/PKG-INFO` & `botocore-a-la-carte-dynamodb-1.30.0/botocore_a_la_carte_dynamodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-dynamodb
-Version: 1.29.99
+Version: 1.30.0
 Summary: dynamodb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/botocore_a_la_carte_dynamodb.egg-info/SOURCES.txt` & `botocore-a-la-carte-dynamodb-1.30.0/botocore_a_la_carte_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dynamodb-1.29.99/setup.py` & `botocore-a-la-carte-dynamodb-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-dynamodb',
-    version="1.29.99",
+    version="1.30.0",
     description='dynamodb data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/dynamodb/*/*.json'],
```

