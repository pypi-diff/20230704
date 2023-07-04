# Comparing `tmp/simple_dwd_weatherforecast-2.0.8.tar.gz` & `tmp/simple_dwd_weatherforecast-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_dwd_weatherforecast-2.0.8.tar", last modified: Sun Jul  2 15:46:33 2023, max compression
+gzip compressed data, was "simple_dwd_weatherforecast-2.0.9.tar", last modified: Tue Jul  4 16:04:08 2023, max compression
```

## Comparing `simple_dwd_weatherforecast-2.0.8.tar` & `simple_dwd_weatherforecast-2.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:33.526230 simple_dwd_weatherforecast-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-02 15:46:33.526230 simple_dwd_weatherforecast-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:46:33.526230 simple_dwd_weatherforecast-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:33.522230 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30450 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/dwdforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/dwdmap.py
--rw-r--r--   0 runner    (1001) docker     (123)   861420 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/stations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:33.522230 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:33.526230 simple_dwd_weatherforecast-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63395 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)    28680 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_day_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_forecast_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_forecast_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_station_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_is_in_timerange.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_is_valid_timeframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_location_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_parsekml.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_reported_weather.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_station.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_update_hourly.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:04:08.779688 simple_dwd_weatherforecast-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-04 16:04:08.779688 simple_dwd_weatherforecast-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 16:04:08.779688 simple_dwd_weatherforecast-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:04:08.775688 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30473 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast/dwdforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast/dwdmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   861378 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast/stations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:04:08.779688 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-04 16:04:08.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-04 16:04:08.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:04:08.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 16:04:08.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 16:04:08.000000 simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:04:08.779688 simple_dwd_weatherforecast-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63395 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_daily_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_daily_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_daily_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_daily_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28680 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_day_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_forecast_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_forecast_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_station_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_is_in_timerange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_is_valid_timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_location_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_parsekml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_reported_weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_update_hourly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 16:03:59.000000 simple_dwd_weatherforecast-2.0.9/tests/test_weather.py
```

### Comparing `simple_dwd_weatherforecast-2.0.8/LICENCE` & `simple_dwd_weatherforecast-2.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/PKG-INFO` & `simple_dwd_weatherforecast-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_dwd_weatherforecast
-Version: 2.0.8
+Version: 2.0.9
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `simple_dwd_weatherforecast-2.0.8/README.md` & `simple_dwd_weatherforecast-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/setup.py` & `simple_dwd_weatherforecast-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_dwd_weatherforecast",
-    version="2.0.8",
+    version="2.0.9",
     author="Max Fermor",
     description="A simple tool to retrieve a weather forecast from DWD OpenData",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FL550/simple_dwd_weatherforecast.git",
     packages=setuptools.find_packages(),
     package_data={'': ['stations.json']},
```

### Comparing `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/dwdforecast.py` & `simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast/dwdforecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from enum import Enum
 from lxml import etree
 from datetime import datetime, timedelta, timezone
 import time
 import math
 import json
 import csv
-import importlib.resources
+import importlib
 
-with importlib.resources.open_text(
-    "simple_dwd_weatherforecast", "stations.json"
-) as file:
+with importlib.resources.files("simple_dwd_weatherforecast").joinpath(
+    "stations.json"
+).open("r", encoding="utf-8") as file:
     stations = json.load(file)
 
 
 def load_station_id(station_id: str):
     if station_id in stations:
         return stations[station_id]
     return None
```

### Comparing `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/dwdmap.py` & `simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast/dwdmap.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/stations.json` & `simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast/stations.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991427142618995%*

 * *Differences: {"'01180'": "{'name': 'Borken in Westfalen'}",*

 * * "'02586'": "{'name': 'Holzhausen a.d. Haide'}",*

 * * "'02929'": "{'name': 'Neuhausen ob Eck-Unterschwandorf'}",*

 * * "'10007'": "{'name': 'UFS Deutsche Bucht'}",*

 * * "'10020'": "{'name': 'List auf Sylt'}",*

 * * "'10038'": "{'name': 'Kastellaun (PH)'}",*

 * * "'10130'": "{'name': 'Wittlich (PH)'}",*

 * * "'10177'": "{'name': 'Alzey (PH)'}",*

 * * "'10210'": "{'name': 'Speyer, kreisfreie Stadt Speyer'}",*

 * * "'10277'": "{'name': 'Neuglobsow (HM)'}",*

 * * "'10324'": "{'name': 'Adelmannsfelden (PH)'} […]*

```diff
@@ -109,15 +109,15 @@
     },
     "01180": {
         "bundesland": "NW",
         "elev": "47",
         "icao": "----",
         "lat": "51.873",
         "lon": "6.886",
-        "name": "Borken In Westfalen",
+        "name": "Borken in Westfalen",
         "report_available": 1
     },
     "01194": {
         "bundesland": "NW",
         "elev": "76",
         "icao": "----",
         "lat": "51.131",
@@ -703,15 +703,15 @@
     },
     "02586": {
         "bundesland": "RP",
         "elev": "397",
         "icao": "----",
         "lat": "50.218",
         "lon": "7.913",
-        "name": "Holzhausen A.D. Haide",
+        "name": "Holzhausen a.d. Haide",
         "report_available": 0
     },
     "02590": {
         "bundesland": "HE",
         "elev": "263",
         "icao": "ESSV",
         "lat": "50.132",
@@ -1000,15 +1000,15 @@
     },
     "02929": {
         "bundesland": "BW",
         "elev": "663",
         "icao": "EFJO",
         "lat": "47.952",
         "lon": "8.993",
-        "name": "Neuhausen Ob Eck-Unterschwandorf",
+        "name": "Neuhausen ob Eck-Unterschwandorf",
         "report_available": 0
     },
     "02935": {
         "bundesland": "BW",
         "elev": "655",
         "icao": "EFJY",
         "lat": "48.148",
@@ -5194,15 +5194,15 @@
     },
     "10007": {
         "bundesland": "HH",
         "elev": "0",
         "icao": "----",
         "lat": "54.1796",
         "lon": "7.4587",
-        "name": "Ufs Deutsche Bucht",
+        "name": "UFS Deutsche Bucht",
         "report_available": 1
     },
     "10015": {
         "bundesland": "RP",
         "elev": "200",
         "icao": "----",
         "lat": "50.333",
@@ -5221,15 +5221,15 @@
     },
     "10020": {
         "bundesland": "SH",
         "elev": "25",
         "icao": "----",
         "lat": "55.011",
         "lon": "8.4125",
-        "name": "List Auf Sylt",
+        "name": "List auf Sylt",
         "report_available": 1
     },
     "10022": {
         "bundesland": "RP",
         "elev": "120",
         "icao": "EDXK",
         "lat": "50.467",
@@ -5293,15 +5293,15 @@
     },
     "10038": {
         "bundesland": "RP",
         "elev": "400",
         "icao": "ETNH",
         "lat": "50.083",
         "lon": "7.45",
-        "name": "Kastellaun (Ph)",
+        "name": "Kastellaun (PH)",
         "report_available": 1
     },
     "10042": {
         "bundesland": "RP",
         "elev": "140",
         "icao": "----",
         "lat": "50.033",
@@ -5428,15 +5428,15 @@
     },
     "10130": {
         "bundesland": "RP",
         "elev": "160",
         "icao": "----",
         "lat": "49.983",
         "lon": "6.883",
-        "name": "Wittlich (Ph)",
+        "name": "Wittlich (PH)",
         "report_available": 1
     },
     "10131": {
         "bundesland": "RP",
         "elev": "200",
         "icao": "----",
         "lat": "50",
@@ -5572,15 +5572,15 @@
     },
     "10177": {
         "bundesland": "RP",
         "elev": "190",
         "icao": "----",
         "lat": "49.75",
         "lon": "8.117",
-        "name": "Alzey (Ph)",
+        "name": "Alzey (PH)",
         "report_available": 0
     },
     "10180": {
         "bundesland": "RP",
         "elev": "190",
         "icao": "----",
         "lat": "49.8",
@@ -5635,15 +5635,15 @@
     },
     "10210": {
         "bundesland": "RP",
         "elev": "95",
         "icao": "----",
         "lat": "49.317",
         "lon": "8.433",
-        "name": "Speyer, Kreisfreie Stadt Speyer",
+        "name": "Speyer, kreisfreie Stadt Speyer",
         "report_available": 1
     },
     "10215": {
         "bundesland": "RP",
         "elev": "240",
         "icao": "EDWH",
         "lat": "49.167",
@@ -5797,15 +5797,15 @@
     },
     "10277": {
         "bundesland": "BB",
         "elev": "62",
         "icao": "----",
         "lat": "53.1424",
         "lon": "13.0319",
-        "name": "Neuglobsow (Hm)",
+        "name": "Neuglobsow (HM)",
         "report_available": 0
     },
     "10280": {
         "bundesland": "RP",
         "elev": "160",
         "icao": "----",
         "lat": "49.433",
@@ -5950,15 +5950,15 @@
     },
     "10324": {
         "bundesland": "BW",
         "elev": "470",
         "icao": "----",
         "lat": "48.95",
         "lon": "10",
-        "name": "Adelmannsfelden (Ph)",
+        "name": "Adelmannsfelden (PH)",
         "report_available": 0
     },
     "10325": {
         "bundesland": "NW",
         "elev": "135",
         "icao": "----",
         "lat": "52.1042",
@@ -6013,15 +6013,15 @@
     },
     "10348": {
         "bundesland": "BW",
         "elev": "460",
         "icao": "----",
         "lat": "48.683",
         "lon": "9.017",
-        "name": "B\u00f6blingen (Ph)",
+        "name": "B\u00f6blingen (PH)",
         "report_available": 1
     },
     "10356": {
         "bundesland": "ST",
         "elev": "159",
         "icao": "----",
         "lat": "52.1601",
@@ -6103,15 +6103,15 @@
     },
     "10384": {
         "bundesland": "BW",
         "elev": "600",
         "icao": "EDDI",
         "lat": "48.567",
         "lon": "9.633",
-        "name": "Wiesensteig (Ph)",
+        "name": "Wiesensteig (PH)",
         "report_available": 1
     },
     "10385": {
         "bundesland": "BW",
         "elev": "580",
         "icao": "EDDB",
         "lat": "48.6",
@@ -6292,15 +6292,15 @@
     },
     "10438": {
         "bundesland": "BW",
         "elev": "230",
         "icao": "----",
         "lat": "48.933",
         "lon": "9.267",
-        "name": "Marbach A. Neckar",
+        "name": "Marbach a. Neckar",
         "report_available": 0
     },
     "10439": {
         "bundesland": "BW",
         "elev": "280",
         "icao": "ETHF",
         "lat": "48.9",
@@ -6373,33 +6373,33 @@
     },
     "10457": {
         "bundesland": "BW",
         "elev": "230",
         "icao": "----",
         "lat": "49.483",
         "lon": "9.9",
-        "name": "Weikersheim (Ph)",
+        "name": "Weikersheim (PH)",
         "report_available": 0
     },
     "10458": {
         "bundesland": "BW",
         "elev": "310",
         "icao": "----",
         "lat": "48.65",
         "lon": "9.467",
-        "name": "Kirchheim Unter Teck",
+        "name": "Kirchheim unter Teck",
         "report_available": 1
     },
     "10460": {
         "bundesland": "BW",
         "elev": "290",
         "icao": "----",
         "lat": "48.617",
         "lon": "9.35",
-        "name": "N\u00fcrtingen (Ph)",
+        "name": "N\u00fcrtingen (PH)",
         "report_available": 1
     },
     "10466": {
         "bundesland": "BW",
         "elev": "210",
         "icao": "----",
         "lat": "49.217",
@@ -6499,15 +6499,15 @@
     },
     "10495": {
         "bundesland": "BW",
         "elev": "280",
         "icao": "----",
         "lat": "48.917",
         "lon": "8.95",
-        "name": "Vaihingen A. D. Enz-Aurich",
+        "name": "Vaihingen a. d. Enz-Aurich",
         "report_available": 1
     },
     "10496": {
         "bundesland": "BW",
         "elev": "190",
         "icao": "ETCO",
         "lat": "49.067",
@@ -6517,15 +6517,15 @@
     },
     "10499": {
         "bundesland": "BW",
         "elev": "200",
         "icao": "EDBX",
         "lat": "49.033",
         "lon": "8.767",
-        "name": "Knittlingen (Ph)",
+        "name": "Knittlingen (PH)",
         "report_available": 1
     },
     "10500": {
         "bundesland": "BW",
         "elev": "250",
         "icao": "ETNG",
         "lat": "49",
@@ -6580,15 +6580,15 @@
     },
     "10513": {
         "bundesland": "BW",
         "elev": "500",
         "icao": "EDDK",
         "lat": "48.883",
         "lon": "9.65",
-        "name": "Welzheim (Ph)",
+        "name": "Welzheim (PH)",
         "report_available": 1
     },
     "10514": {
         "bundesland": "RP",
         "elev": "181",
         "icao": "ETHM",
         "lat": "50.3667",
@@ -6751,15 +6751,15 @@
     },
     "10548": {
         "bundesland": "BW",
         "elev": "270",
         "icao": "----",
         "lat": "49.433",
         "lon": "9.433",
-        "name": "Osterburken (Ph)",
+        "name": "Osterburken (PH)",
         "report_available": 1
     },
     "10552": {
         "bundesland": "TH",
         "elev": "938",
         "icao": "----",
         "lat": "50.6545",
@@ -6787,15 +6787,15 @@
     },
     "10557": {
         "bundesland": "TH",
         "elev": "845",
         "icao": "----",
         "lat": "50.5003",
         "lon": "11.1345",
-        "name": "Neuhaus Am Rennweg",
+        "name": "Neuhaus am Rennweg",
         "report_available": 1
     },
     "10558": {
         "bundesland": "TH",
         "elev": "626",
         "icao": "----",
         "lat": "50.3746",
@@ -6823,15 +6823,15 @@
     },
     "10567": {
         "bundesland": "BW",
         "elev": "340",
         "icao": "----",
         "lat": "49.467",
         "lon": "8.767",
-        "name": "Wilhelmsfeld (Ph)",
+        "name": "Wilhelmsfeld (PH)",
         "report_available": 1
     },
     "10569": {
         "bundesland": "BW",
         "elev": "110",
         "icao": "----",
         "lat": "49.083",
@@ -7129,15 +7129,15 @@
     },
     "10704": {
         "bundesland": "BW",
         "elev": "420",
         "icao": "----",
         "lat": "47.733",
         "lon": "8.833",
-        "name": "Rielasingen (Ph)",
+        "name": "Rielasingen (PH)",
         "report_available": 1
     },
     "10706": {
         "bundesland": "SL",
         "elev": "387",
         "icao": "----",
         "lat": "49.4737",
@@ -7273,24 +7273,24 @@
     },
     "10747": {
         "bundesland": "BW",
         "elev": "950",
         "icao": "----",
         "lat": "47.833",
         "lon": "8.183",
-        "name": "Schluchsee (Ph)",
+        "name": "Schluchsee (PH)",
         "report_available": 1
     },
     "10755": {
         "bundesland": "BW",
         "elev": "230",
         "icao": "ETEB",
         "lat": "48.733",
         "lon": "8.367",
-        "name": "Au I. Murgtal",
+        "name": "Au i. Murgtal",
         "report_available": 0
     },
     "10756": {
         "bundesland": "BY",
         "elev": "475",
         "icao": "----",
         "lat": "49.1623",
@@ -7408,15 +7408,15 @@
     },
     "10815": {
         "bundesland": "BW",
         "elev": "360",
         "icao": "----",
         "lat": "48.3",
         "lon": "8.233",
-        "name": "Wolfach (Ph)",
+        "name": "Wolfach (PH)",
         "report_available": 1
     },
     "10818": {
         "bundesland": "BW",
         "elev": "974",
         "icao": "----",
         "lat": "48.1054",
@@ -7624,15 +7624,15 @@
     },
     "10935": {
         "bundesland": "BW",
         "elev": "350",
         "icao": "EDNY",
         "lat": "48.467",
         "lon": "8.933",
-        "name": "Rottenburg A. Neckar",
+        "name": "Rottenburg a. Neckar",
         "report_available": 0
     },
     "10945": {
         "bundesland": "BW",
         "elev": "672",
         "icao": "----",
         "lat": "47.7955",
@@ -7642,15 +7642,15 @@
     },
     "10946": {
         "bundesland": "BW",
         "elev": "650",
         "icao": "EDMK",
         "lat": "47.783",
         "lon": "9.883",
-        "name": "Ki\u00dflegg (Ph)",
+        "name": "Ki\u00dflegg (PH)",
         "report_available": 1
     },
     "10947": {
         "bundesland": "BY",
         "elev": "630",
         "icao": "ETSM",
         "lat": "47.9833",
@@ -7669,15 +7669,15 @@
     },
     "10954": {
         "bundesland": "BY",
         "elev": "630",
         "icao": "ETHA",
         "lat": "48.05",
         "lon": "10.883",
-        "name": "Landsberg A. Lech",
+        "name": "Landsberg a. Lech",
         "report_available": 1
     },
     "10961": {
         "bundesland": "BY",
         "elev": "2956",
         "icao": "----",
         "lat": "47.421",
@@ -7876,24 +7876,24 @@
     },
     "11053": {
         "bundesland": "BY",
         "elev": "500",
         "icao": "----",
         "lat": "47.85",
         "lon": "12.817",
-        "name": "Teisendorf (Ph)",
+        "name": "Teisendorf (PH)",
         "report_available": 0
     },
     "11055": {
         "bundesland": "BY",
         "elev": "390",
         "icao": "----",
         "lat": "48.067",
         "lon": "12.767",
-        "name": "Tittmoning (Ph)",
+        "name": "Tittmoning (PH)",
         "report_available": 0
     },
     "11060": {
         "bundesland": "BY",
         "elev": "690",
         "icao": "----",
         "lat": "47.783",
@@ -8092,15 +8092,15 @@
     },
     "11145": {
         "bundesland": "BY",
         "elev": "690",
         "icao": "----",
         "lat": "47.683",
         "lon": "11.2",
-        "name": "Murnau Am Staffelsee",
+        "name": "Murnau am Staffelsee",
         "report_available": 0
     },
     "11146": {
         "bundesland": "BY",
         "elev": "590",
         "icao": "----",
         "lat": "47.917",
@@ -8173,15 +8173,15 @@
     },
     "11165": {
         "bundesland": "BY",
         "elev": "800",
         "icao": "LOXZ",
         "lat": "49.017",
         "lon": "12.817",
-        "name": "Sankt Englmar (Ph)",
+        "name": "Sankt Englmar (PH)",
         "report_available": 0
     },
     "11170": {
         "bundesland": "BY",
         "elev": "530",
         "icao": "----",
         "lat": "49.067",
@@ -8236,15 +8236,15 @@
     },
     "11190": {
         "bundesland": "BY",
         "elev": "770",
         "icao": "----",
         "lat": "48.833",
         "lon": "13.233",
-        "name": "Sch\u00f6fweg (Ph)",
+        "name": "Sch\u00f6fweg (PH)",
         "report_available": 1
     },
     "11192": {
         "bundesland": "BY",
         "elev": "950",
         "icao": "----",
         "lat": "48.933",
@@ -8335,15 +8335,15 @@
     },
     "11240": {
         "bundesland": "BY",
         "elev": "330",
         "icao": "LOWG",
         "lat": "48.467",
         "lon": "13.417",
-        "name": "Sulzbach Am Inn",
+        "name": "Sulzbach am Inn",
         "report_available": 1
     },
     "11245": {
         "bundesland": "BY",
         "elev": "360",
         "icao": "----",
         "lat": "48.433",
@@ -8497,24 +8497,24 @@
     },
     "11350": {
         "bundesland": "BY",
         "elev": "406",
         "icao": "----",
         "lat": "49.333",
         "lon": "11.433",
-        "name": "Berg Bei Neumarkt I. D. Oberpf.",
+        "name": "Berg bei Neumarkt i. d. Oberpf.",
         "report_available": 0
     },
     "11354": {
         "bundesland": "BY",
         "elev": "440",
         "icao": "----",
         "lat": "49.3",
         "lon": "11.283",
-        "name": "Pyrbaum (Ph)",
+        "name": "Pyrbaum (PH)",
         "report_available": 0
     },
     "11355": {
         "bundesland": "BY",
         "elev": "425",
         "icao": "----",
         "lat": "49.267",
@@ -8542,15 +8542,15 @@
     },
     "11390": {
         "bundesland": "BY",
         "elev": "370",
         "icao": "----",
         "lat": "49.033",
         "lon": "12.217",
-        "name": "Donaustauf (Ph)",
+        "name": "Donaustauf (PH)",
         "report_available": 0
     },
     "11406": {
         "bundesland": "BY",
         "elev": "332",
         "icao": "----",
         "lat": "48.983",
@@ -8614,15 +8614,15 @@
     },
     "11487": {
         "bundesland": "BY",
         "elev": "400",
         "icao": "----",
         "lat": "50.05",
         "lon": "11.667",
-        "name": "Berneck, Bad (Ph)",
+        "name": "Berneck, Bad (PH)",
         "report_available": 1
     },
     "11502": {
         "bundesland": "BY",
         "elev": "340",
         "icao": "----",
         "lat": "50.367",
@@ -8758,15 +8758,15 @@
     },
     "11693": {
         "bundesland": "BY",
         "elev": "290",
         "icao": "----",
         "lat": "49.583",
         "lon": "10.6",
-        "name": "Neustadt A. D. Aisch",
+        "name": "Neustadt a. d. Aisch",
         "report_available": 0
     },
     "11698": {
         "bundesland": "BY",
         "elev": "440",
         "icao": "----",
         "lat": "49.367",
@@ -8875,15 +8875,15 @@
     },
     "11867": {
         "bundesland": "BY",
         "elev": "210",
         "icao": "----",
         "lat": "49.817",
         "lon": "9.633",
-        "name": "Erlenbach A. Main",
+        "name": "Erlenbach a. Main",
         "report_available": 0
     },
     "11880": {
         "bundesland": "BY",
         "elev": "380",
         "icao": "----",
         "lat": "50.383",
@@ -8902,15 +8902,15 @@
     },
     "11927": {
         "bundesland": "BY",
         "elev": "470",
         "icao": "----",
         "lat": "48.433",
         "lon": "10.883",
-        "name": "Gersthofen (Ph)",
+        "name": "Gersthofen (PH)",
         "report_available": 0
     },
     "11933": {
         "bundesland": "BY",
         "elev": "450",
         "icao": "----",
         "lat": "48.717",
@@ -8920,15 +8920,15 @@
     },
     "11934": {
         "bundesland": "BY",
         "elev": "410",
         "icao": "LZTT",
         "lat": "48.633",
         "lon": "10.617",
-        "name": "Blindheim (Ph)",
+        "name": "Blindheim (PH)",
         "report_available": 1
     },
     "11938": {
         "bundesland": "BY",
         "elev": "450",
         "icao": "----",
         "lat": "48.617",
@@ -8956,15 +8956,15 @@
     },
     "11978": {
         "bundesland": "BY",
         "elev": "890",
         "icao": "----",
         "lat": "47.7",
         "lon": "10.233",
-        "name": "Buchenberg (Ph)",
+        "name": "Buchenberg (PH)",
         "report_available": 0
     },
     "11993": {
         "bundesland": "BY",
         "elev": "760",
         "icao": "LZKC",
         "lat": "47.85",
@@ -9019,15 +9019,15 @@
     },
     "12185": {
         "bundesland": "BB",
         "elev": "135",
         "icao": "----",
         "lat": "51.433",
         "lon": "13.217",
-        "name": "M\u00fchlberg/Elbe (Ph)",
+        "name": "M\u00fchlberg/Elbe (PH)",
         "report_available": 0
     },
     "12195": {
         "bundesland": "BB",
         "elev": "50",
         "icao": "EPSU",
         "lat": "52.217",
@@ -9064,15 +9064,15 @@
     },
     "12230": {
         "bundesland": "BB",
         "elev": "85",
         "icao": "EPPI",
         "lat": "51.667",
         "lon": "14.217",
-        "name": "Drebkau (Ph)",
+        "name": "Drebkau (PH)",
         "report_available": 0
     },
     "12235": {
         "bundesland": "BB",
         "elev": "50",
         "icao": "----",
         "lat": "52.917",
@@ -9118,15 +9118,15 @@
     },
     "12300": {
         "bundesland": "BB",
         "elev": "80",
         "icao": "----",
         "lat": "51.7",
         "lon": "13.233",
-        "name": "Herzberg/Elster (Ph)",
+        "name": "Herzberg/Elster (PH)",
         "report_available": 1
     },
     "12310": {
         "bundesland": "BB",
         "elev": "91",
         "icao": "----",
         "lat": "51.917",
@@ -9163,15 +9163,15 @@
     },
     "12360": {
         "bundesland": "BB",
         "elev": "30",
         "icao": "EPPL",
         "lat": "52.75",
         "lon": "12.583",
-        "name": "Friesack (Ph)",
+        "name": "Friesack (PH)",
         "report_available": 0
     },
     "12375": {
         "bundesland": "BB",
         "elev": "45",
         "icao": "EPWA",
         "lat": "52.933",
@@ -9316,15 +9316,15 @@
     },
     "12530": {
         "bundesland": "MV",
         "elev": "5",
         "icao": "----",
         "lat": "53.933",
         "lon": "12.1",
-        "name": "Schwaan (Ph)",
+        "name": "Schwaan (PH)",
         "report_available": 1
     },
     "12540": {
         "bundesland": "MV",
         "elev": "30",
         "icao": "----",
         "lat": "53.7",
@@ -9334,15 +9334,15 @@
     },
     "12550": {
         "bundesland": "MV",
         "elev": "30",
         "icao": "EPCH",
         "lat": "54.117",
         "lon": "13.617",
-        "name": "Wusterhusen (Ph)",
+        "name": "Wusterhusen (PH)",
         "report_available": 0
     },
     "12555": {
         "bundesland": "MV",
         "elev": "15",
         "icao": "EPKT",
         "lat": "53.85",
@@ -9361,15 +9361,15 @@
     },
     "12566": {
         "bundesland": "MV",
         "elev": "20",
         "icao": "EPKK",
         "lat": "53.933",
         "lon": "12.35",
-        "name": "Laage (Ph)",
+        "name": "Laage (PH)",
         "report_available": 1
     },
     "12570": {
         "bundesland": "MV",
         "elev": "80",
         "icao": "EPKA",
         "lat": "53.683",
@@ -9415,15 +9415,15 @@
     },
     "12660": {
         "bundesland": "MV",
         "elev": "10",
         "icao": "EPNL",
         "lat": "54.033",
         "lon": "12.467",
-        "name": "Tessin B. Rostock",
+        "name": "Tessin b. Rostock",
         "report_available": 0
     },
     "12690": {
         "bundesland": "MV",
         "elev": "55",
         "icao": "----",
         "lat": "53.55",
@@ -9514,24 +9514,24 @@
     },
     "12843": {
         "bundesland": "SN",
         "elev": "150",
         "icao": "----",
         "lat": "51.217",
         "lon": "13.733",
-        "name": "Radeburg (Ph)",
+        "name": "Radeburg (PH)",
         "report_available": 1
     },
     "12846": {
         "bundesland": "SN",
         "elev": "115",
         "icao": "----",
         "lat": "51.45",
         "lon": "12.65",
-        "name": "Eilenburg (Ph)",
+        "name": "Eilenburg (PH)",
         "report_available": 0
     },
     "12882": {
         "bundesland": "SN",
         "elev": "244",
         "icao": "LHDC",
         "lat": "51.133",
@@ -9613,15 +9613,15 @@
     },
     "13168": {
         "bundesland": "ST",
         "elev": "80",
         "icao": "----",
         "lat": "51.717",
         "lon": "12.05",
-        "name": "Libehna (Ph)",
+        "name": "Libehna (PH)",
         "report_available": 1
     },
     "13262": {
         "bundesland": "ST",
         "elev": "200",
         "icao": "----",
         "lat": "51.5",
@@ -9631,15 +9631,15 @@
     },
     "13269": {
         "bundesland": "ST",
         "elev": "50",
         "icao": "----",
         "lat": "52",
         "lon": "11.833",
-        "name": "P\u00f6mmelte (Ph)",
+        "name": "P\u00f6mmelte (PH)",
         "report_available": 1
     },
     "13272": {
         "bundesland": "ST",
         "elev": "80",
         "icao": "----",
         "lat": "51.883",
@@ -9649,24 +9649,24 @@
     },
     "13274": {
         "bundesland": "ST",
         "elev": "80",
         "icao": "LYBE",
         "lat": "51.85",
         "lon": "11.533",
-        "name": "Hecklingen B. Sta\u00dffurt",
+        "name": "Hecklingen b. Sta\u00dffurt",
         "report_available": 1
     },
     "13278": {
         "bundesland": "ST",
         "elev": "45",
         "icao": "----",
         "lat": "52.617",
         "lon": "11.733",
-        "name": "Steinfeld-Sch\u00f6nfeld (Ph)",
+        "name": "Steinfeld-Sch\u00f6nfeld (PH)",
         "report_available": 1
     },
     "13295": {
         "bundesland": "ST",
         "elev": "105",
         "icao": "----",
         "lat": "51.267",
@@ -9703,15 +9703,15 @@
     },
     "13388": {
         "bundesland": "TH",
         "elev": "215",
         "icao": "LYNI",
         "lat": "50.967",
         "lon": "10.083",
-        "name": "Gerstungen (Ph)",
+        "name": "Gerstungen (PH)",
         "report_available": 1
     },
     "13389": {
         "bundesland": "TH",
         "elev": "280",
         "icao": "----",
         "lat": "51.133",
@@ -9730,24 +9730,24 @@
     },
     "13457": {
         "bundesland": "TH",
         "elev": "670",
         "icao": "----",
         "lat": "50.583",
         "lon": "11",
-        "name": "Gro\u00dfbreitenbach (Ph)",
+        "name": "Gro\u00dfbreitenbach (PH)",
         "report_available": 0
     },
     "13459": {
         "bundesland": "TH",
         "elev": "430",
         "icao": "----",
         "lat": "50.733",
         "lon": "10.883",
-        "name": "Martinroda B. Ilmenau",
+        "name": "Martinroda b. Ilmenau",
         "report_available": 0
     },
     "13461": {
         "bundesland": "TH",
         "elev": "240",
         "icao": "----",
         "lat": "50.8",
@@ -9757,33 +9757,33 @@
     },
     "13462": {
         "bundesland": "TH",
         "elev": "135",
         "icao": "LYTI",
         "lat": "51.05",
         "lon": "11.7",
-        "name": "Camburg (Ph)",
+        "name": "Camburg (PH)",
         "report_available": 1
     },
     "13463": {
         "bundesland": "TH",
         "elev": "300",
         "icao": "----",
         "lat": "51.017",
         "lon": "11.667",
-        "name": "Dornburg/Saale (Ph)",
+        "name": "Dornburg/Saale (PH)",
         "report_available": 0
     },
     "13473": {
         "bundesland": "TH",
         "elev": "186",
         "icao": "----",
         "lat": "51.167",
         "lon": "10.633",
-        "name": "Langensalza, Bad-Gro\u00dfwelsbach (Ph)",
+        "name": "Langensalza, Bad-Gro\u00dfwelsbach (PH)",
         "report_available": 1
     },
     "13477": {
         "bundesland": "TH",
         "elev": "480",
         "icao": "----",
         "lat": "50.4",
@@ -9802,15 +9802,15 @@
     },
     "13489": {
         "bundesland": "TH",
         "elev": "310",
         "icao": "----",
         "lat": "50.533",
         "lon": "10.5",
-        "name": "Belrieth (Ph)",
+        "name": "Belrieth (PH)",
         "report_available": 1
     },
     "13586": {
         "bundesland": "TH",
         "elev": "180",
         "icao": "LWSK",
         "lat": "51.183",
@@ -9820,15 +9820,15 @@
     },
     "13600": {
         "bundesland": "TH",
         "elev": "450",
         "icao": "----",
         "lat": "50.367",
         "lon": "11.283",
-        "name": "Heinersdorf B. Sonneberg/Th\u00fcr.",
+        "name": "Heinersdorf b. Sonneberg/Th\u00fcr.",
         "report_available": 0
     },
     "13610": {
         "bundesland": "TH",
         "elev": "210",
         "icao": "----",
         "lat": "50.867",
@@ -19225,15 +19225,15 @@
     },
     "70361": {
         "bundesland": "BW",
         "elev": "255",
         "icao": "PAYA",
         "lat": "47.995",
         "lon": "7.824",
-        "name": "Freiburg Im Breisgau-Haslach",
+        "name": "Freiburg im Breisgau-Haslach",
         "report_available": 0
     },
     "70381": {
         "bundesland": "Britisch-Kolumbien",
         "elev": "5",
         "icao": "PAJN",
         "lat": "58.22",
@@ -21565,42 +21565,42 @@
     },
     "82244": {
         "bundesland": "Par\u00e1",
         "elev": "72",
         "icao": "SBSN",
         "lat": "-2.25",
         "lon": "-54.48",
-        "name": "Santar\ufffdM",
+        "name": "Santar\u00e9m",
         "report_available": 0
     },
     "82280": {
         "bundesland": "",
         "elev": "51",
         "icao": "SBSL",
         "lat": "-2.32",
         "lon": "-44.18",
-        "name": "S\ufffdO Luiz",
+        "name": "S\u00e3o Luiz",
         "report_available": 0
     },
     "82288": {
         "bundesland": "",
         "elev": "5",
         "icao": "SBPB",
         "lat": "-2.54",
         "lon": "-41.44",
-        "name": "Parna\ufffdBa",
+        "name": "Parna\u00edba",
         "report_available": 0
     },
     "82317": {
         "bundesland": "Amazonas",
         "elev": "47",
         "icao": "SBTF",
         "lat": "-3.22",
         "lon": "-64.42",
-        "name": "Tef\ufffd",
+        "name": "Tef\u00e9",
         "report_available": 0
     },
     "82332": {
         "bundesland": "Amazonas",
         "elev": "84",
         "icao": "SBEG",
         "lat": "-3.09",
@@ -21664,15 +21664,15 @@
     },
     "82562": {
         "bundesland": "Par\u00e1",
         "elev": "95",
         "icao": "SBMA",
         "lat": "-5.22",
         "lon": "-49.08",
-        "name": "Marab\ufffd",
+        "name": "Marab\u00e1",
         "report_available": 0
     },
     "82564": {
         "bundesland": "Maranh\u00e3o",
         "elev": "123",
         "icao": "SBIZ",
         "lat": "-5.32",
@@ -21727,15 +21727,15 @@
     },
     "82610": {
         "bundesland": "Amazonas",
         "elev": "104",
         "icao": "SWEI",
         "lat": "-6.40",
         "lon": "-69.52",
-        "name": "Eirunep\ufffd",
+        "name": "Eirunep\u00e9",
         "report_available": 0
     },
     "82640": {
         "bundesland": "Par\u00e1",
         "elev": "98",
         "icao": "SBEK",
         "lat": "-6.14",
@@ -21745,15 +21745,15 @@
     },
     "82659": {
         "bundesland": "Tocantins",
         "elev": "229",
         "icao": "SWGN",
         "lat": "-7.06",
         "lon": "-48.12",
-        "name": "Aragua\ufffdNa",
+        "name": "Aragua\u00edna",
         "report_available": 0
     },
     "82795": {
         "bundesland": "",
         "elev": "548",
         "icao": "SBKG",
         "lat": "-7.14",
@@ -21763,15 +21763,15 @@
     },
     "82798": {
         "bundesland": "",
         "elev": "7",
         "icao": "SBJP",
         "lat": "-7.06",
         "lon": "-34.51",
-        "name": "Jo\ufffdO Pessoa",
+        "name": "Jo\u00e3o Pessoa",
         "report_available": 0
     },
     "82824": {
         "bundesland": "Amazonas",
         "elev": "102",
         "icao": "SBPV",
         "lat": "-8.43",
@@ -21853,15 +21853,15 @@
     },
     "83095": {
         "bundesland": "Pernambuco",
         "elev": "8",
         "icao": "SBAR",
         "lat": "-10.59",
         "lon": "-37.04",
-        "name": "Aracaj\ufffd",
+        "name": "Aracaj\u00fa",
         "report_available": 0
     },
     "83096": {
         "bundesland": "Pernambuco",
         "elev": "9",
         "icao": "----",
         "lat": "-10.55",
@@ -21889,15 +21889,15 @@
     },
     "83242": {
         "bundesland": "Bahia",
         "elev": "439",
         "icao": "SBLE",
         "lat": "-12.33",
         "lon": "-41.23",
-        "name": "Len\ufffd\ufffdIs",
+        "name": "Len\u00e7\u00f3is",
         "report_available": 0
     },
     "83248": {
         "bundesland": "Sergipe",
         "elev": "6",
         "icao": "SBSV",
         "lat": "-12.54",
@@ -21907,15 +21907,15 @@
     },
     "83344": {
         "bundesland": "Bahia",
         "elev": "875",
         "icao": "SBQV",
         "lat": "-14.53",
         "lon": "-40.48",
-        "name": "Vit\ufffdRia Da Conquista",
+        "name": "Vit\u00f3ria Da Conquista",
         "report_available": 0
     },
     "83349": {
         "bundesland": "Bahia",
         "elev": "4",
         "icao": "SBIL",
         "lat": "-14.49",
@@ -21925,15 +21925,15 @@
     },
     "83359": {
         "bundesland": "Mato Grosso",
         "elev": "350",
         "icao": "SBBW",
         "lat": "-15.52",
         "lon": "-52.23",
-        "name": "Barra Do Gar\ufffdAs",
+        "name": "Barra Do Gar\u00e7as",
         "report_available": 0
     },
     "83362": {
         "bundesland": "Mato Grosso",
         "elev": "187",
         "icao": "SBCY",
         "lat": "-15.39",
@@ -21961,15 +21961,15 @@
     },
     "83410": {
         "bundesland": "Mato Grosso",
         "elev": "284",
         "icao": "SBRD",
         "lat": "-16.28",
         "lon": "-54.35",
-        "name": "Rondon\ufffdPolis",
+        "name": "Rondon\u00f3polis",
         "report_available": 0
     },
     "83423": {
         "bundesland": "Goi\u00e1s",
         "elev": "747",
         "icao": "----",
         "lat": "-16.41",
@@ -21979,15 +21979,15 @@
     },
     "83424": {
         "bundesland": "Goi\u00e1s",
         "elev": "747",
         "icao": "SBGO",
         "lat": "-16.38",
         "lon": "-49.13",
-        "name": "Goi\ufffdNia",
+        "name": "Goi\u00e2nia",
         "report_available": 0
     },
     "83437": {
         "bundesland": "Minas Gerais",
         "elev": "646",
         "icao": "SBMK",
         "lat": "-16.43",
@@ -22024,15 +22024,15 @@
     },
     "83525": {
         "bundesland": "Goi\u00e1s",
         "elev": "945",
         "icao": "SBUL",
         "lat": "-18.53",
         "lon": "-48.14",
-        "name": "Uberl\ufffdNdia",
+        "name": "Uberl\u00e2ndia",
         "report_available": 0
     },
     "83531": {
         "bundesland": "Minas Gerais",
         "elev": "940",
         "icao": "SNPD",
         "lat": "-18.31",
@@ -22051,15 +22051,15 @@
     },
     "83552": {
         "bundesland": "Mato Grosso do Sul",
         "elev": "130",
         "icao": "SBCR",
         "lat": "-19.01",
         "lon": "-57.40",
-        "name": "Corumb\ufffd",
+        "name": "Corumb\u00e1",
         "report_available": 0
     },
     "83576": {
         "bundesland": "Minas Gerais",
         "elev": "808",
         "icao": "SBUR",
         "lat": "-19.46",
@@ -22096,24 +22096,24 @@
     },
     "83618": {
         "bundesland": "Minas Gerais",
         "elev": "313",
         "icao": "SBTG",
         "lat": "-20.47",
         "lon": "-51.42",
-        "name": "Tr\ufffdS Lagoas",
+        "name": "Tr\u00eas Lagoas",
         "report_available": 0
     },
     "83635": {
         "bundesland": "Minas Gerais",
         "elev": "789",
         "icao": "SNDV",
         "lat": "-20.10",
         "lon": "-44.52",
-        "name": "Divin\ufffdPolis",
+        "name": "Divin\u00f3polis",
         "report_available": 0
     },
     "83648": {
         "bundesland": "",
         "elev": "8",
         "icao": "----",
         "lat": "-20.19",
@@ -22123,24 +22123,24 @@
     },
     "83649": {
         "bundesland": "",
         "elev": "3",
         "icao": "SBVT",
         "lat": "-20.15",
         "lon": "-40.17",
-        "name": "Vit\ufffdRia",
+        "name": "Vit\u00f3ria",
         "report_available": 0
     },
     "83652": {
         "bundesland": "Minas Gerais",
         "elev": "549",
         "icao": "SBRP",
         "lat": "-21.08",
         "lon": "-47.46",
-        "name": "Ribeir\ufffdO Preto",
+        "name": "Ribeir\u00e3o Preto",
         "report_available": 0
     },
     "83659": {
         "bundesland": "Mato Grosso do Sul",
         "elev": "452",
         "icao": "SBDO",
         "lat": "-22.14",
@@ -22150,15 +22150,15 @@
     },
     "83672": {
         "bundesland": "S\u00e3o Paulo",
         "elev": "397",
         "icao": "SBAU",
         "lat": "-21.12",
         "lon": "-50.26",
-        "name": "Ara\ufffdAtuba",
+        "name": "Ara\u00e7atuba",
         "report_available": 0
     },
     "83692": {
         "bundesland": "Minas Gerais",
         "elev": "939",
         "icao": "SBJF",
         "lat": "-21.46",
@@ -22267,15 +22267,15 @@
     },
     "83767": {
         "bundesland": "S\u00e3o Paulo",
         "elev": "542",
         "icao": "SBMG",
         "lat": "-23.25",
         "lon": "-51.57",
-        "name": "Maring\ufffd",
+        "name": "Maring\u00e1",
         "report_available": 0
     },
     "83768": {
         "bundesland": "S\u00e3o Paulo",
         "elev": "569",
         "icao": "SBLO",
         "lat": "-23.20",
@@ -22321,15 +22321,15 @@
     },
     "83809": {
         "bundesland": "Rio de Janeiro",
         "elev": "646",
         "icao": "SBSJ",
         "lat": "-23.14",
         "lon": "-45.52",
-        "name": "S\ufffdO Jos\ufffd Dos Campos",
+        "name": "S\u00e3o Jos\u00e9 Dos Campos",
         "report_available": 0
     },
     "83818": {
         "bundesland": "Minas Gerais",
         "elev": "3",
         "icao": "SBST",
         "lat": "-23.56",
@@ -22780,15 +22780,15 @@
     },
     "86676": {
         "bundesland": "Bahia",
         "elev": "105",
         "icao": "SNVB",
         "lat": "-13.21",
         "lon": "-39.08",
-        "name": "Valen\ufffdA",
+        "name": "Valen\u00e7a",
         "report_available": 0
     },
     "86816": {
         "bundesland": "Minas Gerais",
         "elev": "578",
         "icao": "SBBT",
         "lat": "-20.35",
@@ -24454,15 +24454,15 @@
     },
     "B040": {
         "bundesland": "MV",
         "elev": "4",
         "icao": "----",
         "lat": "54.474",
         "lon": "12.501",
-        "name": "Dar\u00dfer Ort (Swn)",
+        "name": "Dar\u00dfer Ort (SWN)",
         "report_available": 0
     },
     "B085": {
         "bundesland": "MV",
         "elev": "4",
         "icao": "----",
         "lat": "54.516",
@@ -24481,15 +24481,15 @@
     },
     "B203": {
         "bundesland": "MV",
         "elev": "51",
         "icao": "----",
         "lat": "54.132",
         "lon": "11.672",
-        "name": "Bastorf-K\u00e4gsdorf (Swn)",
+        "name": "Bastorf-K\u00e4gsdorf (SWN)",
         "report_available": 0
     },
     "B258": {
         "bundesland": "MV",
         "elev": "10",
         "icao": "----",
         "lat": "54.065",
@@ -24679,15 +24679,15 @@
     },
     "B747": {
         "bundesland": "MV",
         "elev": "66",
         "icao": "----",
         "lat": "53.458",
         "lon": "12.242",
-        "name": "Plau Am See",
+        "name": "Plau am See",
         "report_available": 0
     },
     "B766": {
         "bundesland": "MV",
         "elev": "54",
         "icao": "----",
         "lat": "53.526",
@@ -24814,15 +24814,15 @@
     },
     "E031": {
         "bundesland": "NI",
         "elev": "14",
         "icao": "----",
         "lat": "53.767",
         "lon": "7.672",
-        "name": "Spiekeroog (Swn)",
+        "name": "Spiekeroog (SWN)",
         "report_available": 0
     },
     "E043": {
         "bundesland": "NI",
         "elev": "4",
         "icao": "----",
         "lat": "53.641",
@@ -26758,15 +26758,15 @@
     },
     "E667": {
         "bundesland": "NI",
         "elev": "41",
         "icao": "----",
         "lat": "52.5",
         "lon": "9.494",
-        "name": "Neustadt Am R\u00fcbenberge",
+        "name": "Neustadt am R\u00fcbenberge",
         "report_available": 0
     },
     "E672": {
         "bundesland": "NI",
         "elev": "39",
         "icao": "----",
         "lat": "52.588",
@@ -27964,15 +27964,15 @@
     },
     "F9404": {
         "bundesland": "",
         "elev": "28",
         "icao": "SBCM",
         "lat": "-28.44",
         "lon": "-49.26",
-        "name": "Crici\ufffdMa",
+        "name": "Crici\u00fama",
         "report_available": 0
     },
     "F9405": {
         "bundesland": "Goi\u00e1s",
         "elev": "685",
         "icao": "SBCN",
         "lat": "-17.44",
@@ -28018,15 +28018,15 @@
     },
     "F9410": {
         "bundesland": "Mato Grosso",
         "elev": "182",
         "icao": "SBJI",
         "lat": "-10.52",
         "lon": "-61.51",
-        "name": "Ji-Paran\ufffd",
+        "name": "Ji-Paran\u00e1",
         "report_available": 0
     },
     "F9411": {
         "bundesland": "Cear\u00e1",
         "elev": "409",
         "icao": "SBJU",
         "lat": "-7.13",
@@ -28045,24 +28045,24 @@
     },
     "F9413": {
         "bundesland": "Rio Grande do Sul",
         "elev": "322",
         "icao": "SBNM",
         "lat": "-28.17",
         "lon": "-54.10",
-        "name": "Santo \ufffdNgelo",
+        "name": "Santo \u00c2ngelo",
         "report_available": 0
     },
     "F9414": {
         "bundesland": "Minas Gerais",
         "elev": "544",
         "icao": "SBSR",
         "lat": "-20.49",
         "lon": "-49.24",
-        "name": "S\ufffdO Jos\ufffd D. R. Preto",
+        "name": "S\u00e3o Jos\u00e9 D. R. Preto",
         "report_available": 0
     },
     "F9415": {
         "bundesland": "Par\u00e1",
         "elev": "88",
         "icao": "SBTB",
         "lat": "-1.29",
@@ -28288,15 +28288,15 @@
     },
     "F9504": {
         "bundesland": "NI",
         "elev": "27",
         "icao": "----",
         "lat": "52.29",
         "lon": "7.18",
-        "name": "Hanekenf\ufffdHr Umspwk.",
+        "name": "Hanekenf\u00e4hr Umspwk.",
         "report_available": 0
     },
     "F9505": {
         "bundesland": "BW",
         "elev": "275",
         "icao": "----",
         "lat": "48.55",
@@ -28306,15 +28306,15 @@
     },
     "F9506": {
         "bundesland": "BW",
         "elev": "736",
         "icao": "----",
         "lat": "47.36",
         "lon": "7.57",
-        "name": "K\ufffdHmoos Umspwk.",
+        "name": "K\u00fchmoos Umspwk.",
         "report_available": 0
     },
     "F9507": {
         "bundesland": "BY",
         "elev": "721",
         "icao": "----",
         "lat": "47.44",
@@ -28378,15 +28378,15 @@
     },
     "F9513": {
         "bundesland": "RP",
         "elev": "141",
         "icao": "----",
         "lat": "50.24",
         "lon": "7.27",
-        "name": "Wei\ufffdEnturm Umspwk.",
+        "name": "Wei\u00dfenturm Umspwk.",
         "report_available": 0
     },
     "F9514": {
         "bundesland": "NW",
         "elev": "80",
         "icao": "----",
         "lat": "52.17",
@@ -28486,15 +28486,15 @@
     },
     "F9525": {
         "bundesland": "NW",
         "elev": "110",
         "icao": "----",
         "lat": "50.52",
         "lon": "6.50",
-        "name": "Knapsack (H\ufffdRth)",
+        "name": "Knapsack (H\u00fcrth)",
         "report_available": 0
     },
     "F9526": {
         "bundesland": "NW",
         "elev": "56",
         "icao": "----",
         "lat": "50.59",
@@ -29269,15 +29269,15 @@
     },
     "G303": {
         "bundesland": "BY",
         "elev": "624",
         "icao": "----",
         "lat": "48.896",
         "lon": "13.19",
-        "name": "Kirchberg Im Wald",
+        "name": "Kirchberg im Wald",
         "report_available": 0
     },
     "G306": {
         "bundesland": "BY",
         "elev": "420",
         "icao": "----",
         "lat": "48.882",
@@ -29584,15 +29584,15 @@
     },
     "G372": {
         "bundesland": "BY",
         "elev": "536",
         "icao": "----",
         "lat": "48.18",
         "lon": "10.466",
-        "name": "Kirchheim In Schwaben",
+        "name": "Kirchheim in Schwaben",
         "report_available": 0
     },
     "G373": {
         "bundesland": "BY",
         "elev": "450",
         "icao": "----",
         "lat": "48.167",
@@ -29872,15 +29872,15 @@
     },
     "G427": {
         "bundesland": "HE",
         "elev": "89",
         "icao": "----",
         "lat": "49.843",
         "lon": "8.546",
-        "name": "Griesheim B. Darmstadt",
+        "name": "Griesheim b. Darmstadt",
         "report_available": 0
     },
     "G428": {
         "bundesland": "HE",
         "elev": "185",
         "icao": "----",
         "lat": "50.325",
@@ -30241,15 +30241,15 @@
     },
     "H375": {
         "bundesland": "NW",
         "elev": "304",
         "icao": "----",
         "lat": "51.605",
         "lon": "8.818",
-        "name": "Lichtenau-Ebbinghausen (Hrb)",
+        "name": "Lichtenau-Ebbinghausen (HRB)",
         "report_available": 0
     },
     "H376": {
         "bundesland": "NW",
         "elev": "93",
         "icao": "----",
         "lat": "51.71",
@@ -30295,15 +30295,15 @@
     },
     "H411": {
         "bundesland": "NW",
         "elev": "47",
         "icao": "----",
         "lat": "51.873",
         "lon": "6.886",
-        "name": "Borken In Westfalen",
+        "name": "Borken in Westfalen",
         "report_available": 1
     },
     "H419": {
         "bundesland": "NW",
         "elev": "24",
         "icao": "----",
         "lat": "51.509",
@@ -31492,15 +31492,15 @@
     },
     "K212": {
         "bundesland": "RP",
         "elev": "593",
         "icao": "----",
         "lat": "50.305",
         "lon": "6.386",
-        "name": "Roth Bei Pr\u00fcm",
+        "name": "Roth bei Pr\u00fcm",
         "report_available": 0
     },
     "K219": {
         "bundesland": "RP",
         "elev": "407",
         "icao": "----",
         "lat": "50.311",
@@ -32185,15 +32185,15 @@
     },
     "K290": {
         "bundesland": "RP",
         "elev": "286",
         "icao": "----",
         "lat": "50.426",
         "lon": "7.94",
-        "name": "Nentershausen (Ka)",
+        "name": "Nentershausen (KA)",
         "report_available": 0
     },
     "K2913": {
         "bundesland": "BW",
         "elev": "445",
         "icao": "----",
         "lat": "48.41",
@@ -32230,15 +32230,15 @@
     },
     "K295": {
         "bundesland": "RP",
         "elev": "155",
         "icao": "----",
         "lat": "50.357",
         "lon": "8.049",
-        "name": "Holzheim Bei Diez",
+        "name": "Holzheim bei Diez",
         "report_available": 0
     },
     "K300": {
         "bundesland": "RP",
         "elev": "426",
         "icao": "----",
         "lat": "50.228",
@@ -33265,15 +33265,15 @@
     },
     "K584": {
         "bundesland": "RP",
         "elev": "195",
         "icao": "----",
         "lat": "49.966",
         "lon": "8.214",
-        "name": "Mainz-Lerchenberg (Zdf)",
+        "name": "Mainz-Lerchenberg (ZDF)",
         "report_available": 1
     },
     "K587": {
         "bundesland": "RP",
         "elev": "150",
         "icao": "----",
         "lat": "49.51",
@@ -33607,15 +33607,15 @@
     },
     "K787": {
         "bundesland": "RP",
         "elev": "311",
         "icao": "----",
         "lat": "49.32",
         "lon": "8.07",
-        "name": "Grosss\ufffdGm\ufffdHle (Alt.)",
+        "name": "Grosss\u00e4gm\u00fchle (Alt.)",
         "report_available": 0
     },
     "K795": {
         "bundesland": "RP",
         "elev": "98",
         "icao": "----",
         "lat": "49.587",
@@ -34237,15 +34237,15 @@
     },
     "L543": {
         "bundesland": "HE",
         "elev": "314",
         "icao": "----",
         "lat": "50.35",
         "lon": "8.59",
-        "name": "Gr\ufffdNberg",
+        "name": "Gr\u00fcnberg",
         "report_available": 0
     },
     "L555": {
         "bundesland": "HE",
         "elev": "265",
         "icao": "----",
         "lat": "50.493",
@@ -34300,15 +34300,15 @@
     },
     "L595": {
         "bundesland": "HE",
         "elev": "667",
         "icao": "----",
         "lat": "50.25",
         "lon": "9.50",
-        "name": "Gersfeld_(Rh\ufffdN)-Dalh",
+        "name": "Gersfeld_(Rh\u00f6n)-Dalh",
         "report_available": 0
     },
     "L602": {
         "bundesland": "HE",
         "elev": "168",
         "icao": "----",
         "lat": "50.394",
@@ -34372,15 +34372,15 @@
     },
     "L643": {
         "bundesland": "HE",
         "elev": "132",
         "icao": "----",
         "lat": "50.24",
         "lon": "8.59",
-        "name": "Nidda-Kl\ufffdRanlage",
+        "name": "Nidda-Kl\u00e4ranlage",
         "report_available": 0
     },
     "L648": {
         "bundesland": "HE",
         "elev": "184",
         "icao": "----",
         "lat": "50.19",
@@ -34678,15 +34678,15 @@
     },
     "L918": {
         "bundesland": "HE",
         "elev": "92",
         "icao": "----",
         "lat": "49.40",
         "lon": "8.34",
-        "name": "Lorsch-Kl\ufffdRanlage",
+        "name": "Lorsch-Kl\u00e4ranlage",
         "report_available": 0
     },
     "L926": {
         "bundesland": "HE",
         "elev": "208",
         "icao": "----",
         "lat": "49.709",
@@ -37756,15 +37756,15 @@
     },
     "N553": {
         "bundesland": "ST",
         "elev": "82",
         "icao": "----",
         "lat": "52.022",
         "lon": "12.16",
-        "name": "Badewitz Bei Zerbst",
+        "name": "Badewitz bei Zerbst",
         "report_available": 0
     },
     "N5537": {
         "bundesland": "TH",
         "elev": "470",
         "icao": "----",
         "lat": "50.48",
@@ -37900,15 +37900,15 @@
     },
     "N616": {
         "bundesland": "ST",
         "elev": "504",
         "icao": "----",
         "lat": "51.665",
         "lon": "10.881",
-        "name": "Oberharz Am Brocken-Stiege",
+        "name": "Oberharz am Brocken-Stiege",
         "report_available": 1
     },
     "N6160": {
         "bundesland": "HE",
         "elev": "238",
         "icao": "----",
         "lat": "50.28",
@@ -39115,15 +39115,15 @@
     },
     "N9610": {
         "bundesland": "ST",
         "elev": "100",
         "icao": "----",
         "lat": "51.12",
         "lon": "11.58",
-        "name": "Wei\ufffdEnfels",
+        "name": "Wei\u00dfenfels",
         "report_available": 0
     },
     "N977": {
         "bundesland": "ST",
         "elev": "264",
         "icao": "----",
         "lat": "51.031",
@@ -39169,15 +39169,15 @@
     },
     "O057": {
         "bundesland": "SN",
         "elev": "90",
         "icao": "----",
         "lat": "51.519",
         "lon": "12.907",
-        "name": "Klitzschen Bei Torgau",
+        "name": "Klitzschen bei Torgau",
         "report_available": 1
     },
     "O099": {
         "bundesland": "SN",
         "elev": "163",
         "icao": "----",
         "lat": "51.345",
@@ -41563,15 +41563,15 @@
     },
     "P022": {
         "bundesland": "BY",
         "elev": "314",
         "icao": "----",
         "lat": "50.454",
         "lon": "10.221",
-        "name": "Ostheim V.D. Rh\u00f6n",
+        "name": "Ostheim v.d. Rh\u00f6n",
         "report_available": 1
     },
     "P0220": {
         "bundesland": "NW",
         "elev": "57",
         "icao": "----",
         "lat": "51.01",
@@ -42922,15 +42922,15 @@
     },
     "P038": {
         "bundesland": "BY",
         "elev": "333",
         "icao": "----",
         "lat": "50.242",
         "lon": "10.567",
-        "name": "Sulzdorf An Der Lederhecke",
+        "name": "Sulzdorf an der Lederhecke",
         "report_available": 0
     },
     "P0380": {
         "bundesland": "Trentino-S\u00fcdtirol",
         "elev": "1100",
         "icao": "----",
         "lat": "46.56",
@@ -44155,15 +44155,15 @@
     },
     "P052": {
         "bundesland": "BY",
         "elev": "330",
         "icao": "----",
         "lat": "50.32",
         "lon": "11.11",
-        "name": "Neustadt Bei Coburg (Kl\u00e4ranlage)",
+        "name": "Neustadt bei Coburg (Kl\u00e4ranlage)",
         "report_available": 0
     },
     "P0520": {
         "bundesland": "Pernambuco",
         "elev": "228",
         "icao": "----",
         "lat": "-9.56",
@@ -45739,15 +45739,15 @@
     },
     "P280": {
         "bundesland": "BY",
         "elev": "452",
         "icao": "----",
         "lat": "49.817",
         "lon": "11.864",
-        "name": "Neustadt Am Kulm-Filchendorf",
+        "name": "Neustadt am Kulm-Filchendorf",
         "report_available": 1
     },
     "P287": {
         "bundesland": "BY",
         "elev": "492",
         "icao": "----",
         "lat": "49.575",
@@ -45829,15 +45829,15 @@
     },
     "P305": {
         "bundesland": "BY",
         "elev": "415",
         "icao": "----",
         "lat": "49.385",
         "lon": "10.173",
-        "name": "Rothenburg Ob Der Tauber",
+        "name": "Rothenburg ob der Tauber",
         "report_available": 1
     },
     "P306": {
         "bundesland": "BY",
         "elev": "434",
         "icao": "----",
         "lat": "49.383",
@@ -46072,15 +46072,15 @@
     },
     "P376": {
         "bundesland": "BY",
         "elev": "420",
         "icao": "----",
         "lat": "49.361",
         "lon": "12.448",
-        "name": "Neunburg V. Wald-Eixendorf (Seemeister)",
+        "name": "Neunburg v. Wald-Eixendorf (Seemeister)",
         "report_available": 0
     },
     "P379": {
         "bundesland": "BY",
         "elev": "388",
         "icao": "----",
         "lat": "49.241",
@@ -46117,15 +46117,15 @@
     },
     "P396": {
         "bundesland": "BY",
         "elev": "460",
         "icao": "----",
         "lat": "49.259",
         "lon": "12.96",
-        "name": "Neukirchen Beim Heiligen Blut",
+        "name": "Neukirchen beim Heiligen Blut",
         "report_available": 0
     },
     "P401": {
         "bundesland": "BY",
         "elev": "462",
         "icao": "----",
         "lat": "49.13",
@@ -46189,15 +46189,15 @@
     },
     "P422": {
         "bundesland": "BY",
         "elev": "376",
         "icao": "----",
         "lat": "49.211",
         "lon": "11.184",
-        "name": "Rothsee Bei Allersberg",
+        "name": "Rothsee bei Allersberg",
         "report_available": 0
     },
     "P425": {
         "bundesland": "BY",
         "elev": "417",
         "icao": "----",
         "lat": "49.087",
@@ -46387,15 +46387,15 @@
     },
     "P505": {
         "bundesland": "BY",
         "elev": "293",
         "icao": "----",
         "lat": "50.181",
         "lon": "9.574",
-        "name": "Aura Im Sinngrund",
+        "name": "Aura im Sinngrund",
         "report_available": 0
     },
     "P515": {
         "bundesland": "BY",
         "elev": "435",
         "icao": "----",
         "lat": "48.737",
@@ -46693,15 +46693,15 @@
     },
     "P621": {
         "bundesland": "BY",
         "elev": "462",
         "icao": "----",
         "lat": "48.619",
         "lon": "11.006",
-        "name": "Rain Am Lech-Wallerdorf",
+        "name": "Rain am Lech-Wallerdorf",
         "report_available": 0
     },
     "P626": {
         "bundesland": "BY",
         "elev": "460",
         "icao": "----",
         "lat": "48.395",
@@ -46909,15 +46909,15 @@
     },
     "P682": {
         "bundesland": "BY",
         "elev": "415",
         "icao": "----",
         "lat": "48.73",
         "lon": "13.274",
-        "name": "Eging Am See-Rohrbachholz",
+        "name": "Eging am See-Rohrbachholz",
         "report_available": 0
     },
     "P687": {
         "bundesland": "BY",
         "elev": "381",
         "icao": "----",
         "lat": "48.425",
@@ -47404,15 +47404,15 @@
     },
     "P892": {
         "bundesland": "BY",
         "elev": "476",
         "icao": "----",
         "lat": "47.924",
         "lon": "12.756",
-        "name": "Waging Am See",
+        "name": "Waging am See",
         "report_available": 0
     },
     "P893": {
         "bundesland": "BY",
         "elev": "498",
         "icao": "----",
         "lat": "47.853",
@@ -47422,24 +47422,24 @@
     },
     "P894": {
         "bundesland": "BY",
         "elev": "470",
         "icao": "----",
         "lat": "47.959",
         "lon": "12.772",
-        "name": "Waging Am See-Schn\u00f6bling",
+        "name": "Waging am See-Schn\u00f6bling",
         "report_available": 0
     },
     "P903": {
         "bundesland": "BY",
         "elev": "397",
         "icao": "----",
         "lat": "47.54",
         "lon": "9.684",
-        "name": "Lindau (Swn)",
+        "name": "Lindau (SWN)",
         "report_available": 0
     },
     "P904": {
         "bundesland": "BY",
         "elev": "719",
         "icao": "----",
         "lat": "47.835",
@@ -47557,15 +47557,15 @@
     },
     "P929": {
         "bundesland": "BY",
         "elev": "796",
         "icao": "----",
         "lat": "47.577",
         "lon": "10.718",
-        "name": "Schwangau-Horn (Lfw)",
+        "name": "Schwangau-Horn (LfW)",
         "report_available": 0
     },
     "P931": {
         "bundesland": "BY",
         "elev": "936",
         "icao": "----",
         "lat": "47.739",
@@ -47827,15 +47827,15 @@
     },
     "P982": {
         "bundesland": "BY",
         "elev": "686",
         "icao": "----",
         "lat": "47.675",
         "lon": "12.47",
-        "name": "Reit Im Winkl",
+        "name": "Reit im Winkl",
         "report_available": 1
     },
     "P983": {
         "bundesland": "BY",
         "elev": "650",
         "icao": "----",
         "lat": "47.773",
@@ -48745,15 +48745,15 @@
     },
     "Q715": {
         "bundesland": "BW",
         "elev": "218",
         "icao": "----",
         "lat": "48.277",
         "lon": "8.084",
-        "name": "Haslach Im Kinzigtal",
+        "name": "Haslach im Kinzigtal",
         "report_available": 0
     },
     "Q716": {
         "bundesland": "BW",
         "elev": "428",
         "icao": "----",
         "lat": "48.082",
@@ -48790,15 +48790,15 @@
     },
     "Q739": {
         "bundesland": "BW",
         "elev": "663",
         "icao": "----",
         "lat": "47.952",
         "lon": "8.993",
-        "name": "Neuhausen Ob Eck-Unterschwandorf",
+        "name": "Neuhausen ob Eck-Unterschwandorf",
         "report_available": 0
     },
     "Q740": {
         "bundesland": "BW",
         "elev": "619",
         "icao": "----",
         "lat": "48.264",
@@ -48853,15 +48853,15 @@
     },
     "Q786": {
         "bundesland": "BW",
         "elev": "604",
         "icao": "----",
         "lat": "48.1",
         "lon": "9.806",
-        "name": "Biberach An Der Ri\u00df-Bergerhausen",
+        "name": "Biberach an der Ri\u00df-Bergerhausen",
         "report_available": 0
     },
     "Q788": {
         "bundesland": "BW",
         "elev": "581",
         "icao": "----",
         "lat": "48.072",
@@ -48988,15 +48988,15 @@
     },
     "Q891": {
         "bundesland": "BW",
         "elev": "690",
         "icao": "----",
         "lat": "47.959",
         "lon": "10.014",
-        "name": "Rot An Der Rot-Buch",
+        "name": "Rot an der Rot-Buch",
         "report_available": 0
     },
     "Q902": {
         "bundesland": "BW",
         "elev": "716",
         "icao": "----",
         "lat": "47.767",
@@ -49105,15 +49105,15 @@
     },
     "Q951": {
         "bundesland": "BW",
         "elev": "703",
         "icao": "----",
         "lat": "47.808",
         "lon": "9.104",
-        "name": "Sipplingen (Swn)",
+        "name": "Sipplingen (SWN)",
         "report_available": 0
     },
     "Q976": {
         "bundesland": "BW",
         "elev": "394",
         "icao": "----",
         "lat": "47.645",
```

### Comparing `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/PKG-INFO` & `simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-dwd-weatherforecast
-Version: 2.0.8
+Version: 2.0.9
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/SOURCES.txt` & `simple_dwd_weatherforecast-2.0.9/simple_dwd_weatherforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/dummy_data.py` & `simple_dwd_weatherforecast-2.0.9/tests/dummy_data.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_condition.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_daily_condition.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_max.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_daily_max.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_min.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_daily_min.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_sum.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_daily_sum.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_day_values.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_day_values.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_forecast_condition.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_forecast_condition.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_forecast_data.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_forecast_data.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_avg.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_avg.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_condition.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_condition.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_max.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_max.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_min.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_min.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_sum.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_sum.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_values.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_get_timeframe_values.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_is_in_timerange.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_is_in_timerange.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_is_valid_timeframe.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_is_valid_timeframe.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_location_tools.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_location_tools.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_map.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_region.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_reported_weather.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_reported_weather.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_station.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_station.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_update.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_update_hourly.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_update_hourly.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.8/tests/test_weather.py` & `simple_dwd_weatherforecast-2.0.9/tests/test_weather.py`

 * *Files identical despite different names*

