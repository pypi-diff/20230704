# Comparing `tmp/tah_data-1.1.0.tar.gz` & `tmp/tah_data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tah_data-1.1.0.tar", max compression
+gzip compressed data, was "tah_data-1.2.0.tar", max compression
```

## Comparing `tah_data-1.1.0.tar` & `tah_data-1.2.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      306 2023-07-03 11:44:01.875625 tah_data-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      564 2023-07-03 11:34:54.232946 tah_data-1.1.0/src/tah_data.py
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 tah_data-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      306 2023-07-04 13:12:48.650085 tah_data-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2934 2023-07-04 13:05:41.591737 tah_data-1.2.0/src/tah_data.py
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 tah_data-1.2.0/PKG-INFO
```

### Comparing `tah_data-1.1.0/PKG-INFO` & `tah_data-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tah-data
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: Ahmed Sherif
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

