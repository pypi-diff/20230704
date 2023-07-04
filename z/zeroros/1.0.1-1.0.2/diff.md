# Comparing `tmp/zeroros-1.0.1.tar.gz` & `tmp/zeroros-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroros-1.0.1.tar", last modified: Tue Jun 27 15:25:04 2023, max compression
+gzip compressed data, was "zeroros-1.0.2.tar", last modified: Tue Jul  4 10:20:22 2023, max compression
```

## Comparing `zeroros-1.0.1.tar` & `zeroros-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.802597 zeroros-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-27 15:24:54.000000 zeroros-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-27 15:25:04.802597 zeroros-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-27 15:24:54.000000 zeroros-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:25:04.802597 zeroros-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-27 15:24:54.000000 zeroros-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.798597 zeroros-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.798597 zeroros-1.0.1/src/zeroros/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/datalogger.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.802597 zeroros-1.0.1/src/zeroros/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/geometry_msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/nav_msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/sensor_msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/messages/std_msgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 15:24:54.000000 zeroros-1.0.1/src/zeroros/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:25:04.802597 zeroros-1.0.1/src/zeroros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 15:25:04.000000 zeroros-1.0.1/src/zeroros.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:22.292613 zeroros-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-04 10:20:12.000000 zeroros-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-04 10:20:22.292613 zeroros-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-04 10:20:12.000000 zeroros-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:20:22.292613 zeroros-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-04 10:20:12.000000 zeroros-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:22.288613 zeroros-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:22.292613 zeroros-1.0.2/src/zeroros/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/datalogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:22.292613 zeroros-1.0.2/src/zeroros/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/messages/geometry_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/messages/nav_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/messages/sensor_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/messages/std_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-04 10:20:12.000000 zeroros-1.0.2/src/zeroros/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:22.292613 zeroros-1.0.2/src/zeroros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-04 10:20:22.000000 zeroros-1.0.2/src/zeroros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-04 10:20:22.000000 zeroros-1.0.2/src/zeroros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:20:22.000000 zeroros-1.0.2/src/zeroros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-04 10:20:22.000000 zeroros-1.0.2/src/zeroros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 10:20:22.000000 zeroros-1.0.2/src/zeroros.egg-info/top_level.txt
```

### Comparing `zeroros-1.0.1/LICENSE` & `zeroros-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/PKG-INFO` & `zeroros-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroros
-Version: 1.0.1
+Version: 1.0.2
 Summary: ZeroROS middleware
 Home-page: https://github.com/miquelmassot/zeroros
 Author: Miquel Massot
 Author-email: miquel.massot@gmail.com
 Maintainer: Miquel Massot
 Maintainer-email: miquel.massot@gmail.com
 License: BSD-3-Clause
@@ -32,14 +32,20 @@
 <p align="center">
     <a href="https://pypi.org/project/zeroros/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/zeroros">
     </a>
     <a href="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml">
         <img alt="Wheels" src="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml/badge.svg">
     </a>
+    <a href="https://github.com/miquelmassot/zeroros">
+    	<img src="https://img.shields.io/badge/platform-Linux%20%7C%20Windows%20%7C%20macOS-blue.svg" alt="platforms" />
+    </a>
+    <a href="https://github.com/miquelmassot/zeroros">
+    	<img src="https://static.pepy.tech/badge/zeroros" alt="Downloads" />
+    </a>
     <a href="https://github.com/miquelmassot/zeroros/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg">
     </a>
     <br/>
 </p>
 
 ## Installation
```

### Comparing `zeroros-1.0.1/README.md` & `zeroros-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 <p align="center">
     <a href="https://pypi.org/project/zeroros/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/zeroros">
     </a>
     <a href="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml">
         <img alt="Wheels" src="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml/badge.svg">
     </a>
+    <a href="https://github.com/miquelmassot/zeroros">
+    	<img src="https://img.shields.io/badge/platform-Linux%20%7C%20Windows%20%7C%20macOS-blue.svg" alt="platforms" />
+    </a>
+    <a href="https://github.com/miquelmassot/zeroros">
+    	<img src="https://static.pepy.tech/badge/zeroros" alt="Downloads" />
+    </a>
     <a href="https://github.com/miquelmassot/zeroros/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg">
     </a>
     <br/>
 </p>
 
 ## Installation
```

### Comparing `zeroros-1.0.1/setup.py` & `zeroros-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # read the contents of README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="zeroros",
-    version="1.0.1",
+    version="1.0.2",
     description="ZeroROS middleware",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Miquel Massot",
     author_email="miquel.massot@gmail.com",
     maintainer="Miquel Massot",
     maintainer_email="miquel.massot@gmail.com",
```

### Comparing `zeroros-1.0.1/src/zeroros/datalogger.py` & `zeroros-1.0.2/src/zeroros/datalogger.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/src/zeroros/message_broker.py` & `zeroros-1.0.2/src/zeroros/message_broker.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/src/zeroros/messages/geometry_msgs.py` & `zeroros-1.0.2/src/zeroros/messages/geometry_msgs.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/src/zeroros/messages/nav_msgs.py` & `zeroros-1.0.2/src/zeroros/messages/nav_msgs.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/src/zeroros/messages/sensor_msgs.py` & `zeroros-1.0.2/src/zeroros/messages/sensor_msgs.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/src/zeroros/messages/std_msgs.py` & `zeroros-1.0.2/src/zeroros/messages/std_msgs.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/src/zeroros/publisher.py` & `zeroros-1.0.2/src/zeroros/publisher.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/src/zeroros/subscriber.py` & `zeroros-1.0.2/src/zeroros/subscriber.py`

 * *Files identical despite different names*

### Comparing `zeroros-1.0.1/src/zeroros.egg-info/PKG-INFO` & `zeroros-1.0.2/src/zeroros.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroros
-Version: 1.0.1
+Version: 1.0.2
 Summary: ZeroROS middleware
 Home-page: https://github.com/miquelmassot/zeroros
 Author: Miquel Massot
 Author-email: miquel.massot@gmail.com
 Maintainer: Miquel Massot
 Maintainer-email: miquel.massot@gmail.com
 License: BSD-3-Clause
@@ -32,14 +32,20 @@
 <p align="center">
     <a href="https://pypi.org/project/zeroros/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/zeroros">
     </a>
     <a href="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml">
         <img alt="Wheels" src="https://github.com/miquelmassot/zeroros/actions/workflows/python-publish.yml/badge.svg">
     </a>
+    <a href="https://github.com/miquelmassot/zeroros">
+    	<img src="https://img.shields.io/badge/platform-Linux%20%7C%20Windows%20%7C%20macOS-blue.svg" alt="platforms" />
+    </a>
+    <a href="https://github.com/miquelmassot/zeroros">
+    	<img src="https://static.pepy.tech/badge/zeroros" alt="Downloads" />
+    </a>
     <a href="https://github.com/miquelmassot/zeroros/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg">
     </a>
     <br/>
 </p>
 
 ## Installation
```

### Comparing `zeroros-1.0.1/src/zeroros.egg-info/SOURCES.txt` & `zeroros-1.0.2/src/zeroros.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 README.md
 setup.py
 src/zeroros/__init__.py
 src/zeroros/datalogger.py
 src/zeroros/message_broker.py
 src/zeroros/publisher.py
+src/zeroros/rate.py
 src/zeroros/subscriber.py
+src/zeroros/timer.py
 src/zeroros/topic.py
 src/zeroros.egg-info/PKG-INFO
 src/zeroros.egg-info/SOURCES.txt
 src/zeroros.egg-info/dependency_links.txt
 src/zeroros.egg-info/requires.txt
 src/zeroros.egg-info/top_level.txt
 src/zeroros/messages/__init__.py
```

