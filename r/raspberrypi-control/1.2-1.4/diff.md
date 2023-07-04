# Comparing `tmp/raspberrypi_control-1.2.tar.gz` & `tmp/raspberrypi_control-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberrypi_control-1.2.tar", last modified: Tue Jul  4 18:32:11 2023, max compression
+gzip compressed data, was "raspberrypi_control-1.4.tar", last modified: Tue Jul  4 19:03:06 2023, max compression
```

## Comparing `raspberrypi_control-1.2.tar` & `raspberrypi_control-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/raspberrypi_control/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/raspberrypi_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57409 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/raspberrypi_control/raspberrypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/raspberrypi_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:03:06.157053 raspberrypi_control-1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 19:02:56.000000 raspberrypi_control-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-04 19:03:06.157053 raspberrypi_control-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 19:02:56.000000 raspberrypi_control-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 19:02:56.000000 raspberrypi_control-1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:03:06.157053 raspberrypi_control-1.4/raspberrypi_control/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 19:02:56.000000 raspberrypi_control-1.4/raspberrypi_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57409 2023-07-04 19:02:56.000000 raspberrypi_control-1.4/raspberrypi_control/raspberrypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:03:06.157053 raspberrypi_control-1.4/raspberrypi_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-04 19:03:06.000000 raspberrypi_control-1.4/raspberrypi_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 19:03:06.000000 raspberrypi_control-1.4/raspberrypi_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:03:06.000000 raspberrypi_control-1.4/raspberrypi_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 19:03:06.000000 raspberrypi_control-1.4/raspberrypi_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 19:03:06.000000 raspberrypi_control-1.4/raspberrypi_control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:03:06.157053 raspberrypi_control-1.4/setup.cfg
```

### Comparing `raspberrypi_control-1.2/LICENSE` & `raspberrypi_control-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-1.2/PKG-INFO` & `raspberrypi_control-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberrypi_control
-Version: 1.2
+Version: 1.4
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `raspberrypi_control-1.2/README.md` & `raspberrypi_control-1.4/README.md`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-1.2/pyproject.toml` & `raspberrypi_control-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raspberrypi_control"
-version = "1.2"
+version = "1.4"
 authors = [
   { name="Geoloup Team", email="franckiebbb@gmail.com"},
 ]
 description = "Control Raspberrypi board with ssh and python"
 readme = "README.md"
 dependencies = [
     "requests",
```

### Comparing `raspberrypi_control-1.2/raspberrypi_control/raspberrypi.py` & `raspberrypi_control-1.4/raspberrypi_control/raspberrypi.py`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-1.2/raspberrypi_control.egg-info/PKG-INFO` & `raspberrypi_control-1.4/raspberrypi_control.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberrypi-control
-Version: 1.2
+Version: 1.4
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

