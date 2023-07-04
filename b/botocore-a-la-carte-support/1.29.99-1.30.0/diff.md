# Comparing `tmp/botocore-a-la-carte-support-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-support-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-support-1.29.99.tar", last modified: Sat Mar 25 01:23:09 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-support-1.30.0.tar", last modified: Tue Jul  4 01:45:01 2023, max compression
```

## Comparing `botocore-a-la-carte-support-1.29.99.tar` & `botocore-a-la-carte-support-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:09.833154 botocore-a-la-carte-support-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:09.000000 botocore-a-la-carte-support-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-25 01:23:09.833154 botocore-a-la-carte-support-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:09.829154 botocore-a-la-carte-support-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:09.829154 botocore-a-la-carte-support-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:09.829154 botocore-a-la-carte-support-1.29.99/botocore/data/support/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:09.829154 botocore-a-la-carte-support-1.29.99/botocore/data/support/2013-04-15/
--rw-r--r--   0 runner    (1001) docker     (123)    60899 2023-03-25 01:22:12.000000 botocore-a-la-carte-support-1.29.99/botocore/data/support/2013-04-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-support-1.29.99/botocore/data/support/2013-04-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-25 01:22:12.000000 botocore-a-la-carte-support-1.29.99/botocore/data/support/2013-04-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    75209 2023-03-25 01:22:12.000000 botocore-a-la-carte-support-1.29.99/botocore/data/support/2013-04-15/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:09.829154 botocore-a-la-carte-support-1.29.99/botocore_a_la_carte_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-25 01:23:09.000000 botocore-a-la-carte-support-1.29.99/botocore_a_la_carte_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-25 01:23:09.000000 botocore-a-la-carte-support-1.29.99/botocore_a_la_carte_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:09.000000 botocore-a-la-carte-support-1.29.99/botocore_a_la_carte_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:09.000000 botocore-a-la-carte-support-1.29.99/botocore_a_la_carte_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:09.833154 botocore-a-la-carte-support-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-25 01:23:09.000000 botocore-a-la-carte-support-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.690843 botocore-a-la-carte-support-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:01.000000 botocore-a-la-carte-support-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-04 01:45:01.690843 botocore-a-la-carte-support-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.690843 botocore-a-la-carte-support-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.690843 botocore-a-la-carte-support-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.690843 botocore-a-la-carte-support-1.30.0/botocore/data/support/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.690843 botocore-a-la-carte-support-1.30.0/botocore/data/support/2013-04-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-07-04 01:44:02.000000 botocore-a-la-carte-support-1.30.0/botocore/data/support/2013-04-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-support-1.30.0/botocore/data/support/2013-04-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 01:44:02.000000 botocore-a-la-carte-support-1.30.0/botocore/data/support/2013-04-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    86587 2023-07-04 01:44:02.000000 botocore-a-la-carte-support-1.30.0/botocore/data/support/2013-04-15/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.690843 botocore-a-la-carte-support-1.30.0/botocore_a_la_carte_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-04 01:45:01.000000 botocore-a-la-carte-support-1.30.0/botocore_a_la_carte_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 01:45:01.000000 botocore-a-la-carte-support-1.30.0/botocore_a_la_carte_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:01.000000 botocore-a-la-carte-support-1.30.0/botocore_a_la_carte_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:01.000000 botocore-a-la-carte-support-1.30.0/botocore_a_la_carte_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:01.690843 botocore-a-la-carte-support-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 01:45:01.000000 botocore-a-la-carte-support-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-support-1.29.99/LICENSE.txt` & `botocore-a-la-carte-support-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-support-1.29.99/PKG-INFO` & `botocore-a-la-carte-support-1.30.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-support
-Version: 1.29.99
+Version: 1.30.0
 Summary: support data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-support-1.29.99/botocore/data/support/2013-04-15/service-2.json` & `botocore-a-la-carte-support-1.30.0/botocore/data/support/2013-04-15/service-2.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9673583080150461%*

 * *Differences: {"'operations'": "{'DescribeTrustedAdvisorCheckRefreshStatuses': {'errors': {insert: [(1, "*

 * *                 "OrderedDict([('shape', 'ThrottlingException')]))]}}, "*

 * *                 "'DescribeTrustedAdvisorCheckResult': {'errors': {insert: [(1, "*

 * *                 "OrderedDict([('shape', 'ThrottlingException')]))]}}, "*

 * *                 "'DescribeTrustedAdvisorCheckSummaries': {'errors': {insert: [(1, "*

 * *                 "OrderedDict([('shape', 'ThrottlingException')]))]}}, "*

 * *                 "'DescribeTrusted […]*

```diff
@@ -164,14 +164,36 @@
                 "shape": "DescribeCommunicationsRequest"
             },
             "name": "DescribeCommunications",
             "output": {
                 "shape": "DescribeCommunicationsResponse"
             }
         },
+        "DescribeCreateCaseOptions": {
+            "documentation": "<p>Returns a list of CreateCaseOption types along with the corresponding supported hours and language availability. You can specify the <code>language</code> <code>categoryCode</code>, <code>issueType</code> and <code>serviceCode</code> used to retrieve the CreateCaseOptions.</p> <note> <ul> <li> <p>You must have a Business, Enterprise On-Ramp, or Enterprise Support plan to use the Amazon Web Services Support API. </p> </li> <li> <p>If you call the Amazon Web Services Support API from an account that doesn't have a Business, Enterprise On-Ramp, or Enterprise Support plan, the <code>SubscriptionRequiredException</code> error message appears. For information about changing your support plan, see <a href=\"http://aws.amazon.com/premiumsupport/\">Amazon Web Services Support</a>.</p> </li> </ul> </note>",
+            "errors": [
+                {
+                    "shape": "InternalServerError"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DescribeCreateCaseOptionsRequest"
+            },
+            "name": "DescribeCreateCaseOptions",
+            "output": {
+                "shape": "DescribeCreateCaseOptionsResponse"
+            }
+        },
         "DescribeServices": {
             "documentation": "<p>Returns the current list of Amazon Web Services services and a list of service categories for each service. You then use service names and categories in your <a>CreateCase</a> requests. Each Amazon Web Services service has its own set of categories.</p> <p>The service codes and category codes correspond to the values that appear in the <b>Service</b> and <b>Category</b> lists on the Amazon Web Services Support Center <a href=\"https://console.aws.amazon.com/support/home#/case/create\">Create Case</a> page. The values in those fields don't necessarily match the service codes and categories returned by the <code>DescribeServices</code> operation. Always use the service codes and categories that the <code>DescribeServices</code> operation returns, so that you have the most recent set of service and category codes.</p> <note> <ul> <li> <p>You must have a Business, Enterprise On-Ramp, or Enterprise Support plan to use the Amazon Web Services Support API. </p> </li> <li> <p>If you call the Amazon Web Services Support API from an account that doesn't have a Business, Enterprise On-Ramp, or Enterprise Support plan, the <code>SubscriptionRequiredException</code> error message appears. For information about changing your support plan, see <a href=\"http://aws.amazon.com/premiumsupport/\">Amazon Web Services Support</a>.</p> </li> </ul> </note>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 }
             ],
@@ -202,19 +224,44 @@
                 "shape": "DescribeSeverityLevelsRequest"
             },
             "name": "DescribeSeverityLevels",
             "output": {
                 "shape": "DescribeSeverityLevelsResponse"
             }
         },
+        "DescribeSupportedLanguages": {
+            "documentation": "<p>Returns a list of supported languages for a specified <code>categoryCode</code>, <code>issueType</code> and <code>serviceCode</code>. The returned supported languages will include a ISO 639-1 code for the <code>language</code>, and the language display name.</p> <note> <ul> <li> <p>You must have a Business, Enterprise On-Ramp, or Enterprise Support plan to use the Amazon Web Services Support API. </p> </li> <li> <p>If you call the Amazon Web Services Support API from an account that doesn't have a Business, Enterprise On-Ramp, or Enterprise Support plan, the <code>SubscriptionRequiredException</code> error message appears. For information about changing your support plan, see <a href=\"http://aws.amazon.com/premiumsupport/\">Amazon Web Services Support</a>.</p> </li> </ul> </note>",
+            "errors": [
+                {
+                    "shape": "InternalServerError"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DescribeSupportedLanguagesRequest"
+            },
+            "name": "DescribeSupportedLanguages",
+            "output": {
+                "shape": "DescribeSupportedLanguagesResponse"
+            }
+        },
         "DescribeTrustedAdvisorCheckRefreshStatuses": {
             "documentation": "<p>Returns the refresh status of the Trusted Advisor checks that have the specified check IDs. You can get the check IDs by calling the <a>DescribeTrustedAdvisorChecks</a> operation.</p> <p>Some checks are refreshed automatically, and you can't return their refresh statuses by using the <code>DescribeTrustedAdvisorCheckRefreshStatuses</code> operation. If you call this operation for these checks, you might see an <code>InvalidParameterValue</code> error.</p> <note> <ul> <li> <p>You must have a Business, Enterprise On-Ramp, or Enterprise Support plan to use the Amazon Web Services Support API. </p> </li> <li> <p>If you call the Amazon Web Services Support API from an account that doesn't have a Business, Enterprise On-Ramp, or Enterprise Support plan, the <code>SubscriptionRequiredException</code> error message appears. For information about changing your support plan, see <a href=\"http://aws.amazon.com/premiumsupport/\">Amazon Web Services Support</a>.</p> </li> </ul> </note> <p>To call the Trusted Advisor operations in the Amazon Web Services Support API, you must use the US East (N. Virginia) endpoint. Currently, the US West (Oregon) and Europe (Ireland) endpoints don't support the Trusted Advisor operations. For more information, see <a href=\"https://docs.aws.amazon.com/awssupport/latest/user/about-support-api.html#endpoint\">About the Amazon Web Services Support API</a> in the <i>Amazon Web Services Support User Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
+                },
+                {
+                    "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -226,14 +273,17 @@
             }
         },
         "DescribeTrustedAdvisorCheckResult": {
             "documentation": "<p>Returns the results of the Trusted Advisor check that has the specified check ID. You can get the check IDs by calling the <a>DescribeTrustedAdvisorChecks</a> operation.</p> <p>The response contains a <a>TrustedAdvisorCheckResult</a> object, which contains these three objects:</p> <ul> <li> <p> <a>TrustedAdvisorCategorySpecificSummary</a> </p> </li> <li> <p> <a>TrustedAdvisorResourceDetail</a> </p> </li> <li> <p> <a>TrustedAdvisorResourcesSummary</a> </p> </li> </ul> <p>In addition, the response contains these fields:</p> <ul> <li> <p> <b>status</b> - The alert status of the check can be <code>ok</code> (green), <code>warning</code> (yellow), <code>error</code> (red), or <code>not_available</code>.</p> </li> <li> <p> <b>timestamp</b> - The time of the last refresh of the check.</p> </li> <li> <p> <b>checkId</b> - The unique identifier for the check.</p> </li> </ul> <note> <ul> <li> <p>You must have a Business, Enterprise On-Ramp, or Enterprise Support plan to use the Amazon Web Services Support API. </p> </li> <li> <p>If you call the Amazon Web Services Support API from an account that doesn't have a Business, Enterprise On-Ramp, or Enterprise Support plan, the <code>SubscriptionRequiredException</code> error message appears. For information about changing your support plan, see <a href=\"http://aws.amazon.com/premiumsupport/\">Amazon Web Services Support</a>.</p> </li> </ul> </note> <p>To call the Trusted Advisor operations in the Amazon Web Services Support API, you must use the US East (N. Virginia) endpoint. Currently, the US West (Oregon) and Europe (Ireland) endpoints don't support the Trusted Advisor operations. For more information, see <a href=\"https://docs.aws.amazon.com/awssupport/latest/user/about-support-api.html#endpoint\">About the Amazon Web Services Support API</a> in the <i>Amazon Web Services Support User Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
+                },
+                {
+                    "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -245,14 +295,17 @@
             }
         },
         "DescribeTrustedAdvisorCheckSummaries": {
             "documentation": "<p>Returns the results for the Trusted Advisor check summaries for the check IDs that you specified. You can get the check IDs by calling the <a>DescribeTrustedAdvisorChecks</a> operation.</p> <p>The response contains an array of <a>TrustedAdvisorCheckSummary</a> objects.</p> <note> <ul> <li> <p>You must have a Business, Enterprise On-Ramp, or Enterprise Support plan to use the Amazon Web Services Support API. </p> </li> <li> <p>If you call the Amazon Web Services Support API from an account that doesn't have a Business, Enterprise On-Ramp, or Enterprise Support plan, the <code>SubscriptionRequiredException</code> error message appears. For information about changing your support plan, see <a href=\"http://aws.amazon.com/premiumsupport/\">Amazon Web Services Support</a>.</p> </li> </ul> </note> <p>To call the Trusted Advisor operations in the Amazon Web Services Support API, you must use the US East (N. Virginia) endpoint. Currently, the US West (Oregon) and Europe (Ireland) endpoints don't support the Trusted Advisor operations. For more information, see <a href=\"https://docs.aws.amazon.com/awssupport/latest/user/about-support-api.html#endpoint\">About the Amazon Web Services Support API</a> in the <i>Amazon Web Services Support User Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
+                },
+                {
+                    "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -264,14 +317,17 @@
             }
         },
         "DescribeTrustedAdvisorChecks": {
             "documentation": "<p>Returns information about all available Trusted Advisor checks, including the name, ID, category, description, and metadata. You must specify a language code.</p> <p>The response contains a <a>TrustedAdvisorCheckDescription</a> object for each check. You must set the Amazon Web Services Region to us-east-1.</p> <note> <ul> <li> <p>You must have a Business, Enterprise On-Ramp, or Enterprise Support plan to use the Amazon Web Services Support API. </p> </li> <li> <p>If you call the Amazon Web Services Support API from an account that doesn't have a Business, Enterprise On-Ramp, or Enterprise Support plan, the <code>SubscriptionRequiredException</code> error message appears. For information about changing your support plan, see <a href=\"http://aws.amazon.com/premiumsupport/\">Amazon Web Services Support</a>.</p> </li> <li> <p>The names and descriptions for Trusted Advisor checks are subject to change. We recommend that you specify the check ID in your code to uniquely identify a check.</p> </li> </ul> </note> <p>To call the Trusted Advisor operations in the Amazon Web Services Support API, you must use the US East (N. Virginia) endpoint. Currently, the US West (Oregon) and Europe (Ireland) endpoints don't support the Trusted Advisor operations. For more information, see <a href=\"https://docs.aws.amazon.com/awssupport/latest/user/about-support-api.html#endpoint\">About the Amazon Web Services Support API</a> in the <i>Amazon Web Services Support User Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
+                },
+                {
+                    "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -489,14 +545,17 @@
         },
         "Attachments": {
             "member": {
                 "shape": "Attachment"
             },
             "type": "list"
         },
+        "AvailabilityErrorMessage": {
+            "type": "string"
+        },
         "BeforeTime": {
             "type": "string"
         },
         "Boolean": {
             "type": "boolean"
         },
         "CaseCreationLimitExceeded": {
@@ -507,15 +566,15 @@
                     "documentation": "<p>An error message that indicates that you have exceeded the number of cases you can have open.</p>",
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
         },
         "CaseDetails": {
-            "documentation": "<p>A JSON-formatted object that contains the metadata for a support case. It is contained in the response from a <a>DescribeCases</a> request. <b>CaseDetails</b> contains the following fields:</p> <ul> <li> <p> <b>caseId</b> - The support case ID requested or returned in the call. The case ID is an alphanumeric string formatted as shown in this example: case-<i>12345678910-2013-c4c1d2bf33c5cf47</i>.</p> </li> <li> <p> <b>categoryCode</b> - The category of problem for the support case. Corresponds to the <code>CategoryCode</code> values returned by a call to <a>DescribeServices</a>.</p> </li> <li> <p> <b>displayId</b> - The identifier for the case on pages in the Amazon Web Services Support Center.</p> </li> <li> <p> <b>language</b> - The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports English (\"en\") and Japanese (\"ja\"). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p> </li> <li> <p> <b>nextToken</b> - A resumption point for pagination.</p> </li> <li> <p> <b>recentCommunications</b> - One or more <a>Communication</a> objects. Fields of these objects are <code>attachments</code>, <code>body</code>, <code>caseId</code>, <code>submittedBy</code>, and <code>timeCreated</code>.</p> </li> <li> <p> <b>serviceCode</b> - The identifier for the Amazon Web Services service that corresponds to the service code defined in the call to <a>DescribeServices</a>.</p> </li> <li> <p> <b>severityCode</b> - The severity code assigned to the case. Contains one of the values returned by the call to <a>DescribeSeverityLevels</a>. The possible values are: <code>low</code>, <code>normal</code>, <code>high</code>, <code>urgent</code>, and <code>critical</code>.</p> </li> <li> <p> <b>status</b> - The status of the case in the Amazon Web Services Support Center. Valid values:</p> <ul> <li> <p> <code>opened</code> </p> </li> <li> <p> <code>pending-customer-action</code> </p> </li> <li> <p> <code>reopened</code> </p> </li> <li> <p> <code>resolved</code> </p> </li> <li> <p> <code>unassigned</code> </p> </li> <li> <p> <code>work-in-progress</code> </p> </li> </ul> </li> <li> <p> <b>subject</b> - The subject line of the case.</p> </li> <li> <p> <b>submittedBy</b> - The email address of the account that submitted the case.</p> </li> <li> <p> <b>timeCreated</b> - The time the case was created, in ISO-8601 format.</p> </li> </ul>",
+            "documentation": "<p>A JSON-formatted object that contains the metadata for a support case. It is contained in the response from a <a>DescribeCases</a> request. <b>CaseDetails</b> contains the following fields:</p> <ul> <li> <p> <b>caseId</b> - The support case ID requested or returned in the call. The case ID is an alphanumeric string formatted as shown in this example: case-<i>12345678910-2013-c4c1d2bf33c5cf47</i>.</p> </li> <li> <p> <b>categoryCode</b> - The category of problem for the support case. Corresponds to the <code>CategoryCode</code> values returned by a call to <a>DescribeServices</a>.</p> </li> <li> <p> <b>displayId</b> - The identifier for the case on pages in the Amazon Web Services Support Center.</p> </li> <li> <p> <b>language</b> - The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports Chinese (\u201czh\u201d), English (\"en\"), Japanese (\"ja\") and Korean (\u201cko\u201d). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p> </li> <li> <p> <b>nextToken</b> - A resumption point for pagination.</p> </li> <li> <p> <b>recentCommunications</b> - One or more <a>Communication</a> objects. Fields of these objects are <code>attachments</code>, <code>body</code>, <code>caseId</code>, <code>submittedBy</code>, and <code>timeCreated</code>.</p> </li> <li> <p> <b>serviceCode</b> - The identifier for the Amazon Web Services service that corresponds to the service code defined in the call to <a>DescribeServices</a>.</p> </li> <li> <p> <b>severityCode</b> - The severity code assigned to the case. Contains one of the values returned by the call to <a>DescribeSeverityLevels</a>. The possible values are: <code>low</code>, <code>normal</code>, <code>high</code>, <code>urgent</code>, and <code>critical</code>.</p> </li> <li> <p> <b>status</b> - The status of the case in the Amazon Web Services Support Center. Valid values:</p> <ul> <li> <p> <code>opened</code> </p> </li> <li> <p> <code>pending-customer-action</code> </p> </li> <li> <p> <code>reopened</code> </p> </li> <li> <p> <code>resolved</code> </p> </li> <li> <p> <code>unassigned</code> </p> </li> <li> <p> <code>work-in-progress</code> </p> </li> </ul> </li> <li> <p> <b>subject</b> - The subject line of the case.</p> </li> <li> <p> <b>submittedBy</b> - The email address of the account that submitted the case.</p> </li> <li> <p> <b>timeCreated</b> - The time the case was created, in ISO-8601 format.</p> </li> </ul>",
             "members": {
                 "caseId": {
                     "documentation": "<p>The support case ID requested or returned in the call. The case ID is an alphanumeric string formatted as shown in this example: case-<i>12345678910-2013-c4c1d2bf33c5cf47</i> </p>",
                     "shape": "CaseId"
                 },
                 "categoryCode": {
                     "documentation": "<p>The category of problem for the support case.</p>",
@@ -526,15 +585,15 @@
                     "shape": "CcEmailAddressList"
                 },
                 "displayId": {
                     "documentation": "<p>The ID displayed for the case in the Amazon Web Services Support Center. This is a numeric string.</p>",
                     "shape": "DisplayId"
                 },
                 "language": {
-                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports English (\"en\") and Japanese (\"ja\"). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
+                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports Chinese (\u201czh\u201d), English (\"en\"), Japanese (\"ja\") and Korean (\u201cko\u201d). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
                     "shape": "Language"
                 },
                 "recentCommunications": {
                     "documentation": "<p>The five most recent communications between you and Amazon Web Services Support Center, including the IDs of any attachments to the communications. Also includes a <code>nextToken</code> that you can use to retrieve earlier communications.</p>",
                     "shape": "RecentCaseCommunications"
                 },
                 "serviceCode": {
@@ -628,31 +687,34 @@
             "max": 10,
             "member": {
                 "shape": "CcEmailAddress"
             },
             "min": 0,
             "type": "list"
         },
+        "Code": {
+            "type": "string"
+        },
         "Communication": {
             "documentation": "<p>A communication associated with a support case. The communication consists of the case ID, the message body, attachment information, the submitter of the communication, and the date and time of the communication.</p>",
             "members": {
                 "attachmentSet": {
                     "documentation": "<p>Information about the attachments to the case communication.</p>",
                     "shape": "AttachmentSet"
                 },
                 "body": {
                     "documentation": "<p>The text of the communication between the customer and Amazon Web Services Support.</p>",
-                    "shape": "CommunicationBody"
+                    "shape": "ValidatedCommunicationBody"
                 },
                 "caseId": {
                     "documentation": "<p>The support case ID requested or returned in the call. The case ID is an alphanumeric string formatted as shown in this example: case-<i>12345678910-2013-c4c1d2bf33c5cf47</i> </p>",
                     "shape": "CaseId"
                 },
                 "submittedBy": {
-                    "documentation": "<p>The identity of the account that submitted, or responded to, the support case. Customer entries include the role or IAM user as well as the email address. For example, \"AdminRole (Role) &lt;janedoe@example.com&gt;. Entries from the Amazon Web Services Support team display \"Amazon Web Services,\" and don't show an email address. </p>",
+                    "documentation": "<p>The identity of the account that submitted, or responded to, the support case. Customer entries include the IAM role as well as the email address (for example, \"AdminRole (Role) &lt;janedoe@example.com&gt;). Entries from the Amazon Web Services Support team display \"Amazon Web Services,\" and don't show an email address. </p>",
                     "shape": "SubmittedBy"
                 },
                 "timeCreated": {
                     "documentation": "<p>The time the communication was created.</p>",
                     "shape": "TimeCreated"
                 }
             },
@@ -665,14 +727,40 @@
         },
         "CommunicationList": {
             "member": {
                 "shape": "Communication"
             },
             "type": "list"
         },
+        "CommunicationTypeOptions": {
+            "documentation": "<p>A JSON-formatted object that contains the CommunicationTypeOptions for creating a case for a certain communication channel. It is contained in the response from a <a>DescribeCreateCaseOptions</a> request. <b>CommunicationTypeOptions</b> contains the following fields:</p> <ul> <li> <p> <b>datesWithoutSupport</b> - A JSON-formatted list containing date and time ranges for periods without support in UTC time. Date and time format is RFC 3339 : 'yyyy-MM-dd'T'HH:mm:ss.SSSZZ'. </p> </li> <li> <p> <b>supportedHours</b> - A JSON-formatted list containing time ranges when support are available. Time format is RFC 3339 : 'HH:mm:ss.SSS'. </p> </li> <li> <p> <b>type</b> - A string value indicating the communication type that the aforementioned rules apply to. At the moment the type value can assume one of 3 values at the moment <code>chat</code>, <code>web</code> and <code>call</code>. </p> </li> </ul>",
+            "members": {
+                "datesWithoutSupport": {
+                    "documentation": "<p> A JSON-formatted list containing date and time ranges for periods without support </p>",
+                    "shape": "DatesWithoutSupportList"
+                },
+                "supportedHours": {
+                    "documentation": "<p> A JSON-formatted list containing time ranges when support is available. </p>",
+                    "shape": "SupportedHoursList"
+                },
+                "type": {
+                    "documentation": "<p> A string value indicating the communication type. At the moment the type value can assume one of 3 values at the moment chat, web and call. </p>",
+                    "shape": "Type"
+                }
+            },
+            "type": "structure"
+        },
+        "CommunicationTypeOptionsList": {
+            "max": 100,
+            "member": {
+                "shape": "CommunicationTypeOptions"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "CreateCaseRequest": {
             "members": {
                 "attachmentSetId": {
                     "documentation": "<p>The ID of a set of one or more attachments for the case. Create the set by using the <a>AddAttachmentsToSet</a> operation.</p>",
                     "shape": "AttachmentSetId"
                 },
                 "categoryCode": {
@@ -688,15 +776,15 @@
                     "shape": "CommunicationBody"
                 },
                 "issueType": {
                     "documentation": "<p>The type of issue for the case. You can specify <code>customer-service</code> or <code>technical</code>. If you don't specify a value, the default is <code>technical</code>.</p>",
                     "shape": "IssueType"
                 },
                 "language": {
-                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports English (\"en\") and Japanese (\"ja\"). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
+                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports Chinese (\u201czh\u201d), English (\"en\"), Japanese (\"ja\") and Korean (\u201cko\u201d). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
                     "shape": "Language"
                 },
                 "serviceCode": {
                     "documentation": "<p>The code for the Amazon Web Services service. You can use the <a>DescribeServices</a> operation to get the possible <code>serviceCode</code> values.</p>",
                     "shape": "ServiceCode"
                 },
                 "severityCode": {
@@ -723,14 +811,34 @@
                 }
             },
             "type": "structure"
         },
         "Data": {
             "type": "blob"
         },
+        "DateInterval": {
+            "documentation": "<p>Date and time (UTC) format in RFC 3339 : 'yyyy-MM-dd'T'HH:mm:ss.SSSZZ'.</p>",
+            "members": {
+                "endDateTime": {
+                    "documentation": "<p> End Date Time (UTC). RFC 3339 format : 'yyyy-MM-dd'T'HH:mm:ss.SSSZZ'. </p>",
+                    "shape": "ValidatedDateTime"
+                },
+                "startDateTime": {
+                    "documentation": "<p> A JSON object containing start and date time (UTC). Date and time format is RFC 3339 : 'yyyy-MM-dd'T'HH:mm:ss.SSSZZ'. </p>",
+                    "shape": "ValidatedDateTime"
+                }
+            },
+            "type": "structure"
+        },
+        "DatesWithoutSupportList": {
+            "member": {
+                "shape": "DateInterval"
+            },
+            "type": "list"
+        },
         "DescribeAttachmentLimitExceeded": {
             "documentation": "<p>The limit for the number of <a>DescribeAttachment</a> requests in a short period of time has been exceeded.</p>",
             "exception": true,
             "members": {
                 "message": {
                     "documentation": "<p>The limit for the number of <a>DescribeAttachment</a> requests in a short period of time has been exceeded.</p>",
                     "shape": "ErrorMessage"
@@ -783,15 +891,15 @@
                     "shape": "IncludeCommunications"
                 },
                 "includeResolvedCases": {
                     "documentation": "<p>Specifies whether to include resolved support cases in the <code>DescribeCases</code> response. By default, resolved cases aren't included.</p>",
                     "shape": "IncludeResolvedCases"
                 },
                 "language": {
-                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports English (\"en\") and Japanese (\"ja\"). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
+                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports Chinese (\u201czh\u201d), English (\"en\"), Japanese (\"ja\") and Korean (\u201cko\u201d). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
                     "shape": "Language"
                 },
                 "maxResults": {
                     "documentation": "<p>The maximum number of results to return before paginating.</p>",
                     "shape": "MaxResults"
                 },
                 "nextToken": {
@@ -853,18 +961,58 @@
                 "nextToken": {
                     "documentation": "<p>A resumption point for pagination.</p>",
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
+        "DescribeCreateCaseOptionsRequest": {
+            "members": {
+                "categoryCode": {
+                    "documentation": "<p>The category of problem for the support case. You also use the <a>DescribeServices</a> operation to get the category code for a service. Each Amazon Web Services service defines its own set of category codes.</p>",
+                    "shape": "CategoryCode"
+                },
+                "issueType": {
+                    "documentation": "<p>The type of issue for the case. You can specify <code>customer-service</code> or <code>technical</code>. If you don't specify a value, the default is <code>technical</code>.</p>",
+                    "shape": "IssueType"
+                },
+                "language": {
+                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports Chinese (\u201czh\u201d), English (\"en\"), Japanese (\"ja\") and Korean (\u201cko\u201d). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
+                    "shape": "Language"
+                },
+                "serviceCode": {
+                    "documentation": "<p>The code for the Amazon Web Services service. You can use the <a>DescribeServices</a> operation to get the possible <code>serviceCode</code> values.</p>",
+                    "shape": "ServiceCode"
+                }
+            },
+            "required": [
+                "issueType",
+                "serviceCode",
+                "language",
+                "categoryCode"
+            ],
+            "type": "structure"
+        },
+        "DescribeCreateCaseOptionsResponse": {
+            "members": {
+                "communicationTypes": {
+                    "documentation": "<p> A JSON-formatted array that contains the available communication type options, along with the available support timeframes for the given inputs. </p>",
+                    "shape": "CommunicationTypeOptionsList"
+                },
+                "languageAvailability": {
+                    "documentation": "<p>Language availability can be any of the following:</p> <ul> <li> <p> available </p> </li> <li> <p> best_effort </p> </li> <li> <p> unavailable </p> </li> </ul>",
+                    "shape": "ValidatedLanguageAvailability"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeServicesRequest": {
             "members": {
                 "language": {
-                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports English (\"en\") and Japanese (\"ja\"). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
+                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports Chinese (\u201czh\u201d), English (\"en\"), Japanese (\"ja\") and Korean (\u201cko\u201d). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
                     "shape": "Language"
                 },
                 "serviceCodeList": {
                     "documentation": "<p>A JSON-formatted list of service codes available for Amazon Web Services services.</p>",
                     "shape": "ServiceCodeList"
                 }
             },
@@ -879,15 +1027,15 @@
                 }
             },
             "type": "structure"
         },
         "DescribeSeverityLevelsRequest": {
             "members": {
                 "language": {
-                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports English (\"en\") and Japanese (\"ja\"). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
+                    "documentation": "<p>The language in which Amazon Web Services Support handles the case. Amazon Web Services Support currently supports Chinese (\u201czh\u201d), English (\"en\"), Japanese (\"ja\") and Korean (\u201cko\u201d). You must specify the ISO 639-1 code for the <code>language</code> parameter if you want support in that language.</p>",
                     "shape": "Language"
                 }
             },
             "type": "structure"
         },
         "DescribeSeverityLevelsResponse": {
             "documentation": "<p>The list of severity levels returned by the <a>DescribeSeverityLevels</a> operation.</p>",
@@ -895,14 +1043,45 @@
                 "severityLevels": {
                     "documentation": "<p>The available severity levels for the support case. Available severity levels are defined by your service level agreement with Amazon Web Services.</p>",
                     "shape": "SeverityLevelsList"
                 }
             },
             "type": "structure"
         },
+        "DescribeSupportedLanguagesRequest": {
+            "members": {
+                "categoryCode": {
+                    "documentation": "<p>The category of problem for the support case. You also use the <a>DescribeServices</a> operation to get the category code for a service. Each Amazon Web Services service defines its own set of category codes.</p>",
+                    "shape": "ValidatedCategoryCode"
+                },
+                "issueType": {
+                    "documentation": "<p>The type of issue for the case. You can specify <code>customer-service</code> or <code>technical</code>.</p>",
+                    "shape": "ValidatedIssueTypeString"
+                },
+                "serviceCode": {
+                    "documentation": "<p>The code for the Amazon Web Services service. You can use the <a>DescribeServices</a> operation to get the possible <code>serviceCode</code> values.</p>",
+                    "shape": "ValidatedServiceCode"
+                }
+            },
+            "required": [
+                "issueType",
+                "serviceCode",
+                "categoryCode"
+            ],
+            "type": "structure"
+        },
+        "DescribeSupportedLanguagesResponse": {
+            "members": {
+                "supportedLanguages": {
+                    "documentation": "<p> A JSON-formatted array that contains the available ISO 639-1 language codes. </p>",
+                    "shape": "SupportedLanguagesList"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeTrustedAdvisorCheckRefreshStatusesRequest": {
             "members": {
                 "checkIds": {
                     "documentation": "<p>The IDs of the Trusted Advisor checks to get the status.</p> <note> <p>If you specify the check ID of a check that is automatically refreshed, you might see an <code>InvalidParameterValue</code> error.</p> </note>",
                     "shape": "StringList"
                 }
             },
@@ -997,20 +1176,26 @@
                 }
             },
             "required": [
                 "checks"
             ],
             "type": "structure"
         },
+        "Display": {
+            "type": "string"
+        },
         "DisplayId": {
             "type": "string"
         },
         "Double": {
             "type": "double"
         },
+        "EndTime": {
+            "type": "string"
+        },
         "ErrorMessage": {
             "type": "string"
         },
         "ExpiryTime": {
             "type": "string"
         },
         "FileName": {
@@ -1180,14 +1365,17 @@
         },
         "SeverityLevelsList": {
             "member": {
                 "shape": "SeverityLevel"
             },
             "type": "list"
         },
+        "StartTime": {
+            "type": "string"
+        },
         "Status": {
             "type": "string"
         },
         "String": {
             "type": "string"
         },
         "StringList": {
@@ -1198,14 +1386,71 @@
         },
         "Subject": {
             "type": "string"
         },
         "SubmittedBy": {
             "type": "string"
         },
+        "SupportedHour": {
+            "documentation": "<p>Time range object with <code>startTime</code> and <code>endTime</code> range in RFC 3339 format. <code>'HH:mm:ss.SSS'</code>.</p>",
+            "members": {
+                "endTime": {
+                    "documentation": "<p> End Time. RFC 3339 format <code>'HH:mm:ss.SSS'</code>. </p>",
+                    "shape": "EndTime"
+                },
+                "startTime": {
+                    "documentation": "<p> Start Time. RFC 3339 format <code>'HH:mm:ss.SSS'</code>. </p>",
+                    "shape": "StartTime"
+                }
+            },
+            "type": "structure"
+        },
+        "SupportedHoursList": {
+            "member": {
+                "shape": "SupportedHour"
+            },
+            "type": "list"
+        },
+        "SupportedLanguage": {
+            "documentation": "<p> A JSON-formatted object that contains the available ISO 639-1 language <code>code</code>, <code>language</code> name and langauge <code>display</code> value. The language code is what should be used in the <a>CreateCase</a> call. </p>",
+            "members": {
+                "code": {
+                    "documentation": "<p> 2 digit ISO 639-1 code. e.g. <code>en</code> </p>",
+                    "shape": "Code"
+                },
+                "display": {
+                    "documentation": "<p> Language display value e.g. <code>ENGLISH</code> </p>",
+                    "shape": "Display"
+                },
+                "language": {
+                    "documentation": "<p> Full language description e.g. <code>ENGLISH</code> </p>",
+                    "shape": "Language"
+                }
+            },
+            "type": "structure"
+        },
+        "SupportedLanguagesList": {
+            "max": 100,
+            "member": {
+                "shape": "SupportedLanguage"
+            },
+            "min": 0,
+            "type": "list"
+        },
+        "ThrottlingException": {
+            "documentation": "<p> You have exceeded the maximum allowed TPS (Transactions Per Second) for the operations. </p>",
+            "exception": true,
+            "members": {
+                "message": {
+                    "shape": "AvailabilityErrorMessage"
+                }
+            },
+            "synthetic": true,
+            "type": "structure"
+        },
         "TimeCreated": {
             "type": "string"
         },
         "TrustedAdvisorCategorySpecificSummary": {
             "documentation": "<p>The container for summary information that relates to the category of the Trusted Advisor check.</p>",
             "members": {
                 "costOptimizing": {
@@ -1440,11 +1685,44 @@
             "required": [
                 "resourcesProcessed",
                 "resourcesFlagged",
                 "resourcesIgnored",
                 "resourcesSuppressed"
             ],
             "type": "structure"
+        },
+        "Type": {
+            "type": "string"
+        },
+        "ValidatedCategoryCode": {
+            "max": 100,
+            "min": 0,
+            "type": "string"
+        },
+        "ValidatedCommunicationBody": {
+            "max": 8000,
+            "min": 1,
+            "type": "string"
+        },
+        "ValidatedDateTime": {
+            "max": 30,
+            "min": 8,
+            "type": "string"
+        },
+        "ValidatedIssueTypeString": {
+            "max": 22,
+            "min": 9,
+            "type": "string"
+        },
+        "ValidatedLanguageAvailability": {
+            "max": 100,
+            "min": 0,
+            "type": "string"
+        },
+        "ValidatedServiceCode": {
+            "max": 100,
+            "min": 0,
+            "type": "string"
         }
     },
     "version": "2.0"
 }
```

### Comparing `botocore-a-la-carte-support-1.29.99/botocore_a_la_carte_support.egg-info/PKG-INFO` & `botocore-a-la-carte-support-1.30.0/botocore_a_la_carte_support.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-support
-Version: 1.29.99
+Version: 1.30.0
 Summary: support data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-support-1.29.99/setup.py` & `botocore-a-la-carte-support-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-support',
-    version="1.29.99",
+    version="1.30.0",
     description='support data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/support/*/*.json'],
```

