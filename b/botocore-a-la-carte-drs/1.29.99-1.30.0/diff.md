# Comparing `tmp/botocore-a-la-carte-drs-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-drs-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-drs-1.29.99.tar", last modified: Sat Mar 25 01:22:35 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-drs-1.30.0.tar", last modified: Tue Jul  4 01:44:26 2023, max compression
```

## Comparing `botocore-a-la-carte-drs-1.29.99.tar` & `botocore-a-la-carte-drs-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.903122 botocore-a-la-carte-drs-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:35.000000 botocore-a-la-carte-drs-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:22:35.903122 botocore-a-la-carte-drs-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.899122 botocore-a-la-carte-drs-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.899122 botocore-a-la-carte-drs-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.899122 botocore-a-la-carte-drs-1.29.99/botocore/data/drs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.899122 botocore-a-la-carte-drs-1.29.99/botocore/data/drs/2020-02-26/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-03-25 01:22:12.000000 botocore-a-la-carte-drs-1.29.99/botocore/data/drs/2020-02-26/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-drs-1.29.99/botocore/data/drs/2020-02-26/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-25 01:22:12.000000 botocore-a-la-carte-drs-1.29.99/botocore/data/drs/2020-02-26/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   125593 2023-03-25 01:22:12.000000 botocore-a-la-carte-drs-1.29.99/botocore/data/drs/2020-02-26/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.899122 botocore-a-la-carte-drs-1.29.99/botocore_a_la_carte_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:22:35.000000 botocore-a-la-carte-drs-1.29.99/botocore_a_la_carte_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-25 01:22:35.000000 botocore-a-la-carte-drs-1.29.99/botocore_a_la_carte_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:35.000000 botocore-a-la-carte-drs-1.29.99/botocore_a_la_carte_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:35.000000 botocore-a-la-carte-drs-1.29.99/botocore_a_la_carte_drs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:35.903122 botocore-a-la-carte-drs-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-25 01:22:35.000000 botocore-a-la-carte-drs-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.578511 botocore-a-la-carte-drs-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:26.000000 botocore-a-la-carte-drs-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:26.578511 botocore-a-la-carte-drs-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.578511 botocore-a-la-carte-drs-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.578511 botocore-a-la-carte-drs-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.578511 botocore-a-la-carte-drs-1.30.0/botocore/data/drs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.578511 botocore-a-la-carte-drs-1.30.0/botocore/data/drs/2020-02-26/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-04 01:44:02.000000 botocore-a-la-carte-drs-1.30.0/botocore/data/drs/2020-02-26/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-drs-1.30.0/botocore/data/drs/2020-02-26/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-04 01:44:02.000000 botocore-a-la-carte-drs-1.30.0/botocore/data/drs/2020-02-26/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   156756 2023-07-04 01:44:02.000000 botocore-a-la-carte-drs-1.30.0/botocore/data/drs/2020-02-26/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.578511 botocore-a-la-carte-drs-1.30.0/botocore_a_la_carte_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:26.000000 botocore-a-la-carte-drs-1.30.0/botocore_a_la_carte_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 01:44:26.000000 botocore-a-la-carte-drs-1.30.0/botocore_a_la_carte_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:26.000000 botocore-a-la-carte-drs-1.30.0/botocore_a_la_carte_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:26.000000 botocore-a-la-carte-drs-1.30.0/botocore_a_la_carte_drs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:26.578511 botocore-a-la-carte-drs-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-04 01:44:26.000000 botocore-a-la-carte-drs-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-drs-1.29.99/LICENSE.txt` & `botocore-a-la-carte-drs-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-drs-1.29.99/PKG-INFO` & `botocore-a-la-carte-drs-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-drs
-Version: 1.29.99
+Version: 1.30.0
 Summary: drs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-drs-1.29.99/botocore/data/drs/2020-02-26/endpoint-rule-set-1.json` & `botocore-a-la-carte-drs-1.30.0/botocore/data/drs/2020-02-26/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-drs-1.29.99/botocore/data/drs/2020-02-26/paginators-1.json` & `botocore-a-la-carte-drs-1.30.0/botocore/data/drs/2020-02-26/paginators-1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'pagination'": "{'DescribeLaunchConfigurationTemplates': OrderedDict([('input_token', "*

 * *                 "'nextToken'), ('output_token', 'nextToken'), ('limit_key', 'maxResults'), "*

 * *                 "('result_key', 'items')]), 'DescribeSourceNetworks': "*

 * *                 "OrderedDict([('input_token', 'nextToken'), ('output_token', 'nextToken'), "*

 * *                 "('limit_key', 'maxResults'), ('result_key', 'items')])}"}*

```diff
@@ -8,14 +8,20 @@
         },
         "DescribeJobs": {
             "input_token": "nextToken",
             "limit_key": "maxResults",
             "output_token": "nextToken",
             "result_key": "items"
         },
+        "DescribeLaunchConfigurationTemplates": {
+            "input_token": "nextToken",
+            "limit_key": "maxResults",
+            "output_token": "nextToken",
+            "result_key": "items"
+        },
         "DescribeRecoveryInstances": {
             "input_token": "nextToken",
             "limit_key": "maxResults",
             "output_token": "nextToken",
             "result_key": "items"
         },
         "DescribeRecoverySnapshots": {
@@ -26,14 +32,20 @@
         },
         "DescribeReplicationConfigurationTemplates": {
             "input_token": "nextToken",
             "limit_key": "maxResults",
             "output_token": "nextToken",
             "result_key": "items"
         },
+        "DescribeSourceNetworks": {
+            "input_token": "nextToken",
+            "limit_key": "maxResults",
+            "output_token": "nextToken",
+            "result_key": "items"
+        },
         "DescribeSourceServers": {
             "input_token": "nextToken",
             "limit_key": "maxResults",
             "output_token": "nextToken",
             "result_key": "items"
         },
         "ListExtensibleSourceServers": {
```

### Comparing `botocore-a-la-carte-drs-1.29.99/botocore/data/drs/2020-02-26/service-2.json` & `botocore-a-la-carte-drs-1.30.0/botocore/data/drs/2020-02-26/service-2.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.954315090357731%*

 * *Differences: {"'operations'": "{'RetryDataReplication': {'documentation': '<p>WARNING: RetryDataReplication is "*

 * *                 'deprecated. Causes the data replication initiation sequence to begin immediately '*

 * *                 'upon next Handshake for the specified Source Server ID, regardless of when the '*

 * *                 'previous initiation started. This command will work only if the Source Server is '*

 * *                 "stalled or is in a DISCONNECTED or STOPPED state. </p>', 'deprecated': True, "*

 * *               […]*

```diff
@@ -9,14 +9,52 @@
         "serviceFullName": "Elastic Disaster Recovery Service",
         "serviceId": "drs",
         "signatureVersion": "v4",
         "signingName": "drs",
         "uid": "drs-2020-02-26"
     },
     "operations": {
+        "AssociateSourceNetworkStack": {
+            "documentation": "<p>Associate a Source Network to an existing CloudFormation Stack and modify launch templates to use this network. Can be used for reverting to previously deployed CloudFormation stacks.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/AssociateSourceNetworkStack",
+                "responseCode": 202
+            },
+            "input": {
+                "shape": "AssociateSourceNetworkStackRequest"
+            },
+            "name": "AssociateSourceNetworkStack",
+            "output": {
+                "shape": "AssociateSourceNetworkStackResponse"
+            }
+        },
         "CreateExtendedSourceServer": {
             "documentation": "<p>Create an extended source server in the target Account based on the source server in staging account.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -47,14 +85,49 @@
                 "shape": "CreateExtendedSourceServerRequest"
             },
             "name": "CreateExtendedSourceServer",
             "output": {
                 "shape": "CreateExtendedSourceServerResponse"
             }
         },
+        "CreateLaunchConfigurationTemplate": {
+            "documentation": "<p>Creates a new Launch Configuration Template.</p>",
+            "errors": [
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/CreateLaunchConfigurationTemplate",
+                "responseCode": 201
+            },
+            "input": {
+                "shape": "CreateLaunchConfigurationTemplateRequest"
+            },
+            "name": "CreateLaunchConfigurationTemplate",
+            "output": {
+                "shape": "CreateLaunchConfigurationTemplateResponse"
+            }
+        },
         "CreateReplicationConfigurationTemplate": {
             "documentation": "<p>Creates a new ReplicationConfigurationTemplate.</p>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
                 {
@@ -82,14 +155,52 @@
                 "shape": "CreateReplicationConfigurationTemplateRequest"
             },
             "name": "CreateReplicationConfigurationTemplate",
             "output": {
                 "shape": "ReplicationConfigurationTemplate"
             }
         },
+        "CreateSourceNetwork": {
+            "documentation": "<p>Create a new Source Network resource for a provided VPC ID.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/CreateSourceNetwork",
+                "responseCode": 201
+            },
+            "input": {
+                "shape": "CreateSourceNetworkRequest"
+            },
+            "name": "CreateSourceNetwork",
+            "output": {
+                "shape": "CreateSourceNetworkResponse"
+            }
+        },
         "DeleteJob": {
             "documentation": "<p>Deletes a single Job by ID.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -115,14 +226,47 @@
                 "shape": "DeleteJobRequest"
             },
             "name": "DeleteJob",
             "output": {
                 "shape": "DeleteJobResponse"
             }
         },
+        "DeleteLaunchConfigurationTemplate": {
+            "documentation": "<p>Deletes a single Launch Configuration Template by ID.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/DeleteLaunchConfigurationTemplate",
+                "responseCode": 204
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "DeleteLaunchConfigurationTemplateRequest"
+            },
+            "name": "DeleteLaunchConfigurationTemplate",
+            "output": {
+                "shape": "DeleteLaunchConfigurationTemplateResponse"
+            }
+        },
         "DeleteRecoveryInstance": {
             "documentation": "<p>Deletes a single Recovery Instance by ID. This deletes the Recovery Instance resource from Elastic Disaster Recovery. The Recovery Instance must be disconnected first in order to delete it.</p>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
                 {
@@ -177,14 +321,47 @@
                 "shape": "DeleteReplicationConfigurationTemplateRequest"
             },
             "name": "DeleteReplicationConfigurationTemplate",
             "output": {
                 "shape": "DeleteReplicationConfigurationTemplateResponse"
             }
         },
+        "DeleteSourceNetwork": {
+            "documentation": "<p>Delete Source Network resource.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/DeleteSourceNetwork",
+                "responseCode": 204
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "DeleteSourceNetworkRequest"
+            },
+            "name": "DeleteSourceNetwork",
+            "output": {
+                "shape": "DeleteSourceNetworkResponse"
+            }
+        },
         "DeleteSourceServer": {
             "documentation": "<p>Deletes a single Source Server by ID. The Source Server must be disconnected first.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -268,14 +445,46 @@
                 "shape": "DescribeJobsRequest"
             },
             "name": "DescribeJobs",
             "output": {
                 "shape": "DescribeJobsResponse"
             }
         },
+        "DescribeLaunchConfigurationTemplates": {
+            "documentation": "<p>Lists all Launch Configuration Templates, filtered by Launch Configuration Template IDs</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/DescribeLaunchConfigurationTemplates",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "DescribeLaunchConfigurationTemplatesRequest"
+            },
+            "name": "DescribeLaunchConfigurationTemplates",
+            "output": {
+                "shape": "DescribeLaunchConfigurationTemplatesResponse"
+            }
+        },
         "DescribeRecoveryInstances": {
             "documentation": "<p>Lists all Recovery Instances or multiple Recovery Instances by ID.</p>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
                 {
@@ -361,14 +570,43 @@
                 "shape": "DescribeReplicationConfigurationTemplatesRequest"
             },
             "name": "DescribeReplicationConfigurationTemplates",
             "output": {
                 "shape": "DescribeReplicationConfigurationTemplatesResponse"
             }
         },
+        "DescribeSourceNetworks": {
+            "documentation": "<p>Lists all Source Networks or multiple Source Networks filtered by ID.</p>",
+            "errors": [
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/DescribeSourceNetworks",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "DescribeSourceNetworksRequest"
+            },
+            "name": "DescribeSourceNetworks",
+            "output": {
+                "shape": "DescribeSourceNetworksResponse"
+            }
+        },
         "DescribeSourceServers": {
             "documentation": "<p>Lists all Source Servers or multiple Source Servers filtered by ID.</p>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
                 {
@@ -454,14 +692,49 @@
                 "shape": "DisconnectSourceServerRequest"
             },
             "name": "DisconnectSourceServer",
             "output": {
                 "shape": "SourceServer"
             }
         },
+        "ExportSourceNetworkCfnTemplate": {
+            "documentation": "<p>Export the Source Network CloudFormation template to an S3 bucket.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/ExportSourceNetworkCfnTemplate",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ExportSourceNetworkCfnTemplateRequest"
+            },
+            "name": "ExportSourceNetworkCfnTemplate",
+            "output": {
+                "shape": "ExportSourceNetworkCfnTemplateResponse"
+            }
+        },
         "GetFailbackReplicationConfiguration": {
             "documentation": "<p>Lists all Failback ReplicationConfigurations, filtered by Recovery Instance ID.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -670,15 +943,17 @@
             },
             "name": "ListTagsForResource",
             "output": {
                 "shape": "ListTagsForResourceResponse"
             }
         },
         "RetryDataReplication": {
-            "documentation": "<p>Causes the data replication initiation sequence to begin immediately upon next Handshake for the specified Source Server ID, regardless of when the previous initiation started. This command will work only if the Source Server is stalled or is in a DISCONNECTED or STOPPED state.</p>",
+            "deprecated": true,
+            "deprecatedMessage": "WARNING: RetryDataReplication is deprecated",
+            "documentation": "<p>WARNING: RetryDataReplication is deprecated. Causes the data replication initiation sequence to begin immediately upon next Handshake for the specified Source Server ID, regardless of when the previous initiation started. This command will work only if the Source Server is stalled or is in a DISCONNECTED or STOPPED state. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "InternalServerException"
                 },
@@ -838,14 +1113,81 @@
                 "shape": "StartReplicationRequest"
             },
             "name": "StartReplication",
             "output": {
                 "shape": "StartReplicationResponse"
             }
         },
+        "StartSourceNetworkRecovery": {
+            "documentation": "<p>Deploy VPC for the specified Source Network and modify launch templates to use this network. The VPC will be deployed using a dedicated CloudFormation stack.</p>",
+            "errors": [
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/StartSourceNetworkRecovery",
+                "responseCode": 202
+            },
+            "input": {
+                "shape": "StartSourceNetworkRecoveryRequest"
+            },
+            "name": "StartSourceNetworkRecovery",
+            "output": {
+                "shape": "StartSourceNetworkRecoveryResponse"
+            }
+        },
+        "StartSourceNetworkReplication": {
+            "documentation": "<p>Starts replication for a Source Network. This action would make the Source Network protected.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/StartSourceNetworkReplication",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "StartSourceNetworkReplicationRequest"
+            },
+            "name": "StartSourceNetworkReplication",
+            "output": {
+                "shape": "StartSourceNetworkReplicationResponse"
+            }
+        },
         "StopFailback": {
             "documentation": "<p>Stops the failback process for a specified Recovery Instance. This changes the Failback State of the Recovery Instance back to FAILBACK_NOT_STARTED.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -896,14 +1238,49 @@
                 "shape": "StopReplicationRequest"
             },
             "name": "StopReplication",
             "output": {
                 "shape": "StopReplicationResponse"
             }
         },
+        "StopSourceNetworkReplication": {
+            "documentation": "<p>Stops replication for a Source Network. This action would make the Source Network unprotected.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/StopSourceNetworkReplication",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "StopSourceNetworkReplicationRequest"
+            },
+            "name": "StopSourceNetworkReplication",
+            "output": {
+                "shape": "StopSourceNetworkReplicationResponse"
+            }
+        },
         "TagResource": {
             "documentation": "<p>Adds or overwrites only the specified tags for the specified Elastic Disaster Recovery resource or resources. When you specify an existing tag key, the value is overwritten with the new value. Each resource can have a maximum of 50 tags. Each tag consists of a key and optional value.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -1053,14 +1430,49 @@
                 "shape": "UpdateLaunchConfigurationRequest"
             },
             "name": "UpdateLaunchConfiguration",
             "output": {
                 "shape": "LaunchConfiguration"
             }
         },
+        "UpdateLaunchConfigurationTemplate": {
+            "documentation": "<p>Updates an existing Launch Configuration Template by ID.</p>",
+            "errors": [
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "UninitializedAccountException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/UpdateLaunchConfigurationTemplate",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "UpdateLaunchConfigurationTemplateRequest"
+            },
+            "name": "UpdateLaunchConfigurationTemplate",
+            "output": {
+                "shape": "UpdateLaunchConfigurationTemplateResponse"
+            }
+        },
         "UpdateReplicationConfiguration": {
             "documentation": "<p>Allows you to update a ReplicationConfiguration by Source Server ID.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -1184,14 +1596,40 @@
             "max": 50,
             "member": {
                 "shape": "Account"
             },
             "min": 0,
             "type": "list"
         },
+        "AssociateSourceNetworkStackRequest": {
+            "members": {
+                "cfnStackName": {
+                    "documentation": "<p>CloudFormation template to associate with a Source Network.</p>",
+                    "shape": "CfnStackName"
+                },
+                "sourceNetworkID": {
+                    "documentation": "<p>The Source Network ID to associate with CloudFormation template.</p>",
+                    "shape": "SourceNetworkID"
+                }
+            },
+            "required": [
+                "cfnStackName",
+                "sourceNetworkID"
+            ],
+            "type": "structure"
+        },
+        "AssociateSourceNetworkStackResponse": {
+            "members": {
+                "job": {
+                    "documentation": "<p>The Source Network association Job.</p>",
+                    "shape": "Job"
+                }
+            },
+            "type": "structure"
+        },
         "AwsAvailabilityZone": {
             "max": 255,
             "min": 0,
             "pattern": "^(us(-gov)?|ap|ca|cn|eu|sa|af|me)-(central|north|(north(?:east|west))|south|south(?:east|west)|east|west)-[0-9][a-z]$",
             "type": "string"
         },
         "AwsRegion": {
@@ -1219,14 +1657,21 @@
                 "modelName": {
                     "documentation": "<p>The model name of the CPU.</p>",
                     "shape": "BoundedString"
                 }
             },
             "type": "structure"
         },
+        "CfnStackName": {
+            "max": 128,
+            "min": 1,
+            "pattern": "^[a-zA-Z][-a-zA-Z0-9]*$",
+            "sensitive": true,
+            "type": "string"
+        },
         "ConflictException": {
             "documentation": "<p>The request could not be completed due to a conflict with the current state of the target resource.</p>",
             "error": {
                 "httpStatusCode": 409,
                 "senderFault": true
             },
             "exception": true,
@@ -1246,19 +1691,19 @@
                     "shape": "LargeBoundedString"
                 }
             },
             "type": "structure"
         },
         "ConversionMap": {
             "key": {
-                "shape": "ebsSnapshot"
+                "shape": "EbsSnapshot"
             },
             "type": "map",
             "value": {
-                "shape": "ebsSnapshot"
+                "shape": "EbsSnapshot"
             }
         },
         "ConversionProperties": {
             "documentation": "<p>Properties of a conversion job</p>",
             "members": {
                 "dataTimestamp": {
                     "documentation": "<p>The timestamp of when the snapshot being converted was taken</p>",
@@ -1312,20 +1757,66 @@
                 "sourceServer": {
                     "documentation": "<p>Created extended source server.</p>",
                     "shape": "SourceServer"
                 }
             },
             "type": "structure"
         },
+        "CreateLaunchConfigurationTemplateRequest": {
+            "members": {
+                "copyPrivateIp": {
+                    "documentation": "<p>Copy private IP.</p>",
+                    "shape": "Boolean"
+                },
+                "copyTags": {
+                    "documentation": "<p>Copy tags.</p>",
+                    "shape": "Boolean"
+                },
+                "exportBucketArn": {
+                    "documentation": "<p>S3 bucket ARN to export Source Network templates.</p>",
+                    "shape": "ARN"
+                },
+                "launchDisposition": {
+                    "documentation": "<p>Launch disposition.</p>",
+                    "shape": "LaunchDisposition"
+                },
+                "licensing": {
+                    "documentation": "<p>Licensing.</p>",
+                    "shape": "Licensing"
+                },
+                "tags": {
+                    "documentation": "<p>Request to associate tags during creation of a Launch Configuration Template.</p>",
+                    "shape": "TagsMap"
+                },
+                "targetInstanceTypeRightSizingMethod": {
+                    "documentation": "<p>Target instance type right-sizing method.</p>",
+                    "shape": "TargetInstanceTypeRightSizingMethod"
+                }
+            },
+            "type": "structure"
+        },
+        "CreateLaunchConfigurationTemplateResponse": {
+            "members": {
+                "launchConfigurationTemplate": {
+                    "documentation": "<p>Created Launch Configuration Template.</p>",
+                    "shape": "LaunchConfigurationTemplate"
+                }
+            },
+            "type": "structure"
+        },
         "CreateReplicationConfigurationTemplateRequest": {
             "members": {
                 "associateDefaultSecurityGroup": {
                     "documentation": "<p>Whether to associate the default Elastic Disaster Recovery Security group with the Replication Configuration Template.</p>",
                     "shape": "Boolean"
                 },
+                "autoReplicateNewDisks": {
+                    "documentation": "<p>Whether to allow the AWS replication agent to automatically replicate newly added disks.</p>",
+                    "shape": "Boolean"
+                },
                 "bandwidthThrottling": {
                     "documentation": "<p>Configure bandwidth throttling for the outbound data transfer rate of the Source Server in Mbps.</p>",
                     "shape": "PositiveInteger"
                 },
                 "createPublicIP": {
                     "documentation": "<p>Whether to create a Public IP for the Recovery Instance by default.</p>",
                     "shape": "Boolean"
@@ -1387,14 +1878,49 @@
                 "replicationServersSecurityGroupsIDs",
                 "stagingAreaSubnetId",
                 "stagingAreaTags",
                 "useDedicatedReplicationServer"
             ],
             "type": "structure"
         },
+        "CreateSourceNetworkRequest": {
+            "members": {
+                "originAccountID": {
+                    "documentation": "<p>Account containing the VPC to protect.</p>",
+                    "shape": "AccountID"
+                },
+                "originRegion": {
+                    "documentation": "<p>Region containing the VPC to protect.</p>",
+                    "shape": "AwsRegion"
+                },
+                "tags": {
+                    "documentation": "<p>A set of tags to be associated with the Source Network resource.</p>",
+                    "shape": "TagsMap"
+                },
+                "vpcID": {
+                    "documentation": "<p>Which VPC ID to protect.</p>",
+                    "shape": "VpcID"
+                }
+            },
+            "required": [
+                "originAccountID",
+                "originRegion",
+                "vpcID"
+            ],
+            "type": "structure"
+        },
+        "CreateSourceNetworkResponse": {
+            "members": {
+                "sourceNetworkID": {
+                    "documentation": "<p>ID of the created Source Network.</p>",
+                    "shape": "SourceNetworkID"
+                }
+            },
+            "type": "structure"
+        },
         "DataReplicationError": {
             "documentation": "<p>Error in data replication.</p>",
             "members": {
                 "error": {
                     "documentation": "<p>Error in data replication.</p>",
                     "shape": "DataReplicationErrorString"
                 },
@@ -1583,14 +2109,30 @@
             ],
             "type": "structure"
         },
         "DeleteJobResponse": {
             "members": {},
             "type": "structure"
         },
+        "DeleteLaunchConfigurationTemplateRequest": {
+            "members": {
+                "launchConfigurationTemplateID": {
+                    "documentation": "<p>The ID of the Launch Configuration Template to be deleted.</p>",
+                    "shape": "LaunchConfigurationTemplateID"
+                }
+            },
+            "required": [
+                "launchConfigurationTemplateID"
+            ],
+            "type": "structure"
+        },
+        "DeleteLaunchConfigurationTemplateResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "DeleteRecoveryInstanceRequest": {
             "members": {
                 "recoveryInstanceID": {
                     "documentation": "<p>The ID of the Recovery Instance to be deleted.</p>",
                     "shape": "RecoveryInstanceID"
                 }
             },
@@ -1611,14 +2153,30 @@
             ],
             "type": "structure"
         },
         "DeleteReplicationConfigurationTemplateResponse": {
             "members": {},
             "type": "structure"
         },
+        "DeleteSourceNetworkRequest": {
+            "members": {
+                "sourceNetworkID": {
+                    "documentation": "<p>ID of the Source Network to delete.</p>",
+                    "shape": "SourceNetworkID"
+                }
+            },
+            "required": [
+                "sourceNetworkID"
+            ],
+            "type": "structure"
+        },
+        "DeleteSourceNetworkResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "DeleteSourceServerRequest": {
             "members": {
                 "sourceServerID": {
                     "documentation": "<p>The ID of the Source Server to be deleted.</p>",
                     "shape": "SourceServerID"
                 }
             },
@@ -1716,14 +2274,44 @@
                 "nextToken": {
                     "documentation": "<p>The token of the next Job to retrieve.</p>",
                     "shape": "PaginationToken"
                 }
             },
             "type": "structure"
         },
+        "DescribeLaunchConfigurationTemplatesRequest": {
+            "members": {
+                "launchConfigurationTemplateIDs": {
+                    "documentation": "<p>Request to filter Launch Configuration Templates list by Launch Configuration Template ID.</p>",
+                    "shape": "LaunchConfigurationTemplateIDs"
+                },
+                "maxResults": {
+                    "documentation": "<p>Maximum results to be returned in DescribeLaunchConfigurationTemplates.</p>",
+                    "shape": "MaxResultsType"
+                },
+                "nextToken": {
+                    "documentation": "<p>The token of the next Launch Configuration Template to retrieve.</p>",
+                    "shape": "PaginationToken"
+                }
+            },
+            "type": "structure"
+        },
+        "DescribeLaunchConfigurationTemplatesResponse": {
+            "members": {
+                "items": {
+                    "documentation": "<p>List of items returned by DescribeLaunchConfigurationTemplates.</p>",
+                    "shape": "LaunchConfigurationTemplates"
+                },
+                "nextToken": {
+                    "documentation": "<p>The token of the next Launch Configuration Template to retrieve.</p>",
+                    "shape": "PaginationToken"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeRecoveryInstancesItems": {
             "member": {
                 "shape": "RecoveryInstance"
             },
             "type": "list"
         },
         "DescribeRecoveryInstancesRequest": {
@@ -1851,14 +2439,70 @@
                 "nextToken": {
                     "documentation": "<p>The token of the next Replication Configuration Template to retrieve.</p>",
                     "shape": "PaginationToken"
                 }
             },
             "type": "structure"
         },
+        "DescribeSourceNetworksRequest": {
+            "members": {
+                "filters": {
+                    "documentation": "<p>A set of filters by which to return Source Networks.</p>",
+                    "shape": "DescribeSourceNetworksRequestFilters"
+                },
+                "maxResults": {
+                    "documentation": "<p>Maximum number of Source Networks to retrieve.</p>",
+                    "shape": "StrictlyPositiveInteger"
+                },
+                "nextToken": {
+                    "documentation": "<p>The token of the next Source Networks to retrieve.</p>",
+                    "shape": "PaginationToken"
+                }
+            },
+            "type": "structure"
+        },
+        "DescribeSourceNetworksRequestFilters": {
+            "documentation": "<p>A set of filters by which to return Source Networks.</p>",
+            "members": {
+                "originAccountID": {
+                    "documentation": "<p>Filter Source Networks by account ID containing the protected VPCs.</p>",
+                    "shape": "AccountID"
+                },
+                "originRegion": {
+                    "documentation": "<p>Filter Source Networks by the region containing the protected VPCs.</p>",
+                    "shape": "AwsRegion"
+                },
+                "sourceNetworkIDs": {
+                    "documentation": "<p>An array of Source Network IDs that should be returned. An empty array means all Source Networks.</p>",
+                    "shape": "DescribeSourceNetworksRequestFiltersIDs"
+                }
+            },
+            "type": "structure"
+        },
+        "DescribeSourceNetworksRequestFiltersIDs": {
+            "max": 100,
+            "member": {
+                "shape": "SourceNetworkID"
+            },
+            "min": 0,
+            "type": "list"
+        },
+        "DescribeSourceNetworksResponse": {
+            "members": {
+                "items": {
+                    "documentation": "<p>An array of Source Networks.</p>",
+                    "shape": "SourceNetworksList"
+                },
+                "nextToken": {
+                    "documentation": "<p>The token of the next Source Networks to retrieve.</p>",
+                    "shape": "PaginationToken"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeSourceServersRequest": {
             "members": {
                 "filters": {
                     "documentation": "<p>A set of filters by which to return Source Servers.</p>",
                     "shape": "DescribeSourceServersRequestFilters"
                 },
                 "maxResults": {
@@ -1976,26 +2620,62 @@
             "type": "string"
         },
         "EC2InstanceType": {
             "max": 255,
             "min": 0,
             "type": "string"
         },
+        "EbsSnapshot": {
+            "pattern": "^snap-[0-9a-zA-Z]{17}$",
+            "type": "string"
+        },
         "EbsSnapshotsList": {
             "member": {
-                "shape": "ebsSnapshot"
+                "shape": "EbsSnapshot"
             },
             "type": "list"
         },
         "EbsVolumeID": {
             "max": 19,
             "min": 10,
             "pattern": "^vol-([0-9a-fA-F]{8}|[0-9a-fA-F]{17})$",
             "type": "string"
         },
+        "EventResourceData": {
+            "documentation": "<p>Properties of resource related to a job event.</p>",
+            "members": {
+                "sourceNetworkData": {
+                    "documentation": "<p>Source Network properties.</p>",
+                    "shape": "SourceNetworkData"
+                }
+            },
+            "type": "structure",
+            "union": true
+        },
+        "ExportSourceNetworkCfnTemplateRequest": {
+            "members": {
+                "sourceNetworkID": {
+                    "documentation": "<p>The Source Network ID to export its CloudFormation template to an S3 bucket.</p>",
+                    "shape": "SourceNetworkID"
+                }
+            },
+            "required": [
+                "sourceNetworkID"
+            ],
+            "type": "structure"
+        },
+        "ExportSourceNetworkCfnTemplateResponse": {
+            "members": {
+                "s3DestinationUrl": {
+                    "documentation": "<p>S3 bucket URL where the Source Network CloudFormation template was exported to.</p>",
+                    "shape": "LargeBoundedString"
+                }
+            },
+            "type": "structure"
+        },
         "ExtensionStatus": {
             "enum": [
                 "EXTENDED",
                 "EXTENSION_ERROR",
                 "NOT_EXTENDED"
             ],
             "type": "string"
@@ -2155,15 +2835,18 @@
         "InitiatedBy": {
             "enum": [
                 "START_RECOVERY",
                 "START_DRILL",
                 "FAILBACK",
                 "DIAGNOSTIC",
                 "TERMINATE_RECOVERY_INSTANCES",
-                "TARGET_ACCOUNT"
+                "TARGET_ACCOUNT",
+                "CREATE_NETWORK_RECOVERY",
+                "UPDATE_NETWORK_RECOVERY",
+                "ASSOCIATE_NETWORK_RECOVERY"
             ],
             "type": "string"
         },
         "InternalServerException": {
             "documentation": "<p>The request processing has failed because of an unknown error, exception or failure.</p>",
             "error": {
                 "httpStatusCode": 500
@@ -2205,14 +2888,18 @@
                     "documentation": "<p>A string representing who initiated the Job.</p>",
                     "shape": "InitiatedBy"
                 },
                 "jobID": {
                     "documentation": "<p>The ID of the Job.</p>",
                     "shape": "JobID"
                 },
+                "participatingResources": {
+                    "documentation": "<p>A list of resources that the Job is acting upon.</p>",
+                    "shape": "ParticipatingResources"
+                },
                 "participatingServers": {
                     "documentation": "<p>A list of servers that the Job is acting upon.</p>",
                     "shape": "ParticipatingServers"
                 },
                 "status": {
                     "documentation": "<p>The status of the Job.</p>",
                     "shape": "JobStatus"
@@ -2269,29 +2956,43 @@
                 "USING_PREVIOUS_SNAPSHOT_FAILED",
                 "CONVERSION_START",
                 "CONVERSION_END",
                 "CONVERSION_FAIL",
                 "LAUNCH_START",
                 "LAUNCH_FAILED",
                 "JOB_CANCEL",
-                "JOB_END"
+                "JOB_END",
+                "DEPLOY_NETWORK_CONFIGURATION_START",
+                "DEPLOY_NETWORK_CONFIGURATION_END",
+                "DEPLOY_NETWORK_CONFIGURATION_FAILED",
+                "UPDATE_NETWORK_CONFIGURATION_START",
+                "UPDATE_NETWORK_CONFIGURATION_END",
+                "UPDATE_NETWORK_CONFIGURATION_FAILED",
+                "UPDATE_LAUNCH_TEMPLATE_START",
+                "UPDATE_LAUNCH_TEMPLATE_END",
+                "UPDATE_LAUNCH_TEMPLATE_FAILED",
+                "NETWORK_RECOVERY_FAIL"
             ],
             "type": "string"
         },
         "JobLogEventData": {
             "documentation": "<p>Metadata associated with a Job log.</p>",
             "members": {
                 "conversionProperties": {
                     "documentation": "<p>Properties of a conversion job</p>",
                     "shape": "ConversionProperties"
                 },
                 "conversionServerID": {
                     "documentation": "<p>The ID of a conversion server.</p>",
                     "shape": "EC2InstanceID"
                 },
+                "eventResourceData": {
+                    "documentation": "<p>Properties of resource related to a job event.</p>",
+                    "shape": "EventResourceData"
+                },
                 "rawError": {
                     "documentation": "<p>A string representing a job error.</p>",
                     "shape": "LargeBoundedString"
                 },
                 "sourceServerID": {
                     "documentation": "<p>The ID of a Source Server.</p>",
                     "shape": "SourceServerID"
@@ -2385,14 +3086,78 @@
                 "targetInstanceTypeRightSizingMethod": {
                     "documentation": "<p>Whether Elastic Disaster Recovery should try to automatically choose the instance type that best matches the OS, CPU, and RAM of your Source Server.</p>",
                     "shape": "TargetInstanceTypeRightSizingMethod"
                 }
             },
             "type": "structure"
         },
+        "LaunchConfigurationTemplate": {
+            "documentation": "<p>Account level Launch Configuration Template.</p>",
+            "members": {
+                "arn": {
+                    "documentation": "<p>ARN of the Launch Configuration Template.</p>",
+                    "shape": "ARN"
+                },
+                "copyPrivateIp": {
+                    "documentation": "<p>Copy private IP.</p>",
+                    "shape": "Boolean"
+                },
+                "copyTags": {
+                    "documentation": "<p>Copy tags.</p>",
+                    "shape": "Boolean"
+                },
+                "exportBucketArn": {
+                    "documentation": "<p>S3 bucket ARN to export Source Network templates.</p>",
+                    "shape": "ARN"
+                },
+                "launchConfigurationTemplateID": {
+                    "documentation": "<p>ID of the Launch Configuration Template.</p>",
+                    "shape": "LaunchConfigurationTemplateID"
+                },
+                "launchDisposition": {
+                    "documentation": "<p>Launch disposition.</p>",
+                    "shape": "LaunchDisposition"
+                },
+                "licensing": {
+                    "documentation": "<p>Licensing.</p>",
+                    "shape": "Licensing"
+                },
+                "tags": {
+                    "documentation": "<p>Tags of the Launch Configuration Template.</p>",
+                    "shape": "TagsMap"
+                },
+                "targetInstanceTypeRightSizingMethod": {
+                    "documentation": "<p>Target instance type right-sizing method.</p>",
+                    "shape": "TargetInstanceTypeRightSizingMethod"
+                }
+            },
+            "type": "structure"
+        },
+        "LaunchConfigurationTemplateID": {
+            "max": 21,
+            "min": 21,
+            "pattern": "^lct-[0-9a-zA-Z]{17}$",
+            "type": "string"
+        },
+        "LaunchConfigurationTemplateIDs": {
+            "max": 1,
+            "member": {
+                "shape": "LaunchConfigurationTemplateID"
+            },
+            "min": 0,
+            "type": "list"
+        },
+        "LaunchConfigurationTemplates": {
+            "max": 200,
+            "member": {
+                "shape": "LaunchConfigurationTemplate"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "LaunchDisposition": {
             "enum": [
                 "STOPPED",
                 "STARTED"
             ],
             "type": "string"
         },
@@ -2567,14 +3332,19 @@
             "type": "structure"
         },
         "MaxResultsReplicatingSourceServers": {
             "max": 300,
             "min": 1,
             "type": "integer"
         },
+        "MaxResultsType": {
+            "max": 1000,
+            "min": 1,
+            "type": "integer"
+        },
         "NetworkInterface": {
             "documentation": "<p>Network interface.</p>",
             "members": {
                 "ips": {
                     "documentation": "<p>Network interface IPs.</p>",
                     "shape": "IPsList"
                 },
@@ -2662,14 +3432,45 @@
             "type": "string"
         },
         "PaginationToken": {
             "max": 2048,
             "min": 0,
             "type": "string"
         },
+        "ParticipatingResource": {
+            "documentation": "<p>Represents a resource participating in an asynchronous Job.</p>",
+            "members": {
+                "launchStatus": {
+                    "documentation": "<p>The launch status of a participating resource.</p>",
+                    "shape": "LaunchStatus"
+                },
+                "participatingResourceID": {
+                    "documentation": "<p>The ID of a participating resource.</p>",
+                    "shape": "ParticipatingResourceID"
+                }
+            },
+            "type": "structure"
+        },
+        "ParticipatingResourceID": {
+            "documentation": "<p>ID of a resource participating in an asynchronous Job.</p>",
+            "members": {
+                "sourceNetworkID": {
+                    "documentation": "<p>Source Network ID.</p>",
+                    "shape": "SourceNetworkID"
+                }
+            },
+            "type": "structure",
+            "union": true
+        },
+        "ParticipatingResources": {
+            "member": {
+                "shape": "ParticipatingResource"
+            },
+            "type": "list"
+        },
         "ParticipatingServer": {
             "documentation": "<p>Represents a server participating in an asynchronous Job.</p>",
             "members": {
                 "launchStatus": {
                     "documentation": "<p>The launch status of a participating server.</p>",
                     "shape": "LaunchStatus"
                 },
@@ -3046,14 +3847,44 @@
             "max": 200,
             "member": {
                 "shape": "RecoveryInstanceID"
             },
             "min": 1,
             "type": "list"
         },
+        "RecoveryLifeCycle": {
+            "documentation": "<p>An object representing the Source Network recovery Lifecycle.</p>",
+            "members": {
+                "apiCallDateTime": {
+                    "documentation": "<p>The date and time the last Source Network recovery was initiated.</p>",
+                    "shape": "SyntheticTimestamp_date_time"
+                },
+                "jobID": {
+                    "documentation": "<p>The ID of the Job that was used to last recover the Source Network.</p>",
+                    "shape": "JobID"
+                },
+                "lastRecoveryResult": {
+                    "documentation": "<p>The status of the last recovery status of this Source Network.</p>",
+                    "shape": "RecoveryResult"
+                }
+            },
+            "type": "structure"
+        },
+        "RecoveryResult": {
+            "enum": [
+                "NOT_STARTED",
+                "IN_PROGRESS",
+                "SUCCESS",
+                "FAIL",
+                "PARTIAL_SUCCESS",
+                "ASSOCIATE_SUCCESS",
+                "ASSOCIATE_FAIL"
+            ],
+            "type": "string"
+        },
         "RecoverySnapshot": {
             "documentation": "<p>A snapshot of a Source Server used during recovery.</p>",
             "members": {
                 "ebsSnapshots": {
                     "documentation": "<p>A list of EBS snapshots.</p>",
                     "shape": "EbsSnapshotsList"
                 },
@@ -3102,14 +3933,18 @@
         },
         "ReplicationConfiguration": {
             "members": {
                 "associateDefaultSecurityGroup": {
                     "documentation": "<p>Whether to associate the default Elastic Disaster Recovery Security group with the Replication Configuration.</p>",
                     "shape": "Boolean"
                 },
+                "autoReplicateNewDisks": {
+                    "documentation": "<p>Whether to allow the AWS replication agent to automatically replicate newly added disks.</p>",
+                    "shape": "Boolean"
+                },
                 "bandwidthThrottling": {
                     "documentation": "<p>Configure bandwidth throttling for the outbound data transfer rate of the Source Server in Mbps.</p>",
                     "shape": "PositiveInteger"
                 },
                 "createPublicIP": {
                     "documentation": "<p>Whether to create a Public IP for the Recovery Instance by default.</p>",
                     "shape": "Boolean"
@@ -3184,15 +4019,16 @@
                 "AUTO"
             ],
             "type": "string"
         },
         "ReplicationConfigurationEbsEncryption": {
             "enum": [
                 "DEFAULT",
-                "CUSTOM"
+                "CUSTOM",
+                "NONE"
             ],
             "type": "string"
         },
         "ReplicationConfigurationReplicatedDisk": {
             "documentation": "<p>The configuration of a disk of the Source Server to be replicated.</p>",
             "members": {
                 "deviceName": {
@@ -3248,14 +4084,18 @@
                     "documentation": "<p>The Replication Configuration Template ARN.</p>",
                     "shape": "ARN"
                 },
                 "associateDefaultSecurityGroup": {
                     "documentation": "<p>Whether to associate the default Elastic Disaster Recovery Security group with the Replication Configuration Template.</p>",
                     "shape": "Boolean"
                 },
+                "autoReplicateNewDisks": {
+                    "documentation": "<p>Whether to allow the AWS replication agent to automatically replicate newly added disks.</p>",
+                    "shape": "Boolean"
+                },
                 "bandwidthThrottling": {
                     "documentation": "<p>Configure bandwidth throttling for the outbound data transfer rate of the Source Server in Mbps.</p>",
                     "shape": "PositiveInteger"
                 },
                 "createPublicIP": {
                     "documentation": "<p>Whether to create a Public IP for the Recovery Instance by default.</p>",
                     "shape": "Boolean"
@@ -3346,14 +4186,23 @@
             "max": 32,
             "member": {
                 "shape": "SecurityGroupID"
             },
             "min": 0,
             "type": "list"
         },
+        "ReplicationStatus": {
+            "enum": [
+                "STOPPED",
+                "IN_PROGRESS",
+                "PROTECTED",
+                "ERROR"
+            ],
+            "type": "string"
+        },
         "ResourceNotFoundException": {
             "documentation": "<p>The resource for this operation was not found.</p>",
             "error": {
                 "httpStatusCode": 404,
                 "senderFault": true
             },
             "exception": true,
@@ -3372,14 +4221,16 @@
                     "documentation": "<p>The type of the resource.</p>",
                     "shape": "LargeBoundedString"
                 }
             },
             "type": "structure"
         },
         "RetryDataReplicationRequest": {
+            "deprecated": true,
+            "deprecatedMessage": "WARNING: RetryDataReplication is deprecated",
             "members": {
                 "sourceServerID": {
                     "documentation": "<p>The ID of the Source Server whose data replication should be retried.</p>",
                     "shape": "SourceServerID"
                 }
             },
             "required": [
@@ -3410,14 +4261,20 @@
         },
         "SecurityGroupID": {
             "max": 255,
             "min": 0,
             "pattern": "^sg-[0-9a-fA-F]{8,}$",
             "type": "string"
         },
+        "SensitiveBoundedString": {
+            "max": 256,
+            "min": 0,
+            "sensitive": true,
+            "type": "string"
+        },
         "ServiceQuotaExceededException": {
             "documentation": "<p>The request could not be completed because its exceeded the service quota.</p>",
             "error": {
                 "httpStatusCode": 402,
                 "senderFault": true
             },
             "exception": true,
@@ -3466,14 +4323,98 @@
                 "originRegion": {
                     "documentation": "<p>AWS Region for an EC2-originated Source Server.</p>",
                     "shape": "AwsRegion"
                 }
             },
             "type": "structure"
         },
+        "SourceNetwork": {
+            "documentation": "<p>The ARN of the Source Network.</p>",
+            "members": {
+                "arn": {
+                    "documentation": "<p>The ARN of the Source Network.</p>",
+                    "shape": "ARN"
+                },
+                "cfnStackName": {
+                    "documentation": "<p>CloudFormation stack name that was deployed for recovering the Source Network.</p>",
+                    "shape": "CfnStackName"
+                },
+                "lastRecovery": {
+                    "documentation": "<p>An object containing information regarding the last recovery of the Source Network.</p>",
+                    "shape": "RecoveryLifeCycle"
+                },
+                "launchedVpcID": {
+                    "documentation": "<p>ID of the recovered VPC following Source Network recovery.</p>",
+                    "shape": "VpcID"
+                },
+                "replicationStatus": {
+                    "documentation": "<p>Status of Source Network Replication. Possible values: (a) STOPPED - Source Network is not replicating. (b) IN_PROGRESS - Source Network is being replicated. (c) PROTECTED - Source Network was replicated successfully and is being synchronized for changes. (d) ERROR - Source Network replication has failed</p>",
+                    "shape": "ReplicationStatus"
+                },
+                "replicationStatusDetails": {
+                    "documentation": "<p>Error details in case Source Network replication status is ERROR.</p>",
+                    "shape": "SensitiveBoundedString"
+                },
+                "sourceAccountID": {
+                    "documentation": "<p>Account ID containing the VPC protected by the Source Network.</p>",
+                    "shape": "AccountID"
+                },
+                "sourceNetworkID": {
+                    "documentation": "<p>Source Network ID.</p>",
+                    "shape": "SourceNetworkID"
+                },
+                "sourceRegion": {
+                    "documentation": "<p>Region containing the VPC protected by the Source Network.</p>",
+                    "shape": "AwsRegion"
+                },
+                "sourceVpcID": {
+                    "documentation": "<p>VPC ID protected by the Source Network.</p>",
+                    "shape": "VpcID"
+                },
+                "tags": {
+                    "documentation": "<p>A list of tags associated with the Source Network.</p>",
+                    "shape": "TagsMap"
+                }
+            },
+            "type": "structure"
+        },
+        "SourceNetworkData": {
+            "documentation": "<p>Properties of Source Network related to a job event.</p>",
+            "members": {
+                "sourceNetworkID": {
+                    "documentation": "<p>Source Network ID.</p>",
+                    "shape": "SourceNetworkID"
+                },
+                "sourceVpc": {
+                    "documentation": "<p>VPC ID protected by the Source Network.</p>",
+                    "shape": "VpcID"
+                },
+                "stackName": {
+                    "documentation": "<p>CloudFormation stack name that was deployed for recovering the Source Network.</p>",
+                    "shape": "LargeBoundedString"
+                },
+                "targetVpc": {
+                    "documentation": "<p>ID of the recovered VPC following Source Network recovery.</p>",
+                    "shape": "VpcID"
+                }
+            },
+            "type": "structure"
+        },
+        "SourceNetworkID": {
+            "max": 20,
+            "min": 20,
+            "pattern": "^sn-[0-9a-zA-Z]{17}$",
+            "type": "string"
+        },
+        "SourceNetworksList": {
+            "member": {
+                "shape": "SourceNetwork"
+            },
+            "type": "list"
+        },
         "SourceProperties": {
             "documentation": "<p>Properties of the Source Server machine.</p>",
             "members": {
                 "cpus": {
                     "documentation": "<p>An array of CPUs.</p>",
                     "shape": "Cpus"
                 },
@@ -3500,14 +4441,18 @@
                 "ramBytes": {
                     "documentation": "<p>The amount of RAM in bytes.</p>",
                     "shape": "PositiveInteger"
                 },
                 "recommendedInstanceType": {
                     "documentation": "<p>The recommended EC2 instance type that will be used when recovering the Source Server.</p>",
                     "shape": "EC2InstanceType"
+                },
+                "supportsNitroInstances": {
+                    "documentation": "<p>Are EC2 nitro instance types supported when recovering the Source Server.</p>",
+                    "shape": "Boolean"
                 }
             },
             "type": "structure"
         },
         "SourceServer": {
             "members": {
                 "arn": {
@@ -3538,14 +4483,18 @@
                     "documentation": "<p>For EC2-originated Source Servers which have been failed over and then failed back, this value will mean the ARN of the Source Server on the opposite replication direction.</p>",
                     "shape": "SourceServerARN"
                 },
                 "sourceCloudProperties": {
                     "documentation": "<p>Source cloud properties of the Source Server.</p>",
                     "shape": "SourceCloudProperties"
                 },
+                "sourceNetworkID": {
+                    "documentation": "<p>ID of the Source Network which is protecting this Source Server's network.</p>",
+                    "shape": "SourceNetworkID"
+                },
                 "sourceProperties": {
                     "documentation": "<p>The source properties of the Source Server.</p>",
                     "shape": "SourceProperties"
                 },
                 "sourceServerID": {
                     "documentation": "<p>The ID of the Source Server.</p>",
                     "shape": "SourceServerID"
@@ -3735,14 +4684,89 @@
                 "sourceServer": {
                     "documentation": "<p>The Source Server that this action was targeted on.</p>",
                     "shape": "SourceServer"
                 }
             },
             "type": "structure"
         },
+        "StartSourceNetworkRecoveryRequest": {
+            "members": {
+                "deployAsNew": {
+                    "documentation": "<p>Don't update existing CloudFormation Stack, recover the network using a new stack.</p>",
+                    "shape": "Boolean"
+                },
+                "sourceNetworks": {
+                    "documentation": "<p>The Source Networks that we want to start a Recovery Job for.</p>",
+                    "shape": "StartSourceNetworkRecoveryRequestNetworkEntries"
+                },
+                "tags": {
+                    "documentation": "<p>The tags to be associated with the Source Network recovery Job.</p>",
+                    "shape": "TagsMap"
+                }
+            },
+            "required": [
+                "sourceNetworks"
+            ],
+            "type": "structure"
+        },
+        "StartSourceNetworkRecoveryRequestNetworkEntries": {
+            "max": 100,
+            "member": {
+                "shape": "StartSourceNetworkRecoveryRequestNetworkEntry"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "StartSourceNetworkRecoveryRequestNetworkEntry": {
+            "documentation": "<p>An object representing the Source Network to recover.</p>",
+            "members": {
+                "cfnStackName": {
+                    "documentation": "<p>CloudFormation stack name to be used for recovering the network.</p>",
+                    "shape": "CfnStackName"
+                },
+                "sourceNetworkID": {
+                    "documentation": "<p>The ID of the Source Network you want to recover.</p>",
+                    "shape": "SourceNetworkID"
+                }
+            },
+            "required": [
+                "sourceNetworkID"
+            ],
+            "type": "structure"
+        },
+        "StartSourceNetworkRecoveryResponse": {
+            "members": {
+                "job": {
+                    "documentation": "<p>The Source Network recovery Job.</p>",
+                    "shape": "Job"
+                }
+            },
+            "type": "structure"
+        },
+        "StartSourceNetworkReplicationRequest": {
+            "members": {
+                "sourceNetworkID": {
+                    "documentation": "<p>ID of the Source Network to replicate.</p>",
+                    "shape": "SourceNetworkID"
+                }
+            },
+            "required": [
+                "sourceNetworkID"
+            ],
+            "type": "structure"
+        },
+        "StartSourceNetworkReplicationResponse": {
+            "members": {
+                "sourceNetwork": {
+                    "documentation": "<p>Source Network which was requested for replication.</p>",
+                    "shape": "SourceNetwork"
+                }
+            },
+            "type": "structure"
+        },
         "StopFailbackRequest": {
             "members": {
                 "recoveryInstanceID": {
                     "documentation": "<p>The ID of the Recovery Instance we want to stop failback for.</p>",
                     "shape": "RecoveryInstanceID"
                 }
             },
@@ -3768,24 +4792,49 @@
                 "sourceServer": {
                     "documentation": "<p>The Source Server that this action was targeted on.</p>",
                     "shape": "SourceServer"
                 }
             },
             "type": "structure"
         },
+        "StopSourceNetworkReplicationRequest": {
+            "members": {
+                "sourceNetworkID": {
+                    "documentation": "<p>ID of the Source Network to stop replication.</p>",
+                    "shape": "SourceNetworkID"
+                }
+            },
+            "required": [
+                "sourceNetworkID"
+            ],
+            "type": "structure"
+        },
+        "StopSourceNetworkReplicationResponse": {
+            "members": {
+                "sourceNetwork": {
+                    "documentation": "<p>Source Network which was requested to stop replication.</p>",
+                    "shape": "SourceNetwork"
+                }
+            },
+            "type": "structure"
+        },
         "StrictlyPositiveInteger": {
             "min": 1,
             "type": "integer"
         },
         "SubnetID": {
             "max": 255,
             "min": 0,
             "pattern": "^subnet-[0-9a-fA-F]{8,}$",
             "type": "string"
         },
+        "SyntheticTimestamp_date_time": {
+            "timestampFormat": "iso8601",
+            "type": "timestamp"
+        },
         "TagKey": {
             "max": 256,
             "min": 0,
             "type": "string"
         },
         "TagKeys": {
             "member": {
@@ -3981,20 +5030,69 @@
                 }
             },
             "required": [
                 "sourceServerID"
             ],
             "type": "structure"
         },
+        "UpdateLaunchConfigurationTemplateRequest": {
+            "members": {
+                "copyPrivateIp": {
+                    "documentation": "<p>Copy private IP.</p>",
+                    "shape": "Boolean"
+                },
+                "copyTags": {
+                    "documentation": "<p>Copy tags.</p>",
+                    "shape": "Boolean"
+                },
+                "exportBucketArn": {
+                    "documentation": "<p>S3 bucket ARN to export Source Network templates.</p>",
+                    "shape": "ARN"
+                },
+                "launchConfigurationTemplateID": {
+                    "documentation": "<p>Launch Configuration Template ID.</p>",
+                    "shape": "LaunchConfigurationTemplateID"
+                },
+                "launchDisposition": {
+                    "documentation": "<p>Launch disposition.</p>",
+                    "shape": "LaunchDisposition"
+                },
+                "licensing": {
+                    "documentation": "<p>Licensing.</p>",
+                    "shape": "Licensing"
+                },
+                "targetInstanceTypeRightSizingMethod": {
+                    "documentation": "<p>Target instance type right-sizing method.</p>",
+                    "shape": "TargetInstanceTypeRightSizingMethod"
+                }
+            },
+            "required": [
+                "launchConfigurationTemplateID"
+            ],
+            "type": "structure"
+        },
+        "UpdateLaunchConfigurationTemplateResponse": {
+            "members": {
+                "launchConfigurationTemplate": {
+                    "documentation": "<p>Updated Launch Configuration Template.</p>",
+                    "shape": "LaunchConfigurationTemplate"
+                }
+            },
+            "type": "structure"
+        },
         "UpdateReplicationConfigurationRequest": {
             "members": {
                 "associateDefaultSecurityGroup": {
                     "documentation": "<p>Whether to associate the default Elastic Disaster Recovery Security group with the Replication Configuration.</p>",
                     "shape": "Boolean"
                 },
+                "autoReplicateNewDisks": {
+                    "documentation": "<p>Whether to allow the AWS replication agent to automatically replicate newly added disks.</p>",
+                    "shape": "Boolean"
+                },
                 "bandwidthThrottling": {
                     "documentation": "<p>Configure bandwidth throttling for the outbound data transfer rate of the Source Server in Mbps.</p>",
                     "shape": "PositiveInteger"
                 },
                 "createPublicIP": {
                     "documentation": "<p>Whether to create a Public IP for the Recovery Instance by default.</p>",
                     "shape": "Boolean"
@@ -4063,14 +5161,18 @@
                     "documentation": "<p>The Replication Configuration Template ARN.</p>",
                     "shape": "ARN"
                 },
                 "associateDefaultSecurityGroup": {
                     "documentation": "<p>Whether to associate the default Elastic Disaster Recovery Security group with the Replication Configuration Template.</p>",
                     "shape": "Boolean"
                 },
+                "autoReplicateNewDisks": {
+                    "documentation": "<p>Whether to allow the AWS replication agent to automatically replicate newly added disks.</p>",
+                    "shape": "Boolean"
+                },
                 "bandwidthThrottling": {
                     "documentation": "<p>Configure bandwidth throttling for the outbound data transfer rate of the Source Server in Mbps.</p>",
                     "shape": "PositiveInteger"
                 },
                 "createPublicIP": {
                     "documentation": "<p>Whether to create a Public IP for the Recovery Instance by default.</p>",
                     "shape": "Boolean"
@@ -4193,14 +5295,16 @@
                 "shape": "LargeBoundedString"
             },
             "type": "map",
             "value": {
                 "shape": "PositiveInteger"
             }
         },
-        "ebsSnapshot": {
-            "pattern": "^snap-[0-9a-zA-Z]{17}$",
+        "VpcID": {
+            "max": 21,
+            "min": 12,
+            "pattern": "^vpc-[0-9a-fA-F]{8,}$",
             "type": "string"
         }
     },
     "version": "2.0"
 }
```

### Comparing `botocore-a-la-carte-drs-1.29.99/botocore_a_la_carte_drs.egg-info/PKG-INFO` & `botocore-a-la-carte-drs-1.30.0/botocore_a_la_carte_drs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-drs
-Version: 1.29.99
+Version: 1.30.0
 Summary: drs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-drs-1.29.99/setup.py` & `botocore-a-la-carte-drs-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-drs',
-    version="1.29.99",
+    version="1.30.0",
     description='drs data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/drs/*/*.json'],
```

