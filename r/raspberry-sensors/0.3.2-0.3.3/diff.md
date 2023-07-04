# Comparing `tmp/raspberry-sensors-0.3.2.tar.gz` & `tmp/raspberry-sensors-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberry-sensors-0.3.2.tar", last modified: Tue Jul  4 14:46:37 2023, max compression
+gzip compressed data, was "raspberry-sensors-0.3.3.tar", last modified: Tue Jul  4 19:04:52 2023, max compression
```

## Comparing `raspberry-sensors-0.3.2.tar` & `raspberry-sensors-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 14:46:37.114729 raspberry-sensors-0.3.2/
--rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     1787 2023-07-04 14:46:37.113590 raspberry-sensors-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1362 2023-07-01 18:34:08.000000 raspberry-sensors-0.3.2/README.md
--rw-rw-rw-   0        0        0      501 2023-07-04 12:43:15.000000 raspberry-sensors-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 14:46:37.114729 raspberry-sensors-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 14:46:37.078592 raspberry-sensors-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 14:46:37.095686 raspberry-sensors-0.3.2/src/raspberry-sensors/
--rw-rw-rw-   0        0        0        0 2023-06-28 10:37:28.000000 raspberry-sensors-0.3.2/src/raspberry-sensors/__init__.py
--rw-rw-rw-   0        0        0     3820 2023-07-04 12:18:45.000000 raspberry-sensors-0.3.2/src/raspberry-sensors/sensors.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:46:37.108375 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/
--rw-rw-rw-   0        0        0     1787 2023-07-04 14:46:37.000000 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-04 14:46:37.000000 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 14:46:37.000000 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-04 14:46:37.000000 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 19:04:52.270344 raspberry-sensors-0.3.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     1787 2023-07-04 19:04:52.270079 raspberry-sensors-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1362 2023-07-01 18:34:08.000000 raspberry-sensors-0.3.3/README.md
+-rw-rw-rw-   0        0        0      501 2023-07-04 19:04:29.000000 raspberry-sensors-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 19:04:52.271161 raspberry-sensors-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 19:04:52.237473 raspberry-sensors-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 19:04:52.246189 raspberry-sensors-0.3.3/src/raspberry-sensors/
+-rw-rw-rw-   0        0        0       21 2023-07-04 19:03:28.000000 raspberry-sensors-0.3.3/src/raspberry-sensors/__init__.py
+-rw-rw-rw-   0        0        0     3820 2023-07-04 12:18:45.000000 raspberry-sensors-0.3.3/src/raspberry-sensors/sensors.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:04:52.267946 raspberry-sensors-0.3.3/src/raspberry_sensors.egg-info/
+-rw-rw-rw-   0        0        0     1787 2023-07-04 19:04:52.000000 raspberry-sensors-0.3.3/src/raspberry_sensors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-04 19:04:52.000000 raspberry-sensors-0.3.3/src/raspberry_sensors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 19:04:52.000000 raspberry-sensors-0.3.3/src/raspberry_sensors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-04 19:04:52.000000 raspberry-sensors-0.3.3/src/raspberry_sensors.egg-info/top_level.txt
```

### Comparing `raspberry-sensors-0.3.2/LICENSE` & `raspberry-sensors-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.3.2/PKG-INFO` & `raspberry-sensors-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberry-sensors
-Version: 0.3.2
+Version: 0.3.3
 Summary: This package for getting values from sensors mh_z19, DHT, ads1015
 Author-email: Develper <testerlzt@mail.ru>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `raspberry-sensors-0.3.2/README.md` & `raspberry-sensors-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.3.2/src/raspberry-sensors/sensors.py` & `raspberry-sensors-0.3.3/src/raspberry-sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/PKG-INFO` & `raspberry-sensors-0.3.3/src/raspberry_sensors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberry-sensors
-Version: 0.3.2
+Version: 0.3.3
 Summary: This package for getting values from sensors mh_z19, DHT, ads1015
 Author-email: Develper <testerlzt@mail.ru>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

