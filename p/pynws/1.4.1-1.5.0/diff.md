# Comparing `tmp/pynws-1.4.1.tar.gz` & `tmp/pynws-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynws-1.4.1.tar", last modified: Thu Mar 31 01:17:18 2022, max compression
+gzip compressed data, was "pynws-1.5.0.tar", last modified: Tue Jul  4 14:41:03 2023, max compression
```

## Comparing `pynws-1.4.1.tar` & `pynws-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 01:17:18.230107 pynws-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-31 01:17:08.000000 pynws-1.4.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-03-31 01:17:08.000000 pynws-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-03-31 01:17:08.000000 pynws-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-03-31 01:17:18.230107 pynws-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-03-31 01:17:08.000000 pynws-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 01:17:18.230107 pynws-1.4.1/pynws/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 01:17:18.230107 pynws-1.4.1/pynws/backports/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/backports/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     6781 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     6712 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/nws.py
--rw-r--r--   0 runner    (1001) docker     (121)     3807 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    13372 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/simple_nws.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-31 01:17:08.000000 pynws-1.4.1/pynws/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 01:17:18.230107 pynws-1.4.1/pynws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-03-31 01:17:17.000000 pynws-1.4.1/pynws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-03-31 01:17:17.000000 pynws-1.4.1/pynws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-31 01:17:17.000000 pynws-1.4.1/pynws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-31 01:17:17.000000 pynws-1.4.1/pynws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-31 01:17:17.000000 pynws-1.4.1/pynws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-03-31 01:17:08.000000 pynws-1.4.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-03-31 01:17:18.234107 pynws-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-03-31 01:17:08.000000 pynws-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:41:03.174653 pynws-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 14:40:53.000000 pynws-1.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-04 14:40:53.000000 pynws-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 14:40:53.000000 pynws-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-04 14:41:03.174653 pynws-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-04 14:40:53.000000 pynws-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:41:03.174653 pynws-1.5.0/pynws/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:41:03.174653 pynws-1.5.0/pynws/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/backports/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/nws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/simple_nws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 14:40:53.000000 pynws-1.5.0/pynws/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:41:03.174653 pynws-1.5.0/pynws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-04 14:41:03.000000 pynws-1.5.0/pynws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 14:41:03.000000 pynws-1.5.0/pynws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:41:03.000000 pynws-1.5.0/pynws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 14:41:03.000000 pynws-1.5.0/pynws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 14:41:03.000000 pynws-1.5.0/pynws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-04 14:40:53.000000 pynws-1.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 14:41:03.174653 pynws-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-04 14:40:53.000000 pynws-1.5.0/setup.py
```

### Comparing `pynws-1.4.1/LICENSE` & `pynws-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynws-1.4.1/PKG-INFO` & `pynws-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pynws
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python library to retrieve observations and forecasts from NWS/NOAA
 Home-page: https://github.com/MatthewFlamm/pynws
 Author: Matthew Flamm
 Author-email: matthewflamm0@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynws
 
 A python library to asynchronously retrieve weather observation from NWS/NOAA.
@@ -51,9 +50,7 @@
 |------------|----------------|------------|
 |temperature | degF, degC     | Celsius    |
 |pressure    | Pa             | Pascal     |
 |speed       | m_s-1, km_h-1  | km_h-1     |
 |percent     | percent        | percent    |
 |angle       | degree_(angle) | degrees    |
 |distance    | m              | meter      |
-
-
```

### Comparing `pynws-1.4.1/README.md` & `pynws-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pynws-1.4.1/pynws/backports/enum.py` & `pynws-1.5.0/pynws/backports/enum.py`

 * *Files identical despite different names*

### Comparing `pynws-1.4.1/pynws/const.py` & `pynws-1.5.0/pynws/const.py`

 * *Files identical despite different names*

### Comparing `pynws-1.4.1/pynws/forecast.py` & `pynws-1.5.0/pynws/forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,17 @@
         if not isinstance(when, datetime):
             raise TypeError(f"{when!r} is not a datetime")
 
         when = when.astimezone(timezone.utc)
 
         details: Dict[Detail, DetailValue] = {}
         for detail, time_values in self.details.items():
-            details[detail] = self._get_value_for_time(when, time_values)
+            value = self._get_value_for_time(when, time_values)
+            if value is not None:
+                details[detail] = value
         return details
 
     def get_details_for_times(
         self: DetailedForecast, iterable_when: Iterable[datetime]
     ) -> Iterator[Dict[Detail, DetailValue]]:
         """Retrieve all forecast details for a list of times.
```

### Comparing `pynws-1.4.1/pynws/nws.py` & `pynws-1.5.0/pynws/nws.py`

 * *Files identical despite different names*

### Comparing `pynws-1.4.1/pynws/raw_data.py` & `pynws-1.5.0/pynws/raw_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,19 @@
     """Get observation response from station"""
     params: Dict[str, Any] = {}
     if limit > 0:
         params["limit"] = limit
 
     if start:
         if not isinstance(start, datetime):
-            raise ValueError
+            raise ValueError(
+                f"start parameter needs to be datetime, but got {type(start)}"
+            )
+        if start.tzinfo is None:
+            raise ValueError("start parameter must be timezone aware")
         params["start"] = start.isoformat(timespec="seconds")
 
     url = urls.stations_observations_url(station)
     header = get_header(userid)
     return await _make_request(websession, url, header, params)
```

### Comparing `pynws-1.4.1/pynws/simple_nws.py` & `pynws-1.5.0/pynws/simple_nws.py`

 * *Files 7% similar despite different names*

```diff
@@ -236,40 +236,38 @@
 
     @property
     def all_zones(self: SimpleNWS) -> List[str]:
         """All alert zones."""
         return self._all_zones
 
     @staticmethod
-    def extract_observation_value(
-        observation: Dict[str, Any], value: str
-    ) -> Union[None, Tuple[float, str], str]:
+    def extract_value(
+        values: Dict[str, Any], key: str
+    ) -> Union[None, Tuple[float, Any], str]:
         """Returns observation or observation value."""
-        obs_value = observation.get(value)
-        if obs_value is None:
+        value = values.get(key)
+        if value is None:
             return None
-        if isinstance(observation[value], dict):
-            obs_sub_value = observation[value].get("value")
-            if obs_sub_value is None:
+        if isinstance(value, dict):
+            sub_value = value.get("value")
+            if sub_value is None:
                 return None
-            return float(obs_sub_value), observation[value].get("unitCode")
-        return observation[value]
+            return float(sub_value), value.get("unitCode")
+        return value
 
     @property
     def observation(self: SimpleNWS) -> Optional[Dict[str, Any]]:
         """Observation dict"""
 
         if self._observation is None or self._observation == []:
             return None
 
         data: Dict[str, Any] = {}
         for obs, metar_param in OBSERVATIONS.items():
-            obs_list = [
-                self.extract_observation_value(o, obs) for o in self._observation
-            ]
+            obs_list = [self.extract_value(o, obs) for o in self._observation]
             obs_item = next(iter([o for o in obs_list if o]), None)
             if isinstance(obs_item, tuple):
                 data[obs] = convert_unit(obs_item[1], obs_item[0])
             else:
                 data[obs] = obs_item
 
             if (
@@ -330,16 +328,29 @@
             # get weather
             if filter_forecast:
                 end_time = forecast_entry.get("endTime")
                 if not end_time:
                     continue
                 if now > datetime.fromisoformat(end_time):
                     continue
-            if forecast_entry.get("temperature"):
-                forecast_entry["temperature"] = int(forecast_entry["temperature"])
+
+            if (value := forecast_entry.get("temperature")) is not None:
+                forecast_entry["temperature"] = int(value)
+
+            temp_unit = forecast_entry.get("temperatureUnit")
+
+            for key in ("probabilityOfPrecipitation", "dewpoint", "relativeHumidity"):
+                extracted = SimpleNWS.extract_value(forecast_entry, key)
+                if isinstance(extracted, tuple):
+                    value, value_unit = extracted
+                    if value_unit.endswith("degC") and temp_unit == "F":
+                        value = round(float(value) * 1.8 + 32, 0)
+                    elif value_unit.endswith("degF") and temp_unit == "C":
+                        value = round((float(value) - 32) / 1.8, 0)
+                    forecast_entry[key] = int(value)
 
             if forecast_entry.get("icon"):
                 time, weather = parse_icon(forecast_entry["icon"])
                 weather = convert_weather(weather)
             else:
                 time, weather = (None, None)
             forecast_entry["iconTime"] = time
```

### Comparing `pynws-1.4.1/pynws/units.py` & `pynws-1.5.0/pynws/units.py`

 * *Files identical despite different names*

### Comparing `pynws-1.4.1/pynws/urls.py` & `pynws-1.5.0/pynws/urls.py`

 * *Files identical despite different names*

### Comparing `pynws-1.4.1/pynws.egg-info/PKG-INFO` & `pynws-1.5.0/pynws.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pynws
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python library to retrieve observations and forecasts from NWS/NOAA
 Home-page: https://github.com/MatthewFlamm/pynws
 Author: Matthew Flamm
 Author-email: matthewflamm0@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynws
 
 A python library to asynchronously retrieve weather observation from NWS/NOAA.
@@ -51,9 +50,7 @@
 |------------|----------------|------------|
 |temperature | degF, degC     | Celsius    |
 |pressure    | Pa             | Pascal     |
 |speed       | m_s-1, km_h-1  | km_h-1     |
 |percent     | percent        | percent    |
 |angle       | degree_(angle) | degrees    |
 |distance    | m              | meter      |
-
-
```

### Comparing `pynws-1.4.1/setup.py` & `pynws-1.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     install_requires=[
         "aiohttp",
         "metar",
     ],
     python_requires=">=3.7",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

