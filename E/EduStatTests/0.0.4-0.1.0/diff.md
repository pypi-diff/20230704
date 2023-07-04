# Comparing `tmp/EduStatTests-0.0.4.tar.gz` & `tmp/EduStatTests-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EduStatTests-0.0.4.tar", last modified: Sun Jul  2 13:21:22 2023, max compression
+gzip compressed data, was "EduStatTests-0.1.0.tar", last modified: Tue Jul  4 20:03:56 2023, max compression
```

## Comparing `EduStatTests-0.0.4.tar` & `EduStatTests-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 13:21:22.591949 EduStatTests-0.0.4/
--rw-rw-r--   0 hakan     (1000) hakan     (1000)     1070 2023-07-02 11:36:16.000000 EduStatTests-0.0.4/LICENSE
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      551 2023-07-02 13:21:22.587949 EduStatTests-0.0.4/PKG-INFO
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       79 2023-07-02 11:36:16.000000 EduStatTests-0.0.4/README.md
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      587 2023-07-02 13:21:09.000000 EduStatTests-0.0.4/pyproject.toml
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       38 2023-07-02 13:21:22.591949 EduStatTests-0.0.4/setup.cfg
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 13:21:22.587949 EduStatTests-0.0.4/src/
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 13:21:22.587949 EduStatTests-0.0.4/src/EduStatTests.egg-info/
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      551 2023-07-02 13:21:22.000000 EduStatTests-0.0.4/src/EduStatTests.egg-info/PKG-INFO
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      228 2023-07-02 13:21:22.000000 EduStatTests-0.0.4/src/EduStatTests.egg-info/SOURCES.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)        1 2023-07-02 13:21:22.000000 EduStatTests-0.0.4/src/EduStatTests.egg-info/dependency_links.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       22 2023-07-02 13:21:22.000000 EduStatTests-0.0.4/src/EduStatTests.egg-info/top_level.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)     1227 2023-07-02 13:19:19.000000 EduStatTests-0.0.4/src/EduStatTests.py
--rw-rw-r--   0 hakan     (1000) hakan     (1000)        0 2023-07-02 11:47:24.000000 EduStatTests-0.0.4/src/__init__.py
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:03:56.553835 EduStatTests-0.1.0/
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)     1070 2023-07-02 11:36:16.000000 EduStatTests-0.1.0/LICENSE
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-04 20:03:56.553835 EduStatTests-0.1.0/PKG-INFO
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       67 2023-07-03 20:02:42.000000 EduStatTests-0.1.0/README.md
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      587 2023-07-04 20:02:28.000000 EduStatTests-0.1.0/pyproject.toml
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       38 2023-07-04 20:03:56.553835 EduStatTests-0.1.0/setup.cfg
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:03:56.553835 EduStatTests-0.1.0/src/
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:03:56.553835 EduStatTests-0.1.0/src/EduStatTests.egg-info/
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-04 20:03:56.000000 EduStatTests-0.1.0/src/EduStatTests.egg-info/PKG-INFO
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      228 2023-07-04 20:03:56.000000 EduStatTests-0.1.0/src/EduStatTests.egg-info/SOURCES.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)        1 2023-07-04 20:03:56.000000 EduStatTests-0.1.0/src/EduStatTests.egg-info/dependency_links.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       22 2023-07-04 20:03:56.000000 EduStatTests-0.1.0/src/EduStatTests.egg-info/top_level.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)     2965 2023-07-04 19:55:22.000000 EduStatTests-0.1.0/src/EduStatTests.py
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)        0 2023-07-02 11:47:24.000000 EduStatTests-0.1.0/src/__init__.py
```

### Comparing `EduStatTests-0.0.4/LICENSE` & `EduStatTests-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EduStatTests-0.0.4/PKG-INFO` & `EduStatTests-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: EduStatTests
-Version: 0.0.4
+Version: 0.1.0
 Author-email: Hakan Güldal <hguldal@gmail.com>
 Project-URL: Homepage, https://github.com/hguldal/EduStatTests
 Project-URL: Bug Tracker, https://github.com/hguldal/EduStatTests/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EduStatTests
-Python library for statistical analysis in educational research
+Python package for educational statistical analysis
```

### Comparing `EduStatTests-0.0.4/pyproject.toml` & `EduStatTests-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy; python_version>='3.12'"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EduStatTests"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="Hakan Güldal", email="hguldal@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `EduStatTests-0.0.4/src/EduStatTests.egg-info/PKG-INFO` & `EduStatTests-0.1.0/src/EduStatTests.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: EduStatTests
-Version: 0.0.4
+Version: 0.1.0
 Author-email: Hakan Güldal <hguldal@gmail.com>
 Project-URL: Homepage, https://github.com/hguldal/EduStatTests
 Project-URL: Bug Tracker, https://github.com/hguldal/EduStatTests/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EduStatTests
-Python library for statistical analysis in educational research
+Python package for educational statistical analysis
```

