# Comparing `tmp/khala_python_utils-0.0.3.tar.gz` & `tmp/khala_python_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khala_python_utils-0.0.3.tar", max compression
+gzip compressed data, was "khala_python_utils-0.0.4.tar", max compression
```

## Comparing `khala_python_utils-0.0.3.tar` & `khala_python_utils-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      622 2023-04-25 13:46:14.372944 khala_python_utils-0.0.3/http_request/__init__.py
--rw-r--r--   0        0        0    11558 2023-04-11 14:04:49.208986 khala_python_utils-0.0.3/LICENSE
--rw-r--r--   0        0        0      470 2023-07-04 03:16:47.337651 khala_python_utils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-11 14:04:49.208986 khala_python_utils-0.0.3/README.md
--rw-r--r--   0        0        0      294 2023-04-27 02:20:28.671526 khala_python_utils-0.0.3/syntax/__init__.py
--rw-r--r--   0        0        0      311 2023-07-04 03:13:16.166966 khala_python_utils-0.0.3/syntax/fs.py
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 khala_python_utils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      622 2023-04-25 13:46:14.372944 khala_python_utils-0.0.4/http_request/__init__.py
+-rw-r--r--   0        0        0    11558 2023-04-11 14:04:49.208986 khala_python_utils-0.0.4/LICENSE
+-rw-r--r--   0        0        0      470 2023-07-04 04:42:49.422395 khala_python_utils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-11 14:04:49.208986 khala_python_utils-0.0.4/README.md
+-rw-r--r--   0        0        0      294 2023-04-27 02:20:28.671526 khala_python_utils-0.0.4/syntax/__init__.py
+-rw-r--r--   0        0        0      439 2023-07-04 04:42:14.578361 khala_python_utils-0.0.4/syntax/fs.py
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 khala_python_utils-0.0.4/PKG-INFO
```

### Comparing `khala_python_utils-0.0.3/http_request/__init__.py` & `khala_python_utils-0.0.4/http_request/__init__.py`

 * *Files identical despite different names*

### Comparing `khala_python_utils-0.0.3/LICENSE` & `khala_python_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

