# Comparing `tmp/botocore-a-la-carte-appflow-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-appflow-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-appflow-1.29.99.tar", last modified: Sat Mar 25 01:22:22 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-appflow-1.30.0.tar", last modified: Tue Jul  4 01:44:13 2023, max compression
```

## Comparing `botocore-a-la-carte-appflow-1.29.99.tar` & `botocore-a-la-carte-appflow-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:22.638394 botocore-a-la-carte-appflow-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:22.000000 botocore-a-la-carte-appflow-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-25 01:22:22.638394 botocore-a-la-carte-appflow-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:22.638394 botocore-a-la-carte-appflow-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:22.638394 botocore-a-la-carte-appflow-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:22.638394 botocore-a-la-carte-appflow-1.29.99/botocore/data/appflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:22.638394 botocore-a-la-carte-appflow-1.29.99/botocore/data/appflow/2020-08-23/
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-03-25 01:22:12.000000 botocore-a-la-carte-appflow-1.29.99/botocore/data/appflow/2020-08-23/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-appflow-1.29.99/botocore/data/appflow/2020-08-23/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-25 01:22:12.000000 botocore-a-la-carte-appflow-1.29.99/botocore/data/appflow/2020-08-23/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   212422 2023-03-25 01:22:12.000000 botocore-a-la-carte-appflow-1.29.99/botocore/data/appflow/2020-08-23/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:22.638394 botocore-a-la-carte-appflow-1.29.99/botocore_a_la_carte_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-25 01:22:22.000000 botocore-a-la-carte-appflow-1.29.99/botocore_a_la_carte_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-25 01:22:22.000000 botocore-a-la-carte-appflow-1.29.99/botocore_a_la_carte_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:22.000000 botocore-a-la-carte-appflow-1.29.99/botocore_a_la_carte_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:22.000000 botocore-a-la-carte-appflow-1.29.99/botocore_a_la_carte_appflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:22.638394 botocore-a-la-carte-appflow-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-25 01:22:22.000000 botocore-a-la-carte-appflow-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:13.158377 botocore-a-la-carte-appflow-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:12.000000 botocore-a-la-carte-appflow-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-04 01:44:13.154377 botocore-a-la-carte-appflow-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:13.154377 botocore-a-la-carte-appflow-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:13.154377 botocore-a-la-carte-appflow-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:13.154377 botocore-a-la-carte-appflow-1.30.0/botocore/data/appflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:13.154377 botocore-a-la-carte-appflow-1.30.0/botocore/data/appflow/2020-08-23/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-04 01:44:02.000000 botocore-a-la-carte-appflow-1.30.0/botocore/data/appflow/2020-08-23/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-appflow-1.30.0/botocore/data/appflow/2020-08-23/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-appflow-1.30.0/botocore/data/appflow/2020-08-23/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233245 2023-07-04 01:44:02.000000 botocore-a-la-carte-appflow-1.30.0/botocore/data/appflow/2020-08-23/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:13.154377 botocore-a-la-carte-appflow-1.30.0/botocore_a_la_carte_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-04 01:44:13.000000 botocore-a-la-carte-appflow-1.30.0/botocore_a_la_carte_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 01:44:13.000000 botocore-a-la-carte-appflow-1.30.0/botocore_a_la_carte_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:13.000000 botocore-a-la-carte-appflow-1.30.0/botocore_a_la_carte_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:13.000000 botocore-a-la-carte-appflow-1.30.0/botocore_a_la_carte_appflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:13.158377 botocore-a-la-carte-appflow-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 01:44:12.000000 botocore-a-la-carte-appflow-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-appflow-1.29.99/LICENSE.txt` & `botocore-a-la-carte-appflow-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appflow-1.29.99/PKG-INFO` & `botocore-a-la-carte-appflow-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-appflow
-Version: 1.29.99
+Version: 1.30.0
 Summary: appflow data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-appflow-1.29.99/botocore/data/appflow/2020-08-23/endpoint-rule-set-1.json` & `botocore-a-la-carte-appflow-1.30.0/botocore/data/appflow/2020-08-23/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appflow-1.29.99/botocore/data/appflow/2020-08-23/service-2.json` & `botocore-a-la-carte-appflow-1.30.0/botocore/data/appflow/2020-08-23/service-2.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.988716686218283%*

 * *Differences: {"'operations'": "{'CancelFlowExecutions': OrderedDict([('name', 'CancelFlowExecutions'), ('http', "*

 * *                 "OrderedDict([('method', 'POST'), ('requestUri', '/cancel-flow-executions')])), "*

 * *                 "('input', OrderedDict([('shape', 'CancelFlowExecutionsRequest')])), ('output', "*

 * *                 "OrderedDict([('shape', 'CancelFlowExecutionsResponse')])), ('errors', "*

 * *                 "[OrderedDict([('shape', 'ValidationException')]), OrderedDict([('shape', "*

 * *                 "'AccessDenie […]*

```diff
@@ -8,14 +8,45 @@
         "serviceFullName": "Amazon Appflow",
         "serviceId": "Appflow",
         "signatureVersion": "v4",
         "signingName": "appflow",
         "uid": "appflow-2020-08-23"
     },
     "operations": {
+        "CancelFlowExecutions": {
+            "documentation": "<p>Cancels active runs for a flow.</p> <p>You can cancel all of the active runs for a flow, or you can cancel specific runs by providing their IDs.</p> <p>You can cancel a flow run only when the run is in progress. You can't cancel a run that has already completed or failed. You also can't cancel a run that's scheduled to occur but hasn't started yet. To prevent a scheduled run, you can deactivate the flow with the <code>StopFlow</code> action.</p> <p>You cannot resume a run after you cancel it.</p> <p>When you send your request, the status for each run becomes <code>CancelStarted</code>. When the cancellation completes, the status becomes <code>Canceled</code>.</p> <note> <p>When you cancel a run, you still incur charges for any data that the run already processed before the cancellation. If the run had already written some data to the flow destination, then that data remains in the destination. If you configured the flow to use a batch API (such as the Salesforce Bulk API 2.0), then the run will finish reading or writing its entire batch of data after the cancellation. For these operations, the data processing charges for Amazon AppFlow apply. For the pricing information, see <a href=\"http://aws.amazon.com/appflow/pricing/\">Amazon AppFlow pricing</a>.</p> </note>",
+            "errors": [
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/cancel-flow-executions"
+            },
+            "input": {
+                "shape": "CancelFlowExecutionsRequest"
+            },
+            "name": "CancelFlowExecutions",
+            "output": {
+                "shape": "CancelFlowExecutionsResponse"
+            }
+        },
         "CreateConnectorProfile": {
             "documentation": "<p> Creates a new connector profile associated with your Amazon Web Services account. There is a soft quota of 100 connector profiles per Amazon Web Services account. If you need more connector profiles than this quota allows, you can submit a request to the Amazon AppFlow team through the Amazon AppFlow support channel. In each connector profile that you create, you can provide the credentials and properties for only one connector.</p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
@@ -416,14 +447,42 @@
                 "shape": "RegisterConnectorRequest"
             },
             "name": "RegisterConnector",
             "output": {
                 "shape": "RegisterConnectorResponse"
             }
         },
+        "ResetConnectorMetadataCache": {
+            "documentation": "<p>Resets metadata about your connector entities that Amazon AppFlow stored in its cache. Use this action when you want Amazon AppFlow to return the latest information about the data that you have in a source application.</p> <p>Amazon AppFlow returns metadata about your entities when you use the ListConnectorEntities or DescribeConnectorEntities actions. Following these actions, Amazon AppFlow caches the metadata to reduce the number of API requests that it must send to the source application. Amazon AppFlow automatically resets the cache once every hour, but you can use this action when you want to get the latest metadata right away.</p>",
+            "errors": [
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/reset-connector-metadata-cache"
+            },
+            "input": {
+                "shape": "ResetConnectorMetadataCacheRequest"
+            },
+            "name": "ResetConnectorMetadataCache",
+            "output": {
+                "shape": "ResetConnectorMetadataCacheResponse"
+            }
+        },
         "StartFlow": {
             "documentation": "<p> Activates an existing flow. For on-demand flows, this operation runs the flow immediately. For schedule and event-triggered flows, this operation activates the flow. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -823,15 +882,15 @@
         },
         "ApplicationType": {
             "max": 512,
             "pattern": "\\S+",
             "type": "string"
         },
         "AuthCode": {
-            "max": 2048,
+            "max": 4096,
             "pattern": "\\S+",
             "type": "string"
         },
         "AuthCodeUrl": {
             "max": 256,
             "pattern": "^(https?)://[-a-zA-Z0-9+&@#/%?=~_|!:,.;]*[-a-zA-Z0-9+&@#/%=~_|]",
             "type": "string"
@@ -950,14 +1009,39 @@
             "type": "string"
         },
         "BusinessUnitId": {
             "max": 18,
             "pattern": "\\S+",
             "type": "string"
         },
+        "CancelFlowExecutionsRequest": {
+            "members": {
+                "executionIds": {
+                    "documentation": "<p>The ID of each active run to cancel. These runs must belong to the flow you specify in your request.</p> <p>If you omit this parameter, your request ends all active runs that belong to the flow.</p>",
+                    "shape": "ExecutionIds"
+                },
+                "flowName": {
+                    "documentation": "<p>The name of a flow with active runs that you want to cancel.</p>",
+                    "shape": "FlowName"
+                }
+            },
+            "required": [
+                "flowName"
+            ],
+            "type": "structure"
+        },
+        "CancelFlowExecutionsResponse": {
+            "members": {
+                "invalidExecutions": {
+                    "documentation": "<p>The IDs of runs that Amazon AppFlow couldn't cancel. These runs might be ineligible for canceling because they haven't started yet or have already completed.</p>",
+                    "shape": "ExecutionIds"
+                }
+            },
+            "type": "structure"
+        },
         "CatalogType": {
             "enum": [
                 "GLUE"
             ],
             "type": "string"
         },
         "ClientCredentialsArn": {
@@ -980,14 +1064,20 @@
         },
         "ClientSecret": {
             "max": 512,
             "pattern": "\\S+",
             "sensitive": true,
             "type": "string"
         },
+        "ClientToken": {
+            "max": 256,
+            "min": 1,
+            "pattern": "[ -~]+",
+            "type": "string"
+        },
         "ClusterIdentifier": {
             "max": 512,
             "pattern": "\\S+",
             "type": "string"
         },
         "ConflictException": {
             "documentation": "<p> There was a conflict when processing the request (for example, a flow with the given name already exists within the account. Check for conflicting resource names and try again. </p>",
@@ -1105,14 +1195,22 @@
                     "documentation": "<p>Information about who registered the connector.</p>",
                     "shape": "RegisteredBy"
                 },
                 "supportedApiVersions": {
                     "documentation": "<p>A list of API versions that are supported by the connector.</p>",
                     "shape": "SupportedApiVersionList"
                 },
+                "supportedDataTransferApis": {
+                    "documentation": "<p>The APIs of the connector application that Amazon AppFlow can use to transfer your data.</p>",
+                    "shape": "SupportedDataTransferApis"
+                },
+                "supportedDataTransferTypes": {
+                    "documentation": "<p>The data transfer types that the connector supports.</p> <dl> <dt>RECORD</dt> <dd> <p>Structured records.</p> </dd> <dt>FILE</dt> <dd> <p>Files or binary data.</p> </dd> </dl>",
+                    "shape": "SupportedDataTransferTypeList"
+                },
                 "supportedDestinationConnectors": {
                     "documentation": "<p> Lists the connectors that are available for use as destinations. </p>",
                     "shape": "ConnectorTypeList"
                 },
                 "supportedOperators": {
                     "documentation": "<p>A list of operators supported by the connector.</p>",
                     "shape": "SupportedOperatorList"
@@ -1188,14 +1286,18 @@
                 "registeredAt": {
                     "documentation": "<p>The time at which the connector was registered.</p>",
                     "shape": "Date"
                 },
                 "registeredBy": {
                     "documentation": "<p>The user who registered the connector.</p>",
                     "shape": "RegisteredBy"
+                },
+                "supportedDataTransferTypes": {
+                    "documentation": "<p>The data transfer types that the connector supports.</p> <dl> <dt>RECORD</dt> <dd> <p>Structured records.</p> </dd> <dt>FILE</dt> <dd> <p>Files or binary data.</p> </dd> </dl>",
+                    "shape": "SupportedDataTransferTypeList"
                 }
             },
             "type": "structure"
         },
         "ConnectorEntity": {
             "documentation": "<p> The high-level entity that can be queried in Amazon AppFlow. For example, a Salesforce entity might be an <i>Account</i> or <i>Opportunity</i>, whereas a ServiceNow entity might be an <i>Incident</i>. </p>",
             "members": {
@@ -1889,14 +1991,19 @@
         "ConnectorVersion": {
             "max": 256,
             "pattern": "\\S+",
             "type": "string"
         },
         "CreateConnectorProfileRequest": {
             "members": {
+                "clientToken": {
+                    "documentation": "<p>The <code>clientToken</code> parameter is an idempotency token. It ensures that your <code>CreateConnectorProfile</code> request completes only once. You choose the value to pass. For example, if you don't receive a response from your request, you can safely retry the request with the same <code>clientToken</code> parameter value.</p> <p>If you omit a <code>clientToken</code> value, the Amazon Web Services SDK that you are using inserts a value for you. This way, the SDK can safely retry requests multiple times after a network error. You must provide your own value for other use cases.</p> <p>If you specify input parameters that differ from your first request, an error occurs. If you use a different value for <code>clientToken</code>, Amazon AppFlow considers it a new call to <code>CreateConnectorProfile</code>. The token is active for 8 hours.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ClientToken"
+                },
                 "connectionMode": {
                     "documentation": "<p> Indicates the connection mode and specifies whether it is public or private. Private flows use Amazon Web Services PrivateLink to route data over Amazon Web Services infrastructure without exposing it to the public internet. </p>",
                     "shape": "ConnectionMode"
                 },
                 "connectorLabel": {
                     "documentation": "<p>The label of the connector. The label is unique for each <code>ConnectorRegistration</code> in your Amazon Web Services account. Only needed if calling for CUSTOMCONNECTOR connector type/.</p>",
                     "shape": "ConnectorLabel"
@@ -1933,14 +2040,19 @@
                     "shape": "ConnectorProfileArn"
                 }
             },
             "type": "structure"
         },
         "CreateFlowRequest": {
             "members": {
+                "clientToken": {
+                    "documentation": "<p>The <code>clientToken</code> parameter is an idempotency token. It ensures that your <code>CreateFlow</code> request completes only once. You choose the value to pass. For example, if you don't receive a response from your request, you can safely retry the request with the same <code>clientToken</code> parameter value.</p> <p>If you omit a <code>clientToken</code> value, the Amazon Web Services SDK that you are using inserts a value for you. This way, the SDK can safely retry requests multiple times after a network error. You must provide your own value for other use cases.</p> <p>If you specify input parameters that differ from your first request, an error occurs. If you use a different value for <code>clientToken</code>, Amazon AppFlow considers it a new call to <code>CreateFlow</code>. The token is active for 8 hours.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ClientToken"
+                },
                 "description": {
                     "documentation": "<p> A description of the flow you want to create. </p>",
                     "shape": "FlowDescription"
                 },
                 "destinationFlowConfigList": {
                     "documentation": "<p> The configuration that controls how Amazon AppFlow places data in the destination connector. </p>",
                     "shape": "DestinationFlowConfigList"
@@ -2141,14 +2253,18 @@
         "CustomConnectorSourceProperties": {
             "documentation": "<p>The properties that are applied when the custom connector is being used as a source.</p>",
             "members": {
                 "customProperties": {
                     "documentation": "<p>Custom properties that are required to use the custom connector as a source.</p>",
                     "shape": "CustomProperties"
                 },
+                "dataTransferApi": {
+                    "documentation": "<p>The API of the connector application that Amazon AppFlow uses to transfer your data.</p>",
+                    "shape": "DataTransferApi"
+                },
                 "entityName": {
                     "documentation": "<p>The entity specified in the custom connector as a source in the flow.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "entityName"
@@ -2207,14 +2323,41 @@
         "DataPullMode": {
             "enum": [
                 "Incremental",
                 "Complete"
             ],
             "type": "string"
         },
+        "DataTransferApi": {
+            "documentation": "<p>The API of the connector application that Amazon AppFlow uses to transfer your data.</p>",
+            "members": {
+                "Name": {
+                    "documentation": "<p>The name of the connector application API.</p>",
+                    "shape": "DataTransferApiTypeName"
+                },
+                "Type": {
+                    "documentation": "<p>You can specify one of the following types:</p> <dl> <dt>AUTOMATIC</dt> <dd> <p>The default. Optimizes a flow for datasets that fluctuate in size from small to large. For each flow run, Amazon AppFlow chooses to use the SYNC or ASYNC API type based on the amount of data that the run transfers.</p> </dd> <dt>SYNC</dt> <dd> <p>A synchronous API. This type of API optimizes a flow for small to medium-sized datasets.</p> </dd> <dt>ASYNC</dt> <dd> <p>An asynchronous API. This type of API optimizes a flow for large datasets.</p> </dd> </dl>",
+                    "shape": "DataTransferApiType"
+                }
+            },
+            "type": "structure"
+        },
+        "DataTransferApiType": {
+            "enum": [
+                "SYNC",
+                "ASYNC",
+                "AUTOMATIC"
+            ],
+            "type": "string"
+        },
+        "DataTransferApiTypeName": {
+            "max": 64,
+            "pattern": "[\\w/-]+",
+            "type": "string"
+        },
         "DatabaseName": {
             "max": 512,
             "pattern": "\\S+",
             "type": "string"
         },
         "DatabaseUrl": {
             "max": 512,
@@ -2891,14 +3034,22 @@
             "type": "structure"
         },
         "ExecutionId": {
             "max": 256,
             "pattern": "\\S+",
             "type": "string"
         },
+        "ExecutionIds": {
+            "max": 100,
+            "member": {
+                "shape": "ExecutionId"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "ExecutionMessage": {
             "max": 2048,
             "pattern": "[\\s\\w/!@#+=.-]*",
             "type": "string"
         },
         "ExecutionRecord": {
             "documentation": "<p> Specifies information about the past flow run instances for a given flow. </p>",
@@ -2960,15 +3111,17 @@
             },
             "type": "structure"
         },
         "ExecutionStatus": {
             "enum": [
                 "InProgress",
                 "Successful",
-                "Error"
+                "Error",
+                "CancelStarted",
+                "Canceled"
             ],
             "type": "string"
         },
         "FieldType": {
             "type": "string"
         },
         "FieldTypeDetails": {
@@ -3412,14 +3565,20 @@
                 }
             },
             "type": "structure"
         },
         "JavaBoolean": {
             "type": "boolean"
         },
+        "JwtToken": {
+            "max": 8000,
+            "pattern": "^([a-zA-Z0-9_=]+)\\.([a-zA-Z0-9_=]+)\\.([a-zA-Z0-9_\\-\\+\\/=]*)",
+            "sensitive": true,
+            "type": "string"
+        },
         "KMSArn": {
             "max": 2048,
             "min": 20,
             "pattern": "arn:aws:kms:.*:[0-9]+:.*",
             "type": "string"
         },
         "Key": {
@@ -3837,15 +3996,16 @@
                 }
             },
             "type": "structure"
         },
         "OAuth2GrantType": {
             "enum": [
                 "CLIENT_CREDENTIALS",
-                "AUTHORIZATION_CODE"
+                "AUTHORIZATION_CODE",
+                "JWT_BEARER"
             ],
             "type": "string"
         },
         "OAuth2GrantTypeSupportedList": {
             "member": {
                 "shape": "OAuth2GrantType"
             },
@@ -4337,15 +4497,15 @@
         },
         "RedshiftMetadata": {
             "documentation": "<p> The connector metadata specific to Amazon Redshift. </p>",
             "members": {},
             "type": "structure"
         },
         "RefreshToken": {
-            "max": 2048,
+            "max": 4096,
             "pattern": "\\S+",
             "type": "string"
         },
         "Region": {
             "max": 64,
             "pattern": "\\S+",
             "type": "string"
@@ -4354,14 +4514,19 @@
             "member": {
                 "shape": "Region"
             },
             "type": "list"
         },
         "RegisterConnectorRequest": {
             "members": {
+                "clientToken": {
+                    "documentation": "<p>The <code>clientToken</code> parameter is an idempotency token. It ensures that your <code>RegisterConnector</code> request completes only once. You choose the value to pass. For example, if you don't receive a response from your request, you can safely retry the request with the same <code>clientToken</code> parameter value.</p> <p>If you omit a <code>clientToken</code> value, the Amazon Web Services SDK that you are using inserts a value for you. This way, the SDK can safely retry requests multiple times after a network error. You must provide your own value for other use cases.</p> <p>If you specify input parameters that differ from your first request, an error occurs. If you use a different value for <code>clientToken</code>, Amazon AppFlow considers it a new call to <code>RegisterConnector</code>. The token is active for 8 hours.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ClientToken"
+                },
                 "connectorLabel": {
                     "documentation": "<p> The name of the connector. The name is unique for each <code>ConnectorRegistration</code> in your Amazon Web Services account.</p>",
                     "shape": "ConnectorLabel"
                 },
                 "connectorProvisioningConfig": {
                     "documentation": "<p>The provisioning type of the connector. Currently the only supported value is LAMBDA.</p>",
                     "shape": "ConnectorProvisioningConfig"
@@ -4405,14 +4570,43 @@
                 "status": {
                     "documentation": "<p>Indicates the status of the registration attempt from Amazon AppFlow.</p>",
                     "shape": "ExecutionStatus"
                 }
             },
             "type": "structure"
         },
+        "ResetConnectorMetadataCacheRequest": {
+            "members": {
+                "apiVersion": {
+                    "documentation": "<p>The API version that you specified in the connector profile that you\u2019re resetting cached metadata for. You must use this parameter only if the connector supports multiple API versions or if the connector type is CustomConnector.</p> <p>To look up how many versions a connector supports, use the DescribeConnectors action. In the response, find the value that Amazon AppFlow returns for the connectorVersion parameter.</p> <p>To look up the connector type, use the DescribeConnectorProfiles action. In the response, find the value that Amazon AppFlow returns for the connectorType parameter.</p> <p>To look up the API version that you specified in a connector profile, use the DescribeConnectorProfiles action.</p>",
+                    "shape": "ApiVersion"
+                },
+                "connectorEntityName": {
+                    "documentation": "<p>Use this parameter if you want to reset cached metadata about the details for an individual entity.</p> <p>If you don't include this parameter in your request, Amazon AppFlow only resets cached metadata about entity names, not entity details.</p>",
+                    "shape": "EntityName"
+                },
+                "connectorProfileName": {
+                    "documentation": "<p>The name of the connector profile that you want to reset cached metadata for.</p> <p>You can omit this parameter if you're resetting the cache for any of the following connectors: Amazon Connect, Amazon EventBridge, Amazon Lookout for Metrics, Amazon S3, or Upsolver. If you're resetting the cache for any other connector, you must include this parameter in your request.</p>",
+                    "shape": "ConnectorProfileName"
+                },
+                "connectorType": {
+                    "documentation": "<p>The type of connector to reset cached metadata for.</p> <p>You must include this parameter in your request if you're resetting the cache for any of the following connectors: Amazon Connect, Amazon EventBridge, Amazon Lookout for Metrics, Amazon S3, or Upsolver. If you're resetting the cache for any other connector, you can omit this parameter from your request. </p>",
+                    "shape": "ConnectorType"
+                },
+                "entitiesPath": {
+                    "documentation": "<p>Use this parameter only if you\u2019re resetting the cached metadata about a nested entity. Only some connectors support nested entities. A nested entity is one that has another entity as a parent. To use this parameter, specify the name of the parent entity.</p> <p>To look up the parent-child relationship of entities, you can send a ListConnectorEntities request that omits the entitiesPath parameter. Amazon AppFlow will return a list of top-level entities. For each one, it indicates whether the entity has nested entities. Then, in a subsequent ListConnectorEntities request, you can specify a parent entity name for the entitiesPath parameter. Amazon AppFlow will return a list of the child entities for that parent.</p>",
+                    "shape": "EntitiesPath"
+                }
+            },
+            "type": "structure"
+        },
+        "ResetConnectorMetadataCacheResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "ResourceNotFoundException": {
             "documentation": "<p> The resource specified in the request (such as the source or destination connector profile) is not found. </p>",
             "error": {
                 "httpStatusCode": 404
             },
             "exception": true,
             "members": {
@@ -4586,14 +4780,18 @@
                     "documentation": "<p> The application path to catalog service. </p>",
                     "shape": "ApplicationServicePath"
                 },
                 "clientNumber": {
                     "documentation": "<p> The client number for the client creating the connection. </p>",
                     "shape": "ClientNumber"
                 },
+                "disableSSO": {
+                    "documentation": "<p>If you set this parameter to <code>true</code>, Amazon AppFlow bypasses the single sign-on (SSO) settings in your SAP account when it accesses your SAP OData instance.</p> <p>Whether you need this option depends on the types of credentials that you applied to your SAP OData connection profile. If your profile uses basic authentication credentials, SAP SSO can prevent Amazon AppFlow from connecting to your account with your username and password. In this case, bypassing SSO makes it possible for Amazon AppFlow to connect successfully. However, if your profile uses OAuth credentials, this parameter has no affect.</p>",
+                    "shape": "Boolean"
+                },
                 "logonLanguage": {
                     "documentation": "<p> The logon language of SAPOData instance. </p>",
                     "shape": "LogonLanguage"
                 },
                 "oAuthProperties": {
                     "documentation": "<p> The SAPOData OAuth properties required for OAuth type authentication. </p>",
                     "shape": "OAuthProperties"
@@ -4690,14 +4888,22 @@
                     "documentation": "<p> The credentials used to access protected Salesforce resources. </p>",
                     "shape": "AccessToken"
                 },
                 "clientCredentialsArn": {
                     "documentation": "<p> The secret manager ARN, which contains the client ID and client secret of the connected app. </p>",
                     "shape": "ClientCredentialsArn"
                 },
+                "jwtToken": {
+                    "documentation": "<p>A JSON web token (JWT) that authorizes Amazon AppFlow to access your Salesforce records.</p>",
+                    "shape": "JwtToken"
+                },
+                "oAuth2GrantType": {
+                    "documentation": "<p>Specifies the OAuth 2.0 grant type that Amazon AppFlow uses when it requests an access token from Salesforce. Amazon AppFlow requires an access token each time it attempts to access your Salesforce records.</p> <p>You can specify one of the following values:</p> <dl> <dt>AUTHORIZATION_CODE</dt> <dd> <p>Amazon AppFlow passes an authorization code when it requests the access token from Salesforce. Amazon AppFlow receives the authorization code from Salesforce after you log in to your Salesforce account and authorize Amazon AppFlow to access your records.</p> </dd> <dt>CLIENT_CREDENTIALS</dt> <dd> <p>Amazon AppFlow passes client credentials (a client ID and client secret) when it requests the access token from Salesforce. You provide these credentials to Amazon AppFlow when you define the connection to your Salesforce account.</p> </dd> <dt>JWT_BEARER</dt> <dd> <p>Amazon AppFlow passes a JSON web token (JWT) when it requests the access token from Salesforce. You provide the JWT to Amazon AppFlow when you define the connection to your Salesforce account. When you use this grant type, you don't need to log in to your Salesforce account to authorize Amazon AppFlow to access your records.</p> </dd> </dl>",
+                    "shape": "OAuth2GrantType"
+                },
                 "oAuthRequest": {
                     "documentation": "<p> The OAuth requirement needed to request security tokens from the connector endpoint. </p>",
                     "shape": "ConnectorOAuthRequest"
                 },
                 "refreshToken": {
                     "documentation": "<p> The credentials used to acquire new access tokens. </p>",
                     "shape": "RefreshToken"
@@ -4772,14 +4978,18 @@
                 "dataTransferApis": {
                     "documentation": "<p>The Salesforce APIs that you can have Amazon AppFlow use when your flows transfers data to or from Salesforce.</p>",
                     "shape": "SalesforceDataTransferApiList"
                 },
                 "oAuthScopes": {
                     "documentation": "<p> The desired authorization scope for the Salesforce account. </p>",
                     "shape": "OAuthScopeList"
+                },
+                "oauth2GrantTypesSupported": {
+                    "documentation": "<p>The OAuth 2.0 grant types that Amazon AppFlow can use when it requests an access token from Salesforce. Amazon AppFlow requires an access token each time it attempts to access your Salesforce records.</p> <dl> <dt>AUTHORIZATION_CODE</dt> <dd> <p>Amazon AppFlow passes an authorization code when it requests the access token from Salesforce. Amazon AppFlow receives the authorization code from Salesforce after you log in to your Salesforce account and authorize Amazon AppFlow to access your records.</p> </dd> <dt>CLIENT_CREDENTIALS</dt> <dd> <p>Amazon AppFlow passes client credentials (a client ID and client secret) when it requests the access token from Salesforce. You provide these credentials to Amazon AppFlow when you define the connection to your Salesforce account.</p> </dd> <dt>JWT_BEARER</dt> <dd> <p>Amazon AppFlow passes a JSON web token (JWT) when it requests the access token from Salesforce. You provide the JWT to Amazon AppFlow when you define the connection to your Salesforce account. When you use this grant type, you don't need to log in to your Salesforce account to authorize Amazon AppFlow to access your records.</p> </dd> </dl>",
+                    "shape": "OAuth2GrantTypeSupportedList"
                 }
             },
             "type": "structure"
         },
         "SalesforceSourceProperties": {
             "documentation": "<p> The properties that are applied when Salesforce is being used as a source. </p>",
             "members": {
@@ -5332,14 +5542,19 @@
         "Stage": {
             "max": 512,
             "pattern": "\\S+",
             "type": "string"
         },
         "StartFlowRequest": {
             "members": {
+                "clientToken": {
+                    "documentation": "<p>The <code>clientToken</code> parameter is an idempotency token. It ensures that your <code>StartFlow</code> request completes only once. You choose the value to pass. For example, if you don't receive a response from your request, you can safely retry the request with the same <code>clientToken</code> parameter value.</p> <p>If you omit a <code>clientToken</code> value, the Amazon Web Services SDK that you are using inserts a value for you. This way, the SDK can safely retry requests multiple times after a network error. You must provide your own value for other use cases.</p> <p>If you specify input parameters that differ from your first request, an error occurs for flows that run on a schedule or based on an event. However, the error doesn't occur for flows that run on demand. You set the conditions that initiate your flow for the <code>triggerConfig</code> parameter.</p> <p>If you use a different value for <code>clientToken</code>, Amazon AppFlow considers it a new call to <code>StartFlow</code>. The token is active for 8 hours.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ClientToken"
+                },
                 "flowName": {
                     "documentation": "<p> The specified name of the flow. Spaces are not allowed. Use underscores (_) or hyphens (-) only. </p>",
                     "shape": "FlowName"
                 }
             },
             "required": [
                 "flowName"
@@ -5414,14 +5629,33 @@
         },
         "SupportedApiVersionList": {
             "member": {
                 "shape": "SupportedApiVersion"
             },
             "type": "list"
         },
+        "SupportedDataTransferApis": {
+            "member": {
+                "shape": "DataTransferApi"
+            },
+            "type": "list"
+        },
+        "SupportedDataTransferType": {
+            "enum": [
+                "RECORD",
+                "FILE"
+            ],
+            "type": "string"
+        },
+        "SupportedDataTransferTypeList": {
+            "member": {
+                "shape": "SupportedDataTransferType"
+            },
+            "type": "list"
+        },
         "SupportedFieldTypeDetails": {
             "documentation": "<p> Contains details regarding all the supported <code>FieldTypes</code> and their corresponding <code>filterOperators</code> and <code>supportedValues</code>. </p>",
             "members": {
                 "v1": {
                     "documentation": "<p> The initial supported version for <code>fieldType</code>. If this is later changed to a different version, v2 will be introduced. </p>",
                     "shape": "FieldTypeDetails"
                 }
@@ -5754,14 +5988,19 @@
         },
         "UntagResourceResponse": {
             "members": {},
             "type": "structure"
         },
         "UpdateConnectorProfileRequest": {
             "members": {
+                "clientToken": {
+                    "documentation": "<p>The <code>clientToken</code> parameter is an idempotency token. It ensures that your <code>UpdateConnectorProfile</code> request completes only once. You choose the value to pass. For example, if you don't receive a response from your request, you can safely retry the request with the same <code>clientToken</code> parameter value.</p> <p>If you omit a <code>clientToken</code> value, the Amazon Web Services SDK that you are using inserts a value for you. This way, the SDK can safely retry requests multiple times after a network error. You must provide your own value for other use cases.</p> <p>If you specify input parameters that differ from your first request, an error occurs. If you use a different value for <code>clientToken</code>, Amazon AppFlow considers it a new call to <code>UpdateConnectorProfile</code>. The token is active for 8 hours.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ClientToken"
+                },
                 "connectionMode": {
                     "documentation": "<p> Indicates the connection mode and if it is public or private. </p>",
                     "shape": "ConnectionMode"
                 },
                 "connectorProfileConfig": {
                     "documentation": "<p> Defines the connector-specific profile configuration and credentials. </p>",
                     "shape": "ConnectorProfileConfig"
@@ -5785,14 +6024,19 @@
                     "shape": "ConnectorProfileArn"
                 }
             },
             "type": "structure"
         },
         "UpdateConnectorRegistrationRequest": {
             "members": {
+                "clientToken": {
+                    "documentation": "<p>The <code>clientToken</code> parameter is an idempotency token. It ensures that your <code>UpdateConnectorRegistration</code> request completes only once. You choose the value to pass. For example, if you don't receive a response from your request, you can safely retry the request with the same <code>clientToken</code> parameter value.</p> <p>If you omit a <code>clientToken</code> value, the Amazon Web Services SDK that you are using inserts a value for you. This way, the SDK can safely retry requests multiple times after a network error. You must provide your own value for other use cases.</p> <p>If you specify input parameters that differ from your first request, an error occurs. If you use a different value for <code>clientToken</code>, Amazon AppFlow considers it a new call to <code>UpdateConnectorRegistration</code>. The token is active for 8 hours.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ClientToken"
+                },
                 "connectorLabel": {
                     "documentation": "<p>The name of the connector. The name is unique for each connector registration in your AWS account.</p>",
                     "shape": "ConnectorLabel"
                 },
                 "connectorProvisioningConfig": {
                     "shape": "ConnectorProvisioningConfig"
                 },
@@ -5813,14 +6057,19 @@
                     "shape": "ARN"
                 }
             },
             "type": "structure"
         },
         "UpdateFlowRequest": {
             "members": {
+                "clientToken": {
+                    "documentation": "<p>The <code>clientToken</code> parameter is an idempotency token. It ensures that your <code>UpdateFlow</code> request completes only once. You choose the value to pass. For example, if you don't receive a response from your request, you can safely retry the request with the same <code>clientToken</code> parameter value.</p> <p>If you omit a <code>clientToken</code> value, the Amazon Web Services SDK that you are using inserts a value for you. This way, the SDK can safely retry requests multiple times after a network error. You must provide your own value for other use cases.</p> <p>If you specify input parameters that differ from your first request, an error occurs. If you use a different value for <code>clientToken</code>, Amazon AppFlow considers it a new call to <code>UpdateFlow</code>. The token is active for 8 hours.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ClientToken"
+                },
                 "description": {
                     "documentation": "<p> A description of the flow. </p>",
                     "shape": "FlowDescription"
                 },
                 "destinationFlowConfigList": {
                     "documentation": "<p> The configuration that controls how Amazon AppFlow transfers data to the destination connector. </p>",
                     "shape": "DestinationFlowConfigList"
```

### Comparing `botocore-a-la-carte-appflow-1.29.99/botocore_a_la_carte_appflow.egg-info/PKG-INFO` & `botocore-a-la-carte-appflow-1.30.0/botocore_a_la_carte_appflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-appflow
-Version: 1.29.99
+Version: 1.30.0
 Summary: appflow data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-appflow-1.29.99/setup.py` & `botocore-a-la-carte-appflow-1.30.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-appflow',
-    version="1.29.99",
+    version="1.30.0",
     description='appflow data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/appflow/*/*.json'],
```

