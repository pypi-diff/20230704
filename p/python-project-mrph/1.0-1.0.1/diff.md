# Comparing `tmp/python-project-mrph-1.0.tar.gz` & `tmp/python_project_mrph-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-mrph-1.0.tar", last modified: Tue Jul  4 16:40:05 2023, max compression
+gzip compressed data, was "python_project_mrph-1.0.1.tar", last modified: Tue Jul  4 17:30:18 2023, max compression
```

## Comparing `python-project-mrph-1.0.tar` & `python_project_mrph-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maggie.hunt   (502) staff       (20)        0 2023-07-04 16:40:05.087668 python-project-mrph-1.0/
--rw-r--r--   0 maggie.hunt   (502) staff       (20)     1068 2023-07-04 15:42:10.000000 python-project-mrph-1.0/LICENSE.txt
--rw-r--r--   0 maggie.hunt   (502) staff       (20)      616 2023-07-04 16:40:05.087937 python-project-mrph-1.0/PKG-INFO
--rw-r--r--   0 maggie.hunt   (502) staff       (20)      103 2023-07-03 15:55:17.000000 python-project-mrph-1.0/README.md
-drwxr-xr-x   0 maggie.hunt   (502) staff       (20)        0 2023-07-04 16:40:05.079841 python-project-mrph-1.0/python-project-mrph/
--rw-r--r--   0 maggie.hunt   (502) staff       (20)        0 2023-07-04 16:14:19.000000 python-project-mrph-1.0/python-project-mrph/__init__.py
-drwxr-xr-x   0 maggie.hunt   (502) staff       (20)        0 2023-07-04 16:40:05.086656 python-project-mrph-1.0/python_project_mrph.egg-info/
--rw-r--r--   0 maggie.hunt   (502) staff       (20)      616 2023-07-04 16:40:04.000000 python-project-mrph-1.0/python_project_mrph.egg-info/PKG-INFO
--rw-r--r--   0 maggie.hunt   (502) staff       (20)      286 2023-07-04 16:40:05.000000 python-project-mrph-1.0/python_project_mrph.egg-info/SOURCES.txt
--rw-r--r--   0 maggie.hunt   (502) staff       (20)        1 2023-07-04 16:40:04.000000 python-project-mrph-1.0/python_project_mrph.egg-info/dependency_links.txt
--rw-r--r--   0 maggie.hunt   (502) staff       (20)       78 2023-07-04 16:40:04.000000 python-project-mrph-1.0/python_project_mrph.egg-info/requires.txt
--rw-r--r--   0 maggie.hunt   (502) staff       (20)       20 2023-07-04 16:40:04.000000 python-project-mrph-1.0/python_project_mrph.egg-info/top_level.txt
--rw-r--r--   0 maggie.hunt   (502) staff       (20)       79 2023-07-04 16:40:05.089301 python-project-mrph-1.0/setup.cfg
--rw-r--r--   0 maggie.hunt   (502) staff       (20)      838 2023-07-04 16:06:33.000000 python-project-mrph-1.0/setup.py
+drwxr-xr-x   0 maggie.hunt   (502) staff       (20)        0 2023-07-04 17:30:18.748301 python_project_mrph-1.0.1/
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)     1068 2023-07-04 15:42:10.000000 python_project_mrph-1.0.1/LICENSE.txt
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)      618 2023-07-04 17:30:18.748498 python_project_mrph-1.0.1/PKG-INFO
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)      103 2023-07-03 15:55:17.000000 python_project_mrph-1.0.1/README.md
+drwxr-xr-x   0 maggie.hunt   (502) staff       (20)        0 2023-07-04 17:30:18.742923 python_project_mrph-1.0.1/python_project_mrph/
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)        0 2023-07-04 16:14:19.000000 python_project_mrph-1.0.1/python_project_mrph/__init__.py
+drwxr-xr-x   0 maggie.hunt   (502) staff       (20)        0 2023-07-04 17:30:18.747549 python_project_mrph-1.0.1/python_project_mrph.egg-info/
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)      618 2023-07-04 17:30:18.000000 python_project_mrph-1.0.1/python_project_mrph.egg-info/PKG-INFO
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)      286 2023-07-04 17:30:18.000000 python_project_mrph-1.0.1/python_project_mrph.egg-info/SOURCES.txt
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)        1 2023-07-04 17:30:18.000000 python_project_mrph-1.0.1/python_project_mrph.egg-info/dependency_links.txt
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)       78 2023-07-04 17:30:18.000000 python_project_mrph-1.0.1/python_project_mrph.egg-info/requires.txt
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)       20 2023-07-04 17:30:18.000000 python_project_mrph-1.0.1/python_project_mrph.egg-info/top_level.txt
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)       79 2023-07-04 17:30:18.749473 python_project_mrph-1.0.1/setup.cfg
+-rw-r--r--   0 maggie.hunt   (502) staff       (20)      840 2023-07-04 17:28:25.000000 python_project_mrph-1.0.1/setup.py
```

### Comparing `python-project-mrph-1.0/LICENSE.txt` & `python_project_mrph-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-project-mrph-1.0/PKG-INFO` & `python_project_mrph-1.0.1/python_project_mrph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-project-mrph
-Version: 1.0
+Version: 1.0.1
 Summary: python example package
 Home-page: https://github.com/maggiehuntpa/python-project-mrph.git
 Author: MRPH
 Author-email: maggie.hunt@paconsulting.com
 License: UNKNOWN
 Download-URL: https://github.com/maggiehuntpa/python-project-mrph/archive/refs/tags/Python.tar.gz
 Description: UNKNOWN
```

### Comparing `python-project-mrph-1.0/python_project_mrph.egg-info/PKG-INFO` & `python_project_mrph-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: python-project-mrph
-Version: 1.0
+Name: python_project_mrph
+Version: 1.0.1
 Summary: python example package
 Home-page: https://github.com/maggiehuntpa/python-project-mrph.git
 Author: MRPH
 Author-email: maggie.hunt@paconsulting.com
 License: UNKNOWN
 Download-URL: https://github.com/maggiehuntpa/python-project-mrph/archive/refs/tags/Python.tar.gz
 Description: UNKNOWN
```

### Comparing `python-project-mrph-1.0/setup.py` & `python_project_mrph-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 
 setup(
-    name="python-project-mrph",
-    version="1.0",
+    name="python_project_mrph",
+    version="1.0.1",
     author="MRPH",
     author_email="maggie.hunt@paconsulting.com",
     description="python example package",
     url="https://github.com/maggiehuntpa/python-project-mrph.git",
     download_url='https://github.com/maggiehuntpa/python-project-mrph/archive/refs/tags/Python.tar.gz',
-    packages=["python-project-mrph"],
+    packages=["python_project_mrph"],
     install_requires=[
         "certifi>=2023.5",
         "charset-normalizer>=3.1",
         "idna>=3.4",
         "requests>=2.31",
         "urllib3>=2.0"
     ],
```

