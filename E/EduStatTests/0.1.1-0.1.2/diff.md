# Comparing `tmp/EduStatTests-0.1.1.tar.gz` & `tmp/EduStatTests-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EduStatTests-0.1.1.tar", last modified: Tue Jul  4 20:11:16 2023, max compression
+gzip compressed data, was "EduStatTests-0.1.2.tar", last modified: Tue Jul  4 20:15:42 2023, max compression
```

## Comparing `EduStatTests-0.1.1.tar` & `EduStatTests-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:11:16.818737 EduStatTests-0.1.1/
--rw-rw-r--   0 hakan     (1000) hakan     (1000)     1070 2023-07-02 11:36:16.000000 EduStatTests-0.1.1/LICENSE
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-04 20:11:16.818737 EduStatTests-0.1.1/PKG-INFO
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       67 2023-07-03 20:02:42.000000 EduStatTests-0.1.1/README.md
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      587 2023-07-04 20:10:38.000000 EduStatTests-0.1.1/pyproject.toml
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       38 2023-07-04 20:11:16.818737 EduStatTests-0.1.1/setup.cfg
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:11:16.814737 EduStatTests-0.1.1/src/
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:11:16.818737 EduStatTests-0.1.1/src/EduStatTests.egg-info/
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-04 20:11:16.000000 EduStatTests-0.1.1/src/EduStatTests.egg-info/PKG-INFO
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      228 2023-07-04 20:11:16.000000 EduStatTests-0.1.1/src/EduStatTests.egg-info/SOURCES.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)        1 2023-07-04 20:11:16.000000 EduStatTests-0.1.1/src/EduStatTests.egg-info/dependency_links.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       22 2023-07-04 20:11:16.000000 EduStatTests-0.1.1/src/EduStatTests.egg-info/top_level.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)     3001 2023-07-04 20:10:27.000000 EduStatTests-0.1.1/src/EduStatTests.py
--rw-rw-r--   0 hakan     (1000) hakan     (1000)        0 2023-07-02 11:47:24.000000 EduStatTests-0.1.1/src/__init__.py
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:15:42.289446 EduStatTests-0.1.2/
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)     1070 2023-07-02 11:36:16.000000 EduStatTests-0.1.2/LICENSE
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-04 20:15:42.289446 EduStatTests-0.1.2/PKG-INFO
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       67 2023-07-03 20:02:42.000000 EduStatTests-0.1.2/README.md
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      587 2023-07-04 20:13:29.000000 EduStatTests-0.1.2/pyproject.toml
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       38 2023-07-04 20:15:42.289446 EduStatTests-0.1.2/setup.cfg
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:15:42.285447 EduStatTests-0.1.2/src/
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:15:42.289446 EduStatTests-0.1.2/src/EduStatTests.egg-info/
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-04 20:15:42.000000 EduStatTests-0.1.2/src/EduStatTests.egg-info/PKG-INFO
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      228 2023-07-04 20:15:42.000000 EduStatTests-0.1.2/src/EduStatTests.egg-info/SOURCES.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)        1 2023-07-04 20:15:42.000000 EduStatTests-0.1.2/src/EduStatTests.egg-info/dependency_links.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       22 2023-07-04 20:15:42.000000 EduStatTests-0.1.2/src/EduStatTests.egg-info/top_level.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)     3001 2023-07-04 20:13:16.000000 EduStatTests-0.1.2/src/EduStatTests.py
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)        0 2023-07-02 11:47:24.000000 EduStatTests-0.1.2/src/__init__.py
```

### Comparing `EduStatTests-0.1.1/LICENSE` & `EduStatTests-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EduStatTests-0.1.1/PKG-INFO` & `EduStatTests-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduStatTests
-Version: 0.1.1
+Version: 0.1.2
 Author-email: Hakan Güldal <hguldal@gmail.com>
 Project-URL: Homepage, https://github.com/hguldal/EduStatTests
 Project-URL: Bug Tracker, https://github.com/hguldal/EduStatTests/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `EduStatTests-0.1.1/pyproject.toml` & `EduStatTests-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy; python_version>='3.12'"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EduStatTests"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Hakan Güldal", email="hguldal@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `EduStatTests-0.1.1/src/EduStatTests.egg-info/PKG-INFO` & `EduStatTests-0.1.2/src/EduStatTests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduStatTests
-Version: 0.1.1
+Version: 0.1.2
 Author-email: Hakan Güldal <hguldal@gmail.com>
 Project-URL: Homepage, https://github.com/hguldal/EduStatTests
 Project-URL: Bug Tracker, https://github.com/hguldal/EduStatTests/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `EduStatTests-0.1.1/src/EduStatTests.py` & `EduStatTests-0.1.2/src/EduStatTests.py`

 * *Files identical despite different names*

