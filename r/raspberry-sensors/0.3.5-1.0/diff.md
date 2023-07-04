# Comparing `tmp/raspberry-sensors-0.3.5.tar.gz` & `tmp/raspberry-sensors-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberry-sensors-0.3.5.tar", last modified: Tue Jul  4 19:42:44 2023, max compression
+gzip compressed data, was "raspberry-sensors-1.0.tar", last modified: Tue Jul  4 21:04:16 2023, max compression
```

## Comparing `raspberry-sensors-0.3.5.tar` & `raspberry-sensors-1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 19:42:44.685583 raspberry-sensors-0.3.5/
--rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-0.3.5/LICENSE
--rw-rw-rw-   0        0        0     1787 2023-07-04 19:42:44.685583 raspberry-sensors-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1362 2023-07-01 18:34:08.000000 raspberry-sensors-0.3.5/README.md
--rw-rw-rw-   0        0        0      501 2023-07-04 19:23:42.000000 raspberry-sensors-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 19:42:44.687486 raspberry-sensors-0.3.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 19:42:44.655847 raspberry-sensors-0.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 19:42:44.662061 raspberry-sensors-0.3.5/src/raspberry-sensors/
--rw-rw-rw-   0        0        0     3820 2023-07-04 12:18:45.000000 raspberry-sensors-0.3.5/src/raspberry-sensors/sensors.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:42:44.682634 raspberry-sensors-0.3.5/src/raspberry_sensors.egg-info/
--rw-rw-rw-   0        0        0     1787 2023-07-04 19:42:44.000000 raspberry-sensors-0.3.5/src/raspberry_sensors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-07-04 19:42:44.000000 raspberry-sensors-0.3.5/src/raspberry_sensors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 19:42:44.000000 raspberry-sensors-0.3.5/src/raspberry_sensors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-04 19:42:44.000000 raspberry-sensors-0.3.5/src/raspberry_sensors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 21:04:16.043497 raspberry-sensors-1.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-1.0/LICENSE
+-rw-rw-rw-   0        0        0     1785 2023-07-04 21:04:16.042114 raspberry-sensors-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1362 2023-07-01 18:34:08.000000 raspberry-sensors-1.0/README.md
+-rw-rw-rw-   0        0        0      499 2023-07-04 20:58:06.000000 raspberry-sensors-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 21:04:16.043497 raspberry-sensors-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 21:04:16.007954 raspberry-sensors-1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 21:04:16.017705 raspberry-sensors-1.0/src/raspberry-sensors/
+-rw-rw-rw-   0        0        0        0 2023-07-04 21:02:26.000000 raspberry-sensors-1.0/src/raspberry-sensors/__init__.py
+-rw-rw-rw-   0        0        0     3820 2023-07-04 12:18:45.000000 raspberry-sensors-1.0/src/raspberry-sensors/sensors.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:04:16.040234 raspberry-sensors-1.0/src/raspberry_sensors.egg-info/
+-rw-rw-rw-   0        0        0     1785 2023-07-04 21:04:15.000000 raspberry-sensors-1.0/src/raspberry_sensors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-04 21:04:15.000000 raspberry-sensors-1.0/src/raspberry_sensors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 21:04:15.000000 raspberry-sensors-1.0/src/raspberry_sensors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-04 21:04:15.000000 raspberry-sensors-1.0/src/raspberry_sensors.egg-info/top_level.txt
```

### Comparing `raspberry-sensors-0.3.5/LICENSE` & `raspberry-sensors-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.3.5/PKG-INFO` & `raspberry-sensors-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberry-sensors
-Version: 0.3.5
+Version: 1.0
 Summary: This package for getting values from sensors mh_z19, DHT, ads1015
 Author-email: Develper <testerlzt@mail.ru>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `raspberry-sensors-0.3.5/README.md` & `raspberry-sensors-1.0/README.md`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.3.5/src/raspberry-sensors/sensors.py` & `raspberry-sensors-1.0/src/raspberry-sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.3.5/src/raspberry_sensors.egg-info/PKG-INFO` & `raspberry-sensors-1.0/src/raspberry_sensors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberry-sensors
-Version: 0.3.5
+Version: 1.0
 Summary: This package for getting values from sensors mh_z19, DHT, ads1015
 Author-email: Develper <testerlzt@mail.ru>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

