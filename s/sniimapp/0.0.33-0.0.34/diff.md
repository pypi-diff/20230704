# Comparing `tmp/sniimapp-0.0.33.tar.gz` & `tmp/sniimapp-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp-0.0.33.tar", last modified: Sun Jul  2 06:32:55 2023, max compression
+gzip compressed data, was "sniimapp-0.0.34.tar", last modified: Tue Jul  4 16:16:47 2023, max compression
```

## Comparing `sniimapp-0.0.33.tar` & `sniimapp-0.0.34.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 06:32:55.356493 sniimapp-0.0.33/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.33/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-02 06:32:55.356493 sniimapp-0.0.33/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1163 2023-07-02 06:32:13.000000 sniimapp-0.0.33/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-02 06:32:33.000000 sniimapp-0.0.33/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 06:32:55.356493 sniimapp-0.0.33/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 06:32:55.356493 sniimapp-0.0.33/sniimapp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-02 06:32:55.000000 sniimapp-0.0.33/sniimapp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-07-02 06:32:55.000000 sniimapp-0.0.33/sniimapp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 06:32:55.000000 sniimapp-0.0.33/sniimapp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 06:32:55.000000 sniimapp-0.0.33/sniimapp.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-07-02 06:18:38.000000 sniimapp-0.0.33/sniimapp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 16:16:47.891988 sniimapp-0.0.34/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.34/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-04 16:16:47.891988 sniimapp-0.0.34/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1163 2023-07-02 06:32:13.000000 sniimapp-0.0.34/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-04 16:16:10.000000 sniimapp-0.0.34/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-04 16:16:47.891988 sniimapp-0.0.34/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 16:16:47.891988 sniimapp-0.0.34/sniimapp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-04 16:16:47.000000 sniimapp-0.0.34/sniimapp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-07-04 16:16:47.000000 sniimapp-0.0.34/sniimapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-04 16:16:47.000000 sniimapp-0.0.34/sniimapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-04 16:16:47.000000 sniimapp-0.0.34/sniimapp.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-07-02 06:18:38.000000 sniimapp-0.0.34/sniimapp.py
```

### Comparing `sniimapp-0.0.33/LICENSE` & `sniimapp-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.33/PKG-INFO` & `sniimapp-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.33
+Version: 0.0.34
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.33/README.md` & `sniimapp-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.33/pyproject.toml` & `sniimapp-0.0.34/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sniimapp"
-version = "0.0.33"
+version = "0.0.34"
 authors = [
   { name="Rodolfo Lopez", email="1803672F@umich.mx" },
 ]
 description = "Libreria para extraccion de precios SNIIM"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sniimapp-0.0.33/sniimapp.egg-info/PKG-INFO` & `sniimapp-0.0.34/sniimapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.33
+Version: 0.0.34
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.33/sniimapp.py` & `sniimapp-0.0.34/sniimapp.py`

 * *Files identical despite different names*

