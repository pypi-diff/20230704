# Comparing `tmp/botocore-a-la-carte-auditmanager-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-auditmanager-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-auditmanager-1.29.99.tar", last modified: Sat Mar 25 01:22:26 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-auditmanager-1.30.0.tar", last modified: Tue Jul  4 01:44:17 2023, max compression
```

## Comparing `botocore-a-la-carte-auditmanager-1.29.99.tar` & `botocore-a-la-carte-auditmanager-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:26.366536 botocore-a-la-carte-auditmanager-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:26.000000 botocore-a-la-carte-auditmanager-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-25 01:22:26.366536 botocore-a-la-carte-auditmanager-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:26.366536 botocore-a-la-carte-auditmanager-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:26.366536 botocore-a-la-carte-auditmanager-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:26.366536 botocore-a-la-carte-auditmanager-1.29.99/botocore/data/auditmanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:26.366536 botocore-a-la-carte-auditmanager-1.29.99/botocore/data/auditmanager/2017-07-25/
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-03-25 01:22:12.000000 botocore-a-la-carte-auditmanager-1.29.99/botocore/data/auditmanager/2017-07-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-auditmanager-1.29.99/botocore/data/auditmanager/2017-07-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-25 01:22:12.000000 botocore-a-la-carte-auditmanager-1.29.99/botocore/data/auditmanager/2017-07-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   207284 2023-03-25 01:22:12.000000 botocore-a-la-carte-auditmanager-1.29.99/botocore/data/auditmanager/2017-07-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:26.366536 botocore-a-la-carte-auditmanager-1.29.99/botocore_a_la_carte_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-25 01:22:26.000000 botocore-a-la-carte-auditmanager-1.29.99/botocore_a_la_carte_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-25 01:22:26.000000 botocore-a-la-carte-auditmanager-1.29.99/botocore_a_la_carte_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:26.000000 botocore-a-la-carte-auditmanager-1.29.99/botocore_a_la_carte_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:26.000000 botocore-a-la-carte-auditmanager-1.29.99/botocore_a_la_carte_auditmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:26.366536 botocore-a-la-carte-auditmanager-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-25 01:22:26.000000 botocore-a-la-carte-auditmanager-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:17.014411 botocore-a-la-carte-auditmanager-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:16.000000 botocore-a-la-carte-auditmanager-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-04 01:44:17.014411 botocore-a-la-carte-auditmanager-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:17.010411 botocore-a-la-carte-auditmanager-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:17.010411 botocore-a-la-carte-auditmanager-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:17.010411 botocore-a-la-carte-auditmanager-1.30.0/botocore/data/auditmanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:17.010411 botocore-a-la-carte-auditmanager-1.30.0/botocore/data/auditmanager/2017-07-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-04 01:44:02.000000 botocore-a-la-carte-auditmanager-1.30.0/botocore/data/auditmanager/2017-07-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-auditmanager-1.30.0/botocore/data/auditmanager/2017-07-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-auditmanager-1.30.0/botocore/data/auditmanager/2017-07-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   216101 2023-07-04 01:44:02.000000 botocore-a-la-carte-auditmanager-1.30.0/botocore/data/auditmanager/2017-07-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:17.010411 botocore-a-la-carte-auditmanager-1.30.0/botocore_a_la_carte_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-04 01:44:16.000000 botocore-a-la-carte-auditmanager-1.30.0/botocore_a_la_carte_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-04 01:44:16.000000 botocore-a-la-carte-auditmanager-1.30.0/botocore_a_la_carte_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:16.000000 botocore-a-la-carte-auditmanager-1.30.0/botocore_a_la_carte_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:16.000000 botocore-a-la-carte-auditmanager-1.30.0/botocore_a_la_carte_auditmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:17.014411 botocore-a-la-carte-auditmanager-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-04 01:44:16.000000 botocore-a-la-carte-auditmanager-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-auditmanager-1.29.99/LICENSE.txt` & `botocore-a-la-carte-auditmanager-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-auditmanager-1.29.99/PKG-INFO` & `botocore-a-la-carte-auditmanager-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-auditmanager
-Version: 1.29.99
+Version: 1.30.0
 Summary: auditmanager data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-auditmanager-1.29.99/botocore/data/auditmanager/2017-07-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-auditmanager-1.30.0/botocore/data/auditmanager/2017-07-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-auditmanager-1.29.99/botocore/data/auditmanager/2017-07-25/service-2.json` & `botocore-a-la-carte-auditmanager-1.30.0/botocore/data/auditmanager/2017-07-25/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9952196263444874%*

 * *Differences: {"'operations'": "{'BatchImportEvidenceToAssessmentControl': {'errors': {insert: [(4, "*

 * *                 "OrderedDict([('shape', 'ThrottlingException')]))]}, 'documentation': '<p>Adds "*

 * *                 'one or more pieces of evidence to a control in an Audit Manager assessment. </p> '*

 * *                 '<p>You can import manual evidence from any S3 bucket by specifying the S3 URI of '*

 * *                 'the object. You can also upload a file from your browser, or enter plain text in '*

 * *                 'respo […]*

```diff
@@ -149,27 +149,30 @@
             },
             "name": "BatchDisassociateAssessmentReportEvidence",
             "output": {
                 "shape": "BatchDisassociateAssessmentReportEvidenceResponse"
             }
         },
         "BatchImportEvidenceToAssessmentControl": {
-            "documentation": "<p>Uploads one or more pieces of evidence to a control in an Audit Manager assessment. You can upload manual evidence from any Amazon Simple Storage Service (Amazon S3) bucket by specifying the S3 URI of the evidence. </p> <p>You must upload manual evidence to your S3 bucket before you can upload it to your assessment. For instructions, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_CreateBucket.html\">CreateBucket</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html\">PutObject</a> in the <i>Amazon Simple Storage Service API Reference.</i> </p> <p>The following restrictions apply to this action:</p> <ul> <li> <p>Maximum size of an individual evidence file: 100 MB</p> </li> <li> <p>Number of daily manual evidence uploads per control: 100</p> </li> <li> <p>Supported file formats: See <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/upload-evidence.html#supported-manual-evidence-files\">Supported file types for manual evidence</a> in the <i>Audit Manager User Guide</i> </p> </li> </ul> <p>For more information about Audit Manager service restrictions, see <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/service-quotas.html\">Quotas and restrictions for Audit Manager</a>.</p>",
+            "documentation": "<p>Adds one or more pieces of evidence to a control in an Audit Manager assessment. </p> <p>You can import manual evidence from any S3 bucket by specifying the S3 URI of the object. You can also upload a file from your browser, or enter plain text in response to a risk assessment question. </p> <p>The following restrictions apply to this action:</p> <ul> <li> <p> <code>manualEvidence</code> can be only one of the following: <code>evidenceFileName</code>, <code>s3ResourcePath</code>, or <code>textResponse</code> </p> </li> <li> <p>Maximum size of an individual evidence file: 100 MB</p> </li> <li> <p>Number of daily manual evidence uploads per control: 100</p> </li> <li> <p>Supported file formats: See <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/upload-evidence.html#supported-manual-evidence-files\">Supported file types for manual evidence</a> in the <i>Audit Manager User Guide</i> </p> </li> </ul> <p>For more information about Audit Manager service restrictions, see <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/service-quotas.html\">Quotas and restrictions for Audit Manager</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/assessments/{assessmentId}/controlSets/{controlSetId}/controls/{controlId}/evidence"
             },
             "input": {
@@ -410,15 +413,15 @@
             },
             "name": "DeleteAssessmentReport",
             "output": {
                 "shape": "DeleteAssessmentReportResponse"
             }
         },
         "DeleteControl": {
-            "documentation": "<p> Deletes a custom control in Audit Manager. </p>",
+            "documentation": "<p> Deletes a custom control in Audit Manager. </p> <important> <p>When you invoke this operation, the custom control is deleted from any frameworks or assessments that it\u2019s currently part of. As a result, Audit Manager will stop collecting evidence for that custom control in all of your assessments. This includes assessments that you previously created before you deleted the custom control.</p> </important>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -522,15 +525,15 @@
             },
             "name": "DisassociateAssessmentReportEvidenceFolder",
             "output": {
                 "shape": "DisassociateAssessmentReportEvidenceFolderResponse"
             }
         },
         "GetAccountStatus": {
-            "documentation": "<p> Returns the registration status of an account in Audit Manager. </p>",
+            "documentation": "<p> Gets the registration status of an account in Audit Manager. </p>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 }
             ],
             "http": {
                 "method": "GET",
@@ -541,15 +544,15 @@
             },
             "name": "GetAccountStatus",
             "output": {
                 "shape": "GetAccountStatusResponse"
             }
         },
         "GetAssessment": {
-            "documentation": "<p>Returns an assessment from Audit Manager. </p>",
+            "documentation": "<p>Gets information about a specified assessment. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -569,15 +572,15 @@
             },
             "name": "GetAssessment",
             "output": {
                 "shape": "GetAssessmentResponse"
             }
         },
         "GetAssessmentFramework": {
-            "documentation": "<p>Returns a framework from Audit Manager. </p>",
+            "documentation": "<p>Gets information about a specified framework.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -597,15 +600,15 @@
             },
             "name": "GetAssessmentFramework",
             "output": {
                 "shape": "GetAssessmentFrameworkResponse"
             }
         },
         "GetAssessmentReportUrl": {
-            "documentation": "<p> Returns the URL of an assessment report in Audit Manager. </p>",
+            "documentation": "<p> Gets the URL of an assessment report in Audit Manager. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -625,15 +628,15 @@
             },
             "name": "GetAssessmentReportUrl",
             "output": {
                 "shape": "GetAssessmentReportUrlResponse"
             }
         },
         "GetChangeLogs": {
-            "documentation": "<p> Returns a list of changelogs from Audit Manager. </p>",
+            "documentation": "<p> Gets a list of changelogs from Audit Manager. </p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -653,15 +656,15 @@
             },
             "name": "GetChangeLogs",
             "output": {
                 "shape": "GetChangeLogsResponse"
             }
         },
         "GetControl": {
-            "documentation": "<p> Returns a control from Audit Manager. </p>",
+            "documentation": "<p> Gets information about a specified control.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -681,15 +684,15 @@
             },
             "name": "GetControl",
             "output": {
                 "shape": "GetControlResponse"
             }
         },
         "GetDelegations": {
-            "documentation": "<p> Returns a list of delegations from an audit owner to a delegate. </p>",
+            "documentation": "<p> Gets a list of delegations from an audit owner to a delegate. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -706,15 +709,15 @@
             },
             "name": "GetDelegations",
             "output": {
                 "shape": "GetDelegationsResponse"
             }
         },
         "GetEvidence": {
-            "documentation": "<p> Returns evidence from Audit Manager. </p>",
+            "documentation": "<p> Gets information about a specified evidence item.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -734,15 +737,15 @@
             },
             "name": "GetEvidence",
             "output": {
                 "shape": "GetEvidenceResponse"
             }
         },
         "GetEvidenceByEvidenceFolder": {
-            "documentation": "<p> Returns all evidence from a specified evidence folder in Audit Manager. </p>",
+            "documentation": "<p> Gets all evidence from a specified evidence folder in Audit Manager. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -761,16 +764,44 @@
                 "shape": "GetEvidenceByEvidenceFolderRequest"
             },
             "name": "GetEvidenceByEvidenceFolder",
             "output": {
                 "shape": "GetEvidenceByEvidenceFolderResponse"
             }
         },
+        "GetEvidenceFileUploadUrl": {
+            "documentation": "<p>Creates a presigned Amazon S3 URL that can be used to upload a file as manual evidence. For instructions on how to use this operation, see <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/upload-evidence.html#how-to-upload-manual-evidence-files\">Upload a file from your browser </a> in the <i>Audit Manager User Guide</i>.</p> <p>The following restrictions apply to this operation:</p> <ul> <li> <p>Maximum size of an individual evidence file: 100 MB</p> </li> <li> <p>Number of daily manual evidence uploads per control: 100</p> </li> <li> <p>Supported file formats: See <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/upload-evidence.html#supported-manual-evidence-files\">Supported file types for manual evidence</a> in the <i>Audit Manager User Guide</i> </p> </li> </ul> <p>For more information about Audit Manager service restrictions, see <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/service-quotas.html\">Quotas and restrictions for Audit Manager</a>.</p>",
+            "errors": [
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/evidenceFileUploadUrl"
+            },
+            "input": {
+                "shape": "GetEvidenceFileUploadUrlRequest"
+            },
+            "name": "GetEvidenceFileUploadUrl",
+            "output": {
+                "shape": "GetEvidenceFileUploadUrlResponse"
+            }
+        },
         "GetEvidenceFolder": {
-            "documentation": "<p> Returns an evidence folder from the specified assessment in Audit Manager. </p>",
+            "documentation": "<p> Gets an evidence folder from a specified assessment in Audit Manager. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -790,15 +821,15 @@
             },
             "name": "GetEvidenceFolder",
             "output": {
                 "shape": "GetEvidenceFolderResponse"
             }
         },
         "GetEvidenceFoldersByAssessment": {
-            "documentation": "<p> Returns the evidence folders from a specified assessment in Audit Manager. </p>",
+            "documentation": "<p> Gets the evidence folders from a specified assessment in Audit Manager. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -818,15 +849,15 @@
             },
             "name": "GetEvidenceFoldersByAssessment",
             "output": {
                 "shape": "GetEvidenceFoldersByAssessmentResponse"
             }
         },
         "GetEvidenceFoldersByAssessmentControl": {
-            "documentation": "<p> Returns a list of evidence folders that are associated with a specified control in an Audit Manager assessment. </p>",
+            "documentation": "<p> Gets a list of evidence folders that are associated with a specified control in an Audit Manager assessment. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -896,15 +927,15 @@
             },
             "name": "GetInsightsByAssessment",
             "output": {
                 "shape": "GetInsightsByAssessmentResponse"
             }
         },
         "GetOrganizationAdminAccount": {
-            "documentation": "<p> Returns the name of the delegated Amazon Web Services administrator account for the organization. </p>",
+            "documentation": "<p> Gets the name of the delegated Amazon Web Services administrator account for a specified organization. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -924,15 +955,15 @@
             },
             "name": "GetOrganizationAdminAccount",
             "output": {
                 "shape": "GetOrganizationAdminAccountResponse"
             }
         },
         "GetServicesInScope": {
-            "documentation": "<p>Returns a list of all of the Amazon Web Services that you can choose to include in your assessment. When you <a href=\"https://docs.aws.amazon.com/audit-manager/latest/APIReference/API_CreateAssessment.html\">create an assessment</a>, specify which of these services you want to include to narrow the assessment's <a href=\"https://docs.aws.amazon.com/audit-manager/latest/APIReference/API_Scope.html\">scope</a>.</p>",
+            "documentation": "<p>Gets a list of all of the Amazon Web Services that you can choose to include in your assessment. When you <a href=\"https://docs.aws.amazon.com/audit-manager/latest/APIReference/API_CreateAssessment.html\">create an assessment</a>, specify which of these services you want to include to narrow the assessment's <a href=\"https://docs.aws.amazon.com/audit-manager/latest/APIReference/API_Scope.html\">scope</a>.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -949,15 +980,15 @@
             },
             "name": "GetServicesInScope",
             "output": {
                 "shape": "GetServicesInScopeResponse"
             }
         },
         "GetSettings": {
-            "documentation": "<p> Returns the settings for the specified Amazon Web Services account. </p>",
+            "documentation": "<p> Gets the settings for a specified Amazon Web Services account. </p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "InternalServerException"
                 }
@@ -2370,15 +2401,15 @@
             ],
             "type": "string"
         },
         "AssessmentReportsDestination": {
             "documentation": "<p> The location where Audit Manager saves assessment reports for the given assessment. </p>",
             "members": {
                 "destination": {
-                    "documentation": "<p> The destination of the assessment report. </p>",
+                    "documentation": "<p> The destination bucket where Audit Manager stores assessment reports. </p>",
                     "shape": "S3Url"
                 },
                 "destinationType": {
                     "documentation": "<p> The destination type, such as Amazon S3. </p>",
                     "shape": "AssessmentReportDestinationType"
                 }
             },
@@ -2776,15 +2807,15 @@
                     "shape": "TagMap"
                 },
                 "testingInformation": {
                     "documentation": "<p> The steps that you should follow to determine if the control has been satisfied. </p>",
                     "shape": "TestingInformation"
                 },
                 "type": {
-                    "documentation": "<p> The type of control, such as a custom control or a standard control. </p>",
+                    "documentation": "<p> Specifies whether the control is a standard control or a custom control.</p>",
                     "shape": "ControlType"
                 }
             },
             "type": "structure"
         },
         "ControlComment": {
             "documentation": "<p> A comment that's posted by a user on a control. This includes the author's name, the comment text, and a timestamp. </p>",
@@ -2920,15 +2951,15 @@
             "documentation": "<p> The data source that determines where Audit Manager collects evidence from for the control. </p>",
             "members": {
                 "sourceDescription": {
                     "documentation": "<p> The description of the source. </p>",
                     "shape": "SourceDescription"
                 },
                 "sourceFrequency": {
-                    "documentation": "<p> The frequency of evidence collection for the control mapping source. </p>",
+                    "documentation": "<p>Specifies how often evidence is collected from the control mapping source. </p>",
                     "shape": "SourceFrequency"
                 },
                 "sourceId": {
                     "documentation": "<p> The unique identifier for the source. </p>",
                     "shape": "UUID"
                 },
                 "sourceKeyword": {
@@ -3259,15 +3290,15 @@
             "documentation": "<p> The control mapping fields that represent the source for evidence collection, along with related parameters and metadata. This doesn't contain <code>mappingID</code>. </p>",
             "members": {
                 "sourceDescription": {
                     "documentation": "<p> The description of the data source that determines where Audit Manager collects evidence from for the control. </p>",
                     "shape": "SourceDescription"
                 },
                 "sourceFrequency": {
-                    "documentation": "<p> The frequency of evidence collection for the control mapping source. </p>",
+                    "documentation": "<p>Specifies how often evidence is collected from the control mapping source. </p>",
                     "shape": "SourceFrequency"
                 },
                 "sourceKeyword": {
                     "shape": "SourceKeyword"
                 },
                 "sourceName": {
                     "documentation": "<p> The name of the control mapping data source. </p>",
@@ -3373,14 +3404,28 @@
         },
         "CreatedBy": {
             "max": 100,
             "min": 1,
             "pattern": "^[a-zA-Z0-9\\s-_()\\[\\]]+$",
             "type": "string"
         },
+        "DefaultExportDestination": {
+            "documentation": "<p>The default s3 bucket where Audit Manager saves the files that you export from evidence finder.</p>",
+            "members": {
+                "destination": {
+                    "documentation": "<p>The destination bucket where Audit Manager stores exported files.</p>",
+                    "shape": "S3Url"
+                },
+                "destinationType": {
+                    "documentation": "<p>The destination type, such as Amazon S3.</p>",
+                    "shape": "ExportDestinationType"
+                }
+            },
+            "type": "structure"
+        },
         "Delegation": {
             "documentation": "<p> The assignment of a control set to a delegate for review. </p>",
             "members": {
                 "assessmentId": {
                     "documentation": "<p> The identifier for the assessment that's associated with the delegation. </p>",
                     "shape": "UUID"
                 },
@@ -3844,37 +3889,43 @@
         },
         "EvidenceSources": {
             "member": {
                 "shape": "NonEmptyString"
             },
             "type": "list"
         },
+        "ExportDestinationType": {
+            "enum": [
+                "S3"
+            ],
+            "type": "string"
+        },
         "Filename": {
             "max": 255,
             "min": 1,
             "pattern": "^[\\w,\\s-]+\\.[A-Za-z]+$",
             "type": "string"
         },
         "Framework": {
             "documentation": "<p> The file that's used to structure and automate Audit Manager assessments for a given compliance standard. </p>",
             "members": {
                 "arn": {
                     "documentation": "<p> The Amazon Resource Name (ARN) of the framework. </p>",
                     "shape": "AuditManagerArn"
                 },
                 "complianceType": {
-                    "documentation": "<p> The compliance type that the new custom framework supports, such as CIS or HIPAA. </p>",
+                    "documentation": "<p> The compliance type that the framework supports, such as CIS or HIPAA. </p>",
                     "shape": "ComplianceType"
                 },
                 "controlSets": {
                     "documentation": "<p> The control sets that are associated with the framework. </p>",
                     "shape": "ControlSets"
                 },
                 "controlSources": {
-                    "documentation": "<p> The sources that Audit Manager collects evidence from for the control. </p>",
+                    "documentation": "<p> The control data sources where Audit Manager collects evidence from.</p>",
                     "shape": "ControlSources"
                 },
                 "createdAt": {
                     "documentation": "<p> The time when the framework was created. </p>",
                     "shape": "Timestamp"
                 },
                 "createdBy": {
@@ -3906,15 +3957,15 @@
                     "shape": "FrameworkName"
                 },
                 "tags": {
                     "documentation": "<p> The tags that are associated with the framework. </p>",
                     "shape": "TagMap"
                 },
                 "type": {
-                    "documentation": "<p> The framework type, such as a custom framework or a standard framework. </p>",
+                    "documentation": "<p> Specifies whether the framework is a standard framework or a custom framework.</p>",
                     "shape": "FrameworkType"
                 }
             },
             "type": "structure"
         },
         "FrameworkDescription": {
             "max": 1000,
@@ -4123,15 +4174,15 @@
                 "controlId"
             ],
             "type": "structure"
         },
         "GetControlResponse": {
             "members": {
                 "control": {
-                    "documentation": "<p> The name of the control that the <code>GetControl</code> API returned. </p>",
+                    "documentation": "<p> The details of the control that the <code>GetControl</code> API returned. </p>",
                     "shape": "Control"
                 }
             },
             "type": "structure"
         },
         "GetDelegationsRequest": {
             "members": {
@@ -4212,14 +4263,41 @@
                 "nextToken": {
                     "documentation": "<p> The pagination token that's used to fetch the next set of results. </p>",
                     "shape": "Token"
                 }
             },
             "type": "structure"
         },
+        "GetEvidenceFileUploadUrlRequest": {
+            "members": {
+                "fileName": {
+                    "documentation": "<p>The file that you want to upload. For a list of supported file formats, see <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/upload-evidence.html#supported-manual-evidence-files\">Supported file types for manual evidence</a> in the <i>Audit Manager User Guide</i>.</p>",
+                    "location": "querystring",
+                    "locationName": "fileName",
+                    "shape": "ManualEvidenceLocalFileName"
+                }
+            },
+            "required": [
+                "fileName"
+            ],
+            "type": "structure"
+        },
+        "GetEvidenceFileUploadUrlResponse": {
+            "members": {
+                "evidenceFileName": {
+                    "documentation": "<p>The name of the uploaded manual evidence file that the presigned URL was generated for.</p>",
+                    "shape": "NonEmptyString"
+                },
+                "uploadUrl": {
+                    "documentation": "<p>The presigned URL that was generated.</p>",
+                    "shape": "NonEmptyString"
+                }
+            },
+            "type": "structure"
+        },
         "GetEvidenceFolderRequest": {
             "members": {
                 "assessmentId": {
                     "documentation": "<p> The unique identifier for the assessment. </p>",
                     "location": "uri",
                     "locationName": "assessmentId",
                     "shape": "UUID"
@@ -4572,15 +4650,17 @@
             "required": [
                 "message"
             ],
             "type": "structure"
         },
         "KeywordInputType": {
             "enum": [
-                "SELECT_FROM_LIST"
+                "SELECT_FROM_LIST",
+                "UPLOAD_FILE",
+                "INPUT_TEXT"
             ],
             "type": "string"
         },
         "KeywordValue": {
             "max": 100,
             "min": 1,
             "pattern": "^[a-zA-Z_0-9-\\s().]+$",
@@ -4714,15 +4794,15 @@
                 "frameworkType"
             ],
             "type": "structure"
         },
         "ListAssessmentFrameworksResponse": {
             "members": {
                 "frameworkMetadataList": {
-                    "documentation": "<p> The list of metadata objects for the framework. </p>",
+                    "documentation": "<p> A list of metadata that the <code>ListAssessmentFrameworks</code> API returns for each framework.</p>",
                     "shape": "FrameworkMetadataList"
                 },
                 "nextToken": {
                     "documentation": "<p> The pagination token that's used to fetch the next set of results. </p>",
                     "shape": "Token"
                 }
             },
@@ -4786,15 +4866,15 @@
                 }
             },
             "type": "structure"
         },
         "ListAssessmentsResponse": {
             "members": {
                 "assessmentMetadata": {
-                    "documentation": "<p> The metadata that's associated with the assessment. </p>",
+                    "documentation": "<p>The metadata that the <code>ListAssessments</code> API returns for each assessment.</p>",
                     "shape": "ListAssessmentMetadata"
                 },
                 "nextToken": {
                     "documentation": "<p> The pagination token that's used to fetch the next set of results. </p>",
                     "shape": "Token"
                 }
             },
@@ -4933,15 +5013,15 @@
                 "controlType"
             ],
             "type": "structure"
         },
         "ListControlsResponse": {
             "members": {
                 "controlMetadataList": {
-                    "documentation": "<p> The list of control metadata objects that the <code>ListControls</code> API returned. </p>",
+                    "documentation": "<p> A list of metadata that the <code>ListControls</code> API returns for each control.</p>",
                     "shape": "ControlMetadataList"
                 },
                 "nextToken": {
                     "documentation": "<p> The pagination token that's used to fetch the next set of results. </p>",
                     "shape": "Token"
                 }
             },
@@ -5036,31 +5116,51 @@
                     "documentation": "<p> The list of tags that the <code>ListTagsForResource</code> API returned. </p>",
                     "shape": "TagMap"
                 }
             },
             "type": "structure"
         },
         "ManualEvidence": {
-            "documentation": "<p> Evidence that's uploaded to Audit Manager manually. </p>",
+            "documentation": "<p> Evidence that's manually added to a control in Audit Manager. <code>manualEvidence</code> can be one of the following: <code>evidenceFileName</code>, <code>s3ResourcePath</code>, or <code>textResponse</code>.</p>",
             "members": {
+                "evidenceFileName": {
+                    "documentation": "<p>The name of the file that's uploaded as manual evidence. This name is populated using the <code>evidenceFileName</code> value from the <a href=\"https://docs.aws.amazon.com/audit-manager/latest/APIReference/API_GetEvidenceFileUploadUrl.html\"> <code>GetEvidenceFileUploadUrl</code> </a> API response.</p>",
+                    "shape": "ManualEvidenceLocalFileName"
+                },
                 "s3ResourcePath": {
-                    "documentation": "<p> The Amazon S3 URL that points to a manual evidence object. </p>",
+                    "documentation": "<p>The S3 URL of the object that's imported as manual evidence. </p>",
                     "shape": "S3Url"
+                },
+                "textResponse": {
+                    "documentation": "<p>The plain text response that's entered and saved as manual evidence.</p>",
+                    "shape": "ManualEvidenceTextResponse"
                 }
             },
             "type": "structure"
         },
         "ManualEvidenceList": {
             "max": 50,
             "member": {
                 "shape": "ManualEvidence"
             },
             "min": 1,
             "type": "list"
         },
+        "ManualEvidenceLocalFileName": {
+            "max": 300,
+            "min": 1,
+            "pattern": "[^\\/]*",
+            "type": "string"
+        },
+        "ManualEvidenceTextResponse": {
+            "max": 1000,
+            "min": 1,
+            "pattern": "^[\\w\\W\\s\\S]*$",
+            "type": "string"
+        },
         "MaxResults": {
             "documentation": "Max results in the page.",
             "max": 1000,
             "min": 1,
             "type": "integer"
         },
         "NonEmptyString": {
@@ -5338,25 +5438,30 @@
             "enum": [
                 "ALL",
                 "IS_AWS_ORG_ENABLED",
                 "SNS_TOPIC",
                 "DEFAULT_ASSESSMENT_REPORTS_DESTINATION",
                 "DEFAULT_PROCESS_OWNERS",
                 "EVIDENCE_FINDER_ENABLEMENT",
-                "DEREGISTRATION_POLICY"
+                "DEREGISTRATION_POLICY",
+                "DEFAULT_EXPORT_DESTINATION"
             ],
             "type": "string"
         },
         "Settings": {
             "documentation": "<p> The settings object that holds all supported Audit Manager settings. </p>",
             "members": {
                 "defaultAssessmentReportsDestination": {
-                    "documentation": "<p> The default storage destination for assessment reports. </p>",
+                    "documentation": "<p>The default S3 destination bucket for storing assessment reports.</p>",
                     "shape": "AssessmentReportsDestination"
                 },
+                "defaultExportDestination": {
+                    "documentation": "<p>The default S3 destination bucket for storing evidence finder exports.</p>",
+                    "shape": "DefaultExportDestination"
+                },
                 "defaultProcessOwners": {
                     "documentation": "<p> The designated default audit owners. </p>",
                     "shape": "Roles"
                 },
                 "deregistrationPolicy": {
                     "documentation": "<p>The deregistration policy for your Audit Manager data. You can use this attribute to determine how your data is handled when you deregister Audit Manager.</p>",
                     "shape": "DeregistrationPolicy"
@@ -5429,22 +5534,22 @@
                 "DAILY",
                 "WEEKLY",
                 "MONTHLY"
             ],
             "type": "string"
         },
         "SourceKeyword": {
-            "documentation": "<p> The keyword to search for in CloudTrail logs, Config rules, Security Hub checks, and Amazon Web Services API names. </p> <p> To learn more about the supported keywords that you can use when mapping a control data source, see the following pages in the <i>Audit Manager User Guide</i>:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-ash.html\">Config rules supported by Audit Manager</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-config.html\">Security Hub controls supported by Audit Manager</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-api.html\">API calls supported by Audit Manager</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-cloudtrail.html\">CloudTrail event names supported by Audit Manager</a> </p> </li> </ul>",
+            "documentation": "<p>A keyword that relates to the control data source.</p> <p>For manual evidence, this keyword indicates if the manual evidence is a file or text.</p> <p>For automated evidence, this keyword identifies a specific CloudTrail event, Config rule, Security Hub control, or Amazon Web Services API name. </p> <p> To learn more about the supported keywords that you can use when mapping a control data source, see the following pages in the <i>Audit Manager User Guide</i>:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-config.html\">Config rules supported by Audit Manager</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-ash.html\">Security Hub controls supported by Audit Manager</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-api.html\">API calls supported by Audit Manager</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-cloudtrail.html\">CloudTrail event names supported by Audit Manager</a> </p> </li> </ul>",
             "members": {
                 "keywordInputType": {
-                    "documentation": "<p> The input method for the keyword. </p>",
+                    "documentation": "<p> The input method for the keyword. </p> <ul> <li> <p> <code>SELECT_FROM_LIST</code> is used when mapping a data source for automated evidence.</p> <ul> <li> <p>When <code>keywordInputType</code> is <code>SELECT_FROM_LIST</code>, a keyword must be selected to collect automated evidence. For example, this keyword can be a CloudTrail event name, a rule name for Config, a Security Hub control, or the name of an Amazon Web Services API call.</p> </li> </ul> </li> <li> <p> <code>UPLOAD_FILE</code> and <code>INPUT_TEXT</code> are only used when mapping a data source for manual evidence.</p> <ul> <li> <p>When <code>keywordInputType</code> is <code>UPLOAD_FILE</code>, a file must be uploaded as manual evidence.</p> </li> <li> <p>When <code>keywordInputType</code> is <code>INPUT_TEXT</code>, text must be entered as manual evidence.</p> </li> </ul> </li> </ul>",
                     "shape": "KeywordInputType"
                 },
                 "keywordValue": {
-                    "documentation": "<p> The value of the keyword that's used when mapping a control data source. For example, this can be a CloudTrail event name, a rule name for Config, a Security Hub control, or the name of an Amazon Web Services API call. </p> <p>If you\u2019re mapping a data source to a rule in Config, the <code>keywordValue</code> that you specify depends on the type of rule:</p> <ul> <li> <p>For <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config_use-managed-rules.html\">managed rules</a>, you can use the rule identifier as the <code>keywordValue</code>. You can find the rule identifier from the <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html\">list of Config managed rules</a>.</p> <ul> <li> <p>Managed rule name: <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-acl-prohibited.html\">s3-bucket-acl-prohibited</a> </p> <p> <code>keywordValue</code>: <code>S3_BUCKET_ACL_PROHIBITED</code> </p> </li> </ul> </li> <li> <p>For <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config_develop-rules.html\">custom rules</a>, you form the <code>keywordValue</code> by adding the <code>Custom_</code> prefix to the rule name. This prefix distinguishes the rule from a managed rule.</p> <ul> <li> <p>Custom rule name: my-custom-config-rule</p> <p> <code>keywordValue</code>: <code>Custom_my-custom-config-rule</code> </p> </li> </ul> </li> <li> <p>For <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/service-linked-awsconfig-rules.html\">service-linked rules</a>, you form the <code>keywordValue</code> by adding the <code>Custom_</code> prefix to the rule name. In addition, you remove the suffix ID that appears at the end of the rule name.</p> <ul> <li> <p>Service-linked rule name: CustomRuleForAccount-conformance-pack-szsm1uv0w</p> <p> <code>keywordValue</code>: <code>Custom_CustomRuleForAccount-conformance-pack</code> </p> </li> <li> <p>Service-linked rule name: OrgConfigRule-s3-bucket-versioning-enabled-dbgzf8ba</p> <p> <code>keywordValue</code>: <code>Custom_OrgConfigRule-s3-bucket-versioning-enabled</code> </p> </li> </ul> </li> </ul>",
+                    "documentation": "<p> The value of the keyword that's used when mapping a control data source. For example, this can be a CloudTrail event name, a rule name for Config, a Security Hub control, or the name of an Amazon Web Services API call. </p> <p>If you\u2019re mapping a data source to a rule in Config, the <code>keywordValue</code> that you specify depends on the type of rule:</p> <ul> <li> <p>For <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config_use-managed-rules.html\">managed rules</a>, you can use the rule identifier as the <code>keywordValue</code>. You can find the rule identifier from the <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html\">list of Config managed rules</a>. For some rules, the rule identifier is different from the rule name. For example, the rule name <code>restricted-ssh</code> has the following rule identifier: <code>INCOMING_SSH_DISABLED</code>. Make sure to use the rule identifier, not the rule name. </p> <p>Keyword example for managed rules:</p> <ul> <li> <p>Managed rule name: <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-acl-prohibited.html\">s3-bucket-acl-prohibited</a> </p> <p> <code>keywordValue</code>: <code>S3_BUCKET_ACL_PROHIBITED</code> </p> </li> </ul> </li> <li> <p>For <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config_develop-rules.html\">custom rules</a>, you form the <code>keywordValue</code> by adding the <code>Custom_</code> prefix to the rule name. This prefix distinguishes the custom rule from a managed rule. </p> <p>Keyword example for custom rules:</p> <ul> <li> <p>Custom rule name: my-custom-config-rule</p> <p> <code>keywordValue</code>: <code>Custom_my-custom-config-rule</code> </p> </li> </ul> </li> <li> <p>For <a href=\"https://docs.aws.amazon.com/config/latest/developerguide/service-linked-awsconfig-rules.html\">service-linked rules</a>, you form the <code>keywordValue</code> by adding the <code>Custom_</code> prefix to the rule name. In addition, you remove the suffix ID that appears at the end of the rule name. </p> <p>Keyword examples for service-linked rules:</p> <ul> <li> <p>Service-linked rule name: CustomRuleForAccount-conformance-pack-szsm1uv0w</p> <p> <code>keywordValue</code>: <code>Custom_CustomRuleForAccount-conformance-pack</code> </p> </li> <li> <p>Service-linked rule name: OrgConfigRule-s3-bucket-versioning-enabled-dbgzf8ba</p> <p> <code>keywordValue</code>: <code>Custom_OrgConfigRule-s3-bucket-versioning-enabled</code> </p> </li> </ul> </li> </ul> <important> <p>The <code>keywordValue</code> is case sensitive. If you enter a value incorrectly, Audit Manager might not recognize the data source mapping. As a result, you might not successfully collect evidence from that data source as intended. </p> <p>Keep in mind the following requirements, depending on the data source type that you're using. </p> <ol> <li> <p>For Config: </p> <ul> <li> <p>For managed rules, make sure that the <code>keywordValue</code> is the rule identifier in <code>ALL_CAPS_WITH_UNDERSCORES</code>. For example, <code>CLOUDWATCH_LOG_GROUP_ENCRYPTED</code>. For accuracy, we recommend that you reference the list of <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-config.html\">supported Config managed rules</a>.</p> </li> <li> <p>For custom rules, make sure that the <code>keywordValue</code> has the <code>Custom_</code> prefix followed by the custom rule name. The format of the custom rule name itself may vary. For accuracy, we recommend that you visit the <a href=\"https://console.aws.amazon.com/config/\">Config console</a> to verify your custom rule name.</p> </li> </ul> </li> <li> <p>For Security Hub: The format varies for Security Hub control names. For accuracy, we recommend that you reference the list of <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-ash.html\">supported Security Hub controls</a>.</p> </li> <li> <p>For Amazon Web Services API calls: Make sure that the <code>keywordValue</code> is written as <code>serviceprefix_ActionName</code>. For example, <code>iam_ListGroups</code>. For accuracy, we recommend that you reference the list of <a href=\"https://docs.aws.amazon.com/audit-manager/latest/userguide/control-data-sources-api.html\">supported API calls</a>.</p> </li> <li> <p>For CloudTrail: Make sure that the <code>keywordValue</code> is written as <code>serviceprefix_ActionName</code>. For example, <code>cloudtrail_StartLogging</code>. For accuracy, we recommend that you review the Amazon Web Service prefix and action names in the <a href=\"https://docs.aws.amazon.com/service-authorization/latest/reference/reference_policies_actions-resources-contextkeys.html\">Service Authorization Reference</a>.</p> </li> </ol> </important>",
                     "shape": "KeywordValue"
                 }
             },
             "type": "structure"
         },
         "SourceName": {
             "max": 100,
@@ -5959,17 +6064,21 @@
                 }
             },
             "type": "structure"
         },
         "UpdateSettingsRequest": {
             "members": {
                 "defaultAssessmentReportsDestination": {
-                    "documentation": "<p> The default storage destination for assessment reports. </p>",
+                    "documentation": "<p> The default S3 destination bucket for storing assessment reports. </p>",
                     "shape": "AssessmentReportsDestination"
                 },
+                "defaultExportDestination": {
+                    "documentation": "<p> The default S3 destination bucket for storing evidence finder exports. </p>",
+                    "shape": "DefaultExportDestination"
+                },
                 "defaultProcessOwners": {
                     "documentation": "<p> A list of the default audit owners. </p>",
                     "shape": "Roles"
                 },
                 "deregistrationPolicy": {
                     "documentation": "<p>The deregistration policy for your Audit Manager data. You can use this attribute to determine how your data is handled when you deregister Audit Manager.</p>",
                     "shape": "DeregistrationPolicy"
```

### Comparing `botocore-a-la-carte-auditmanager-1.29.99/botocore_a_la_carte_auditmanager.egg-info/PKG-INFO` & `botocore-a-la-carte-auditmanager-1.30.0/botocore_a_la_carte_auditmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-auditmanager
-Version: 1.29.99
+Version: 1.30.0
 Summary: auditmanager data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-auditmanager-1.29.99/setup.py` & `botocore-a-la-carte-auditmanager-1.30.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-auditmanager',
-    version="1.29.99",
+    version="1.30.0",
     description='auditmanager data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/auditmanager/*/*.json'],
```

