# Comparing `tmp/botocore-a-la-carte-cleanrooms-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-cleanrooms-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-cleanrooms-1.29.99.tar", last modified: Sat Mar 25 01:22:32 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-cleanrooms-1.30.0.tar", last modified: Tue Jul  4 01:44:23 2023, max compression
```

## Comparing `botocore-a-la-carte-cleanrooms-1.29.99.tar` & `botocore-a-la-carte-cleanrooms-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:32.338913 botocore-a-la-carte-cleanrooms-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:32.000000 botocore-a-la-carte-cleanrooms-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-25 01:22:32.338913 botocore-a-la-carte-cleanrooms-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:32.334913 botocore-a-la-carte-cleanrooms-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:32.334913 botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:32.334913 botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:32.334913 botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/2022-02-17/
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-03-25 01:22:12.000000 botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/2022-02-17/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-25 01:22:12.000000 botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/2022-02-17/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   125521 2023-03-25 01:22:12.000000 botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/2022-02-17/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-25 01:22:12.000000 botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/2022-02-17/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:32.338913 botocore-a-la-carte-cleanrooms-1.29.99/botocore_a_la_carte_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-25 01:22:32.000000 botocore-a-la-carte-cleanrooms-1.29.99/botocore_a_la_carte_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-25 01:22:32.000000 botocore-a-la-carte-cleanrooms-1.29.99/botocore_a_la_carte_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:32.000000 botocore-a-la-carte-cleanrooms-1.29.99/botocore_a_la_carte_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:32.000000 botocore-a-la-carte-cleanrooms-1.29.99/botocore_a_la_carte_cleanrooms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:32.338913 botocore-a-la-carte-cleanrooms-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-25 01:22:32.000000 botocore-a-la-carte-cleanrooms-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:23.014464 botocore-a-la-carte-cleanrooms-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:22.000000 botocore-a-la-carte-cleanrooms-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:44:23.014464 botocore-a-la-carte-cleanrooms-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:23.010464 botocore-a-la-carte-cleanrooms-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:23.010464 botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:23.010464 botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:23.014464 botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/2022-02-17/
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-07-04 01:44:02.000000 botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/2022-02-17/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-04 01:44:02.000000 botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/2022-02-17/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   126382 2023-07-04 01:44:02.000000 botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/2022-02-17/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 01:44:02.000000 botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/2022-02-17/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:23.014464 botocore-a-la-carte-cleanrooms-1.30.0/botocore_a_la_carte_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:44:22.000000 botocore-a-la-carte-cleanrooms-1.30.0/botocore_a_la_carte_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 01:44:22.000000 botocore-a-la-carte-cleanrooms-1.30.0/botocore_a_la_carte_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:22.000000 botocore-a-la-carte-cleanrooms-1.30.0/botocore_a_la_carte_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:22.000000 botocore-a-la-carte-cleanrooms-1.30.0/botocore_a_la_carte_cleanrooms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:23.014464 botocore-a-la-carte-cleanrooms-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 01:44:22.000000 botocore-a-la-carte-cleanrooms-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-cleanrooms-1.29.99/LICENSE.txt` & `botocore-a-la-carte-cleanrooms-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cleanrooms-1.29.99/PKG-INFO` & `botocore-a-la-carte-cleanrooms-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cleanrooms
-Version: 1.29.99
+Version: 1.30.0
 Summary: cleanrooms data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/2022-02-17/endpoint-rule-set-1.json` & `botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/2022-02-17/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/2022-02-17/paginators-1.json` & `botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/2022-02-17/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cleanrooms-1.29.99/botocore/data/cleanrooms/2022-02-17/service-2.json` & `botocore-a-la-carte-cleanrooms-1.30.0/botocore/data/cleanrooms/2022-02-17/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8971662409986326%*

 * *Differences: {"'documentation'": "'<p>Welcome to the <i>Clean Rooms API Reference</i>.</p> <p>Clean Rooms is an "*

 * *                    'Amazon Web Services service that helps multiple parties to join their data '*

 * *                    'together in a secure collaboration workspace. In the collaboration, members '*

 * *                    'who can query and receive results can get insights into the collective '*

 * *                    "datasets without either party getting access to the other party\\'s raw "*

 * *                    'data […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p>Welcome to the <i>AWS Clean Rooms API Reference</i>.</p> <p>AWS Clean Rooms is an AWS service that helps multiple parties to join their data together in a secure collaboration workspace. In the collaboration, members who can query and receive results can get insights into the collective datasets without either party getting access to the other party's raw data.</p> <p>To learn more about AWS Clean Rooms concepts, procedures, and best practices, see the <a href=\"https://docs.aws.amazon.com/clean-rooms/latest/userguide/what-is.html\">AWS Clean Rooms User Guide</a>.</p>",
+    "documentation": "<p>Welcome to the <i>Clean Rooms API Reference</i>.</p> <p>Clean Rooms is an Amazon Web Services service that helps multiple parties to join their data together in a secure collaboration workspace. In the collaboration, members who can query and receive results can get insights into the collective datasets without either party getting access to the other party's raw data.</p> <p>To learn more about Clean Rooms concepts, procedures, and best practices, see the <a href=\"https://docs.aws.amazon.com/clean-rooms/latest/userguide/what-is.html\">Clean Rooms User Guide</a>.</p>",
     "metadata": {
         "apiVersion": "2022-02-17",
         "endpointPrefix": "cleanrooms",
         "jsonVersion": "1.1",
         "protocol": "rest-json",
         "serviceFullName": "AWS Clean Rooms Service",
         "serviceId": "CleanRooms",
@@ -925,15 +925,15 @@
             },
             "name": "ListTagsForResource",
             "output": {
                 "shape": "ListTagsForResourceOutput"
             }
         },
         "StartProtectedQuery": {
-            "documentation": "<p>Creates a protected query that is started by AWS Clean Rooms.</p>",
+            "documentation": "<p>Creates a protected query that is started by Clean Rooms .</p>",
             "errors": [
                 {
                     "shape": "ServiceQuotaExceededException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -1372,30 +1372,34 @@
                 "createTime",
                 "updateTime",
                 "policy"
             ],
             "type": "structure"
         },
         "AnalysisRuleAggregation": {
-            "documentation": "<p>Enables query structure and specified queries that product aggregate statistics.</p>",
+            "documentation": "<p>Enables query structure and specified queries that produce aggregate statistics.</p>",
             "members": {
                 "aggregateColumns": {
                     "documentation": "<p>The columns that query runners are allowed to use in aggregation queries.</p>",
                     "shape": "AnalysisRuleAggregationAggregateColumnsList"
                 },
+                "allowedJoinOperators": {
+                    "documentation": "<p>Which logical operators (if any) are to be used in an INNER JOIN match condition. Default is <code>AND</code>.</p>",
+                    "shape": "JoinOperatorsList"
+                },
                 "dimensionColumns": {
                     "documentation": "<p>The columns that query runners are allowed to select, group by, or filter by.</p>",
                     "shape": "AnalysisRuleColumnList"
                 },
                 "joinColumns": {
                     "documentation": "<p>Columns in configured table that can be used in join statements and/or as aggregate columns. They can never be outputted directly.</p>",
                     "shape": "AnalysisRuleColumnList"
                 },
                 "joinRequired": {
-                    "documentation": "<p>Control that requires member who runs query to do a join with their configured table and/or other configured table in query</p>",
+                    "documentation": "<p>Control that requires member who runs query to do a join with their configured table and/or other configured table in query.</p>",
                     "shape": "JoinRequiredOption"
                 },
                 "outputConstraints": {
                     "documentation": "<p>Columns that must meet a specific threshold value (after an aggregation function is applied to it) for each output row to be returned.</p>",
                     "shape": "AggregationConstraints"
                 },
                 "scalarFunctions": {
@@ -1430,16 +1434,20 @@
             "min": 1,
             "pattern": "[a-z0-9_](([a-z0-9_ ]+-)*([a-z0-9_ ]+))?",
             "type": "string"
         },
         "AnalysisRuleList": {
             "documentation": "<p>A type of analysis rule that enables row-level analysis.</p>",
             "members": {
+                "allowedJoinOperators": {
+                    "documentation": "<p>Which logical operators (if any) are to be used in an INNER JOIN match condition. Default is <code>AND</code>.</p>",
+                    "shape": "JoinOperatorsList"
+                },
                 "joinColumns": {
-                    "documentation": "<p>Columns that can be used to join a configured table with the table of the member who can query and another members' configured tables.</p>",
+                    "documentation": "<p>Columns that can be used to join a configured table with the table of the member who can query and other members' configured tables.</p>",
                     "shape": "AnalysisRuleListJoinColumnsList"
                 },
                 "listColumns": {
                     "documentation": "<p>Columns that can be listed in the output.</p>",
                     "shape": "AnalysisRuleColumnList"
                 }
             },
@@ -1580,15 +1588,15 @@
                     "shape": "CollaborationArn"
                 },
                 "createTime": {
                     "documentation": "<p>The time when the collaboration was created.</p>",
                     "shape": "Timestamp"
                 },
                 "creatorAccountId": {
-                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports AWS account ID.</p>",
+                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports Amazon Web Services account ID.</p>",
                     "shape": "AccountId"
                 },
                 "creatorDisplayName": {
                     "documentation": "<p>A display name of the collaboration creator.</p>",
                     "shape": "DisplayName"
                 },
                 "dataEncryptionMetadata": {
@@ -1680,15 +1688,15 @@
                     "shape": "CollaborationArn"
                 },
                 "createTime": {
                     "documentation": "<p>The time when the collaboration was created.</p>",
                     "shape": "Timestamp"
                 },
                 "creatorAccountId": {
-                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports AWS Account ID.</p>",
+                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports Amazon Web Services account ID.</p>",
                     "shape": "AccountId"
                 },
                 "creatorDisplayName": {
                     "documentation": "<p>The display name of the collaboration creator.</p>",
                     "shape": "DisplayName"
                 },
                 "id": {
@@ -1731,15 +1739,15 @@
         "CollaborationSummaryList": {
             "member": {
                 "shape": "CollaborationSummary"
             },
             "type": "list"
         },
         "Column": {
-            "documentation": "<p>A column within a schema relation, derived from the underlying AWS Glue table.</p>",
+            "documentation": "<p>A column within a schema relation, derived from the underlying Glue table.</p>",
             "members": {
                 "name": {
                     "documentation": "<p>The name of the column.</p>",
                     "shape": "ColumnName"
                 },
                 "type": {
                     "documentation": "<p>The type of the column.</p>",
@@ -1770,15 +1778,15 @@
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDBFF-\\uDC00\\uDFFF\\t]*",
             "type": "string"
         },
         "ConfiguredTable": {
             "documentation": "<p>A table that has been configured for use in a collaboration.</p>",
             "members": {
                 "allowedColumns": {
-                    "documentation": "<p>The columns within the underlying AWS Glue table that can be utilized within collaborations.</p>",
+                    "documentation": "<p>The columns within the underlying Glue table that can be utilized within collaborations.</p>",
                     "shape": "AllowedColumnList"
                 },
                 "analysisMethod": {
                     "documentation": "<p>The analysis method for the configured table. The only valid value is currently `DIRECT_QUERY`.</p>",
                     "shape": "AnalysisMethod"
                 },
                 "analysisRuleTypes": {
@@ -1802,15 +1810,15 @@
                     "shape": "UUID"
                 },
                 "name": {
                     "documentation": "<p>A name for the configured table.</p>",
                     "shape": "DisplayName"
                 },
                 "tableReference": {
-                    "documentation": "<p>The AWS Glue table that this configured table represents.</p>",
+                    "documentation": "<p>The Glue table that this configured table represents.</p>",
                     "shape": "TableReference"
                 },
                 "updateTime": {
                     "documentation": "<p>The time the configured table was last updated</p>",
                     "shape": "Timestamp"
                 }
             },
@@ -2285,15 +2293,15 @@
                     "shape": "TableDescription"
                 },
                 "name": {
                     "documentation": "<p>The name of the configured table.</p>",
                     "shape": "DisplayName"
                 },
                 "tableReference": {
-                    "documentation": "<p>A reference to the AWS Glue table being configured.</p>",
+                    "documentation": "<p>A reference to the Glue table being configured.</p>",
                     "shape": "TableReference"
                 },
                 "tags": {
                     "documentation": "<p>An optional label that you can assign to a resource when you create it. Each tag consists of a key and an optional value, both of which you define. When you use tagging, you can also use tag-based access control in IAM policies to control access to this resource.</p>",
                     "shape": "TagMap"
                 }
             },
@@ -2772,30 +2780,36 @@
                 }
             },
             "required": [
                 "schema"
             ],
             "type": "structure"
         },
-        "GlueResourceName": {
+        "GlueDatabaseName": {
+            "max": 128,
+            "min": 0,
+            "pattern": "[a-zA-Z0-9_](([a-zA-Z0-9_]+-)*([a-zA-Z0-9_]+))?",
+            "type": "string"
+        },
+        "GlueTableName": {
             "max": 128,
             "min": 0,
             "pattern": "[a-zA-Z0-9_](([a-zA-Z0-9_ ]+-)*([a-zA-Z0-9_ ]+))?",
             "type": "string"
         },
         "GlueTableReference": {
-            "documentation": "<p>A reference to a table within an AWS Glue data catalog.</p>",
+            "documentation": "<p>A reference to a table within an Glue data catalog.</p>",
             "members": {
                 "databaseName": {
-                    "documentation": "<p>The name of the database the AWS Glue table belongs to.</p>",
-                    "shape": "GlueResourceName"
+                    "documentation": "<p>The name of the database the Glue table belongs to.</p>",
+                    "shape": "GlueDatabaseName"
                 },
                 "tableName": {
-                    "documentation": "<p>The name of the AWS Glue table.</p>",
-                    "shape": "GlueResourceName"
+                    "documentation": "<p>The name of the Glue table.</p>",
+                    "shape": "GlueTableName"
                 }
             },
             "required": [
                 "tableName",
                 "databaseName"
             ],
             "type": "structure"
@@ -2810,14 +2824,29 @@
             "members": {
                 "message": {
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
+        "JoinOperator": {
+            "enum": [
+                "OR",
+                "AND"
+            ],
+            "type": "string"
+        },
+        "JoinOperatorsList": {
+            "max": 2,
+            "member": {
+                "shape": "JoinOperator"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "JoinRequiredOption": {
             "enum": [
                 "QUERY_RUNNER"
             ],
             "type": "string"
         },
         "KeyPrefix": {
@@ -3172,15 +3201,15 @@
             "min": 0,
             "type": "list"
         },
         "MemberSpecification": {
             "documentation": "<p>Basic metadata used to construct a new member.</p>",
             "members": {
                 "accountId": {
-                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports AWS Account ID.</p>",
+                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports Amazon Web Services account ID.</p>",
                     "shape": "AccountId"
                 },
                 "displayName": {
                     "documentation": "<p>The member's display name.</p>",
                     "shape": "DisplayName"
                 },
                 "memberAbilities": {
@@ -3208,15 +3237,15 @@
             "documentation": "<p>The member object listed by the request.</p>",
             "members": {
                 "abilities": {
                     "documentation": "<p>The abilities granted to the collaboration member.</p>",
                     "shape": "MemberAbilities"
                 },
                 "accountId": {
-                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports AWS Account ID.</p>",
+                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports Amazon Web Services account ID.</p>",
                     "shape": "AccountId"
                 },
                 "createTime": {
                     "documentation": "<p>The time when the member was created.</p>",
                     "shape": "Timestamp"
                 },
                 "displayName": {
@@ -3264,15 +3293,15 @@
                     "shape": "MembershipArn"
                 },
                 "collaborationArn": {
                     "documentation": "<p>The unique ARN for the membership's associated collaboration.</p>",
                     "shape": "CollaborationArn"
                 },
                 "collaborationCreatorAccountId": {
-                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports AWS account ID.</p>",
+                    "documentation": "<p>The identifier used to reference members of the collaboration. Currently only supports Amazon Web Services account ID.</p>",
                     "shape": "AccountId"
                 },
                 "collaborationCreatorDisplayName": {
                     "documentation": "<p>The display name of the collaboration creator.</p>",
                     "shape": "DisplayName"
                 },
                 "collaborationId": {
@@ -3359,15 +3388,15 @@
                     "shape": "MembershipArn"
                 },
                 "collaborationArn": {
                     "documentation": "<p>The unique ARN for the membership's associated collaboration.</p>",
                     "shape": "CollaborationArn"
                 },
                 "collaborationCreatorAccountId": {
-                    "documentation": "<p>The identifier of the AWS principal that created the collaboration. Currently only supports AWS account ID.</p>",
+                    "documentation": "<p>The identifier of the Amazon Web Services principal that created the collaboration. Currently only supports Amazon Web Services account ID.</p>",
                     "shape": "AccountId"
                 },
                 "collaborationCreatorDisplayName": {
                     "documentation": "<p>The display name of the collaboration creator.</p>",
                     "shape": "DisplayName"
                 },
                 "collaborationId": {
@@ -3422,15 +3451,15 @@
         },
         "PaginationToken": {
             "max": 10240,
             "min": 0,
             "type": "string"
         },
         "ProtectedQuery": {
-            "documentation": "<p>The parameters for an AWS Clean Rooms protected query.</p>",
+            "documentation": "<p>The parameters for an Clean Rooms protected query.</p>",
             "members": {
                 "createTime": {
                     "documentation": "<p>The time at which the protected query was created.</p>",
                     "shape": "Timestamp"
                 },
                 "error": {
                     "documentation": "<p>An error thrown by the protected query.</p>",
@@ -3597,17 +3626,14 @@
             "documentation": "<p>The parameters for the SQL type Protected Query.</p>",
             "members": {
                 "queryString": {
                     "documentation": "<p>The query string to be submitted.</p>",
                     "shape": "ProtectedQuerySQLParametersQueryStringString"
                 }
             },
-            "required": [
-                "queryString"
-            ],
             "sensitive": true,
             "type": "structure"
         },
         "ProtectedQuerySQLParametersQueryStringString": {
             "max": 15000,
             "min": 0,
             "type": "string"
@@ -3776,15 +3802,15 @@
                     "shape": "ColumnList"
                 },
                 "createTime": {
                     "documentation": "<p>The time the schema was created.</p>",
                     "shape": "Timestamp"
                 },
                 "creatorAccountId": {
-                    "documentation": "<p>The unique account ID for the AWS account that owns the schema.</p>",
+                    "documentation": "<p>The unique account ID for the Amazon Web Services account that owns the schema.</p>",
                     "shape": "AccountId"
                 },
                 "description": {
                     "documentation": "<p>A description for the schema.</p>",
                     "shape": "TableDescription"
                 },
                 "name": {
@@ -3847,15 +3873,15 @@
                     "shape": "UUID"
                 },
                 "createTime": {
                     "documentation": "<p>The time the schema object was created.</p>",
                     "shape": "Timestamp"
                 },
                 "creatorAccountId": {
-                    "documentation": "<p>The unique account ID for the AWS account that owns the schema.</p>",
+                    "documentation": "<p>The unique account ID for the Amazon Web Services account that owns the schema.</p>",
                     "shape": "AccountId"
                 },
                 "name": {
                     "documentation": "<p>The name for the schema object.</p>",
                     "shape": "TableAlias"
                 },
                 "type": {
@@ -3979,28 +4005,27 @@
         "TableDescription": {
             "max": 255,
             "min": 0,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDBFF-\\uDC00\\uDFFF\\t\\r\\n]*",
             "type": "string"
         },
         "TableReference": {
-            "documentation": "<p>A pointer to the dataset that underlies this table. Currently, this can only be an AWS Glue table.</p>",
+            "documentation": "<p>A pointer to the dataset that underlies this table. Currently, this can only be an Glue table.</p>",
             "members": {
                 "glue": {
-                    "documentation": "<p>If present, a reference to the AWS Glue table referred to by this table reference.</p>",
+                    "documentation": "<p>If present, a reference to the Glue table referred to by this table reference.</p>",
                     "shape": "GlueTableReference"
                 }
             },
             "type": "structure",
             "union": true
         },
         "TagKey": {
             "max": 128,
             "min": 1,
-            "pattern": "(?!aws:).{1,128}",
             "type": "string"
         },
         "TagKeys": {
             "member": {
                 "shape": "TagKey"
             },
             "type": "list"
```

### Comparing `botocore-a-la-carte-cleanrooms-1.29.99/botocore_a_la_carte_cleanrooms.egg-info/PKG-INFO` & `botocore-a-la-carte-cleanrooms-1.30.0/botocore_a_la_carte_cleanrooms.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cleanrooms
-Version: 1.29.99
+Version: 1.30.0
 Summary: cleanrooms data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cleanrooms-1.29.99/setup.py` & `botocore-a-la-carte-cleanrooms-1.30.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-cleanrooms',
-    version="1.29.99",
+    version="1.30.0",
     description='cleanrooms data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/cleanrooms/*/*.json'],
```

