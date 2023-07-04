# Comparing `tmp/botocore-a-la-carte-ssm-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-ssm-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ssm-1.29.99.tar", last modified: Sat Mar 25 01:23:06 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ssm-1.30.0.tar", last modified: Tue Jul  4 01:44:58 2023, max compression
```

## Comparing `botocore-a-la-carte-ssm-1.29.99.tar` & `botocore-a-la-carte-ssm-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.264943 botocore-a-la-carte-ssm-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:23:06.260943 botocore-a-la-carte-ssm-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.260943 botocore-a-la-carte-ssm-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.260943 botocore-a-la-carte-ssm-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.260943 botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.260943 botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   808711 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.260943 botocore-a-la-carte-ssm-1.29.99/botocore_a_la_carte_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-1.29.99/botocore_a_la_carte_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-1.29.99/botocore_a_la_carte_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-1.29.99/botocore_a_la_carte_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-1.29.99/botocore_a_la_carte_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:06.264943 botocore-a-la-carte-ssm-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.078810 botocore-a-la-carte-ssm-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:57.000000 botocore-a-la-carte-ssm-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:58.078810 botocore-a-la-carte-ssm-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.074810 botocore-a-la-carte-ssm-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.074810 botocore-a-la-carte-ssm-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.074810 botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.078810 botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   808159 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.078810 botocore-a-la-carte-ssm-1.30.0/botocore_a_la_carte_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-1.30.0/botocore_a_la_carte_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-1.30.0/botocore_a_la_carte_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-1.30.0/botocore_a_la_carte_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-1.30.0/botocore_a_la_carte_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:58.078810 botocore-a-la-carte-ssm-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-04 01:44:57.000000 botocore-a-la-carte-ssm-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-ssm-1.29.99/LICENSE.txt` & `botocore-a-la-carte-ssm-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-1.29.99/PKG-INFO` & `botocore-a-la-carte-ssm-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ssm
-Version: 1.29.99
+Version: 1.30.0
 Summary: ssm data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/endpoint-rule-set-1.json` & `botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/paginators-1.json` & `botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/service-2.json` & `botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8998420909580513%*

 * *Differences: {"'documentation'": "'<p>Amazon Web Services Systems Manager is the operations hub for your Amazon "*

 * *                    'Web Services applications and resources and a secure end-to-end management '*

 * *                    'solution for hybrid cloud environments that enables safe and secure '*

 * *                    'operations at scale.</p> <p>This reference is intended to be used with the <a '*

 * *                    'href="https://docs.aws.amazon.com/systems-manager/latest/userguide/">Amazon '*

 * *                    'W […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p>Amazon Web Services Systems Manager is the operations hub for your Amazon Web Services applications and resources and a secure end-to-end management solution for hybrid cloud environments that enables safe and secure operations at scale.</p> <p>This reference is intended to be used with the <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/\">Amazon Web Services Systems Manager User Guide</a>. To get started, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-setting-up.html\">Setting up Amazon Web Services Systems Manager</a>.</p> <p class=\"title\"> <b>Related resources</b> </p> <ul> <li> <p>For information about each of the capabilities that comprise Systems Manager, see <a href=\"https://docs.aws.amazon.com/systems-manager-automation-runbooks/latest/userguide/what-is-systems-manager.html#systems-manager-capabilities\">Systems Manager capabilities</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> </li> <li> <p>For details about predefined runbooks for Automation, a capability of Amazon Web Services Systems Manager, see the <i> <a href=\"https://docs.aws.amazon.com/systems-manager-automation-runbooks/latest/userguide/automation-runbook-reference.html\">Systems Manager Automation runbook reference</a> </i>.</p> </li> <li> <p>For information about AppConfig, a capability of Systems Manager, see the <i> <a href=\"https://docs.aws.amazon.com/appconfig/latest/userguide/\">AppConfig User Guide</a> </i> and the <i> <a href=\"https://docs.aws.amazon.com/appconfig/2019-10-09/APIReference/\">AppConfig API Reference</a> </i>.</p> </li> <li> <p>For information about Incident Manager, a capability of Systems Manager, see the <i> <a href=\"https://docs.aws.amazon.com/incident-manager/latest/userguide/\">Systems Manager Incident Manager User Guide</a> </i> and the <i> <a href=\"https://docs.aws.amazon.com/incident-manager/latest/APIReference/\">Systems Manager Incident Manager API Reference</a> </i>.</p> </li> </ul>",
+    "documentation": "<p>Amazon Web Services Systems Manager is the operations hub for your Amazon Web Services applications and resources and a secure end-to-end management solution for hybrid cloud environments that enables safe and secure operations at scale.</p> <p>This reference is intended to be used with the <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/\">Amazon Web Services Systems Manager User Guide</a>. To get started, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-setting-up.html\">Setting up Amazon Web Services Systems Manager</a>.</p> <p class=\"title\"> <b>Related resources</b> </p> <ul> <li> <p>For information about each of the capabilities that comprise Systems Manager, see <a href=\"https://docs.aws.amazon.com/systems-manager-automation-runbooks/latest/userguide/systems-manager-capabilities.html\">Systems Manager capabilities</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> </li> <li> <p>For details about predefined runbooks for Automation, a capability of Amazon Web Services Systems Manager, see the <i> <a href=\"https://docs.aws.amazon.com/systems-manager-automation-runbooks/latest/userguide/automation-runbook-reference.html\">Systems Manager Automation runbook reference</a> </i>.</p> </li> <li> <p>For information about AppConfig, a capability of Systems Manager, see the <i> <a href=\"https://docs.aws.amazon.com/appconfig/latest/userguide/\">AppConfig User Guide</a> </i> and the <i> <a href=\"https://docs.aws.amazon.com/appconfig/2019-10-09/APIReference/\">AppConfig API Reference</a> </i>.</p> </li> <li> <p>For information about Incident Manager, a capability of Systems Manager, see the <i> <a href=\"https://docs.aws.amazon.com/incident-manager/latest/userguide/\">Systems Manager Incident Manager User Guide</a> </i> and the <i> <a href=\"https://docs.aws.amazon.com/incident-manager/latest/APIReference/\">Systems Manager Incident Manager API Reference</a> </i>.</p> </li> </ul>",
     "metadata": {
         "apiVersion": "2014-11-06",
         "endpointPrefix": "ssm",
         "jsonVersion": "1.1",
         "protocol": "json",
         "serviceAbbreviation": "Amazon SSM",
         "serviceFullName": "Amazon Simple Systems Manager (SSM)",
@@ -310,15 +310,15 @@
             },
             "name": "CreateMaintenanceWindow",
             "output": {
                 "shape": "CreateMaintenanceWindowResult"
             }
         },
         "CreateOpsItem": {
-            "documentation": "<p>Creates a new OpsItem. You must have permission in Identity and Access Management (IAM) to create a new OpsItem. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-getting-started.html\">Getting started with OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Operations engineers and IT professionals use Amazon Web Services Systems Manager OpsCenter to view, investigate, and remediate operational issues impacting the performance and health of their Amazon Web Services resources. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter.html\">Amazon Web Services Systems Manager OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>. </p>",
+            "documentation": "<p>Creates a new OpsItem. You must have permission in Identity and Access Management (IAM) to create a new OpsItem. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-setup.html\">Set up OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Operations engineers and IT professionals use Amazon Web Services Systems Manager OpsCenter to view, investigate, and remediate operational issues impacting the performance and health of their Amazon Web Services resources. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter.html\">Amazon Web Services Systems Manager OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>. </p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 },
                 {
                     "shape": "OpsItemAlreadyExistsException"
                 },
@@ -1112,15 +1112,15 @@
             },
             "name": "DescribeInstanceAssociationsStatus",
             "output": {
                 "shape": "DescribeInstanceAssociationsStatusResult"
             }
         },
         "DescribeInstanceInformation": {
-            "documentation": "<p>Describes one or more of your managed nodes, including information about the operating system platform, the version of SSM Agent installed on the managed node, node status, and so on.</p> <p>If you specify one or more managed node IDs, it returns information for those managed nodes. If you don't specify node IDs, it returns information for all your managed nodes. If you specify a node ID that isn't valid or a node that you don't own, you receive an error.</p> <note> <p>The <code>IamRole</code> field for this API operation is the Identity and Access Management (IAM) role assigned to on-premises managed nodes. This call doesn't return the IAM role for EC2 instances.</p> </note>",
+            "documentation": "<p>Provides information about one or more of your managed nodes, including the operating system platform, SSM Agent version, association status, and IP address. This operation does not return information for nodes that are either Stopped or Terminated.</p> <p>If you specify one or more node IDs, the operation returns information for those managed nodes. If you don't specify node IDs, it returns information for all your managed nodes. If you specify a node ID that isn't valid or a node that you don't own, you receive an error.</p> <note> <p>The <code>IamRole</code> field returned for this API operation is the Identity and Access Management (IAM) role assigned to on-premises managed nodes. This operation does not return the IAM role for EC2 instances.</p> </note>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 },
                 {
                     "shape": "InvalidInstanceId"
                 },
@@ -1410,15 +1410,15 @@
             },
             "name": "DescribeMaintenanceWindowsForTarget",
             "output": {
                 "shape": "DescribeMaintenanceWindowsForTargetResult"
             }
         },
         "DescribeOpsItems": {
-            "documentation": "<p>Query a set of OpsItems. You must have permission in Identity and Access Management (IAM) to query a list of OpsItems. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-getting-started.html\">Getting started with OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Operations engineers and IT professionals use Amazon Web Services Systems Manager OpsCenter to view, investigate, and remediate operational issues impacting the performance and health of their Amazon Web Services resources. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter.html\">OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>. </p>",
+            "documentation": "<p>Query a set of OpsItems. You must have permission in Identity and Access Management (IAM) to query a list of OpsItems. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-setup.html\">Set up OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Operations engineers and IT professionals use Amazon Web Services Systems Manager OpsCenter to view, investigate, and remediate operational issues impacting the performance and health of their Amazon Web Services resources. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter.html\">OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>. </p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1933,15 +1933,15 @@
             },
             "name": "GetMaintenanceWindowTask",
             "output": {
                 "shape": "GetMaintenanceWindowTaskResult"
             }
         },
         "GetOpsItem": {
-            "documentation": "<p>Get information about an OpsItem by using the ID. You must have permission in Identity and Access Management (IAM) to view information about an OpsItem. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-getting-started.html\">Getting started with OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Operations engineers and IT professionals use Amazon Web Services Systems Manager OpsCenter to view, investigate, and remediate operational issues impacting the performance and health of their Amazon Web Services resources. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter.html\">OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>. </p>",
+            "documentation": "<p>Get information about an OpsItem by using the ID. You must have permission in Identity and Access Management (IAM) to view information about an OpsItem. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-setup.html\">Set up OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Operations engineers and IT professionals use Amazon Web Services Systems Manager OpsCenter to view, investigate, and remediate operational issues impacting the performance and health of their Amazon Web Services resources. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter.html\">OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>. </p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 },
                 {
                     "shape": "OpsItemNotFoundException"
                 },
@@ -3617,15 +3617,15 @@
             },
             "name": "UpdateManagedInstanceRole",
             "output": {
                 "shape": "UpdateManagedInstanceRoleResult"
             }
         },
         "UpdateOpsItem": {
-            "documentation": "<p>Edit or change an OpsItem. You must have permission in Identity and Access Management (IAM) to update an OpsItem. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-getting-started.html\">Getting started with OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Operations engineers and IT professionals use Amazon Web Services Systems Manager OpsCenter to view, investigate, and remediate operational issues impacting the performance and health of their Amazon Web Services resources. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter.html\">OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>. </p>",
+            "documentation": "<p>Edit or change an OpsItem. You must have permission in Identity and Access Management (IAM) to update an OpsItem. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-setup.html\">Set up OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Operations engineers and IT professionals use Amazon Web Services Systems Manager OpsCenter to view, investigate, and remediate operational issues impacting the performance and health of their Amazon Web Services resources. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter.html\">OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>. </p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 },
                 {
                     "shape": "OpsItemNotFoundException"
                 },
@@ -3870,15 +3870,15 @@
                 "shape": "Activation"
             },
             "type": "list"
         },
         "AddTagsToResourceRequest": {
             "members": {
                 "ResourceId": {
-                    "documentation": "<p>The resource ID you want to tag.</p> <p>Use the ID of the resource. Here are some examples:</p> <p> <code>MaintenanceWindow</code>: <code>mw-012345abcde</code> </p> <p> <code>PatchBaseline</code>: <code>pb-012345abcde</code> </p> <p> <code>Automation</code>: <code>example-c160-4567-8519-012345abcde</code> </p> <p> <code>OpsMetadata</code> object: <code>ResourceID</code> for tagging is created from the Amazon Resource Name (ARN) for the object. Specifically, <code>ResourceID</code> is created from the strings that come after the word <code>opsmetadata</code> in the ARN. For example, an OpsMetadata object with an ARN of <code>arn:aws:ssm:us-east-2:1234567890:opsmetadata/aws/ssm/MyGroup/appmanager</code> has a <code>ResourceID</code> of either <code>aws/ssm/MyGroup/appmanager</code> or <code>/aws/ssm/MyGroup/appmanager</code>.</p> <p>For the <code>Document</code> and <code>Parameter</code> values, use the name of the resource.</p> <p> <code>ManagedInstance</code>: <code>mi-012345abcde</code> </p> <note> <p>The <code>ManagedInstance</code> type for this API operation is only for on-premises managed nodes. You must specify the name of the managed node in the following format: <code>mi-<i>ID_number</i> </code>. For example, <code>mi-1a2b3c4d5e6f</code>.</p> </note>",
+                    "documentation": "<p>The resource ID you want to tag.</p> <p>Use the ID of the resource. Here are some examples:</p> <p> <code>MaintenanceWindow</code>: <code>mw-012345abcde</code> </p> <p> <code>PatchBaseline</code>: <code>pb-012345abcde</code> </p> <p> <code>Automation</code>: <code>example-c160-4567-8519-012345abcde</code> </p> <p> <code>OpsMetadata</code> object: <code>ResourceID</code> for tagging is created from the Amazon Resource Name (ARN) for the object. Specifically, <code>ResourceID</code> is created from the strings that come after the word <code>opsmetadata</code> in the ARN. For example, an OpsMetadata object with an ARN of <code>arn:aws:ssm:us-east-2:1234567890:opsmetadata/aws/ssm/MyGroup/appmanager</code> has a <code>ResourceID</code> of either <code>aws/ssm/MyGroup/appmanager</code> or <code>/aws/ssm/MyGroup/appmanager</code>.</p> <p>For the <code>Document</code> and <code>Parameter</code> values, use the name of the resource. If you're tagging a shared document, you must use the full ARN of the document.</p> <p> <code>ManagedInstance</code>: <code>mi-012345abcde</code> </p> <note> <p>The <code>ManagedInstance</code> type for this API operation is only for on-premises managed nodes. You must specify the name of the managed node in the following format: <code>mi-<i>ID_number</i> </code>. For example, <code>mi-1a2b3c4d5e6f</code>.</p> </note>",
                     "shape": "ResourceId"
                 },
                 "ResourceType": {
                     "documentation": "<p>Specifies the type of resource you are tagging.</p> <note> <p>The <code>ManagedInstance</code> type for this API operation is for on-premises managed nodes. You must specify the name of the managed node in the following format: <code>mi-<i>ID_number</i> </code>. For example, <code>mi-1a2b3c4d5e6f</code>.</p> </note>",
                     "shape": "ResourceTypeForTagging"
                 },
                 "Tags": {
@@ -6526,15 +6526,15 @@
                 }
             },
             "type": "structure"
         },
         "CreateOpsItemRequest": {
             "members": {
                 "AccountId": {
-                    "documentation": "<p>The target Amazon Web Services account where you want to create an OpsItem. To make this call, your account must be configured to work with OpsItems across accounts. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-OpsCenter-multiple-accounts.html\">Setting up OpsCenter to work with OpsItems across accounts</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
+                    "documentation": "<p>The target Amazon Web Services account where you want to create an OpsItem. To make this call, your account must be configured to work with OpsItems across accounts. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-setup.html\">Set up OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
                     "shape": "OpsItemAccountId"
                 },
                 "ActualEndTime": {
                     "documentation": "<p>The time a runbook workflow ended. Currently reported only for the OpsItem type <code>/aws/changerequest</code>.</p>",
                     "shape": "DateTime"
                 },
                 "ActualStartTime": {
@@ -6550,15 +6550,15 @@
                     "shape": "OpsItemDescription"
                 },
                 "Notifications": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an SNS topic where notifications are sent when this OpsItem is edited or changed.</p>",
                     "shape": "OpsItemNotifications"
                 },
                 "OperationalData": {
-                    "documentation": "<p>Operational data is custom data that provides useful reference details about the OpsItem. For example, you can specify log files, error strings, license keys, troubleshooting tips, or other relevant data. You enter operational data as key-value pairs. The key has a maximum length of 128 characters. The value has a maximum size of 20 KB.</p> <important> <p>Operational data keys <i>can't</i> begin with the following: <code>amazon</code>, <code>aws</code>, <code>amzn</code>, <code>ssm</code>, <code>/amazon</code>, <code>/aws</code>, <code>/amzn</code>, <code>/ssm</code>.</p> </important> <p>You can choose to make the data searchable by other users in the account or you can restrict search access. Searchable data means that all users with access to the OpsItem Overview page (as provided by the <a>DescribeOpsItems</a> API operation) can view and search on the specified data. Operational data that isn't searchable is only viewable by users who have access to the OpsItem (as provided by the <a>GetOpsItem</a> API operation).</p> <p>Use the <code>/aws/resources</code> key in OperationalData to specify a related resource in the request. Use the <code>/aws/automations</code> key in OperationalData to associate an Automation runbook with the OpsItem. To view Amazon Web Services CLI example commands that use these keys, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-creating-OpsItems.html#OpsCenter-manually-create-OpsItems\">Creating OpsItems manually</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
+                    "documentation": "<p>Operational data is custom data that provides useful reference details about the OpsItem. For example, you can specify log files, error strings, license keys, troubleshooting tips, or other relevant data. You enter operational data as key-value pairs. The key has a maximum length of 128 characters. The value has a maximum size of 20 KB.</p> <important> <p>Operational data keys <i>can't</i> begin with the following: <code>amazon</code>, <code>aws</code>, <code>amzn</code>, <code>ssm</code>, <code>/amazon</code>, <code>/aws</code>, <code>/amzn</code>, <code>/ssm</code>.</p> </important> <p>You can choose to make the data searchable by other users in the account or you can restrict search access. Searchable data means that all users with access to the OpsItem Overview page (as provided by the <a>DescribeOpsItems</a> API operation) can view and search on the specified data. Operational data that isn't searchable is only viewable by users who have access to the OpsItem (as provided by the <a>GetOpsItem</a> API operation).</p> <p>Use the <code>/aws/resources</code> key in OperationalData to specify a related resource in the request. Use the <code>/aws/automations</code> key in OperationalData to associate an Automation runbook with the OpsItem. To view Amazon Web Services CLI example commands that use these keys, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-manually-create-OpsItems.html\">Creating OpsItems manually</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
                     "shape": "OpsItemOperationalData"
                 },
                 "OpsItemType": {
                     "documentation": "<p>The type of OpsItem to create. Systems Manager supports the following types of OpsItems:</p> <ul> <li> <p> <code>/aws/issue</code> </p> <p>This type of OpsItem is used for default OpsItems created by OpsCenter. </p> </li> <li> <p> <code>/aws/changerequest</code> </p> <p>This type of OpsItem is used by Change Manager for reviewing and approving or rejecting change requests. </p> </li> <li> <p> <code>/aws/insights</code> </p> <p>This type of OpsItem is used by OpsCenter for aggregating and reporting on duplicate OpsItems. </p> </li> </ul>",
                     "shape": "OpsItemType"
                 },
                 "PlannedEndTime": {
@@ -6582,15 +6582,15 @@
                     "shape": "OpsItemSeverity"
                 },
                 "Source": {
                     "documentation": "<p>The origin of the OpsItem, such as Amazon EC2 or Systems Manager.</p> <note> <p>The source name can't contain the following strings: <code>aws</code>, <code>amazon</code>, and <code>amzn</code>. </p> </note>",
                     "shape": "OpsItemSource"
                 },
                 "Tags": {
-                    "documentation": "<p>Optional metadata that you assign to a resource. You can restrict access to OpsItems by using an inline IAM policy that specifies tags. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-getting-started.html#OpsCenter-getting-started-user-permissions\">Getting started with OpsCenter</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p> <p>Tags use a key-value pair. For example:</p> <p> <code>Key=Department,Value=Finance</code> </p> <important> <p>To add tags to a new OpsItem, a user must have IAM permissions for both the <code>ssm:CreateOpsItems</code> operation and the <code>ssm:AddTagsToResource</code> operation. To add tags to an existing OpsItem, use the <a>AddTagsToResource</a> operation.</p> </important>",
+                    "documentation": "<p>Optional metadata that you assign to a resource.</p> <p>Tags use a key-value pair. For example:</p> <p> <code>Key=Department,Value=Finance</code> </p> <important> <p>To add tags to a new OpsItem, a user must have IAM permissions for both the <code>ssm:CreateOpsItems</code> operation and the <code>ssm:AddTagsToResource</code> operation. To add tags to an existing OpsItem, use the <a>AddTagsToResource</a> operation.</p> </important>",
                     "shape": "TagList"
                 },
                 "Title": {
                     "documentation": "<p>A short heading that describes the nature of the OpsItem and the impacted resource.</p>",
                     "shape": "OpsItemTitle"
                 }
             },
@@ -7581,24 +7581,24 @@
                 }
             },
             "type": "structure"
         },
         "DescribeInstanceInformationRequest": {
             "members": {
                 "Filters": {
-                    "documentation": "<p>One or more filters. Use a filter to return a more specific list of managed nodes. You can filter based on tags applied to your managed nodes. Use this <code>Filters</code> data type instead of <code>InstanceInformationFilterList</code>, which is deprecated.</p>",
+                    "documentation": "<p>One or more filters. Use a filter to return a more specific list of managed nodes. You can filter based on tags applied to your managed nodes. Tag filters can't be combined with other filter types. Use this <code>Filters</code> data type instead of <code>InstanceInformationFilterList</code>, which is deprecated.</p>",
                     "shape": "InstanceInformationStringFilterList"
                 },
                 "InstanceInformationFilterList": {
                     "documentation": "<p>This is a legacy method. We recommend that you don't use this method. Instead, use the <code>Filters</code> data type. <code>Filters</code> enables you to return node information by filtering based on tags applied to managed nodes.</p> <note> <p>Attempting to use <code>InstanceInformationFilterList</code> and <code>Filters</code> leads to an exception error. </p> </note>",
                     "shape": "InstanceInformationFilterList"
                 },
                 "MaxResults": {
                     "box": true,
-                    "documentation": "<p>The maximum number of items to return for this call. The call also returns a token that you can specify in a subsequent call to get the next set of results. </p>",
+                    "documentation": "<p>The maximum number of items to return for this call. The call also returns a token that you can specify in a subsequent call to get the next set of results. The default value is 10 items. </p>",
                     "shape": "MaxResultsEC2Compatible"
                 },
                 "NextToken": {
                     "documentation": "<p>The token for the next set of items to return. (You received this token from a previous call.)</p>",
                     "shape": "NextToken"
                 }
             },
@@ -8073,15 +8073,15 @@
                     "shape": "OpsItemMaxResults"
                 },
                 "NextToken": {
                     "documentation": "<p>A token to start the list. Use this token to get the next set of results.</p>",
                     "shape": "String"
                 },
                 "OpsItemFilters": {
-                    "documentation": "<p>One or more filters to limit the response.</p> <ul> <li> <p>Key: CreatedTime</p> <p>Operations: GreaterThan, LessThan</p> </li> <li> <p>Key: LastModifiedBy</p> <p>Operations: Contains, Equals</p> </li> <li> <p>Key: LastModifiedTime</p> <p>Operations: GreaterThan, LessThan</p> </li> <li> <p>Key: Priority</p> <p>Operations: Equals</p> </li> <li> <p>Key: Source</p> <p>Operations: Contains, Equals</p> </li> <li> <p>Key: Status</p> <p>Operations: Equals</p> </li> <li> <p>Key: Title*</p> <p>Operations: Equals,Contains</p> </li> <li> <p>Key: OperationalData**</p> <p>Operations: Equals</p> </li> <li> <p>Key: OperationalDataKey</p> <p>Operations: Equals</p> </li> <li> <p>Key: OperationalDataValue</p> <p>Operations: Equals, Contains</p> </li> <li> <p>Key: OpsItemId</p> <p>Operations: Equals</p> </li> <li> <p>Key: ResourceId</p> <p>Operations: Contains</p> </li> <li> <p>Key: AutomationId</p> <p>Operations: Equals</p> </li> </ul> <p>*The Equals operator for Title matches the first 100 characters. If you specify more than 100 characters, they system returns an error that the filter value exceeds the length limit.</p> <p>**If you filter the response by using the OperationalData operator, specify a key-value pair by using the following JSON format: {\"key\":\"key_name\",\"value\":\"a_value\"}</p>",
+                    "documentation": "<p>One or more filters to limit the response.</p> <ul> <li> <p>Key: CreatedTime</p> <p>Operations: GreaterThan, LessThan</p> </li> <li> <p>Key: LastModifiedBy</p> <p>Operations: Contains, Equals</p> </li> <li> <p>Key: LastModifiedTime</p> <p>Operations: GreaterThan, LessThan</p> </li> <li> <p>Key: Priority</p> <p>Operations: Equals</p> </li> <li> <p>Key: Source</p> <p>Operations: Contains, Equals</p> </li> <li> <p>Key: Status</p> <p>Operations: Equals</p> </li> <li> <p>Key: Title*</p> <p>Operations: Equals,Contains</p> </li> <li> <p>Key: OperationalData**</p> <p>Operations: Equals</p> </li> <li> <p>Key: OperationalDataKey</p> <p>Operations: Equals</p> </li> <li> <p>Key: OperationalDataValue</p> <p>Operations: Equals, Contains</p> </li> <li> <p>Key: OpsItemId</p> <p>Operations: Equals</p> </li> <li> <p>Key: ResourceId</p> <p>Operations: Contains</p> </li> <li> <p>Key: AutomationId</p> <p>Operations: Equals</p> </li> <li> <p>Key: AccountId</p> <p>Operations: Equals</p> </li> </ul> <p>*The Equals operator for Title matches the first 100 characters. If you specify more than 100 characters, they system returns an error that the filter value exceeds the length limit.</p> <p>**If you filter the response by using the OperationalData operator, specify a key-value pair by using the following JSON format: {\"key\":\"key_name\",\"value\":\"a_value\"}</p>",
                     "shape": "OpsItemFilters"
                 }
             },
             "type": "structure"
         },
         "DescribeOpsItemsResponse": {
             "members": {
@@ -10650,15 +10650,15 @@
                     "shape": "ComputerName"
                 },
                 "IPAddress": {
                     "documentation": "<p>The IP address of the managed node.</p>",
                     "shape": "IPAddress"
                 },
                 "IamRole": {
-                    "documentation": "<p>The Identity and Access Management (IAM) role assigned to the on-premises Systems Manager managed node. This call doesn't return the IAM role for Amazon Elastic Compute Cloud (Amazon EC2) instances. To retrieve the IAM role for an EC2 instance, use the Amazon EC2 <code>DescribeInstances</code> operation. For information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html\">DescribeInstances</a> in the <i>Amazon EC2 API Reference</i> or <a href=\"https://docs.aws.amazon.com/cli/latest/ec2/describe-instances.html\">describe-instances</a> in the <i>Amazon Web Services CLI Command Reference</i>.</p>",
+                    "documentation": "<p>The Identity and Access Management (IAM) role assigned to the on-premises Systems Manager managed node. This call doesn't return the IAM role for Amazon Elastic Compute Cloud (Amazon EC2) instances. To retrieve the IAM role for an EC2 instance, use the Amazon EC2 <code>DescribeInstances</code> operation. For information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html\">DescribeInstances</a> in the <i>Amazon EC2 API Reference</i> or <a href=\"https://docs.aws.amazon.com/cli/latest/reference/ec2/describe-instances.html\">describe-instances</a> in the <i>Amazon Web Services CLI Command Reference</i>.</p>",
                     "shape": "IamRole"
                 },
                 "InstanceId": {
                     "documentation": "<p>The managed node ID. </p>",
                     "shape": "InstanceId"
                 },
                 "IsLatestVersion": {
@@ -10676,15 +10676,15 @@
                     "shape": "DateTime"
                 },
                 "LastSuccessfulAssociationExecutionDate": {
                     "documentation": "<p>The last date the association was successfully run.</p>",
                     "shape": "DateTime"
                 },
                 "Name": {
-                    "documentation": "<p>The name assigned to an on-premises server, edge device, or virtual machine (VM) when it is activated as a Systems Manager managed node. The name is specified as the <code>DefaultInstanceName</code> property using the <a>CreateActivation</a> command. It is applied to the managed node by specifying the Activation Code and Activation ID when you install SSM Agent on the node, as explained in <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-install-managed-linux.html\">Install SSM Agent for a hybrid environment (Linux)</a> and <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-install-managed-win.html\">Install SSM Agent for a hybrid environment (Windows)</a>. To retrieve the <code>Name</code> tag of an EC2 instance, use the Amazon EC2 <code>DescribeInstances</code> operation. For information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html\">DescribeInstances</a> in the <i>Amazon EC2 API Reference</i> or <a href=\"https://docs.aws.amazon.com/cli/latest/ec2/describe-instances.html\">describe-instances</a> in the <i>Amazon Web Services CLI Command Reference</i>.</p>",
+                    "documentation": "<p>The name assigned to an on-premises server, edge device, or virtual machine (VM) when it is activated as a Systems Manager managed node. The name is specified as the <code>DefaultInstanceName</code> property using the <a>CreateActivation</a> command. It is applied to the managed node by specifying the Activation Code and Activation ID when you install SSM Agent on the node, as explained in <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-install-managed-linux.html\">Install SSM Agent for a hybrid environment (Linux)</a> and <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-install-managed-win.html\">Install SSM Agent for a hybrid environment (Windows)</a>. To retrieve the <code>Name</code> tag of an EC2 instance, use the Amazon EC2 <code>DescribeInstances</code> operation. For information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html\">DescribeInstances</a> in the <i>Amazon EC2 API Reference</i> or <a href=\"https://docs.aws.amazon.com/cli/latest/reference/ec2/describe-instances.html\">describe-instances</a> in the <i>Amazon Web Services CLI Command Reference</i>.</p>",
                     "shape": "String"
                 },
                 "PingStatus": {
                     "documentation": "<p>Connection status of SSM Agent. </p> <note> <p>The status <code>Inactive</code> has been deprecated and is no longer in use.</p> </note>",
                     "shape": "PingStatus"
                 },
                 "PlatformName": {
@@ -13815,15 +13815,15 @@
                     "shape": "DateTime"
                 },
                 "Notifications": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an Amazon Simple Notification Service (Amazon SNS) topic where notifications are sent when this OpsItem is edited or changed.</p>",
                     "shape": "OpsItemNotifications"
                 },
                 "OperationalData": {
-                    "documentation": "<p>Operational data is custom data that provides useful reference details about the OpsItem. For example, you can specify log files, error strings, license keys, troubleshooting tips, or other relevant data. You enter operational data as key-value pairs. The key has a maximum length of 128 characters. The value has a maximum size of 20 KB.</p> <important> <p>Operational data keys <i>can't</i> begin with the following: <code>amazon</code>, <code>aws</code>, <code>amzn</code>, <code>ssm</code>, <code>/amazon</code>, <code>/aws</code>, <code>/amzn</code>, <code>/ssm</code>.</p> </important> <p>You can choose to make the data searchable by other users in the account or you can restrict search access. Searchable data means that all users with access to the OpsItem Overview page (as provided by the <a>DescribeOpsItems</a> API operation) can view and search on the specified data. Operational data that isn't searchable is only viewable by users who have access to the OpsItem (as provided by the <a>GetOpsItem</a> API operation).</p> <p>Use the <code>/aws/resources</code> key in OperationalData to specify a related resource in the request. Use the <code>/aws/automations</code> key in OperationalData to associate an Automation runbook with the OpsItem. To view Amazon Web Services CLI example commands that use these keys, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-creating-OpsItems.html#OpsCenter-manually-create-OpsItems\">Creating OpsItems manually</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
+                    "documentation": "<p>Operational data is custom data that provides useful reference details about the OpsItem. For example, you can specify log files, error strings, license keys, troubleshooting tips, or other relevant data. You enter operational data as key-value pairs. The key has a maximum length of 128 characters. The value has a maximum size of 20 KB.</p> <important> <p>Operational data keys <i>can't</i> begin with the following: <code>amazon</code>, <code>aws</code>, <code>amzn</code>, <code>ssm</code>, <code>/amazon</code>, <code>/aws</code>, <code>/amzn</code>, <code>/ssm</code>.</p> </important> <p>You can choose to make the data searchable by other users in the account or you can restrict search access. Searchable data means that all users with access to the OpsItem Overview page (as provided by the <a>DescribeOpsItems</a> API operation) can view and search on the specified data. Operational data that isn't searchable is only viewable by users who have access to the OpsItem (as provided by the <a>GetOpsItem</a> API operation).</p> <p>Use the <code>/aws/resources</code> key in OperationalData to specify a related resource in the request. Use the <code>/aws/automations</code> key in OperationalData to associate an Automation runbook with the OpsItem. To view Amazon Web Services CLI example commands that use these keys, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-manually-create-OpsItems.html\">Creating OpsItems manually</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
                     "shape": "OpsItemOperationalData"
                 },
                 "OpsItemArn": {
                     "documentation": "<p>The OpsItem Amazon Resource Name (ARN).</p>",
                     "shape": "OpsItemArn"
                 },
                 "OpsItemId": {
@@ -14151,15 +14151,15 @@
                 "ParameterNames": {
                     "shape": "OpsItemParameterNamesList"
                 }
             },
             "type": "structure"
         },
         "OpsItemLimitExceededException": {
-            "documentation": "<p>The request caused OpsItems to exceed one or more quotas. For information about OpsItem quotas, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-learn-more.html#OpsCenter-learn-more-limits\">What are the resource limits for OpsCenter?</a>.</p>",
+            "documentation": "<p>The request caused OpsItems to exceed one or more quotas.</p>",
             "exception": true,
             "members": {
                 "Limit": {
                     "shape": "Integer"
                 },
                 "LimitType": {
                     "shape": "String"
@@ -18958,15 +18958,15 @@
                     "shape": "OpsItemDescription"
                 },
                 "Notifications": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an SNS topic where notifications are sent when this OpsItem is edited or changed.</p>",
                     "shape": "OpsItemNotifications"
                 },
                 "OperationalData": {
-                    "documentation": "<p>Add new keys or edit existing key-value pairs of the OperationalData map in the OpsItem object.</p> <p>Operational data is custom data that provides useful reference details about the OpsItem. For example, you can specify log files, error strings, license keys, troubleshooting tips, or other relevant data. You enter operational data as key-value pairs. The key has a maximum length of 128 characters. The value has a maximum size of 20 KB.</p> <important> <p>Operational data keys <i>can't</i> begin with the following: <code>amazon</code>, <code>aws</code>, <code>amzn</code>, <code>ssm</code>, <code>/amazon</code>, <code>/aws</code>, <code>/amzn</code>, <code>/ssm</code>.</p> </important> <p>You can choose to make the data searchable by other users in the account or you can restrict search access. Searchable data means that all users with access to the OpsItem Overview page (as provided by the <a>DescribeOpsItems</a> API operation) can view and search on the specified data. Operational data that isn't searchable is only viewable by users who have access to the OpsItem (as provided by the <a>GetOpsItem</a> API operation).</p> <p>Use the <code>/aws/resources</code> key in OperationalData to specify a related resource in the request. Use the <code>/aws/automations</code> key in OperationalData to associate an Automation runbook with the OpsItem. To view Amazon Web Services CLI example commands that use these keys, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-creating-OpsItems.html#OpsCenter-manually-create-OpsItems\">Creating OpsItems manually</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
+                    "documentation": "<p>Add new keys or edit existing key-value pairs of the OperationalData map in the OpsItem object.</p> <p>Operational data is custom data that provides useful reference details about the OpsItem. For example, you can specify log files, error strings, license keys, troubleshooting tips, or other relevant data. You enter operational data as key-value pairs. The key has a maximum length of 128 characters. The value has a maximum size of 20 KB.</p> <important> <p>Operational data keys <i>can't</i> begin with the following: <code>amazon</code>, <code>aws</code>, <code>amzn</code>, <code>ssm</code>, <code>/amazon</code>, <code>/aws</code>, <code>/amzn</code>, <code>/ssm</code>.</p> </important> <p>You can choose to make the data searchable by other users in the account or you can restrict search access. Searchable data means that all users with access to the OpsItem Overview page (as provided by the <a>DescribeOpsItems</a> API operation) can view and search on the specified data. Operational data that isn't searchable is only viewable by users who have access to the OpsItem (as provided by the <a>GetOpsItem</a> API operation).</p> <p>Use the <code>/aws/resources</code> key in OperationalData to specify a related resource in the request. Use the <code>/aws/automations</code> key in OperationalData to associate an Automation runbook with the OpsItem. To view Amazon Web Services CLI example commands that use these keys, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-manually-create-OpsItems.html\">Creating OpsItems manually</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
                     "shape": "OpsItemOperationalData"
                 },
                 "OperationalDataToDelete": {
                     "documentation": "<p>Keys that you want to remove from the OperationalData map.</p>",
                     "shape": "OpsItemOpsDataKeysList"
                 },
                 "OpsItemArn": {
@@ -18994,15 +18994,15 @@
                     "shape": "RelatedOpsItems"
                 },
                 "Severity": {
                     "documentation": "<p>Specify a new severity for an OpsItem.</p>",
                     "shape": "OpsItemSeverity"
                 },
                 "Status": {
-                    "documentation": "<p>The OpsItem status. Status can be <code>Open</code>, <code>In Progress</code>, or <code>Resolved</code>. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-working-with-OpsItems.html#OpsCenter-working-with-OpsItems-editing-details\">Editing OpsItem details</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
+                    "documentation": "<p>The OpsItem status. Status can be <code>Open</code>, <code>In Progress</code>, or <code>Resolved</code>. For more information, see <a href=\"https://docs.aws.amazon.com/systems-manager/latest/userguide/OpsCenter-working-with-OpsItems-editing-details.html\">Editing OpsItem details</a> in the <i>Amazon Web Services Systems Manager User Guide</i>.</p>",
                     "shape": "OpsItemStatus"
                 },
                 "Title": {
                     "documentation": "<p>A short heading that describes the nature of the OpsItem and the impacted resource.</p>",
                     "shape": "OpsItemTitle"
                 }
             },
```

### Comparing `botocore-a-la-carte-ssm-1.29.99/botocore/data/ssm/2014-11-06/waiters-2.json` & `botocore-a-la-carte-ssm-1.30.0/botocore/data/ssm/2014-11-06/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-1.29.99/botocore_a_la_carte_ssm.egg-info/PKG-INFO` & `botocore-a-la-carte-ssm-1.30.0/botocore_a_la_carte_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ssm
-Version: 1.29.99
+Version: 1.30.0
 Summary: ssm data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ssm-1.29.99/setup.py` & `botocore-a-la-carte-ssm-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ssm',
-    version="1.29.99",
+    version="1.30.0",
     description='ssm data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ssm/*/*.json'],
```

