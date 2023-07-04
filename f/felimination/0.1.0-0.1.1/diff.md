# Comparing `tmp/felimination-0.1.0.tar.gz` & `tmp/felimination-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felimination-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "felimination-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `felimination-0.1.0.tar` & `felimination-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-28 08:53:24.089466 felimination-0.1.0/felimination/__init__.py
--rw-r--r--   0        0        0     3863 2023-07-04 12:15:27.235064 felimination-0.1.0/felimination/importance.py
--rw-r--r--   0        0        0    31833 2023-07-04 12:45:51.804203 felimination-0.1.0/felimination/rfe.py
--rw-r--r--   0        0        0     1111 2023-07-04 12:55:28.906697 felimination-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 felimination-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2225 2023-07-04 13:44:43.576127 felimination-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 13:44:43.576127 felimination-0.1.1/felimination/__init__.py
+-rw-r--r--   0        0        0     3863 2023-07-04 13:44:43.576127 felimination-0.1.1/felimination/importance.py
+-rw-r--r--   0        0        0    31833 2023-07-04 13:44:43.576127 felimination-0.1.1/felimination/rfe.py
+-rw-r--r--   0        0        0     1344 2023-07-04 13:44:43.576127 felimination-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 felimination-0.1.1/PKG-INFO
```

### Comparing `felimination-0.1.0/felimination/importance.py` & `felimination-0.1.1/felimination/importance.py`

 * *Files identical despite different names*

### Comparing `felimination-0.1.0/felimination/rfe.py` & `felimination-0.1.1/felimination/rfe.py`

 * *Files identical despite different names*

### Comparing `felimination-0.1.0/pyproject.toml` & `felimination-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 [project]
 name = "felimination"
 description = "This library contains some useful scikit-learn compatible classes for feature selection."
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Claudio Salvatore Arcidiacono", email = "author@email.com" }
 ]
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
 
 dependencies = [
     "scikit-learn>=1.0.1,<2.0.0",
     "pandas>=1.1.1,<3.0.0",
     "seaborn>=0.11.1,<1.0.0",
 ]
 
@@ -21,14 +28,18 @@
     "pytest",
 ]
 doc = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]",
 ]
+build = [
+    "build",
+    "twine"
+]
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project.urls]
 "Homepage" = "https://github.com/ClaudioSalvatoreArcidiacono/felimination"
```

