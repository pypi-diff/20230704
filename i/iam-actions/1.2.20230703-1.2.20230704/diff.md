# Comparing `tmp/iam_actions-1.2.20230703.tar.gz` & `tmp/iam_actions-1.2.20230704.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230703.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230704.tar", max compression
```

## Comparing `iam_actions-1.2.20230703.tar` & `iam_actions-1.2.20230704.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/README.md
--rw-r--r--   0        0        0      228 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/__init__.py
--rw-r--r--   0        0        0  4362506 2023-07-03 02:53:51.930833 iam_actions-1.2.20230703/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-03 02:52:02.540667 iam_actions-1.2.20230703/iam_actions/generate/services.py
--rw-r--r--   0        0        0   560956 2023-07-03 02:53:51.930833 iam_actions-1.2.20230703/iam_actions/policies.json
--rw-r--r--   0        0        0   197380 2023-07-03 02:53:51.930833 iam_actions-1.2.20230703/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   544073 2023-07-03 02:53:51.930833 iam_actions-1.2.20230703/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-03 02:53:52.706848 iam_actions-1.2.20230703/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230703/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230703/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/README.md
+-rw-r--r--   0        0        0      228 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4362696 2023-07-04 02:56:01.959111 iam_actions-1.2.20230704/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   560956 2023-07-04 02:56:01.959111 iam_actions-1.2.20230704/iam_actions/policies.json
+-rw-r--r--   0        0        0   197380 2023-07-04 02:56:01.959111 iam_actions-1.2.20230704/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   544073 2023-07-04 02:56:01.959111 iam_actions-1.2.20230704/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-04 02:56:02.963124 iam_actions-1.2.20230704/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230704/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230704/PKG-INFO
```

### Comparing `iam_actions-1.2.20230703/LICENSE` & `iam_actions-1.2.20230704/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/README.md` & `iam_actions-1.2.20230704/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/actions.json` & `iam_actions-1.2.20230704/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999955226019055%*

 * *Differences: {"'redshift'": "{'DescribeCustomDomainAssociations': {'access_level': 'List', 'description': "*

 * *               "'Grants permission to describe custom domain names for a cluster'}, "*

 * *               "'ModifyCustomDomainAssociation': {'access_level': 'Write', 'description': 'Grants "*

 * *               "permission to modify a custom domain name for a cluster', 'resources': "*

 * *               "['cluster']}, 'DeleteCustomDomainAssociation': {'access_level': 'Write', "*

 * *               "'description': 'Grants permission t […]*

```diff
@@ -115725,20 +115725,22 @@
             "description": "Grants permission to automatically create the specified Amazon Redshift user if it does not exist",
             "orphan": false,
             "resources": [
                 "dbuser"
             ]
         },
         "CreateCustomDomainAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCustomDomainAssociation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a custom domain name for a cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "CreateEndpointAccess": {
             "access_level": "Write",
             "action": "CreateEndpointAccess",
             "condition_keys": [],
             "description": "Grants permission to create a redshift-managed vpc endpoint",
             "orphan": false,
@@ -115933,20 +115935,22 @@
             "description": "Grants permission to delete a cluster subnet group",
             "orphan": false,
             "resources": [
                 "subnetgroup"
             ]
         },
         "DeleteCustomDomainAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteCustomDomainAssociation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a custom domain name for a cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "DeleteEndpointAccess": {
             "access_level": "Write",
             "action": "DeleteEndpointAccess",
             "condition_keys": [],
             "description": "Grants permission to delete a redshift-managed vpc endpoint",
             "orphan": false,
@@ -116150,18 +116154,18 @@
             "action": "DescribeClusters",
             "condition_keys": [],
             "description": "Grants permission to describe properties of provisioned clusters",
             "orphan": false,
             "resources": []
         },
         "DescribeCustomDomainAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeCustomDomainAssociations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe custom domain names for a cluster",
             "orphan": false,
             "resources": []
         },
         "DescribeDataShares": {
             "access_level": "Read",
             "action": "DescribeDataShares",
             "condition_keys": [],
@@ -116666,20 +116670,22 @@
             "description": "Grants permission to modify a cluster subnet group to include the specified list of VPC subnets",
             "orphan": false,
             "resources": [
                 "subnetgroup"
             ]
         },
         "ModifyCustomDomainAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyCustomDomainAssociation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to modify a custom domain name for a cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "ModifyEndpointAccess": {
             "access_level": "Write",
             "action": "ModifyEndpointAccess",
             "condition_keys": [],
             "description": "Grants permission to modify a redshift-managed vpc endpoint",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230703/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230704/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230704/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/generate/generate.py` & `iam_actions-1.2.20230704/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230704/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230704/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/generate/services.py` & `iam_actions-1.2.20230704/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/policies.json` & `iam_actions-1.2.20230704/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230704/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/iam_actions/services.json` & `iam_actions-1.2.20230704/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230703/pyproject.toml` & `iam_actions-1.2.20230704/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230703"
+version = "1.2.20230704"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230703/setup.py` & `iam_actions-1.2.20230704/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230703',
+    'version': '1.2.20230704',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230703/PKG-INFO` & `iam_actions-1.2.20230704/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230703
+Version: 1.2.20230704
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

