# Comparing `tmp/botocore-a-la-carte-quicksight-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-quicksight-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-quicksight-1.29.99.tar", last modified: Sat Mar 25 01:23:02 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-quicksight-1.30.0.tar", last modified: Tue Jul  4 01:44:54 2023, max compression
```

## Comparing `botocore-a-la-carte-quicksight-1.29.99.tar` & `botocore-a-la-carte-quicksight-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:02.032706 botocore-a-la-carte-quicksight-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:01.000000 botocore-a-la-carte-quicksight-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-25 01:23:02.032706 botocore-a-la-carte-quicksight-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:02.028706 botocore-a-la-carte-quicksight-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:02.028706 botocore-a-la-carte-quicksight-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:02.028706 botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:02.032706 botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-03-25 01:22:12.000000 botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-25 01:22:12.000000 botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-25 01:22:12.000000 botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)   975971 2023-03-25 01:22:12.000000 botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:02.032706 botocore-a-la-carte-quicksight-1.29.99/botocore_a_la_carte_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-25 01:23:01.000000 botocore-a-la-carte-quicksight-1.29.99/botocore_a_la_carte_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-25 01:23:02.000000 botocore-a-la-carte-quicksight-1.29.99/botocore_a_la_carte_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:01.000000 botocore-a-la-carte-quicksight-1.29.99/botocore_a_la_carte_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:01.000000 botocore-a-la-carte-quicksight-1.29.99/botocore_a_la_carte_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:02.032706 botocore-a-la-carte-quicksight-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-25 01:23:01.000000 botocore-a-la-carte-quicksight-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:54.018773 botocore-a-la-carte-quicksight-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:53.000000 botocore-a-la-carte-quicksight-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:44:54.018773 botocore-a-la-carte-quicksight-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:54.014773 botocore-a-la-carte-quicksight-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:54.014773 botocore-a-la-carte-quicksight-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:54.014773 botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:54.018773 botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-07-04 01:44:02.000000 botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-04 01:44:02.000000 botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-04 01:44:02.000000 botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1163089 2023-07-04 01:44:02.000000 botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:54.018773 botocore-a-la-carte-quicksight-1.30.0/botocore_a_la_carte_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:44:53.000000 botocore-a-la-carte-quicksight-1.30.0/botocore_a_la_carte_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-04 01:44:53.000000 botocore-a-la-carte-quicksight-1.30.0/botocore_a_la_carte_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:53.000000 botocore-a-la-carte-quicksight-1.30.0/botocore_a_la_carte_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:53.000000 botocore-a-la-carte-quicksight-1.30.0/botocore_a_la_carte_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:54.018773 botocore-a-la-carte-quicksight-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 01:44:53.000000 botocore-a-la-carte-quicksight-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-quicksight-1.29.99/LICENSE.txt` & `botocore-a-la-carte-quicksight-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-quicksight-1.29.99/PKG-INFO` & `botocore-a-la-carte-quicksight-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-quicksight
-Version: 1.29.99
+Version: 1.30.0
 Summary: quicksight data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/paginators-1.json` & `botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/paginators-1.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'pagination'": "{'ListAssetBundleExportJobs': OrderedDict([('input_token', 'NextToken'), "*

 * *                 "('output_token', 'NextToken'), ('limit_key', 'MaxResults'), ('result_key', "*

 * *                 "'AssetBundleExportJobSummaryList')]), 'ListAssetBundleImportJobs': "*

 * *                 "OrderedDict([('input_token', 'NextToken'), ('output_token', 'NextToken'), "*

 * *                 "('limit_key', 'MaxResults'), ('result_key', "*

 * *                 "'AssetBundleImportJobSummaryList')])}"}*

```diff
@@ -2,14 +2,26 @@
     "pagination": {
         "ListAnalyses": {
             "input_token": "NextToken",
             "limit_key": "MaxResults",
             "output_token": "NextToken",
             "result_key": "AnalysisSummaryList"
         },
+        "ListAssetBundleExportJobs": {
+            "input_token": "NextToken",
+            "limit_key": "MaxResults",
+            "output_token": "NextToken",
+            "result_key": "AssetBundleExportJobSummaryList"
+        },
+        "ListAssetBundleImportJobs": {
+            "input_token": "NextToken",
+            "limit_key": "MaxResults",
+            "output_token": "NextToken",
+            "result_key": "AssetBundleImportJobSummaryList"
+        },
         "ListDashboardVersions": {
             "input_token": "NextToken",
             "limit_key": "MaxResults",
             "output_token": "NextToken",
             "result_key": "DashboardVersionSummaryList"
         },
         "ListDashboards": {
```

### Comparing `botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/paginators-1.sdk-extras.json` & `botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/paginators-1.sdk-extras.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'merge'": "{'pagination': {'ListAssetBundleExportJobs': OrderedDict([('non_aggregate_keys', "*

 * *            "['Status', 'RequestId'])]), 'ListAssetBundleImportJobs': "*

 * *            "OrderedDict([('non_aggregate_keys', ['Status', 'RequestId'])])}}"}*

```diff
@@ -3,14 +3,26 @@
         "pagination": {
             "ListAnalyses": {
                 "non_aggregate_keys": [
                     "Status",
                     "RequestId"
                 ]
             },
+            "ListAssetBundleExportJobs": {
+                "non_aggregate_keys": [
+                    "Status",
+                    "RequestId"
+                ]
+            },
+            "ListAssetBundleImportJobs": {
+                "non_aggregate_keys": [
+                    "Status",
+                    "RequestId"
+                ]
+            },
             "ListDashboardVersions": {
                 "non_aggregate_keys": [
                     "Status",
                     "RequestId"
                 ]
             },
             "ListDashboards": {
```

### Comparing `botocore-a-la-carte-quicksight-1.29.99/botocore/data/quicksight/2018-04-01/service-2.json` & `botocore-a-la-carte-quicksight-1.30.0/botocore/data/quicksight/2018-04-01/service-2.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9631274883263448%*

 * *Differences: {"'operations'": "{'ListIAMPolicyAssignments': {'http': {'requestUri': "*

 * *                 "'/accounts/{AwsAccountId}/namespaces/{Namespace}/v2/iam-policy-assignments'}, "*

 * *                 "'documentation': '<p>Lists the IAM policy assignments in the current Amazon "*

 * *                 "QuickSight account.</p>'}, 'ListIAMPolicyAssignmentsForUser': {'documentation': "*

 * *                 "'<p>Lists all of the IAM policy assignments, including the Amazon Resource Names "*

 * *                 '(ARNs), for the IAM polici […]*

```diff
@@ -570,14 +570,54 @@
                 "shape": "CreateNamespaceRequest"
             },
             "name": "CreateNamespace",
             "output": {
                 "shape": "CreateNamespaceResponse"
             }
         },
+        "CreateRefreshSchedule": {
+            "documentation": "<p>Creates a refresh schedule for a dataset. You can create up to 5 different schedules for a single dataset.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "PreconditionNotMetException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/accounts/{AwsAccountId}/data-sets/{DataSetId}/refresh-schedules"
+            },
+            "input": {
+                "shape": "CreateRefreshScheduleRequest"
+            },
+            "name": "CreateRefreshSchedule",
+            "output": {
+                "shape": "CreateRefreshScheduleResponse"
+            }
+        },
         "CreateTemplate": {
             "documentation": "<p>Creates a template either from a <code>TemplateDefinition</code> or from an existing Amazon QuickSight analysis or template. You can use the resulting template to create additional dashboards, templates, or analyses.</p> <p>A <i>template</i> is an entity in Amazon QuickSight that encapsulates the metadata required to create an analysis and that you can use to create s dashboard. A template adds a layer of abstraction by using placeholders to replace the dataset associated with the analysis. You can use templates to create dashboards by replacing dataset placeholders with datasets that follow the same schema that was used to create the source analysis and template.</p>",
             "errors": [
                 {
                     "shape": "InvalidParameterValueException"
                 },
                 {
@@ -733,14 +773,134 @@
                 "shape": "CreateThemeAliasRequest"
             },
             "name": "CreateThemeAlias",
             "output": {
                 "shape": "CreateThemeAliasResponse"
             }
         },
+        "CreateTopic": {
+            "documentation": "<p>Creates a new Q topic.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/accounts/{AwsAccountId}/topics"
+            },
+            "input": {
+                "shape": "CreateTopicRequest"
+            },
+            "name": "CreateTopic",
+            "output": {
+                "shape": "CreateTopicResponse"
+            }
+        },
+        "CreateTopicRefreshSchedule": {
+            "documentation": "<p>Creates a topic refresh schedule.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}/schedules"
+            },
+            "input": {
+                "shape": "CreateTopicRefreshScheduleRequest"
+            },
+            "name": "CreateTopicRefreshSchedule",
+            "output": {
+                "shape": "CreateTopicRefreshScheduleResponse"
+            }
+        },
+        "CreateVPCConnection": {
+            "documentation": "<p>Creates a new VPC connection.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/accounts/{AwsAccountId}/vpc-connections"
+            },
+            "input": {
+                "shape": "CreateVPCConnectionRequest"
+            },
+            "name": "CreateVPCConnection",
+            "output": {
+                "shape": "CreateVPCConnectionResponse"
+            }
+        },
         "DeleteAccountCustomization": {
             "documentation": "<p>Deletes all Amazon QuickSight customizations in this Amazon Web Services Region for the specified Amazon Web Services account and Amazon QuickSight namespace.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -906,14 +1066,51 @@
                 "shape": "DeleteDataSetRequest"
             },
             "name": "DeleteDataSet",
             "output": {
                 "shape": "DeleteDataSetResponse"
             }
         },
+        "DeleteDataSetRefreshProperties": {
+            "documentation": "<p>Deletes the dataset refresh properties of the dataset.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/accounts/{AwsAccountId}/data-sets/{DataSetId}/refresh-properties"
+            },
+            "input": {
+                "shape": "DeleteDataSetRefreshPropertiesRequest"
+            },
+            "name": "DeleteDataSetRefreshProperties",
+            "output": {
+                "shape": "DeleteDataSetRefreshPropertiesResponse"
+            }
+        },
         "DeleteDataSource": {
             "documentation": "<p>Deletes the data source permanently. This operation breaks all the datasets that reference the deleted data source.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -1159,14 +1356,48 @@
                 "shape": "DeleteNamespaceRequest"
             },
             "name": "DeleteNamespace",
             "output": {
                 "shape": "DeleteNamespaceResponse"
             }
         },
+        "DeleteRefreshSchedule": {
+            "documentation": "<p>Deletes a refresh schedule from a dataset.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/accounts/{AwsAccountId}/data-sets/{DataSetId}/refresh-schedules/{ScheduleId}"
+            },
+            "input": {
+                "shape": "DeleteRefreshScheduleRequest"
+            },
+            "name": "DeleteRefreshSchedule",
+            "output": {
+                "shape": "DeleteRefreshScheduleResponse"
+            }
+        },
         "DeleteTemplate": {
             "documentation": "<p>Deletes a template.</p>",
             "errors": [
                 {
                     "shape": "InvalidParameterValueException"
                 },
                 {
@@ -1298,14 +1529,88 @@
                 "shape": "DeleteThemeAliasRequest"
             },
             "name": "DeleteThemeAlias",
             "output": {
                 "shape": "DeleteThemeAliasResponse"
             }
         },
+        "DeleteTopic": {
+            "documentation": "<p>Deletes a topic.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}"
+            },
+            "input": {
+                "shape": "DeleteTopicRequest"
+            },
+            "name": "DeleteTopic",
+            "output": {
+                "shape": "DeleteTopicResponse"
+            }
+        },
+        "DeleteTopicRefreshSchedule": {
+            "documentation": "<p>Deletes a topic refresh schedule.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}/schedules/{DatasetId}"
+            },
+            "input": {
+                "shape": "DeleteTopicRefreshScheduleRequest"
+            },
+            "name": "DeleteTopicRefreshSchedule",
+            "output": {
+                "shape": "DeleteTopicRefreshScheduleResponse"
+            }
+        },
         "DeleteUser": {
             "documentation": "<p>Deletes the Amazon QuickSight user that is associated with the identity of the IAM user or role that's making the call. The IAM user isn't deleted as a result of this call. </p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -1372,14 +1677,51 @@
                 "shape": "DeleteUserByPrincipalIdRequest"
             },
             "name": "DeleteUserByPrincipalId",
             "output": {
                 "shape": "DeleteUserByPrincipalIdResponse"
             }
         },
+        "DeleteVPCConnection": {
+            "documentation": "<p>Deletes a VPC connection.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/accounts/{AwsAccountId}/vpc-connections/{VPCConnectionId}"
+            },
+            "input": {
+                "shape": "DeleteVPCConnectionRequest"
+            },
+            "name": "DeleteVPCConnection",
+            "output": {
+                "shape": "DeleteVPCConnectionResponse"
+            }
+        },
         "DescribeAccountCustomization": {
             "documentation": "<p>Describes the customizations associated with the provided Amazon Web Services account and Amazon Amazon QuickSight namespace in an Amazon Web Services Region. The Amazon QuickSight console evaluates which customizations to apply by running this API operation with the <code>Resolved</code> flag included. </p> <p>To determine what customizations display when you run this command, it can help to visualize the relationship of the entities involved. </p> <ul> <li> <p> <code>Amazon Web Services account</code> - The Amazon Web Services account exists at the top of the hierarchy. It has the potential to use all of the Amazon Web Services Regions and Amazon Web Services Services. When you subscribe to Amazon QuickSight, you choose one Amazon Web Services Region to use as your home Region. That's where your free SPICE capacity is located. You can use Amazon QuickSight in any supported Amazon Web Services Region. </p> </li> <li> <p> <code>Amazon Web Services Region</code> - In each Amazon Web Services Region where you sign in to Amazon QuickSight at least once, Amazon QuickSight acts as a separate instance of the same service. If you have a user directory, it resides in us-east-1, which is the US East (N. Virginia). Generally speaking, these users have access to Amazon QuickSight in any Amazon Web Services Region, unless they are constrained to a namespace. </p> <p>To run the command in a different Amazon Web Services Region, you change your Region settings. If you're using the CLI, you can use one of the following options:</p> <ul> <li> <p>Use <a href=\"https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-options.html\">command line options</a>. </p> </li> <li> <p>Use <a href=\"https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-profiles.html\">named profiles</a>. </p> </li> <li> <p>Run <code>aws configure</code> to change your default Amazon Web Services Region. Use Enter to key the same settings for your keys. For more information, see <a href=\"https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html\">Configuring the CLI</a>.</p> </li> </ul> </li> <li> <p> <code>Namespace</code> - A QuickSight namespace is a partition that contains users and assets (data sources, datasets, dashboards, and so on). To access assets that are in a specific namespace, users and groups must also be part of the same namespace. People who share a namespace are completely isolated from users and assets in other namespaces, even if they are in the same Amazon Web Services account and Amazon Web Services Region.</p> </li> <li> <p> <code>Applied customizations</code> - Within an Amazon Web Services Region, a set of Amazon QuickSight customizations can apply to an Amazon Web Services account or to a namespace. Settings that you apply to a namespace override settings that you apply to an Amazon Web Services account. All settings are isolated to a single Amazon Web Services Region. To apply them in other Amazon Web Services Regions, run the <code>CreateAccountCustomization</code> command in each Amazon Web Services Region where you want to apply the same customizations. </p> </li> </ul>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -1579,14 +1921,64 @@
                 "shape": "DescribeAnalysisPermissionsRequest"
             },
             "name": "DescribeAnalysisPermissions",
             "output": {
                 "shape": "DescribeAnalysisPermissionsResponse"
             }
         },
+        "DescribeAssetBundleExportJob": {
+            "documentation": "<p>Describes an existing export job.</p> <p>Poll job descriptions after a job starts to know the status of the job. When a job succeeds, a URL is provided to download the exported assets' data from. Download URLs are valid for five minutes after they are generated. You can call the <code>DescribeAssetBundleExportJob</code> API for a new download URL as needed.</p> <p>Job descriptions are available for 14 days after the job starts.</p>",
+            "errors": [
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/asset-bundle-export-jobs/{AssetBundleExportJobId}"
+            },
+            "input": {
+                "shape": "DescribeAssetBundleExportJobRequest"
+            },
+            "name": "DescribeAssetBundleExportJob",
+            "output": {
+                "shape": "DescribeAssetBundleExportJobResponse"
+            }
+        },
+        "DescribeAssetBundleImportJob": {
+            "documentation": "<p>Describes an existing import job.</p> <p>Poll job descriptions after starting a job to know when it has succeeded or failed. Job descriptions are available for 14 days after job starts.</p>",
+            "errors": [
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/asset-bundle-import-jobs/{AssetBundleImportJobId}"
+            },
+            "input": {
+                "shape": "DescribeAssetBundleImportJobRequest"
+            },
+            "name": "DescribeAssetBundleImportJob",
+            "output": {
+                "shape": "DescribeAssetBundleImportJobResponse"
+            }
+        },
         "DescribeDashboard": {
             "documentation": "<p>Provides a summary for a dashboard.</p>",
             "errors": [
                 {
                     "shape": "InvalidParameterValueException"
                 },
                 {
@@ -1746,14 +2138,51 @@
                 "shape": "DescribeDataSetPermissionsRequest"
             },
             "name": "DescribeDataSetPermissions",
             "output": {
                 "shape": "DescribeDataSetPermissionsResponse"
             }
         },
+        "DescribeDataSetRefreshProperties": {
+            "documentation": "<p>Describes the refresh properties of a dataset.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "PreconditionNotMetException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/data-sets/{DataSetId}/refresh-properties"
+            },
+            "input": {
+                "shape": "DescribeDataSetRefreshPropertiesRequest"
+            },
+            "name": "DescribeDataSetRefreshProperties",
+            "output": {
+                "shape": "DescribeDataSetRefreshPropertiesResponse"
+            }
+        },
         "DescribeDataSource": {
             "documentation": "<p>Describes a data source.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -2117,14 +2546,48 @@
                 "shape": "DescribeNamespaceRequest"
             },
             "name": "DescribeNamespace",
             "output": {
                 "shape": "DescribeNamespaceResponse"
             }
         },
+        "DescribeRefreshSchedule": {
+            "documentation": "<p>Provides a summary of a refresh schedule.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/data-sets/{DataSetId}/refresh-schedules/{ScheduleId}"
+            },
+            "input": {
+                "shape": "DescribeRefreshScheduleRequest"
+            },
+            "name": "DescribeRefreshSchedule",
+            "output": {
+                "shape": "DescribeRefreshScheduleResponse"
+            }
+        },
         "DescribeTemplate": {
             "documentation": "<p>Describes a template's metadata.</p>",
             "errors": [
                 {
                     "shape": "InvalidParameterValueException"
                 },
                 {
@@ -2364,14 +2827,147 @@
                 "shape": "DescribeThemePermissionsRequest"
             },
             "name": "DescribeThemePermissions",
             "output": {
                 "shape": "DescribeThemePermissionsResponse"
             }
         },
+        "DescribeTopic": {
+            "documentation": "<p>Describes a topic.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}"
+            },
+            "input": {
+                "shape": "DescribeTopicRequest"
+            },
+            "name": "DescribeTopic",
+            "output": {
+                "shape": "DescribeTopicResponse"
+            }
+        },
+        "DescribeTopicPermissions": {
+            "documentation": "<p>Describes the permissions of a topic.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}/permissions"
+            },
+            "input": {
+                "shape": "DescribeTopicPermissionsRequest"
+            },
+            "name": "DescribeTopicPermissions",
+            "output": {
+                "shape": "DescribeTopicPermissionsResponse"
+            }
+        },
+        "DescribeTopicRefresh": {
+            "documentation": "<p>Describes the status of a topic refresh.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}/refresh/{RefreshId}"
+            },
+            "input": {
+                "shape": "DescribeTopicRefreshRequest"
+            },
+            "name": "DescribeTopicRefresh",
+            "output": {
+                "shape": "DescribeTopicRefreshResponse"
+            }
+        },
+        "DescribeTopicRefreshSchedule": {
+            "documentation": "<p>Deletes a topic refresh schedule.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}/schedules/{DatasetId}"
+            },
+            "input": {
+                "shape": "DescribeTopicRefreshScheduleRequest"
+            },
+            "name": "DescribeTopicRefreshSchedule",
+            "output": {
+                "shape": "DescribeTopicRefreshScheduleResponse"
+            }
+        },
         "DescribeUser": {
             "documentation": "<p>Returns information about a user, given the user name. </p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -2401,14 +2997,48 @@
                 "shape": "DescribeUserRequest"
             },
             "name": "DescribeUser",
             "output": {
                 "shape": "DescribeUserResponse"
             }
         },
+        "DescribeVPCConnection": {
+            "documentation": "<p>Describes a VPC connection.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/vpc-connections/{VPCConnectionId}"
+            },
+            "input": {
+                "shape": "DescribeVPCConnectionRequest"
+            },
+            "name": "DescribeVPCConnection",
+            "output": {
+                "shape": "DescribeVPCConnectionResponse"
+            }
+        },
         "GenerateEmbedUrlForAnonymousUser": {
             "documentation": "<p>Generates an embed URL that you can use to embed an Amazon QuickSight dashboard or visual in your website, without having to register any reader users. Before you use this action, make sure that you have configured the dashboards and permissions.</p> <p>The following rules apply to the generated URL:</p> <ul> <li> <p>It contains a temporary bearer token. It is valid for 5 minutes after it is generated. Once redeemed within this period, it cannot be re-used again.</p> </li> <li> <p>The URL validity period should not be confused with the actual session lifetime that can be customized using the <code> <a href=\"https://docs.aws.amazon.com/quicksight/latest/APIReference/API_GenerateEmbedUrlForAnonymousUser.html#QS-GenerateEmbedUrlForAnonymousUser-request-SessionLifetimeInMinutes\">SessionLifetimeInMinutes</a> </code> parameter. The resulting user session is valid for 15 minutes (minimum) to 10 hours (maximum). The default session duration is 10 hours.</p> </li> <li> <p>You are charged only when the URL is used or there is interaction with Amazon QuickSight.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/quicksight/latest/user/embedded-analytics.html\">Embedded Analytics</a> in the <i>Amazon QuickSight User Guide</i>.</p> <p>For more information about the high-level steps for embedding and for an interactive demo of the ways you can customize embedding, visit the <a href=\"https://docs.aws.amazon.com/quicksight/latest/user/quicksight-dev-portal.html\">Amazon QuickSight Developer Portal</a>.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -2607,14 +3237,76 @@
                 "shape": "ListAnalysesRequest"
             },
             "name": "ListAnalyses",
             "output": {
                 "shape": "ListAnalysesResponse"
             }
         },
+        "ListAssetBundleExportJobs": {
+            "documentation": "<p>Lists all asset bundle export jobs that have been taken place in the last 14 days. Jobs created more than 14 days ago are deleted forever and are not returned. If you are using the same job ID for multiple jobs, <code>ListAssetBundleExportJobs</code> only returns the most recent job that uses the repeated job ID.</p>",
+            "errors": [
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidNextTokenException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/asset-bundle-export-jobs"
+            },
+            "input": {
+                "shape": "ListAssetBundleExportJobsRequest"
+            },
+            "name": "ListAssetBundleExportJobs",
+            "output": {
+                "shape": "ListAssetBundleExportJobsResponse"
+            }
+        },
+        "ListAssetBundleImportJobs": {
+            "documentation": "<p>Lists all asset bundle import jobs that have taken place in the last 14 days. Jobs created more than 14 days ago are deleted forever and are not returned. If you are using the same job ID for multiple jobs, <code>ListAssetBundleImportJobs</code> only returns the most recent job that uses the repeated job ID.</p>",
+            "errors": [
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidNextTokenException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/asset-bundle-import-jobs"
+            },
+            "input": {
+                "shape": "ListAssetBundleImportJobsRequest"
+            },
+            "name": "ListAssetBundleImportJobs",
+            "output": {
+                "shape": "ListAssetBundleImportJobsResponse"
+            }
+        },
         "ListDashboardVersions": {
             "documentation": "<p>Lists all the versions of the dashboards in the Amazon QuickSight subscription.</p>",
             "errors": [
                 {
                     "shape": "InvalidParameterValueException"
                 },
                 {
@@ -2886,15 +3578,15 @@
             },
             "name": "ListGroups",
             "output": {
                 "shape": "ListGroupsResponse"
             }
         },
         "ListIAMPolicyAssignments": {
-            "documentation": "<p>Lists IAM policy assignments in the current Amazon QuickSight account.</p>",
+            "documentation": "<p>Lists the IAM policy assignments in the current Amazon QuickSight account.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "InvalidParameterValueException"
                 },
@@ -2909,26 +3601,26 @@
                 },
                 {
                     "shape": "InternalFailureException"
                 }
             ],
             "http": {
                 "method": "GET",
-                "requestUri": "/accounts/{AwsAccountId}/namespaces/{Namespace}/iam-policy-assignments"
+                "requestUri": "/accounts/{AwsAccountId}/namespaces/{Namespace}/v2/iam-policy-assignments"
             },
             "input": {
                 "shape": "ListIAMPolicyAssignmentsRequest"
             },
             "name": "ListIAMPolicyAssignments",
             "output": {
                 "shape": "ListIAMPolicyAssignmentsResponse"
             }
         },
         "ListIAMPolicyAssignmentsForUser": {
-            "documentation": "<p>Lists all the IAM policy assignments, including the Amazon Resource Names (ARNs) for the IAM policies assigned to the specified user and group or groups that the user belongs to.</p>",
+            "documentation": "<p>Lists all of the IAM policy assignments, including the Amazon Resource Names (ARNs), for the IAM policies assigned to the specified user and group, or groups that the user belongs to.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "InvalidParameterValueException"
                 },
@@ -3033,14 +3725,48 @@
                 "shape": "ListNamespacesRequest"
             },
             "name": "ListNamespaces",
             "output": {
                 "shape": "ListNamespacesResponse"
             }
         },
+        "ListRefreshSchedules": {
+            "documentation": "<p>Lists the refresh schedules of a dataset. Each dataset can have up to 5 schedules. </p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/data-sets/{DataSetId}/refresh-schedules"
+            },
+            "input": {
+                "shape": "ListRefreshSchedulesRequest"
+            },
+            "name": "ListRefreshSchedules",
+            "output": {
+                "shape": "ListRefreshSchedulesResponse"
+            }
+        },
         "ListTagsForResource": {
             "documentation": "<p>Lists the tags assigned to a resource.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -3274,14 +4000,85 @@
                 "shape": "ListThemesRequest"
             },
             "name": "ListThemes",
             "output": {
                 "shape": "ListThemesResponse"
             }
         },
+        "ListTopicRefreshSchedules": {
+            "documentation": "<p>Lists all of the refresh schedules for a topic.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}/schedules"
+            },
+            "input": {
+                "shape": "ListTopicRefreshSchedulesRequest"
+            },
+            "name": "ListTopicRefreshSchedules",
+            "output": {
+                "shape": "ListTopicRefreshSchedulesResponse"
+            }
+        },
+        "ListTopics": {
+            "documentation": "<p>Lists all of the topics within an account.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InvalidNextTokenException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/topics"
+            },
+            "input": {
+                "shape": "ListTopicsRequest"
+            },
+            "name": "ListTopics",
+            "output": {
+                "shape": "ListTopicsResponse"
+            }
+        },
         "ListUserGroups": {
             "documentation": "<p>Lists the Amazon QuickSight groups that an Amazon QuickSight user is a member of.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -3351,14 +4148,88 @@
                 "shape": "ListUsersRequest"
             },
             "name": "ListUsers",
             "output": {
                 "shape": "ListUsersResponse"
             }
         },
+        "ListVPCConnections": {
+            "documentation": "<p>Lists all of the VPC connections in the current set Amazon Web Services Region of an Amazon Web Services account.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InvalidNextTokenException"
+                },
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/accounts/{AwsAccountId}/vpc-connections"
+            },
+            "input": {
+                "shape": "ListVPCConnectionsRequest"
+            },
+            "name": "ListVPCConnections",
+            "output": {
+                "shape": "ListVPCConnectionsResponse"
+            }
+        },
+        "PutDataSetRefreshProperties": {
+            "documentation": "<p>Creates or updates the dataset refresh properties for the dataset.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "PreconditionNotMetException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "PUT",
+                "requestUri": "/accounts/{AwsAccountId}/data-sets/{DataSetId}/refresh-properties"
+            },
+            "input": {
+                "shape": "PutDataSetRefreshPropertiesRequest"
+            },
+            "name": "PutDataSetRefreshProperties",
+            "output": {
+                "shape": "PutDataSetRefreshPropertiesResponse"
+            }
+        },
         "RegisterUser": {
             "documentation": "<p>Creates an Amazon QuickSight user whose identity is associated with the Identity and Access Management (IAM) identity or role specified in the request. When you register a new user from the Amazon QuickSight API, Amazon QuickSight generates a registration URL. The user accesses this registration URL to create their account. Amazon QuickSight doesn't send a registration email to users who are registered from the Amazon QuickSight API. If you want new users to receive a registration email, then add those users in the Amazon QuickSight console. For more information on registering a new user in the Amazon QuickSight console, see <a href=\"https://docs.aws.amazon.com/quicksight/latest/user/managing-users.html#inviting-users\"> Inviting users to access Amazon QuickSight</a>.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -3644,16 +4515,90 @@
                 "shape": "SearchGroupsRequest"
             },
             "name": "SearchGroups",
             "output": {
                 "shape": "SearchGroupsResponse"
             }
         },
+        "StartAssetBundleExportJob": {
+            "documentation": "<p>Starts an Asset Bundle export job.</p> <p>An Asset Bundle export job exports specified Amazon QuickSight assets. You can also choose to export any asset dependencies in the same job. Export jobs run asynchronously and can be polled with a <code>DescribeAssetBundleExportJob</code> API call. When a job is successfully completed, a download URL that contains the exported assets is returned. The URL is valid for 5 minutes and can be refreshed with a <code>DescribeAssetBundleExportJob</code> API call. Each Amazon QuickSight account can run up to 10 export jobs concurrently.</p> <p>The API caller must have the necessary permissions in their IAM role to access each resource before the resources can be exported.</p>",
+            "errors": [
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/accounts/{AwsAccountId}/asset-bundle-export-jobs/export"
+            },
+            "input": {
+                "shape": "StartAssetBundleExportJobRequest"
+            },
+            "name": "StartAssetBundleExportJob",
+            "output": {
+                "shape": "StartAssetBundleExportJobResponse"
+            }
+        },
+        "StartAssetBundleImportJob": {
+            "documentation": "<p>Starts an Asset Bundle import job.</p> <p>An Asset Bundle import job imports specified Amazon QuickSight assets into an Amazon QuickSight account. You can also choose to import a naming prefix and specified configuration overrides. The assets that are contained in the bundle file that you provide are used to create or update a new or existing asset in your Amazon QuickSight account. Each Amazon QuickSight account can run up to 10 import jobs concurrently.</p> <p>The API caller must have the necessary <code>\"create\"</code>, <code>\"describe\"</code>, and <code>\"update\"</code> permissions in their IAM role to access each resource type that is contained in the bundle file before the resources can be imported.</p>",
+            "errors": [
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/accounts/{AwsAccountId}/asset-bundle-import-jobs/import"
+            },
+            "input": {
+                "shape": "StartAssetBundleImportJobRequest"
+            },
+            "name": "StartAssetBundleImportJob",
+            "output": {
+                "shape": "StartAssetBundleImportJobResponse"
+            }
+        },
         "TagResource": {
-            "documentation": "<p>Assigns one or more tags (key-value pairs) to the specified Amazon QuickSight resource. </p> <p>Tags can help you organize and categorize your resources. You can also use them to scope user permissions, by granting a user permission to access or change only resources with certain tag values. You can use the <code>TagResource</code> operation with a resource that already has tags. If you specify a new tag key for the resource, this tag is appended to the list of tags associated with the resource. If you specify a tag key that is already associated with the resource, the new tag value that you specify replaces the previous value for that tag.</p> <p>You can associate as many as 50 tags with a resource. Amazon QuickSight supports tagging on data set, data source, dashboard, and template. </p> <p>Tagging for Amazon QuickSight works in a similar way to tagging for other Amazon Web Services services, except for the following:</p> <ul> <li> <p>You can't use tags to track costs for Amazon QuickSight. This isn't possible because you can't tag the resources that Amazon QuickSight costs are based on, for example Amazon QuickSight storage capacity (SPICE), number of users, type of users, and usage metrics.</p> </li> <li> <p>Amazon QuickSight doesn't currently support the tag editor for Resource Groups.</p> </li> </ul>",
+            "documentation": "<p>Assigns one or more tags (key-value pairs) to the specified Amazon QuickSight resource. </p> <p>Tags can help you organize and categorize your resources. You can also use them to scope user permissions, by granting a user permission to access or change only resources with certain tag values. You can use the <code>TagResource</code> operation with a resource that already has tags. If you specify a new tag key for the resource, this tag is appended to the list of tags associated with the resource. If you specify a tag key that is already associated with the resource, the new tag value that you specify replaces the previous value for that tag.</p> <p>You can associate as many as 50 tags with a resource. Amazon QuickSight supports tagging on data set, data source, dashboard, template, and topic. </p> <p>Tagging for Amazon QuickSight works in a similar way to tagging for other Amazon Web Services services, except for the following:</p> <ul> <li> <p>You can't use tags to track costs for Amazon QuickSight. This isn't possible because you can't tag the resources that Amazon QuickSight costs are based on, for example Amazon QuickSight storage capacity (SPICE), number of users, type of users, and usage metrics.</p> </li> <li> <p>Amazon QuickSight doesn't currently support the tag editor for Resource Groups.</p> </li> </ul>",
             "errors": [
                 {
                     "shape": "LimitExceededException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -4256,15 +5201,15 @@
             },
             "name": "UpdateIAMPolicyAssignment",
             "output": {
                 "shape": "UpdateIAMPolicyAssignmentResponse"
             }
         },
         "UpdateIpRestriction": {
-            "documentation": "<p>Updates the content and status of IP rules. To use this operation, you need to provide the entire map of rules. You can use the <code>DescribeIpRestriction</code> operation to get the current rule map.</p>",
+            "documentation": "<p>Updates the content and status of IP rules. To use this operation, you must provide the entire map of rules. You can use the <code>DescribeIpRestriction</code> operation to get the current rule map.</p>",
             "errors": [
                 {
                     "shape": "LimitExceededException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -4323,14 +5268,51 @@
                 "shape": "UpdatePublicSharingSettingsRequest"
             },
             "name": "UpdatePublicSharingSettings",
             "output": {
                 "shape": "UpdatePublicSharingSettingsResponse"
             }
         },
+        "UpdateRefreshSchedule": {
+            "documentation": "<p>Updates a refresh schedule for a dataset.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "PreconditionNotMetException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "PUT",
+                "requestUri": "/accounts/{AwsAccountId}/data-sets/{DataSetId}/refresh-schedules"
+            },
+            "input": {
+                "shape": "UpdateRefreshScheduleRequest"
+            },
+            "name": "UpdateRefreshSchedule",
+            "output": {
+                "shape": "UpdateRefreshScheduleResponse"
+            }
+        },
         "UpdateTemplate": {
             "documentation": "<p>Updates a template from an existing Amazon QuickSight analysis or another template.</p>",
             "errors": [
                 {
                     "shape": "InvalidParameterValueException"
                 },
                 {
@@ -4548,14 +5530,134 @@
                 "shape": "UpdateThemePermissionsRequest"
             },
             "name": "UpdateThemePermissions",
             "output": {
                 "shape": "UpdateThemePermissionsResponse"
             }
         },
+        "UpdateTopic": {
+            "documentation": "<p>Updates a topic.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "PUT",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}"
+            },
+            "input": {
+                "shape": "UpdateTopicRequest"
+            },
+            "name": "UpdateTopic",
+            "output": {
+                "shape": "UpdateTopicResponse"
+            }
+        },
+        "UpdateTopicPermissions": {
+            "documentation": "<p>Updates the permissions of a topic.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "PUT",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}/permissions"
+            },
+            "input": {
+                "shape": "UpdateTopicPermissionsRequest"
+            },
+            "name": "UpdateTopicPermissions",
+            "output": {
+                "shape": "UpdateTopicPermissionsResponse"
+            }
+        },
+        "UpdateTopicRefreshSchedule": {
+            "documentation": "<p>Updates a topic refresh schedule.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ResourceExistsException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "PUT",
+                "requestUri": "/accounts/{AwsAccountId}/topics/{TopicId}/schedules/{DatasetId}"
+            },
+            "input": {
+                "shape": "UpdateTopicRefreshScheduleRequest"
+            },
+            "name": "UpdateTopicRefreshSchedule",
+            "output": {
+                "shape": "UpdateTopicRefreshScheduleResponse"
+            }
+        },
         "UpdateUser": {
             "documentation": "<p>Updates an Amazon QuickSight user.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
@@ -4584,14 +5686,54 @@
             "input": {
                 "shape": "UpdateUserRequest"
             },
             "name": "UpdateUser",
             "output": {
                 "shape": "UpdateUserResponse"
             }
+        },
+        "UpdateVPCConnection": {
+            "documentation": "<p>Updates a VPC connection.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InvalidParameterValueException"
+                },
+                {
+                    "shape": "LimitExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "UnsupportedUserEditionException"
+                },
+                {
+                    "shape": "InternalFailureException"
+                }
+            ],
+            "http": {
+                "method": "PUT",
+                "requestUri": "/accounts/{AwsAccountId}/vpc-connections/{VPCConnectionId}"
+            },
+            "input": {
+                "shape": "UpdateVPCConnectionRequest"
+            },
+            "name": "UpdateVPCConnection",
+            "output": {
+                "shape": "UpdateVPCConnectionResponse"
+            }
         }
     },
     "shapes": {
         "AccessDeniedException": {
             "documentation": "<p>You don't have access to this item. The provided credentials couldn't be validated. You might not be authorized to carry out the request. Make sure that your account is authorized to use the Amazon QuickSight service, that your policies have the correct permissions, and that you are using the correct credentials.</p>",
             "error": {
                 "httpStatusCode": 401
@@ -4738,14 +5880,23 @@
                 "NumericalAggregationFunction": {
                     "documentation": "<p>Aggregation for numerical values.</p>",
                     "shape": "NumericalAggregationFunction"
                 }
             },
             "type": "structure"
         },
+        "AggregationFunctionParameters": {
+            "key": {
+                "shape": "LimitedString"
+            },
+            "type": "map",
+            "value": {
+                "shape": "LimitedString"
+            }
+        },
         "AggregationSortConfiguration": {
             "documentation": "<p>The configuration options to sort aggregated values.</p>",
             "members": {
                 "AggregationFunction": {
                     "documentation": "<p>The function that aggregates the values in <code>Column</code>.</p>",
                     "shape": "AggregationFunction"
                 },
@@ -5201,14 +6352,836 @@
         },
         "ArnList": {
             "member": {
                 "shape": "Arn"
             },
             "type": "list"
         },
+        "AssetBundleCloudFormationOverridePropertyConfiguration": {
+            "documentation": "<p>An optional collection of CloudFormation property configurations that control how the export job is generated.</p>",
+            "members": {
+                "Analyses": {
+                    "documentation": "<p>An optional list of structures that control how <code>Analysis</code> resources are parameterized in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobAnalysisOverridePropertiesList"
+                },
+                "Dashboards": {
+                    "documentation": "<p>An optional list of structures that control how <code>Dashboard</code> resources are parameterized in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobDashboardOverridePropertiesList"
+                },
+                "DataSets": {
+                    "documentation": "<p>An optional list of structures that control how <code>DataSet</code> resources are parameterized in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobDataSetOverridePropertiesList"
+                },
+                "DataSources": {
+                    "documentation": "<p>An optional list of structures that control how <code>DataSource</code> resources are parameterized in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobDataSourceOverridePropertiesList"
+                },
+                "RefreshSchedules": {
+                    "documentation": "<p>An optional list of structures that control how <code>RefreshSchedule</code> resources are parameterized in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobRefreshScheduleOverridePropertiesList"
+                },
+                "ResourceIdOverrideConfiguration": {
+                    "documentation": "<p>An optional list of structures that control how resource IDs are parameterized in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobResourceIdOverrideConfiguration"
+                },
+                "Themes": {
+                    "documentation": "<p>An optional list of structures that control how <code>Theme</code> resources are parameterized in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobThemeOverridePropertiesList"
+                },
+                "VPCConnections": {
+                    "documentation": "<p>An optional list of structures that control how <code>VPCConnection</code> resources are parameterized in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobVPCConnectionOverridePropertiesList"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleExportFormat": {
+            "enum": [
+                "CLOUDFORMATION_JSON",
+                "QUICKSIGHT_JSON"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobAnalysisOverrideProperties": {
+            "documentation": "<p>Controls how a specific <code>Analysis</code> resource is parameterized in the returned CloudFormation template.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the specific <code>Analysis</code> resource whose override properties are configured in this structure.</p>",
+                    "shape": "Arn"
+                },
+                "Properties": {
+                    "documentation": "<p>A list of <code>Analysis</code> resource properties to generate variables for in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobAnalysisPropertyToOverrideList"
+                }
+            },
+            "required": [
+                "Properties"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleExportJobAnalysisOverridePropertiesList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleExportJobAnalysisOverrideProperties"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobAnalysisPropertyToOverride": {
+            "enum": [
+                "Name"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobAnalysisPropertyToOverrideList": {
+            "max": 10,
+            "member": {
+                "shape": "AssetBundleExportJobAnalysisPropertyToOverride"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobDashboardOverrideProperties": {
+            "documentation": "<p>Controls how a specific <code>Dashboard</code> resource is parameterized in the returned CloudFormation template.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the specific <code>Dashboard</code> resource whose override properties are configured in this structure.</p>",
+                    "shape": "Arn"
+                },
+                "Properties": {
+                    "documentation": "<p>A list of <code>Dashboard</code> resource properties to generate variables for in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobDashboardPropertyToOverrideList"
+                }
+            },
+            "required": [
+                "Properties"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleExportJobDashboardOverridePropertiesList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleExportJobDashboardOverrideProperties"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobDashboardPropertyToOverride": {
+            "enum": [
+                "Name"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobDashboardPropertyToOverrideList": {
+            "max": 10,
+            "member": {
+                "shape": "AssetBundleExportJobDashboardPropertyToOverride"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobDataSetOverrideProperties": {
+            "documentation": "<p>Controls how a specific <code>DataSet</code> resource is parameterized in the returned CloudFormation template.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the specific <code>DataSet</code> resource whose override properties are configured in this structure.</p>",
+                    "shape": "Arn"
+                },
+                "Properties": {
+                    "documentation": "<p>A list of <code>DataSet</code> resource properties to generate variables for in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobDataSetPropertyToOverrideList"
+                }
+            },
+            "required": [
+                "Properties"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleExportJobDataSetOverridePropertiesList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleExportJobDataSetOverrideProperties"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobDataSetPropertyToOverride": {
+            "enum": [
+                "Name"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobDataSetPropertyToOverrideList": {
+            "max": 10,
+            "member": {
+                "shape": "AssetBundleExportJobDataSetPropertyToOverride"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobDataSourceOverrideProperties": {
+            "documentation": "<p>Controls how a specific <code>DataSource</code> resource is parameterized in the returned CloudFormation template.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the specific <code>DataSource</code> resource whose override properties are configured in this structure.</p>",
+                    "shape": "Arn"
+                },
+                "Properties": {
+                    "documentation": "<p>A list of <code>DataSource</code> resource properties to generate variables for in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobDataSourcePropertyToOverrideList"
+                }
+            },
+            "required": [
+                "Properties"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleExportJobDataSourceOverridePropertiesList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleExportJobDataSourceOverrideProperties"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobDataSourcePropertyToOverride": {
+            "enum": [
+                "Name",
+                "DisableSsl",
+                "SecretArn",
+                "Username",
+                "Password",
+                "Domain",
+                "WorkGroup",
+                "Host",
+                "Port",
+                "Database",
+                "DataSetName",
+                "Catalog",
+                "InstanceId",
+                "ClusterId",
+                "ManifestFileLocation",
+                "Warehouse",
+                "RoleArn"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobDataSourcePropertyToOverrideList": {
+            "max": 10,
+            "member": {
+                "shape": "AssetBundleExportJobDataSourcePropertyToOverride"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobError": {
+            "documentation": "<p>Describes an error that occurred during an Asset Bundle export job.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the resource whose processing caused an error.</p>",
+                    "shape": "Arn"
+                },
+                "Message": {
+                    "documentation": "<p>A description of the error.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "Type": {
+                    "documentation": "<p>The specific error type of the error that occurred.</p>",
+                    "shape": "NonEmptyString"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleExportJobErrorList": {
+            "member": {
+                "shape": "AssetBundleExportJobError"
+            },
+            "type": "list"
+        },
+        "AssetBundleExportJobRefreshScheduleOverrideProperties": {
+            "documentation": "<p>Controls how a specific <code>RefreshSchedule</code> resource is parameterized in the returned CloudFormation template.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the specific <code>RefreshSchedule</code> resource whose override properties are configured in this structure.</p>",
+                    "shape": "Arn"
+                },
+                "Properties": {
+                    "documentation": "<p>A list of <code>RefreshSchedule</code> resource properties to generate variables for in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobRefreshSchedulePropertyToOverrideList"
+                }
+            },
+            "required": [
+                "Properties"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleExportJobRefreshScheduleOverridePropertiesList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleExportJobRefreshScheduleOverrideProperties"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobRefreshSchedulePropertyToOverride": {
+            "enum": [
+                "StartAfterDateTime"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobRefreshSchedulePropertyToOverrideList": {
+            "max": 10,
+            "member": {
+                "shape": "AssetBundleExportJobRefreshSchedulePropertyToOverride"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobResourceIdOverrideConfiguration": {
+            "documentation": "<p>An optional structure that configures resource ID overrides for the export job.</p>",
+            "members": {
+                "PrefixForAllResources": {
+                    "documentation": "<p>An option to request a CloudFormation variable for a prefix to be prepended to each resource's ID before import. The prefix is only added to the asset IDs and does not change the name of the asset.</p>",
+                    "shape": "Boolean"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleExportJobStatus": {
+            "enum": [
+                "QUEUED_FOR_IMMEDIATE_EXECUTION",
+                "IN_PROGRESS",
+                "SUCCESSFUL",
+                "FAILED"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobSummary": {
+            "documentation": "<p>A summary of the export job that includes details of the job's configuration and its current status.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the export job.</p>",
+                    "shape": "Arn"
+                },
+                "AssetBundleExportJobId": {
+                    "documentation": "<p>The ID of the export job.</p>",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "CreatedTime": {
+                    "documentation": "<p>The time that the export job was created.</p>",
+                    "shape": "Timestamp"
+                },
+                "ExportFormat": {
+                    "documentation": "<p>The format for the export job.</p>",
+                    "shape": "AssetBundleExportFormat"
+                },
+                "IncludeAllDependencies": {
+                    "documentation": "<p>The flag that determines the inclusion of resource dependencies in the returned asset bundle.</p>",
+                    "shape": "Boolean"
+                },
+                "JobStatus": {
+                    "documentation": "<p>The current status of the export job.</p>",
+                    "shape": "AssetBundleExportJobStatus"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleExportJobSummaryList": {
+            "member": {
+                "shape": "AssetBundleExportJobSummary"
+            },
+            "type": "list"
+        },
+        "AssetBundleExportJobThemeOverrideProperties": {
+            "documentation": "<p>Controls how a specific <code>Theme</code> resource is parameterized in the returned CloudFormation template.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the specific <code>Theme</code> resource whose override properties are configured in this structure.</p>",
+                    "shape": "Arn"
+                },
+                "Properties": {
+                    "documentation": "<p>A list of <code>Theme</code> resource properties to generate variables for in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobThemePropertyToOverrideList"
+                }
+            },
+            "required": [
+                "Properties"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleExportJobThemeOverridePropertiesList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleExportJobThemeOverrideProperties"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobThemePropertyToOverride": {
+            "enum": [
+                "Name"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobThemePropertyToOverrideList": {
+            "max": 10,
+            "member": {
+                "shape": "AssetBundleExportJobThemePropertyToOverride"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobVPCConnectionOverrideProperties": {
+            "documentation": "<p>Controls how a specific <code>VPCConnection</code> resource is parameterized in the outputted CloudFormation template.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the specific <code>VPCConnection</code> resource whose override properties are configured in this structure.</p>",
+                    "shape": "Arn"
+                },
+                "Properties": {
+                    "documentation": "<p>A list of <code>VPCConnection</code> resource properties to generate variables for in the returned CloudFormation template.</p>",
+                    "shape": "AssetBundleExportJobVPCConnectionPropertyToOverrideList"
+                }
+            },
+            "required": [
+                "Properties"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleExportJobVPCConnectionOverridePropertiesList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleExportJobVPCConnectionOverrideProperties"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleExportJobVPCConnectionPropertyToOverride": {
+            "enum": [
+                "Name",
+                "DnsResolvers",
+                "RoleArn"
+            ],
+            "type": "string"
+        },
+        "AssetBundleExportJobVPCConnectionPropertyToOverrideList": {
+            "max": 10,
+            "member": {
+                "shape": "AssetBundleExportJobVPCConnectionPropertyToOverride"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleImportBodyBlob": {
+            "max": 20971520,
+            "min": 0,
+            "sensitive": true,
+            "type": "blob"
+        },
+        "AssetBundleImportFailureAction": {
+            "enum": [
+                "DO_NOTHING",
+                "ROLLBACK"
+            ],
+            "type": "string"
+        },
+        "AssetBundleImportJobAnalysisOverrideParameters": {
+            "documentation": "<p>The override parameters for a single analysis that is being imported.</p>",
+            "members": {
+                "AnalysisId": {
+                    "documentation": "<p>The ID of the analysis that you ant to apply overrides to.</p>",
+                    "shape": "ResourceId"
+                },
+                "Name": {
+                    "documentation": "<p>A new name for the analysis.</p>",
+                    "shape": "ResourceName"
+                }
+            },
+            "required": [
+                "AnalysisId"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleImportJobAnalysisOverrideParametersList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleImportJobAnalysisOverrideParameters"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleImportJobDashboardOverrideParameters": {
+            "documentation": "<p>The override parameters for a single dashboard that is being imported.</p>",
+            "members": {
+                "DashboardId": {
+                    "documentation": "<p>The ID of the dashboard that you want to apply overrides to.</p>",
+                    "shape": "ResourceId"
+                },
+                "Name": {
+                    "documentation": "<p>A new name for the dashboard.</p>",
+                    "shape": "ResourceName"
+                }
+            },
+            "required": [
+                "DashboardId"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleImportJobDashboardOverrideParametersList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleImportJobDashboardOverrideParameters"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleImportJobDataSetOverrideParameters": {
+            "documentation": "<p>The override parameters for a single dataset that is being imported.</p>",
+            "members": {
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset to apply overrides to.</p>",
+                    "shape": "ResourceId"
+                },
+                "Name": {
+                    "documentation": "<p>A new name for the dataset.</p>",
+                    "shape": "ResourceName"
+                }
+            },
+            "required": [
+                "DataSetId"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleImportJobDataSetOverrideParametersList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleImportJobDataSetOverrideParameters"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleImportJobDataSourceCredentialPair": {
+            "documentation": "<p>A username and password credential pair to use to import a data source resource.</p>",
+            "members": {
+                "Password": {
+                    "documentation": "<p>The password for the data source connection.</p>",
+                    "shape": "Password"
+                },
+                "Username": {
+                    "documentation": "<p>The username for the data source connection.</p>",
+                    "shape": "DbUsername"
+                }
+            },
+            "required": [
+                "Username",
+                "Password"
+            ],
+            "sensitive": true,
+            "type": "structure"
+        },
+        "AssetBundleImportJobDataSourceCredentials": {
+            "documentation": "<p>The login credentials to use to import a data source resource.</p>",
+            "members": {
+                "CredentialPair": {
+                    "documentation": "<p>A username and password credential pair to be used to create the imported data source. Keep this field blank if you are using a Secrets Manager secret to provide credentials.</p>",
+                    "shape": "AssetBundleImportJobDataSourceCredentialPair"
+                },
+                "SecretArn": {
+                    "documentation": "<p>The ARN of the Secrets Manager secret that's used to create the imported data source. Keep this field blank, unless you are using a secret in place of a credential pair.</p>",
+                    "shape": "SecretArn"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleImportJobDataSourceOverrideParameters": {
+            "documentation": "<p>The override parameters for a single data source that is being imported.</p>",
+            "members": {
+                "Credentials": {
+                    "documentation": "<p>An optional structure that provides the credentials to be used to create the imported data source.</p>",
+                    "shape": "AssetBundleImportJobDataSourceCredentials"
+                },
+                "DataSourceId": {
+                    "documentation": "<p>The ID of the data source to apply overrides to.</p>",
+                    "shape": "ResourceId"
+                },
+                "DataSourceParameters": {
+                    "shape": "DataSourceParameters"
+                },
+                "Name": {
+                    "documentation": "<p>A new name for the data source.</p>",
+                    "shape": "ResourceName"
+                },
+                "SslProperties": {
+                    "shape": "SslProperties"
+                },
+                "VpcConnectionProperties": {
+                    "shape": "VpcConnectionProperties"
+                }
+            },
+            "required": [
+                "DataSourceId"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleImportJobDataSourceOverrideParametersList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleImportJobDataSourceOverrideParameters"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleImportJobError": {
+            "documentation": "<p>Describes an error that occurred within an Asset Bundle import execution.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the resource whose processing caused an error.</p>",
+                    "shape": "Arn"
+                },
+                "Message": {
+                    "documentation": "<p>A description of the error.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "Type": {
+                    "documentation": "<p>The specific error type or the error that occurred.</p>",
+                    "shape": "NonEmptyString"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleImportJobErrorList": {
+            "member": {
+                "shape": "AssetBundleImportJobError"
+            },
+            "type": "list"
+        },
+        "AssetBundleImportJobOverrideParameters": {
+            "documentation": "<p>A list of overrides that modify the asset bundle resource configuration before the resource is imported.</p>",
+            "members": {
+                "Analyses": {
+                    "documentation": "<p>A list of overrides for any <code>Analysis</code> resources that are present in the asset bundle that is imported.</p>",
+                    "shape": "AssetBundleImportJobAnalysisOverrideParametersList"
+                },
+                "Dashboards": {
+                    "documentation": "<p>A list of overrides for any <code>Dashboard</code> resources that are present in the asset bundle that is imported.</p>",
+                    "shape": "AssetBundleImportJobDashboardOverrideParametersList"
+                },
+                "DataSets": {
+                    "documentation": "<p>A list of overrides for any <code>DataSet</code> resources that are present in the asset bundle that is imported.</p>",
+                    "shape": "AssetBundleImportJobDataSetOverrideParametersList"
+                },
+                "DataSources": {
+                    "documentation": "<p> A list of overrides for any <code>DataSource</code> resources that are present in the asset bundle that is imported.</p>",
+                    "shape": "AssetBundleImportJobDataSourceOverrideParametersList"
+                },
+                "RefreshSchedules": {
+                    "documentation": "<p>A list of overrides for any <code>RefreshSchedule</code> resources that are present in the asset bundle that is imported.</p>",
+                    "shape": "AssetBundleImportJobRefreshScheduleOverrideParametersList"
+                },
+                "ResourceIdOverrideConfiguration": {
+                    "documentation": "<p>An optional structure that configures resource ID overrides to be applied within the import job.</p>",
+                    "shape": "AssetBundleImportJobResourceIdOverrideConfiguration"
+                },
+                "Themes": {
+                    "documentation": "<p>A list of overrides for any <code>Theme</code> resources that are present in the asset bundle that is imported.</p>",
+                    "shape": "AssetBundleImportJobThemeOverrideParametersList"
+                },
+                "VPCConnections": {
+                    "documentation": "<p>A list of overrides for any <code>VPCConnection</code> resources that are present in the asset bundle that is imported.</p>",
+                    "shape": "AssetBundleImportJobVPCConnectionOverrideParametersList"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleImportJobRefreshScheduleOverrideParameters": {
+            "documentation": "<p>A list of overrides for a specific <code>RefreshsSchedule</code> resource that is present in the asset bundle that is imported.</p>",
+            "members": {
+                "DataSetId": {
+                    "documentation": "<p>A partial identifier for the specific <code>RefreshSchedule</code> resource that is being overridden. This structure is used together with the <code>ScheduleID</code> structure.</p>",
+                    "shape": "ResourceId"
+                },
+                "ScheduleId": {
+                    "documentation": "<p>A partial identifier for the specific <code>RefreshSchedule</code> resource being overridden. This structure is used together with the <code>DataSetId</code> structure.</p>",
+                    "shape": "String"
+                },
+                "StartAfterDateTime": {
+                    "documentation": "<p>An override for the <code>StartAfterDateTime</code> of a <code>RefreshSchedule</code>. Make sure that the <code>StartAfterDateTime</code> is set to a time that takes place in the future.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "DataSetId",
+                "ScheduleId"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleImportJobRefreshScheduleOverrideParametersList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleImportJobRefreshScheduleOverrideParameters"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleImportJobResourceIdOverrideConfiguration": {
+            "documentation": "<p>An optional structure that configures resource ID overrides for the import job.</p>",
+            "members": {
+                "PrefixForAllResources": {
+                    "documentation": "<p>An option to request a CloudFormation variable for a prefix to be prepended to each resource's ID before import. The prefix is only added to the asset IDs and does not change the name of the asset.</p>",
+                    "shape": "String"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleImportJobStatus": {
+            "enum": [
+                "QUEUED_FOR_IMMEDIATE_EXECUTION",
+                "IN_PROGRESS",
+                "SUCCESSFUL",
+                "FAILED",
+                "FAILED_ROLLBACK_IN_PROGRESS",
+                "FAILED_ROLLBACK_COMPLETED",
+                "FAILED_ROLLBACK_ERROR"
+            ],
+            "type": "string"
+        },
+        "AssetBundleImportJobSummary": {
+            "documentation": "<p>A summary of the import job that includes details of the requested job's configuration and its current status.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN of the import job.</p>",
+                    "shape": "Arn"
+                },
+                "AssetBundleImportJobId": {
+                    "documentation": "<p>The ID of the job. This ID is unique while the job is running. After the job is completed, you can reuse this ID for another job.</p>",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "CreatedTime": {
+                    "documentation": "<p>The time that the import job was created.</p>",
+                    "shape": "Timestamp"
+                },
+                "FailureAction": {
+                    "documentation": "<p>The failure action for the import job.</p>",
+                    "shape": "AssetBundleImportFailureAction"
+                },
+                "JobStatus": {
+                    "documentation": "<p>The current status of the import job.</p>",
+                    "shape": "AssetBundleImportJobStatus"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleImportJobSummaryList": {
+            "member": {
+                "shape": "AssetBundleImportJobSummary"
+            },
+            "type": "list"
+        },
+        "AssetBundleImportJobThemeOverrideParameters": {
+            "documentation": "<p>The override parameters for a single theme that is imported.</p>",
+            "members": {
+                "Name": {
+                    "documentation": "<p>A new name for the theme.</p>",
+                    "shape": "ResourceName"
+                },
+                "ThemeId": {
+                    "documentation": "<p>The ID of the theme to apply overrides to.</p>",
+                    "shape": "ResourceId"
+                }
+            },
+            "required": [
+                "ThemeId"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleImportJobThemeOverrideParametersList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleImportJobThemeOverrideParameters"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleImportJobVPCConnectionOverrideParameters": {
+            "documentation": "<p>The override parameters for a single VPC connection that is imported.</p>",
+            "members": {
+                "DnsResolvers": {
+                    "documentation": "<p>An optional override of DNS resolvers to be used by the VPC connection.</p>",
+                    "shape": "DnsResolverList"
+                },
+                "Name": {
+                    "documentation": "<p>A new name for the VPC connection.</p>",
+                    "shape": "ResourceName"
+                },
+                "RoleArn": {
+                    "documentation": "<p>An optional override of the role ARN to be used by the VPC connection.</p>",
+                    "shape": "RoleArn"
+                },
+                "SecurityGroupIds": {
+                    "documentation": "<p>A new security group ID for the VPC connection you are importing. This field is required if you are importing the VPC connection from another Amazon Web Services account or Region.</p>",
+                    "shape": "SecurityGroupIdList"
+                },
+                "SubnetIds": {
+                    "documentation": "<p>A list of new subnet IDs for the VPC connection you are importing. This field is required if you are importing the VPC connection from another Amazon Web Services account or Region.</p>",
+                    "shape": "SubnetIdList"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC Connection to apply overrides to.</p>",
+                    "shape": "VPCConnectionResourceIdUnrestricted"
+                }
+            },
+            "required": [
+                "VPCConnectionId"
+            ],
+            "type": "structure"
+        },
+        "AssetBundleImportJobVPCConnectionOverrideParametersList": {
+            "max": 50,
+            "member": {
+                "shape": "AssetBundleImportJobVPCConnectionOverrideParameters"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AssetBundleImportSource": {
+            "documentation": "<p>The source of the asset bundle zip file that contains the data that you want to import.</p>",
+            "members": {
+                "Body": {
+                    "documentation": "<p>The bytes of the base64 encoded asset bundle import zip file. This file can't exceed 20 MB.</p> <p>If you are calling the API operations from the Amazon Web Services SDK for Java, JavaScript, Python, or PHP, the SDK encodes base64 automatically to allow the direct setting of the zip file's bytes. If you are using an SDK for a different language or receiving related errors, try to base64 encode your data.</p>",
+                    "shape": "AssetBundleImportBodyBlob"
+                },
+                "S3Uri": {
+                    "documentation": "<p>The Amazon S3 URI for an asset bundle import file that exists in an Amazon S3 bucket that the caller has read access to. The file must be a zip format file and can't exceed 20 MB.</p>",
+                    "shape": "S3Uri"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleImportSourceDescription": {
+            "documentation": "<p>A description of the import source that you provide at the start of an import job. This value is set to either <code>Body</code> or <code>S3Uri</code>, depending on how the <code>StartAssetBundleImportJobRequest</code> is configured.</p>",
+            "members": {
+                "Body": {
+                    "documentation": "<p>An HTTPS download URL for the provided asset bundle that you optionally provided at the start of the import job. This URL is valid for five minutes after issuance. Call <code>DescribeAssetBundleExportJob</code> again for a fresh URL if needed. The downloaded asset bundle is a <code>.qs</code> zip file.</p>",
+                    "shape": "String"
+                },
+                "S3Uri": {
+                    "documentation": "<p>The Amazon S3 URI that you provided at the start of the import job.</p>",
+                    "shape": "S3Uri"
+                }
+            },
+            "type": "structure"
+        },
+        "AssetBundleResourceArns": {
+            "max": 100,
+            "member": {
+                "shape": "Arn"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "AssignmentStatus": {
             "enum": [
                 "ENABLED",
                 "DRAFT",
                 "DISABLED"
             ],
             "type": "string"
@@ -5277,14 +7250,37 @@
             "enum": [
                 "IAM_AND_QUICKSIGHT",
                 "IAM_ONLY",
                 "ACTIVE_DIRECTORY"
             ],
             "type": "string"
         },
+        "AuthorSpecifiedAggregation": {
+            "enum": [
+                "COUNT",
+                "DISTINCT_COUNT",
+                "MIN",
+                "MAX",
+                "MEDIAN",
+                "SUM",
+                "AVERAGE",
+                "STDEV",
+                "STDEVP",
+                "VAR",
+                "VARP",
+                "PERCENTILE"
+            ],
+            "type": "string"
+        },
+        "AuthorSpecifiedAggregations": {
+            "member": {
+                "shape": "AuthorSpecifiedAggregation"
+            },
+            "type": "list"
+        },
         "AwsAccountId": {
             "max": 12,
             "min": 12,
             "pattern": "^[0-9]{12}$",
             "type": "string"
         },
         "AwsAndAccountId": {
@@ -5754,14 +7750,27 @@
                 "Layout": {
                     "documentation": "<p>The layout configuration of a body section.</p>",
                     "shape": "SectionLayoutConfiguration"
                 }
             },
             "type": "structure"
         },
+        "BookmarksConfigurations": {
+            "documentation": "<p>The bookmarks configuration of an embedded dashboard.</p>",
+            "members": {
+                "Enabled": {
+                    "documentation": "<p>A Boolean value that determines whether a user can bookmark an embedded dashboard.</p>",
+                    "shape": "Boolean"
+                }
+            },
+            "required": [
+                "Enabled"
+            ],
+            "type": "structure"
+        },
         "Boolean": {
             "type": "boolean"
         },
         "BooleanObject": {
             "type": "boolean"
         },
         "BorderStyle": {
@@ -5984,30 +7993,36 @@
             "members": {
                 "DataSetIdentifier": {
                     "documentation": "<p>The data set that is used in this calculated field.</p>",
                     "shape": "DataSetIdentifier"
                 },
                 "Expression": {
                     "documentation": "<p>The expression of the calculated field.</p>",
-                    "shape": "Expression"
+                    "shape": "CalculatedFieldExpression"
                 },
                 "Name": {
                     "documentation": "<p>The name of the calculated field.</p>",
                     "shape": "ColumnName"
                 }
             },
             "required": [
                 "DataSetIdentifier",
                 "Name",
                 "Expression"
             ],
             "type": "structure"
         },
+        "CalculatedFieldExpression": {
+            "max": 32000,
+            "min": 1,
+            "sensitive": true,
+            "type": "string"
+        },
         "CalculatedFields": {
-            "max": 100,
+            "max": 500,
             "member": {
                 "shape": "CalculatedField"
             },
             "type": "list"
         },
         "CalculatedMeasureField": {
             "documentation": "<p>The table calculation measure field for pivot tables.</p>",
@@ -6248,14 +8263,21 @@
                 "FilterListConfiguration": {
                     "documentation": "<p>A list of filter configurations. In the Amazon QuickSight console, this filter type is called a filter list.</p>",
                     "shape": "FilterListConfiguration"
                 }
             },
             "type": "structure"
         },
+        "CategoryFilterFunction": {
+            "enum": [
+                "EXACT",
+                "CONTAINS"
+            ],
+            "type": "string"
+        },
         "CategoryFilterMatchOperator": {
             "enum": [
                 "EQUALS",
                 "DOES_NOT_EQUAL",
                 "CONTAINS",
                 "DOES_NOT_CONTAIN",
                 "STARTS_WITH",
@@ -6265,25 +8287,53 @@
         },
         "CategoryFilterSelectAllOptions": {
             "enum": [
                 "FILTER_ALL_VALUES"
             ],
             "type": "string"
         },
+        "CategoryFilterType": {
+            "enum": [
+                "CUSTOM_FILTER",
+                "CUSTOM_FILTER_LIST",
+                "FILTER_LIST"
+            ],
+            "type": "string"
+        },
         "CategoryValue": {
             "max": 512,
             "type": "string"
         },
         "CategoryValueList": {
             "max": 100000,
             "member": {
                 "shape": "CategoryValue"
             },
             "type": "list"
         },
+        "CellValueSynonym": {
+            "documentation": "<p>A structure that represents the cell value synonym.</p>",
+            "members": {
+                "CellValue": {
+                    "documentation": "<p>The cell value.</p>",
+                    "shape": "LimitedString"
+                },
+                "Synonyms": {
+                    "documentation": "<p>Other names or aliases for the cell value.</p>",
+                    "shape": "StringList"
+                }
+            },
+            "type": "structure"
+        },
+        "CellValueSynonyms": {
+            "member": {
+                "shape": "CellValueSynonym"
+            },
+            "type": "list"
+        },
         "ChartAxisLabelOptions": {
             "documentation": "<p>The label options for an axis on a chart.</p>",
             "members": {
                 "AxisLabelOptions": {
                     "documentation": "<p>The label options for a chart axis.</p>",
                     "shape": "AxisLabelOptionsList"
                 },
@@ -6313,20 +8363,30 @@
             },
             "type": "structure"
         },
         "ClusterMarkerConfiguration": {
             "documentation": "<p>The cluster marker configuration of the geospatial map selected point style.</p>",
             "members": {
                 "ClusterMarker": {
-                    "documentation": "<p>The cluster marker that is a part of the cluster marker configuration</p>",
+                    "documentation": "<p>The cluster marker that is a part of the cluster marker configuration.</p>",
                     "shape": "ClusterMarker"
                 }
             },
             "type": "structure"
         },
+        "CollectiveConstant": {
+            "documentation": "<p>A structure that represents a collective constant.</p>",
+            "members": {
+                "ValueList": {
+                    "documentation": "<p>A list of values for the collective constant.</p>",
+                    "shape": "StringList"
+                }
+            },
+            "type": "structure"
+        },
         "ColorFillType": {
             "enum": [
                 "DISCRETE",
                 "GRADIENT"
             ],
             "type": "string"
         },
@@ -6391,14 +8451,21 @@
         "ColumnConfigurationList": {
             "max": 200,
             "member": {
                 "shape": "ColumnConfiguration"
             },
             "type": "list"
         },
+        "ColumnDataRole": {
+            "enum": [
+                "DIMENSION",
+                "MEASURE"
+            ],
+            "type": "string"
+        },
         "ColumnDataType": {
             "enum": [
                 "STRING",
                 "INTEGER",
                 "DECIMAL",
                 "DATETIME"
             ],
@@ -6565,14 +8632,22 @@
         "ColumnNameList": {
             "member": {
                 "shape": "String"
             },
             "min": 1,
             "type": "list"
         },
+        "ColumnOrderingType": {
+            "enum": [
+                "GREATER_IS_BETTER",
+                "LESSER_IS_BETTER",
+                "SPECIFIED"
+            ],
+            "type": "string"
+        },
         "ColumnRole": {
             "enum": [
                 "DIMENSION",
                 "MEASURE"
             ],
             "type": "string"
         },
@@ -6835,14 +8910,32 @@
                 }
             },
             "required": [
                 "VisualId"
             ],
             "type": "structure"
         },
+        "ComparativeOrder": {
+            "documentation": "<p>A structure that represents a comparative order.</p>",
+            "members": {
+                "SpecifedOrder": {
+                    "documentation": "<p>The list of columns to be used in the ordering.</p>",
+                    "shape": "StringList"
+                },
+                "TreatUndefinedSpecifiedValues": {
+                    "documentation": "<p>The treat of undefined specified values. Valid values for this structure are <code>LEAST</code> and <code>MOST</code>.</p>",
+                    "shape": "UndefinedSpecifiedValueType"
+                },
+                "UseOrdering": {
+                    "documentation": "<p>The ordering type for a column. Valid values for this structure are <code>GREATER_IS_BETTER</code>, <code>LESSER_IS_BETTER</code> and <code>SPECIFIED</code>.</p>",
+                    "shape": "ColumnOrderingType"
+                }
+            },
+            "type": "structure"
+        },
         "ComparisonConfiguration": {
             "documentation": "<p>The comparison display configuration of a KPI or gauge chart.</p>",
             "members": {
                 "ComparisonFormat": {
                     "documentation": "<p>The format of the comparison.</p>",
                     "shape": "ComparisonFormatConfiguration"
                 },
@@ -7109,14 +9202,22 @@
                 "RequestId": {
                     "documentation": "<p>The Amazon Web Services request ID for this request.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
+        "ConstantType": {
+            "enum": [
+                "SINGULAR",
+                "RANGE",
+                "COLLECTIVE"
+            ],
+            "type": "string"
+        },
         "ContributionAnalysisDefault": {
             "documentation": "<p>The contribution analysis visual display for a line, pie, or bar chart.</p>",
             "members": {
                 "ContributorDimensions": {
                     "documentation": "<p>The dimensions columns that are used in the contribution analysis, usually a list of <code>ColumnIdentifiers</code>.</p>",
                     "shape": "ContributorDimensionList"
                 },
@@ -7498,14 +9599,18 @@
                 "DataSetId": {
                     "documentation": "<p>An ID for the dataset that you want to create. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
                     "shape": "ResourceId"
                 },
                 "DataSetUsageConfiguration": {
                     "shape": "DataSetUsageConfiguration"
                 },
+                "DatasetParameters": {
+                    "documentation": "<p>The parameter declarations of the dataset.</p>",
+                    "shape": "DatasetParameterList"
+                },
                 "FieldFolders": {
                     "documentation": "<p>The folder that contains fields and nested subfolders for your dataset.</p>",
                     "shape": "FieldFolderMap"
                 },
                 "ImportMode": {
                     "documentation": "<p>Indicates whether you want to import the data into SPICE.</p>",
                     "shape": "DataSetImportMode"
@@ -7874,15 +9979,15 @@
                 }
             },
             "type": "structure"
         },
         "CreateIAMPolicyAssignmentRequest": {
             "members": {
                 "AssignmentName": {
-                    "documentation": "<p>The name of the assignment, also called a rule. It must be unique within an Amazon Web Services account.</p>",
+                    "documentation": "<p>The name of the assignment, also called a rule. The name must be unique within the Amazon Web Services account.</p>",
                     "shape": "IAMPolicyAssignmentName"
                 },
                 "AssignmentStatus": {
                     "documentation": "<p>The status of the assignment. Possible values are as follows:</p> <ul> <li> <p> <code>ENABLED</code> - Anything specified in this assignment is used when creating the data source.</p> </li> <li> <p> <code>DISABLED</code> - This assignment isn't used when creating the data source.</p> </li> <li> <p> <code>DRAFT</code> - This assignment is an unfinished draft and isn't used when creating the data source.</p> </li> </ul>",
                     "shape": "AssignmentStatus"
                 },
                 "AwsAccountId": {
@@ -7917,15 +10022,15 @@
         "CreateIAMPolicyAssignmentResponse": {
             "members": {
                 "AssignmentId": {
                     "documentation": "<p>The ID for the assignment.</p>",
                     "shape": "String"
                 },
                 "AssignmentName": {
-                    "documentation": "<p>The name of the assignment. This name must be unique within the Amazon Web Services account.</p>",
+                    "documentation": "<p>The name of the assignment. The name must be unique within the Amazon Web Services account.</p>",
                     "shape": "IAMPolicyAssignmentName"
                 },
                 "AssignmentStatus": {
                     "documentation": "<p>The status of the assignment. Possible values are as follows:</p> <ul> <li> <p> <code>ENABLED</code> - Anything specified in this assignment is used when creating the data source.</p> </li> <li> <p> <code>DISABLED</code> - This assignment isn't used when creating the data source.</p> </li> <li> <p> <code>DRAFT</code> - This assignment is an unfinished draft and isn't used when creating the data source.</p> </li> </ul>",
                     "shape": "AssignmentStatus"
                 },
                 "Identities": {
@@ -8064,14 +10169,62 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "CreateRefreshScheduleRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DataSetId",
+                    "shape": "ResourceId"
+                },
+                "Schedule": {
+                    "documentation": "<p>The refresh schedule.</p>",
+                    "shape": "RefreshSchedule"
+                }
+            },
+            "required": [
+                "DataSetId",
+                "AwsAccountId",
+                "Schedule"
+            ],
+            "type": "structure"
+        },
+        "CreateRefreshScheduleResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the refresh schedule.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "ScheduleId": {
+                    "documentation": "<p>The ID of the refresh schedule.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "CreateTemplateAliasRequest": {
             "members": {
                 "AliasName": {
                     "documentation": "<p>The name that you want to give to the template alias that you're creating. Don't start the alias name with the <code>$</code> character. Alias names that start with <code>$</code> are reserved by Amazon QuickSight. </p>",
                     "location": "uri",
                     "locationName": "AliasName",
                     "shape": "AliasName"
@@ -8319,28 +10472,220 @@
                 "VersionArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the new theme.</p>",
                     "shape": "Arn"
                 }
             },
             "type": "structure"
         },
+        "CreateTopicRefreshScheduleRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topic you're creating a refresh schedule for.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DatasetArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the dataset.</p>",
+                    "shape": "Arn"
+                },
+                "DatasetName": {
+                    "documentation": "<p>The name of the dataset.</p>",
+                    "shape": "String"
+                },
+                "RefreshSchedule": {
+                    "documentation": "<p>The definition of a refresh schedule.</p>",
+                    "shape": "TopicRefreshSchedule"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId",
+                "DatasetArn",
+                "RefreshSchedule"
+            ],
+            "type": "structure"
+        },
+        "CreateTopicRefreshScheduleResponse": {
+            "members": {
+                "DatasetArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the dataset.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "CreateTopicRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that you want to create a topic in.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "Tags": {
+                    "documentation": "<p>Contains a map of the key-value pairs for the resource tag or tags that are assigned to the dataset.</p>",
+                    "shape": "TagList"
+                },
+                "Topic": {
+                    "documentation": "<p>The definition of a topic to create.</p>",
+                    "shape": "TopicDetails"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID for the topic that you want to create. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId",
+                "Topic"
+            ],
+            "type": "structure"
+        },
+        "CreateTopicResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "RefreshArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic refresh.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID for the topic that you want to create. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "CreateVPCConnectionRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID of the account where you want to create a new VPC connection.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DnsResolvers": {
+                    "documentation": "<p>A list of IP addresses of DNS resolver endpoints for the VPC connection.</p>",
+                    "shape": "DnsResolverList"
+                },
+                "Name": {
+                    "documentation": "<p>The display name for the VPC connection.</p>",
+                    "shape": "ResourceName"
+                },
+                "RoleArn": {
+                    "documentation": "<p>The IAM role to associate with the VPC connection.</p>",
+                    "shape": "RoleArn"
+                },
+                "SecurityGroupIds": {
+                    "documentation": "<p>A list of security group IDs for the VPC connection.</p>",
+                    "shape": "SecurityGroupIdList"
+                },
+                "SubnetIds": {
+                    "documentation": "<p>A list of subnet IDs for the VPC connection.</p>",
+                    "shape": "SubnetIdList"
+                },
+                "Tags": {
+                    "documentation": "<p>A map of the key-value pairs for the resource tag or tags assigned to the VPC connection.</p>",
+                    "shape": "TagList"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC connection that you're creating. This ID is a unique identifier for each Amazon Web Services Region in an Amazon Web Services account.</p>",
+                    "shape": "VPCConnectionResourceIdRestricted"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "VPCConnectionId",
+                "Name",
+                "SubnetIds",
+                "SecurityGroupIds",
+                "RoleArn"
+            ],
+            "type": "structure"
+        },
+        "CreateVPCConnectionResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the VPC connection.</p>",
+                    "shape": "Arn"
+                },
+                "AvailabilityStatus": {
+                    "documentation": "<p>The availability status of the VPC connection.</p>",
+                    "shape": "VPCConnectionAvailabilityStatus"
+                },
+                "CreationStatus": {
+                    "documentation": "<p>The status of the creation of the VPC connection.</p>",
+                    "shape": "VPCConnectionResourceStatus"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID for the VPC connection that you're creating. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "VPCConnectionResourceIdRestricted"
+                }
+            },
+            "type": "structure"
+        },
         "CredentialPair": {
             "documentation": "<p>The combination of user name and password that are used as credentials.</p>",
             "members": {
                 "AlternateDataSourceParameters": {
                     "documentation": "<p>A set of alternate data source parameters that you want to share for these credentials. The credentials are applied in tandem with the data source parameters when you copy a data source by using a create or update request. The API operation compares the <code>DataSourceParameters</code> structure that's in the request with the structures in the <code>AlternateDataSourceParameters</code> allow list. If the structures are an exact match, the request is allowed to use the new data source with the existing credentials. If the <code>AlternateDataSourceParameters</code> list is null, the <code>DataSourceParameters</code> originally used with these <code>Credentials</code> is automatically allowed.</p>",
                     "shape": "DataSourceParametersList"
                 },
                 "Password": {
                     "documentation": "<p>Password.</p>",
                     "shape": "Password"
                 },
                 "Username": {
                     "documentation": "<p>User name.</p>",
-                    "shape": "Username"
+                    "shape": "DbUsername"
                 }
             },
             "required": [
                 "Username",
                 "Password"
             ],
             "type": "structure"
@@ -8390,14 +10735,21 @@
                 "Symbol": {
                     "documentation": "<p>Determines the symbol for the currency format.</p>",
                     "shape": "CurrencyCode"
                 }
             },
             "type": "structure"
         },
+        "CustomActionColumnList": {
+            "max": 10,
+            "member": {
+                "shape": "ColumnIdentifier"
+            },
+            "type": "list"
+        },
         "CustomActionFilterOperation": {
             "documentation": "<p>The filter operation that filters data included in a visual or in an entire sheet.</p>",
             "members": {
                 "SelectedFieldsConfiguration": {
                     "documentation": "<p>The configuration that chooses the fields to be filtered.</p>",
                     "shape": "FilterOperationSelectedFieldsConfiguration"
                 },
@@ -9068,14 +11420,28 @@
                 "ExportHiddenFieldsOption": {
                     "documentation": "<p>Determines if hidden fields are included in an exported dashboard.</p>",
                     "shape": "ExportHiddenFieldsOption"
                 }
             },
             "type": "structure"
         },
+        "DataAggregation": {
+            "documentation": "<p>A structure that represents a data aggregation.</p>",
+            "members": {
+                "DatasetRowDateGranularity": {
+                    "documentation": "<p>The level of time precision that is used to aggregate <code>DateTime</code> values.</p>",
+                    "shape": "TopicTimeGranularity"
+                },
+                "DefaultDateColumnName": {
+                    "documentation": "<p>The column name for the default date.</p>",
+                    "shape": "LimitedString"
+                }
+            },
+            "type": "structure"
+        },
         "DataBarsOptions": {
             "documentation": "<p>The options for data bars.</p>",
             "members": {
                 "FieldId": {
                     "documentation": "<p>The field ID for the data bars options.</p>",
                     "shape": "FieldId"
                 },
@@ -9191,14 +11557,18 @@
                     "documentation": "<p>Determines whether overlap is enabled or disabled for the data labels.</p>",
                     "shape": "DataLabelOverlap"
                 },
                 "Position": {
                     "documentation": "<p>Determines the position of the data labels.</p>",
                     "shape": "DataLabelPosition"
                 },
+                "TotalsVisibility": {
+                    "documentation": "<p>Determines the visibility of the total.</p>",
+                    "shape": "Visibility"
+                },
                 "Visibility": {
                     "documentation": "<p>Determines the visibility of the data labels.</p>",
                     "shape": "Visibility"
                 }
             },
             "type": "structure"
         },
@@ -9400,14 +11770,18 @@
                     "documentation": "<p>The ID of the dataset.</p>",
                     "shape": "ResourceId"
                 },
                 "DataSetUsageConfiguration": {
                     "documentation": "<p>The usage configuration to apply to child datasets that reference this dataset as a source.</p>",
                     "shape": "DataSetUsageConfiguration"
                 },
+                "DatasetParameters": {
+                    "documentation": "<p>The parameters that are declared in a dataset.</p>",
+                    "shape": "DatasetParameterList"
+                },
                 "FieldFolders": {
                     "documentation": "<p>The folder that contains fields and nested subfolders for your dataset.</p>",
                     "shape": "FieldFolderMap"
                 },
                 "ImportMode": {
                     "documentation": "<p>A value that indicates whether you want to import the data into SPICE.</p>",
                     "shape": "DataSetImportMode"
@@ -9550,14 +11924,27 @@
         "DataSetReferenceList": {
             "member": {
                 "shape": "DataSetReference"
             },
             "min": 1,
             "type": "list"
         },
+        "DataSetRefreshProperties": {
+            "documentation": "<p>The refresh properties of a dataset.</p>",
+            "members": {
+                "RefreshConfiguration": {
+                    "documentation": "<p>The refresh configuration for a dataset.</p>",
+                    "shape": "RefreshConfiguration"
+                }
+            },
+            "required": [
+                "RefreshConfiguration"
+            ],
+            "type": "structure"
+        },
         "DataSetSchema": {
             "documentation": "<p>Dataset schema.</p>",
             "members": {
                 "ColumnSchemaList": {
                     "documentation": "<p>A structure containing the list of column schemas.</p>",
                     "shape": "ColumnSchemaList"
                 }
@@ -10004,14 +12391,110 @@
             "required": [
                 "Host",
                 "Port",
                 "SqlEndpointPath"
             ],
             "type": "structure"
         },
+        "DatasetMetadata": {
+            "documentation": "<p>A structure that represents a dataset.</p>",
+            "members": {
+                "CalculatedFields": {
+                    "documentation": "<p>The list of calculated field definitions.</p>",
+                    "shape": "TopicCalculatedFields"
+                },
+                "Columns": {
+                    "documentation": "<p>The list of column definitions.</p>",
+                    "shape": "TopicColumns"
+                },
+                "DataAggregation": {
+                    "documentation": "<p>The definition of a data aggregation.</p>",
+                    "shape": "DataAggregation"
+                },
+                "DatasetArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the dataset.</p>",
+                    "shape": "Arn"
+                },
+                "DatasetDescription": {
+                    "documentation": "<p>The description of the dataset.</p>",
+                    "shape": "LimitedString"
+                },
+                "DatasetName": {
+                    "documentation": "<p>The name of the dataset.</p>",
+                    "shape": "LimitedString"
+                },
+                "Filters": {
+                    "documentation": "<p>The list of filter definitions.</p>",
+                    "shape": "TopicFilters"
+                },
+                "NamedEntities": {
+                    "documentation": "<p>The list of named entities definitions.</p>",
+                    "shape": "TopicNamedEntities"
+                }
+            },
+            "required": [
+                "DatasetArn"
+            ],
+            "type": "structure"
+        },
+        "DatasetParameter": {
+            "documentation": "<p>A dataset parameter.</p>",
+            "members": {
+                "DateTimeDatasetParameter": {
+                    "documentation": "<p>A date time parameter that is created in the dataset.</p>",
+                    "shape": "DateTimeDatasetParameter"
+                },
+                "DecimalDatasetParameter": {
+                    "documentation": "<p>A decimal parameter that is created in the dataset.</p>",
+                    "shape": "DecimalDatasetParameter"
+                },
+                "IntegerDatasetParameter": {
+                    "documentation": "<p>An integer parameter that is created in the dataset.</p>",
+                    "shape": "IntegerDatasetParameter"
+                },
+                "StringDatasetParameter": {
+                    "documentation": "<p>A string parameter that is created in the dataset.</p>",
+                    "shape": "StringDatasetParameter"
+                }
+            },
+            "type": "structure"
+        },
+        "DatasetParameterId": {
+            "max": 128,
+            "min": 1,
+            "pattern": "^[a-zA-Z0-9-]+$",
+            "type": "string"
+        },
+        "DatasetParameterList": {
+            "max": 32,
+            "member": {
+                "shape": "DatasetParameter"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "DatasetParameterName": {
+            "max": 2048,
+            "min": 1,
+            "pattern": "^[a-zA-Z0-9]+$",
+            "type": "string"
+        },
+        "DatasetParameterValueType": {
+            "enum": [
+                "MULTI_VALUED",
+                "SINGLE_VALUED"
+            ],
+            "type": "string"
+        },
+        "Datasets": {
+            "member": {
+                "shape": "DatasetMetadata"
+            },
+            "type": "list"
+        },
         "DateAggregationFunction": {
             "enum": [
                 "COUNT",
                 "DISTINCT_COUNT",
                 "MIN",
                 "MAX"
             ],
@@ -10079,14 +12562,67 @@
             },
             "required": [
                 "FieldId",
                 "Column"
             ],
             "type": "structure"
         },
+        "DateTimeDatasetParameter": {
+            "documentation": "<p>A date time parameter for a dataset.</p>",
+            "members": {
+                "DefaultValues": {
+                    "documentation": "<p>A list of default values for a given date time parameter. This structure only accepts static values.</p>",
+                    "shape": "DateTimeDatasetParameterDefaultValues"
+                },
+                "Id": {
+                    "documentation": "<p>An identifier for the parameter that is created in the dataset.</p>",
+                    "shape": "DatasetParameterId"
+                },
+                "Name": {
+                    "documentation": "<p>The name of the date time parameter that is created in the dataset.</p>",
+                    "shape": "DatasetParameterName"
+                },
+                "TimeGranularity": {
+                    "documentation": "<p>The time granularity of the date time parameter.</p>",
+                    "shape": "TimeGranularity"
+                },
+                "ValueType": {
+                    "documentation": "<p>The value type of the dataset parameter. Valid values are <code>single value</code> or <code>multi value</code>.</p>",
+                    "shape": "DatasetParameterValueType"
+                }
+            },
+            "required": [
+                "Id",
+                "Name",
+                "ValueType"
+            ],
+            "type": "structure"
+        },
+        "DateTimeDatasetParameterDefaultValue": {
+            "documentation": "<p>The default value for the date time parameter.</p>",
+            "type": "timestamp"
+        },
+        "DateTimeDatasetParameterDefaultValues": {
+            "documentation": "<p>The default values of a date time parameter.</p>",
+            "members": {
+                "StaticValues": {
+                    "documentation": "<p>A list of static default values for a given date time parameter.</p>",
+                    "shape": "DateTimeDatasetParameterValueList"
+                }
+            },
+            "type": "structure"
+        },
+        "DateTimeDatasetParameterValueList": {
+            "max": 32,
+            "member": {
+                "shape": "DateTimeDatasetParameterDefaultValue"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "DateTimeDefaultValueList": {
             "max": 50000,
             "member": {
                 "shape": "SensitiveTimestamp"
             },
             "type": "list"
         },
@@ -10169,14 +12705,17 @@
         "DateTimeParameterDeclaration": {
             "documentation": "<p>A parameter declaration for the <code>DateTime</code> data type.</p>",
             "members": {
                 "DefaultValues": {
                     "documentation": "<p>The default values of a parameter. If the parameter is a single-value parameter, a maximum of one default value can be provided.</p>",
                     "shape": "DateTimeDefaultValues"
                 },
+                "MappedDataSetParameters": {
+                    "shape": "MappedDataSetParameters"
+                },
                 "Name": {
                     "documentation": "<p>The name of the parameter that is being declared.</p>",
                     "shape": "ParameterName"
                 },
                 "TimeGranularity": {
                     "documentation": "<p>The level of time precision that is used to aggregate <code>DateTime</code> values.</p>",
                     "shape": "TimeGranularity"
@@ -10222,14 +12761,86 @@
                 "ValueWhenUnsetOption": {
                     "documentation": "<p>The built-in options for default values. The value can be one of the following:</p> <ul> <li> <p> <code>RECOMMENDED</code>: The recommended value.</p> </li> <li> <p> <code>NULL</code>: The <code>NULL</code> value.</p> </li> </ul>",
                     "shape": "ValueWhenUnsetOption"
                 }
             },
             "type": "structure"
         },
+        "DayOfMonth": {
+            "max": 17,
+            "min": 1,
+            "pattern": "^(?:LAST_DAY_OF_MONTH|1[0-9]|2[0-8]|[12]|[3-9])$",
+            "type": "string"
+        },
+        "DayOfWeek": {
+            "enum": [
+                "SUNDAY",
+                "MONDAY",
+                "TUESDAY",
+                "WEDNESDAY",
+                "THURSDAY",
+                "FRIDAY",
+                "SATURDAY"
+            ],
+            "type": "string"
+        },
+        "DbUsername": {
+            "max": 64,
+            "min": 1,
+            "type": "string"
+        },
+        "DecimalDatasetParameter": {
+            "documentation": "<p>A decimal parameter for a dataset.</p>",
+            "members": {
+                "DefaultValues": {
+                    "documentation": "<p>A list of default values for a given decimal parameter. This structure only accepts static values.</p>",
+                    "shape": "DecimalDatasetParameterDefaultValues"
+                },
+                "Id": {
+                    "documentation": "<p>An identifier for the decimal parameter created in the dataset.</p>",
+                    "shape": "DatasetParameterId"
+                },
+                "Name": {
+                    "documentation": "<p>The name of the decimal parameter that is created in the dataset.</p>",
+                    "shape": "DatasetParameterName"
+                },
+                "ValueType": {
+                    "documentation": "<p>The value type of the dataset parameter. Valid values are <code>single value</code> or <code>multi value</code>.</p>",
+                    "shape": "DatasetParameterValueType"
+                }
+            },
+            "required": [
+                "Id",
+                "Name",
+                "ValueType"
+            ],
+            "type": "structure"
+        },
+        "DecimalDatasetParameterDefaultValue": {
+            "documentation": "<p>The default value for the decimal parameter.</p>",
+            "type": "double"
+        },
+        "DecimalDatasetParameterDefaultValues": {
+            "documentation": "<p>The default values of a decimal parameter.</p>",
+            "members": {
+                "StaticValues": {
+                    "documentation": "<p>A list of static default values for a given decimal parameter.</p>",
+                    "shape": "DecimalDatasetParameterValueList"
+                }
+            },
+            "type": "structure"
+        },
+        "DecimalDatasetParameterValueList": {
+            "max": 32,
+            "member": {
+                "shape": "DecimalDatasetParameterDefaultValue"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "DecimalDefaultValueList": {
             "max": 50000,
             "member": {
                 "shape": "SensitiveDoubleObject"
             },
             "type": "list"
         },
@@ -10268,14 +12879,17 @@
         "DecimalParameterDeclaration": {
             "documentation": "<p>A parameter declaration for the <code>Decimal</code> data type.</p>",
             "members": {
                 "DefaultValues": {
                     "documentation": "<p>The default values of a parameter. If the parameter is a single-value parameter, a maximum of one default value can be provided.</p>",
                     "shape": "DecimalDefaultValues"
                 },
+                "MappedDataSetParameters": {
+                    "shape": "MappedDataSetParameters"
+                },
                 "Name": {
                     "documentation": "<p>The name of the parameter that is being declared.</p>",
                     "shape": "ParameterName"
                 },
                 "ParameterValueType": {
                     "documentation": "<p>The value type determines whether the parameter is a single-value or multi-value parameter.</p>",
                     "shape": "ParameterValueType"
@@ -10327,14 +12941,39 @@
                 "ValueWhenUnsetOption": {
                     "documentation": "<p>The built-in options for default values. The value can be one of the following:</p> <ul> <li> <p> <code>RECOMMENDED</code>: The recommended value.</p> </li> <li> <p> <code>NULL</code>: The <code>NULL</code> value.</p> </li> </ul>",
                     "shape": "ValueWhenUnsetOption"
                 }
             },
             "type": "structure"
         },
+        "DefaultAggregation": {
+            "enum": [
+                "SUM",
+                "MAX",
+                "MIN",
+                "COUNT",
+                "DISTINCT_COUNT",
+                "AVERAGE"
+            ],
+            "type": "string"
+        },
+        "DefaultFormatting": {
+            "documentation": "<p>A structure that represents a default formatting definition.</p>",
+            "members": {
+                "DisplayFormat": {
+                    "documentation": "<p>The display format. Valid values for this structure are <code>AUTO</code>, <code>PERCENT</code>, <code>CURRENCY</code>, <code>NUMBER</code>, <code>DATE</code>, and <code>STRING</code>.</p>",
+                    "shape": "DisplayFormat"
+                },
+                "DisplayFormatOptions": {
+                    "documentation": "<p>The additional options for display formatting.</p>",
+                    "shape": "DisplayFormatOptions"
+                }
+            },
+            "type": "structure"
+        },
         "DefaultFreeFormLayoutConfiguration": {
             "documentation": "<p>The options that determine the default settings of a free-form layout configuration.</p>",
             "members": {
                 "CanvasSizeOptions": {
                     "documentation": "<p>Determines the screen canvas size options for a free-form layout.</p>",
                     "shape": "FreeFormLayoutCanvasSizeOptions"
                 }
@@ -10578,14 +13217,49 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "DeleteDataSetRefreshPropertiesRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DataSetId",
+                    "shape": "ResourceId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "DataSetId"
+            ],
+            "type": "structure"
+        },
+        "DeleteDataSetRefreshPropertiesResponse": {
+            "members": {
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "DeleteDataSetRequest": {
             "members": {
                 "AwsAccountId": {
                     "documentation": "<p>The Amazon Web Services account ID.</p>",
                     "location": "uri",
                     "locationName": "AwsAccountId",
                     "shape": "AwsAccountId"
@@ -10927,14 +13601,64 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "DeleteRefreshScheduleRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DataSetId",
+                    "shape": "ResourceId"
+                },
+                "ScheduleId": {
+                    "documentation": "<p>The ID of the refresh schedule.</p>",
+                    "location": "uri",
+                    "locationName": "ScheduleId",
+                    "shape": "String"
+                }
+            },
+            "required": [
+                "DataSetId",
+                "AwsAccountId",
+                "ScheduleId"
+            ],
+            "type": "structure"
+        },
+        "DeleteRefreshScheduleResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the refresh schedule.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "ScheduleId": {
+                    "documentation": "<p>The ID of the refresh schedule.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "DeleteTemplateAliasRequest": {
             "members": {
                 "AliasName": {
                     "documentation": "<p>The name for the template alias. To delete a specific alias, you delete the version that the alias points to. You can specify the alias name, or specify the latest version of the template by providing the keyword <code>$LATEST</code> in the <code>AliasName</code> parameter. </p>",
                     "location": "uri",
                     "locationName": "AliasName",
                     "shape": "AliasName"
@@ -11133,14 +13857,111 @@
                 "ThemeId": {
                     "documentation": "<p>An ID for the theme.</p>",
                     "shape": "ShortRestrictiveResourceId"
                 }
             },
             "type": "structure"
         },
+        "DeleteTopicRefreshScheduleRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DatasetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DatasetId",
+                    "shape": "String"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId",
+                "DatasetId"
+            ],
+            "type": "structure"
+        },
+        "DeleteTopicRefreshScheduleResponse": {
+            "members": {
+                "DatasetArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the dataset.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "DeleteTopicRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topic that you want to delete.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to delete. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId"
+            ],
+            "type": "structure"
+        },
+        "DeleteTopicResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to delete. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
         "DeleteUserByPrincipalIdRequest": {
             "documentation": "<p/>",
             "members": {
                 "AwsAccountId": {
                     "documentation": "<p>The ID for the Amazon Web Services account that the user is in. Currently, you use the ID for the Amazon Web Services account that contains your Amazon QuickSight account.</p>",
                     "location": "uri",
                     "locationName": "AwsAccountId",
@@ -11218,14 +14039,65 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "DeleteVPCConnectionRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID of the account where you want to delete a VPC connection.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC connection that you're creating. This ID is a unique identifier for each Amazon Web Services Region in an Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "VPCConnectionId",
+                    "shape": "VPCConnectionResourceIdUnrestricted"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "VPCConnectionId"
+            ],
+            "type": "structure"
+        },
+        "DeleteVPCConnectionResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the deleted VPC connection.</p>",
+                    "shape": "Arn"
+                },
+                "AvailabilityStatus": {
+                    "documentation": "<p>The availability status of the VPC connection.</p>",
+                    "shape": "VPCConnectionAvailabilityStatus"
+                },
+                "DeletionStatus": {
+                    "documentation": "<p>The deletion status of the VPC connection.</p>",
+                    "shape": "VPCConnectionResourceStatus"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC connection that you're creating. This ID is a unique identifier for each Amazon Web Services Region in an Amazon Web Services account.</p>",
+                    "shape": "VPCConnectionResourceIdUnrestricted"
+                }
+            },
+            "type": "structure"
+        },
         "Delimiter": {
             "max": 1,
             "min": 1,
             "type": "string"
         },
         "DescribeAccountCustomizationRequest": {
             "members": {
@@ -11488,14 +14360,168 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "DescribeAssetBundleExportJobRequest": {
+            "members": {
+                "AssetBundleExportJobId": {
+                    "documentation": "<p>The ID of the job that you want described. The job ID is set when you start a new job with a <code>StartAssetBundleExportJob</code> API call.</p>",
+                    "location": "uri",
+                    "locationName": "AssetBundleExportJobId",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account the export job is executed in. </p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "AssetBundleExportJobId"
+            ],
+            "type": "structure"
+        },
+        "DescribeAssetBundleExportJobResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the export job.</p>",
+                    "shape": "Arn"
+                },
+                "AssetBundleExportJobId": {
+                    "documentation": "<p>The ID of the job. The job ID is set when you start a new job with a <code>StartAssetBundleExportJob</code> API call.</p>",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that the export job was executed in. </p>",
+                    "shape": "AwsAccountId"
+                },
+                "CloudFormationOverridePropertyConfiguration": {
+                    "documentation": "<p>The CloudFormation override property configuration for the export job.</p>",
+                    "shape": "AssetBundleCloudFormationOverridePropertyConfiguration"
+                },
+                "CreatedTime": {
+                    "documentation": "<p>The time that the export job was created.</p>",
+                    "shape": "Timestamp"
+                },
+                "DownloadUrl": {
+                    "documentation": "<p>The URL to download the exported asset bundle data from.</p> <p>This URL is available only after the job has succeeded. This URL is valid for 5 minutes after issuance. Call <code>DescribeAssetBundleExportJob</code> again for a fresh URL if needed.</p> <p>The downloaded asset bundle is a zip file named <code>assetbundle-{jobId}.qs</code>. The file has a <code>.qs</code> extension.</p> <p>This URL can't be used in a <code>StartAssetBundleImportJob</code> API call and should only be used for download purposes.</p>",
+                    "shape": "String"
+                },
+                "Errors": {
+                    "documentation": "<p>An array of error records that describes any failures that occurred during the export job processing.</p> <p>Error records accumulate while the job runs. The complete set of error records is available after the job has completed and failed.</p>",
+                    "shape": "AssetBundleExportJobErrorList"
+                },
+                "ExportFormat": {
+                    "documentation": "<p>The format of the export.</p>",
+                    "shape": "AssetBundleExportFormat"
+                },
+                "IncludeAllDependencies": {
+                    "documentation": "<p>The include dependencies flag.</p>",
+                    "shape": "Boolean"
+                },
+                "JobStatus": {
+                    "documentation": "<p>Indicates the status of a job through its queuing and execution.</p> <p>Poll this <code>DescribeAssetBundleExportApi</code> until <code>JobStatus</code> is either <code>SUCCESSFUL</code> or <code>FAILED</code>.</p>",
+                    "shape": "AssetBundleExportJobStatus"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "ResourceArns": {
+                    "documentation": "<p>A list of resource ARNs that exported with the job.</p>",
+                    "shape": "AssetBundleResourceArns"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the response.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
+        "DescribeAssetBundleImportJobRequest": {
+            "members": {
+                "AssetBundleImportJobId": {
+                    "documentation": "<p>The ID of the job. The job ID is set when you start a new job with a <code>StartAssetBundleImportJob</code> API call.</p>",
+                    "location": "uri",
+                    "locationName": "AssetBundleImportJobId",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account the import job was executed in. </p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "AssetBundleImportJobId"
+            ],
+            "type": "structure"
+        },
+        "DescribeAssetBundleImportJobResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the import job.</p>",
+                    "shape": "Arn"
+                },
+                "AssetBundleImportJobId": {
+                    "documentation": "<p>The ID of the job. The job ID is set when you start a new job with a <code>StartAssetBundleImportJob</code> API call.</p>",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "AssetBundleImportSource": {
+                    "documentation": "<p>The source of the asset bundle zip file that contains the data that is imported by the job.</p>",
+                    "shape": "AssetBundleImportSourceDescription"
+                },
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account the import job was executed in. </p>",
+                    "shape": "AwsAccountId"
+                },
+                "CreatedTime": {
+                    "documentation": "<p>The time that the import job was created.</p>",
+                    "shape": "Timestamp"
+                },
+                "Errors": {
+                    "documentation": "<p>An array of error records that describes any failures that occurred during the export job processing.</p> <p>Error records accumulate while the job is still running. The complete set of error records is available after the job has completed and failed.</p>",
+                    "shape": "AssetBundleImportJobErrorList"
+                },
+                "FailureAction": {
+                    "documentation": "<p>The failure action for the import job.</p>",
+                    "shape": "AssetBundleImportFailureAction"
+                },
+                "JobStatus": {
+                    "documentation": "<p>Indicates the status of a job through its queuing and execution.</p> <p>Poll the <code>DescribeAssetBundleImport</code> API until <code>JobStatus</code> returns one of the following values:</p> <ul> <li> <p> <code>SUCCESSFUL</code> </p> </li> <li> <p> <code>FAILED</code> </p> </li> <li> <p> <code>FAILED_ROLLBACK_COMPLETED</code> </p> </li> <li> <p> <code>FAILED_ROLLBACK_ERROR</code> </p> </li> </ul>",
+                    "shape": "AssetBundleImportJobStatus"
+                },
+                "OverrideParameters": {
+                    "documentation": "<p>Optional overrides to be applied to the resource configuration before import.</p>",
+                    "shape": "AssetBundleImportJobOverrideParameters"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "RollbackErrors": {
+                    "documentation": "<p>An array of error records that describes any failures that occurred while an import job was attempting a rollback.</p> <p>Error records accumulate while the job is still running. The complete set of error records is available after the job has completed and failed.</p>",
+                    "shape": "AssetBundleImportJobErrorList"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the response.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeDashboardDefinitionRequest": {
             "members": {
                 "AliasName": {
                     "documentation": "<p>The alias name.</p>",
                     "location": "querystring",
                     "locationName": "alias-name",
                     "shape": "AliasName"
@@ -11712,14 +14738,53 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "DescribeDataSetRefreshPropertiesRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DataSetId",
+                    "shape": "ResourceId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "DataSetId"
+            ],
+            "type": "structure"
+        },
+        "DescribeDataSetRefreshPropertiesResponse": {
+            "members": {
+                "DataSetRefreshProperties": {
+                    "documentation": "<p>The dataset refresh properties.</p>",
+                    "shape": "DataSetRefreshProperties"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeDataSetRequest": {
             "members": {
                 "AwsAccountId": {
                     "documentation": "<p>The Amazon Web Services account ID.</p>",
                     "location": "uri",
                     "locationName": "AwsAccountId",
                     "shape": "AwsAccountId"
@@ -12239,14 +15304,64 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "DescribeRefreshScheduleRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DataSetId",
+                    "shape": "ResourceId"
+                },
+                "ScheduleId": {
+                    "documentation": "<p>The ID of the refresh schedule.</p>",
+                    "location": "uri",
+                    "locationName": "ScheduleId",
+                    "shape": "String"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "DataSetId",
+                "ScheduleId"
+            ],
+            "type": "structure"
+        },
+        "DescribeRefreshScheduleResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the refresh schedule.</p>",
+                    "shape": "Arn"
+                },
+                "RefreshSchedule": {
+                    "documentation": "<p>The refresh schedule.</p>",
+                    "shape": "RefreshSchedule"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeTemplateAliasRequest": {
             "members": {
                 "AliasName": {
                     "documentation": "<p>The name of the template alias that you want to describe. If you name a specific alias, you describe the version that the alias points to. You can specify the latest version of the template by providing the keyword <code>$LATEST</code> in the <code>AliasName</code> parameter. The keyword <code>$PUBLISHED</code> doesn't apply to templates.</p>",
                     "location": "uri",
                     "locationName": "AliasName",
                     "shape": "AliasName"
@@ -12598,14 +15713,212 @@
                 "Theme": {
                     "documentation": "<p>The information about the theme that you are describing.</p>",
                     "shape": "Theme"
                 }
             },
             "type": "structure"
         },
+        "DescribeTopicPermissionsRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topic that you want described.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId"
+            ],
+            "type": "structure"
+        },
+        "DescribeTopicPermissionsResponse": {
+            "members": {
+                "Permissions": {
+                    "documentation": "<p>A list of resource permissions that are configured to the topic.</p>",
+                    "shape": "ResourcePermissionList"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "DescribeTopicRefreshRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topic whose refresh you want to describe.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "RefreshId": {
+                    "documentation": "<p>The ID of the refresh, which is performed when the topic is created or updated.</p>",
+                    "location": "uri",
+                    "locationName": "RefreshId",
+                    "shape": "ResourceId"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId",
+                "RefreshId"
+            ],
+            "type": "structure"
+        },
+        "DescribeTopicRefreshResponse": {
+            "members": {
+                "RefreshDetails": {
+                    "documentation": "<p>Details of the refresh, which is performed when the topic is created or updated.</p>",
+                    "shape": "TopicRefreshDetails"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
+        "DescribeTopicRefreshScheduleRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DatasetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DatasetId",
+                    "shape": "String"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that contains the refresh schedule that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId",
+                "DatasetId"
+            ],
+            "type": "structure"
+        },
+        "DescribeTopicRefreshScheduleResponse": {
+            "members": {
+                "DatasetArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the dataset.</p>",
+                    "shape": "Arn"
+                },
+                "RefreshSchedule": {
+                    "documentation": "<p>The definition of a refresh schedule.</p>",
+                    "shape": "TopicRefreshSchedule"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that contains the refresh schedule that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "DescribeTopicRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId"
+            ],
+            "type": "structure"
+        },
+        "DescribeTopicResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "Topic": {
+                    "documentation": "<p>The definition of a topic.</p>",
+                    "shape": "TopicDetails"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeUserRequest": {
             "members": {
                 "AwsAccountId": {
                     "documentation": "<p>The ID for the Amazon Web Services account that the user is in. Currently, you use the ID for the Amazon Web Services account that contains your Amazon QuickSight account.</p>",
                     "location": "uri",
                     "locationName": "AwsAccountId",
                     "shape": "AwsAccountId"
@@ -12644,25 +15957,66 @@
                 "User": {
                     "documentation": "<p>The user name.</p>",
                     "shape": "User"
                 }
             },
             "type": "structure"
         },
+        "DescribeVPCConnectionRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID of the account that contains the VPC connection that you want described.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC connection that you're creating. This ID is a unique identifier for each Amazon Web Services Region in an Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "VPCConnectionId",
+                    "shape": "VPCConnectionResourceIdUnrestricted"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "VPCConnectionId"
+            ],
+            "type": "structure"
+        },
+        "DescribeVPCConnectionResponse": {
+            "members": {
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "shape": "StatusCode"
+                },
+                "VPCConnection": {
+                    "documentation": "<p>A response object that provides information for the specified VPC connection.</p>",
+                    "shape": "VPCConnection"
+                }
+            },
+            "type": "structure"
+        },
         "DestinationParameterValueConfiguration": {
             "documentation": "<p>The configuration of destination parameter values.</p> <p>This is a union type structure. For this structure to be valid, only one of the attributes can be defined.</p>",
             "members": {
                 "CustomValuesConfiguration": {
                     "documentation": "<p>The configuration of custom values for destination parameter in <code>DestinationParameterValueConfiguration</code>.</p>",
                     "shape": "CustomValuesConfiguration"
                 },
                 "SelectAllValueOptions": {
                     "documentation": "<p>The configuration that selects all options.</p>",
                     "shape": "SelectAllValueOptions"
                 },
+                "SourceColumn": {
+                    "shape": "ColumnIdentifier"
+                },
                 "SourceField": {
                     "documentation": "<p>The source field ID of the destination parameter.</p>",
                     "shape": "FieldId"
                 },
                 "SourceParameterName": {
                     "documentation": "<p>The source parameter name of the destination parameter.</p>",
                     "shape": "String"
@@ -12691,14 +16045,86 @@
         "DimensionFieldList": {
             "max": 200,
             "member": {
                 "shape": "DimensionField"
             },
             "type": "list"
         },
+        "DisplayFormat": {
+            "enum": [
+                "AUTO",
+                "PERCENT",
+                "CURRENCY",
+                "NUMBER",
+                "DATE",
+                "STRING"
+            ],
+            "type": "string"
+        },
+        "DisplayFormatOptions": {
+            "documentation": "<p>A structure that represents additional options for display formatting.</p>",
+            "members": {
+                "BlankCellFormat": {
+                    "documentation": "<p>Determines the blank cell format.</p>",
+                    "shape": "LimitedString"
+                },
+                "CurrencySymbol": {
+                    "documentation": "<p>The currency symbol, such as <code>USD</code>.</p>",
+                    "shape": "LimitedString"
+                },
+                "DateFormat": {
+                    "documentation": "<p>Determines the <code>DateTime</code> format.</p>",
+                    "shape": "LimitedString"
+                },
+                "DecimalSeparator": {
+                    "documentation": "<p>Determines the decimal separator.</p>",
+                    "shape": "TopicNumericSeparatorSymbol"
+                },
+                "FractionDigits": {
+                    "documentation": "<p>Determines the number of fraction digits.</p>",
+                    "shape": "Integer"
+                },
+                "GroupingSeparator": {
+                    "documentation": "<p>Determines the grouping separator.</p>",
+                    "shape": "LimitedString"
+                },
+                "NegativeFormat": {
+                    "documentation": "<p>The negative format.</p>",
+                    "shape": "NegativeFormat"
+                },
+                "Prefix": {
+                    "documentation": "<p>The prefix value for a display format.</p>",
+                    "shape": "LimitedString"
+                },
+                "Suffix": {
+                    "documentation": "<p>The suffix value for a display format.</p>",
+                    "shape": "LimitedString"
+                },
+                "UnitScaler": {
+                    "documentation": "<p>The unit scaler. Valid values for this structure are: <code>NONE</code>, <code>AUTO</code>, <code>THOUSANDS</code>, <code>MILLIONS</code>, <code>BILLIONS</code>, and <code>TRILLIONS</code>.</p>",
+                    "shape": "NumberScale"
+                },
+                "UseBlankCellFormat": {
+                    "documentation": "<p>A Boolean value that indicates whether to use blank cell format.</p>",
+                    "shape": "Boolean"
+                },
+                "UseGrouping": {
+                    "documentation": "<p>A Boolean value that indicates whether to use grouping.</p>",
+                    "shape": "Boolean"
+                }
+            },
+            "type": "structure"
+        },
+        "DnsResolverList": {
+            "max": 15,
+            "member": {
+                "shape": "IPv4Address"
+            },
+            "type": "list"
+        },
         "Domain": {
             "max": 64,
             "min": 1,
             "type": "string"
         },
         "DomainNotWhitelistedException": {
             "documentation": "<p>The domain specified isn't on the allow list. All domains for embedded dashboards must be added to the approved list by an Amazon QuickSight admin.</p>",
@@ -13377,14 +16803,22 @@
                 "TopBottomFilter": {
                     "documentation": "<p>A <code>TopBottomFilter</code> filters data to the top or bottom values for a given column.</p>",
                     "shape": "TopBottomFilter"
                 }
             },
             "type": "structure"
         },
+        "FilterClass": {
+            "enum": [
+                "ENFORCED_VALUE_FILTER",
+                "CONDITIONAL_VALUE_FILTER",
+                "NAMED_VALUE_FILTER"
+            ],
+            "type": "string"
+        },
         "FilterControl": {
             "documentation": "<p>The control of a filter that is used to interact with a dashboard or an analysis.</p> <p>This is a union type structure. For this structure to be valid, only one of the attributes can be defined.</p>",
             "members": {
                 "DateTimePicker": {
                     "documentation": "<p>A control from a date filter that is used to specify date and time.</p>",
                     "shape": "FilterDateTimePickerControl"
                 },
@@ -13618,14 +17052,18 @@
                 "ConditionExpression"
             ],
             "type": "structure"
         },
         "FilterOperationSelectedFieldsConfiguration": {
             "documentation": "<p>The configuration of selected fields in the<code>CustomActionFilterOperation</code>.</p> <p>This is a union type structure. For this structure to be valid, only one of the attributes can be defined.</p>",
             "members": {
+                "SelectedColumns": {
+                    "documentation": "<p>The selected columns of a dataset.</p>",
+                    "shape": "CustomActionColumnList"
+                },
                 "SelectedFieldOptions": {
                     "documentation": "<p>A structure that contains the options that choose which fields are filtered in the <code>CustomActionFilterOperation</code>.</p> <p>Valid values are defined as follows:</p> <ul> <li> <p> <code>ALL_FIELDS</code>: Applies the filter operation to all fields.</p> </li> </ul>",
                     "shape": "SelectedFieldOptions"
                 },
                 "SelectedFields": {
                     "documentation": "<p>Chooses the fields that are filtered in <code>CustomActionFilterOperation</code>.</p>",
                     "shape": "SelectedFieldList"
@@ -14823,14 +18261,55 @@
                 "North",
                 "South",
                 "West",
                 "East"
             ],
             "type": "structure"
         },
+        "GeospatialHeatmapColorScale": {
+            "documentation": "<p>The color scale specification for the heatmap point style.</p>",
+            "members": {
+                "Colors": {
+                    "documentation": "<p>The list of colors to be used in heatmap point style.</p>",
+                    "shape": "GeospatialHeatmapDataColorList"
+                }
+            },
+            "type": "structure"
+        },
+        "GeospatialHeatmapConfiguration": {
+            "documentation": "<p>The heatmap configuration of the geospatial point style.</p>",
+            "members": {
+                "HeatmapColor": {
+                    "documentation": "<p>The color scale specification for the heatmap point style.</p>",
+                    "shape": "GeospatialHeatmapColorScale"
+                }
+            },
+            "type": "structure"
+        },
+        "GeospatialHeatmapDataColor": {
+            "documentation": "<p>The color to be used in the heatmap point style.</p>",
+            "members": {
+                "Color": {
+                    "documentation": "<p>The hex color to be used in the heatmap point style.</p>",
+                    "shape": "HexColor"
+                }
+            },
+            "required": [
+                "Color"
+            ],
+            "type": "structure"
+        },
+        "GeospatialHeatmapDataColorList": {
+            "max": 2,
+            "member": {
+                "shape": "GeospatialHeatmapDataColor"
+            },
+            "min": 2,
+            "type": "list"
+        },
         "GeospatialMapAggregatedFieldWells": {
             "documentation": "<p>The aggregated field wells for a geospatial map.</p>",
             "members": {
                 "Colors": {
                     "documentation": "<p>The color field wells of a geospatial map.</p>",
                     "shape": "DimensionFieldList"
                 },
@@ -14934,25 +18413,30 @@
         "GeospatialPointStyleOptions": {
             "documentation": "<p>The point style of the geospatial map.</p>",
             "members": {
                 "ClusterMarkerConfiguration": {
                     "documentation": "<p>The cluster marker configuration of the geospatial point style.</p>",
                     "shape": "ClusterMarkerConfiguration"
                 },
+                "HeatmapConfiguration": {
+                    "documentation": "<p>The heatmap configuration of the geospatial point style.</p>",
+                    "shape": "GeospatialHeatmapConfiguration"
+                },
                 "SelectedPointStyle": {
                     "documentation": "<p>The selected point styles (point, cluster) of the geospatial map.</p>",
                     "shape": "GeospatialSelectedPointStyle"
                 }
             },
             "type": "structure"
         },
         "GeospatialSelectedPointStyle": {
             "enum": [
                 "POINT",
-                "CLUSTER"
+                "CLUSTER",
+                "HEATMAP"
             ],
             "type": "string"
         },
         "GeospatialWindowOptions": {
             "documentation": "<p>The window options of the geospatial map visual.</p>",
             "members": {
                 "Bounds": {
@@ -15790,14 +19274,19 @@
         },
         "IAMPolicyAssignmentSummaryList": {
             "member": {
                 "shape": "IAMPolicyAssignmentSummary"
             },
             "type": "list"
         },
+        "IPv4Address": {
+            "max": 15,
+            "min": 7,
+            "type": "string"
+        },
         "Icon": {
             "enum": [
                 "CARET_UP",
                 "CARET_DOWN",
                 "PLUS",
                 "MINUS",
                 "ARROW_UP",
@@ -15871,14 +19360,27 @@
                 "RequestId": {
                     "documentation": "<p>The Amazon Web Services request ID for this request.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
+        "IncrementalRefresh": {
+            "documentation": "<p>The incremental refresh configuration for a dataset.</p>",
+            "members": {
+                "LookbackWindow": {
+                    "documentation": "<p>The lookback window setup for an incremental refresh configuration.</p>",
+                    "shape": "LookbackWindow"
+                }
+            },
+            "required": [
+                "LookbackWindow"
+            ],
+            "type": "structure"
+        },
         "Ingestion": {
             "documentation": "<p>Information about the SPICE ingestion for a dataset.</p>",
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the resource.</p>",
                     "shape": "Arn"
                 },
@@ -15971,15 +19473,16 @@
                 "DATA_SOURCE_AUTH_FAILED",
                 "DATA_SOURCE_CONNECTION_FAILED",
                 "FAILURE_TO_PROCESS_JSON_FILE",
                 "INTERNAL_SERVICE_ERROR",
                 "REFRESH_SUPPRESSED_BY_EDIT",
                 "PERMISSION_NOT_FOUND",
                 "ELASTICSEARCH_CURSOR_NOT_ENABLED",
-                "CURSOR_NOT_ENABLED"
+                "CURSOR_NOT_ENABLED",
+                "DUPLICATE_COLUMN_NAMES_FOUND"
             ],
             "type": "string"
         },
         "IngestionId": {
             "max": 128,
             "min": 1,
             "pattern": "^[a-zA-Z0-9-_]+$",
@@ -16122,14 +19625,63 @@
             "max": 64,
             "min": 1,
             "type": "string"
         },
         "Integer": {
             "type": "integer"
         },
+        "IntegerDatasetParameter": {
+            "documentation": "<p>An integer parameter for a dataset.</p>",
+            "members": {
+                "DefaultValues": {
+                    "documentation": "<p>A list of default values for a given integer parameter. This structure only accepts static values.</p>",
+                    "shape": "IntegerDatasetParameterDefaultValues"
+                },
+                "Id": {
+                    "documentation": "<p>An identifier for the integer parameter created in the dataset.</p>",
+                    "shape": "DatasetParameterId"
+                },
+                "Name": {
+                    "documentation": "<p>The name of the integer parameter that is created in the dataset.</p>",
+                    "shape": "DatasetParameterName"
+                },
+                "ValueType": {
+                    "documentation": "<p>The value type of the dataset parameter. Valid values are <code>single value</code> or <code>multi value</code>.</p>",
+                    "shape": "DatasetParameterValueType"
+                }
+            },
+            "required": [
+                "Id",
+                "Name",
+                "ValueType"
+            ],
+            "type": "structure"
+        },
+        "IntegerDatasetParameterDefaultValue": {
+            "documentation": "<p>The default value for the integer parameter.</p>",
+            "type": "long"
+        },
+        "IntegerDatasetParameterDefaultValues": {
+            "documentation": "<p>The default values of an integer parameter.</p>",
+            "members": {
+                "StaticValues": {
+                    "documentation": "<p>A list of static default values for a given integer parameter.</p>",
+                    "shape": "IntegerDatasetParameterValueList"
+                }
+            },
+            "type": "structure"
+        },
+        "IntegerDatasetParameterValueList": {
+            "max": 32,
+            "member": {
+                "shape": "IntegerDatasetParameterDefaultValue"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "IntegerDefaultValueList": {
             "max": 50000,
             "member": {
                 "shape": "SensitiveLongObject"
             },
             "type": "list"
         },
@@ -16168,14 +19720,17 @@
         "IntegerParameterDeclaration": {
             "documentation": "<p>A parameter declaration for the <code>Integer</code> data type.</p>",
             "members": {
                 "DefaultValues": {
                     "documentation": "<p>The default values of a parameter. If the parameter is a single-value parameter, a maximum of one default value can be provided.</p>",
                     "shape": "IntegerDefaultValues"
                 },
+                "MappedDataSetParameters": {
+                    "shape": "MappedDataSetParameters"
+                },
                 "Name": {
                     "documentation": "<p>The name of the parameter that is being declared.</p>",
                     "shape": "ParameterName"
                 },
                 "ParameterValueType": {
                     "documentation": "<p>The value type determines whether the parameter is a single-value or multi-value parameter.</p>",
                     "shape": "ParameterValueType"
@@ -16679,14 +20234,18 @@
                 "ResourceType": {
                     "documentation": "<p>Limit exceeded.</p>",
                     "shape": "ExceptionResourceType"
                 }
             },
             "type": "structure"
         },
+        "LimitedString": {
+            "max": 256,
+            "type": "string"
+        },
         "LineChartAggregatedFieldWells": {
             "documentation": "<p>The field well configuration of a line chart.</p>",
             "members": {
                 "Category": {
                     "documentation": "<p>The category field wells of a line chart. Values are grouped by category fields.</p>",
                     "shape": "DimensionFieldList"
                 },
@@ -17035,14 +20594,112 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "ListAssetBundleExportJobsRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that the export jobs were executed in. </p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "MaxResults": {
+                    "box": true,
+                    "documentation": "<p>The maximum number of results to be returned per request.</p>",
+                    "location": "querystring",
+                    "locationName": "max-results",
+                    "shape": "MaxResults"
+                },
+                "NextToken": {
+                    "documentation": "<p>The token for the next set of results, or null if there are no more results.</p>",
+                    "location": "querystring",
+                    "locationName": "next-token",
+                    "shape": "String"
+                }
+            },
+            "required": [
+                "AwsAccountId"
+            ],
+            "type": "structure"
+        },
+        "ListAssetBundleExportJobsResponse": {
+            "members": {
+                "AssetBundleExportJobSummaryList": {
+                    "documentation": "<p>A list of export job summaries.</p>",
+                    "shape": "AssetBundleExportJobSummaryList"
+                },
+                "NextToken": {
+                    "documentation": "<p>The token for the next set of results, or null if there are no more results.</p>",
+                    "shape": "String"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
+        "ListAssetBundleImportJobsRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that the import jobs were executed in.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "MaxResults": {
+                    "box": true,
+                    "documentation": "<p>The maximum number of results to be returned per request.</p>",
+                    "location": "querystring",
+                    "locationName": "max-results",
+                    "shape": "MaxResults"
+                },
+                "NextToken": {
+                    "documentation": "<p>The token for the next set of results, or null if there are no more results.</p>",
+                    "location": "querystring",
+                    "locationName": "next-token",
+                    "shape": "String"
+                }
+            },
+            "required": [
+                "AwsAccountId"
+            ],
+            "type": "structure"
+        },
+        "ListAssetBundleImportJobsResponse": {
+            "members": {
+                "AssetBundleImportJobSummaryList": {
+                    "documentation": "<p>A list of import job summaries.</p>",
+                    "shape": "AssetBundleImportJobSummaryList"
+                },
+                "NextToken": {
+                    "documentation": "<p>The token for the next set of results, or null if there are no more results.</p>",
+                    "shape": "String"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the response.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "ListControlDisplayOptions": {
             "documentation": "<p>The display options of a control.</p>",
             "members": {
                 "SearchOptions": {
                     "documentation": "<p>The configuration of the search options in a list control.</p>",
                     "shape": "ListControlSearchOptions"
                 },
@@ -17567,14 +21224,16 @@
             },
             "type": "structure"
         },
         "ListIAMPolicyAssignmentsRequest": {
             "members": {
                 "AssignmentStatus": {
                     "documentation": "<p>The status of the assignments.</p>",
+                    "location": "querystring",
+                    "locationName": "assignment-status",
                     "shape": "AssignmentStatus"
                 },
                 "AwsAccountId": {
                     "documentation": "<p>The ID of the Amazon Web Services account that contains these IAM policy assignments.</p>",
                     "location": "uri",
                     "locationName": "AwsAccountId",
                     "shape": "AwsAccountId"
@@ -17728,14 +21387,53 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "ListRefreshSchedulesRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DataSetId",
+                    "shape": "ResourceId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "DataSetId"
+            ],
+            "type": "structure"
+        },
+        "ListRefreshSchedulesResponse": {
+            "members": {
+                "RefreshSchedules": {
+                    "documentation": "<p>The list of refresh schedules for the dataset.</p>",
+                    "shape": "RefreshSchedules"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "ListTagsForResourceRequest": {
             "members": {
                 "ResourceArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the resource that you want a list of tags for.</p>",
                     "location": "uri",
                     "locationName": "ResourceArn",
                     "shape": "Arn"
@@ -18088,14 +21786,110 @@
                 "ThemeSummaryList": {
                     "documentation": "<p>Information about the themes in the list.</p>",
                     "shape": "ThemeSummaryList"
                 }
             },
             "type": "structure"
         },
+        "ListTopicRefreshSchedulesRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topic whose refresh schedule you want described.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID for the topic that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId"
+            ],
+            "type": "structure"
+        },
+        "ListTopicRefreshSchedulesResponse": {
+            "members": {
+                "RefreshSchedules": {
+                    "documentation": "<p>The list of topic refresh schedules.</p>",
+                    "shape": "TopicRefreshScheduleSummaries"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID for the topic that you want to describe. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "ListTopicsRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topics that you want to list.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "MaxResults": {
+                    "box": true,
+                    "documentation": "<p>The maximum number of results to be returned per request.</p>",
+                    "location": "querystring",
+                    "locationName": "max-results",
+                    "shape": "MaxResults"
+                },
+                "NextToken": {
+                    "documentation": "<p>The token for the next set of results, or null if there are no more results.</p>",
+                    "location": "querystring",
+                    "locationName": "next-token",
+                    "shape": "String"
+                }
+            },
+            "required": [
+                "AwsAccountId"
+            ],
+            "type": "structure"
+        },
+        "ListTopicsResponse": {
+            "members": {
+                "NextToken": {
+                    "documentation": "<p>The token for the next set of results, or null if there are no more results.</p>",
+                    "shape": "String"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicsSummaries": {
+                    "documentation": "<p>A list of topic summaries.</p>",
+                    "shape": "TopicSummaries"
+                }
+            },
+            "type": "structure"
+        },
         "ListUserGroupsRequest": {
             "members": {
                 "AwsAccountId": {
                     "documentation": "<p>The Amazon Web Services account ID that the user is in. Currently, you use the ID for the Amazon Web Services account that contains your Amazon QuickSight account.</p>",
                     "location": "uri",
                     "locationName": "AwsAccountId",
                     "shape": "AwsAccountId"
@@ -18207,14 +22001,63 @@
                 "UserList": {
                     "documentation": "<p>The list of users.</p>",
                     "shape": "UserList"
                 }
             },
             "type": "structure"
         },
+        "ListVPCConnectionsRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID of the account that contains the VPC connections that you want to list.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "MaxResults": {
+                    "box": true,
+                    "documentation": "<p>The maximum number of results to be returned per request.</p>",
+                    "location": "querystring",
+                    "locationName": "max-results",
+                    "shape": "MaxResults"
+                },
+                "NextToken": {
+                    "documentation": "<p>The token for the next set of results, or null if there are no more results.</p>",
+                    "location": "querystring",
+                    "locationName": "next-token",
+                    "shape": "String"
+                }
+            },
+            "required": [
+                "AwsAccountId"
+            ],
+            "type": "structure"
+        },
+        "ListVPCConnectionsResponse": {
+            "members": {
+                "NextToken": {
+                    "documentation": "<p>The token for the next set of results, or null if there are no more results.</p>",
+                    "shape": "String"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "VPCConnectionSummaries": {
+                    "documentation": "<p>A <code>VPCConnectionSummaries</code> object that returns a summary of VPC connection objects.</p>",
+                    "shape": "VPCConnectionSummaryList"
+                }
+            },
+            "type": "structure"
+        },
         "LoadingAnimation": {
             "documentation": "<p>The configuration of loading animation in free-form layout. </p>",
             "members": {
                 "Visibility": {
                     "documentation": "<p>The visibility configuration of <code>LoadingAnimation</code>.</p>",
                     "shape": "Visibility"
                 }
@@ -18258,14 +22101,15 @@
         },
         "LogicalTableAlias": {
             "max": 64,
             "min": 1,
             "type": "string"
         },
         "LogicalTableId": {
+            "documentation": "<p>An identifier for the logical table that is defined in the dataset</p>",
             "max": 64,
             "min": 1,
             "pattern": "[0-9a-zA-Z-]*",
             "type": "string"
         },
         "LogicalTableMap": {
             "key": {
@@ -18324,14 +22168,45 @@
             "type": "string"
         },
         "Longitude": {
             "max": 1800,
             "min": -1800,
             "type": "double"
         },
+        "LookbackWindow": {
+            "documentation": "<p>The lookback window setup of an incremental refresh configuration.</p>",
+            "members": {
+                "ColumnName": {
+                    "documentation": "<p>The name of the lookback window column.</p>",
+                    "shape": "String"
+                },
+                "Size": {
+                    "documentation": "<p>The lookback window column size.</p>",
+                    "shape": "PositiveLong"
+                },
+                "SizeUnit": {
+                    "documentation": "<p>The size unit that is used for the lookback window column. Valid values for this structure are <code>HOUR</code>, <code>DAY</code>, and <code>WEEK</code>.</p>",
+                    "shape": "LookbackWindowSizeUnit"
+                }
+            },
+            "required": [
+                "ColumnName",
+                "Size",
+                "SizeUnit"
+            ],
+            "type": "structure"
+        },
+        "LookbackWindowSizeUnit": {
+            "enum": [
+                "HOUR",
+                "DAY",
+                "WEEK"
+            ],
+            "type": "string"
+        },
         "ManifestFileLocation": {
             "documentation": "<p>Amazon S3 manifest file location.</p>",
             "members": {
                 "Bucket": {
                     "documentation": "<p>Amazon S3 bucket.</p>",
                     "shape": "S3Bucket"
                 },
@@ -18349,14 +22224,41 @@
         "MapZoomMode": {
             "enum": [
                 "AUTO",
                 "MANUAL"
             ],
             "type": "string"
         },
+        "MappedDataSetParameter": {
+            "documentation": "<p>A dataset parameter that is mapped to an analysis parameter.</p>",
+            "members": {
+                "DataSetIdentifier": {
+                    "documentation": "<p>A unique name that identifies a dataset within the analysis or dashboard.</p>",
+                    "shape": "DataSetIdentifier"
+                },
+                "DataSetParameterName": {
+                    "documentation": "<p>The name of the dataset parameter.</p>",
+                    "shape": "ParameterName"
+                }
+            },
+            "required": [
+                "DataSetIdentifier",
+                "DataSetParameterName"
+            ],
+            "type": "structure"
+        },
+        "MappedDataSetParameters": {
+            "documentation": "<p>A list of dataset parameters that are mapped to an analysis parameter.</p>",
+            "max": 150,
+            "member": {
+                "shape": "MappedDataSetParameter"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "MarginStyle": {
             "documentation": "<p>The display options for margins around the outside edge of sheets.</p>",
             "members": {
                 "Show": {
                     "box": true,
                     "documentation": "<p>This Boolean value controls whether to display sheet margins.</p>",
                     "shape": "Boolean"
@@ -18577,14 +22479,105 @@
             "required": [
                 "Host",
                 "Port",
                 "Database"
             ],
             "type": "structure"
         },
+        "NamedEntityAggType": {
+            "enum": [
+                "SUM",
+                "MIN",
+                "MAX",
+                "COUNT",
+                "AVERAGE",
+                "DISTINCT_COUNT",
+                "STDEV",
+                "STDEVP",
+                "VAR",
+                "VARP",
+                "PERCENTILE",
+                "MEDIAN",
+                "CUSTOM"
+            ],
+            "type": "string"
+        },
+        "NamedEntityDefinition": {
+            "documentation": "<p>A structure that represents a named entity.</p>",
+            "members": {
+                "FieldName": {
+                    "documentation": "<p>The name of the entity.</p>",
+                    "shape": "LimitedString"
+                },
+                "Metric": {
+                    "documentation": "<p>The definition of a metric.</p>",
+                    "shape": "NamedEntityDefinitionMetric"
+                },
+                "PropertyName": {
+                    "documentation": "<p>The property name to be used for the named entity.</p>",
+                    "shape": "LimitedString"
+                },
+                "PropertyRole": {
+                    "documentation": "<p>The property role. Valid values for this structure are <code>PRIMARY</code> and <code>ID</code>.</p>",
+                    "shape": "PropertyRole"
+                },
+                "PropertyUsage": {
+                    "documentation": "<p>The property usage. Valid values for this structure are <code>INHERIT</code>, <code>DIMENSION</code>, and <code>MEASURE</code>.</p>",
+                    "shape": "PropertyUsage"
+                }
+            },
+            "type": "structure"
+        },
+        "NamedEntityDefinitionMetric": {
+            "documentation": "<p>A structure that represents a metric.</p>",
+            "members": {
+                "Aggregation": {
+                    "documentation": "<p>The aggregation of a named entity. Valid values for this structure are <code>SUM</code>, <code>MIN</code>, <code>MAX</code>, <code>COUNT</code>, <code>AVERAGE</code>, <code>DISTINCT_COUNT</code>, <code>STDEV</code>, <code>STDEVP</code>, <code>VAR</code>, <code>VARP</code>, <code>PERCENTILE</code>, <code>MEDIAN</code>, and <code>CUSTOM</code>.</p>",
+                    "shape": "NamedEntityAggType"
+                },
+                "AggregationFunctionParameters": {
+                    "documentation": "<p>The additional parameters for an aggregation function.</p>",
+                    "shape": "AggregationFunctionParameters"
+                }
+            },
+            "type": "structure"
+        },
+        "NamedEntityDefinitions": {
+            "member": {
+                "shape": "NamedEntityDefinition"
+            },
+            "type": "list"
+        },
+        "NamedFilterAggType": {
+            "enum": [
+                "NO_AGGREGATION",
+                "SUM",
+                "AVERAGE",
+                "COUNT",
+                "DISTINCT_COUNT",
+                "MAX",
+                "MEDIAN",
+                "MIN",
+                "STDEV",
+                "STDEVP",
+                "VAR",
+                "VARP"
+            ],
+            "type": "string"
+        },
+        "NamedFilterType": {
+            "enum": [
+                "CATEGORY_FILTER",
+                "NUMERIC_EQUALITY_FILTER",
+                "NUMERIC_RANGE_FILTER",
+                "DATE_RANGE_FILTER",
+                "RELATIVE_DATE_FILTER"
+            ],
+            "type": "string"
+        },
         "Namespace": {
             "max": 64,
             "pattern": "^[a-zA-Z0-9._-]*$",
             "type": "string"
         },
         "NamespaceError": {
             "documentation": "<p>Errors that occur during namespace creation.</p>",
@@ -18653,14 +22646,28 @@
             },
             "type": "list"
         },
         "NarrativeString": {
             "max": 150000,
             "type": "string"
         },
+        "NegativeFormat": {
+            "documentation": "<p>A structure that represents a negative format.</p>",
+            "members": {
+                "Prefix": {
+                    "documentation": "<p>The prefix for a negative format.</p>",
+                    "shape": "LimitedString"
+                },
+                "Suffix": {
+                    "documentation": "<p>The suffix for a negative format.</p>",
+                    "shape": "LimitedString"
+                }
+            },
+            "type": "structure"
+        },
         "NegativeValueConfiguration": {
             "documentation": "<p>The options that determine the negative value configuration.</p>",
             "members": {
                 "DisplayMode": {
                     "documentation": "<p>Determines the display mode of the negative value configuration.</p>",
                     "shape": "NegativeValueDisplayMode"
                 }
@@ -18673,14 +22680,88 @@
         "NegativeValueDisplayMode": {
             "enum": [
                 "POSITIVE",
                 "NEGATIVE"
             ],
             "type": "string"
         },
+        "NetworkInterface": {
+            "documentation": "<p>The structure that contains information about a network interface.</p>",
+            "members": {
+                "AvailabilityZone": {
+                    "documentation": "<p>The availability zone that the network interface resides in.</p>",
+                    "shape": "String"
+                },
+                "ErrorMessage": {
+                    "documentation": "<p>An error message.</p>",
+                    "shape": "String"
+                },
+                "NetworkInterfaceId": {
+                    "documentation": "<p>The network interface ID.</p>",
+                    "shape": "NetworkInterfaceId"
+                },
+                "Status": {
+                    "documentation": "<p>The status of the network interface.</p>",
+                    "shape": "NetworkInterfaceStatus"
+                },
+                "SubnetId": {
+                    "documentation": "<p>The subnet ID associated with the network interface.</p>",
+                    "shape": "SubnetId"
+                }
+            },
+            "type": "structure"
+        },
+        "NetworkInterfaceId": {
+            "max": 255,
+            "pattern": "^eni-[0-9a-z]*$",
+            "type": "string"
+        },
+        "NetworkInterfaceList": {
+            "member": {
+                "shape": "NetworkInterface"
+            },
+            "type": "list"
+        },
+        "NetworkInterfaceStatus": {
+            "enum": [
+                "CREATING",
+                "AVAILABLE",
+                "CREATION_FAILED",
+                "UPDATING",
+                "UPDATE_FAILED",
+                "DELETING",
+                "DELETED",
+                "DELETION_FAILED",
+                "DELETION_SCHEDULED",
+                "ATTACHMENT_FAILED_ROLLBACK_FAILED"
+            ],
+            "type": "string"
+        },
+        "NewDefaultValues": {
+            "documentation": "<p>The configuration that overrides the existing default values for a dataset parameter that is inherited from another dataset.</p>",
+            "members": {
+                "DateTimeStaticValues": {
+                    "documentation": "<p>A list of static default values for a given date time parameter.</p>",
+                    "shape": "DateTimeDatasetParameterValueList"
+                },
+                "DecimalStaticValues": {
+                    "documentation": "<p>A list of static default values for a given decimal parameter.</p>",
+                    "shape": "DecimalDatasetParameterValueList"
+                },
+                "IntegerStaticValues": {
+                    "documentation": "<p>A list of static default values for a given integer parameter.</p>",
+                    "shape": "IntegerDatasetParameterValueList"
+                },
+                "StringStaticValues": {
+                    "documentation": "<p>A list of static default values for a given string parameter.</p>",
+                    "shape": "StringDatasetParameterValueList"
+                }
+            },
+            "type": "structure"
+        },
         "NonEmptyString": {
             "pattern": ".*\\S.*",
             "type": "string"
         },
         "NullString": {
             "max": 128,
             "min": 1,
@@ -19030,23 +23111,23 @@
             "min": 0,
             "type": "integer"
         },
         "OracleParameters": {
             "documentation": "<p>The parameters for Oracle.</p>",
             "members": {
                 "Database": {
-                    "documentation": "<p>Database.</p>",
+                    "documentation": "<p>The database.</p>",
                     "shape": "Database"
                 },
                 "Host": {
                     "documentation": "<p>An Oracle host.</p>",
                     "shape": "Host"
                 },
                 "Port": {
-                    "documentation": "<p>Port.</p>",
+                    "documentation": "<p>The port.</p>",
                     "shape": "Port"
                 }
             },
             "required": [
                 "Host",
                 "Port",
                 "Database"
@@ -19068,26 +23149,47 @@
                     "shape": "ColumnDescriptiveText"
                 },
                 "Name": {
                     "documentation": "<p>A display name for the dataset.</p>",
                     "shape": "ColumnName"
                 },
                 "Type": {
-                    "documentation": "<p>Type.</p>",
+                    "documentation": "<p>The type.</p>",
                     "shape": "ColumnDataType"
                 }
             },
             "type": "structure"
         },
         "OutputColumnList": {
             "member": {
                 "shape": "OutputColumn"
             },
             "type": "list"
         },
+        "OverrideDatasetParameterOperation": {
+            "documentation": "<p>A transform operation that overrides the dataset parameter values that are defined in another dataset.</p>",
+            "members": {
+                "NewDefaultValues": {
+                    "documentation": "<p>The new default values for the parameter.</p>",
+                    "shape": "NewDefaultValues"
+                },
+                "NewParameterName": {
+                    "documentation": "<p>The new name for the parameter.</p>",
+                    "shape": "DatasetParameterName"
+                },
+                "ParameterName": {
+                    "documentation": "<p>The name of the parameter to be overridden with different values.</p>",
+                    "shape": "DatasetParameterName"
+                }
+            },
+            "required": [
+                "ParameterName"
+            ],
+            "type": "structure"
+        },
         "PageNumber": {
             "min": 0,
             "type": "long"
         },
         "PaginationConfiguration": {
             "documentation": "<p>The pagination configuration for a table visual or boxplot.</p>",
             "members": {
@@ -19894,14 +23996,18 @@
                     "documentation": "<p>The field ID of the cell for conditional formatting.</p>",
                     "shape": "FieldId"
                 },
                 "Scope": {
                     "documentation": "<p>The scope of the cell for conditional formatting.</p>",
                     "shape": "PivotTableConditionalFormattingScope"
                 },
+                "Scopes": {
+                    "documentation": "<p>A list of cell scopes for conditional formatting.</p>",
+                    "shape": "PivotTableConditionalFormattingScopeList"
+                },
                 "TextFormat": {
                     "documentation": "<p>The text format of the cell for conditional formatting.</p>",
                     "shape": "TextConditionalFormat"
                 }
             },
             "required": [
                 "FieldId"
@@ -19941,14 +24047,21 @@
                 "Role": {
                     "documentation": "<p>The role (field, field total, grand total) of the cell for conditional formatting.</p>",
                     "shape": "PivotTableConditionalFormattingScopeRole"
                 }
             },
             "type": "structure"
         },
+        "PivotTableConditionalFormattingScopeList": {
+            "max": 3,
+            "member": {
+                "shape": "PivotTableConditionalFormattingScope"
+            },
+            "type": "list"
+        },
         "PivotTableConditionalFormattingScopeRole": {
             "enum": [
                 "FIELD",
                 "FIELD_TOTAL",
                 "GRAND_TOTAL"
             ],
             "type": "string"
@@ -20010,14 +24123,58 @@
         "PivotTableDimensionList": {
             "max": 40,
             "member": {
                 "shape": "DimensionField"
             },
             "type": "list"
         },
+        "PivotTableFieldCollapseState": {
+            "enum": [
+                "COLLAPSED",
+                "EXPANDED"
+            ],
+            "type": "string"
+        },
+        "PivotTableFieldCollapseStateOption": {
+            "documentation": "<p>The collapse state options for the pivot table field options.</p>",
+            "members": {
+                "State": {
+                    "documentation": "<p>The state of the field target of a pivot table. Choose one of the following options:</p> <ul> <li> <p> <code>COLLAPSED</code> </p> </li> <li> <p> <code>EXPANDED</code> </p> </li> </ul>",
+                    "shape": "PivotTableFieldCollapseState"
+                },
+                "Target": {
+                    "documentation": "<p>A tagged-union object that sets the collapse state.</p>",
+                    "shape": "PivotTableFieldCollapseStateTarget"
+                }
+            },
+            "required": [
+                "Target"
+            ],
+            "type": "structure"
+        },
+        "PivotTableFieldCollapseStateOptionList": {
+            "member": {
+                "shape": "PivotTableFieldCollapseStateOption"
+            },
+            "type": "list"
+        },
+        "PivotTableFieldCollapseStateTarget": {
+            "documentation": "<p>The target of a pivot table field collapse state.</p>",
+            "members": {
+                "FieldDataPathValues": {
+                    "documentation": "<p>The data path of the pivot table's header. Used to set the collapse state.</p>",
+                    "shape": "DataPathValueList"
+                },
+                "FieldId": {
+                    "documentation": "<p>The field ID of the pivot table that the collapse state needs to be set to.</p>",
+                    "shape": "String"
+                }
+            },
+            "type": "structure"
+        },
         "PivotTableFieldOption": {
             "documentation": "<p>The selected field options for the pivot table field options.</p>",
             "members": {
                 "CustomLabel": {
                     "documentation": "<p>The custom label of the pivot table field.</p>",
                     "shape": "CustomLabel"
                 },
@@ -20041,14 +24198,18 @@
                 "shape": "PivotTableFieldOption"
             },
             "type": "list"
         },
         "PivotTableFieldOptions": {
             "documentation": "<p>The field options for a pivot table visual.</p>",
             "members": {
+                "CollapseStateOptions": {
+                    "documentation": "<p>The collapse state options for the pivot table field options.</p>",
+                    "shape": "PivotTableFieldCollapseStateOptionList"
+                },
                 "DataPathOptions": {
                     "documentation": "<p>The data path options for the pivot table field options.</p>",
                     "shape": "PivotTableDataPathOptionList"
                 },
                 "SelectedFieldOptions": {
                     "documentation": "<p>The selected field options for the pivot table field options.</p>",
                     "shape": "PivotTableFieldOptionList"
@@ -20284,14 +24445,18 @@
             "min": 1,
             "type": "integer"
         },
         "PositiveInteger": {
             "min": 1,
             "type": "integer"
         },
+        "PositiveLong": {
+            "min": 1,
+            "type": "long"
+        },
         "PostgreSqlParameters": {
             "documentation": "<p>The parameters for PostgreSQL.</p>",
             "members": {
                 "Database": {
                     "documentation": "<p>Database.</p>",
                     "shape": "Database"
                 },
@@ -20440,14 +24605,69 @@
             "max": 2000,
             "member": {
                 "shape": "String"
             },
             "min": 1,
             "type": "list"
         },
+        "PropertyRole": {
+            "enum": [
+                "PRIMARY",
+                "ID"
+            ],
+            "type": "string"
+        },
+        "PropertyUsage": {
+            "enum": [
+                "INHERIT",
+                "DIMENSION",
+                "MEASURE"
+            ],
+            "type": "string"
+        },
+        "PutDataSetRefreshPropertiesRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DataSetId",
+                    "shape": "ResourceId"
+                },
+                "DataSetRefreshProperties": {
+                    "documentation": "<p>The dataset refresh properties.</p>",
+                    "shape": "DataSetRefreshProperties"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "DataSetId",
+                "DataSetRefreshProperties"
+            ],
+            "type": "structure"
+        },
+        "PutDataSetRefreshPropertiesResponse": {
+            "members": {
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "Query": {
             "max": 256,
             "min": 1,
             "type": "string"
         },
         "QueueInfo": {
             "documentation": "<p>Information about a queued dataset SPICE ingestion.</p>",
@@ -20508,14 +24728,22 @@
                 "Visibility": {
                     "documentation": "<p>The visibility settings of a radar chart.</p>",
                     "shape": "Visibility"
                 }
             },
             "type": "structure"
         },
+        "RadarChartAxesRangeScale": {
+            "enum": [
+                "AUTO",
+                "INDEPENDENT",
+                "SHARED"
+            ],
+            "type": "string"
+        },
         "RadarChartCategoryFieldList": {
             "max": 1,
             "member": {
                 "shape": "DimensionField"
             },
             "type": "list"
         },
@@ -20537,14 +24765,18 @@
                     "documentation": "<p>The color of the even-numbered alternate bands of a radar chart.</p>",
                     "shape": "HexColor"
                 },
                 "AlternateBandOddColor": {
                     "documentation": "<p>The color of the odd-numbered alternate bands of a radar chart.</p>",
                     "shape": "HexColor"
                 },
+                "AxesRangeScale": {
+                    "documentation": "<p>The axis behavior options of a radar chart.</p>",
+                    "shape": "RadarChartAxesRangeScale"
+                },
                 "BaseSeriesSettings": {
                     "documentation": "<p>The base sreies settings of a radar chart.</p>",
                     "shape": "RadarChartSeriesSettings"
                 },
                 "CategoryAxis": {
                     "documentation": "<p>The category axis of a radar chart.</p>",
                     "shape": "AxisDisplayOptions"
@@ -20678,14 +24910,28 @@
                 }
             },
             "required": [
                 "VisualId"
             ],
             "type": "structure"
         },
+        "RangeConstant": {
+            "documentation": "<p>A structure that represents a range constant.</p>",
+            "members": {
+                "Maximum": {
+                    "documentation": "<p>The maximum value for a range constant.</p>",
+                    "shape": "LimitedString"
+                },
+                "Minimum": {
+                    "documentation": "<p>The minimum value for a range constant.</p>",
+                    "shape": "LimitedString"
+                }
+            },
+            "type": "structure"
+        },
         "RangeEndsLabelType": {
             "documentation": "<p>The range ends label type of a data path label.</p>",
             "members": {
                 "Visibility": {
                     "documentation": "<p>The visibility of the range ends label.</p>",
                     "shape": "Visibility"
                 }
@@ -20810,15 +25056,14 @@
                 "MeasureAggregationFunction": {
                     "documentation": "<p>The aggregation function that is used in the dynamic data.</p>",
                     "shape": "AggregationFunction"
                 }
             },
             "required": [
                 "Column",
-                "MeasureAggregationFunction",
                 "Calculation"
             ],
             "type": "structure"
         },
         "ReferenceLineLabelConfiguration": {
             "documentation": "<p>The label configuration of a reference line.</p>",
             "members": {
@@ -20923,14 +25168,101 @@
         "ReferenceLineValueLabelRelativePosition": {
             "enum": [
                 "BEFORE_CUSTOM_LABEL",
                 "AFTER_CUSTOM_LABEL"
             ],
             "type": "string"
         },
+        "RefreshConfiguration": {
+            "documentation": "<p>The refresh configuration of a dataset.</p>",
+            "members": {
+                "IncrementalRefresh": {
+                    "documentation": "<p>The incremental refresh for the dataset.</p>",
+                    "shape": "IncrementalRefresh"
+                }
+            },
+            "required": [
+                "IncrementalRefresh"
+            ],
+            "type": "structure"
+        },
+        "RefreshFrequency": {
+            "documentation": "<p>Specifies the interval between each scheduled refresh of a dataset.</p>",
+            "members": {
+                "Interval": {
+                    "documentation": "<p>The interval between scheduled refreshes. Valid values are as follows:</p> <ul> <li> <p> <code>MINUTE15</code>: The dataset refreshes every 15 minutes. This value is only supported for incremental refreshes. This interval can only be used for one schedule per dataset.</p> </li> <li> <p> <code>MINUTE30</code>:The dataset refreshes every 30 minutes. This value is only supported for incremental refreshes. This interval can only be used for one schedule per dataset.</p> </li> <li> <p> <code>HOURLY</code>: The dataset refreshes every hour. This interval can only be used for one schedule per dataset.</p> </li> <li> <p> <code>DAILY</code>: The dataset refreshes every day.</p> </li> <li> <p> <code>WEEKLY</code>: The dataset refreshes every week.</p> </li> <li> <p> <code>MONTHLY</code>: The dataset refreshes every month.</p> </li> </ul>",
+                    "shape": "RefreshInterval"
+                },
+                "RefreshOnDay": {
+                    "documentation": "<p>The day of the week that you want to schedule the refresh on. This value is required for weekly and monthly refresh intervals.</p>",
+                    "shape": "ScheduleRefreshOnEntity"
+                },
+                "TimeOfTheDay": {
+                    "documentation": "<p>The time of day that you want the datset to refresh. This value is expressed in HH:MM format. This field is not required for schedules that refresh hourly.</p>",
+                    "shape": "String"
+                },
+                "Timezone": {
+                    "documentation": "<p>The timezone that you want the refresh schedule to use. The timezone ID must match a corresponding ID found on <code>java.util.time.getAvailableIDs()</code>.</p>",
+                    "shape": "String"
+                }
+            },
+            "required": [
+                "Interval"
+            ],
+            "type": "structure"
+        },
+        "RefreshInterval": {
+            "enum": [
+                "MINUTE15",
+                "MINUTE30",
+                "HOURLY",
+                "DAILY",
+                "WEEKLY",
+                "MONTHLY"
+            ],
+            "type": "string"
+        },
+        "RefreshSchedule": {
+            "documentation": "<p>The refresh schedule of a dataset.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the refresh schedule.</p>",
+                    "shape": "Arn"
+                },
+                "RefreshType": {
+                    "documentation": "<p>The type of refresh that a datset undergoes. Valid values are as follows:</p> <ul> <li> <p> <code>FULL_REFRESH</code>: A complete refresh of a dataset.</p> </li> <li> <p> <code>INCREMENTAL_REFRESH</code>: A partial refresh of some rows of a dataset, based on the time window specified.</p> </li> </ul> <p>For more information on full and incremental refreshes, see <a href=\"https://docs.aws.amazon.com/quicksight/latest/user/refreshing-imported-data.html\">Refreshing SPICE data</a> in the <i>Amazon QuickSight User Guide</i>.</p>",
+                    "shape": "IngestionType"
+                },
+                "ScheduleFrequency": {
+                    "documentation": "<p>The frequency for the refresh schedule.</p>",
+                    "shape": "RefreshFrequency"
+                },
+                "ScheduleId": {
+                    "documentation": "<p>An identifier for the refresh schedule.</p>",
+                    "shape": "String"
+                },
+                "StartAfterDateTime": {
+                    "documentation": "<p>Time after which the refresh schedule can be started, expressed in <code>YYYY-MM-DDTHH:MM:SS</code> format.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "ScheduleId",
+                "ScheduleFrequency",
+                "RefreshType"
+            ],
+            "type": "structure"
+        },
+        "RefreshSchedules": {
+            "member": {
+                "documentation": "<p>A list of <code>RefreshSchedule</code> objects.</p>",
+                "shape": "RefreshSchedule"
+            },
+            "type": "list"
+        },
         "RegisterUserRequest": {
             "members": {
                 "AwsAccountId": {
                     "documentation": "<p>The ID for the Amazon Web Services account that the user is in. Currently, you use the ID for the Amazon Web Services account that contains your Amazon QuickSight account.</p>",
                     "location": "uri",
                     "locationName": "AwsAccountId",
                     "shape": "AwsAccountId"
@@ -21039,14 +25371,18 @@
                 "InitialDashboardId"
             ],
             "type": "structure"
         },
         "RegisteredUserDashboardFeatureConfigurations": {
             "documentation": "<p>The feature configuration for an embedded dashboard.</p>",
             "members": {
+                "Bookmarks": {
+                    "documentation": "<p>The bookmarks configuration for an embedded dashboard in Amazon QuickSight.</p>",
+                    "shape": "BookmarksConfigurations"
+                },
                 "StatePersistence": {
                     "documentation": "<p>The state persistence settings of an embedded dashboard.</p>",
                     "shape": "StatePersistenceConfigurations"
                 }
             },
             "type": "structure"
         },
@@ -21548,14 +25884,18 @@
         "RowLevelPermissionTagConfiguration": {
             "documentation": "<p>The configuration of tags on a dataset to set row-level security. </p>",
             "members": {
                 "Status": {
                     "documentation": "<p>The status of row-level security tags. If enabled, the status is <code>ENABLED</code>. If disabled, the status is <code>DISABLED</code>.</p>",
                     "shape": "Status"
                 },
+                "TagRuleConfigurations": {
+                    "documentation": "<p>A list of tag configuration rules to apply to a dataset. All tag configurations have the OR condition. Tags within each tile will be joined (AND). At least one rule in this structure must have all tag values assigned to it to apply Row-level security (RLS) to the dataset.</p>",
+                    "shape": "RowLevelPermissionTagRuleConfigurationList"
+                },
                 "TagRules": {
                     "documentation": "<p>A set of rules associated with row-level security, such as the tag names and columns that they are assigned to.</p>",
                     "shape": "RowLevelPermissionTagRuleList"
                 }
             },
             "required": [
                 "TagRules"
@@ -21588,14 +25928,30 @@
             },
             "required": [
                 "TagKey",
                 "ColumnName"
             ],
             "type": "structure"
         },
+        "RowLevelPermissionTagRuleConfiguration": {
+            "max": 50,
+            "member": {
+                "shape": "SessionTagKey"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "RowLevelPermissionTagRuleConfigurationList": {
+            "max": 50,
+            "member": {
+                "shape": "RowLevelPermissionTagRuleConfiguration"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "RowLevelPermissionTagRuleList": {
             "max": 50,
             "member": {
                 "shape": "RowLevelPermissionTagRule"
             },
             "min": 1,
             "type": "list"
@@ -21652,14 +26008,18 @@
             },
             "required": [
                 "DataSourceArn",
                 "InputColumns"
             ],
             "type": "structure"
         },
+        "S3Uri": {
+            "pattern": "^(https|s3)://([^/]+)/?(.*)$",
+            "type": "string"
+        },
         "SameSheetTargetVisualConfiguration": {
             "documentation": "<p>The configuration of the same-sheet target visuals that you want to be filtered.</p> <p>This is a union type structure. For this structure to be valid, only one of the attributes can be defined.</p>",
             "members": {
                 "TargetVisualOptions": {
                     "documentation": "<p>The options that choose the target visual in the same sheet.</p> <p>Valid values are defined as follows:</p> <ul> <li> <p> <code>ALL_VISUALS</code>: Applies the filter operation to all visuals in the same sheet.</p> </li> </ul>",
                     "shape": "TargetVisualOptions"
                 },
@@ -21766,14 +26126,18 @@
         "ScatterPlotCategoricallyAggregatedFieldWells": {
             "documentation": "<p>The aggregated field well of a scatter plot.</p>",
             "members": {
                 "Category": {
                     "documentation": "<p>The category field well of a scatter plot.</p>",
                     "shape": "DimensionFieldList"
                 },
+                "Label": {
+                    "documentation": "<p>The label field well of a scatter plot.</p>",
+                    "shape": "DimensionFieldList"
+                },
                 "Size": {
                     "documentation": "<p>The size field well of a scatter plot.</p>",
                     "shape": "MeasureFieldList"
                 },
                 "XAxis": {
                     "documentation": "<p>The x-axis field well of a scatter plot.</p> <p>The x-axis is aggregated by category.</p>",
                     "shape": "MeasureFieldList"
@@ -21827,27 +26191,35 @@
             },
             "type": "structure"
         },
         "ScatterPlotFieldWells": {
             "documentation": "<p>The field well configuration of a scatter plot.</p> <p>This is a union type structure. For this structure to be valid, only one of the attributes can be defined.</p>",
             "members": {
                 "ScatterPlotCategoricallyAggregatedFieldWells": {
-                    "documentation": "<p>The aggregated field wells of a scatter plot. Scatter plots that have a field in the category (group/color) field will have aggregated field wells. The x and y-axes of these scatter plots are aggregated by category.</p>",
+                    "documentation": "<p>The aggregated field wells of a scatter plot. The x and y-axes of scatter plots with aggregated field wells are aggregated by category, label, or both.</p>",
                     "shape": "ScatterPlotCategoricallyAggregatedFieldWells"
                 },
                 "ScatterPlotUnaggregatedFieldWells": {
-                    "documentation": "<p>The unaggregated field wells of a scatter plot. Scatter plots without a category field well have unaggregated field wells. The x and y-axes of these scatter plots are unaggregated.</p>",
+                    "documentation": "<p>The unaggregated field wells of a scatter plot. The x and y-axes of these scatter plots are unaggregated.</p>",
                     "shape": "ScatterPlotUnaggregatedFieldWells"
                 }
             },
             "type": "structure"
         },
         "ScatterPlotUnaggregatedFieldWells": {
             "documentation": "<p>The unaggregated field wells of a scatter plot.</p>",
             "members": {
+                "Category": {
+                    "documentation": "<p>The category field well of a scatter plot.</p>",
+                    "shape": "DimensionFieldList"
+                },
+                "Label": {
+                    "documentation": "<p>The label field well of a scatter plot.</p>",
+                    "shape": "DimensionFieldList"
+                },
                 "Size": {
                     "documentation": "<p>The size field well of a scatter plot.</p>",
                     "shape": "MeasureFieldList"
                 },
                 "XAxis": {
                     "documentation": "<p>The x-axis field well of a scatter plot.</p> <p>The x-axis is a dimension field and cannot be aggregated.</p>",
                     "shape": "DimensionFieldList"
@@ -21888,14 +26260,28 @@
                 }
             },
             "required": [
                 "VisualId"
             ],
             "type": "structure"
         },
+        "ScheduleRefreshOnEntity": {
+            "documentation": "<p>The refresh on entity for weekly or monthly schedules.</p>",
+            "members": {
+                "DayOfMonth": {
+                    "documentation": "<p>The day of the month that you want to schedule refresh on.</p>",
+                    "shape": "DayOfMonth"
+                },
+                "DayOfWeek": {
+                    "documentation": "<p>The day of the week that you want to schedule a refresh on.</p>",
+                    "shape": "DayOfWeek"
+                }
+            },
+            "type": "structure"
+        },
         "ScrollBarOptions": {
             "documentation": "<p>The visual display options for a data zoom scroll bar.</p>",
             "members": {
                 "Visibility": {
                     "documentation": "<p>The visibility of the data zoom scroll bar.</p>",
                     "shape": "Visibility"
                 },
@@ -22344,14 +26730,28 @@
                 "Padding": {
                     "documentation": "<p>The spacing between section content and its top, bottom, left, and right edges.</p> <p>There is no padding by default.</p>",
                     "shape": "Spacing"
                 }
             },
             "type": "structure"
         },
+        "SecurityGroupId": {
+            "max": 255,
+            "min": 1,
+            "pattern": "^sg-[0-9a-z]*$",
+            "type": "string"
+        },
+        "SecurityGroupIdList": {
+            "max": 16,
+            "member": {
+                "shape": "SecurityGroupId"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "SelectAllValueOptions": {
             "enum": [
                 "ALL_VALUES"
             ],
             "type": "string"
         },
         "SelectedFieldList": {
@@ -22381,14 +26781,66 @@
         "SelectedTooltipType": {
             "enum": [
                 "BASIC",
                 "DETAILED"
             ],
             "type": "string"
         },
+        "SemanticEntityType": {
+            "documentation": "<p>A structure that represents a semantic entity type.</p>",
+            "members": {
+                "SubTypeName": {
+                    "documentation": "<p>The semantic entity sub type name.</p>",
+                    "shape": "LimitedString"
+                },
+                "TypeName": {
+                    "documentation": "<p>The semantic entity type name.</p>",
+                    "shape": "LimitedString"
+                },
+                "TypeParameters": {
+                    "documentation": "<p>The semantic entity type parameters.</p>",
+                    "shape": "TypeParameters"
+                }
+            },
+            "type": "structure"
+        },
+        "SemanticType": {
+            "documentation": "<p>A structure that represents a semantic type.</p>",
+            "members": {
+                "FalseyCellValue": {
+                    "documentation": "<p>The semantic type falsey cell value.</p>",
+                    "shape": "SensitiveString"
+                },
+                "FalseyCellValueSynonyms": {
+                    "documentation": "<p>The other names or aliases for the false cell value.</p>",
+                    "shape": "SensitiveStringList"
+                },
+                "SubTypeName": {
+                    "documentation": "<p>The semantic type sub type name.</p>",
+                    "shape": "LimitedString"
+                },
+                "TruthyCellValue": {
+                    "documentation": "<p>The semantic type truthy cell value.</p>",
+                    "shape": "SensitiveString"
+                },
+                "TruthyCellValueSynonyms": {
+                    "documentation": "<p>The other names or aliases for the true cell value.</p>",
+                    "shape": "SensitiveStringList"
+                },
+                "TypeName": {
+                    "documentation": "<p>The semantic type name.</p>",
+                    "shape": "LimitedString"
+                },
+                "TypeParameters": {
+                    "documentation": "<p>The semantic type parameters.</p>",
+                    "shape": "TypeParameters"
+                }
+            },
+            "type": "structure"
+        },
         "SensitiveDouble": {
             "sensitive": true,
             "type": "double"
         },
         "SensitiveDoubleList": {
             "member": {
                 "shape": "SensitiveDouble"
@@ -23082,14 +27534,127 @@
                 "DisableSsl": {
                     "documentation": "<p>A Boolean option to control whether SSL should be disabled.</p>",
                     "shape": "Boolean"
                 }
             },
             "type": "structure"
         },
+        "StartAssetBundleExportJobRequest": {
+            "members": {
+                "AssetBundleExportJobId": {
+                    "documentation": "<p>The ID of the job. This ID is unique while the job is running. After the job is completed, you can reuse this ID for another job.</p>",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account to export assets from.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "CloudFormationOverridePropertyConfiguration": {
+                    "documentation": "<p>An optional collection of structures that generate CloudFormation parameters to override the existing resource property values when the resource is exported to a new CloudFormation template.</p> <p>Use this field if the <code>ExportFormat</code> field of a <code>StartAssetBundleExportJobRequest</code> API call is set to <code>CLOUDFORMATION_JSON</code>.</p>",
+                    "shape": "AssetBundleCloudFormationOverridePropertyConfiguration"
+                },
+                "ExportFormat": {
+                    "documentation": "<p>The export data format.</p>",
+                    "shape": "AssetBundleExportFormat"
+                },
+                "IncludeAllDependencies": {
+                    "documentation": "<p>A Boolean that determines whether all dependencies of each resource ARN are recursively exported with the job. For example, say you provided a Dashboard ARN to the <code>ResourceArns</code> parameter. If you set <code>IncludeAllDependencies</code> to <code>TRUE</code>, any theme, dataset, and data source resource that is a dependency of the dashboard is also exported.</p>",
+                    "shape": "Boolean"
+                },
+                "ResourceArns": {
+                    "documentation": "<p>An array of resource ARNs to export. The following resources are supported.</p> <ul> <li> <p> <code>Analysis</code> </p> </li> <li> <p> <code>Dashboard</code> </p> </li> <li> <p> <code>DataSet</code> </p> </li> <li> <p> <code>DataSource</code> </p> </li> <li> <p> <code>RefreshSchedule</code> </p> </li> <li> <p> <code>Theme</code> </p> </li> <li> <p> <code>VPCConnection</code> </p> </li> </ul> <p>The API caller must have the necessary permissions in their IAM role to access each resource before the resources can be exported.</p>",
+                    "shape": "AssetBundleResourceArns"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "AssetBundleExportJobId",
+                "ResourceArns",
+                "ExportFormat"
+            ],
+            "type": "structure"
+        },
+        "StartAssetBundleExportJobResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the export job.</p>",
+                    "shape": "Arn"
+                },
+                "AssetBundleExportJobId": {
+                    "documentation": "<p>The ID of the job. This ID is unique while the job is running. After the job is completed, you can reuse this ID for another job.</p>",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services response ID for this operation.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the response.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
+        "StartAssetBundleImportJobRequest": {
+            "members": {
+                "AssetBundleImportJobId": {
+                    "documentation": "<p>The ID of the job. This ID is unique while the job is running. After the job is completed, you can reuse this ID for another job.</p>",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "AssetBundleImportSource": {
+                    "documentation": "<p>The source of the asset bundle zip file that contains the data that you want to import.</p>",
+                    "shape": "AssetBundleImportSource"
+                },
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account to import assets into. </p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "FailureAction": {
+                    "documentation": "<p>The failure action for the import job.</p> <p>If you choose <code>ROLLBACK</code>, failed import jobs will attempt to undo any asset changes caused by the failed job.</p> <p>If you choose <code>DO_NOTHING</code>, failed import jobs will not attempt to roll back any asset changes caused by the failed job, possibly keeping the Amazon QuickSight account in an inconsistent state.</p>",
+                    "shape": "AssetBundleImportFailureAction"
+                },
+                "OverrideParameters": {
+                    "documentation": "<p>Optional overrides to be applied to the resource configuration before import.</p>",
+                    "shape": "AssetBundleImportJobOverrideParameters"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "AssetBundleImportJobId",
+                "AssetBundleImportSource"
+            ],
+            "type": "structure"
+        },
+        "StartAssetBundleImportJobResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the import job.</p>",
+                    "shape": "Arn"
+                },
+                "AssetBundleImportJobId": {
+                    "documentation": "<p>The ID of the job. This ID is unique while the job is running. After the job is completed, you can reuse this ID for another job.</p>",
+                    "shape": "ShortRestrictiveResourceId"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services response ID for this operation.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the response.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "StatePersistenceConfigurations": {
             "documentation": "<p>The state perssitence configuration of an embedded dashboard.</p>",
             "members": {
                 "Enabled": {
                     "documentation": "<p>Determines if a Amazon QuickSight dashboard's state persistence settings are turned on or off.</p>",
                     "shape": "Boolean"
                 }
@@ -23108,14 +27673,65 @@
         },
         "StatusCode": {
             "type": "integer"
         },
         "String": {
             "type": "string"
         },
+        "StringDatasetParameter": {
+            "documentation": "<p>A string parameter for a dataset.</p>",
+            "members": {
+                "DefaultValues": {
+                    "documentation": "<p>A list of default values for a given string dataset parameter type. This structure only accepts static values.</p>",
+                    "shape": "StringDatasetParameterDefaultValues"
+                },
+                "Id": {
+                    "documentation": "<p>An identifier for the string parameter that is created in the dataset.</p>",
+                    "shape": "DatasetParameterId"
+                },
+                "Name": {
+                    "documentation": "<p>The name of the string parameter that is created in the dataset.</p>",
+                    "shape": "DatasetParameterName"
+                },
+                "ValueType": {
+                    "documentation": "<p>The value type of the dataset parameter. Valid values are <code>single value</code> or <code>multi value</code>.</p>",
+                    "shape": "DatasetParameterValueType"
+                }
+            },
+            "required": [
+                "Id",
+                "Name",
+                "ValueType"
+            ],
+            "type": "structure"
+        },
+        "StringDatasetParameterDefaultValue": {
+            "documentation": "<p>The default value for the string parameter.</p>",
+            "max": 512,
+            "min": 0,
+            "type": "string"
+        },
+        "StringDatasetParameterDefaultValues": {
+            "documentation": "<p>The default values of a string parameter.</p>",
+            "members": {
+                "StaticValues": {
+                    "documentation": "<p>A list of static default values for a given string parameter.</p>",
+                    "shape": "StringDatasetParameterValueList"
+                }
+            },
+            "type": "structure"
+        },
+        "StringDatasetParameterValueList": {
+            "max": 32,
+            "member": {
+                "shape": "StringDatasetParameterDefaultValue"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "StringDefaultValueList": {
             "max": 50000,
             "member": {
                 "shape": "SensitiveStringObject"
             },
             "type": "list"
         },
@@ -23174,14 +27790,17 @@
         "StringParameterDeclaration": {
             "documentation": "<p>A parameter declaration for the <code>String</code> data type.</p>",
             "members": {
                 "DefaultValues": {
                     "documentation": "<p>The default values of a parameter. If the parameter is a single-value parameter, a maximum of one default value can be provided.</p>",
                     "shape": "StringDefaultValues"
                 },
+                "MappedDataSetParameters": {
+                    "shape": "MappedDataSetParameters"
+                },
                 "Name": {
                     "documentation": "<p>The name of the parameter that is being declared.</p>",
                     "shape": "ParameterName"
                 },
                 "ParameterValueType": {
                     "documentation": "<p>The value type determines whether the parameter is a single-value or multi-value parameter.</p>",
                     "shape": "ParameterValueType"
@@ -23214,14 +27833,28 @@
                 "ValueWhenUnsetOption": {
                     "documentation": "<p>The built-in options for default values. The value can be one of the following:</p> <ul> <li> <p> <code>RECOMMENDED</code>: The recommended value.</p> </li> <li> <p> <code>NULL</code>: The <code>NULL</code> value.</p> </li> </ul>",
                     "shape": "ValueWhenUnsetOption"
                 }
             },
             "type": "structure"
         },
+        "SubnetId": {
+            "max": 255,
+            "min": 1,
+            "pattern": "^subnet-[0-9a-z]*$",
+            "type": "string"
+        },
+        "SubnetIdList": {
+            "max": 15,
+            "member": {
+                "shape": "SubnetId"
+            },
+            "min": 2,
+            "type": "list"
+        },
         "SubtotalOptions": {
             "documentation": "<p>The subtotal options.</p>",
             "members": {
                 "CustomLabel": {
                     "documentation": "<p>The custom label string for the subtotal cells.</p>",
                     "shape": "String"
                 },
@@ -23254,14 +27887,20 @@
         },
         "Suffix": {
             "max": 128,
             "min": 1,
             "sensitive": true,
             "type": "string"
         },
+        "Synonyms": {
+            "member": {
+                "shape": "LimitedString"
+            },
+            "type": "list"
+        },
         "TableAggregatedFieldWells": {
             "documentation": "<p>The aggregated field well for the table.</p>",
             "members": {
                 "GroupBy": {
                     "documentation": "<p>The group by field well for a pivot table. Values are grouped by group by fields.</p>",
                     "shape": "DimensionFieldList"
                 },
@@ -23865,15 +28504,15 @@
         },
         "TagValue": {
             "max": 256,
             "min": 1,
             "type": "string"
         },
         "TargetVisualList": {
-            "max": 30,
+            "max": 50,
             "member": {
                 "shape": "ShortRestrictiveResourceId"
             },
             "min": 1,
             "type": "list"
         },
         "TargetVisualOptions": {
@@ -24908,14 +29547,579 @@
         "TopBottomSortOrder": {
             "enum": [
                 "PERCENT_DIFFERENCE",
                 "ABSOLUTE_DIFFERENCE"
             ],
             "type": "string"
         },
+        "TopicCalculatedField": {
+            "documentation": "<p>A structure that represents a calculated field.</p>",
+            "members": {
+                "Aggregation": {
+                    "documentation": "<p>The default aggregation. Valid values for this structure are <code>SUM</code>, <code>MAX</code>, <code>MIN</code>, <code>COUNT</code>, <code>DISTINCT_COUNT</code>, and <code>AVERAGE</code>.</p>",
+                    "shape": "DefaultAggregation"
+                },
+                "AllowedAggregations": {
+                    "documentation": "<p>The list of aggregation types that are allowed for the calculated field. Valid values for this structure are <code>COUNT</code>, <code>DISTINCT_COUNT</code>, <code>MIN</code>, <code>MAX</code>, <code>MEDIAN</code>, <code>SUM</code>, <code>AVERAGE</code>, <code>STDEV</code>, <code>STDEVP</code>, <code>VAR</code>, <code>VARP</code>, and <code>PERCENTILE</code>.</p>",
+                    "shape": "AuthorSpecifiedAggregations"
+                },
+                "CalculatedFieldDescription": {
+                    "documentation": "<p>The calculated field description.</p>",
+                    "shape": "LimitedString"
+                },
+                "CalculatedFieldName": {
+                    "documentation": "<p>The calculated field name.</p>",
+                    "shape": "LimitedString"
+                },
+                "CalculatedFieldSynonyms": {
+                    "documentation": "<p>The other names or aliases for the calculated field.</p>",
+                    "shape": "Synonyms"
+                },
+                "CellValueSynonyms": {
+                    "documentation": "<p>The other names or aliases for the calculated field cell value.</p>",
+                    "shape": "CellValueSynonyms"
+                },
+                "ColumnDataRole": {
+                    "documentation": "<p>The column data role for a calculated field. Valid values for this structure are <code>DIMENSION</code> and <code>MEASURE</code>.</p>",
+                    "shape": "ColumnDataRole"
+                },
+                "ComparativeOrder": {
+                    "documentation": "<p>The order in which data is displayed for the calculated field when it's used in a comparative context.</p>",
+                    "shape": "ComparativeOrder"
+                },
+                "DefaultFormatting": {
+                    "documentation": "<p>The default formatting definition.</p>",
+                    "shape": "DefaultFormatting"
+                },
+                "DisableIndexing": {
+                    "documentation": "<p>A Boolean value that indicates if a calculated field is visible in the autocomplete.</p>",
+                    "shape": "NullableBoolean"
+                },
+                "Expression": {
+                    "documentation": "<p>The calculated field expression.</p>",
+                    "shape": "Expression"
+                },
+                "IsIncludedInTopic": {
+                    "documentation": "<p>A boolean value that indicates if a calculated field is included in the topic.</p>",
+                    "shape": "Boolean"
+                },
+                "NeverAggregateInFilter": {
+                    "documentation": "<p>A Boolean value that indicates whether to never aggregate calculated field in filters.</p>",
+                    "shape": "Boolean"
+                },
+                "NotAllowedAggregations": {
+                    "documentation": "<p>The list of aggregation types that are not allowed for the calculated field. Valid values for this structure are <code>COUNT</code>, <code>DISTINCT_COUNT</code>, <code>MIN</code>, <code>MAX</code>, <code>MEDIAN</code>, <code>SUM</code>, <code>AVERAGE</code>, <code>STDEV</code>, <code>STDEVP</code>, <code>VAR</code>, <code>VARP</code>, and <code>PERCENTILE</code>.</p>",
+                    "shape": "AuthorSpecifiedAggregations"
+                },
+                "SemanticType": {
+                    "documentation": "<p>The semantic type.</p>",
+                    "shape": "SemanticType"
+                },
+                "TimeGranularity": {
+                    "documentation": "<p>The level of time precision that is used to aggregate <code>DateTime</code> values.</p>",
+                    "shape": "TopicTimeGranularity"
+                }
+            },
+            "required": [
+                "CalculatedFieldName",
+                "Expression"
+            ],
+            "type": "structure"
+        },
+        "TopicCalculatedFields": {
+            "member": {
+                "shape": "TopicCalculatedField"
+            },
+            "type": "list"
+        },
+        "TopicCategoryFilter": {
+            "documentation": "<p>A structure that represents a category filter.</p>",
+            "members": {
+                "CategoryFilterFunction": {
+                    "documentation": "<p>The category filter function. Valid values for this structure are <code>EXACT</code> and <code>CONTAINS</code>.</p>",
+                    "shape": "CategoryFilterFunction"
+                },
+                "CategoryFilterType": {
+                    "documentation": "<p>The category filter type. This element is used to specify whether a filter is a simple category filter or an inverse category filter.</p>",
+                    "shape": "CategoryFilterType"
+                },
+                "Constant": {
+                    "documentation": "<p>The constant used in a category filter.</p>",
+                    "shape": "TopicCategoryFilterConstant"
+                },
+                "Inverse": {
+                    "documentation": "<p>A Boolean value that indicates if the filter is inverse.</p>",
+                    "shape": "Boolean"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicCategoryFilterConstant": {
+            "documentation": "<p>A constant used in a category filter.</p>",
+            "members": {
+                "CollectiveConstant": {
+                    "documentation": "<p>A collective constant used in a category filter. This element is used to specify a list of values for the constant.</p>",
+                    "shape": "CollectiveConstant"
+                },
+                "ConstantType": {
+                    "documentation": "<p>The type of category filter constant. This element is used to specify whether a constant is a singular or collective. Valid values are <code>SINGULAR</code> and <code>COLLECTIVE</code>.</p>",
+                    "shape": "ConstantType"
+                },
+                "SingularConstant": {
+                    "documentation": "<p>A singular constant used in a category filter. This element is used to specify a single value for the constant.</p>",
+                    "shape": "LimitedString"
+                }
+            },
+            "sensitive": true,
+            "type": "structure"
+        },
+        "TopicColumn": {
+            "documentation": "<p>Represents a column in a dataset.</p>",
+            "members": {
+                "Aggregation": {
+                    "documentation": "<p>The type of aggregation that is performed on the column data when it's queried. Valid values for this structure are <code>SUM</code>, <code>MAX</code>, <code>MIN</code>, <code>COUNT</code>, <code>DISTINCT_COUNT</code>, and <code>AVERAGE</code>.</p>",
+                    "shape": "DefaultAggregation"
+                },
+                "AllowedAggregations": {
+                    "documentation": "<p>The list of aggregation types that are allowed for the column. Valid values for this structure are <code>COUNT</code>, <code>DISTINCT_COUNT</code>, <code>MIN</code>, <code>MAX</code>, <code>MEDIAN</code>, <code>SUM</code>, <code>AVERAGE</code>, <code>STDEV</code>, <code>STDEVP</code>, <code>VAR</code>, <code>VARP</code>, and <code>PERCENTILE</code>.</p>",
+                    "shape": "AuthorSpecifiedAggregations"
+                },
+                "CellValueSynonyms": {
+                    "documentation": "<p>The other names or aliases for the column cell value.</p>",
+                    "shape": "CellValueSynonyms"
+                },
+                "ColumnDataRole": {
+                    "documentation": "<p>The role of the column in the data. Valid values are <code>DIMENSION</code> and <code>MEASURE</code>.</p>",
+                    "shape": "ColumnDataRole"
+                },
+                "ColumnDescription": {
+                    "documentation": "<p>A description of the column and its contents.</p>",
+                    "shape": "LimitedString"
+                },
+                "ColumnFriendlyName": {
+                    "documentation": "<p>A user-friendly name for the column.</p>",
+                    "shape": "LimitedString"
+                },
+                "ColumnName": {
+                    "documentation": "<p>The name of the column.</p>",
+                    "shape": "LimitedString"
+                },
+                "ColumnSynonyms": {
+                    "documentation": "<p>The other names or aliases for the column.</p>",
+                    "shape": "Synonyms"
+                },
+                "ComparativeOrder": {
+                    "documentation": "<p>The order in which data is displayed for the column when it's used in a comparative context.</p>",
+                    "shape": "ComparativeOrder"
+                },
+                "DefaultFormatting": {
+                    "documentation": "<p>The default formatting used for values in the column.</p>",
+                    "shape": "DefaultFormatting"
+                },
+                "DisableIndexing": {
+                    "documentation": "<p>A Boolean value that indicates whether the column shows in the autocomplete functionality.</p>",
+                    "shape": "NullableBoolean"
+                },
+                "IsIncludedInTopic": {
+                    "documentation": "<p>A Boolean value that indicates whether the column is included in the query results.</p>",
+                    "shape": "Boolean"
+                },
+                "NeverAggregateInFilter": {
+                    "documentation": "<p>A Boolean value that indicates whether to aggregate the column data when it's used in a filter context.</p>",
+                    "shape": "Boolean"
+                },
+                "NotAllowedAggregations": {
+                    "documentation": "<p>The list of aggregation types that are not allowed for the column. Valid values for this structure are <code>COUNT</code>, <code>DISTINCT_COUNT</code>, <code>MIN</code>, <code>MAX</code>, <code>MEDIAN</code>, <code>SUM</code>, <code>AVERAGE</code>, <code>STDEV</code>, <code>STDEVP</code>, <code>VAR</code>, <code>VARP</code>, and <code>PERCENTILE</code>.</p>",
+                    "shape": "AuthorSpecifiedAggregations"
+                },
+                "SemanticType": {
+                    "documentation": "<p>The semantic type of data contained in the column.</p>",
+                    "shape": "SemanticType"
+                },
+                "TimeGranularity": {
+                    "documentation": "<p>The level of time precision that is used to aggregate <code>DateTime</code> values.</p>",
+                    "shape": "TopicTimeGranularity"
+                }
+            },
+            "required": [
+                "ColumnName"
+            ],
+            "type": "structure"
+        },
+        "TopicColumns": {
+            "member": {
+                "shape": "TopicColumn"
+            },
+            "type": "list"
+        },
+        "TopicDateRangeFilter": {
+            "documentation": "<p>A filter used to restrict data based on a range of dates or times.</p>",
+            "members": {
+                "Constant": {
+                    "documentation": "<p>The constant used in a date range filter.</p>",
+                    "shape": "TopicRangeFilterConstant"
+                },
+                "Inclusive": {
+                    "documentation": "<p>A Boolean value that indicates whether the date range filter should include the boundary values. If set to true, the filter includes the start and end dates. If set to false, the filter excludes them.</p>",
+                    "shape": "Boolean"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicDetails": {
+            "documentation": "<p>A structure that describes the details of a topic, such as its name, description, and associated data sets.</p>",
+            "members": {
+                "DataSets": {
+                    "documentation": "<p>The data sets that the topic is associated with.</p>",
+                    "shape": "Datasets"
+                },
+                "Description": {
+                    "documentation": "<p>The description of the topic.</p>",
+                    "shape": "LimitedString"
+                },
+                "Name": {
+                    "documentation": "<p>The name of the topic.</p>",
+                    "shape": "ResourceName"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicFilter": {
+            "documentation": "<p>A structure that represents a filter used to select items for a topic.</p>",
+            "members": {
+                "CategoryFilter": {
+                    "documentation": "<p>The category filter that is associated with this filter.</p>",
+                    "shape": "TopicCategoryFilter"
+                },
+                "DateRangeFilter": {
+                    "documentation": "<p>The date range filter.</p>",
+                    "shape": "TopicDateRangeFilter"
+                },
+                "FilterClass": {
+                    "documentation": "<p>The class of the filter. Valid values for this structure are <code>ENFORCED_VALUE_FILTER</code>, <code>CONDITIONAL_VALUE_FILTER</code>, and <code>NAMED_VALUE_FILTER</code>.</p>",
+                    "shape": "FilterClass"
+                },
+                "FilterDescription": {
+                    "documentation": "<p>A description of the filter used to select items for a topic.</p>",
+                    "shape": "LimitedString"
+                },
+                "FilterName": {
+                    "documentation": "<p>The name of the filter.</p>",
+                    "shape": "LimitedString"
+                },
+                "FilterSynonyms": {
+                    "documentation": "<p>The other names or aliases for the filter.</p>",
+                    "shape": "Synonyms"
+                },
+                "FilterType": {
+                    "documentation": "<p>The type of the filter. Valid values for this structure are <code>CATEGORY_FILTER</code>, <code>NUMERIC_EQUALITY_FILTER</code>, <code>NUMERIC_RANGE_FILTER</code>, <code>DATE_RANGE_FILTER</code>, and <code>RELATIVE_DATE_FILTER</code>.</p>",
+                    "shape": "NamedFilterType"
+                },
+                "NumericEqualityFilter": {
+                    "documentation": "<p>The numeric equality filter.</p>",
+                    "shape": "TopicNumericEqualityFilter"
+                },
+                "NumericRangeFilter": {
+                    "documentation": "<p>The numeric range filter.</p>",
+                    "shape": "TopicNumericRangeFilter"
+                },
+                "OperandFieldName": {
+                    "documentation": "<p>The name of the field that the filter operates on.</p>",
+                    "shape": "LimitedString"
+                },
+                "RelativeDateFilter": {
+                    "documentation": "<p>The relative date filter.</p>",
+                    "shape": "TopicRelativeDateFilter"
+                }
+            },
+            "required": [
+                "FilterName",
+                "OperandFieldName"
+            ],
+            "type": "structure"
+        },
+        "TopicFilters": {
+            "member": {
+                "shape": "TopicFilter"
+            },
+            "type": "list"
+        },
+        "TopicId": {
+            "max": 256,
+            "pattern": "^[A-Za-z0-9-_.\\\\+]*$",
+            "type": "string"
+        },
+        "TopicNamedEntities": {
+            "member": {
+                "shape": "TopicNamedEntity"
+            },
+            "type": "list"
+        },
+        "TopicNamedEntity": {
+            "documentation": "<p>A structure that represents a named entity.</p>",
+            "members": {
+                "Definition": {
+                    "documentation": "<p>The definition of a named entity.</p>",
+                    "shape": "NamedEntityDefinitions"
+                },
+                "EntityDescription": {
+                    "documentation": "<p>The description of the named entity.</p>",
+                    "shape": "LimitedString"
+                },
+                "EntityName": {
+                    "documentation": "<p>The name of the named entity.</p>",
+                    "shape": "LimitedString"
+                },
+                "EntitySynonyms": {
+                    "documentation": "<p>The other names or aliases for the named entity.</p>",
+                    "shape": "Synonyms"
+                },
+                "SemanticEntityType": {
+                    "documentation": "<p>The type of named entity that a topic represents.</p>",
+                    "shape": "SemanticEntityType"
+                }
+            },
+            "required": [
+                "EntityName"
+            ],
+            "type": "structure"
+        },
+        "TopicNumericEqualityFilter": {
+            "documentation": "<p>A filter that filters topics based on the value of a numeric field. The filter includes only topics whose numeric field value matches the specified value.</p>",
+            "members": {
+                "Aggregation": {
+                    "documentation": "<p>An aggregation function that specifies how to calculate the value of a numeric field for a topic. Valid values for this structure are <code>NO_AGGREGATION</code>, <code>SUM</code>, <code>AVERAGE</code>, <code>COUNT</code>, <code>DISTINCT_COUNT</code>, <code>MAX</code>, <code>MEDIAN</code>, <code>MIN</code>, <code>STDEV</code>, <code>STDEVP</code>, <code>VAR</code>, and <code>VARP</code>.</p>",
+                    "shape": "NamedFilterAggType"
+                },
+                "Constant": {
+                    "documentation": "<p>The constant used in a numeric equality filter.</p>",
+                    "shape": "TopicSingularFilterConstant"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicNumericRangeFilter": {
+            "documentation": "<p>A filter that filters topics based on the value of a numeric field. The filter includes only topics whose numeric field value falls within the specified range.</p>",
+            "members": {
+                "Aggregation": {
+                    "documentation": "<p>An aggregation function that specifies how to calculate the value of a numeric field for a topic, Valid values for this structure are <code>NO_AGGREGATION</code>, <code>SUM</code>, <code>AVERAGE</code>, <code>COUNT</code>, <code>DISTINCT_COUNT</code>, <code>MAX</code>, <code>MEDIAN</code>, <code>MIN</code>, <code>STDEV</code>, <code>STDEVP</code>, <code>VAR</code>, and <code>VARP</code>.</p>",
+                    "shape": "NamedFilterAggType"
+                },
+                "Constant": {
+                    "documentation": "<p>The constant used in a numeric range filter.</p>",
+                    "shape": "TopicRangeFilterConstant"
+                },
+                "Inclusive": {
+                    "documentation": "<p>A Boolean value that indicates whether the endpoints of the numeric range are included in the filter. If set to true, topics whose numeric field value is equal to the endpoint values will be included in the filter. If set to false, topics whose numeric field value is equal to the endpoint values will be excluded from the filter.</p>",
+                    "shape": "Boolean"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicNumericSeparatorSymbol": {
+            "enum": [
+                "COMMA",
+                "DOT"
+            ],
+            "type": "string"
+        },
+        "TopicRangeFilterConstant": {
+            "documentation": "<p>A constant value that is used in a range filter to specify the endpoints of the range.</p>",
+            "members": {
+                "ConstantType": {
+                    "documentation": "<p>The data type of the constant value that is used in a range filter. Valid values for this structure are <code>RANGE</code>.</p>",
+                    "shape": "ConstantType"
+                },
+                "RangeConstant": {
+                    "documentation": "<p>The value of the constant that is used to specify the endpoints of a range filter.</p>",
+                    "shape": "RangeConstant"
+                }
+            },
+            "sensitive": true,
+            "type": "structure"
+        },
+        "TopicRefreshDetails": {
+            "documentation": "<p>The details about the refresh of a topic.</p>",
+            "members": {
+                "RefreshArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic refresh.</p>",
+                    "shape": "Arn"
+                },
+                "RefreshId": {
+                    "documentation": "<p>The ID of the refresh, which occurs as a result of topic creation or topic update.</p>",
+                    "shape": "ResourceId"
+                },
+                "RefreshStatus": {
+                    "documentation": "<p>The status of the refresh job that indicates whether the job is still running, completed successfully, or failed.</p>",
+                    "shape": "TopicRefreshStatus"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicRefreshSchedule": {
+            "documentation": "<p>A structure that represents a topic refresh schedule.</p>",
+            "members": {
+                "BasedOnSpiceSchedule": {
+                    "documentation": "<p>A Boolean value that controls whether to schedule runs at the same schedule that is specified in SPICE dataset.</p>",
+                    "shape": "Boolean"
+                },
+                "IsEnabled": {
+                    "documentation": "<p>A Boolean value that controls whether to schedule is enabled.</p>",
+                    "shape": "NullableBoolean"
+                },
+                "RepeatAt": {
+                    "documentation": "<p>The time of day when the refresh should run, for example, Monday-Sunday.</p>",
+                    "shape": "LimitedString"
+                },
+                "StartingAt": {
+                    "documentation": "<p>The starting date and time for the refresh schedule.</p>",
+                    "shape": "Timestamp"
+                },
+                "Timezone": {
+                    "documentation": "<p>The timezone that you want the refresh schedule to use.</p>",
+                    "shape": "LimitedString"
+                },
+                "TopicScheduleType": {
+                    "documentation": "<p>The type of refresh schedule. Valid values for this structure are <code>HOURLY</code>, <code>DAILY</code>, <code>WEEKLY</code>, and <code>MONTHLY</code>.</p>",
+                    "shape": "TopicScheduleType"
+                }
+            },
+            "required": [
+                "IsEnabled",
+                "BasedOnSpiceSchedule"
+            ],
+            "type": "structure"
+        },
+        "TopicRefreshScheduleSummaries": {
+            "member": {
+                "shape": "TopicRefreshScheduleSummary"
+            },
+            "type": "list"
+        },
+        "TopicRefreshScheduleSummary": {
+            "documentation": "<p>A summary of the refresh schedule details for a dataset.</p>",
+            "members": {
+                "DatasetArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the dataset.</p>",
+                    "shape": "Arn"
+                },
+                "DatasetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "shape": "LimitedString"
+                },
+                "DatasetName": {
+                    "documentation": "<p>The name of the dataset.</p>",
+                    "shape": "LimitedString"
+                },
+                "RefreshSchedule": {
+                    "documentation": "<p>The definition of a refresh schedule.</p>",
+                    "shape": "TopicRefreshSchedule"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicRefreshStatus": {
+            "enum": [
+                "INITIALIZED",
+                "RUNNING",
+                "FAILED",
+                "COMPLETED",
+                "CANCELLED"
+            ],
+            "type": "string"
+        },
+        "TopicRelativeDateFilter": {
+            "documentation": "<p>A structure that represents a relative date filter.</p>",
+            "members": {
+                "Constant": {
+                    "documentation": "<p>The constant used in a relative date filter.</p>",
+                    "shape": "TopicSingularFilterConstant"
+                },
+                "RelativeDateFilterFunction": {
+                    "documentation": "<p>The function to be used in a relative date filter to determine the range of dates to include in the results. Valid values for this structure are <code>BEFORE</code>, <code>AFTER</code>, and <code>BETWEEN</code>.</p>",
+                    "shape": "TopicRelativeDateFilterFunction"
+                },
+                "TimeGranularity": {
+                    "documentation": "<p>The level of time precision that is used to aggregate <code>DateTime</code> values.</p>",
+                    "shape": "TopicTimeGranularity"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicRelativeDateFilterFunction": {
+            "enum": [
+                "PREVIOUS",
+                "THIS",
+                "LAST",
+                "NEXT",
+                "NOW"
+            ],
+            "type": "string"
+        },
+        "TopicScheduleType": {
+            "enum": [
+                "HOURLY",
+                "DAILY",
+                "WEEKLY",
+                "MONTHLY"
+            ],
+            "type": "string"
+        },
+        "TopicSingularFilterConstant": {
+            "documentation": "<p>A structure that represents a singular filter constant, used in filters to specify a single value to match against.</p>",
+            "members": {
+                "ConstantType": {
+                    "documentation": "<p>The type of the singular filter constant. Valid values for this structure are <code>SINGULAR</code>.</p>",
+                    "shape": "ConstantType"
+                },
+                "SingularConstant": {
+                    "documentation": "<p>The value of the singular filter constant.</p>",
+                    "shape": "LimitedString"
+                }
+            },
+            "sensitive": true,
+            "type": "structure"
+        },
+        "TopicSummaries": {
+            "member": {
+                "shape": "TopicSummary"
+            },
+            "type": "list"
+        },
+        "TopicSummary": {
+            "documentation": "<p>A topic summary.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "Name": {
+                    "documentation": "<p>The name of the topic.</p>",
+                    "shape": "ResourceName"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID for the topic. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "TopicTimeGranularity": {
+            "enum": [
+                "SECOND",
+                "MINUTE",
+                "HOUR",
+                "DAY",
+                "WEEK",
+                "MONTH",
+                "QUARTER",
+                "YEAR"
+            ],
+            "type": "string"
+        },
         "TotalAggregationComputation": {
             "documentation": "<p>The total aggregation computation configuration.</p>",
             "members": {
                 "ComputationId": {
                     "documentation": "<p>The ID for a computation.</p>",
                     "shape": "ShortRestrictiveResourceId"
                 },
@@ -24971,14 +30175,17 @@
                     "documentation": "<p>An operation that creates calculated columns. Columns created in one such operation form a lexical closure.</p>",
                     "shape": "CreateColumnsOperation"
                 },
                 "FilterOperation": {
                     "documentation": "<p>An operation that filters rows based on some condition.</p>",
                     "shape": "FilterOperation"
                 },
+                "OverrideDatasetParameterOperation": {
+                    "shape": "OverrideDatasetParameterOperation"
+                },
                 "ProjectOperation": {
                     "documentation": "<p>An operation that projects columns. Operations that come after a projection can only refer to projected columns.</p>",
                     "shape": "ProjectOperation"
                 },
                 "RenameColumnOperation": {
                     "documentation": "<p>An operation that renames a column.</p>",
                     "shape": "RenameColumnOperation"
@@ -25160,14 +30367,23 @@
             ],
             "type": "structure"
         },
         "TypeCastFormat": {
             "max": 32,
             "type": "string"
         },
+        "TypeParameters": {
+            "key": {
+                "shape": "LimitedString"
+            },
+            "type": "map",
+            "value": {
+                "shape": "LimitedString"
+            }
+        },
         "Typography": {
             "documentation": "<p>Determines the typography options.</p>",
             "members": {
                 "FontFamilies": {
                     "documentation": "<p>Determines the list of font families.</p>",
                     "shape": "FontList"
                 }
@@ -25282,14 +30498,21 @@
         "UnaggregatedFieldList": {
             "max": 200,
             "member": {
                 "shape": "UnaggregatedField"
             },
             "type": "list"
         },
+        "UndefinedSpecifiedValueType": {
+            "enum": [
+                "LEAST",
+                "MOST"
+            ],
+            "type": "string"
+        },
         "UnicodeIcon": {
             "pattern": "^[^\\u0000-\\u00FF]$",
             "type": "string"
         },
         "UniqueValuesComputation": {
             "documentation": "<p>The unique values computation configuration.</p>",
             "members": {
@@ -25890,14 +31113,18 @@
                     "location": "uri",
                     "locationName": "DataSetId",
                     "shape": "ResourceId"
                 },
                 "DataSetUsageConfiguration": {
                     "shape": "DataSetUsageConfiguration"
                 },
+                "DatasetParameters": {
+                    "documentation": "<p>The parameter declarations of the dataset.</p>",
+                    "shape": "DatasetParameterList"
+                },
                 "FieldFolders": {
                     "documentation": "<p>The folder that contains fields and nested subfolders for your dataset.</p>",
                     "shape": "FieldFolderMap"
                 },
                 "ImportMode": {
                     "documentation": "<p>Indicates whether you want to import the data into SPICE.</p>",
                     "shape": "DataSetImportMode"
@@ -26232,15 +31459,15 @@
                 }
             },
             "type": "structure"
         },
         "UpdateIAMPolicyAssignmentRequest": {
             "members": {
                 "AssignmentName": {
-                    "documentation": "<p>The name of the assignment, also called a rule. This name must be unique within an Amazon Web Services account.</p>",
+                    "documentation": "<p>The name of the assignment, also called a rule. The name must be unique within the Amazon Web Services account.</p>",
                     "location": "uri",
                     "locationName": "AssignmentName",
                     "shape": "IAMPolicyAssignmentName"
                 },
                 "AssignmentStatus": {
                     "documentation": "<p>The status of the assignment. Possible values are as follows:</p> <ul> <li> <p> <code>ENABLED</code> - Anything specified in this assignment is used when creating the data source.</p> </li> <li> <p> <code>DISABLED</code> - This assignment isn't used when creating the data source.</p> </li> <li> <p> <code>DRAFT</code> - This assignment is an unfinished draft and isn't used when creating the data source.</p> </li> </ul>",
                     "shape": "AssignmentStatus"
@@ -26382,14 +31609,62 @@
                     "documentation": "<p>The HTTP status of the request.</p>",
                     "location": "statusCode",
                     "shape": "StatusCode"
                 }
             },
             "type": "structure"
         },
+        "UpdateRefreshScheduleRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DataSetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DataSetId",
+                    "shape": "ResourceId"
+                },
+                "Schedule": {
+                    "documentation": "<p>The refresh schedule.</p>",
+                    "shape": "RefreshSchedule"
+                }
+            },
+            "required": [
+                "DataSetId",
+                "AwsAccountId",
+                "Schedule"
+            ],
+            "type": "structure"
+        },
+        "UpdateRefreshScheduleResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the refresh schedule.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "ScheduleId": {
+                    "documentation": "<p>The ID of the refresh schedule.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                }
+            },
+            "type": "structure"
+        },
         "UpdateResourcePermissionList": {
             "max": 100,
             "member": {
                 "shape": "ResourcePermission"
             },
             "type": "list"
         },
@@ -26736,14 +32011,180 @@
                 "VersionArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the new version of the theme.</p>",
                     "shape": "Arn"
                 }
             },
             "type": "structure"
         },
+        "UpdateTopicPermissionsRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topic that you want to update the permissions for.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "GrantPermissions": {
+                    "documentation": "<p>The resource permissions that you want to grant to the topic.</p>",
+                    "shape": "UpdateResourcePermissionList"
+                },
+                "RevokePermissions": {
+                    "documentation": "<p>The resource permissions that you want to revoke from the topic.</p>",
+                    "shape": "UpdateResourcePermissionList"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId"
+            ],
+            "type": "structure"
+        },
+        "UpdateTopicPermissionsResponse": {
+            "members": {
+                "Permissions": {
+                    "documentation": "<p>A list of resource permissions on the topic.</p>",
+                    "shape": "ResourcePermissionList"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "UpdateTopicRefreshScheduleRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topic whose refresh schedule you want to update.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DatasetId": {
+                    "documentation": "<p>The ID of the dataset.</p>",
+                    "location": "uri",
+                    "locationName": "DatasetId",
+                    "shape": "String"
+                },
+                "RefreshSchedule": {
+                    "documentation": "<p>The definition of a refresh schedule.</p>",
+                    "shape": "TopicRefreshSchedule"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId",
+                "DatasetId",
+                "RefreshSchedule"
+            ],
+            "type": "structure"
+        },
+        "UpdateTopicRefreshScheduleResponse": {
+            "members": {
+                "DatasetArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the dataset.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
+        "UpdateTopicRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The ID of the Amazon Web Services account that contains the topic that you want to update.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "Topic": {
+                    "documentation": "<p>The definition of the topic that you want to update.</p>",
+                    "shape": "TopicDetails"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "TopicId",
+                    "shape": "TopicId"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "TopicId",
+                "Topic"
+            ],
+            "type": "structure"
+        },
+        "UpdateTopicResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic.</p>",
+                    "shape": "Arn"
+                },
+                "RefreshArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the topic refresh.</p>",
+                    "shape": "Arn"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "TopicId": {
+                    "documentation": "<p>The ID of the topic that you want to modify. This ID is unique per Amazon Web Services Region for each Amazon Web Services account.</p>",
+                    "shape": "TopicId"
+                }
+            },
+            "type": "structure"
+        },
         "UpdateUserRequest": {
             "members": {
                 "AwsAccountId": {
                     "documentation": "<p>The ID for the Amazon Web Services account that the user is in. Currently, you use the ID for the Amazon Web Services account that contains your Amazon QuickSight account.</p>",
                     "location": "uri",
                     "locationName": "AwsAccountId",
                     "shape": "AwsAccountId"
@@ -26812,14 +32253,89 @@
                 "User": {
                     "documentation": "<p>The Amazon QuickSight user.</p>",
                     "shape": "User"
                 }
             },
             "type": "structure"
         },
+        "UpdateVPCConnectionRequest": {
+            "members": {
+                "AwsAccountId": {
+                    "documentation": "<p>The Amazon Web Services account ID of the account that contains the VPC connection that you want to update.</p>",
+                    "location": "uri",
+                    "locationName": "AwsAccountId",
+                    "shape": "AwsAccountId"
+                },
+                "DnsResolvers": {
+                    "documentation": "<p>A list of IP addresses of DNS resolver endpoints for the VPC connection.</p>",
+                    "shape": "DnsResolverList"
+                },
+                "Name": {
+                    "documentation": "<p>The display name for the VPC connection.</p>",
+                    "shape": "ResourceName"
+                },
+                "RoleArn": {
+                    "documentation": "<p>An IAM role associated with the VPC connection.</p>",
+                    "shape": "RoleArn"
+                },
+                "SecurityGroupIds": {
+                    "documentation": "<p>A list of security group IDs for the VPC connection.</p>",
+                    "shape": "SecurityGroupIdList"
+                },
+                "SubnetIds": {
+                    "documentation": "<p>A list of subnet IDs for the VPC connection.</p>",
+                    "shape": "SubnetIdList"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC connection that you're updating. This ID is a unique identifier for each Amazon Web Services Region in an Amazon Web Services account.</p>",
+                    "location": "uri",
+                    "locationName": "VPCConnectionId",
+                    "shape": "VPCConnectionResourceIdUnrestricted"
+                }
+            },
+            "required": [
+                "AwsAccountId",
+                "VPCConnectionId",
+                "Name",
+                "SubnetIds",
+                "SecurityGroupIds",
+                "RoleArn"
+            ],
+            "type": "structure"
+        },
+        "UpdateVPCConnectionResponse": {
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the VPC connection.</p>",
+                    "shape": "Arn"
+                },
+                "AvailabilityStatus": {
+                    "documentation": "<p>The availability status of the VPC connection.</p>",
+                    "shape": "VPCConnectionAvailabilityStatus"
+                },
+                "RequestId": {
+                    "documentation": "<p>The Amazon Web Services request ID for this operation.</p>",
+                    "shape": "String"
+                },
+                "Status": {
+                    "documentation": "<p>The HTTP status of the request.</p>",
+                    "location": "statusCode",
+                    "shape": "StatusCode"
+                },
+                "UpdateStatus": {
+                    "documentation": "<p>The update status of the VPC connection's last update.</p>",
+                    "shape": "VPCConnectionResourceStatus"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC connection that you are updating. This ID is a unique identifier for each Amazon Web Services Region in anAmazon Web Services account.</p>",
+                    "shape": "VPCConnectionResourceIdUnrestricted"
+                }
+            },
+            "type": "structure"
+        },
         "UploadSettings": {
             "documentation": "<p>Information about the format for a source file or files.</p>",
             "members": {
                 "ContainsHeader": {
                     "box": true,
                     "documentation": "<p>Whether the file has a header row, or the files each have a header row.</p>",
                     "shape": "Boolean"
@@ -26911,19 +32427,161 @@
                 "AUTHOR",
                 "READER",
                 "RESTRICTED_AUTHOR",
                 "RESTRICTED_READER"
             ],
             "type": "string"
         },
-        "Username": {
-            "max": 64,
+        "VPCConnection": {
+            "documentation": "<p>The structure of a VPC connection.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the VPC connection.</p>",
+                    "shape": "Arn"
+                },
+                "AvailabilityStatus": {
+                    "documentation": "<p>The availability status of the VPC connection.</p>",
+                    "shape": "VPCConnectionAvailabilityStatus"
+                },
+                "CreatedTime": {
+                    "documentation": "<p>The time that the VPC connection was created.</p>",
+                    "shape": "Timestamp"
+                },
+                "DnsResolvers": {
+                    "documentation": "<p>A list of IP addresses of DNS resolver endpoints for the VPC connection.</p>",
+                    "shape": "StringList"
+                },
+                "LastUpdatedTime": {
+                    "documentation": "<p>The time that the VPC connection was last updated.</p>",
+                    "shape": "Timestamp"
+                },
+                "Name": {
+                    "documentation": "<p>The display name for the VPC connection.</p>",
+                    "shape": "ResourceName"
+                },
+                "NetworkInterfaces": {
+                    "documentation": "<p>A list of network interfaces.</p>",
+                    "shape": "NetworkInterfaceList"
+                },
+                "RoleArn": {
+                    "documentation": "<p>The ARN of the IAM role associated with the VPC connection.</p>",
+                    "shape": "String"
+                },
+                "SecurityGroupIds": {
+                    "documentation": "<p>The Amazon EC2 security group IDs associated with the VPC connection.</p>",
+                    "shape": "SecurityGroupIdList"
+                },
+                "Status": {
+                    "documentation": "<p>The status of the VPC connection.</p>",
+                    "shape": "VPCConnectionResourceStatus"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC connection that you're creating. This ID is a unique identifier for each Amazon Web Services Region in an Amazon Web Services account.</p>",
+                    "shape": "VPCConnectionResourceIdUnrestricted"
+                },
+                "VPCId": {
+                    "documentation": "<p>The Amazon EC2 VPC ID associated with the VPC connection.</p>",
+                    "shape": "String"
+                }
+            },
+            "type": "structure"
+        },
+        "VPCConnectionAvailabilityStatus": {
+            "enum": [
+                "AVAILABLE",
+                "UNAVAILABLE",
+                "PARTIALLY_AVAILABLE"
+            ],
+            "type": "string"
+        },
+        "VPCConnectionResourceIdRestricted": {
+            "max": 1000,
             "min": 1,
+            "pattern": "[\\w\\-]+",
             "type": "string"
         },
+        "VPCConnectionResourceIdUnrestricted": {
+            "max": 1000,
+            "min": 1,
+            "type": "string"
+        },
+        "VPCConnectionResourceStatus": {
+            "enum": [
+                "CREATION_IN_PROGRESS",
+                "CREATION_SUCCESSFUL",
+                "CREATION_FAILED",
+                "UPDATE_IN_PROGRESS",
+                "UPDATE_SUCCESSFUL",
+                "UPDATE_FAILED",
+                "DELETION_IN_PROGRESS",
+                "DELETION_FAILED",
+                "DELETED"
+            ],
+            "type": "string"
+        },
+        "VPCConnectionSummary": {
+            "documentation": "<p>The summary metadata that describes a VPC connection.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the VPC connection.</p>",
+                    "shape": "Arn"
+                },
+                "AvailabilityStatus": {
+                    "documentation": "<p>The availability status of the VPC connection.</p>",
+                    "shape": "VPCConnectionAvailabilityStatus"
+                },
+                "CreatedTime": {
+                    "documentation": "<p>The time that the VPC connection was created.</p>",
+                    "shape": "Timestamp"
+                },
+                "DnsResolvers": {
+                    "documentation": "<p>A list of IP addresses of DNS resolver endpoints for the VPC connection.</p>",
+                    "shape": "StringList"
+                },
+                "LastUpdatedTime": {
+                    "documentation": "<p>The time that the VPC connection was last updated.</p>",
+                    "shape": "Timestamp"
+                },
+                "Name": {
+                    "documentation": "<p>The display name for the VPC connection.</p>",
+                    "shape": "ResourceName"
+                },
+                "NetworkInterfaces": {
+                    "documentation": "<p>A list of network interfaces.</p>",
+                    "shape": "NetworkInterfaceList"
+                },
+                "RoleArn": {
+                    "documentation": "<p>The ARN of the IAM role associated with the VPC connection.</p>",
+                    "shape": "String"
+                },
+                "SecurityGroupIds": {
+                    "documentation": "<p>The Amazon EC2 security group IDs associated with the VPC connection.</p>",
+                    "shape": "SecurityGroupIdList"
+                },
+                "Status": {
+                    "documentation": "<p>The status of the VPC connection.</p>",
+                    "shape": "VPCConnectionResourceStatus"
+                },
+                "VPCConnectionId": {
+                    "documentation": "<p>The ID of the VPC connection that you're creating. This ID is a unique identifier for each Amazon Web Services Region in an Amazon Web Services account.</p>",
+                    "shape": "VPCConnectionResourceIdUnrestricted"
+                },
+                "VPCId": {
+                    "documentation": "<p>The Amazon EC2 VPC ID associated with the VPC connection.</p>",
+                    "shape": "String"
+                }
+            },
+            "type": "structure"
+        },
+        "VPCConnectionSummaryList": {
+            "member": {
+                "shape": "VPCConnectionSummary"
+            },
+            "type": "list"
+        },
         "ValueWhenUnsetOption": {
             "enum": [
                 "RECOMMENDED_VALUE",
                 "NULL"
             ],
             "type": "string"
         },
@@ -27157,15 +32815,15 @@
             "enum": [
                 "DATA_POINT_CLICK",
                 "DATA_POINT_MENU"
             ],
             "type": "string"
         },
         "VisualList": {
-            "max": 30,
+            "max": 50,
             "member": {
                 "shape": "Visual"
             },
             "type": "list"
         },
         "VisualMenuOption": {
             "documentation": "<p>The menu options for a visual.</p>",
```

### Comparing `botocore-a-la-carte-quicksight-1.29.99/botocore_a_la_carte_quicksight.egg-info/PKG-INFO` & `botocore-a-la-carte-quicksight-1.30.0/botocore_a_la_carte_quicksight.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-quicksight
-Version: 1.29.99
+Version: 1.30.0
 Summary: quicksight data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-quicksight-1.29.99/botocore_a_la_carte_quicksight.egg-info/SOURCES.txt` & `botocore-a-la-carte-quicksight-1.30.0/botocore_a_la_carte_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-quicksight-1.29.99/setup.py` & `botocore-a-la-carte-quicksight-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-quicksight',
-    version="1.29.99",
+    version="1.30.0",
     description='quicksight data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/quicksight/*/*.json'],
```

