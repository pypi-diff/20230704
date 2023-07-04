# Comparing `tmp/botocore-a-la-carte-location-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-location-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-location-1.29.99.tar", last modified: Sat Mar 25 01:22:55 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-location-1.30.0.tar", last modified: Tue Jul  4 01:44:46 2023, max compression
```

## Comparing `botocore-a-la-carte-location-1.29.99.tar` & `botocore-a-la-carte-location-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:55.232312 botocore-a-la-carte-location-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:54.000000 botocore-a-la-carte-location-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:22:55.232312 botocore-a-la-carte-location-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:55.228312 botocore-a-la-carte-location-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:55.228312 botocore-a-la-carte-location-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:55.228312 botocore-a-la-carte-location-1.29.99/botocore/data/location/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:55.232312 botocore-a-la-carte-location-1.29.99/botocore/data/location/2020-11-19/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-03-25 01:22:12.000000 botocore-a-la-carte-location-1.29.99/botocore/data/location/2020-11-19/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-location-1.29.99/botocore/data/location/2020-11-19/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-25 01:22:12.000000 botocore-a-la-carte-location-1.29.99/botocore/data/location/2020-11-19/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   272948 2023-03-25 01:22:12.000000 botocore-a-la-carte-location-1.29.99/botocore/data/location/2020-11-19/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:55.232312 botocore-a-la-carte-location-1.29.99/botocore_a_la_carte_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-25 01:22:55.000000 botocore-a-la-carte-location-1.29.99/botocore_a_la_carte_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-25 01:22:55.000000 botocore-a-la-carte-location-1.29.99/botocore_a_la_carte_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:55.000000 botocore-a-la-carte-location-1.29.99/botocore_a_la_carte_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:55.000000 botocore-a-la-carte-location-1.29.99/botocore_a_la_carte_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:55.232312 botocore-a-la-carte-location-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-25 01:22:54.000000 botocore-a-la-carte-location-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:46.194702 botocore-a-la-carte-location-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:45.000000 botocore-a-la-carte-location-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:46.194702 botocore-a-la-carte-location-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:46.190701 botocore-a-la-carte-location-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:46.190701 botocore-a-la-carte-location-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:46.190701 botocore-a-la-carte-location-1.30.0/botocore/data/location/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:46.194702 botocore-a-la-carte-location-1.30.0/botocore/data/location/2020-11-19/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-04 01:44:02.000000 botocore-a-la-carte-location-1.30.0/botocore/data/location/2020-11-19/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-location-1.30.0/botocore/data/location/2020-11-19/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-04 01:44:02.000000 botocore-a-la-carte-location-1.30.0/botocore/data/location/2020-11-19/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   280030 2023-07-04 01:44:02.000000 botocore-a-la-carte-location-1.30.0/botocore/data/location/2020-11-19/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:46.194702 botocore-a-la-carte-location-1.30.0/botocore_a_la_carte_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 01:44:46.000000 botocore-a-la-carte-location-1.30.0/botocore_a_la_carte_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-04 01:44:46.000000 botocore-a-la-carte-location-1.30.0/botocore_a_la_carte_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:46.000000 botocore-a-la-carte-location-1.30.0/botocore_a_la_carte_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:46.000000 botocore-a-la-carte-location-1.30.0/botocore_a_la_carte_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:46.194702 botocore-a-la-carte-location-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-04 01:44:45.000000 botocore-a-la-carte-location-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-location-1.29.99/LICENSE.txt` & `botocore-a-la-carte-location-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-location-1.29.99/PKG-INFO` & `botocore-a-la-carte-location-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-location
-Version: 1.29.99
+Version: 1.30.0
 Summary: location data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-location-1.29.99/botocore/data/location/2020-11-19/endpoint-rule-set-1.json` & `botocore-a-la-carte-location-1.30.0/botocore/data/location/2020-11-19/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-location-1.29.99/botocore/data/location/2020-11-19/paginators-1.json` & `botocore-a-la-carte-location-1.30.0/botocore/data/location/2020-11-19/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-location-1.29.99/botocore/data/location/2020-11-19/service-2.json` & `botocore-a-la-carte-location-1.30.0/botocore/data/location/2020-11-19/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997073001451831%*

 * *Differences: {"'operations'": "{'BatchUpdateDevicePosition': {'documentation': '<p>Uploads position update data "*

 * *                 'for one or more devices to a tracker resource (up to 10 devices per batch). '*

 * *                 'Amazon Location uses the data when it reports the last known device position and '*

 * *                 'position history. Amazon Location retains location data for 30 days.</p> <note> '*

 * *                 '<p>Position updates are handled based on the <code>PositionFiltering</code> '*

 * *                 ' […]*

```diff
@@ -225,15 +225,15 @@
             },
             "name": "BatchPutGeofence",
             "output": {
                 "shape": "BatchPutGeofenceResponse"
             }
         },
         "BatchUpdateDevicePosition": {
-            "documentation": "<p>Uploads position update data for one or more devices to a tracker resource. Amazon Location uses the data when it reports the last known device position and position history. Amazon Location retains location data for 30 days.</p> <note> <p>Position updates are handled based on the <code>PositionFiltering</code> property of the tracker. When <code>PositionFiltering</code> is set to <code>TimeBased</code>, updates are evaluated against linked geofence collections, and location data is stored at a maximum of one position per 30 second interval. If your update frequency is more often than every 30 seconds, only one update per 30 seconds is stored for each unique device ID.</p> <p>When <code>PositionFiltering</code> is set to <code>DistanceBased</code> filtering, location data is stored and evaluated against linked geofence collections only if the device has moved more than 30 m (98.4 ft).</p> <p>When <code>PositionFiltering</code> is set to <code>AccuracyBased</code> filtering, location data is stored and evaluated against linked geofence collections only if the device has moved more than the measured accuracy. For example, if two consecutive updates from a device have a horizontal accuracy of 5 m and 10 m, the second update is neither stored or evaluated if the device has moved less than 15 m. If <code>PositionFiltering</code> is set to <code>AccuracyBased</code> filtering, Amazon Location uses the default value <code>{ \"Horizontal\": 0}</code> when accuracy is not provided on a <code>DevicePositionUpdate</code>.</p> </note>",
+            "documentation": "<p>Uploads position update data for one or more devices to a tracker resource (up to 10 devices per batch). Amazon Location uses the data when it reports the last known device position and position history. Amazon Location retains location data for 30 days.</p> <note> <p>Position updates are handled based on the <code>PositionFiltering</code> property of the tracker. When <code>PositionFiltering</code> is set to <code>TimeBased</code>, updates are evaluated against linked geofence collections, and location data is stored at a maximum of one position per 30 second interval. If your update frequency is more often than every 30 seconds, only one update per 30 seconds is stored for each unique device ID.</p> <p>When <code>PositionFiltering</code> is set to <code>DistanceBased</code> filtering, location data is stored and evaluated against linked geofence collections only if the device has moved more than 30 m (98.4 ft).</p> <p>When <code>PositionFiltering</code> is set to <code>AccuracyBased</code> filtering, location data is stored and evaluated against linked geofence collections only if the device has moved more than the measured accuracy. For example, if two consecutive updates from a device have a horizontal accuracy of 5 m and 10 m, the second update is neither stored or evaluated if the device has moved less than 15 m. If <code>PositionFiltering</code> is set to <code>AccuracyBased</code> filtering, Amazon Location uses the default value <code>{ \"Horizontal\": 0}</code> when accuracy is not provided on a <code>DevicePositionUpdate</code>.</p> </note>",
             "endpoint": {
                 "hostPrefix": "tracking."
             },
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
@@ -543,14 +543,17 @@
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "ValidationException"
                 },
                 {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
                     "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/tracking/v0/trackers",
                 "responseCode": 200
@@ -2087,15 +2090,17 @@
         "ApiKey": {
             "max": 1000,
             "min": 0,
             "sensitive": true,
             "type": "string"
         },
         "ApiKeyAction": {
-            "pattern": "^geo:GetMap\\*$",
+            "max": 200,
+            "min": 5,
+            "pattern": "^geo:\\w*\\*?$",
             "type": "string"
         },
         "ApiKeyFilter": {
             "documentation": "<p>Options for filtering API keys.</p>",
             "members": {
                 "KeyStatus": {
                     "documentation": "<p>Filter on <code>Active</code> or <code>Expired</code> API keys.</p>",
@@ -2123,15 +2128,15 @@
             "required": [
                 "AllowActions",
                 "AllowResources"
             ],
             "type": "structure"
         },
         "ApiKeyRestrictionsAllowActionsList": {
-            "max": 1,
+            "max": 7,
             "member": {
                 "shape": "ApiKeyAction"
             },
             "min": 1,
             "type": "list"
         },
         "ApiKeyRestrictionsAllowReferersList": {
@@ -2530,14 +2535,18 @@
         "BatchPutGeofenceRequestEntry": {
             "documentation": "<p>Contains geofence geometry details. </p>",
             "members": {
                 "GeofenceId": {
                     "documentation": "<p>The identifier for the geofence to be stored in a given geofence collection.</p>",
                     "shape": "Id"
                 },
+                "GeofenceProperties": {
+                    "documentation": "<p>Specifies additional user-defined properties to store with the Geofence. An array of key-value pairs.</p>",
+                    "shape": "PropertyMap"
+                },
                 "Geometry": {
                     "documentation": "<p>Contains the details of the position of the geofence. Can be either a polygon or a circle. Including both will return a validation error.</p> <note> <p>Each <a href=\"https://docs.aws.amazon.com/location-geofences/latest/APIReference/API_GeofenceGeometry.html\"> geofence polygon</a> can have a maximum of 1,000 vertices.</p> </note>",
                     "shape": "GeofenceGeometry"
                 }
             },
             "required": [
                 "GeofenceId",
@@ -2625,15 +2634,15 @@
                 "TrackerName": {
                     "documentation": "<p>The name of the tracker resource to update.</p>",
                     "location": "uri",
                     "locationName": "TrackerName",
                     "shape": "ResourceName"
                 },
                 "Updates": {
-                    "documentation": "<p>Contains the position update details for each device.</p>",
+                    "documentation": "<p>Contains the position update details for each device, up to 10 devices.</p>",
                     "shape": "BatchUpdateDevicePositionRequestUpdatesList"
                 }
             },
             "required": [
                 "TrackerName",
                 "Updates"
             ],
@@ -3019,14 +3028,26 @@
             ],
             "type": "structure"
         },
         "CountryCode": {
             "pattern": "^[A-Z]{3}$",
             "type": "string"
         },
+        "CountryCode3": {
+            "max": 3,
+            "min": 3,
+            "pattern": "^[A-Z]{3}$",
+            "type": "string"
+        },
+        "CountryCode3OrEmpty": {
+            "max": 3,
+            "min": 0,
+            "pattern": "^[A-Z]{3}$|^$",
+            "type": "string"
+        },
         "CountryCodeList": {
             "max": 100,
             "member": {
                 "shape": "CountryCode"
             },
             "min": 1,
             "type": "list"
@@ -3241,15 +3262,15 @@
             "members": {
                 "CreateTime": {
                     "documentation": "<p>The timestamp for when the place index resource was created in <a href=\"https://www.iso.org/iso-8601-date-and-time-format.html\">ISO 8601</a> format: <code>YYYY-MM-DDThh:mm:ss.sssZ</code>. </p>",
                     "shape": "Timestamp"
                 },
                 "IndexArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the place index resource. Used to specify a resource across Amazon Web Services. </p> <ul> <li> <p>Format example: <code>arn:aws:geo:region:account-id:place-index/ExamplePlaceIndex</code> </p> </li> </ul>",
-                    "shape": "Arn"
+                    "shape": "GeoArn"
                 },
                 "IndexName": {
                     "documentation": "<p>The name for the place index resource.</p>",
                     "shape": "ResourceName"
                 }
             },
             "required": [
@@ -3290,15 +3311,15 @@
             ],
             "type": "structure"
         },
         "CreateRouteCalculatorResponse": {
             "members": {
                 "CalculatorArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the route calculator resource. Use the ARN when you specify a resource across all Amazon Web Services.</p> <ul> <li> <p>Format example: <code>arn:aws:geo:region:account-id:route-calculator/ExampleCalculator</code> </p> </li> </ul>",
-                    "shape": "Arn"
+                    "shape": "GeoArn"
                 },
                 "CalculatorName": {
                     "documentation": "<p>The name of the route calculator resource. </p> <ul> <li> <p>For example, <code>ExampleRouteCalculator</code>.</p> </li> </ul>",
                     "shape": "ResourceName"
                 },
                 "CreateTime": {
                     "documentation": "<p>The timestamp when the route calculator resource was created in <a href=\"https://www.iso.org/iso-8601-date-and-time-format.html\">ISO 8601</a> format: <code>YYYY-MM-DDThh:mm:ss.sssZ</code>. </p> <ul> <li> <p>For example, <code>2020\u201307-2T12:15:20.000Z+01:00</code> </p> </li> </ul>",
@@ -3717,15 +3738,15 @@
                 },
                 "Description": {
                     "documentation": "<p>The optional description for the place index resource.</p>",
                     "shape": "ResourceDescription"
                 },
                 "IndexArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the place index resource. Used to specify a resource across Amazon Web Services. </p> <ul> <li> <p>Format example: <code>arn:aws:geo:region:account-id:place-index/ExamplePlaceIndex</code> </p> </li> </ul>",
-                    "shape": "Arn"
+                    "shape": "GeoArn"
                 },
                 "IndexName": {
                     "documentation": "<p>The name of the place index resource being described.</p>",
                     "shape": "ResourceName"
                 },
                 "PricingPlan": {
                     "deprecated": true,
@@ -3767,15 +3788,15 @@
             ],
             "type": "structure"
         },
         "DescribeRouteCalculatorResponse": {
             "members": {
                 "CalculatorArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the Route calculator resource. Use the ARN when you specify a resource across Amazon Web Services.</p> <ul> <li> <p>Format example: <code>arn:aws:geo:region:account-id:route-calculator/ExampleCalculator</code> </p> </li> </ul>",
-                    "shape": "Arn"
+                    "shape": "GeoArn"
                 },
                 "CalculatorName": {
                     "documentation": "<p>The name of the route calculator resource being described.</p>",
                     "shape": "ResourceName"
                 },
                 "CreateTime": {
                     "documentation": "<p>The timestamp when the route calculator resource was created in <a href=\"https://www.iso.org/iso-8601-date-and-time-format.html\">ISO 8601</a> format: <code>YYYY-MM-DDThh:mm:ss.sssZ</code>. </p> <ul> <li> <p>For example, <code>2020\u201307-2T12:15:20.000Z+01:00</code> </p> </li> </ul>",
@@ -3995,14 +4016,22 @@
             ],
             "type": "string"
         },
         "Double": {
             "box": true,
             "type": "double"
         },
+        "FilterPlaceCategoryList": {
+            "max": 5,
+            "member": {
+                "shape": "PlaceCategory"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "GeoArn": {
             "max": 1600,
             "min": 0,
             "pattern": "^arn(:[a-z0-9]+([.-][a-z0-9]+)*):geo(:([a-z0-9]+([.-][a-z0-9]+)*))(:[0-9]+):((\\*)|([-a-z]+[/][*-._\\w]+))$",
             "type": "string"
         },
         "GeofenceGeometry": {
@@ -4160,14 +4189,18 @@
                     "documentation": "<p>The timestamp for when the geofence collection was created in <a href=\"https://www.iso.org/iso-8601-date-and-time-format.html\">ISO 8601</a> format: <code>YYYY-MM-DDThh:mm:ss.sssZ</code> </p>",
                     "shape": "Timestamp"
                 },
                 "GeofenceId": {
                     "documentation": "<p>The geofence identifier.</p>",
                     "shape": "Id"
                 },
+                "GeofenceProperties": {
+                    "documentation": "<p>Contains additional user-defined properties stored with the geofence. An array of key-value pairs.</p>",
+                    "shape": "PropertyMap"
+                },
                 "Geometry": {
                     "documentation": "<p>Contains the geofence geometry details describing a polygon or a circle.</p>",
                     "shape": "GeofenceGeometry"
                 },
                 "Status": {
                     "documentation": "<p>Identifies the state of the geofence. A geofence will hold one of the following states:</p> <ul> <li> <p> <code>ACTIVE</code> \u2014 The geofence has been indexed by the system. </p> </li> <li> <p> <code>PENDING</code> \u2014 The geofence is being processed by the system.</p> </li> <li> <p> <code>FAILED</code> \u2014 The geofence failed to be indexed by the system.</p> </li> <li> <p> <code>DELETED</code> \u2014 The geofence has been deleted from the system index.</p> </li> <li> <p> <code>DELETING</code> \u2014 The geofence is being deleted from the system index.</p> </li> </ul>",
                     "shape": "String"
@@ -4185,15 +4218,15 @@
                 "UpdateTime"
             ],
             "type": "structure"
         },
         "GetMapGlyphsRequest": {
             "members": {
                 "FontStack": {
-                    "documentation": "<p>A comma-separated list of fonts to load glyphs from in order of preference. For example, <code>Noto Sans Regular, Arial Unicode</code>.</p> <p>Valid fonts stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/esri.html\">Esri</a> styles: </p> <ul> <li> <p>VectorEsriDarkGrayCanvas \u2013 <code>Ubuntu Medium Italic</code> | <code>Ubuntu Medium</code> | <code>Ubuntu Italic</code> | <code>Ubuntu Regular</code> | <code>Ubuntu Bold</code> </p> </li> <li> <p>VectorEsriLightGrayCanvas \u2013 <code>Ubuntu Italic</code> | <code>Ubuntu Regular</code> | <code>Ubuntu Light</code> | <code>Ubuntu Bold</code> </p> </li> <li> <p>VectorEsriTopographic \u2013 <code>Noto Sans Italic</code> | <code>Noto Sans Regular</code> | <code>Noto Sans Bold</code> | <code>Noto Serif Regular</code> | <code>Roboto Condensed Light Italic</code> </p> </li> <li> <p>VectorEsriStreets \u2013 <code>Arial Regular</code> | <code>Arial Italic</code> | <code>Arial Bold</code> </p> </li> <li> <p>VectorEsriNavigation \u2013 <code>Arial Regular</code> | <code>Arial Italic</code> | <code>Arial Bold</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/HERE.html\">HERE Technologies</a> styles:</p> <ul> <li> <p>VectorHereContrast \u2013 <code>Fira GO Regular</code> | <code>Fira GO Bold</code> </p> </li> <li> <p>VectorHereExplore, VectorHereExploreTruck, HybridHereExploreSatellite \u2013 <code>Fira GO Italic</code> | <code>Fira GO Map</code> | <code>Fira GO Map Bold</code> | <code>Noto Sans CJK JP Bold</code> | <code>Noto Sans CJK JP Light</code> | <code>Noto Sans CJK JP Regular</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html\">GrabMaps</a> styles:</p> <ul> <li> <p>VectorGrabStandardLight, VectorGrabStandardDark \u2013 <code>Noto Sans Regular</code> | <code>Noto Sans Medium</code> | <code>Noto Sans Bold</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/open-data.html\">Open Data</a> styles:</p> <ul> <li> <p>VectorOpenDataStandardLight, VectorOpenDataStandardDark, VectorOpenDataVisualizationLight, VectorOpenDataVisualizationDark \u2013 <code>Amazon Ember Regular,Noto Sans Regular</code> | <code>Amazon Ember Bold,Noto Sans Bold</code> | <code>Amazon Ember Medium,Noto Sans Medium</code> | <code>Amazon Ember Regular Italic,Noto Sans Italic</code> | <code>Amazon Ember Condensed RC Regular,Noto Sans Regular</code> | <code>Amazon Ember Condensed RC Bold,Noto Sans Bold</code> </p> </li> </ul> <note> <p>The fonts used by the Open Data map styles are combined fonts that use <code>Amazon Ember</code> for most glyphs but <code>Noto Sans</code> for glyphs unsupported by <code>Amazon Ember</code>.</p> </note>",
+                    "documentation": "<p>A comma-separated list of fonts to load glyphs from in order of preference. For example, <code>Noto Sans Regular, Arial Unicode</code>.</p> <p>Valid fonts stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/esri.html\">Esri</a> styles: </p> <ul> <li> <p>VectorEsriDarkGrayCanvas \u2013 <code>Ubuntu Medium Italic</code> | <code>Ubuntu Medium</code> | <code>Ubuntu Italic</code> | <code>Ubuntu Regular</code> | <code>Ubuntu Bold</code> </p> </li> <li> <p>VectorEsriLightGrayCanvas \u2013 <code>Ubuntu Italic</code> | <code>Ubuntu Regular</code> | <code>Ubuntu Light</code> | <code>Ubuntu Bold</code> </p> </li> <li> <p>VectorEsriTopographic \u2013 <code>Noto Sans Italic</code> | <code>Noto Sans Regular</code> | <code>Noto Sans Bold</code> | <code>Noto Serif Regular</code> | <code>Roboto Condensed Light Italic</code> </p> </li> <li> <p>VectorEsriStreets \u2013 <code>Arial Regular</code> | <code>Arial Italic</code> | <code>Arial Bold</code> </p> </li> <li> <p>VectorEsriNavigation \u2013 <code>Arial Regular</code> | <code>Arial Italic</code> | <code>Arial Bold</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/HERE.html\">HERE Technologies</a> styles:</p> <ul> <li> <p>VectorHereContrast \u2013 <code>Fira GO Regular</code> | <code>Fira GO Bold</code> </p> </li> <li> <p>VectorHereExplore, VectorHereExploreTruck, HybridHereExploreSatellite \u2013 <code>Fira GO Italic</code> | <code>Fira GO Map</code> | <code>Fira GO Map Bold</code> | <code>Noto Sans CJK JP Bold</code> | <code>Noto Sans CJK JP Light</code> | <code>Noto Sans CJK JP Regular</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html\">GrabMaps</a> styles:</p> <ul> <li> <p>VectorGrabStandardLight, VectorGrabStandardDark \u2013 <code>Noto Sans Regular</code> | <code>Noto Sans Medium</code> | <code>Noto Sans Bold</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/open-data.html\">Open Data</a> styles:</p> <ul> <li> <p>VectorOpenDataStandardLight, VectorOpenDataStandardDark, VectorOpenDataVisualizationLight, VectorOpenDataVisualizationDark \u2013 <code>Amazon Ember Regular,Noto Sans Regular</code> | <code>Amazon Ember Bold,Noto Sans Bold</code> | <code>Amazon Ember Medium,Noto Sans Medium</code> | <code>Amazon Ember Regular Italic,Noto Sans Italic</code> | <code>Amazon Ember Condensed RC Regular,Noto Sans Regular</code> | <code>Amazon Ember Condensed RC Bold,Noto Sans Bold</code> | <code>Amazon Ember Regular,Noto Sans Regular,Noto Sans Arabic Regular</code> | <code>Amazon Ember Condensed RC Bold,Noto Sans Bold,Noto Sans Arabic Condensed Bold</code> | <code>Amazon Ember Bold,Noto Sans Bold,Noto Sans Arabic Bold</code> | <code>Amazon Ember Regular Italic,Noto Sans Italic,Noto Sans Arabic Regular</code> | <code>Amazon Ember Condensed RC Regular,Noto Sans Regular,Noto Sans Arabic Condensed Regular</code> | <code>Amazon Ember Medium,Noto Sans Medium,Noto Sans Arabic Medium</code> </p> </li> </ul> <note> <p>The fonts used by the Open Data map styles are combined fonts that use <code>Amazon Ember</code> for most glyphs but <code>Noto Sans</code> for glyphs unsupported by <code>Amazon Ember</code>.</p> </note>",
                     "location": "uri",
                     "locationName": "FontStack",
                     "shape": "String"
                 },
                 "FontUnicodeRange": {
                     "documentation": "<p>A Unicode range of characters to download glyphs for. Each response will contain 256 characters. For example, 0\u2013255 includes all characters from range <code>U+0000</code> to <code>00FF</code>. Must be aligned to multiples of 256.</p>",
                     "location": "uri",
@@ -4756,14 +4789,18 @@
                     "documentation": "<p>The timestamp for when the geofence was stored in a geofence collection in <a href=\"https://www.iso.org/iso-8601-date-and-time-format.html\">ISO 8601</a> format: <code>YYYY-MM-DDThh:mm:ss.sssZ</code> </p>",
                     "shape": "Timestamp"
                 },
                 "GeofenceId": {
                     "documentation": "<p>The geofence identifier.</p>",
                     "shape": "Id"
                 },
+                "GeofenceProperties": {
+                    "documentation": "<p>Contains additional user-defined properties stored with the geofence. An array of key-value pairs.</p>",
+                    "shape": "PropertyMap"
+                },
                 "Geometry": {
                     "documentation": "<p>Contains the geofence geometry details describing a polygon or a circle.</p>",
                     "shape": "GeofenceGeometry"
                 },
                 "Status": {
                     "documentation": "<p>Identifies the state of the geofence. A geofence will hold one of the following states:</p> <ul> <li> <p> <code>ACTIVE</code> \u2014 The geofence has been indexed by the system. </p> </li> <li> <p> <code>PENDING</code> \u2014 The geofence is being processed by the system.</p> </li> <li> <p> <code>FAILED</code> \u2014 The geofence failed to be indexed by the system.</p> </li> <li> <p> <code>DELETED</code> \u2014 The geofence has been deleted from the system index.</p> </li> <li> <p> <code>DELETING</code> \u2014 The geofence is being deleted from the system index.</p> </li> </ul>",
                     "shape": "String"
@@ -5300,37 +5337,55 @@
                 "shape": "ListTrackersResponseEntry"
             },
             "type": "list"
         },
         "MapConfiguration": {
             "documentation": "<p>Specifies the map tile style selected from an available provider.</p>",
             "members": {
+                "PoliticalView": {
+                    "documentation": "<p>Specifies the political view for the style. Leave unset to not use a political view, or, for styles that support specific political views, you can choose a view, such as <code>IND</code> for the Indian view.</p> <p>Default is unset.</p> <note> <p>Not all map resources or styles support political view styles. See <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/map-concepts.html#political-views\">Political views</a> for more information.</p> </note>",
+                    "shape": "CountryCode3"
+                },
                 "Style": {
-                    "documentation": "<p>Specifies the map style selected from an available data provider.</p> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/esri.html\">Esri map styles</a>:</p> <ul> <li> <p> <code>VectorEsriDarkGrayCanvas</code> \u2013 The Esri Dark Gray Canvas map style. A vector basemap with a dark gray, neutral background with minimal colors, labels, and features that's designed to draw attention to your thematic content. </p> </li> <li> <p> <code>RasterEsriImagery</code> \u2013 The Esri Imagery map style. A raster basemap that provides one meter or better satellite and aerial imagery in many parts of the world and lower resolution satellite imagery worldwide. </p> </li> <li> <p> <code>VectorEsriLightGrayCanvas</code> \u2013 The Esri Light Gray Canvas map style, which provides a detailed vector basemap with a light gray, neutral background style with minimal colors, labels, and features that's designed to draw attention to your thematic content. </p> </li> <li> <p> <code>VectorEsriTopographic</code> \u2013 The Esri Light map style, which provides a detailed vector basemap with a classic Esri map style.</p> </li> <li> <p> <code>VectorEsriStreets</code> \u2013 The Esri World Streets map style, which provides a detailed vector basemap for the world symbolized with a classic Esri street map style. The vector tile layer is similar in content and style to the World Street Map raster map.</p> </li> <li> <p> <code>VectorEsriNavigation</code> \u2013 The Esri World Navigation map style, which provides a detailed basemap for the world symbolized with a custom navigation map style that's designed for use during the day in mobile devices.</p> </li> </ul> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/HERE.html\">HERE Technologies map styles</a>:</p> <ul> <li> <p> <code>VectorHereContrast</code> \u2013 The HERE Contrast (Berlin) map style is a high contrast detailed base map of the world that blends 3D and 2D rendering.</p> <note> <p>The <code>VectorHereContrast</code> style has been renamed from <code>VectorHereBerlin</code>. <code>VectorHereBerlin</code> has been deprecated, but will continue to work in applications that use it.</p> </note> </li> <li> <p> <code>VectorHereExplore</code> \u2013 A default HERE map style containing a neutral, global map and its features including roads, buildings, landmarks, and water features. It also now includes a fully designed map of Japan.</p> </li> <li> <p> <code>VectorHereExploreTruck</code> \u2013 A global map containing truck restrictions and attributes (e.g. width / height / HAZMAT) symbolized with highlighted segments and icons on top of HERE Explore to support use cases within transport and logistics.</p> </li> <li> <p> <code>RasterHereExploreSatellite</code> \u2013 A global map containing high resolution satellite imagery.</p> </li> <li> <p> <code>HybridHereExploreSatellite</code> \u2013 A global map displaying the road network, street names, and city labels over satellite imagery. This style will automatically retrieve both raster and vector tiles, and your charges will be based on total tiles retrieved.</p> <note> <p>Hybrid styles use both vector and raster tiles when rendering the map that you see. This means that more tiles are retrieved than when using either vector or raster tiles alone. Your charges will include all tiles retrieved.</p> </note> </li> </ul> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html\">GrabMaps map styles</a>:</p> <ul> <li> <p> <code>VectorGrabStandardLight</code> \u2013 The Grab Standard Light map style provides a basemap with detailed land use coloring, area names, roads, landmarks, and points of interest covering Southeast Asia.</p> </li> <li> <p> <code>VectorGrabStandardDark</code> \u2013 The Grab Standard Dark map style provides a dark variation of the standard basemap covering Southeast Asia.</p> </li> </ul> <note> <p>Grab provides maps only for countries in Southeast Asia, and is only available in the Asia Pacific (Singapore) Region (<code>ap-southeast-1</code>). For more information, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html#grab-coverage-area\">GrabMaps countries and area covered</a>.</p> </note> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/open-data.html\">Open Data map styles</a>:</p> <ul> <li> <p> <code>VectorOpenDataStandardLight</code> \u2013 The Open Data Standard Light map style provides a detailed basemap for the world suitable for website and mobile application use. The map includes highways major roads, minor roads, railways, water features, cities, parks, landmarks, building footprints, and administrative boundaries.</p> </li> <li> <p> <code>VectorOpenDataStandardDark</code> \u2013 Open Data Standard Dark is a dark-themed map style that provides a detailed basemap for the world suitable for website and mobile application use. The map includes highways major roads, minor roads, railways, water features, cities, parks, landmarks, building footprints, and administrative boundaries.</p> </li> <li> <p> <code>VectorOpenDataVisualizationLight</code> \u2013 The Open Data Visualization Light map style is a light-themed style with muted colors and fewer features that aids in understanding overlaid data.</p> </li> <li> <p> <code>VectorOpenDataVisualizationDark</code> \u2013 The Open Data Visualization Dark map style is a dark-themed style with muted colors and fewer features that aids in understanding overlaid data.</p> </li> </ul>",
+                    "documentation": "<p>Specifies the map style selected from an available data provider.</p> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/esri.html\">Esri map styles</a>:</p> <ul> <li> <p> <code>VectorEsriDarkGrayCanvas</code> \u2013 The Esri Dark Gray Canvas map style. A vector basemap with a dark gray, neutral background with minimal colors, labels, and features that's designed to draw attention to your thematic content. </p> </li> <li> <p> <code>RasterEsriImagery</code> \u2013 The Esri Imagery map style. A raster basemap that provides one meter or better satellite and aerial imagery in many parts of the world and lower resolution satellite imagery worldwide. </p> </li> <li> <p> <code>VectorEsriLightGrayCanvas</code> \u2013 The Esri Light Gray Canvas map style, which provides a detailed vector basemap with a light gray, neutral background style with minimal colors, labels, and features that's designed to draw attention to your thematic content. </p> </li> <li> <p> <code>VectorEsriTopographic</code> \u2013 The Esri Light map style, which provides a detailed vector basemap with a classic Esri map style.</p> </li> <li> <p> <code>VectorEsriStreets</code> \u2013 The Esri Street Map style, which provides a detailed vector basemap for the world symbolized with a classic Esri street map style. The vector tile layer is similar in content and style to the World Street Map raster map.</p> </li> <li> <p> <code>VectorEsriNavigation</code> \u2013 The Esri Navigation map style, which provides a detailed basemap for the world symbolized with a custom navigation map style that's designed for use during the day in mobile devices.</p> </li> </ul> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/HERE.html\">HERE Technologies map styles</a>:</p> <ul> <li> <p> <code>VectorHereContrast</code> \u2013 The HERE Contrast (Berlin) map style is a high contrast detailed base map of the world that blends 3D and 2D rendering.</p> <note> <p>The <code>VectorHereContrast</code> style has been renamed from <code>VectorHereBerlin</code>. <code>VectorHereBerlin</code> has been deprecated, but will continue to work in applications that use it.</p> </note> </li> <li> <p> <code>VectorHereExplore</code> \u2013 A default HERE map style containing a neutral, global map and its features including roads, buildings, landmarks, and water features. It also now includes a fully designed map of Japan.</p> </li> <li> <p> <code>VectorHereExploreTruck</code> \u2013 A global map containing truck restrictions and attributes (e.g. width / height / HAZMAT) symbolized with highlighted segments and icons on top of HERE Explore to support use cases within transport and logistics.</p> </li> <li> <p> <code>RasterHereExploreSatellite</code> \u2013 A global map containing high resolution satellite imagery.</p> </li> <li> <p> <code>HybridHereExploreSatellite</code> \u2013 A global map displaying the road network, street names, and city labels over satellite imagery. This style will automatically retrieve both raster and vector tiles, and your charges will be based on total tiles retrieved.</p> <note> <p>Hybrid styles use both vector and raster tiles when rendering the map that you see. This means that more tiles are retrieved than when using either vector or raster tiles alone. Your charges will include all tiles retrieved.</p> </note> </li> </ul> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html\">GrabMaps map styles</a>:</p> <ul> <li> <p> <code>VectorGrabStandardLight</code> \u2013 The Grab Standard Light map style provides a basemap with detailed land use coloring, area names, roads, landmarks, and points of interest covering Southeast Asia.</p> </li> <li> <p> <code>VectorGrabStandardDark</code> \u2013 The Grab Standard Dark map style provides a dark variation of the standard basemap covering Southeast Asia.</p> </li> </ul> <note> <p>Grab provides maps only for countries in Southeast Asia, and is only available in the Asia Pacific (Singapore) Region (<code>ap-southeast-1</code>). For more information, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html#grab-coverage-area\">GrabMaps countries and area covered</a>.</p> </note> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/open-data.html\">Open Data map styles</a>:</p> <ul> <li> <p> <code>VectorOpenDataStandardLight</code> \u2013 The Open Data Standard Light map style provides a detailed basemap for the world suitable for website and mobile application use. The map includes highways major roads, minor roads, railways, water features, cities, parks, landmarks, building footprints, and administrative boundaries.</p> </li> <li> <p> <code>VectorOpenDataStandardDark</code> \u2013 Open Data Standard Dark is a dark-themed map style that provides a detailed basemap for the world suitable for website and mobile application use. The map includes highways major roads, minor roads, railways, water features, cities, parks, landmarks, building footprints, and administrative boundaries.</p> </li> <li> <p> <code>VectorOpenDataVisualizationLight</code> \u2013 The Open Data Visualization Light map style is a light-themed style with muted colors and fewer features that aids in understanding overlaid data.</p> </li> <li> <p> <code>VectorOpenDataVisualizationDark</code> \u2013 The Open Data Visualization Dark map style is a dark-themed style with muted colors and fewer features that aids in understanding overlaid data.</p> </li> </ul>",
                     "shape": "MapStyle"
                 }
             },
             "required": [
                 "Style"
             ],
             "type": "structure"
         },
+        "MapConfigurationUpdate": {
+            "documentation": "<p>Specifies the political view for the style.</p>",
+            "members": {
+                "PoliticalView": {
+                    "documentation": "<p>Specifies the political view for the style. Set to an empty string to not use a political view, or, for styles that support specific political views, you can choose a view, such as <code>IND</code> for the Indian view.</p> <note> <p>Not all map resources or styles support political view styles. See <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/map-concepts.html#political-views\">Political views</a> for more information.</p> </note>",
+                    "shape": "CountryCode3OrEmpty"
+                }
+            },
+            "type": "structure"
+        },
         "MapStyle": {
             "max": 100,
             "min": 1,
             "pattern": "^[-._\\w]+$",
             "type": "string"
         },
         "Place": {
             "documentation": "<p>Contains details about addresses or points of interest that match the search criteria.</p> <p>Not all details are included with all responses. Some details may only be returned by specific data partners.</p>",
             "members": {
                 "AddressNumber": {
                     "documentation": "<p>The numerical portion of an address, such as a building number. </p>",
                     "shape": "String"
                 },
+                "Categories": {
+                    "documentation": "<p>The Amazon Location categories that describe this Place.</p> <p>For more information about using categories, including a list of Amazon Location categories, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/category-filtering.html\">Categories and filtering</a>, in the <i>Amazon Location Service Developer Guide</i>.</p>",
+                    "shape": "PlaceCategoryList"
+                },
                 "Country": {
                     "documentation": "<p>A country/region specified using <a href=\"https://www.iso.org/iso-3166-country-codes.html\">ISO 3166</a> 3-digit country/region code. For example, <code>CAN</code>.</p>",
                     "shape": "String"
                 },
                 "Geometry": {
                     "shape": "PlaceGeometry"
                 },
@@ -5362,32 +5417,49 @@
                     "documentation": "<p>The name for a street or a road to identify a location. For example, <code>Main Street</code>.</p>",
                     "shape": "String"
                 },
                 "SubRegion": {
                     "documentation": "<p>A county, or an area that's part of a larger region. For example, <code>Metro Vancouver</code>.</p>",
                     "shape": "String"
                 },
+                "SupplementalCategories": {
+                    "documentation": "<p>Categories from the data provider that describe the Place that are not mapped to any Amazon Location categories.</p>",
+                    "shape": "PlaceSupplementalCategoryList"
+                },
                 "TimeZone": {
-                    "documentation": "<p>The time zone in which the <code>Place</code> is located. Returned only when using HERE as the selected partner.</p>",
+                    "documentation": "<p>The time zone in which the <code>Place</code> is located. Returned only when using HERE or Grab as the selected partner.</p>",
                     "shape": "TimeZone"
                 },
                 "UnitNumber": {
-                    "documentation": "<p>For addresses with multiple units, the unit identifier. Can include numbers and letters, for example <code>3B</code> or <code>Unit 123</code>.</p> <note> <p>Returned only for a place index that uses Esri as a data provider. Is not returned for <code>SearchPlaceIndexForPosition</code>.</p> </note>",
+                    "documentation": "<p>For addresses with multiple units, the unit identifier. Can include numbers and letters, for example <code>3B</code> or <code>Unit 123</code>.</p> <note> <p>Returned only for a place index that uses Esri or Grab as a data provider. Is not returned for <code>SearchPlaceIndexForPosition</code>.</p> </note>",
                     "shape": "String"
                 },
                 "UnitType": {
-                    "documentation": "<p>For addresses with a <code>UnitNumber</code>, the type of unit. For example, <code>Apartment</code>.</p>",
+                    "documentation": "<p>For addresses with a <code>UnitNumber</code>, the type of unit. For example, <code>Apartment</code>.</p> <note> <p>Returned only for a place index that uses Esri as a data provider.</p> </note>",
                     "shape": "String"
                 }
             },
             "required": [
                 "Geometry"
             ],
             "type": "structure"
         },
+        "PlaceCategory": {
+            "max": 35,
+            "min": 0,
+            "type": "string"
+        },
+        "PlaceCategoryList": {
+            "max": 10,
+            "member": {
+                "shape": "PlaceCategory"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "PlaceGeometry": {
             "documentation": "<p>Places uses a point geometry to specify a location or a Place.</p>",
             "members": {
                 "Point": {
                     "documentation": "<p>A single point geometry specifies a location for a Place using <a href=\"https://gisgeography.com/wgs84-world-geodetic-system/\">WGS 84</a> coordinates:</p> <ul> <li> <p> <i>x</i> \u2014 Specifies the x coordinate or longitude. </p> </li> <li> <p> <i>y</i> \u2014 Specifies the y coordinate or latitude. </p> </li> </ul>",
                     "shape": "Position"
                 }
@@ -5398,14 +5470,27 @@
             "type": "string"
         },
         "PlaceIndexSearchResultLimit": {
             "max": 50,
             "min": 1,
             "type": "integer"
         },
+        "PlaceSupplementalCategory": {
+            "max": 35,
+            "min": 0,
+            "type": "string"
+        },
+        "PlaceSupplementalCategoryList": {
+            "max": 10,
+            "member": {
+                "shape": "PlaceSupplementalCategory"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "Position": {
             "max": 2,
             "member": {
                 "shape": "Double"
             },
             "min": 2,
             "sensitive": true,
@@ -5478,14 +5563,18 @@
                 },
                 "GeofenceId": {
                     "documentation": "<p>An identifier for the geofence. For example, <code>ExampleGeofence-1</code>.</p>",
                     "location": "uri",
                     "locationName": "GeofenceId",
                     "shape": "Id"
                 },
+                "GeofenceProperties": {
+                    "documentation": "<p>Specifies additional user-defined properties to store with the Geofence. An array of key-value pairs.</p>",
+                    "shape": "PropertyMap"
+                },
                 "Geometry": {
                     "documentation": "<p>Contains the details to specify the position of the geofence. Can be either a polygon or a circle. Including both will return a validation error.</p> <note> <p>Each <a href=\"https://docs.aws.amazon.com/location-geofences/latest/APIReference/API_GeofenceGeometry.html\"> geofence polygon</a> can have a maximum of 1,000 vertices.</p> </note>",
                     "shape": "GeofenceGeometry"
                 }
             },
             "required": [
                 "CollectionName",
@@ -5651,18 +5740,26 @@
                 "shape": "SearchForPositionResult"
             },
             "type": "list"
         },
         "SearchForSuggestionsResult": {
             "documentation": "<p>Contains a place suggestion resulting from a place suggestion query that is run on a place index resource.</p>",
             "members": {
+                "Categories": {
+                    "documentation": "<p>The Amazon Location categories that describe the Place.</p> <p>For more information about using categories, including a list of Amazon Location categories, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/category-filtering.html\">Categories and filtering</a>, in the <i>Amazon Location Service Developer Guide</i>.</p>",
+                    "shape": "PlaceCategoryList"
+                },
                 "PlaceId": {
-                    "documentation": "<p>The unique identifier of the place. You can use this with the <code>GetPlace</code> operation to find the place again later.</p> <note> <p>For <code>SearchPlaceIndexForSuggestions</code> operations, the <code>PlaceId</code> is returned by place indexes that use Esri, Grab, or HERE as data providers.</p> </note>",
+                    "documentation": "<p>The unique identifier of the Place. You can use this with the <code>GetPlace</code> operation to find the place again later, or to get full information for the Place.</p> <p>The <code>GetPlace</code> request must use the same <code>PlaceIndex</code> resource as the <code>SearchPlaceIndexForSuggestions</code> that generated the Place ID.</p> <note> <p>For <code>SearchPlaceIndexForSuggestions</code> operations, the <code>PlaceId</code> is returned by place indexes that use Esri, Grab, or HERE as data providers.</p> </note>",
                     "shape": "PlaceId"
                 },
+                "SupplementalCategories": {
+                    "documentation": "<p>Categories from the data provider that describe the Place that are not mapped to any Amazon Location categories.</p>",
+                    "shape": "PlaceSupplementalCategoryList"
+                },
                 "Text": {
                     "documentation": "<p>The text of the place suggestion, typically formatted as an address string.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "Text"
@@ -5793,14 +5890,18 @@
                     "documentation": "<p>An optional parameter that indicates a preference for place suggestions that are closer to a specified position.</p> <p> If provided, this parameter must contain a pair of numbers. The first number represents the X coordinate, or longitude; the second number represents the Y coordinate, or latitude.</p> <p>For example, <code>[-123.1174, 49.2847]</code> represents the position with longitude <code>-123.1174</code> and latitude <code>49.2847</code>.</p> <note> <p> <code>BiasPosition</code> and <code>FilterBBox</code> are mutually exclusive. Specifying both options results in an error. </p> </note>",
                     "shape": "Position"
                 },
                 "FilterBBox": {
                     "documentation": "<p>An optional parameter that limits the search results by returning only suggestions within a specified bounding box.</p> <p> If provided, this parameter must contain a total of four consecutive numbers in two pairs. The first pair of numbers represents the X and Y coordinates (longitude and latitude, respectively) of the southwest corner of the bounding box; the second pair of numbers represents the X and Y coordinates (longitude and latitude, respectively) of the northeast corner of the bounding box.</p> <p>For example, <code>[-12.7935, -37.4835, -12.0684, -36.9542]</code> represents a bounding box where the southwest corner has longitude <code>-12.7935</code> and latitude <code>-37.4835</code>, and the northeast corner has longitude <code>-12.0684</code> and latitude <code>-36.9542</code>.</p> <note> <p> <code>FilterBBox</code> and <code>BiasPosition</code> are mutually exclusive. Specifying both options results in an error. </p> </note>",
                     "shape": "BoundingBox"
                 },
+                "FilterCategories": {
+                    "documentation": "<p>A list of one or more Amazon Location categories to filter the returned places. If you include more than one category, the results will include results that match <i>any</i> of the categories listed.</p> <p>For more information about using categories, including a list of Amazon Location categories, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/category-filtering.html\">Categories and filtering</a>, in the <i>Amazon Location Service Developer Guide</i>.</p>",
+                    "shape": "FilterPlaceCategoryList"
+                },
                 "FilterCountries": {
                     "documentation": "<p>An optional parameter that limits the search results by returning only suggestions within the provided list of countries.</p> <ul> <li> <p>Use the <a href=\"https://www.iso.org/iso-3166-country-codes.html\">ISO 3166</a> 3-digit country code. For example, Australia uses three upper-case characters: <code>AUS</code>.</p> </li> </ul>",
                     "shape": "CountryCodeList"
                 },
                 "IndexName": {
                     "documentation": "<p>The name of the place index resource you want to use for the search.</p>",
                     "location": "uri",
@@ -5866,14 +5967,18 @@
                     "documentation": "<p>The geospatial data provider attached to the place index resource specified in the request. Values can be one of the following:</p> <ul> <li> <p>Esri</p> </li> <li> <p>Grab</p> </li> <li> <p>Here</p> </li> </ul> <p>For more information about data providers, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/what-is-data-provider.html\">Amazon Location Service data providers</a>.</p>",
                     "shape": "String"
                 },
                 "FilterBBox": {
                     "documentation": "<p>Contains the coordinates for the optional bounding box specified in the request.</p>",
                     "shape": "BoundingBox"
                 },
+                "FilterCategories": {
+                    "documentation": "<p>The optional category filter specified in the request.</p>",
+                    "shape": "FilterPlaceCategoryList"
+                },
                 "FilterCountries": {
                     "documentation": "<p>Contains the optional country filter specified in the request.</p>",
                     "shape": "CountryCodeList"
                 },
                 "Language": {
                     "documentation": "<p>The preferred language used to return results. Matches the language in the request. The value is a valid <a href=\"https://tools.ietf.org/search/bcp47\">BCP 47</a> language tag, for example, <code>en</code> for English.</p>",
                     "shape": "LanguageTag"
@@ -5899,14 +6004,18 @@
                     "documentation": "<p>An optional parameter that indicates a preference for places that are closer to a specified position.</p> <p> If provided, this parameter must contain a pair of numbers. The first number represents the X coordinate, or longitude; the second number represents the Y coordinate, or latitude.</p> <p>For example, <code>[-123.1174, 49.2847]</code> represents the position with longitude <code>-123.1174</code> and latitude <code>49.2847</code>.</p> <note> <p> <code>BiasPosition</code> and <code>FilterBBox</code> are mutually exclusive. Specifying both options results in an error. </p> </note>",
                     "shape": "Position"
                 },
                 "FilterBBox": {
                     "documentation": "<p>An optional parameter that limits the search results by returning only places that are within the provided bounding box.</p> <p> If provided, this parameter must contain a total of four consecutive numbers in two pairs. The first pair of numbers represents the X and Y coordinates (longitude and latitude, respectively) of the southwest corner of the bounding box; the second pair of numbers represents the X and Y coordinates (longitude and latitude, respectively) of the northeast corner of the bounding box.</p> <p>For example, <code>[-12.7935, -37.4835, -12.0684, -36.9542]</code> represents a bounding box where the southwest corner has longitude <code>-12.7935</code> and latitude <code>-37.4835</code>, and the northeast corner has longitude <code>-12.0684</code> and latitude <code>-36.9542</code>.</p> <note> <p> <code>FilterBBox</code> and <code>BiasPosition</code> are mutually exclusive. Specifying both options results in an error. </p> </note>",
                     "shape": "BoundingBox"
                 },
+                "FilterCategories": {
+                    "documentation": "<p>A list of one or more Amazon Location categories to filter the returned places. If you include more than one category, the results will include results that match <i>any</i> of the categories listed.</p> <p>For more information about using categories, including a list of Amazon Location categories, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/category-filtering.html\">Categories and filtering</a>, in the <i>Amazon Location Service Developer Guide</i>.</p>",
+                    "shape": "FilterPlaceCategoryList"
+                },
                 "FilterCountries": {
                     "documentation": "<p>An optional parameter that limits the search results by returning only places that are in a specified list of countries.</p> <ul> <li> <p>Valid values include <a href=\"https://www.iso.org/iso-3166-country-codes.html\">ISO 3166</a> 3-digit country codes. For example, Australia uses three upper-case characters: <code>AUS</code>.</p> </li> </ul>",
                     "shape": "CountryCodeList"
                 },
                 "IndexName": {
                     "documentation": "<p>The name of the place index resource you want to use for the search.</p>",
                     "location": "uri",
@@ -5966,14 +6075,18 @@
                     "documentation": "<p>The geospatial data provider attached to the place index resource specified in the request. Values can be one of the following:</p> <ul> <li> <p>Esri</p> </li> <li> <p>Grab</p> </li> <li> <p>Here</p> </li> </ul> <p>For more information about data providers, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/what-is-data-provider.html\">Amazon Location Service data providers</a>.</p>",
                     "shape": "String"
                 },
                 "FilterBBox": {
                     "documentation": "<p>Contains the coordinates for the optional bounding box specified in the request.</p>",
                     "shape": "BoundingBox"
                 },
+                "FilterCategories": {
+                    "documentation": "<p>The optional category filter specified in the request.</p>",
+                    "shape": "FilterPlaceCategoryList"
+                },
                 "FilterCountries": {
                     "documentation": "<p>Contains the optional country filter specified in the request.</p>",
                     "shape": "CountryCodeList"
                 },
                 "Language": {
                     "documentation": "<p>The preferred language used to return results. Matches the language in the request. The value is a valid <a href=\"https://tools.ietf.org/search/bcp47\">BCP 47</a> language tag, for example, <code>en</code> for English.</p>",
                     "shape": "LanguageTag"
@@ -6381,14 +6494,18 @@
                 "KeyName",
                 "UpdateTime"
             ],
             "type": "structure"
         },
         "UpdateMapRequest": {
             "members": {
+                "ConfigurationUpdate": {
+                    "documentation": "<p>Updates the parts of the map configuration that can be updated, including the political view.</p>",
+                    "shape": "MapConfigurationUpdate"
+                },
                 "Description": {
                     "documentation": "<p>Updates the description for the map resource.</p>",
                     "shape": "ResourceDescription"
                 },
                 "MapName": {
                     "documentation": "<p>The name of the map resource to update.</p>",
                     "location": "uri",
@@ -6457,15 +6574,15 @@
             ],
             "type": "structure"
         },
         "UpdatePlaceIndexResponse": {
             "members": {
                 "IndexArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the upated place index resource. Used to specify a resource across Amazon Web Services.</p> <ul> <li> <p>Format example: <code>arn:aws:geo:region:account-id:place- index/ExamplePlaceIndex</code> </p> </li> </ul>",
-                    "shape": "Arn"
+                    "shape": "GeoArn"
                 },
                 "IndexName": {
                     "documentation": "<p>The name of the updated place index resource.</p>",
                     "shape": "ResourceName"
                 },
                 "UpdateTime": {
                     "documentation": "<p>The timestamp for when the place index resource was last updated in <a href=\"https://www.iso.org/iso-8601-date-and-time-format.html\"> ISO 8601</a> format: <code>YYYY-MM-DDThh:mm:ss.sssZ</code>. </p>",
@@ -6503,15 +6620,15 @@
             ],
             "type": "structure"
         },
         "UpdateRouteCalculatorResponse": {
             "members": {
                 "CalculatorArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the updated route calculator resource. Used to specify a resource across AWS.</p> <ul> <li> <p>Format example: <code>arn:aws:geo:region:account-id:route- calculator/ExampleCalculator</code> </p> </li> </ul>",
-                    "shape": "Arn"
+                    "shape": "GeoArn"
                 },
                 "CalculatorName": {
                     "documentation": "<p>The name of the updated route calculator resource.</p>",
                     "shape": "ResourceName"
                 },
                 "UpdateTime": {
                     "documentation": "<p>The timestamp for when the route calculator was last updated in <a href=\"https://www.iso.org/iso-8601-date-and-time-format.html\"> ISO 8601</a> format: <code>YYYY-MM-DDThh:mm:ss.sssZ</code>. </p>",
```

### Comparing `botocore-a-la-carte-location-1.29.99/botocore_a_la_carte_location.egg-info/PKG-INFO` & `botocore-a-la-carte-location-1.30.0/botocore_a_la_carte_location.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-location
-Version: 1.29.99
+Version: 1.30.0
 Summary: location data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-location-1.29.99/setup.py` & `botocore-a-la-carte-location-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-location',
-    version="1.29.99",
+    version="1.30.0",
     description='location data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/location/*/*.json'],
```

