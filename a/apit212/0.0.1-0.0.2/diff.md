# Comparing `tmp/apit212-0.0.1.tar.gz` & `tmp/apit212-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-0.0.1.tar", last modified: Mon Jul  3 21:10:45 2023, max compression
+gzip compressed data, was "apit212-0.0.2.tar", last modified: Mon Jul  3 22:41:18 2023, max compression
```

## Comparing `apit212-0.0.1.tar` & `apit212-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 21:10:45.960887 apit212-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-07-03 21:06:14.000000 apit212-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6759 2023-07-03 21:10:45.958655 apit212-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6254 2023-07-03 21:05:54.000000 apit212-0.0.1/README.md
--rw-rw-rw-   0        0        0      585 2023-07-03 21:10:00.000000 apit212-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 21:10:45.961893 apit212-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 21:10:45.674661 apit212-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 21:10:45.818991 apit212-0.0.1/src/apit212/
--rw-rw-rw-   0        0        0        0 2023-07-03 20:55:53.000000 apit212-0.0.1/src/apit212/__init__.py
--rw-rw-rw-   0        0        0    17825 2023-07-03 21:01:19.000000 apit212-0.0.1/src/apit212/apit212.py
--rw-rw-rw-   0        0        0     1250 2023-07-03 20:59:11.000000 apit212-0.0.1/src/apit212/constant.py
-drwxrwxrwx   0        0        0        0 2023-07-03 21:10:45.955194 apit212-0.0.1/src/apit212.egg-info/
--rw-rw-rw-   0        0        0     6759 2023-07-03 21:10:45.000000 apit212-0.0.1/src/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-03 21:10:45.000000 apit212-0.0.1/src/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 21:10:45.000000 apit212-0.0.1/src/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 21:10:45.000000 apit212-0.0.1/src/apit212.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 22:41:18.494489 apit212-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-07-03 22:40:45.000000 apit212-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6763 2023-07-03 22:41:18.491497 apit212-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6254 2023-07-03 22:40:44.000000 apit212-0.0.2/README.md
+-rw-rw-rw-   0        0        0      593 2023-07-03 22:40:40.000000 apit212-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 22:41:18.496484 apit212-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 22:41:18.356827 apit212-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 22:41:18.433021 apit212-0.0.2/src/apit212/
+-rw-rw-rw-   0        0        0       47 2023-07-03 22:40:37.000000 apit212-0.0.2/src/apit212/__init__.py
+-rw-rw-rw-   0        0        0    17825 2023-07-03 22:40:39.000000 apit212-0.0.2/src/apit212/apit212.py
+-rw-rw-rw-   0        0        0     1250 2023-07-03 22:40:42.000000 apit212-0.0.2/src/apit212/constant.py
+drwxrwxrwx   0        0        0        0 2023-07-03 22:41:18.489502 apit212-0.0.2/src/apit212.egg-info/
+-rw-rw-rw-   0        0        0     6763 2023-07-03 22:41:18.000000 apit212-0.0.2/src/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-03 22:41:18.000000 apit212-0.0.2/src/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 22:41:18.000000 apit212-0.0.2/src/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 22:41:18.000000 apit212-0.0.2/src/apit212.egg-info/top_level.txt
```

### Comparing `apit212-0.0.1/LICENSE` & `apit212-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-0.0.1/PKG-INFO` & `apit212-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial trading212 API
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Project-URL: Homepage, https://github.com/Flock92/apit212
 Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Apit212
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212. Please note that either myself or trading212 take responsibility for the use of this API.
```

### Comparing `apit212-0.0.1/README.md` & `apit212-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `apit212-0.0.1/pyproject.toml` & `apit212-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Flock92", email="stuwe_3000@outlook.com" },
 ]
+
 description = "Unofficial trading212 API"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10.11"
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `apit212-0.0.1/src/apit212/apit212.py` & `apit212-0.0.2/src/apit212/apit212.py`

 * *Files identical despite different names*

### Comparing `apit212-0.0.1/src/apit212/constant.py` & `apit212-0.0.2/src/apit212/constant.py`

 * *Files identical despite different names*

### Comparing `apit212-0.0.1/src/apit212.egg-info/PKG-INFO` & `apit212-0.0.2/src/apit212.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial trading212 API
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Project-URL: Homepage, https://github.com/Flock92/apit212
 Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Apit212
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212. Please note that either myself or trading212 take responsibility for the use of this API.
```

