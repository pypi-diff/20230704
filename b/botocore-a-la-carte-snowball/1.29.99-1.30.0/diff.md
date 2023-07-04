# Comparing `tmp/botocore-a-la-carte-snowball-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-snowball-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-snowball-1.29.99.tar", last modified: Sat Mar 25 01:23:05 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-snowball-1.30.0.tar", last modified: Tue Jul  4 01:44:56 2023, max compression
```

## Comparing `botocore-a-la-carte-snowball-1.29.99.tar` & `botocore-a-la-carte-snowball-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:05.216886 botocore-a-la-carte-snowball-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:04.000000 botocore-a-la-carte-snowball-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:23:05.216886 botocore-a-la-carte-snowball-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:05.208886 botocore-a-la-carte-snowball-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:05.208886 botocore-a-la-carte-snowball-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:05.208886 botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:05.208886 botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-03-25 01:22:12.000000 botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18099 2023-03-25 01:22:12.000000 botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-25 01:22:12.000000 botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   104856 2023-03-25 01:22:12.000000 botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:05.216886 botocore-a-la-carte-snowball-1.29.99/botocore_a_la_carte_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:23:05.000000 botocore-a-la-carte-snowball-1.29.99/botocore_a_la_carte_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-25 01:23:05.000000 botocore-a-la-carte-snowball-1.29.99/botocore_a_la_carte_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:05.000000 botocore-a-la-carte-snowball-1.29.99/botocore_a_la_carte_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:05.000000 botocore-a-la-carte-snowball-1.29.99/botocore_a_la_carte_snowball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:05.216886 botocore-a-la-carte-snowball-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-25 01:23:04.000000 botocore-a-la-carte-snowball-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:56.990800 botocore-a-la-carte-snowball-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:56.000000 botocore-a-la-carte-snowball-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:56.990800 botocore-a-la-carte-snowball-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:56.986800 botocore-a-la-carte-snowball-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:56.986800 botocore-a-la-carte-snowball-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:56.986800 botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:56.990800 botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-04 01:44:02.000000 botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18099 2023-07-04 01:44:02.000000 botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-04 01:44:02.000000 botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109375 2023-07-04 01:44:02.000000 botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:56.990800 botocore-a-la-carte-snowball-1.30.0/botocore_a_la_carte_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:56.000000 botocore-a-la-carte-snowball-1.30.0/botocore_a_la_carte_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-04 01:44:56.000000 botocore-a-la-carte-snowball-1.30.0/botocore_a_la_carte_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:56.000000 botocore-a-la-carte-snowball-1.30.0/botocore_a_la_carte_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:56.000000 botocore-a-la-carte-snowball-1.30.0/botocore_a_la_carte_snowball.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:56.990800 botocore-a-la-carte-snowball-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-04 01:44:56.000000 botocore-a-la-carte-snowball-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-snowball-1.29.99/LICENSE.txt` & `botocore-a-la-carte-snowball-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snowball-1.29.99/PKG-INFO` & `botocore-a-la-carte-snowball-1.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-snowball
-Version: 1.29.99
+Version: 1.30.0
 Summary: snowball data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/examples-1.json` & `botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/paginators-1.json` & `botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-snowball-1.29.99/botocore/data/snowball/2016-06-30/service-2.json` & `botocore-a-la-carte-snowball-1.30.0/botocore/data/snowball/2016-06-30/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953909429946901%*

 * *Differences: {"'operations'": "{'CreateJob': {'documentation': '<p>Creates a job to import or export data "*

 * *                 'between Amazon S3 and your on-premises data center. Your Amazon Web Services '*

 * *                 'account must have the right trust policies and permissions in place to create a '*

 * *                 "job for a Snow device. If you\\'re creating a job for a node in a cluster, you "*

 * *                 'only need to provide the <code>clusterId</code> value; the other job attributes '*

 * *                 'are […]*

```diff
@@ -110,15 +110,15 @@
             },
             "name": "CreateCluster",
             "output": {
                 "shape": "CreateClusterResult"
             }
         },
         "CreateJob": {
-            "documentation": "<p>Creates a job to import or export data between Amazon S3 and your on-premises data center. Your Amazon Web Services account must have the right trust policies and permissions in place to create a job for a Snow device. If you're creating a job for a node in a cluster, you only need to provide the <code>clusterId</code> value; the other job attributes are inherited from the cluster. </p> <note> <p>Only the Snowball; Edge device type is supported when ordering clustered jobs.</p> <p>The device capacity is optional.</p> <p>Availability of device types differ by Amazon Web Services Region. For more information about Region availability, see <a href=\"https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services/?p=ngi&amp;loc=4\">Amazon Web Services Regional Services</a>.</p> </note> <p/> <p class=\"title\"> <b>Snow Family devices and their capacities.</b> </p> <ul> <li> <p>Snow Family device type: <b>SNC1_SSD</b> </p> <ul> <li> <p>Capacity: T14</p> </li> <li> <p>Description: Snowcone </p> </li> </ul> <p/> </li> <li> <p>Snow Family device type: <b>SNC1_HDD</b> </p> <ul> <li> <p>Capacity: T8</p> </li> <li> <p>Description: Snowcone </p> </li> </ul> <p/> </li> <li> <p>Device type: <b>EDGE_S</b> </p> <ul> <li> <p>Capacity: T98</p> </li> <li> <p>Description: Snowball Edge Storage Optimized for data transfer only </p> </li> </ul> <p/> </li> <li> <p>Device type: <b>EDGE_CG</b> </p> <ul> <li> <p>Capacity: T42</p> </li> <li> <p>Description: Snowball Edge Compute Optimized with GPU</p> </li> </ul> <p/> </li> <li> <p>Device type: <b>EDGE_C</b> </p> <ul> <li> <p>Capacity: T42</p> </li> <li> <p>Description: Snowball Edge Compute Optimized without GPU</p> </li> </ul> <p/> </li> <li> <p>Device type: <b>EDGE</b> </p> <ul> <li> <p>Capacity: T100</p> </li> <li> <p>Description: Snowball Edge Storage Optimized with EC2 Compute</p> </li> </ul> <p/> </li> <li> <p>Device type: <b>STANDARD</b> </p> <ul> <li> <p>Capacity: T50</p> </li> <li> <p>Description: Original Snowball device</p> <note> <p>This device is only available in the Ningxia, Beijing, and Singapore Amazon Web Services Region </p> </note> </li> </ul> <p/> </li> <li> <p>Device type: <b>STANDARD</b> </p> <ul> <li> <p>Capacity: T80</p> </li> <li> <p>Description: Original Snowball device</p> <note> <p>This device is only available in the Ningxia, Beijing, and Singapore Amazon Web Services Region. </p> </note> </li> </ul> <p/> </li> </ul>",
+            "documentation": "<p>Creates a job to import or export data between Amazon S3 and your on-premises data center. Your Amazon Web Services account must have the right trust policies and permissions in place to create a job for a Snow device. If you're creating a job for a node in a cluster, you only need to provide the <code>clusterId</code> value; the other job attributes are inherited from the cluster. </p> <note> <p>Only the Snowball; Edge device type is supported when ordering clustered jobs.</p> <p>The device capacity is optional.</p> <p>Availability of device types differ by Amazon Web Services Region. For more information about Region availability, see <a href=\"https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services/?p=ngi&amp;loc=4\">Amazon Web Services Regional Services</a>.</p> </note> <p/> <p class=\"title\"> <b>Snow Family devices and their capacities.</b> </p> <ul> <li> <p>Device type: <b>SNC1_SSD</b> </p> <ul> <li> <p>Capacity: T14</p> </li> <li> <p>Description: Snowcone </p> </li> </ul> <p/> </li> <li> <p>Device type: <b>SNC1_HDD</b> </p> <ul> <li> <p>Capacity: T8</p> </li> <li> <p>Description: Snowcone </p> </li> </ul> <p/> </li> <li> <p>Device type: <b>EDGE_S</b> </p> <ul> <li> <p>Capacity: T98</p> </li> <li> <p>Description: Snowball Edge Storage Optimized for data transfer only </p> </li> </ul> <p/> </li> <li> <p>Device type: <b>EDGE_CG</b> </p> <ul> <li> <p>Capacity: T42</p> </li> <li> <p>Description: Snowball Edge Compute Optimized with GPU</p> </li> </ul> <p/> </li> <li> <p>Device type: <b>EDGE_C</b> </p> <ul> <li> <p>Capacity: T42</p> </li> <li> <p>Description: Snowball Edge Compute Optimized without GPU</p> </li> </ul> <p/> </li> <li> <p>Device type: <b>EDGE</b> </p> <ul> <li> <p>Capacity: T100</p> </li> <li> <p>Description: Snowball Edge Storage Optimized with EC2 Compute</p> </li> </ul> <p/> </li> <li> <p>Device type: <b>STANDARD</b> </p> <ul> <li> <p>Capacity: T50</p> </li> <li> <p>Description: Original Snowball device</p> <note> <p>This device is only available in the Ningxia, Beijing, and Singapore Amazon Web Services Region </p> </note> </li> </ul> <p/> </li> <li> <p>Device type: <b>STANDARD</b> </p> <ul> <li> <p>Capacity: T80</p> </li> <li> <p>Description: Original Snowball device</p> <note> <p>This device is only available in the Ningxia, Beijing, and Singapore Amazon Web Services Region. </p> </note> </li> </ul> <p/> </li> <li> <p>Device type: <b>V3_5C</b> </p> <ul> <li> <p>Capacity: T32</p> </li> <li> <p>Description: Snowball Edge Compute Optimized without GPU</p> </li> </ul> <p/> </li> <li> <p>Device type: <b>V3_5S</b> </p> <ul> <li> <p>Capacity: T240</p> </li> <li> <p>Description: Snowball Edge Storage Optimized 210TB</p> </li> </ul> <p/> </li> </ul>",
             "errors": [
                 {
                     "shape": "InvalidResourceException"
                 },
                 {
                     "shape": "KMSRequestFailedException"
                 },
@@ -416,15 +416,15 @@
             },
             "name": "ListClusters",
             "output": {
                 "shape": "ListClustersResult"
             }
         },
         "ListCompatibleImages": {
-            "documentation": "<p>This action returns a list of the different Amazon EC2 Amazon Machine Images (AMIs) that are owned by your Amazon Web Services accountthat would be supported for use on a Snow device. Currently, supported AMIs are based on the CentOS 7 (x86_64) - with Updates HVM, Ubuntu Server 14.04 LTS (HVM), and Ubuntu 16.04 LTS - Xenial (HVM) images, available on the Amazon Web Services Marketplace.</p>",
+            "documentation": "<p>This action returns a list of the different Amazon EC2 Amazon Machine Images (AMIs) that are owned by your Amazon Web Services accountthat would be supported for use on a Snow device. Currently, supported AMIs are based on the Amazon Linux-2, Ubuntu 20.04 LTS - Focal, or Ubuntu 22.04 LTS - Jammy images, available on the Amazon Web Services Marketplace. Ubuntu 16.04 LTS - Xenial (HVM) images are no longer supported in the Market, but still supported for use on devices through Amazon EC2 VM Import/Export and running locally in AMIs.</p>",
             "errors": [
                 {
                     "shape": "InvalidNextTokenException"
                 },
                 {
                     "shape": "Ec2RequestFailedException"
                 }
@@ -908,26 +908,38 @@
                     "documentation": "<p>The ID for the address that you want the cluster shipped to.</p>",
                     "shape": "AddressId"
                 },
                 "Description": {
                     "documentation": "<p>An optional description of this specific cluster, for example <code>Environmental Data Cluster-01</code>.</p>",
                     "shape": "String"
                 },
+                "ForceCreateJobs": {
+                    "documentation": "<p>Force to create cluster when user attempts to overprovision or underprovision a cluster. A cluster is overprovisioned or underprovisioned if the initial size of the cluster is more (overprovisioned) or less (underprovisioned) than what needed to meet capacity requirement specified with <code>OnDeviceServiceConfiguration</code>.</p>",
+                    "shape": "Boolean"
+                },
                 "ForwardingAddressId": {
                     "documentation": "<p>The forwarding address ID for a cluster. This field is not supported in most regions.</p>",
                     "shape": "AddressId"
                 },
+                "InitialClusterSize": {
+                    "documentation": "<p>If provided, each job will be automatically created and associated with the new cluster. If not provided, will be treated as 0.</p>",
+                    "shape": "InitialClusterSize"
+                },
                 "JobType": {
                     "documentation": "<p>The type of job for this cluster. Currently, the only job type supported for clusters is <code>LOCAL_USE</code>.</p> <p>For more information, see \"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>",
                     "shape": "JobType"
                 },
                 "KmsKeyARN": {
                     "documentation": "<p>The <code>KmsKeyARN</code> value that you want to associate with this cluster. <code>KmsKeyARN</code> values are created by using the <a href=\"https://docs.aws.amazon.com/kms/latest/APIReference/API_CreateKey.html\">CreateKey</a> API action in Key Management Service (KMS). </p>",
                     "shape": "KmsKeyARN"
                 },
+                "LongTermPricingIds": {
+                    "documentation": "<p>Lists long-term pricing id that will be used to associate with jobs automatically created for the new cluster.</p>",
+                    "shape": "LongTermPricingIdList"
+                },
                 "Notification": {
                     "documentation": "<p>The Amazon Simple Notification Service (Amazon SNS) notification settings for this cluster.</p>",
                     "shape": "Notification"
                 },
                 "OnDeviceServiceConfiguration": {
                     "documentation": "<p>Specifies the service or services on the Snow Family device that your transferred data will be exported from or imported into. Amazon Web Services Snow Family device clusters support Amazon S3 and NFS (Network File System).</p>",
                     "shape": "OnDeviceServiceConfiguration"
@@ -944,38 +956,44 @@
                     "documentation": "<p>The <code>RoleARN</code> that you want to associate with this cluster. <code>RoleArn</code> values are created by using the <a href=\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateRole.html\">CreateRole</a> API action in Identity and Access Management (IAM).</p>",
                     "shape": "RoleARN"
                 },
                 "ShippingOption": {
                     "documentation": "<p>The shipping speed for each node in this cluster. This speed doesn't dictate how soon you'll get each Snowball Edge device, rather it represents how quickly each device moves to its destination while in transit. Regional shipping speeds are as follows: </p> <ul> <li> <p>In Australia, you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day.</p> </li> <li> <p>In the European Union (EU), you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day. In addition, most countries in the EU have access to standard shipping, which typically takes less than a week, one way.</p> </li> <li> <p>In India, Snow devices are delivered in one to seven days.</p> </li> <li> <p>In the United States of America (US), you have access to one-day shipping and two-day shipping.</p> </li> </ul> <ul> <li> <p>In Australia, you have access to express shipping. Typically, devices shipped express are delivered in about a day.</p> </li> <li> <p>In the European Union (EU), you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day. In addition, most countries in the EU have access to standard shipping, which typically takes less than a week, one way.</p> </li> <li> <p>In India, Snow devices are delivered in one to seven days.</p> </li> <li> <p>In the US, you have access to one-day shipping and two-day shipping.</p> </li> </ul>",
                     "shape": "ShippingOption"
                 },
+                "SnowballCapacityPreference": {
+                    "documentation": "<p>If your job is being created in one of the US regions, you have the option of specifying what size Snow device you'd like for this job. In all other regions, Snowballs come with 80 TB in storage capacity.</p> <p>For more information, see \"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>",
+                    "shape": "SnowballCapacity"
+                },
                 "SnowballType": {
                     "documentation": "<p>The type of Snow Family devices to use for this cluster. </p> <note> <p>For cluster jobs, Amazon Web Services Snow Family currently supports only the <code>EDGE</code> device type.</p> </note> <p>For more information, see \"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>",
                     "shape": "SnowballType"
                 },
                 "TaxDocuments": {
                     "documentation": "<p>The tax documents required in your Amazon Web Services Region.</p>",
                     "shape": "TaxDocuments"
                 }
             },
             "required": [
                 "JobType",
-                "Resources",
                 "AddressId",
-                "RoleARN",
                 "SnowballType",
                 "ShippingOption"
             ],
             "type": "structure"
         },
         "CreateClusterResult": {
             "members": {
                 "ClusterId": {
                     "documentation": "<p>The automatically generated ID for a cluster.</p>",
                     "shape": "ClusterId"
+                },
+                "JobListEntries": {
+                    "documentation": "<p>List of jobs created for this cluster. For syntax, see <a href=\"https://docs.aws.amazon.com/snowball/latest/api-reference/API_ListJobs.html#API_ListJobs_ResponseSyntax\">ListJobsResult$JobListEntries</a> in this guide.</p>",
+                    "shape": "JobListEntryList"
                 }
             },
             "type": "structure"
         },
         "CreateJobRequest": {
             "members": {
                 "AddressId": {
@@ -1327,15 +1345,15 @@
         "Ec2AmiResourceList": {
             "member": {
                 "shape": "Ec2AmiResource"
             },
             "type": "list"
         },
         "Ec2RequestFailedException": {
-            "documentation": "<p>Your IAM user lacks the necessary Amazon EC2 permissions to perform the attempted action.</p>",
+            "documentation": "<p>Your user lacks the necessary Amazon EC2 permissions to perform the attempted action.</p>",
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "String"
                 }
             },
             "type": "structure"
@@ -1448,14 +1466,19 @@
                 "GSTIN": {
                     "documentation": "<p>The Goods and Services Tax (GST) documents required in Amazon Web Services Region in India.</p>",
                     "shape": "GSTIN"
                 }
             },
             "type": "structure"
         },
+        "InitialClusterSize": {
+            "max": 16,
+            "min": 0,
+            "type": "integer"
+        },
         "Integer": {
             "type": "integer"
         },
         "InvalidAddressException": {
             "documentation": "<p>The address provided was invalid. Check the address with your region's carrier, and try again.</p>",
             "exception": true,
             "members": {
@@ -1982,14 +2005,20 @@
         },
         "LongTermPricingId": {
             "max": 41,
             "min": 41,
             "pattern": "LTPID[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}",
             "type": "string"
         },
+        "LongTermPricingIdList": {
+            "member": {
+                "shape": "LongTermPricingId"
+            },
+            "type": "list"
+        },
         "LongTermPricingListEntry": {
             "documentation": "<p>Each <code>LongTermPricingListEntry</code> object contains information about a long-term pricing type.</p>",
             "members": {
                 "CurrentActiveJob": {
                     "documentation": "<p>The current active jobs on the device the long-term pricing type.</p>",
                     "shape": "JobId"
                 },
@@ -2031,15 +2060,16 @@
                 }
             },
             "type": "structure"
         },
         "LongTermPricingType": {
             "enum": [
                 "OneYear",
-                "ThreeYear"
+                "ThreeYear",
+                "OneMonth"
             ],
             "type": "string"
         },
         "NFSOnDeviceServiceConfiguration": {
             "documentation": "<p>An object that represents the metadata and configuration settings for the NFS (Network File System) service on an Amazon Web Services Snow Family device.</p>",
             "members": {
                 "StorageLimit": {
@@ -2049,14 +2079,19 @@
                 "StorageUnit": {
                     "documentation": "<p>The scale unit of the NFS storage on the device.</p> <p>Valid values: TB.</p>",
                     "shape": "StorageUnit"
                 }
             },
             "type": "structure"
         },
+        "NodeFaultTolerance": {
+            "max": 4,
+            "min": 1,
+            "type": "integer"
+        },
         "Notification": {
             "documentation": "<p>The Amazon Simple Notification Service (Amazon SNS) notification settings associated with a specific job. The <code>Notification</code> object is returned as a part of the response syntax of the <code>DescribeJob</code> action in the <code>JobMetadata</code> data type.</p> <p>When the notification settings are defined during job creation, you can choose to notify based on a specific set of job states using the <code>JobStatesToNotify</code> array of strings, or you can specify that you want to have Amazon SNS notifications sent out for all job states with <code>NotifyAll</code> set to true.</p>",
             "members": {
                 "JobStatesToNotify": {
                     "documentation": "<p>The list of job states that will trigger a notification for this job.</p>",
                     "shape": "JobStateList"
                 },
@@ -2078,14 +2113,18 @@
                     "documentation": "<p>The configuration of EKS Anywhere on the Snow Family device.</p>",
                     "shape": "EKSOnDeviceServiceConfiguration"
                 },
                 "NFSOnDeviceService": {
                     "documentation": "<p>Represents the NFS (Network File System) service on a Snow Family device.</p>",
                     "shape": "NFSOnDeviceServiceConfiguration"
                 },
+                "S3OnDeviceService": {
+                    "documentation": "<p>Configuration for Amazon S3 compatible storage on Snow family devices.</p>",
+                    "shape": "S3OnDeviceServiceConfiguration"
+                },
                 "TGWOnDeviceService": {
                     "documentation": "<p>Represents the Storage Gateway service Tape Gateway type on a Snow Family device.</p>",
                     "shape": "TGWOnDeviceServiceConfiguration"
                 }
             },
             "type": "structure"
         },
@@ -2112,14 +2151,36 @@
             "type": "structure"
         },
         "RoleARN": {
             "max": 255,
             "pattern": "arn:aws.*:iam::[0-9]{12}:role/.*",
             "type": "string"
         },
+        "S3OnDeviceServiceConfiguration": {
+            "documentation": "<p>Amazon S3 compatible storage on Snow family devices configuration items.</p>",
+            "members": {
+                "FaultTolerance": {
+                    "documentation": "<p>&gt;Fault tolerance level of the cluster. This indicates the number of nodes that can go down without degrading the performance of the cluster. This additional input helps when the specified <code>StorageLimit</code> matches more than one Amazon S3 compatible storage on Snow family devices service configuration.</p>",
+                    "shape": "NodeFaultTolerance"
+                },
+                "ServiceSize": {
+                    "documentation": "<p>Applicable when creating a cluster. Specifies how many nodes are needed for Amazon S3 compatible storage on Snow family devices. If specified, the other input can be omitted.</p>",
+                    "shape": "ServiceSize"
+                },
+                "StorageLimit": {
+                    "documentation": "<p>If the specified storage limit value matches storage limit of one of the defined configurations, that configuration will be used. If the specified storage limit value does not match any defined configuration, the request will fail. If more than one configuration has the same storage limit as specified, the other input need to be provided.</p>",
+                    "shape": "S3StorageLimit"
+                },
+                "StorageUnit": {
+                    "documentation": "<p>Storage unit. Currently the only supported unit is TB.</p>",
+                    "shape": "StorageUnit"
+                }
+            },
+            "type": "structure"
+        },
         "S3Resource": {
             "documentation": "<p>Each <code>S3Resource</code> object represents an Amazon S3 bucket that your transferred data will be exported from or imported into. For export jobs, this object can have an optional <code>KeyRange</code> value. The length of the range is defined at job creation, and has either an inclusive <code>BeginMarker</code>, an inclusive <code>EndMarker</code>, or both. Ranges are UTF-8 binary sorted.</p>",
             "members": {
                 "BucketArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an Amazon S3 bucket.</p>",
                     "shape": "ResourceARN"
                 },
@@ -2136,21 +2197,30 @@
         },
         "S3ResourceList": {
             "member": {
                 "shape": "S3Resource"
             },
             "type": "list"
         },
+        "S3StorageLimit": {
+            "min": 0.0,
+            "type": "double"
+        },
         "ServiceName": {
             "enum": [
                 "KUBERNETES",
                 "EKS_ANYWHERE"
             ],
             "type": "string"
         },
+        "ServiceSize": {
+            "max": 16,
+            "min": 3,
+            "type": "integer"
+        },
         "ServiceVersion": {
             "documentation": "<p>The version of the requested service.</p>",
             "members": {
                 "Version": {
                     "documentation": "<p>The version number of the requested service.</p>",
                     "shape": "String"
                 }
@@ -2226,28 +2296,30 @@
                 "T80",
                 "T100",
                 "T42",
                 "T98",
                 "T8",
                 "T14",
                 "T32",
-                "NoPreference"
+                "NoPreference",
+                "T240"
             ],
             "type": "string"
         },
         "SnowballType": {
             "enum": [
                 "STANDARD",
                 "EDGE",
                 "EDGE_C",
                 "EDGE_CG",
                 "EDGE_S",
                 "SNC1_HDD",
                 "SNC1_SSD",
-                "V3_5C"
+                "V3_5C",
+                "V3_5S"
             ],
             "type": "string"
         },
         "SnowconeDeviceConfiguration": {
             "documentation": "<p>Specifies the device configuration for an Snowcone job.</p>",
             "members": {
                 "WirelessConnection": {
```

### Comparing `botocore-a-la-carte-snowball-1.29.99/botocore_a_la_carte_snowball.egg-info/PKG-INFO` & `botocore-a-la-carte-snowball-1.30.0/botocore_a_la_carte_snowball.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-snowball
-Version: 1.29.99
+Version: 1.30.0
 Summary: snowball data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-snowball-1.29.99/setup.py` & `botocore-a-la-carte-snowball-1.30.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-snowball',
-    version="1.29.99",
+    version="1.30.0",
     description='snowball data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/snowball/*/*.json'],
```

