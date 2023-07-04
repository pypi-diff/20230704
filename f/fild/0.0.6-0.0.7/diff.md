# Comparing `tmp/fild-0.0.6.tar.gz` & `tmp/fild-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fild-0.0.6.tar", last modified: Wed Oct 26 15:13:04 2022, max compression
+gzip compressed data, was "fild-0.0.7.tar", last modified: Tue Jul  4 15:41:13 2023, max compression
```

## Comparing `fild-0.0.6.tar` & `fild-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:13:04.087681 fild-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-26 15:12:50.000000 fild-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-10-26 15:13:04.087681 fild-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-10-26 15:12:50.000000 fild-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-26 15:12:50.000000 fild-0.0.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      699 2022-10-26 15:13:04.087681 fild-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:13:04.083681 fild-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:13:04.083681 fild-0.0.6/src/fild/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:13:04.087681 fild-0.0.6/src/fild/process/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/process/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2568 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/process/common.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11279 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/process/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:13:04.087681 fild-0.0.6/src/fild/sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2610 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/sdk/array.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1206 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/sdk/dates.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5019 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/sdk/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)     4176 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/sdk/fakeable.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2205 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/sdk/field.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5118 2022-10-26 15:12:50.000000 fild-0.0.6/src/fild/sdk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:13:04.087681 fild-0.0.6/src/fild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-10-26 15:13:04.000000 fild-0.0.6/src/fild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-10-26 15:13:04.000000 fild-0.0.6/src/fild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 15:13:04.000000 fild-0.0.6/src/fild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-26 15:13:04.000000 fild-0.0.6/src/fild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-26 15:13:04.000000 fild-0.0.6/src/fild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:13.507111 fild-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-04 15:41:02.000000 fild-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-04 15:41:13.507111 fild-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-04 15:41:02.000000 fild-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 15:41:02.000000 fild-0.0.7/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-07-04 15:41:13.507111 fild-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:13.503111 fild-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:13.503111 fild-0.0.7/src/fild/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:13.507111 fild-0.0.7/src/fild/process/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/process/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2568 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/process/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11304 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/process/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:13.507111 fild-0.0.7/src/fild/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2610 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/sdk/array.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/sdk/dates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5019 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/sdk/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/sdk/fakeable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2205 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/sdk/field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5118 2023-07-04 15:41:02.000000 fild-0.0.7/src/fild/sdk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:13.507111 fild-0.0.7/src/fild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-04 15:41:13.000000 fild-0.0.7/src/fild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-04 15:41:13.000000 fild-0.0.7/src/fild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:41:13.000000 fild-0.0.7/src/fild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 15:41:13.000000 fild-0.0.7/src/fild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 15:41:13.000000 fild-0.0.7/src/fild.egg-info/top_level.txt
```

### Comparing `fild-0.0.6/LICENSE` & `fild-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/PKG-INFO` & `fild-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fild
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to describe contracts and generate data
 Home-page: https://github.com/elenakulgavaya/fild
 Author: Elena Kulgavaya
 Author-email: elena.kulgavaya@gmail.com
 Project-URL: Bug Tracker, https://github.com/elenakulgavaya/fild/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fild-0.0.6/README.md` & `fild-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/setup.cfg` & `fild-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fild
-version = 0.0.6
+version = 0.0.7
 author = Elena Kulgavaya
 author_email = elena.kulgavaya@gmail.com
 description = Library to describe contracts and generate data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/elenakulgavaya/fild
 project_urls =
```

### Comparing `fild-0.0.6/src/fild/process/common.py` & `fild-0.0.7/src/fild/process/common.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/src/fild/process/dictionary.py` & `fild-0.0.7/src/fild/process/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         if element not in target:
             return len(target)
 
         return target.index(element)
 
     initial = copy.deepcopy(actual)
 
-    if isinstance(initial, list):
+    if isinstance(initial, list) and expected is not None:
         element_key = find_key(initial[0]) if initial else None
         initial = sorted(
             initial,
             key=lambda x: get_index(expected, x, element_key=element_key)
         )
         if len(initial) == len(expected):
             for num, _ in enumerate(initial):
```

### Comparing `fild-0.0.6/src/fild/sdk/array.py` & `fild-0.0.7/src/fild/sdk/array.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/src/fild/sdk/dates.py` & `fild-0.0.7/src/fild/sdk/dates.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/src/fild/sdk/dictionary.py` & `fild-0.0.7/src/fild/sdk/dictionary.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/src/fild/sdk/fakeable.py` & `fild-0.0.7/src/fild/sdk/fakeable.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/src/fild/sdk/field.py` & `fild-0.0.7/src/fild/sdk/field.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/src/fild/sdk/types.py` & `fild-0.0.7/src/fild/sdk/types.py`

 * *Files identical despite different names*

### Comparing `fild-0.0.6/src/fild.egg-info/PKG-INFO` & `fild-0.0.7/src/fild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fild
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to describe contracts and generate data
 Home-page: https://github.com/elenakulgavaya/fild
 Author: Elena Kulgavaya
 Author-email: elena.kulgavaya@gmail.com
 Project-URL: Bug Tracker, https://github.com/elenakulgavaya/fild/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

