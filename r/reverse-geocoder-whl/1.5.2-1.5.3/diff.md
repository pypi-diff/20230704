# Comparing `tmp/reverse_geocoder_whl-1.5.2.tar.gz` & `tmp/reverse_geocoder_whl-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse_geocoder_whl-1.5.2.tar", last modified: Sun Mar 19 11:57:29 2023, max compression
+gzip compressed data, was "reverse_geocoder_whl-1.5.3.tar", last modified: Tue Jul  4 10:52:59 2023, max compression
```

## Comparing `reverse_geocoder_whl-1.5.2.tar` & `reverse_geocoder_whl-1.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 11:57:29.770290 reverse_geocoder_whl-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-03-19 11:57:21.000000 reverse_geocoder_whl-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-19 11:57:29.770290 reverse_geocoder_whl-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-19 11:57:21.000000 reverse_geocoder_whl-1.5.2/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 11:57:29.758290 reverse_geocoder_whl-1.5.2/c++/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 11:57:29.766291 reverse_geocoder_whl-1.5.2/c++/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-19 11:57:21.000000 reverse_geocoder_whl-1.5.2/c++/lib/ReverseGeocode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-19 11:57:21.000000 reverse_geocoder_whl-1.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 11:57:29.762290 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl/
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-03-19 11:57:21.000000 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-03-19 11:57:21.000000 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl/cKDTree_MP.py
--rw-r--r--   0 runner    (1001) docker     (123)  7851524 2023-03-19 11:57:21.000000 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl/rg_cities1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 11:57:29.770290 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-19 11:57:29.000000 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-19 11:57:29.000000 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 11:57:29.000000 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-19 11:57:29.000000 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-19 11:57:29.000000 reverse_geocoder_whl-1.5.2/reverse_geocoder_whl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 11:57:29.770290 reverse_geocoder_whl-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-19 11:57:21.000000 reverse_geocoder_whl-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:52:59.725278 reverse_geocoder_whl-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-07-04 10:52:49.000000 reverse_geocoder_whl-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-04 10:52:59.725278 reverse_geocoder_whl-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-04 10:52:49.000000 reverse_geocoder_whl-1.5.3/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:52:59.717278 reverse_geocoder_whl-1.5.3/c++/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:52:59.725278 reverse_geocoder_whl-1.5.3/c++/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-04 10:52:49.000000 reverse_geocoder_whl-1.5.3/c++/lib/ReverseGeocode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-04 10:52:49.000000 reverse_geocoder_whl-1.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:52:59.717278 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl/
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-04 10:52:49.000000 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-04 10:52:49.000000 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl/cKDTree_MP.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7851524 2023-07-04 10:52:50.000000 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl/rg_cities1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:52:59.725278 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-04 10:52:59.000000 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 10:52:59.000000 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:52:59.000000 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 10:52:59.000000 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 10:52:59.000000 reverse_geocoder_whl-1.5.3/reverse_geocoder_whl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:52:59.725278 reverse_geocoder_whl-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-04 10:52:50.000000 reverse_geocoder_whl-1.5.3/setup.py
```

### Comparing `reverse_geocoder_whl-1.5.2/LICENSE` & `reverse_geocoder_whl-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reverse_geocoder_whl-1.5.2/PKG-INFO` & `reverse_geocoder_whl-1.5.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse_geocoder_whl
-Version: 1.5.2
+Version: 1.5.3
 Summary: Fast, offline reverse geocoder
 Home-page: https://github.com/TalAmuyal/reverse-geocoder-whl
 Author-email: Ajay Thampi <ajay.thampi@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -36,7 +36,14 @@
       'admin2': 'Ernakulam'},
      {'name': 'Mountain View', 
       'cc': 'US', 
       'lat': '37.38605',
       'lon': '-122.08385', 
       'admin1': 'California', 
       'admin2': 'Santa Clara County'}]
+
+
+Changelog
+---------
+
+[1.5.3] Limit `scipy` to `>=0.17.1,<1.11` (previously `>=0.17.1`) due to a breaking change in SciPy 1.11.
+[1.5.2] Re-release to original project with Wheels.
```

### Comparing `reverse_geocoder_whl-1.5.2/README.txt` & `reverse_geocoder_whl-1.5.3/README.txt`

 * *Files 15% similar despite different names*

```diff
@@ -26,7 +26,14 @@
       'admin2': 'Ernakulam'},
      {'name': 'Mountain View', 
       'cc': 'US', 
       'lat': '37.38605',
       'lon': '-122.08385', 
       'admin1': 'California', 
       'admin2': 'Santa Clara County'}]
+
+
+Changelog
+---------
+
+[1.5.3] Limit `scipy` to `>=0.17.1,<1.11` (previously `>=0.17.1`) due to a breaking change in SciPy 1.11.
+[1.5.2] Re-release to original project with Wheels.
```

### Comparing `reverse_geocoder_whl-1.5.2/c++/lib/ReverseGeocode.cpp` & `reverse_geocoder_whl-1.5.3/c++/lib/ReverseGeocode.cpp`

 * *Files identical despite different names*

### Comparing `reverse_geocoder_whl-1.5.2/pyproject.toml` & `reverse_geocoder_whl-1.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "reverse_geocoder_whl"
-version = "1.5.2"
+version = "1.5.3"
 authors = [
     {"name" = "Ajay Thampi", "email" = "ajay.thampi@gmail.com"},
 ]
 classifiers = [
 ]
-dependencies = ["numpy>=1.11.0", "scipy>=0.17.1"]
+dependencies = ["numpy>=1.11.0", "scipy>=0.17.1,<1.11"]
 description = "Fast, offline reverse geocoder"
 #license = "LGPL"
 readme = {file = "README.txt", content-type = "text/markdown"}
 requires-python = ">=3.8"
 
 [build-system]
 requires = [
```

### Comparing `reverse_geocoder_whl-1.5.2/reverse_geocoder_whl/__init__.py` & `reverse_geocoder_whl-1.5.3/reverse_geocoder_whl/__init__.py`

 * *Files identical despite different names*

### Comparing `reverse_geocoder_whl-1.5.2/reverse_geocoder_whl/cKDTree_MP.py` & `reverse_geocoder_whl-1.5.3/reverse_geocoder_whl/cKDTree_MP.py`

 * *Files identical despite different names*

### Comparing `reverse_geocoder_whl-1.5.2/reverse_geocoder_whl/rg_cities1000.csv` & `reverse_geocoder_whl-1.5.3/reverse_geocoder_whl/rg_cities1000.csv`

 * *Files identical despite different names*

### Comparing `reverse_geocoder_whl-1.5.2/reverse_geocoder_whl.egg-info/PKG-INFO` & `reverse_geocoder_whl-1.5.3/reverse_geocoder_whl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse-geocoder-whl
-Version: 1.5.2
+Version: 1.5.3
 Summary: Fast, offline reverse geocoder
 Home-page: https://github.com/TalAmuyal/reverse-geocoder-whl
 Author-email: Ajay Thampi <ajay.thampi@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -36,7 +36,14 @@
       'admin2': 'Ernakulam'},
      {'name': 'Mountain View', 
       'cc': 'US', 
       'lat': '37.38605',
       'lon': '-122.08385', 
       'admin1': 'California', 
       'admin2': 'Santa Clara County'}]
+
+
+Changelog
+---------
+
+[1.5.3] Limit `scipy` to `>=0.17.1,<1.11` (previously `>=0.17.1`) due to a breaking change in SciPy 1.11.
+[1.5.2] Re-release to original project with Wheels.
```

### Comparing `reverse_geocoder_whl-1.5.2/setup.py` & `reverse_geocoder_whl-1.5.3/setup.py`

 * *Files identical despite different names*

