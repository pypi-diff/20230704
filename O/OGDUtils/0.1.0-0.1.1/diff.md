# Comparing `tmp/OGDUtils-0.1.0.tar.gz` & `tmp/OGDUtils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OGDUtils-0.1.0.tar", last modified: Mon Jul  3 20:52:00 2023, max compression
+gzip compressed data, was "OGDUtils-0.1.1.tar", last modified: Tue Jul  4 14:31:00 2023, max compression
```

## Comparing `OGDUtils-0.1.0.tar` & `OGDUtils-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 20:52:00.811008 OGDUtils-0.1.0/
--rw-rw-rw-   0        0        0     1117 2022-06-09 19:09:23.000000 OGDUtils-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1434 2023-07-03 20:52:00.808216 OGDUtils-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      824 2023-06-30 19:27:15.000000 OGDUtils-0.1.0/README.md
--rw-rw-rw-   0        0        0      697 2023-06-30 19:29:28.000000 OGDUtils-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 20:52:00.811008 OGDUtils-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 20:52:00.727802 OGDUtils-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 20:52:00.742745 OGDUtils-0.1.0/src/JOWILDER/
--rw-rw-rw-   0        0        0        0 2023-06-30 18:02:36.000000 OGDUtils-0.1.0/src/JOWILDER/__init__.py
--rw-rw-rw-   0        0        0    38315 2023-06-30 18:01:34.000000 OGDUtils-0.1.0/src/JOWILDER/jowilder_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:52:00.753378 OGDUtils-0.1.0/src/LAKELAND/
--rw-rw-rw-   0        0        0        0 2023-06-30 18:02:44.000000 OGDUtils-0.1.0/src/LAKELAND/__init__.py
--rw-rw-rw-   0        0        0     8530 2023-06-30 18:01:31.000000 OGDUtils-0.1.0/src/LAKELAND/lakeland_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:52:00.764507 OGDUtils-0.1.0/src/OGDUtils.egg-info/
--rw-rw-rw-   0        0        0     1434 2023-07-03 20:52:00.000000 OGDUtils-0.1.0/src/OGDUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-07-03 20:52:00.000000 OGDUtils-0.1.0/src/OGDUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:52:00.000000 OGDUtils-0.1.0/src/OGDUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-03 20:52:00.000000 OGDUtils-0.1.0/src/OGDUtils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 20:52:00.771292 OGDUtils-0.1.0/src/WAVES/
--rw-rw-rw-   0        0        0        0 2023-06-30 18:02:50.000000 OGDUtils-0.1.0/src/WAVES/__init__.py
--rw-rw-rw-   0        0        0     3758 2023-06-30 18:01:22.000000 OGDUtils-0.1.0/src/WAVES/waves_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:52:00.807210 OGDUtils-0.1.0/src/general/
--rw-rw-rw-   0        0        0     1240 2023-06-30 17:47:12.000000 OGDUtils-0.1.0/src/general/FeatureSetOptions.py
--rw-rw-rw-   0        0        0    21204 2023-07-03 20:47:05.000000 OGDUtils-0.1.0/src/general/Workflow.py
--rw-rw-rw-   0        0        0        0 2023-06-30 18:02:29.000000 OGDUtils-0.1.0/src/general/__init__.py
--rw-rw-rw-   0        0        0    25380 2023-06-30 20:25:30.000000 OGDUtils-0.1.0/src/general/feature_utils.py
--rw-rw-rw-   0        0        0     3065 2023-06-30 20:25:43.000000 OGDUtils-0.1.0/src/general/import_utils.py
--rw-rw-rw-   0        0        0     4343 2023-06-30 17:47:12.000000 OGDUtils-0.1.0/src/general/ogd_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:31:00.031884 OGDUtils-0.1.1/
+-rw-rw-rw-   0        0        0     1117 2022-06-09 19:09:23.000000 OGDUtils-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1434 2023-07-04 14:31:00.031884 OGDUtils-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2023-06-30 19:27:15.000000 OGDUtils-0.1.1/README.md
+-rw-rw-rw-   0        0        0      697 2023-07-04 14:30:14.000000 OGDUtils-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 14:31:00.031884 OGDUtils-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.949756 OGDUtils-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.960530 OGDUtils-0.1.1/src/OGDUtils/
+drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.982488 OGDUtils-0.1.1/src/OGDUtils/JOWILDER/
+-rw-rw-rw-   0        0        0        0 2023-06-30 18:02:36.000000 OGDUtils-0.1.1/src/OGDUtils/JOWILDER/__init__.py
+-rw-rw-rw-   0        0        0    38315 2023-06-30 18:01:34.000000 OGDUtils-0.1.1/src/OGDUtils/JOWILDER/jowilder_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.987990 OGDUtils-0.1.1/src/OGDUtils/LAKELAND/
+-rw-rw-rw-   0        0        0        0 2023-06-30 18:02:44.000000 OGDUtils-0.1.1/src/OGDUtils/LAKELAND/__init__.py
+-rw-rw-rw-   0        0        0     8530 2023-06-30 18:01:31.000000 OGDUtils-0.1.1/src/OGDUtils/LAKELAND/lakeland_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.995861 OGDUtils-0.1.1/src/OGDUtils/WAVES/
+-rw-rw-rw-   0        0        0        0 2023-06-30 18:02:50.000000 OGDUtils-0.1.1/src/OGDUtils/WAVES/__init__.py
+-rw-rw-rw-   0        0        0     3758 2023-06-30 18:01:22.000000 OGDUtils-0.1.1/src/OGDUtils/WAVES/waves_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:31:00.031884 OGDUtils-0.1.1/src/OGDUtils/general/
+-rw-rw-rw-   0        0        0     1240 2023-06-30 17:47:12.000000 OGDUtils-0.1.1/src/OGDUtils/general/FeatureSetOptions.py
+-rw-rw-rw-   0        0        0    21204 2023-07-03 20:47:05.000000 OGDUtils-0.1.1/src/OGDUtils/general/Workflow.py
+-rw-rw-rw-   0        0        0        0 2023-06-30 18:02:29.000000 OGDUtils-0.1.1/src/OGDUtils/general/__init__.py
+-rw-rw-rw-   0        0        0    25380 2023-06-30 20:25:30.000000 OGDUtils-0.1.1/src/OGDUtils/general/feature_utils.py
+-rw-rw-rw-   0        0        0     3065 2023-06-30 20:25:43.000000 OGDUtils-0.1.1/src/OGDUtils/general/import_utils.py
+-rw-rw-rw-   0        0        0     4343 2023-06-30 17:47:12.000000 OGDUtils-0.1.1/src/OGDUtils/general/ogd_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.974300 OGDUtils-0.1.1/src/OGDUtils.egg-info/
+-rw-rw-rw-   0        0        0     1434 2023-07-04 14:30:59.000000 OGDUtils-0.1.1/src/OGDUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-07-04 14:30:59.000000 OGDUtils-0.1.1/src/OGDUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 14:30:59.000000 OGDUtils-0.1.1/src/OGDUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 14:30:59.000000 OGDUtils-0.1.1/src/OGDUtils.egg-info/top_level.txt
```

### Comparing `OGDUtils-0.1.0/LICENSE` & `OGDUtils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/PKG-INFO` & `OGDUtils-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OGDUtils
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package with utilities for working with output data from the Open Game Data core
 Author: John McCloskey
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/OGDUtils
 Project-URL: Bug Tracker, https://github.com/opengamedata/OGDUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OGDUtils-0.1.0/README.md` & `OGDUtils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/pyproject.toml` & `OGDUtils-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "OGDUtils"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
    { name="Luke Swanson", email="superscription58@gmail.com" },
    { name="John McCloskey" }
 ]
 description = "A package with utilities for working with output data from the Open Game Data core"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `OGDUtils-0.1.0/src/JOWILDER/jowilder_utils.py` & `OGDUtils-0.1.1/src/OGDUtils/JOWILDER/jowilder_utils.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/src/LAKELAND/lakeland_utils.py` & `OGDUtils-0.1.1/src/OGDUtils/LAKELAND/lakeland_utils.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/src/OGDUtils.egg-info/PKG-INFO` & `OGDUtils-0.1.1/src/OGDUtils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OGDUtils
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package with utilities for working with output data from the Open Game Data core
 Author: John McCloskey
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/OGDUtils
 Project-URL: Bug Tracker, https://github.com/opengamedata/OGDUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OGDUtils-0.1.0/src/WAVES/waves_utils.py` & `OGDUtils-0.1.1/src/OGDUtils/WAVES/waves_utils.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/src/general/FeatureSetOptions.py` & `OGDUtils-0.1.1/src/OGDUtils/general/FeatureSetOptions.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/src/general/Workflow.py` & `OGDUtils-0.1.1/src/OGDUtils/general/Workflow.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/src/general/feature_utils.py` & `OGDUtils-0.1.1/src/OGDUtils/general/feature_utils.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/src/general/import_utils.py` & `OGDUtils-0.1.1/src/OGDUtils/general/import_utils.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-0.1.0/src/general/ogd_utils.py` & `OGDUtils-0.1.1/src/OGDUtils/general/ogd_utils.py`

 * *Files identical despite different names*

