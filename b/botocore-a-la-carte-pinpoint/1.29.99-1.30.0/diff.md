# Comparing `tmp/botocore-a-la-carte-pinpoint-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-pinpoint-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-pinpoint-1.29.99.tar", last modified: Sat Mar 25 01:22:58 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-pinpoint-1.30.0.tar", last modified: Tue Jul  4 01:44:50 2023, max compression
```

## Comparing `botocore-a-la-carte-pinpoint-1.29.99.tar` & `botocore-a-la-carte-pinpoint-1.30.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:58.192472 botocore-a-la-carte-pinpoint-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:57.000000 botocore-a-la-carte-pinpoint-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:22:58.192472 botocore-a-la-carte-pinpoint-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:58.188471 botocore-a-la-carte-pinpoint-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:58.188471 botocore-a-la-carte-pinpoint-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:58.188471 botocore-a-la-carte-pinpoint-1.29.99/botocore/data/pinpoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:58.188471 botocore-a-la-carte-pinpoint-1.29.99/botocore/data/pinpoint/2016-12-01/
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-03-25 01:22:12.000000 botocore-a-la-carte-pinpoint-1.29.99/botocore/data/pinpoint/2016-12-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-pinpoint-1.29.99/botocore/data/pinpoint/2016-12-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   732736 2023-03-25 01:22:12.000000 botocore-a-la-carte-pinpoint-1.29.99/botocore/data/pinpoint/2016-12-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:58.192472 botocore-a-la-carte-pinpoint-1.29.99/botocore_a_la_carte_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:22:58.000000 botocore-a-la-carte-pinpoint-1.29.99/botocore_a_la_carte_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-25 01:22:58.000000 botocore-a-la-carte-pinpoint-1.29.99/botocore_a_la_carte_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:58.000000 botocore-a-la-carte-pinpoint-1.29.99/botocore_a_la_carte_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:58.000000 botocore-a-la-carte-pinpoint-1.29.99/botocore_a_la_carte_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:58.192472 botocore-a-la-carte-pinpoint-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-25 01:22:57.000000 botocore-a-la-carte-pinpoint-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:50.018736 botocore-a-la-carte-pinpoint-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:49.000000 botocore-a-la-carte-pinpoint-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:50.018736 botocore-a-la-carte-pinpoint-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:50.014736 botocore-a-la-carte-pinpoint-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:50.014736 botocore-a-la-carte-pinpoint-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:50.014736 botocore-a-la-carte-pinpoint-1.30.0/botocore/data/pinpoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:50.014736 botocore-a-la-carte-pinpoint-1.30.0/botocore/data/pinpoint/2016-12-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    24183 2023-07-04 01:44:02.000000 botocore-a-la-carte-pinpoint-1.30.0/botocore/data/pinpoint/2016-12-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-pinpoint-1.30.0/botocore/data/pinpoint/2016-12-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   759440 2023-07-04 01:44:02.000000 botocore-a-la-carte-pinpoint-1.30.0/botocore/data/pinpoint/2016-12-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:50.018736 botocore-a-la-carte-pinpoint-1.30.0/botocore_a_la_carte_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:49.000000 botocore-a-la-carte-pinpoint-1.30.0/botocore_a_la_carte_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-04 01:44:49.000000 botocore-a-la-carte-pinpoint-1.30.0/botocore_a_la_carte_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:49.000000 botocore-a-la-carte-pinpoint-1.30.0/botocore_a_la_carte_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:49.000000 botocore-a-la-carte-pinpoint-1.30.0/botocore_a_la_carte_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:50.018736 botocore-a-la-carte-pinpoint-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-04 01:44:49.000000 botocore-a-la-carte-pinpoint-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-pinpoint-1.29.99/LICENSE.txt` & `botocore-a-la-carte-pinpoint-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-pinpoint-1.29.99/PKG-INFO` & `botocore-a-la-carte-pinpoint-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-pinpoint
-Version: 1.29.99
+Version: 1.30.0
 Summary: pinpoint data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-pinpoint-1.29.99/botocore/data/pinpoint/2016-12-01/service-2.json` & `botocore-a-la-carte-pinpoint-1.30.0/botocore/data/pinpoint/2016-12-01/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935929698091495%*

 * *Differences: {"'operations'": "{'GetJourneyRunExecutionActivityMetrics': OrderedDict([('name', "*

 * *                 "'GetJourneyRunExecutionActivityMetrics'), ('http', OrderedDict([('method', "*

 * *                 "'GET'), ('requestUri', "*

 * *                 "'/v1/apps/{application-id}/journeys/{journey-id}/runs/{run-id}/activities/{journey-activity-id}/execution-metrics'), "*

 * *                 "('responseCode', 200)])), ('input', OrderedDict([('shape', "*

 * *                 "'GetJourneyRunExecutionActivityMetricsRequest')])), ('ou […]*

```diff
@@ -3050,14 +3050,152 @@
             },
             "name": "GetJourneyExecutionMetrics",
             "output": {
                 "documentation": "<p>The request succeeded.</p>",
                 "shape": "GetJourneyExecutionMetricsResponse"
             }
         },
+        "GetJourneyRunExecutionActivityMetrics": {
+            "documentation": "<p>Retrieves (queries) pre-aggregated data for a standard run execution metric that applies to a journey activity.</p>",
+            "errors": [
+                {
+                    "documentation": "<p>The request contains a syntax error (BadRequestException).</p>",
+                    "shape": "BadRequestException"
+                },
+                {
+                    "documentation": "<p>The request failed due to an unknown internal server error, exception, or failure (InternalServerErrorException).</p>",
+                    "shape": "InternalServerErrorException"
+                },
+                {
+                    "documentation": "<p>The request failed because the payload for the body of the request is too large (RequestEntityTooLargeException).</p>",
+                    "shape": "PayloadTooLargeException"
+                },
+                {
+                    "documentation": "<p>The request was denied because access to the specified resource is forbidden (ForbiddenException).</p>",
+                    "shape": "ForbiddenException"
+                },
+                {
+                    "documentation": "<p>The request failed because the specified resource was not found (NotFoundException).</p>",
+                    "shape": "NotFoundException"
+                },
+                {
+                    "documentation": "<p>The request failed because the method is not allowed for the specified resource (MethodNotAllowedException).</p>",
+                    "shape": "MethodNotAllowedException"
+                },
+                {
+                    "documentation": "<p>The request failed because too many requests were sent during a certain amount of time (TooManyRequestsException).</p>",
+                    "shape": "TooManyRequestsException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/v1/apps/{application-id}/journeys/{journey-id}/runs/{run-id}/activities/{journey-activity-id}/execution-metrics",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "GetJourneyRunExecutionActivityMetricsRequest"
+            },
+            "name": "GetJourneyRunExecutionActivityMetrics",
+            "output": {
+                "documentation": "<p>The request succeeded.</p>",
+                "shape": "GetJourneyRunExecutionActivityMetricsResponse"
+            }
+        },
+        "GetJourneyRunExecutionMetrics": {
+            "documentation": "<p>Retrieves (queries) pre-aggregated data for a standard run execution metric that applies to a journey.</p>",
+            "errors": [
+                {
+                    "documentation": "<p>The request contains a syntax error (BadRequestException).</p>",
+                    "shape": "BadRequestException"
+                },
+                {
+                    "documentation": "<p>The request failed due to an unknown internal server error, exception, or failure (InternalServerErrorException).</p>",
+                    "shape": "InternalServerErrorException"
+                },
+                {
+                    "documentation": "<p>The request failed because the payload for the body of the request is too large (RequestEntityTooLargeException).</p>",
+                    "shape": "PayloadTooLargeException"
+                },
+                {
+                    "documentation": "<p>The request was denied because access to the specified resource is forbidden (ForbiddenException).</p>",
+                    "shape": "ForbiddenException"
+                },
+                {
+                    "documentation": "<p>The request failed because the specified resource was not found (NotFoundException).</p>",
+                    "shape": "NotFoundException"
+                },
+                {
+                    "documentation": "<p>The request failed because the method is not allowed for the specified resource (MethodNotAllowedException).</p>",
+                    "shape": "MethodNotAllowedException"
+                },
+                {
+                    "documentation": "<p>The request failed because too many requests were sent during a certain amount of time (TooManyRequestsException).</p>",
+                    "shape": "TooManyRequestsException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/v1/apps/{application-id}/journeys/{journey-id}/runs/{run-id}/execution-metrics",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "GetJourneyRunExecutionMetricsRequest"
+            },
+            "name": "GetJourneyRunExecutionMetrics",
+            "output": {
+                "documentation": "<p>The request succeeded.</p>",
+                "shape": "GetJourneyRunExecutionMetricsResponse"
+            }
+        },
+        "GetJourneyRuns": {
+            "documentation": "<p>Provides information about the runs of a journey.</p>",
+            "errors": [
+                {
+                    "documentation": "<p>The request contains a syntax error (BadRequestException).</p>",
+                    "shape": "BadRequestException"
+                },
+                {
+                    "documentation": "<p>The request failed due to an unknown internal server error, exception, or failure (InternalServerErrorException).</p>",
+                    "shape": "InternalServerErrorException"
+                },
+                {
+                    "documentation": "<p>The request failed because the payload for the body of the request is too large (RequestEntityTooLargeException).</p>",
+                    "shape": "PayloadTooLargeException"
+                },
+                {
+                    "documentation": "<p>The request was denied because access to the specified resource is forbidden (ForbiddenException).</p>",
+                    "shape": "ForbiddenException"
+                },
+                {
+                    "documentation": "<p>The request failed because the specified resource was not found (NotFoundException).</p>",
+                    "shape": "NotFoundException"
+                },
+                {
+                    "documentation": "<p>The request failed because the method is not allowed for the specified resource (MethodNotAllowedException).</p>",
+                    "shape": "MethodNotAllowedException"
+                },
+                {
+                    "documentation": "<p>The request failed because too many requests were sent during a certain amount of time (TooManyRequestsException).</p>",
+                    "shape": "TooManyRequestsException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/v1/apps/{application-id}/journeys/{journey-id}/runs",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "GetJourneyRunsRequest"
+            },
+            "name": "GetJourneyRuns",
+            "output": {
+                "documentation": "<p>The request succeeded.</p>",
+                "shape": "GetJourneyRunsResponse"
+            }
+        },
         "GetPushTemplate": {
             "documentation": "<p>Retrieves the content and settings of a message template for messages that are sent through a push notification channel.</p>",
             "errors": [
                 {
                     "documentation": "<p>The request contains a syntax error (BadRequestException).</p>",
                     "shape": "BadRequestException"
                 },
@@ -6068,14 +6206,18 @@
                     "documentation": "<p>The unique identifier for the campaign that the activity applies to.</p>",
                     "shape": "__string"
                 },
                 "End": {
                     "documentation": "<p>The actual time, in ISO 8601 format, when the activity was marked CANCELLED or COMPLETED.</p>",
                     "shape": "__string"
                 },
+                "ExecutionMetrics": {
+                    "documentation": "<p>A JSON object that contains metrics relating to the campaign execution for this campaign activity. For information about the structure and contents of the results, see <a href=\"https://docs.aws.amazon.com//pinpoint/latest/developerguide/analytics-standard-metrics.html\">Standard Amazon Pinpoint analytics metrics</a> in the <i>Amazon Pinpoint Developer Guide</i>.</p>",
+                    "shape": "MapOf__string"
+                },
                 "Id": {
                     "documentation": "<p>The unique identifier for the activity.</p>",
                     "shape": "__string"
                 },
                 "Result": {
                     "documentation": "<p>Specifies whether the activity succeeded. Possible values are SUCCESS and FAIL.</p>",
                     "shape": "__string"
@@ -6953,52 +7095,52 @@
             },
             "required": [
                 "Channels"
             ],
             "type": "structure"
         },
         "ClosedDays": {
-            "documentation": "<p>The time when journey will stop sending messages.</p>",
+            "documentation": "<p>The time when a journey will not send messages. QuietTime should be configured first and SendingSchedule should be set to true.</p>",
             "members": {
                 "CUSTOM": {
-                    "documentation": "<p>Rules for Custom Channel.</p>",
+                    "documentation": "<p>Rules for the Custom channel.</p>",
                     "shape": "ListOfClosedDaysRules"
                 },
                 "EMAIL": {
-                    "documentation": "<p>Rules for Email Channel.</p>",
+                    "documentation": "<p>Rules for the Email channel.</p>",
                     "shape": "ListOfClosedDaysRules"
                 },
                 "PUSH": {
-                    "documentation": "<p>Rules for Push Channel.</p>",
+                    "documentation": "<p>Rules for the Push channel.</p>",
                     "shape": "ListOfClosedDaysRules"
                 },
                 "SMS": {
-                    "documentation": "<p>Rules for SMS Channel.</p>",
+                    "documentation": "<p>Rules for the SMS channel.</p>",
                     "shape": "ListOfClosedDaysRules"
                 },
                 "VOICE": {
-                    "documentation": "<p>Rules for Voice Channel.</p>",
+                    "documentation": "<p>Rules for the Voice channel.</p>",
                     "shape": "ListOfClosedDaysRules"
                 }
             },
             "type": "structure"
         },
         "ClosedDaysRule": {
-            "documentation": "<p>Closed Days Rule. Part of Journey sending schedule.</p>",
+            "documentation": "<p>Specifies the rule settings for when messages can't be sent.</p>",
             "members": {
                 "EndDateTime": {
-                    "documentation": "<p>End Datetime in ISO 8601 format.</p>",
+                    "documentation": "<p>End DateTime ISO 8601 format</p>",
                     "shape": "__string"
                 },
                 "Name": {
-                    "documentation": "<p>Name of the rule.</p>",
+                    "documentation": "<p>The name of the closed day rule.</p>",
                     "shape": "__string"
                 },
                 "StartDateTime": {
-                    "documentation": "<p>Start Datetime in ISO 8601 format.</p>",
+                    "documentation": "<p>Start DateTime ISO 8601 format</p>",
                     "shape": "__string"
                 }
             },
             "type": "structure"
         },
         "Condition": {
             "documentation": "<p>Specifies the conditions to evaluate for an activity in a journey, and how to evaluate those conditions.</p>",
@@ -8582,15 +8724,15 @@
                     "shape": "__string"
                 },
                 "TextPart": {
                     "documentation": "<p>The message body, in plain text format, to use in email messages that are based on the message template. We recommend using plain text format for email clients that don't render HTML content and clients that are connected to high-latency networks, such as mobile devices.</p>",
                     "shape": "__string"
                 },
                 "tags": {
-                    "documentation": "<p>A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
+                    "documentation": "<note><p>As of <b>22-05-2023</b> tags has been deprecated for update operations. After this date any value in tags is not processed and an error code is not returned. To manage tags we recommend using either <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/tags-resource-arn.html\">Tags</a> in the <i>API Reference for Amazon Pinpoint</i>, <a href=\"https://docs.aws.amazon.com/cli/latest/reference/resourcegroupstaggingapi/index.html\">resourcegroupstaggingapi</a> commands in the <i>AWS Command Line Interface Documentation</i> or <a href=\"https://sdk.amazonaws.com/java/api/latest/software/amazon/awssdk/services/resourcegroupstaggingapi/package-summary.html\">resourcegroupstaggingapi</a> in the <i>AWS SDK</i>.</p></note> <p>(Deprecated) A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
                     "locationName": "tags",
                     "shape": "MapOf__string"
                 }
             },
             "type": "structure"
         },
         "EmailTemplateResponse": {
@@ -10587,15 +10729,15 @@
                 "JourneyId": {
                     "documentation": "<p>The unique identifier for the journey.</p>",
                     "location": "uri",
                     "locationName": "journey-id",
                     "shape": "__string"
                 },
                 "NextToken": {
-                    "documentation": "<p>The  string that specifies which page of results to return in a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
+                    "documentation": "<p>The <code/> string that specifies which page of results to return in a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
                     "location": "querystring",
                     "locationName": "next-token",
                     "shape": "__string"
                 },
                 "PageSize": {
                     "documentation": "<p>The maximum number of items to include in each page of a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
                     "location": "querystring",
@@ -10633,15 +10775,15 @@
                 "JourneyId": {
                     "documentation": "<p>The unique identifier for the journey.</p>",
                     "location": "uri",
                     "locationName": "journey-id",
                     "shape": "__string"
                 },
                 "NextToken": {
-                    "documentation": "<p>The  string that specifies which page of results to return in a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
+                    "documentation": "<p>The <code/> string that specifies which page of results to return in a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
                     "location": "querystring",
                     "locationName": "next-token",
                     "shape": "__string"
                 },
                 "PageSize": {
                     "documentation": "<p>The maximum number of items to include in each page of a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
                     "location": "querystring",
@@ -10696,14 +10838,170 @@
             },
             "payload": "JourneyResponse",
             "required": [
                 "JourneyResponse"
             ],
             "type": "structure"
         },
+        "GetJourneyRunExecutionActivityMetricsRequest": {
+            "members": {
+                "ApplicationId": {
+                    "documentation": "<p>The unique identifier for the application. This identifier is displayed as the <b>Project ID</b> on the Amazon Pinpoint console.</p>",
+                    "location": "uri",
+                    "locationName": "application-id",
+                    "shape": "__string"
+                },
+                "JourneyActivityId": {
+                    "documentation": "<p>The unique identifier for the journey activity.</p>",
+                    "location": "uri",
+                    "locationName": "journey-activity-id",
+                    "shape": "__string"
+                },
+                "JourneyId": {
+                    "documentation": "<p>The unique identifier for the journey.</p>",
+                    "location": "uri",
+                    "locationName": "journey-id",
+                    "shape": "__string"
+                },
+                "NextToken": {
+                    "documentation": "<p>The <code/> string that specifies which page of results to return in a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
+                    "location": "querystring",
+                    "locationName": "next-token",
+                    "shape": "__string"
+                },
+                "PageSize": {
+                    "documentation": "<p>The maximum number of items to include in each page of a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
+                    "location": "querystring",
+                    "locationName": "page-size",
+                    "shape": "__string"
+                },
+                "RunId": {
+                    "documentation": "<p>The unique identifier for the journey run.</p>",
+                    "location": "uri",
+                    "locationName": "run-id",
+                    "shape": "__string"
+                }
+            },
+            "required": [
+                "RunId",
+                "JourneyActivityId",
+                "JourneyId",
+                "ApplicationId"
+            ],
+            "type": "structure"
+        },
+        "GetJourneyRunExecutionActivityMetricsResponse": {
+            "members": {
+                "JourneyRunExecutionActivityMetricsResponse": {
+                    "shape": "JourneyRunExecutionActivityMetricsResponse"
+                }
+            },
+            "payload": "JourneyRunExecutionActivityMetricsResponse",
+            "required": [
+                "JourneyRunExecutionActivityMetricsResponse"
+            ],
+            "type": "structure"
+        },
+        "GetJourneyRunExecutionMetricsRequest": {
+            "members": {
+                "ApplicationId": {
+                    "documentation": "<p>The unique identifier for the application. This identifier is displayed as the <b>Project ID</b> on the Amazon Pinpoint console.</p>",
+                    "location": "uri",
+                    "locationName": "application-id",
+                    "shape": "__string"
+                },
+                "JourneyId": {
+                    "documentation": "<p>The unique identifier for the journey.</p>",
+                    "location": "uri",
+                    "locationName": "journey-id",
+                    "shape": "__string"
+                },
+                "NextToken": {
+                    "documentation": "<p>The <code/> string that specifies which page of results to return in a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
+                    "location": "querystring",
+                    "locationName": "next-token",
+                    "shape": "__string"
+                },
+                "PageSize": {
+                    "documentation": "<p>The maximum number of items to include in each page of a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
+                    "location": "querystring",
+                    "locationName": "page-size",
+                    "shape": "__string"
+                },
+                "RunId": {
+                    "documentation": "<p>The unique identifier for the journey run.</p>",
+                    "location": "uri",
+                    "locationName": "run-id",
+                    "shape": "__string"
+                }
+            },
+            "required": [
+                "RunId",
+                "ApplicationId",
+                "JourneyId"
+            ],
+            "type": "structure"
+        },
+        "GetJourneyRunExecutionMetricsResponse": {
+            "members": {
+                "JourneyRunExecutionMetricsResponse": {
+                    "shape": "JourneyRunExecutionMetricsResponse"
+                }
+            },
+            "payload": "JourneyRunExecutionMetricsResponse",
+            "required": [
+                "JourneyRunExecutionMetricsResponse"
+            ],
+            "type": "structure"
+        },
+        "GetJourneyRunsRequest": {
+            "members": {
+                "ApplicationId": {
+                    "documentation": "<p>The unique identifier for the application. This identifier is displayed as the <b>Project ID</b> on the Amazon Pinpoint console.</p>",
+                    "location": "uri",
+                    "locationName": "application-id",
+                    "shape": "__string"
+                },
+                "JourneyId": {
+                    "documentation": "<p>The unique identifier for the journey.</p>",
+                    "location": "uri",
+                    "locationName": "journey-id",
+                    "shape": "__string"
+                },
+                "PageSize": {
+                    "documentation": "<p>The maximum number of items to include in each page of a paginated response. This parameter is not supported for application, campaign, and journey metrics.</p>",
+                    "location": "querystring",
+                    "locationName": "page-size",
+                    "shape": "__string"
+                },
+                "Token": {
+                    "documentation": "<p>The NextToken string that specifies which page of results to return in a paginated response.</p>",
+                    "location": "querystring",
+                    "locationName": "token",
+                    "shape": "__string"
+                }
+            },
+            "required": [
+                "ApplicationId",
+                "JourneyId"
+            ],
+            "type": "structure"
+        },
+        "GetJourneyRunsResponse": {
+            "members": {
+                "JourneyRunsResponse": {
+                    "shape": "JourneyRunsResponse"
+                }
+            },
+            "payload": "JourneyRunsResponse",
+            "required": [
+                "JourneyRunsResponse"
+            ],
+            "type": "structure"
+        },
         "GetPushTemplateRequest": {
             "members": {
                 "TemplateName": {
                     "documentation": "<p>The name of the message template. A template name must start with an alphanumeric character and can contain a maximum of 128 characters. The characters can be alphanumeric characters, underscores (_), or hyphens (-). Template names are case sensitive.</p>",
                     "location": "uri",
                     "locationName": "template-name",
                     "shape": "__string"
@@ -11566,15 +11864,15 @@
                     "shape": "Layout"
                 },
                 "TemplateDescription": {
                     "documentation": "<p>The description of the template.</p>",
                     "shape": "__string"
                 },
                 "tags": {
-                    "documentation": "<p>A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
+                    "documentation": "<note><p>As of <b>22-05-2023</b> tags has been deprecated for update operations. After this date any value in tags is not processed and an error code is not returned. To manage tags we recommend using either <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/tags-resource-arn.html\">Tags</a> in the <i>API Reference for Amazon Pinpoint</i>, <a href=\"https://docs.aws.amazon.com/cli/latest/reference/resourcegroupstaggingapi/index.html\">resourcegroupstaggingapi</a> commands in the <i>AWS Command Line Interface Documentation</i> or <a href=\"https://sdk.amazonaws.com/java/api/latest/software/amazon/awssdk/services/resourcegroupstaggingapi/package-summary.html\">resourcegroupstaggingapi</a> in the <i>AWS SDK</i>.</p></note> <p>(Deprecated) A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
                     "locationName": "tags",
                     "shape": "MapOf__string"
                 }
             },
             "type": "structure"
         },
         "InAppTemplateResponse": {
@@ -11764,15 +12062,15 @@
             },
             "type": "structure"
         },
         "JourneyExecutionActivityMetricsResponse": {
             "documentation": "<p>Provides the results of a query that retrieved the data for a standard execution metric that applies to a journey activity, and provides information about that query.</p>",
             "members": {
                 "ActivityType": {
-                    "documentation": "<p>The type of activity that the metric applies to. Possible values are:</p> <ul><li><p>CONDITIONAL_SPLIT - For a yes/no split activity, which is an activity that sends participants down one of two paths in a journey.</p></li> <li><p>HOLDOUT - For a holdout activity, which is an activity that stops a journey for a specified percentage of participants.</p></li> <li><p>MESSAGE - For an email activity, which is an activity that sends an email message to participants.</p></li> <li><p>MULTI_CONDITIONAL_SPLIT - For a multivariate split activity, which is an activity that sends participants down one of as many as five paths in a journey.</p></li> <li><p>RANDOM_SPLIT - For a random split activity, which is an activity that sends specified percentages of participants down one of as many as five paths in a journey.</p></li> <li><p>WAIT - For a wait activity, which is an activity that waits for a certain amount of time or until a specific date and time before moving participants to the next activity in a journey.</p></li></ul>",
+                    "documentation": "<p>The type of activity that the metric applies to. Possible values are:</p> <ul><li><p>CONDITIONAL_SPLIT \u2013 For a yes/no split activity, which is an activity that sends participants down one of two paths in a journey.</p></li> <li><p>HOLDOUT \u2013 For a holdout activity, which is an activity that stops a journey for a specified percentage of participants.</p></li> <li><p>MESSAGE \u2013 For an email activity, which is an activity that sends an email message to participants.</p></li> <li><p>MULTI_CONDITIONAL_SPLIT \u2013 For a multivariate split activity, which is an activity that sends participants down one of as many as five paths in a journey.</p></li> <li><p>RANDOM_SPLIT \u2013 For a random split activity, which is an activity that sends specified percentages of participants down one of as many as five paths in a journey.</p></li> <li><p>WAIT \u2013 For a wait activity, which is an activity that waits for a certain amount of time or until a specific date and time before moving participants to the next activity in a journey.</p></li></ul>",
                     "shape": "__string"
                 },
                 "ApplicationId": {
                     "documentation": "<p>The unique identifier for the application that the metric applies to.</p>",
                     "shape": "__string"
                 },
                 "JourneyActivityId": {
@@ -11870,15 +12168,15 @@
                     "shape": "MapOfActivity"
                 },
                 "ApplicationId": {
                     "documentation": "<p>The unique identifier for the application that the journey applies to.</p>",
                     "shape": "__string"
                 },
                 "ClosedDays": {
-                    "documentation": "<p>The time when journey will stop sending messages. QuietTime should be configured first and SendingSchedule should be set to true.</p>",
+                    "documentation": "<p>The time when a journey will not send messages. QuietTime should be configured first and SendingSchedule should be set to true.</p>",
                     "shape": "ClosedDays"
                 },
                 "CreationDate": {
                     "documentation": "<p>The date, in ISO 8601 format, when the journey was created.</p>",
                     "shape": "__string"
                 },
                 "Id": {
@@ -11902,51 +12200,55 @@
                     "shape": "__boolean"
                 },
                 "Name": {
                     "documentation": "<p>The name of the journey.</p>",
                     "shape": "__string"
                 },
                 "OpenHours": {
-                    "documentation": "<p>The time when journey allow to send messages. QuietTime should be configured first and SendingSchedule should be set to true.</p>",
+                    "documentation": "<p>The time when a journey can send messages. QuietTime should be configured first and SendingSchedule should be set to true.</p>",
                     "shape": "OpenHours"
                 },
                 "QuietTime": {
                     "documentation": "<p>The quiet time settings for the journey. Quiet time is a specific time range when a journey doesn't send messages to participants, if all the following conditions are met:</p> <ul><li><p>The EndpointDemographic.Timezone property of the endpoint for the participant is set to a valid value.</p></li> <li><p>The current time in the participant's time zone is later than or equal to the time specified by the QuietTime.Start property for the journey.</p></li> <li><p>The current time in the participant's time zone is earlier than or equal to the time specified by the QuietTime.End property for the journey.</p></li></ul> <p>If any of the preceding conditions isn't met, the participant will receive messages from the journey, even if quiet time is enabled.</p>",
                     "shape": "QuietTime"
                 },
                 "RefreshFrequency": {
                     "documentation": "<p>The frequency with which Amazon Pinpoint evaluates segment and event data for the journey, as a duration in ISO 8601 format.</p>",
                     "shape": "__string"
                 },
                 "RefreshOnSegmentUpdate": {
-                    "documentation": "<p>Specifies whether a journey should be refreshed on segment update.</p>",
+                    "documentation": "<p>Indicates whether the journey participants should be refreshed when a segment is updated.</p>",
                     "shape": "__boolean"
                 },
                 "Schedule": {
                     "documentation": "<p>The schedule settings for the journey.</p>",
                     "shape": "JourneySchedule"
                 },
                 "SendingSchedule": {
-                    "documentation": "<p>Indicates if journey have Advance Quiet Time (OpenHours and ClosedDays). This flag should be set to true in order to allow (OpenHours and ClosedDays)</p>",
+                    "documentation": "<p>Indicates if journey has Advance Quiet Time enabled. This flag should be set to true in order to allow using OpenHours and ClosedDays.</p>",
                     "shape": "__boolean"
                 },
                 "StartActivity": {
                     "documentation": "<p>The unique identifier for the first activity in the journey.</p>",
                     "shape": "__string"
                 },
                 "StartCondition": {
                     "documentation": "<p>The segment that defines which users are participants in the journey.</p>",
                     "shape": "StartCondition"
                 },
                 "State": {
                     "documentation": "<p>The current status of the journey. Possible values are:</p> <ul><li><p>DRAFT - The journey is being developed and hasn't been published yet.</p></li> <li><p>ACTIVE - The journey has been developed and published. Depending on the journey's schedule, the journey may currently be running or scheduled to start running at a later time. If a journey's status is ACTIVE, you can't add, change, or remove activities from it.</p></li> <li><p>COMPLETED - The journey has been published and has finished running. All participants have entered the journey and no participants are waiting to complete the journey or any activities in the journey.</p></li> <li><p>CANCELLED - The journey has been stopped. If a journey's status is CANCELLED, you can't add, change, or remove activities or segment settings from the journey.</p></li> <li><p>CLOSED - The journey has been published and has started running. It may have also passed its scheduled end time, or passed its scheduled start time and a refresh frequency hasn't been specified for it. If a journey's status is CLOSED, you can't add participants to it, and no existing participants can enter the journey for the first time. However, any existing participants who are currently waiting to start an activity may continue the journey.</p></li></ul>",
                     "shape": "State"
                 },
+                "TimezoneEstimationMethods": {
+                    "documentation": "<p>An array of time zone estimation methods, if any, to use for determining an <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/apps-application-id-endpoints-endpoint-id.html\">Endpoints</a> time zone if the Endpoint does not have a value for the Demographic.Timezone attribute.</p> <ul> <li><p>PHONE_NUMBER - A time zone is determined based on the Endpoint.Address and Endpoint.Location.Country.</p></li> <li><p>POSTAL_CODE - A time zone is determined based on the Endpoint.Location.PostalCode and Endpoint.Location.Country.</p> <note><p>POSTAL_CODE detection is only supported in the United States, United Kingdom, Australia, New Zealand, Canada, France, Italy, Spain, Germany and in regions where Amazon Pinpoint is available.</p></note></li> </ul>",
+                    "shape": "ListOf__TimezoneEstimationMethodsElement"
+                },
                 "WaitForQuietTime": {
-                    "documentation": "<p>Specifies whether endpoints in quiet hours should enter a wait till the end of their quiet hours.</p>",
+                    "documentation": "<p>Indicates whether endpoints in quiet hours should enter a wait activity until quiet hours have elapsed.</p>",
                     "shape": "__boolean"
                 },
                 "tags": {
                     "documentation": "<p>This object is not used or supported.</p>",
                     "locationName": "tags",
                     "shape": "MapOf__string"
                 }
@@ -11954,14 +12256,144 @@
             "required": [
                 "Name",
                 "Id",
                 "ApplicationId"
             ],
             "type": "structure"
         },
+        "JourneyRunExecutionActivityMetricsResponse": {
+            "documentation": "<p>Provides the results of a query that retrieved the data for a standard execution metric that applies to a journey activity for a particular journey run, and provides information about that query.</p>",
+            "members": {
+                "ActivityType": {
+                    "documentation": "<p>The type of activity that the metric applies to. Possible values are:</p> <ul><li><p>CONDITIONAL_SPLIT \u2013 For a yes/no split activity, which is an activity that sends participants down one of two paths in a journey.</p></li> <li><p>HOLDOUT \u2013 For a holdout activity, which is an activity that stops a journey for a specified percentage of participants.</p></li> <li><p>MESSAGE \u2013 For an email activity, which is an activity that sends an email message to participants.</p></li> <li><p>MULTI_CONDITIONAL_SPLIT \u2013 For a multivariate split activity, which is an activity that sends participants down one of as many as five paths in a journey.</p></li> <li><p>RANDOM_SPLIT \u2013 For a random split activity, which is an activity that sends specified percentages of participants down one of as many as five paths in a journey.</p></li> <li><p>WAIT \u2013 For a wait activity, which is an activity that waits for a certain amount of time or until a specific date and time before moving participants to the next activity in a journey.</p></li></ul>",
+                    "shape": "__string"
+                },
+                "ApplicationId": {
+                    "documentation": "<p>The unique identifier for the application that the metric applies to.</p>",
+                    "shape": "__string"
+                },
+                "JourneyActivityId": {
+                    "documentation": "<p>The unique identifier for the activity that the metric applies to.</p>",
+                    "shape": "__string"
+                },
+                "JourneyId": {
+                    "documentation": "<p>The unique identifier for the journey that the metric applies to.</p>",
+                    "shape": "__string"
+                },
+                "LastEvaluatedTime": {
+                    "documentation": "<p>The date and time, in ISO 8601 format, when Amazon Pinpoint last evaluated the execution status of the activity for this journey run and updated the data for the metric.</p>",
+                    "shape": "__string"
+                },
+                "Metrics": {
+                    "documentation": "<p>A JSON object that contains the results of the query. For information about the structure and contents of the results, see see <a href=\"https://docs.aws.amazon.com//pinpoint/latest/developerguide/analytics-standard-metrics.html\">Standard Amazon Pinpoint analytics metrics</a> in the <i>Amazon Pinpoint Developer Guide</i>.</p>",
+                    "shape": "MapOf__string"
+                },
+                "RunId": {
+                    "documentation": "<p>The unique identifier for the journey run that the metric applies to.</p>",
+                    "shape": "__string"
+                }
+            },
+            "required": [
+                "Metrics",
+                "JourneyId",
+                "LastEvaluatedTime",
+                "JourneyActivityId",
+                "ActivityType",
+                "RunId",
+                "ApplicationId"
+            ],
+            "type": "structure"
+        },
+        "JourneyRunExecutionMetricsResponse": {
+            "documentation": "<p>Provides the results of a query that retrieved the data for a standard execution metric that applies to a journey run, and provides information about that query.</p>",
+            "members": {
+                "ApplicationId": {
+                    "documentation": "<p>The unique identifier for the application that the metric applies to.</p>",
+                    "shape": "__string"
+                },
+                "JourneyId": {
+                    "documentation": "<p>The unique identifier for the journey that the metric applies to.</p>",
+                    "shape": "__string"
+                },
+                "LastEvaluatedTime": {
+                    "documentation": "<p>The date and time, in ISO 8601 format, when Amazon Pinpoint last evaluated the journey run and updated the data for the metric.</p>",
+                    "shape": "__string"
+                },
+                "Metrics": {
+                    "documentation": "<p>A JSON object that contains the results of the query. For information about the structure and contents of the results, see the <a href=\"https://docs.aws.amazon.com//pinpoint/latest/developerguide/analytics-standard-metrics.html\">Standard Amazon Pinpoint analytics metrics</a> in the <i>Amazon Pinpoint Developer Guide</i>.</p>",
+                    "shape": "MapOf__string"
+                },
+                "RunId": {
+                    "documentation": "<p>The unique identifier for the journey run that the metric applies to.</p>",
+                    "shape": "__string"
+                }
+            },
+            "required": [
+                "Metrics",
+                "JourneyId",
+                "LastEvaluatedTime",
+                "RunId",
+                "ApplicationId"
+            ],
+            "type": "structure"
+        },
+        "JourneyRunResponse": {
+            "documentation": "<p>Provides information from a specified run of a journey.</p>",
+            "members": {
+                "CreationTime": {
+                    "documentation": "<p>The time when the journey run was created or scheduled, in ISO 8601 format.</p>",
+                    "shape": "__string"
+                },
+                "LastUpdateTime": {
+                    "documentation": "<p>The last time the journey run was updated, in ISO 8601 format..</p>",
+                    "shape": "__string"
+                },
+                "RunId": {
+                    "documentation": "<p>The unique identifier for the run.</p>",
+                    "shape": "__string"
+                },
+                "Status": {
+                    "documentation": "<p>The current status of the journey run.</p>",
+                    "shape": "JourneyRunStatus"
+                }
+            },
+            "required": [
+                "Status",
+                "LastUpdateTime",
+                "CreationTime",
+                "RunId"
+            ],
+            "type": "structure"
+        },
+        "JourneyRunStatus": {
+            "enum": [
+                "SCHEDULED",
+                "RUNNING",
+                "COMPLETED",
+                "CANCELLED"
+            ],
+            "type": "string"
+        },
+        "JourneyRunsResponse": {
+            "documentation": "<p>Provides information from all runs of a journey.</p>",
+            "members": {
+                "Item": {
+                    "documentation": "<p>An array of responses, one for each run of the journey</p>",
+                    "shape": "ListOfJourneyRunResponse"
+                },
+                "NextToken": {
+                    "documentation": "<p>The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.</p>",
+                    "shape": "__string"
+                }
+            },
+            "required": [
+                "Item"
+            ],
+            "type": "structure"
+        },
         "JourneySMSMessage": {
             "documentation": "<p>Specifies the sender ID and message type for an SMS message that's sent to participants in a journey.</p>",
             "members": {
                 "EntityId": {
                     "documentation": "<p>The entity ID or Principal Entity (PE) id received from the regulatory body for sending SMS in your country.</p>",
                     "shape": "__string"
                 },
@@ -12141,14 +12573,20 @@
         },
         "ListOfJourneyResponse": {
             "member": {
                 "shape": "JourneyResponse"
             },
             "type": "list"
         },
+        "ListOfJourneyRunResponse": {
+            "member": {
+                "shape": "JourneyRunResponse"
+            },
+            "type": "list"
+        },
         "ListOfMultiConditionalBranch": {
             "member": {
                 "shape": "MultiConditionalBranch"
             },
             "type": "list"
         },
         "ListOfOpenHoursRules": {
@@ -12238,14 +12676,20 @@
         },
         "ListOf__EndpointTypesElement": {
             "member": {
                 "shape": "__EndpointTypesElement"
             },
             "type": "list"
         },
+        "ListOf__TimezoneEstimationMethodsElement": {
+            "member": {
+                "shape": "__TimezoneEstimationMethodsElement"
+            },
+            "type": "list"
+        },
         "ListOf__string": {
             "member": {
                 "shape": "__string"
             },
             "type": "list"
         },
         "ListRecommenderConfigurationsResponse": {
@@ -12912,48 +13356,48 @@
                     "documentation": "<p>The postal or ZIP code for the location where the phone number was originally registered.</p>",
                     "shape": "__string"
                 }
             },
             "type": "structure"
         },
         "OpenHours": {
-            "documentation": "<p>The time when journey allow to send messages. QuietTime should be configured first and SendingSchedule should be set to true.</p>",
+            "documentation": "<p>Specifies the times when message are allowed to be sent to endpoints.</p>",
             "members": {
                 "CUSTOM": {
-                    "documentation": "<p>Rules for Custom Channel.</p>",
+                    "documentation": "<p>Specifies the schedule settings for the custom channel.</p>",
                     "shape": "MapOfListOfOpenHoursRules"
                 },
                 "EMAIL": {
-                    "documentation": "<p>Rules for Email Channel.</p>",
+                    "documentation": "<p>Specifies the schedule settings for the email channel.</p>",
                     "shape": "MapOfListOfOpenHoursRules"
                 },
                 "PUSH": {
-                    "documentation": "<p>Rules for Push Channel.</p>",
+                    "documentation": "<p>Specifies the schedule settings for the push channel.</p>",
                     "shape": "MapOfListOfOpenHoursRules"
                 },
                 "SMS": {
-                    "documentation": "<p>Rules for SMS Channel.</p>",
+                    "documentation": "<p>Specifies the schedule settings for the SMS channel.</p>",
                     "shape": "MapOfListOfOpenHoursRules"
                 },
                 "VOICE": {
-                    "documentation": "<p>Rules for Voice Channel.</p>",
+                    "documentation": "<p>Specifies the schedule settings for the voice channel.</p>",
                     "shape": "MapOfListOfOpenHoursRules"
                 }
             },
             "type": "structure"
         },
         "OpenHoursRule": {
-            "documentation": "<p>List of OpenHours Rules.</p>",
+            "documentation": "<p>Specifies the start and end time for OpenHours.</p>",
             "members": {
                 "EndTime": {
-                    "documentation": "<p>Local start time in ISO 8601 format.</p>",
+                    "documentation": "<p>The end of the scheduled time, in ISO 8601 format, when the channel can't send messages.</p>",
                     "shape": "__string"
                 },
                 "StartTime": {
-                    "documentation": "<p>Local start time in ISO 8601 format.</p>",
+                    "documentation": "<p>The start of the scheduled time, in ISO 8601 format, when the channel can send messages.</p>",
                     "shape": "__string"
                 }
             },
             "type": "structure"
         },
         "Operator": {
             "enum": [
@@ -13125,15 +13569,15 @@
                     "shape": "__string"
                 },
                 "TemplateDescription": {
                     "documentation": "<p>A custom description of the message template.</p>",
                     "shape": "__string"
                 },
                 "tags": {
-                    "documentation": "<p>A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
+                    "documentation": "<note><p>As of <b>22-05-2023</b> tags has been deprecated for update operations. After this date any value in tags is not processed and an error code is not returned. To manage tags we recommend using either <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/tags-resource-arn.html\">Tags</a> in the <i>API Reference for Amazon Pinpoint</i>, <a href=\"https://docs.aws.amazon.com/cli/latest/reference/resourcegroupstaggingapi/index.html\">resourcegroupstaggingapi</a> commands in the <i>AWS Command Line Interface Documentation</i> or <a href=\"https://sdk.amazonaws.com/java/api/latest/software/amazon/awssdk/services/resourcegroupstaggingapi/package-summary.html\">resourcegroupstaggingapi</a> in the <i>AWS SDK</i>.</p></note> <p>(Deprecated) A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
                     "locationName": "tags",
                     "shape": "MapOf__string"
                 }
             },
             "type": "structure"
         },
         "PushNotificationTemplateResponse": {
@@ -13647,15 +14091,15 @@
                     "shape": "__string"
                 },
                 "TemplateDescription": {
                     "documentation": "<p>A custom description of the message template.</p>",
                     "shape": "__string"
                 },
                 "tags": {
-                    "documentation": "<p>A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
+                    "documentation": "<note><p>As of <b>22-05-2023</b> tags has been deprecated for update operations. After this date any value in tags is not processed and an error code is not returned. To manage tags we recommend using either <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/tags-resource-arn.html\">Tags</a> in the <i>API Reference for Amazon Pinpoint</i>, <a href=\"https://docs.aws.amazon.com/cli/latest/reference/resourcegroupstaggingapi/index.html\">resourcegroupstaggingapi</a> commands in the <i>AWS Command Line Interface Documentation</i> or <a href=\"https://sdk.amazonaws.com/java/api/latest/software/amazon/awssdk/services/resourcegroupstaggingapi/package-summary.html\">resourcegroupstaggingapi</a> in the <i>AWS SDK</i>.</p></note> <p>(Deprecated) A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
                     "locationName": "tags",
                     "shape": "MapOf__string"
                 }
             },
             "type": "structure"
         },
         "SMSTemplateResponse": {
@@ -15758,15 +16202,15 @@
                     "shape": "__string"
                 },
                 "VoiceId": {
                     "documentation": "<p>The name of the voice to use when delivering messages that are based on the message template. For a list of supported voices, see the <a href=\"https://docs.aws.amazon.com/polly/latest/dg/what-is.html\">Amazon Polly Developer Guide</a>.</p>",
                     "shape": "__string"
                 },
                 "tags": {
-                    "documentation": "<p>A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
+                    "documentation": "<note><p>As of <b>22-05-2023</b> tags has been deprecated for update operations. After this date any value in tags is not processed and an error code is not returned. To manage tags we recommend using either <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/tags-resource-arn.html\">Tags</a> in the <i>API Reference for Amazon Pinpoint</i>, <a href=\"https://docs.aws.amazon.com/cli/latest/reference/resourcegroupstaggingapi/index.html\">resourcegroupstaggingapi</a> commands in the <i>AWS Command Line Interface Documentation</i> or <a href=\"https://sdk.amazonaws.com/java/api/latest/software/amazon/awssdk/services/resourcegroupstaggingapi/package-summary.html\">resourcegroupstaggingapi</a> in the <i>AWS SDK</i>.</p></note> <p>(Deprecated) A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.</p>",
                     "locationName": "tags",
                     "shape": "MapOf__string"
                 }
             },
             "type": "structure"
         },
         "VoiceTemplateResponse": {
@@ -15947,15 +16391,15 @@
                     "shape": "__string"
                 },
                 "TreatmentName": {
                     "documentation": "<p>A custom name of the default treatment for the campaign, if the campaign has multiple treatments. A <i>treatment</i> is a variation of a campaign that's used for A/B testing.</p>",
                     "shape": "__string"
                 },
                 "tags": {
-                    "documentation": "<p>A string-to-string map of key-value pairs that defines the tags to associate with the campaign. Each tag consists of a required tag key and an associated tag value.</p>",
+                    "documentation": "<note><p>As of <b>22-05-2023</b> tags has been deprecated for update operations. After this date any value in tags is not processed and an error code is not returned. To manage tags we recommend using either <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/tags-resource-arn.html\">Tags</a> in the <i>API Reference for Amazon Pinpoint</i>, <a href=\"https://docs.aws.amazon.com/cli/latest/reference/resourcegroupstaggingapi/index.html\">resourcegroupstaggingapi</a> commands in the <i>AWS Command Line Interface Documentation</i> or <a href=\"https://sdk.amazonaws.com/java/api/latest/software/amazon/awssdk/services/resourcegroupstaggingapi/package-summary.html\">resourcegroupstaggingapi</a> in the <i>AWS SDK</i>.</p></note> <p>(Deprecated) A string-to-string map of key-value pairs that defines the tags to associate with the campaign. Each tag consists of a required tag key and an associated tag value.</p>",
                     "locationName": "tags",
                     "shape": "MapOf__string"
                 }
             },
             "type": "structure"
         },
         "WriteEventStream": {
@@ -16020,37 +16464,41 @@
                     "shape": "QuietTime"
                 },
                 "RefreshFrequency": {
                     "documentation": "<p>The frequency with which Amazon Pinpoint evaluates segment and event data for the journey, as a duration in ISO 8601 format.</p>",
                     "shape": "__string"
                 },
                 "RefreshOnSegmentUpdate": {
-                    "documentation": "<p>Specifies whether a journey should be refreshed on segment update.</p>",
+                    "documentation": "<p>Indicates whether the journey participants should be refreshed when a segment is updated.</p>",
                     "shape": "__boolean"
                 },
                 "Schedule": {
                     "documentation": "<p>The schedule settings for the journey.</p>",
                     "shape": "JourneySchedule"
                 },
                 "SendingSchedule": {
-                    "documentation": "<p>Indicates if journey have Advance Quiet Time (OpenHours and ClosedDays). This flag should be set to true in order to allow (OpenHours and ClosedDays)</p>",
+                    "documentation": "<p>Indicates if journey has Advance Quiet Time enabled. This flag should be set to true in order to allow using OpenHours and ClosedDays.</p>",
                     "shape": "__boolean"
                 },
                 "StartActivity": {
                     "documentation": "<p>The unique identifier for the first activity in the journey. The identifier for this activity can contain a maximum of 128 characters. The characters must be alphanumeric characters.</p>",
                     "shape": "__string"
                 },
                 "StartCondition": {
                     "documentation": "<p>The segment that defines which users are participants in the journey.</p>",
                     "shape": "StartCondition"
                 },
                 "State": {
                     "documentation": "<p>The status of the journey. Valid values are:</p> <ul><li><p>DRAFT - Saves the journey and doesn't publish it.</p></li> <li><p>ACTIVE - Saves and publishes the journey. Depending on the journey's schedule, the journey starts running immediately or at the scheduled start time. If a journey's status is ACTIVE, you can't add, change, or remove activities from it.</p></li></ul> <p>PAUSED, CANCELLED, COMPLETED, and CLOSED states are not supported in requests to create or update a journey. To cancel, pause, or resume a journey, use the <link  linkend=\"apps-application-id-journeys-journey-id-state\">Journey State</link> resource.</p>",
                     "shape": "State"
                 },
+                "TimezoneEstimationMethods": {
+                    "documentation": "<p>An array of time zone estimation methods, if any, to use for determining an <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/apps-application-id-endpoints-endpoint-id.html\">Endpoints</a> time zone if the Endpoint does not have a value for the Demographic.Timezone attribute.</p> <ul> <li><p>PHONE_NUMBER - A time zone is determined based on the Endpoint.Address and Endpoint.Location.Country.</p></li> <li><p>POSTAL_CODE - A time zone is determined based on the Endpoint.Location.PostalCode and Endpoint.Location.Country.</p> <note><p>POSTAL_CODE detection is only supported in the United States, United Kingdom, Australia, New Zealand, Canada, France, Italy, Spain, Germany and in regions where Amazon Pinpoint is available.</p></note></li> </ul>",
+                    "shape": "ListOf__TimezoneEstimationMethodsElement"
+                },
                 "WaitForQuietTime": {
                     "documentation": "<p>Specifies whether endpoints in quiet hours should enter a wait till the end of their quiet hours.</p>",
                     "shape": "__boolean"
                 }
             },
             "required": [
                 "Name"
@@ -16069,15 +16517,15 @@
                     "shape": "__string"
                 },
                 "SegmentGroups": {
                     "documentation": "<p>The segment group to use and the dimensions to apply to the group's base segments in order to build the segment. A segment group can consist of zero or more base segments. Your request can include only one segment group.</p>",
                     "shape": "SegmentGroupList"
                 },
                 "tags": {
-                    "documentation": "<p>A string-to-string map of key-value pairs that defines the tags to associate with the segment. Each tag consists of a required tag key and an associated tag value.</p>",
+                    "documentation": "<note><p>As of <b>22-05-2023</b> tags has been deprecated for update operations. After this date any value in tags is not processed and an error code is not returned. To manage tags we recommend using either <a href=\"https://docs.aws.amazon.com/pinpoint/latest/apireference/tags-resource-arn.html\">Tags</a> in the <i>API Reference for Amazon Pinpoint</i>, <a href=\"https://docs.aws.amazon.com/cli/latest/reference/resourcegroupstaggingapi/index.html\">resourcegroupstaggingapi</a> commands in the <i>AWS Command Line Interface Documentation</i> or <a href=\"https://sdk.amazonaws.com/java/api/latest/software/amazon/awssdk/services/resourcegroupstaggingapi/package-summary.html\">resourcegroupstaggingapi</a> in the <i>AWS SDK</i>.</p></note> <p>(Deprecated) A string-to-string map of key-value pairs that defines the tags to associate with the segment. Each tag consists of a required tag key and an associated tag value.</p>",
                     "locationName": "tags",
                     "shape": "MapOf__string"
                 }
             },
             "type": "structure"
         },
         "WriteTreatmentResource": {
@@ -16131,14 +16579,21 @@
                 "EMAIL",
                 "BAIDU",
                 "CUSTOM",
                 "IN_APP"
             ],
             "type": "string"
         },
+        "__TimezoneEstimationMethodsElement": {
+            "enum": [
+                "PHONE_NUMBER",
+                "POSTAL_CODE"
+            ],
+            "type": "string"
+        },
         "__blob": {
             "type": "blob"
         },
         "__boolean": {
             "type": "boolean"
         },
         "__double": {
```

### Comparing `botocore-a-la-carte-pinpoint-1.29.99/botocore_a_la_carte_pinpoint.egg-info/PKG-INFO` & `botocore-a-la-carte-pinpoint-1.30.0/botocore_a_la_carte_pinpoint.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-pinpoint
-Version: 1.29.99
+Version: 1.30.0
 Summary: pinpoint data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-pinpoint-1.29.99/setup.py` & `botocore-a-la-carte-pinpoint-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-pinpoint',
-    version="1.29.99",
+    version="1.30.0",
     description='pinpoint data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/pinpoint/*/*.json'],
```

