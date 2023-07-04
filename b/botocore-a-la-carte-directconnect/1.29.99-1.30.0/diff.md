# Comparing `tmp/botocore-a-la-carte-directconnect-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-directconnect-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-directconnect-1.29.99.tar", last modified: Sat Mar 25 01:22:33 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-directconnect-1.30.0.tar", last modified: Tue Jul  4 01:44:24 2023, max compression
```

## Comparing `botocore-a-la-carte-directconnect-1.29.99.tar` & `botocore-a-la-carte-directconnect-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:33.746976 botocore-a-la-carte-directconnect-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:33.000000 botocore-a-la-carte-directconnect-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-25 01:22:33.746976 botocore-a-la-carte-directconnect-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:33.746976 botocore-a-la-carte-directconnect-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:33.746976 botocore-a-la-carte-directconnect-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:33.746976 botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:33.746976 botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/2012-10-25/
--rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-03-25 01:22:12.000000 botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/2012-10-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/2012-10-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-25 01:22:12.000000 botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/2012-10-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   178693 2023-03-25 01:22:12.000000 botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/2012-10-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:33.746976 botocore-a-la-carte-directconnect-1.29.99/botocore_a_la_carte_directconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-25 01:22:33.000000 botocore-a-la-carte-directconnect-1.29.99/botocore_a_la_carte_directconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-25 01:22:33.000000 botocore-a-la-carte-directconnect-1.29.99/botocore_a_la_carte_directconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:33.000000 botocore-a-la-carte-directconnect-1.29.99/botocore_a_la_carte_directconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:33.000000 botocore-a-la-carte-directconnect-1.29.99/botocore_a_la_carte_directconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:33.746976 botocore-a-la-carte-directconnect-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-25 01:22:33.000000 botocore-a-la-carte-directconnect-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:24.454482 botocore-a-la-carte-directconnect-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:24.000000 botocore-a-la-carte-directconnect-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 01:44:24.454482 botocore-a-la-carte-directconnect-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:24.450482 botocore-a-la-carte-directconnect-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:24.450482 botocore-a-la-carte-directconnect-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:24.450482 botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:24.450482 botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/2012-10-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-04 01:44:02.000000 botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/2012-10-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/2012-10-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-04 01:44:02.000000 botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/2012-10-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   178759 2023-07-04 01:44:02.000000 botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/2012-10-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:24.454482 botocore-a-la-carte-directconnect-1.30.0/botocore_a_la_carte_directconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 01:44:24.000000 botocore-a-la-carte-directconnect-1.30.0/botocore_a_la_carte_directconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-04 01:44:24.000000 botocore-a-la-carte-directconnect-1.30.0/botocore_a_la_carte_directconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:24.000000 botocore-a-la-carte-directconnect-1.30.0/botocore_a_la_carte_directconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:24.000000 botocore-a-la-carte-directconnect-1.30.0/botocore_a_la_carte_directconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:24.454482 botocore-a-la-carte-directconnect-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-04 01:44:24.000000 botocore-a-la-carte-directconnect-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-directconnect-1.29.99/LICENSE.txt` & `botocore-a-la-carte-directconnect-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-directconnect-1.29.99/PKG-INFO` & `botocore-a-la-carte-directconnect-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-directconnect
-Version: 1.29.99
+Version: 1.30.0
 Summary: directconnect data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/2012-10-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/2012-10-25/endpoint-rule-set-1.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999946416323731%*

 * *Differences: {"'rules'": "{1: {'rules': {0: {'rules': {0: {'rules': {3: {'rules': {delete: [1, 0]}}}}}}}}}"}*

```diff
@@ -316,52 +316,14 @@
                                     ],
                                     "type": "tree"
                                 },
                                 {
                                     "conditions": [],
                                     "rules": [
                                         {
-                                            "conditions": [
-                                                {
-                                                    "argv": [
-                                                        {
-                                                            "ref": "Region"
-                                                        },
-                                                        "us-gov-east-1"
-                                                    ],
-                                                    "fn": "stringEquals"
-                                                }
-                                            ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://directconnect.us-gov-east-1.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
-                                            "conditions": [
-                                                {
-                                                    "argv": [
-                                                        {
-                                                            "ref": "Region"
-                                                        },
-                                                        "us-gov-west-1"
-                                                    ],
-                                                    "fn": "stringEquals"
-                                                }
-                                            ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://directconnect.us-gov-west-1.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
                                             "conditions": [],
                                             "endpoint": {
                                                 "headers": {},
                                                 "properties": {},
                                                 "url": "https://directconnect.{Region}.{PartitionResult#dnsSuffix}"
                                             },
                                             "type": "endpoint"
```

### Comparing `botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/2012-10-25/paginators-1.json` & `botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/2012-10-25/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-directconnect-1.29.99/botocore/data/directconnect/2012-10-25/service-2.json` & `botocore-a-la-carte-directconnect-1.30.0/botocore/data/directconnect/2012-10-25/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999315624227773%*

 * *Differences: {"'operations'": '{\'UpdateVirtualInterfaceAttributes\': {\'documentation\': "<p>Updates the '*

 * *                 'specified attributes of the specified virtual private interface.</p> <p>Setting '*

 * *                 'the MTU of a virtual interface to 9001 (jumbo frames) can cause an update to the '*

 * *                 "underlying physical connection if it wasn't updated to support jumbo frames. "*

 * *                 'Updating the connection disrupts network connectivity for all virtual interfaces '*

 * *                 ' […]*

```diff
@@ -1434,15 +1434,15 @@
             },
             "name": "UpdateLag",
             "output": {
                 "shape": "Lag"
             }
         },
         "UpdateVirtualInterfaceAttributes": {
-            "documentation": "<p>Updates the specified attributes of the specified virtual private interface.</p> <p>Setting the MTU of a virtual interface to 9001 (jumbo frames) can cause an update to the underlying physical connection if it wasn't updated to support jumbo frames. Updating the connection disrupts network connectivity for all virtual interfaces associated with the connection for up to 30 seconds. To check whether your connection supports jumbo frames, call <a>DescribeConnections</a>. To check whether your virtual q interface supports jumbo frames, call <a>DescribeVirtualInterfaces</a>.</p>",
+            "documentation": "<p>Updates the specified attributes of the specified virtual private interface.</p> <p>Setting the MTU of a virtual interface to 9001 (jumbo frames) can cause an update to the underlying physical connection if it wasn't updated to support jumbo frames. Updating the connection disrupts network connectivity for all virtual interfaces associated with the connection for up to 30 seconds. To check whether your connection supports jumbo frames, call <a>DescribeConnections</a>. To check whether your virtual interface supports jumbo frames, call <a>DescribeVirtualInterfaces</a>.</p>",
             "errors": [
                 {
                     "shape": "DirectConnectServerException"
                 },
                 {
                     "shape": "DirectConnectClientException"
                 }
@@ -2043,15 +2043,15 @@
                     "shape": "EncryptionMode"
                 },
                 "hasLogicalRedundancy": {
                     "documentation": "<p>Indicates whether the connection supports a secondary BGP peer in the same address family (IPv4/IPv6).</p>",
                     "shape": "HasLogicalRedundancy"
                 },
                 "jumboFrameCapable": {
-                    "documentation": "<p>Indicates whether jumbo frames (9001 MTU) are supported.</p>",
+                    "documentation": "<p>Indicates whether jumbo frames are supported.</p>",
                     "shape": "JumboFrameCapable"
                 },
                 "lagId": {
                     "documentation": "<p>The ID of the LAG.</p>",
                     "shape": "LagId"
                 },
                 "loaIssueTime": {
@@ -2349,15 +2349,15 @@
                     "shape": "LagName"
                 },
                 "location": {
                     "documentation": "<p>The location for the LAG.</p>",
                     "shape": "LocationCode"
                 },
                 "numberOfConnections": {
-                    "documentation": "<p>The number of physical dedicated connections initially provisioned and bundled by the LAG.</p>",
+                    "documentation": "<p>The number of physical dedicated connections initially provisioned and bundled by the LAG. You can have a maximum of four connections when the port speed is 1G or 10G, or two when the port speed is 100G. </p>",
                     "shape": "Count"
                 },
                 "providerName": {
                     "documentation": "<p>The name of the service provider associated with the LAG.</p>",
                     "shape": "ProviderName"
                 },
                 "requestMACSec": {
@@ -3339,15 +3339,15 @@
                     "shape": "InterconnectName"
                 },
                 "interconnectState": {
                     "documentation": "<p>The state of the interconnect. The following are the possible values:</p> <ul> <li> <p> <code>requested</code>: The initial state of an interconnect. The interconnect stays in the requested state until the Letter of Authorization (LOA) is sent to the customer.</p> </li> <li> <p> <code>pending</code>: The interconnect is approved, and is being initialized.</p> </li> <li> <p> <code>available</code>: The network link is up, and the interconnect is ready for use.</p> </li> <li> <p> <code>down</code>: The network link is down.</p> </li> <li> <p> <code>deleting</code>: The interconnect is being deleted.</p> </li> <li> <p> <code>deleted</code>: The interconnect is deleted.</p> </li> <li> <p> <code>unknown</code>: The state of the interconnect is not available.</p> </li> </ul>",
                     "shape": "InterconnectState"
                 },
                 "jumboFrameCapable": {
-                    "documentation": "<p>Indicates whether jumbo frames (9001 MTU) are supported.</p>",
+                    "documentation": "<p>Indicates whether jumbo frames are supported.</p>",
                     "shape": "JumboFrameCapable"
                 },
                 "lagId": {
                     "documentation": "<p>The ID of the LAG.</p>",
                     "shape": "LagId"
                 },
                 "loaIssueTime": {
@@ -3441,15 +3441,15 @@
                     "shape": "EncryptionMode"
                 },
                 "hasLogicalRedundancy": {
                     "documentation": "<p>Indicates whether the LAG supports a secondary BGP peer in the same address family (IPv4/IPv6).</p>",
                     "shape": "HasLogicalRedundancy"
                 },
                 "jumboFrameCapable": {
-                    "documentation": "<p>Indicates whether jumbo frames (9001 MTU) are supported.</p>",
+                    "documentation": "<p>Indicates whether jumbo frames are supported.</p>",
                     "shape": "JumboFrameCapable"
                 },
                 "lagId": {
                     "documentation": "<p>The ID of the LAG.</p>",
                     "shape": "LagId"
                 },
                 "lagName": {
@@ -3946,15 +3946,15 @@
                     "shape": "DirectConnectGatewayId"
                 },
                 "enableSiteLink": {
                     "documentation": "<p>Indicates whether to enable or disable SiteLink.</p>",
                     "shape": "EnableSiteLink"
                 },
                 "mtu": {
-                    "documentation": "<p>The maximum transmission unit (MTU), in bytes. The supported values are 1500 and 9001. The default value is 1500.</p>",
+                    "documentation": "<p>The maximum transmission unit (MTU), in bytes. The supported values are 1500 and 8500. The default value is 1500.</p>",
                     "shape": "MTU"
                 },
                 "tags": {
                     "documentation": "<p>The tags associated with the transitive virtual interface.</p>",
                     "shape": "TagList"
                 },
                 "virtualInterfaceName": {
@@ -3988,15 +3988,15 @@
                     "shape": "BGPAuthKey"
                 },
                 "customerAddress": {
                     "documentation": "<p>The IP address assigned to the customer interface.</p>",
                     "shape": "CustomerAddress"
                 },
                 "mtu": {
-                    "documentation": "<p>The maximum transmission unit (MTU), in bytes. The supported values are 1500 and 9001. The default value is 1500. </p>",
+                    "documentation": "<p>The maximum transmission unit (MTU), in bytes. The supported values are 1500 and 8500. The default value is 1500 </p>",
                     "shape": "MTU"
                 },
                 "tags": {
                     "documentation": "<p>The tags associated with the transitive virtual interface.</p>",
                     "shape": "TagList"
                 },
                 "virtualInterfaceName": {
@@ -4515,23 +4515,23 @@
                     "shape": "RouterConfig"
                 },
                 "directConnectGatewayId": {
                     "documentation": "<p>The ID of the Direct Connect gateway.</p>",
                     "shape": "DirectConnectGatewayId"
                 },
                 "jumboFrameCapable": {
-                    "documentation": "<p>Indicates whether jumbo frames (9001 MTU) are supported.</p>",
+                    "documentation": "<p>Indicates whether jumbo frames are supported.</p>",
                     "shape": "JumboFrameCapable"
                 },
                 "location": {
                     "documentation": "<p>The location of the connection.</p>",
                     "shape": "LocationCode"
                 },
                 "mtu": {
-                    "documentation": "<p>The maximum transmission unit (MTU), in bytes. The supported values are 1500 and 9001. The default value is 1500.</p>",
+                    "documentation": "<p>The maximum transmission unit (MTU), in bytes. The supported values are 1500 and 8500. The default value is 1500</p>",
                     "shape": "MTU"
                 },
                 "ownerAccount": {
                     "documentation": "<p>The ID of the Amazon Web Services account that owns the virtual interface.</p>",
                     "shape": "OwnerAccount"
                 },
                 "region": {
```

### Comparing `botocore-a-la-carte-directconnect-1.29.99/botocore_a_la_carte_directconnect.egg-info/PKG-INFO` & `botocore-a-la-carte-directconnect-1.30.0/botocore_a_la_carte_directconnect.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-directconnect
-Version: 1.29.99
+Version: 1.30.0
 Summary: directconnect data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-directconnect-1.29.99/setup.py` & `botocore-a-la-carte-directconnect-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-directconnect',
-    version="1.29.99",
+    version="1.30.0",
     description='directconnect data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/directconnect/*/*.json'],
```

