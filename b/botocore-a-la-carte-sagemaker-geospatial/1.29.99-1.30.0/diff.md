# Comparing `tmp/botocore-a-la-carte-sagemaker-geospatial-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-sagemaker-geospatial-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-sagemaker-geospatial-1.29.99.tar", last modified: Sat Mar 25 01:23:11 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-sagemaker-geospatial-1.30.0.tar", last modified: Tue Jul  4 01:45:04 2023, max compression
```

## Comparing `botocore-a-la-carte-sagemaker-geospatial-1.29.99.tar` & `botocore-a-la-carte-sagemaker-geospatial-1.30.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:11.989232 botocore-a-la-carte-sagemaker-geospatial-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:11.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-25 01:23:11.989232 botocore-a-la-carte-sagemaker-geospatial-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:11.989232 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:11.989232 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:11.989232 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/data/sagemaker-geospatial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:11.989232 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/data/sagemaker-geospatial/2020-05-27/
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-03-25 01:22:12.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/data/sagemaker-geospatial/2020-05-27/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-25 01:22:12.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/data/sagemaker-geospatial/2020-05-27/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    85100 2023-03-25 01:22:12.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/data/sagemaker-geospatial/2020-05-27/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:11.989232 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore_a_la_carte_sagemaker_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-25 01:23:11.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore_a_la_carte_sagemaker_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-25 01:23:11.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore_a_la_carte_sagemaker_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:11.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore_a_la_carte_sagemaker_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:11.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore_a_la_carte_sagemaker_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:11.989232 botocore-a-la-carte-sagemaker-geospatial-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-25 01:23:11.000000 botocore-a-la-carte-sagemaker-geospatial-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.358867 botocore-a-la-carte-sagemaker-geospatial-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-04 01:45:04.358867 botocore-a-la-carte-sagemaker-geospatial-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.354867 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.354867 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.354867 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/data/sagemaker-geospatial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.358867 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/data/sagemaker-geospatial/2020-05-27/
+-rw-r--r--   0 runner    (1001) docker     (123)    17680 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/data/sagemaker-geospatial/2020-05-27/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/data/sagemaker-geospatial/2020-05-27/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    99551 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/data/sagemaker-geospatial/2020-05-27/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.358867 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore_a_la_carte_sagemaker_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore_a_la_carte_sagemaker_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore_a_la_carte_sagemaker_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore_a_la_carte_sagemaker_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore_a_la_carte_sagemaker_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:04.358867 botocore-a-la-carte-sagemaker-geospatial-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-geospatial-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-sagemaker-geospatial-1.29.99/LICENSE.txt` & `botocore-a-la-carte-sagemaker-geospatial-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-geospatial-1.29.99/PKG-INFO` & `botocore-a-la-carte-sagemaker-geospatial-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker-geospatial
-Version: 1.29.99
+Version: 1.30.0
 Summary: sagemaker-geospatial data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/data/sagemaker-geospatial/2020-05-27/paginators-1.json` & `botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/data/sagemaker-geospatial/2020-05-27/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore/data/sagemaker-geospatial/2020-05-27/service-2.json` & `botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore/data/sagemaker-geospatial/2020-05-27/service-2.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896168261153798%*

 * *Differences: {"'operations'": "{'ExportEarthObservationJob': {'documentation': '<p>Use this operation to export "*

 * *                 'results of an Earth Observation job and optionally source images used as input '*

 * *                 "to the EOJ to an Amazon S3 location.</p>'}, 'ExportVectorEnrichmentJob': "*

 * *                 "{'documentation': '<p>Use this operation to copy results of a Vector Enrichment "*

 * *                 "job to an Amazon S3 location.</p>'}}",*

 * * "'shapes'": "{'AreaOfInterest': {'members': {'AreaOfInterestG […]*

```diff
@@ -81,15 +81,15 @@
             },
             "name": "DeleteVectorEnrichmentJob",
             "output": {
                 "shape": "DeleteVectorEnrichmentJobOutput"
             }
         },
         "ExportEarthObservationJob": {
-            "documentation": "<p>Use this operation to export results of an Earth Observation job and optionally source images used as input to the EOJ to an S3 location.</p>",
+            "documentation": "<p>Use this operation to export results of an Earth Observation job and optionally source images used as input to the EOJ to an Amazon S3 location.</p>",
             "errors": [
                 {
                     "shape": "ServiceQuotaExceededException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -119,15 +119,15 @@
             },
             "name": "ExportEarthObservationJob",
             "output": {
                 "shape": "ExportEarthObservationJobOutput"
             }
         },
         "ExportVectorEnrichmentJob": {
-            "documentation": "<p>Use this operation to copy results of a Vector Enrichment job to an S3 location.</p>",
+            "documentation": "<p>Use this operation to copy results of a Vector Enrichment job to an Amazon S3 location.</p>",
             "errors": [
                 {
                     "shape": "ServiceQuotaExceededException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -722,49 +722,49 @@
                 "Q1",
                 "Q3",
                 "SUM"
             ],
             "type": "string"
         },
         "AreaOfInterest": {
-            "documentation": "<p/>",
+            "documentation": "<p>The geographic extent of the Earth Observation job.</p>",
             "members": {
                 "AreaOfInterestGeometry": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>A GeoJSON object representing the geographic extent in the coordinate space.</p>",
                     "shape": "AreaOfInterestGeometry"
                 }
             },
             "type": "structure",
             "union": true
         },
         "AreaOfInterestGeometry": {
-            "documentation": "<p/>",
+            "documentation": "<p>A GeoJSON object representing the geographic extent in the coordinate space.</p>",
             "members": {
                 "MultiPolygonGeometry": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing the MultiPolygon Geometry.</p>",
                     "shape": "MultiPolygonGeometryInput"
                 },
                 "PolygonGeometry": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing Polygon Geometry.</p>",
                     "shape": "PolygonGeometryInput"
                 }
             },
             "type": "structure",
             "union": true
         },
         "Arn": {
             "max": 2048,
             "min": 1,
             "type": "string"
         },
         "AssetValue": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure containing the asset properties.</p>",
             "members": {
                 "Href": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Link to the asset object.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "AssetsMap": {
             "key": {
@@ -772,93 +772,92 @@
             },
             "type": "map",
             "value": {
                 "shape": "AssetValue"
             }
         },
         "BandMathConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>Input structure for the BandMath operation type. Defines Predefined and CustomIndices to be computed using BandMath.</p>",
             "members": {
                 "CustomIndices": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>CustomIndices that are computed.</p>",
                     "shape": "CustomIndicesInput"
                 },
                 "PredefinedIndices": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>One or many of the supported predefined indices to compute. Allowed values: <code>NDVI</code>, <code>EVI2</code>, <code>MSAVI</code>, <code>NDWI</code>, <code>NDMI</code>, <code>NDSI</code>, and <code>WDRVI</code>.</p>",
                     "shape": "StringListInput"
                 }
             },
             "type": "structure"
         },
         "BinaryFile": {
             "streaming": true,
             "type": "blob"
         },
         "Boolean": {
             "box": true,
             "type": "boolean"
         },
         "CloudMaskingConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>Input structure for CloudMasking operation type.</p>",
             "members": {},
             "type": "structure"
         },
         "CloudRemovalConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>Input structure for Cloud Removal Operation type</p>",
             "members": {
                 "AlgorithmName": {
                     "documentation": "<p>The name of the algorithm used for cloud removal.</p>",
                     "shape": "AlgorithmNameCloudRemoval"
                 },
                 "InterpolationValue": {
                     "documentation": "<p>The interpolation value you provide for cloud removal.</p>",
                     "shape": "String"
                 },
                 "TargetBands": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>TargetBands to be returned in the output of CloudRemoval operation.</p>",
                     "shape": "StringListInput"
                 }
             },
             "type": "structure"
         },
         "ComparisonOperator": {
             "enum": [
                 "EQUALS",
                 "NOT_EQUALS",
                 "STARTS_WITH"
             ],
             "type": "string"
         },
         "ConflictException": {
-            "documentation": "<p/>",
+            "documentation": "<p>Updating or deleting a resource can cause an inconsistent state.</p>",
             "error": {
                 "httpStatusCode": 409,
                 "senderFault": true
             },
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "String"
                 },
                 "ResourceId": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Identifier of the resource affected.</p>",
                     "shape": "String"
                 }
             },
             "required": [
-                "Message",
-                "ResourceId"
+                "Message"
             ],
             "type": "structure"
         },
         "CustomIndicesInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>Input object defining the custom BandMath indices to compute.</p>",
             "members": {
                 "Operations": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>A list of BandMath indices to compute.</p>",
                     "shape": "OperationsListInput"
                 }
             },
             "type": "structure"
         },
         "DataCollectionArn": {
             "pattern": "^arn:aws[a-z-]{0,12}:sagemaker-geospatial:[a-z0-9-]{1,25}:[0-9]{12}:raster-data-collection/(public|premium|user)/[a-z0-9]{12,}$",
@@ -922,19 +921,19 @@
             "pattern": "^arn:aws[a-z-]{0,12}:sagemaker-geospatial:[a-z0-9-]{1,25}:[0-9]{12}:earth-observation-job/[a-z0-9]{12,}$",
             "type": "string"
         },
         "EarthObservationJobErrorDetails": {
             "documentation": "<p>The structure representing the errors in an EarthObservationJob.</p>",
             "members": {
                 "Message": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>A detailed message describing the error in an Earth Observation job.</p>",
                     "shape": "String"
                 },
                 "Type": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The type of error in an Earth Observation job.</p>",
                     "shape": "EarthObservationJobErrorType"
                 }
             },
             "type": "structure"
         },
         "EarthObservationJobErrorType": {
             "enum": [
@@ -973,51 +972,51 @@
                 "FAILED",
                 "DELETING",
                 "DELETED"
             ],
             "type": "string"
         },
         "EoCloudCoverInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing the EoCloudCover filter.</p>",
             "members": {
                 "LowerBound": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Lower bound for EoCloudCover.</p>",
                     "shape": "Float"
                 },
                 "UpperBound": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Upper bound for EoCloudCover.</p>",
                     "shape": "Float"
                 }
             },
             "required": [
                 "LowerBound",
                 "UpperBound"
             ],
             "type": "structure"
         },
-        "EojDataSourceConfigInput": {
-            "documentation": "<p/>",
-            "members": {
-                "S3Data": {
-                    "documentation": "<p/>",
-                    "shape": "S3DataInput"
-                }
-            },
-            "type": "structure",
-            "union": true
+        "ExecutionRoleArn": {
+            "max": 2048,
+            "min": 20,
+            "pattern": "^arn:(aws[a-z-]*):iam::([0-9]{12}):role/[a-zA-Z0-9+=,.@_/-]+$",
+            "type": "string"
         },
         "ExportEarthObservationJobInput": {
             "members": {
                 "Arn": {
                     "documentation": "<p>The input Amazon Resource Name (ARN) of the Earth Observation job being exported.</p>",
                     "shape": "EarthObservationJobArn"
                 },
+                "ClientToken": {
+                    "documentation": "<p>A unique token that guarantees that the call to this API is idempotent.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ExportEarthObservationJobInputClientTokenString"
+                },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the job.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "ExportSourceImages": {
                     "documentation": "<p>The source images provided to the Earth Observation job being exported.</p>",
                     "shape": "Boolean"
                 },
                 "OutputConfig": {
                     "documentation": "<p>An object containing information about the output file.</p>",
@@ -1027,27 +1026,32 @@
             "required": [
                 "Arn",
                 "ExecutionRoleArn",
                 "OutputConfig"
             ],
             "type": "structure"
         },
+        "ExportEarthObservationJobInputClientTokenString": {
+            "max": 64,
+            "min": 36,
+            "type": "string"
+        },
         "ExportEarthObservationJobOutput": {
             "members": {
                 "Arn": {
                     "documentation": "<p>The output Amazon Resource Name (ARN) of the Earth Observation job being exported.</p>",
                     "shape": "EarthObservationJobArn"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time.</p>",
-                    "shape": "Timestamp"
+                    "shape": "SyntheticTimestamp_date_time"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the job.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "ExportSourceImages": {
                     "documentation": "<p>The source images provided to the Earth Observation job being exported.</p>",
                     "shape": "Boolean"
                 },
                 "ExportStatus": {
                     "documentation": "<p>The status of the results of the Earth Observation job being exported.</p>",
@@ -1067,97 +1071,107 @@
             ],
             "type": "structure"
         },
         "ExportErrorDetails": {
             "documentation": "<p>The structure for returning the export error details in a GetEarthObservationJob.</p>",
             "members": {
                 "ExportResults": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure for returning the export error details while exporting results of an Earth Observation job.</p>",
                     "shape": "ExportErrorDetailsOutput"
                 },
                 "ExportSourceImages": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure for returning the export error details while exporting the source images of an Earth Observation job.</p>",
                     "shape": "ExportErrorDetailsOutput"
                 }
             },
             "type": "structure"
         },
         "ExportErrorDetailsOutput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing the errors in an export EarthObservationJob operation.</p>",
             "members": {
                 "Message": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>A detailed message describing the error in an export EarthObservationJob operation.</p>",
                     "shape": "String"
                 },
                 "Type": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The type of error in an export EarthObservationJob operation.</p>",
                     "shape": "ExportErrorType"
                 }
             },
             "type": "structure"
         },
         "ExportErrorType": {
             "enum": [
                 "CLIENT_ERROR",
                 "SERVER_ERROR"
             ],
             "type": "string"
         },
         "ExportS3DataInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure containing the Amazon S3 path to export the Earth Observation job output.</p>",
             "members": {
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
+                    "documentation": "<p>The Key Management Service key ID for server-side encryption.</p>",
+                    "shape": "KmsKey"
                 },
                 "S3Uri": {
                     "documentation": "<p>The URL to the Amazon S3 data input.</p>",
-                    "shape": "String"
+                    "shape": "S3Uri"
                 }
             },
             "required": [
                 "S3Uri"
             ],
             "type": "structure"
         },
         "ExportVectorEnrichmentJobInput": {
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Vector Enrichment job.</p>",
                     "shape": "VectorEnrichmentJobArn"
                 },
+                "ClientToken": {
+                    "documentation": "<p>A unique token that guarantees that the call to this API is idempotent.</p>",
+                    "idempotencyToken": true,
+                    "shape": "ExportVectorEnrichmentJobInputClientTokenString"
+                },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM rolewith permission to upload to the location in OutputConfig.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "OutputConfig": {
                     "documentation": "<p>Output location information for exporting Vector Enrichment Job results. </p>",
                     "shape": "ExportVectorEnrichmentJobOutputConfig"
                 }
             },
             "required": [
                 "Arn",
                 "ExecutionRoleArn",
                 "OutputConfig"
             ],
             "type": "structure"
         },
+        "ExportVectorEnrichmentJobInputClientTokenString": {
+            "max": 64,
+            "min": 36,
+            "type": "string"
+        },
         "ExportVectorEnrichmentJobOutput": {
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Vector Enrichment job being exported.</p>",
                     "shape": "VectorEnrichmentJobArn"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time.</p>",
-                    "shape": "Timestamp"
+                    "shape": "SyntheticTimestamp_date_time"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role with permission to upload to the location in OutputConfig.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "ExportStatus": {
                     "documentation": "<p>The status of the results the Vector Enrichment job being exported.</p>",
                     "shape": "VectorEnrichmentJobExportStatus"
                 },
                 "OutputConfig": {
                     "documentation": "<p>Output location information for exporting Vector Enrichment Job results. </p>",
@@ -1173,15 +1187,15 @@
             ],
             "type": "structure"
         },
         "ExportVectorEnrichmentJobOutputConfig": {
             "documentation": "<p>An object containing information about the output file.</p>",
             "members": {
                 "S3Data": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The input structure for Amazon S3 data; representing the Amazon S3 location of the input data objects.</p>",
                     "shape": "VectorEnrichmentJobS3Data"
                 }
             },
             "required": [
                 "S3Data"
             ],
             "type": "structure"
@@ -1233,22 +1247,22 @@
                     "documentation": "<p>The target bands for geomosaic.</p>",
                     "shape": "StringListInput"
                 }
             },
             "type": "structure"
         },
         "Geometry": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing a Geometry in terms of Type and Coordinates as per GeoJson spec.</p>",
             "members": {
                 "Coordinates": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The coordinates of the GeoJson Geometry.</p>",
                     "shape": "LinearRings"
                 },
                 "Type": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>GeoJson Geometry types like Polygon and MultiPolygon.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "Coordinates",
                 "Type"
             ],
@@ -1272,27 +1286,27 @@
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Earth Observation job.</p>",
                     "shape": "String"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time of the initiated Earth Observation job.</p>",
-                    "shape": "Timestamp"
+                    "shape": "SyntheticTimestamp_date_time"
                 },
                 "DurationInSeconds": {
                     "documentation": "<p>The duration of Earth Observation job, in seconds.</p>",
                     "shape": "Integer"
                 },
                 "ErrorDetails": {
                     "documentation": "<p>Details about the errors generated during the Earth Observation job.</p>",
                     "shape": "EarthObservationJobErrorDetails"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the job.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "ExportErrorDetails": {
                     "documentation": "<p>Details about the errors generated during ExportEarthObservationJob.</p>",
                     "shape": "ExportErrorDetails"
                 },
                 "ExportStatus": {
                     "documentation": "<p>The status of the Earth Observation job.</p>",
@@ -1303,23 +1317,23 @@
                     "shape": "InputConfigOutput"
                 },
                 "JobConfig": {
                     "documentation": "<p>An object containing information about the job configuration.</p>",
                     "shape": "JobConfigInput"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
+                    "documentation": "<p>The Key Management Service key ID for server-side encryption.</p>",
+                    "shape": "KmsKey"
                 },
                 "Name": {
                     "documentation": "<p>The name of the Earth Observation job.</p>",
                     "shape": "String"
                 },
                 "OutputBands": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Bands available in the output of an operation.</p>",
                     "shape": "EarthObservationJobOutputBands"
                 },
                 "Status": {
                     "documentation": "<p>The status of a previously initiated Earth Observation job.</p>",
                     "shape": "EarthObservationJobStatus"
                 },
                 "Tags": {
@@ -1363,15 +1377,15 @@
                     "shape": "String"
                 },
                 "DescriptionPageUrl": {
                     "documentation": "<p>The URL of the description page.</p>",
                     "shape": "String"
                 },
                 "ImageSourceBands": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The list of image source bands in the raster data collection.</p>",
                     "shape": "ImageSourceBandList"
                 },
                 "Name": {
                     "documentation": "<p>The name of the raster data collection.</p>",
                     "shape": "String"
                 },
                 "SupportedFilters": {
@@ -1402,14 +1416,20 @@
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the tile operation.</p>",
                     "location": "querystring",
                     "locationName": "Arn",
                     "shape": "EarthObservationJobArn"
                 },
+                "ExecutionRoleArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specify.</p>",
+                    "location": "querystring",
+                    "locationName": "ExecutionRoleArn",
+                    "shape": "ExecutionRoleArn"
+                },
                 "ImageAssets": {
                     "documentation": "<p>The particular assets or bands to tile.</p>",
                     "location": "querystring",
                     "locationName": "ImageAssets",
                     "shape": "StringListInput"
                 },
                 "ImageMask": {
@@ -1505,27 +1525,27 @@
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Vector Enrichment job.</p>",
                     "shape": "String"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time.</p>",
-                    "shape": "Timestamp"
+                    "shape": "SyntheticTimestamp_date_time"
                 },
                 "DurationInSeconds": {
                     "documentation": "<p>The duration of the Vector Enrichment job, in seconds.</p>",
                     "shape": "Integer"
                 },
                 "ErrorDetails": {
                     "documentation": "<p>Details about the errors generated during the Vector Enrichment job.</p>",
                     "shape": "VectorEnrichmentJobErrorDetails"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the job.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "ExportErrorDetails": {
                     "documentation": "<p>Details about the errors generated during the ExportVectorEnrichmentJob.</p>",
                     "shape": "VectorEnrichmentJobExportErrorDetails"
                 },
                 "ExportStatus": {
                     "documentation": "<p>The export status of the Vector Enrichment job being initiated.</p>",
@@ -1536,16 +1556,16 @@
                     "shape": "VectorEnrichmentJobInputConfig"
                 },
                 "JobConfig": {
                     "documentation": "<p>An object containing information about the job configuration.</p>",
                     "shape": "VectorEnrichmentJobConfig"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
+                    "documentation": "<p>The Key Management Service key ID for server-side encryption.</p>",
+                    "shape": "KmsKey"
                 },
                 "Name": {
                     "documentation": "<p>The name of the Vector Enrichment job.</p>",
                     "shape": "String"
                 },
                 "Status": {
                     "documentation": "<p>The status of the initiated Vector Enrichment job.</p>",
@@ -1585,42 +1605,34 @@
                 "shape": "String"
             },
             "type": "list"
         },
         "InputConfigInput": {
             "documentation": "<p>Input configuration information.</p>",
             "members": {
-                "DataSourceConfig": {
-                    "documentation": "<p>The location of the input data.&gt;</p>",
-                    "shape": "EojDataSourceConfigInput"
-                },
                 "PreviousEarthObservationJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the previous Earth Observation job.</p>",
-                    "shape": "String"
+                    "shape": "EarthObservationJobArn"
                 },
                 "RasterDataCollectionQuery": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing the RasterDataCollection Query consisting of the Area of Interest, RasterDataCollectionArn,TimeRange and Property Filters.</p>",
                     "shape": "RasterDataCollectionQueryInput"
                 }
             },
             "type": "structure"
         },
         "InputConfigOutput": {
             "documentation": "<p>The InputConfig for an EarthObservationJob response.</p>",
             "members": {
-                "DataSourceConfig": {
-                    "documentation": "<p>The location of the input data.</p>",
-                    "shape": "EojDataSourceConfigInput"
-                },
                 "PreviousEarthObservationJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the previous Earth Observation job.</p>",
-                    "shape": "String"
+                    "shape": "EarthObservationJobArn"
                 },
                 "RasterDataCollectionQuery": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing the RasterDataCollection Query consisting of the Area of Interest, RasterDataCollectionArn, RasterDataCollectionName, TimeRange, and Property Filters.</p>",
                     "shape": "RasterDataCollectionQueryOutput"
                 }
             },
             "type": "structure"
         },
         "Integer": {
             "box": true,
@@ -1639,40 +1651,39 @@
                 },
                 "ResourceId": {
                     "documentation": "<p/>",
                     "shape": "String"
                 }
             },
             "required": [
-                "Message",
-                "ResourceId"
+                "Message"
             ],
             "type": "structure"
         },
         "ItemSource": {
-            "documentation": "<p>Structure representing the items in the response for SearchRasterDataCollection.</p>",
+            "documentation": "<p>The structure representing the items in the response for SearchRasterDataCollection.</p>",
             "members": {
                 "Assets": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>This is a dictionary of Asset Objects data associated with the Item that can be downloaded or streamed, each with a unique key.</p>",
                     "shape": "AssetsMap"
                 },
                 "DateTime": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The searchable date and time of the item, in UTC.</p>",
                     "shape": "Timestamp"
                 },
                 "Geometry": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The item Geometry in GeoJson format.</p>",
                     "shape": "Geometry"
                 },
                 "Id": {
                     "documentation": "<p>A unique Id for the source item.</p>",
                     "shape": "String"
                 },
                 "Properties": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>This field contains additional properties of the item.</p>",
                     "shape": "Properties"
                 }
             },
             "required": [
                 "DateTime",
                 "Geometry",
                 "Id"
@@ -1685,15 +1696,15 @@
             },
             "type": "list"
         },
         "JobConfigInput": {
             "documentation": "<p>The input structure for the JobConfig in an EarthObservationJob.</p>",
             "members": {
                 "BandMathConfig": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>An object containing information about the job configuration for BandMath.</p>",
                     "shape": "BandMathConfigInput"
                 },
                 "CloudMaskingConfig": {
                     "documentation": "<p>An object containing information about the job configuration for cloud masking.</p>",
                     "shape": "CloudMaskingConfigInput"
                 },
                 "CloudRemovalConfig": {
@@ -1709,43 +1720,48 @@
                     "shape": "LandCoverSegmentationConfigInput"
                 },
                 "ResamplingConfig": {
                     "documentation": "<p>An object containing information about the job configuration for resampling.</p>",
                     "shape": "ResamplingConfigInput"
                 },
                 "StackConfig": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>An object containing information about the job configuration for a Stacking Earth Observation job.</p>",
                     "shape": "StackConfigInput"
                 },
                 "TemporalStatisticsConfig": {
                     "documentation": "<p>An object containing information about the job configuration for temporal statistics.</p>",
                     "shape": "TemporalStatisticsConfigInput"
                 },
                 "ZonalStatisticsConfig": {
                     "documentation": "<p>An object containing information about the job configuration for zonal statistics.</p>",
                     "shape": "ZonalStatisticsConfigInput"
                 }
             },
             "type": "structure",
             "union": true
         },
+        "KmsKey": {
+            "max": 2048,
+            "min": 0,
+            "type": "string"
+        },
         "LandCoverSegmentationConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for Land Cover Operation type.</p>",
             "members": {},
             "type": "structure"
         },
         "LandsatCloudCoverLandInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing Land Cloud Cover property for Landsat data collection.</p>",
             "members": {
                 "LowerBound": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The minimum value for Land Cloud Cover property filter. This will filter items having Land Cloud Cover greater than or equal to this value.</p>",
                     "shape": "Float"
                 },
                 "UpperBound": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The maximum value for Land Cloud Cover property filter. This will filter items having Land Cloud Cover less than or equal to this value.</p>",
                     "shape": "Float"
                 }
             },
             "required": [
                 "LowerBound",
                 "UpperBound"
             ],
@@ -1823,26 +1839,26 @@
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the list of the Earth Observation jobs.</p>",
                     "shape": "String"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time.</p>",
-                    "shape": "Timestamp"
+                    "shape": "SyntheticTimestamp_date_time"
                 },
                 "DurationInSeconds": {
                     "documentation": "<p>The duration of the session, in seconds.</p>",
                     "shape": "Integer"
                 },
                 "Name": {
                     "documentation": "<p>The names of the Earth Observation jobs in the list.</p>",
                     "shape": "String"
                 },
                 "OperationType": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The operation type for an Earth Observation job.</p>",
                     "shape": "String"
                 },
                 "Status": {
                     "documentation": "<p>The status of the list of the Earth Observation jobs.</p>",
                     "shape": "EarthObservationJobStatus"
                 },
                 "Tags": {
@@ -1974,15 +1990,15 @@
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the list of the Vector Enrichment jobs.</p>",
                     "shape": "VectorEnrichmentJobArn"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time.</p>",
-                    "shape": "Timestamp"
+                    "shape": "SyntheticTimestamp_date_time"
                 },
                 "DurationInSeconds": {
                     "documentation": "<p>The duration of the session, in seconds.</p>",
                     "shape": "Integer"
                 },
                 "Name": {
                     "documentation": "<p>The names of the Vector Enrichment jobs in the list.</p>",
@@ -2014,18 +2030,18 @@
         "LogicalOperator": {
             "enum": [
                 "AND"
             ],
             "type": "string"
         },
         "MapMatchingConfig": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for Map Matching operation type.</p>",
             "members": {
                 "IdAttributeName": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The field name for the data that describes the identifier representing a collection of GPS points belonging to an individual trace.</p>",
                     "shape": "String"
                 },
                 "TimestampAttributeName": {
                     "documentation": "<p>The name of the timestamp attribute.</p>",
                     "shape": "String"
                 },
                 "XAttributeName": {
@@ -2041,22 +2057,16 @@
                 "IdAttributeName",
                 "TimestampAttributeName",
                 "XAttributeName",
                 "YAttributeName"
             ],
             "type": "structure"
         },
-        "MetadataProvider": {
-            "enum": [
-                "PLANET_ORDER"
-            ],
-            "type": "string"
-        },
         "MultiPolygonGeometryInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing Polygon Geometry based on the <a href=\"https://www.rfc-editor.org/rfc/rfc7946#section-3.1.6\">GeoJson spec</a>.</p>",
             "members": {
                 "Coordinates": {
                     "documentation": "<p>The coordinates of the multipolygon geometry.</p>",
                     "shape": "LinearRingsList"
                 }
             },
             "required": [
@@ -2067,18 +2077,18 @@
         "NextToken": {
             "max": 8192,
             "min": 0,
             "sensitive": true,
             "type": "string"
         },
         "Operation": {
-            "documentation": "<p/>",
+            "documentation": "<p>Represents an arithmetic operation to compute spectral index.</p>",
             "members": {
                 "Equation": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Textual representation of the math operation; Equation used to compute the spectral index.</p>",
                     "shape": "String"
                 },
                 "Name": {
                     "documentation": "<p>The name of the operation.</p>",
                     "shape": "String"
                 },
                 "OutputType": {
@@ -2127,35 +2137,35 @@
             },
             "required": [
                 "S3Data"
             ],
             "type": "structure"
         },
         "OutputResolutionResamplingInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>OutputResolution Configuration indicating the target resolution for the output of Resampling operation.</p>",
             "members": {
                 "UserDefined": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>User Defined Resolution for the output of Resampling operation defined by value and unit.</p>",
                     "shape": "UserDefined"
                 }
             },
             "required": [
                 "UserDefined"
             ],
             "type": "structure"
         },
         "OutputResolutionStackInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure representing Output Resolution for Stacking Operation.</p>",
             "members": {
                 "Predefined": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>A string value representing Predefined Output Resolution for a stacking operation. Allowed values are <code>HIGHEST</code>, <code>LOWEST</code>, and <code>AVERAGE</code>.</p>",
                     "shape": "PredefinedResolution"
                 },
                 "UserDefined": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing User Output Resolution for a Stacking operation defined as a value and unit.</p>",
                     "shape": "UserDefined"
                 }
             },
             "type": "structure"
         },
         "OutputType": {
             "enum": [
@@ -2164,35 +2174,35 @@
                 "INT16",
                 "FLOAT64",
                 "UINT16"
             ],
             "type": "string"
         },
         "PlatformInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for specifying Platform. Platform refers to the unique name of the specific platform the instrument is attached to. For satellites it is the name of the satellite, eg. landsat-8 (Landsat-8), sentinel-2a.</p>",
             "members": {
                 "ComparisonOperator": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The ComparisonOperator to use with PlatformInput.</p>",
                     "shape": "ComparisonOperator"
                 },
                 "Value": {
                     "documentation": "<p>The value of the platform.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "Value"
             ],
             "type": "structure"
         },
         "PolygonGeometryInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing Polygon Geometry based on the <a href=\"https://www.rfc-editor.org/rfc/rfc7946#section-3.1.6\">GeoJson spec</a>.</p>",
             "members": {
                 "Coordinates": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Coordinates representing a Polygon based on the <a href=\"https://www.rfc-editor.org/rfc/rfc7946#section-3.1.6\">GeoJson spec</a>.</p>",
                     "shape": "LinearRings"
                 }
             },
             "required": [
                 "Coordinates"
             ],
             "type": "structure"
@@ -2211,96 +2221,96 @@
                 "HIGHEST",
                 "LOWEST",
                 "AVERAGE"
             ],
             "type": "string"
         },
         "Properties": {
-            "documentation": "<p/>",
+            "documentation": "<p>Properties associated with the Item.</p>",
             "members": {
                 "EoCloudCover": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Estimate of cloud cover.</p>",
                     "shape": "Float"
                 },
                 "LandsatCloudCoverLand": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Land cloud cover for Landsat Data Collection.</p>",
                     "shape": "Float"
                 },
                 "Platform": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Platform property. Platform refers to the unique name of the specific platform the instrument is attached to. For satellites it is the name of the satellite, eg. landsat-8 (Landsat-8), sentinel-2a.</p>",
                     "shape": "String"
                 },
                 "ViewOffNadir": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The angle from the sensor between nadir (straight down) and the scene center. Measured in degrees (0-90).</p>",
                     "shape": "Float"
                 },
                 "ViewSunAzimuth": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The sun azimuth angle. From the scene center point on the ground, this is the angle between truth north and the sun. Measured clockwise in degrees (0-360).</p>",
                     "shape": "Float"
                 },
                 "ViewSunElevation": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The sun elevation angle. The angle from the tangent of the scene center point to the sun. Measured from the horizon in degrees (-90-90). Negative values indicate the sun is below the horizon, e.g. sun elevation of -10\u00b0 means the data was captured during <a href=\"https://www.timeanddate.com/astronomy/different-types-twilight.html\">nautical twilight</a>.</p>",
                     "shape": "Float"
                 }
             },
             "type": "structure"
         },
         "Property": {
-            "documentation": "<p/>",
+            "documentation": "<p>Represents a single searchable property to search on.</p>",
             "members": {
                 "EoCloudCover": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing EoCloudCover property filter containing a lower bound and upper bound.</p>",
                     "shape": "EoCloudCoverInput"
                 },
                 "LandsatCloudCoverLand": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing Land Cloud Cover property filter for Landsat collection containing a lower bound and upper bound.</p>",
                     "shape": "LandsatCloudCoverLandInput"
                 },
                 "Platform": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing Platform property filter consisting of value and comparison operator.</p>",
                     "shape": "PlatformInput"
                 },
                 "ViewOffNadir": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing ViewOffNadir property filter containing a lower bound and upper bound.</p>",
                     "shape": "ViewOffNadirInput"
                 },
                 "ViewSunAzimuth": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing ViewSunAzimuth property filter containing a lower bound and upper bound.</p>",
                     "shape": "ViewSunAzimuthInput"
                 },
                 "ViewSunElevation": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing ViewSunElevation property filter containing a lower bound and upper bound.</p>",
                     "shape": "ViewSunElevationInput"
                 }
             },
             "type": "structure",
             "union": true
         },
         "PropertyFilter": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing a single PropertyFilter.</p>",
             "members": {
                 "Property": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Represents a single property to match with when searching a raster data collection.</p>",
                     "shape": "Property"
                 }
             },
             "required": [
                 "Property"
             ],
             "type": "structure"
         },
         "PropertyFilters": {
-            "documentation": "<p/>",
+            "documentation": "<p>A list of PropertyFilter objects.</p>",
             "members": {
                 "LogicalOperator": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The Logical Operator used to combine the Property Filters.</p>",
                     "shape": "LogicalOperator"
                 },
                 "Properties": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>A list of Property Filters.</p>",
                     "shape": "PropertyFiltersList"
                 }
             },
             "type": "structure"
         },
         "PropertyFiltersList": {
             "member": {
@@ -2324,15 +2334,15 @@
                     "shape": "String"
                 },
                 "Name": {
                     "documentation": "<p>The name of the raster data collection.</p>",
                     "shape": "String"
                 },
                 "SupportedFilters": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The list of filters supported by the raster data collection.</p>",
                     "shape": "FilterList"
                 },
                 "Tags": {
                     "documentation": "<p>Each tag consists of a key and a value.</p>",
                     "shape": "Tags"
                 },
                 "Type": {
@@ -2346,207 +2356,188 @@
                 "Name",
                 "SupportedFilters",
                 "Type"
             ],
             "type": "structure"
         },
         "RasterDataCollectionQueryInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for Raster Data Collection Query containing the Area of Interest, TimeRange Filters, and Property Filters.</p>",
             "members": {
                 "AreaOfInterest": {
                     "documentation": "<p>The area of interest being queried for the raster data collection.</p>",
                     "shape": "AreaOfInterest"
                 },
                 "PropertyFilters": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The list of Property filters used in the Raster Data Collection Query.</p>",
                     "shape": "PropertyFilters"
                 },
                 "RasterDataCollectionArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the raster data collection.</p>",
-                    "shape": "String"
+                    "shape": "DataCollectionArn"
                 },
                 "TimeRangeFilter": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The TimeRange Filter used in the RasterDataCollection Query.</p>",
                     "shape": "TimeRangeFilterInput"
                 }
             },
             "required": [
                 "RasterDataCollectionArn",
                 "TimeRangeFilter"
             ],
             "type": "structure"
         },
         "RasterDataCollectionQueryOutput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The output structure contains the Raster Data Collection Query input along with some additional metadata.</p>",
             "members": {
                 "AreaOfInterest": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The Area of Interest used in the search.</p>",
                     "shape": "AreaOfInterest"
                 },
                 "PropertyFilters": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Property filters used in the search.</p>",
                     "shape": "PropertyFilters"
                 },
                 "RasterDataCollectionArn": {
-                    "documentation": "<p/>",
-                    "shape": "String"
+                    "documentation": "<p>The ARN of the Raster Data Collection against which the search is done.</p>",
+                    "shape": "DataCollectionArn"
                 },
                 "RasterDataCollectionName": {
                     "documentation": "<p>The name of the raster data collection.</p>",
                     "shape": "String"
                 },
                 "TimeRangeFilter": {
-                    "documentation": "<p/>",
-                    "shape": "TimeRangeFilterInput"
+                    "documentation": "<p>The TimeRange filter used in the search.</p>",
+                    "shape": "TimeRangeFilterOutput"
                 }
             },
             "required": [
                 "RasterDataCollectionArn",
                 "RasterDataCollectionName",
                 "TimeRangeFilter"
             ],
             "type": "structure"
         },
         "RasterDataCollectionQueryWithBandFilterInput": {
             "documentation": "<p>This is a RasterDataCollectionQueryInput containing AreaOfInterest, Time Range filter and Property filters.</p>",
             "members": {
                 "AreaOfInterest": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The Area of interest to be used in the search query.</p>",
                     "shape": "AreaOfInterest"
                 },
                 "BandFilter": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The list of Bands to be displayed in the result for each item.</p>",
                     "shape": "StringListInput"
                 },
                 "PropertyFilters": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The Property Filters used in the search query.</p>",
                     "shape": "PropertyFilters"
                 },
                 "TimeRangeFilter": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The TimeRange Filter used in the search query.</p>",
                     "shape": "TimeRangeFilterInput"
                 }
             },
             "required": [
                 "TimeRangeFilter"
             ],
             "type": "structure"
         },
         "ResamplingConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing input for resampling operation.</p>",
             "members": {
                 "AlgorithmName": {
                     "documentation": "<p>The name of the algorithm used for resampling.</p>",
                     "shape": "AlgorithmNameResampling"
                 },
                 "OutputResolution": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing output resolution (in target georeferenced units) of the result of resampling operation.</p>",
                     "shape": "OutputResolutionResamplingInput"
                 },
                 "TargetBands": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Bands used in the operation. If no target bands are specified, it uses all bands available in the input.</p>",
                     "shape": "StringListInput"
                 }
             },
             "required": [
                 "OutputResolution"
             ],
             "type": "structure"
         },
         "ResourceNotFoundException": {
-            "documentation": "<p/>",
+            "documentation": "<p>The request references a resource which does not exist.</p>",
             "error": {
                 "httpStatusCode": 404,
                 "senderFault": true
             },
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "String"
                 },
                 "ResourceId": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Identifier of the resource that was not found.</p>",
                     "shape": "String"
                 }
             },
             "required": [
-                "Message",
-                "ResourceId"
+                "Message"
             ],
             "type": "structure"
         },
         "ReverseGeocodingConfig": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for Reverse Geocoding operation type.</p>",
             "members": {
                 "XAttributeName": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The field name for the data that describes x-axis coordinate, eg. longitude of a point.</p>",
                     "shape": "String"
                 },
                 "YAttributeName": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The field name for the data that describes y-axis coordinate, eg. latitude of a point.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "XAttributeName",
                 "YAttributeName"
             ],
             "type": "structure"
         },
-        "S3DataInput": {
-            "documentation": "<p>Path to Amazon S3 storage location for input data.</p>",
-            "members": {
-                "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
-                },
-                "MetadataProvider": {
-                    "documentation": "<p/>",
-                    "shape": "MetadataProvider"
-                },
-                "S3Uri": {
-                    "documentation": "<p>The URL to the Amazon S3 input.</p>",
-                    "shape": "String"
-                }
-            },
-            "required": [
-                "MetadataProvider",
-                "S3Uri"
-            ],
-            "type": "structure"
+        "S3Uri": {
+            "pattern": "^s3://([^/]+)/?(.*)$",
+            "type": "string"
         },
         "SearchRasterDataCollectionInput": {
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the raster data collection.</p>",
                     "shape": "DataCollectionArn"
                 },
                 "NextToken": {
                     "documentation": "<p>If the previous response was truncated, you receive this token. Use it in your next request to receive the next set of results.</p>",
                     "shape": "NextToken"
                 },
                 "RasterDataCollectionQuery": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>RasterDataCollectionQuery consisting of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_geospatial_AreaOfInterest.html\">AreaOfInterest(AOI)</a>, <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_geospatial_PropertyFilter.html\">PropertyFilters</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_geospatial_TimeRangeFilterInput.html\">TimeRangeFilterInput</a> used in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_geospatial_SearchRasterDataCollection.html\">SearchRasterDataCollection</a>.</p>",
                     "shape": "RasterDataCollectionQueryWithBandFilterInput"
                 }
             },
             "required": [
                 "Arn",
                 "RasterDataCollectionQuery"
             ],
             "type": "structure"
         },
         "SearchRasterDataCollectionOutput": {
             "members": {
                 "ApproximateResultCount": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Approximate number of results in the response.</p>",
                     "shape": "Integer"
                 },
                 "Items": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>List of items matching the Raster DataCollectionQuery.</p>",
                     "shape": "ItemSourceList"
                 },
                 "NextToken": {
                     "documentation": "<p>If the previous response was truncated, you receive this token. Use it in your next request to receive the next set of results.</p>",
                     "shape": "NextToken"
                 }
             },
@@ -2563,113 +2554,123 @@
             },
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "String"
                 },
                 "ResourceId": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Identifier of the resource affected.</p>",
                     "shape": "String"
                 }
             },
             "required": [
-                "Message",
-                "ResourceId"
+                "Message"
             ],
             "type": "structure"
         },
         "SortOrder": {
             "enum": [
                 "ASCENDING",
                 "DESCENDING"
             ],
             "type": "string"
         },
         "StackConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for Stacking Operation.</p>",
             "members": {
                 "OutputResolution": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The structure representing output resolution (in target georeferenced units) of the result of stacking operation.</p>",
                     "shape": "OutputResolutionStackInput"
                 },
                 "TargetBands": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>A list of bands to be stacked in the specified order. When the parameter is not provided, all the available bands in the data collection are stacked in the alphabetical order of their asset names.</p>",
                     "shape": "StringListInput"
                 }
             },
             "type": "structure"
         },
         "StartEarthObservationJobInput": {
             "members": {
                 "ClientToken": {
                     "documentation": "<p>A unique token that guarantees that the call to this API is idempotent.</p>",
                     "idempotencyToken": true,
-                    "shape": "String"
+                    "shape": "StartEarthObservationJobInputClientTokenString"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the job.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "InputConfig": {
                     "documentation": "<p>Input configuration information for the Earth Observation job.</p>",
                     "shape": "InputConfigInput"
                 },
                 "JobConfig": {
                     "documentation": "<p>An object containing information about the job configuration.</p>",
                     "shape": "JobConfigInput"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
+                    "documentation": "<p>The Key Management Service key ID for server-side encryption.</p>",
+                    "shape": "KmsKey"
                 },
                 "Name": {
                     "documentation": "<p>The name of the Earth Observation job.</p>",
-                    "shape": "String"
+                    "shape": "StartEarthObservationJobInputNameString"
                 },
                 "Tags": {
                     "documentation": "<p>Each tag consists of a key and a value.</p>",
                     "shape": "Tags"
                 }
             },
             "required": [
+                "ExecutionRoleArn",
                 "InputConfig",
                 "JobConfig",
                 "Name"
             ],
             "type": "structure"
         },
+        "StartEarthObservationJobInputClientTokenString": {
+            "max": 64,
+            "min": 36,
+            "type": "string"
+        },
+        "StartEarthObservationJobInputNameString": {
+            "max": 200,
+            "min": 0,
+            "type": "string"
+        },
         "StartEarthObservationJobOutput": {
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Earth Observation job.</p>",
                     "shape": "String"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time.</p>",
-                    "shape": "Timestamp"
+                    "shape": "SyntheticTimestamp_date_time"
                 },
                 "DurationInSeconds": {
                     "documentation": "<p>The duration of the session, in seconds.</p>",
                     "shape": "Integer"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the job.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "InputConfig": {
                     "documentation": "<p>Input configuration information for the Earth Observation job.</p>",
                     "shape": "InputConfigOutput"
                 },
                 "JobConfig": {
                     "documentation": "<p>An object containing information about the job configuration.</p>",
                     "shape": "JobConfigInput"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
+                    "documentation": "<p>The Key Management Service key ID for server-side encryption.</p>",
+                    "shape": "KmsKey"
                 },
                 "Name": {
                     "documentation": "<p>The name of the Earth Observation job.</p>",
                     "shape": "String"
                 },
                 "Status": {
                     "documentation": "<p>The status of the Earth Observation job.</p>",
@@ -2680,89 +2681,100 @@
                     "shape": "Tags"
                 }
             },
             "required": [
                 "Arn",
                 "CreationTime",
                 "DurationInSeconds",
+                "ExecutionRoleArn",
                 "JobConfig",
                 "Name",
                 "Status"
             ],
             "type": "structure"
         },
         "StartVectorEnrichmentJobInput": {
             "members": {
                 "ClientToken": {
                     "documentation": "<p>A unique token that guarantees that the call to this API is idempotent.</p>",
                     "idempotencyToken": true,
-                    "shape": "String"
+                    "shape": "StartVectorEnrichmentJobInputClientTokenString"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the job.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "InputConfig": {
                     "documentation": "<p>Input configuration information for the Vector Enrichment job.</p>",
                     "shape": "VectorEnrichmentJobInputConfig"
                 },
                 "JobConfig": {
                     "documentation": "<p>An object containing information about the job configuration.</p>",
                     "shape": "VectorEnrichmentJobConfig"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
+                    "documentation": "<p>The Key Management Service key ID for server-side encryption.</p>",
+                    "shape": "KmsKey"
                 },
                 "Name": {
                     "documentation": "<p>The name of the Vector Enrichment job.</p>",
-                    "shape": "String"
+                    "shape": "StartVectorEnrichmentJobInputNameString"
                 },
                 "Tags": {
                     "documentation": "<p>Each tag consists of a key and a value.</p>",
                     "shape": "Tags"
                 }
             },
             "required": [
                 "ExecutionRoleArn",
                 "InputConfig",
                 "JobConfig",
                 "Name"
             ],
             "type": "structure"
         },
+        "StartVectorEnrichmentJobInputClientTokenString": {
+            "max": 64,
+            "min": 36,
+            "type": "string"
+        },
+        "StartVectorEnrichmentJobInputNameString": {
+            "max": 200,
+            "min": 0,
+            "type": "string"
+        },
         "StartVectorEnrichmentJobOutput": {
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Vector Enrichment job.</p>",
                     "shape": "VectorEnrichmentJobArn"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time.</p>",
-                    "shape": "Timestamp"
+                    "shape": "SyntheticTimestamp_date_time"
                 },
                 "DurationInSeconds": {
                     "documentation": "<p>The duration of the Vector Enrichment job, in seconds.</p>",
                     "shape": "Integer"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the job.</p>",
-                    "shape": "String"
+                    "shape": "ExecutionRoleArn"
                 },
                 "InputConfig": {
                     "documentation": "<p>Input configuration information for starting the Vector Enrichment job.</p>",
                     "shape": "VectorEnrichmentJobInputConfig"
                 },
                 "JobConfig": {
                     "documentation": "<p>An object containing information about the job configuration.</p>",
                     "shape": "VectorEnrichmentJobConfig"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
+                    "documentation": "<p>The Key Management Service key ID for server-side encryption.</p>",
+                    "shape": "KmsKey"
                 },
                 "Name": {
                     "documentation": "<p>The name of the Vector Enrichment job.</p>",
                     "shape": "String"
                 },
                 "Status": {
                     "documentation": "<p>The status of the Vector Enrichment job being started.</p>",
@@ -2828,14 +2840,18 @@
         "StringListInput": {
             "member": {
                 "shape": "String"
             },
             "min": 1,
             "type": "list"
         },
+        "SyntheticTimestamp_date_time": {
+            "timestampFormat": "iso8601",
+            "type": "timestamp"
+        },
         "TagKeyList": {
             "max": 50,
             "member": {
                 "shape": "String"
             },
             "min": 1,
             "type": "list"
@@ -2884,26 +2900,26 @@
                 "MEAN",
                 "MEDIAN",
                 "STANDARD_DEVIATION"
             ],
             "type": "string"
         },
         "TemporalStatisticsConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing the configuration for Temporal Statistics operation.</p>",
             "members": {
                 "GroupBy": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The input for the temporal statistics grouping by time frequency option.</p>",
                     "shape": "GroupBy"
                 },
                 "Statistics": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The list of the statistics method options.</p>",
                     "shape": "TemporalStatisticsListInput"
                 },
                 "TargetBands": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The list of target band names for the temporal statistic to calculate.</p>",
                     "shape": "StringListInput"
                 }
             },
             "required": [
                 "Statistics"
             ],
             "type": "structure"
@@ -2928,16 +2944,15 @@
                 },
                 "ResourceId": {
                     "documentation": "<p/>",
                     "shape": "String"
                 }
             },
             "required": [
-                "Message",
-                "ResourceId"
+                "Message"
             ],
             "type": "structure"
         },
         "TimeRangeFilterInput": {
             "documentation": "<p>The input for the time-range filter.</p>",
             "members": {
                 "EndTime": {
@@ -2952,14 +2967,33 @@
             "required": [
                 "EndTime",
                 "StartTime"
             ],
             "sensitive": true,
             "type": "structure"
         },
+        "TimeRangeFilterOutput": {
+            "documentation": "<p>The output structure of the time range filter.</p>",
+            "members": {
+                "EndTime": {
+                    "documentation": "<p>The ending time for the time range filter.</p>",
+                    "shape": "SyntheticTimestamp_date_time"
+                },
+                "StartTime": {
+                    "documentation": "<p>The starting time for the time range filter.</p>",
+                    "shape": "SyntheticTimestamp_date_time"
+                }
+            },
+            "required": [
+                "EndTime",
+                "StartTime"
+            ],
+            "sensitive": true,
+            "type": "structure"
+        },
         "Timestamp": {
             "type": "timestamp"
         },
         "Unit": {
             "enum": [
                 "METERS"
             ],
@@ -2987,22 +3021,22 @@
             "type": "structure"
         },
         "UntagResourceResponse": {
             "members": {},
             "type": "structure"
         },
         "UserDefined": {
-            "documentation": "<p/>",
+            "documentation": "<p>The output resolution (in target georeferenced units) of the result of the operation</p>",
             "members": {
                 "Unit": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The units for output resolution of the result.</p>",
                     "shape": "Unit"
                 },
                 "Value": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The value for output resolution of the result.</p>",
                     "shape": "Float"
                 }
             },
             "required": [
                 "Unit",
                 "Value"
             ],
@@ -3021,43 +3055,42 @@
                 },
                 "ResourceId": {
                     "documentation": "<p/>",
                     "shape": "String"
                 }
             },
             "required": [
-                "Message",
-                "ResourceId"
+                "Message"
             ],
             "type": "structure"
         },
         "VectorEnrichmentJobArn": {
             "pattern": "^arn:aws[a-z-]{0,12}:sagemaker-geospatial:[a-z0-9-]{1,25}:[0-9]{12}:vector-enrichment-job/[a-z0-9]{12,}$",
             "type": "string"
         },
         "VectorEnrichmentJobConfig": {
             "documentation": "<p>It contains configs such as ReverseGeocodingConfig and MapMatchingConfig.</p>",
             "members": {
                 "MapMatchingConfig": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The input structure for Map Matching operation type.</p>",
                     "shape": "MapMatchingConfig"
                 },
                 "ReverseGeocodingConfig": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The input structure for Reverse Geocoding operation type.</p>",
                     "shape": "ReverseGeocodingConfig"
                 }
             },
             "type": "structure",
             "union": true
         },
         "VectorEnrichmentJobDataSourceConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for the data source that represents the storage type of the input data objects.</p>",
             "members": {
                 "S3Data": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The input structure for the Amazon S3 data that represents the Amazon S3 location of the input data objects.</p>",
                     "shape": "VectorEnrichmentJobS3Data"
                 }
             },
             "type": "structure",
             "union": true
         },
         "VectorEnrichmentJobDocumentType": {
@@ -3091,15 +3124,15 @@
             "documentation": "<p>VectorEnrichmentJob export error details in response from GetVectorEnrichmentJob.</p>",
             "members": {
                 "Message": {
                     "documentation": "<p>The message providing details about the errors generated during the Vector Enrichment job.</p>",
                     "shape": "String"
                 },
                 "Type": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The output error details for an Export operation on a Vector Enrichment job.</p>",
                     "shape": "VectorEnrichmentJobExportErrorType"
                 }
             },
             "type": "structure"
         },
         "VectorEnrichmentJobExportErrorType": {
             "enum": [
@@ -3116,19 +3149,19 @@
             ],
             "type": "string"
         },
         "VectorEnrichmentJobInputConfig": {
             "documentation": "<p>The input structure for the InputConfig in a VectorEnrichmentJob.</p>",
             "members": {
                 "DataSourceConfig": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The input structure for the data source that represents the storage type of the input data objects.</p>",
                     "shape": "VectorEnrichmentJobDataSourceConfigInput"
                 },
                 "DocumentType": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The input structure that defines the data source file type.</p>",
                     "shape": "VectorEnrichmentJobDocumentType"
                 }
             },
             "required": [
                 "DataSourceConfig",
                 "DocumentType"
             ],
@@ -3140,20 +3173,20 @@
             },
             "type": "list"
         },
         "VectorEnrichmentJobS3Data": {
             "documentation": "<p>The Amazon S3 data for the Vector Enrichment job.</p>",
             "members": {
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Key Management Service (KMS) key ID for server-side encryption.</p>",
-                    "shape": "String"
+                    "documentation": "<p>The Key Management Service key ID for server-side encryption.</p>",
+                    "shape": "KmsKey"
                 },
                 "S3Uri": {
                     "documentation": "<p>The URL to the Amazon S3 data for the Vector Enrichment job.</p>",
-                    "shape": "String"
+                    "shape": "S3Uri"
                 }
             },
             "required": [
                 "S3Uri"
             ],
             "type": "structure"
         },
@@ -3174,51 +3207,51 @@
             "enum": [
                 "REVERSE_GEOCODING",
                 "MAP_MATCHING"
             ],
             "type": "string"
         },
         "ViewOffNadirInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for specifying ViewOffNadir property filter. ViewOffNadir refers to the angle from the sensor between nadir (straight down) and the scene center. Measured in degrees (0-90).</p>",
             "members": {
                 "LowerBound": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The minimum value for ViewOffNadir property filter. This filters items having ViewOffNadir greater than or equal to this value. </p>",
                     "shape": "Float"
                 },
                 "UpperBound": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The maximum value for ViewOffNadir property filter. This filters items having ViewOffNadir lesser than or equal to this value.</p>",
                     "shape": "Float"
                 }
             },
             "required": [
                 "LowerBound",
                 "UpperBound"
             ],
             "type": "structure"
         },
         "ViewSunAzimuthInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for specifying ViewSunAzimuth property filter. ViewSunAzimuth refers to the Sun azimuth angle. From the scene center point on the ground, this is the angle between truth north and the sun. Measured clockwise in degrees (0-360).</p>",
             "members": {
                 "LowerBound": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The minimum value for ViewSunAzimuth property filter. This filters items having ViewSunAzimuth greater than or equal to this value.</p>",
                     "shape": "Float"
                 },
                 "UpperBound": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The maximum value for ViewSunAzimuth property filter. This filters items having ViewSunAzimuth lesser than or equal to this value.</p>",
                     "shape": "Float"
                 }
             },
             "required": [
                 "LowerBound",
                 "UpperBound"
             ],
             "type": "structure"
         },
         "ViewSunElevationInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The input structure for specifying ViewSunElevation angle property filter. </p>",
             "members": {
                 "LowerBound": {
                     "documentation": "<p>The lower bound to view the sun elevation.</p>",
                     "shape": "Float"
                 },
                 "UpperBound": {
                     "documentation": "<p>The upper bound to view the sun elevation.</p>",
@@ -3239,27 +3272,31 @@
                 "MAX",
                 "MIN",
                 "SUM"
             ],
             "type": "string"
         },
         "ZonalStatisticsConfigInput": {
-            "documentation": "<p/>",
+            "documentation": "<p>The structure representing input configuration of ZonalStatistics operation.</p>",
             "members": {
                 "Statistics": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>List of zonal statistics to compute.</p>",
                     "shape": "ZonalStatisticsListInput"
                 },
                 "TargetBands": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Bands used in the operation. If no target bands are specified, it uses all bands available input.</p>",
                     "shape": "StringListInput"
                 },
                 "ZoneS3Path": {
-                    "documentation": "<p/>",
-                    "shape": "String"
+                    "documentation": "<p>The Amazon S3 path pointing to the GeoJSON containing the polygonal zones.</p>",
+                    "shape": "S3Uri"
+                },
+                "ZoneS3PathKmsKeyId": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) or an ID of a Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to decrypt your output artifacts with Amazon S3 server-side encryption. The SageMaker execution role must have <code>kms:GenerateDataKey</code> permission.</p> <p>The <code>KmsKeyId</code> can be any of the following formats:</p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:&lt;region&gt;:&lt;account&gt;:key/&lt;key-id-12ab-34cd-56ef-1234567890ab&gt;\"</code> </p> </li> </ul> <p>For more information about key identifiers, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id-key-id\">Key identifiers (KeyID)</a> in the Amazon Web Services Key Management Service (Amazon Web Services KMS) documentation.</p>",
+                    "shape": "KmsKey"
                 }
             },
             "required": [
                 "Statistics",
                 "ZoneS3Path"
             ],
             "type": "structure"
```

### Comparing `botocore-a-la-carte-sagemaker-geospatial-1.29.99/botocore_a_la_carte_sagemaker_geospatial.egg-info/PKG-INFO` & `botocore-a-la-carte-sagemaker-geospatial-1.30.0/botocore_a_la_carte_sagemaker_geospatial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker-geospatial
-Version: 1.29.99
+Version: 1.30.0
 Summary: sagemaker-geospatial data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-geospatial-1.29.99/setup.py` & `botocore-a-la-carte-sagemaker-geospatial-1.30.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-sagemaker-geospatial',
-    version="1.29.99",
+    version="1.30.0",
     description='sagemaker-geospatial data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/sagemaker-geospatial/*/*.json'],
```

