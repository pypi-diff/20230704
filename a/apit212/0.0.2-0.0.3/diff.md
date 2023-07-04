# Comparing `tmp/apit212-0.0.2.tar.gz` & `tmp/apit212-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-0.0.2.tar", last modified: Mon Jul  3 22:41:18 2023, max compression
+gzip compressed data, was "apit212-0.0.3.tar", last modified: Tue Jul  4 00:43:10 2023, max compression
```

## Comparing `apit212-0.0.2.tar` & `apit212-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 22:41:18.494489 apit212-0.0.2/
--rw-rw-rw-   0        0        0     1083 2023-07-03 22:40:45.000000 apit212-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     6763 2023-07-03 22:41:18.491497 apit212-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6254 2023-07-03 22:40:44.000000 apit212-0.0.2/README.md
--rw-rw-rw-   0        0        0      593 2023-07-03 22:40:40.000000 apit212-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 22:41:18.496484 apit212-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 22:41:18.356827 apit212-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 22:41:18.433021 apit212-0.0.2/src/apit212/
--rw-rw-rw-   0        0        0       47 2023-07-03 22:40:37.000000 apit212-0.0.2/src/apit212/__init__.py
--rw-rw-rw-   0        0        0    17825 2023-07-03 22:40:39.000000 apit212-0.0.2/src/apit212/apit212.py
--rw-rw-rw-   0        0        0     1250 2023-07-03 22:40:42.000000 apit212-0.0.2/src/apit212/constant.py
-drwxrwxrwx   0        0        0        0 2023-07-03 22:41:18.489502 apit212-0.0.2/src/apit212.egg-info/
--rw-rw-rw-   0        0        0     6763 2023-07-03 22:41:18.000000 apit212-0.0.2/src/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-03 22:41:18.000000 apit212-0.0.2/src/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 22:41:18.000000 apit212-0.0.2/src/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 22:41:18.000000 apit212-0.0.2/src/apit212.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 00:43:10.746127 apit212-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-07-03 22:40:45.000000 apit212-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6963 2023-07-04 00:43:10.746127 apit212-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6254 2023-07-03 22:40:44.000000 apit212-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 00:43:10.741531 apit212-0.0.3/apit212.egg-info/
+-rw-rw-rw-   0        0        0     6963 2023-07-04 00:43:10.000000 apit212-0.0.3/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-07-04 00:43:10.000000 apit212-0.0.3/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 00:43:10.000000 apit212-0.0.3/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 00:43:10.000000 apit212-0.0.3/apit212.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      593 2023-07-04 00:23:46.000000 apit212-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 00:43:10.746127 apit212-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-07-04 00:23:37.000000 apit212-0.0.3/setup.py
```

### Comparing `apit212-0.0.2/LICENSE` & `apit212-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-0.0.2/PKG-INFO` & `apit212-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial trading212 API
+Home-page: https://github.com/Flock92/aPit212
+Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
+License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
 Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
+Keywords: trading apipython3trading212API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires: requests
+Requires: selenium
+Requires: getpass
+Requires: constant
 Requires-Python: >=3.10.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Apit212
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212. Please note that either myself or trading212 take responsibility for the use of this API.
```

### Comparing `apit212-0.0.2/README.md` & `apit212-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `apit212-0.0.2/pyproject.toml` & `apit212-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Flock92", email="stuwe_3000@outlook.com" },
 ]
 
 description = "Unofficial trading212 API"
 readme = "README.md"
 requires-python = ">=3.10.11"
```

### Comparing `apit212-0.0.2/src/apit212.egg-info/PKG-INFO` & `apit212-0.0.3/apit212.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial trading212 API
+Home-page: https://github.com/Flock92/aPit212
+Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
+License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
 Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
+Keywords: trading apipython3trading212API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires: requests
+Requires: selenium
+Requires: getpass
+Requires: constant
 Requires-Python: >=3.10.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Apit212
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212. Please note that either myself or trading212 take responsibility for the use of this API.
```

