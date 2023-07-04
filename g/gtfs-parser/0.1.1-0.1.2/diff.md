# Comparing `tmp/gtfs_parser-0.1.1.tar.gz` & `tmp/gtfs_parser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfs_parser-0.1.1.tar", max compression
+gzip compressed data, was "gtfs_parser-0.1.2.tar", max compression
```

## Comparing `gtfs_parser-0.1.1.tar` & `gtfs_parser-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1051 2023-07-04 11:19:04.015372 gtfs_parser-0.1.1/LICENSE
--rw-r--r--   0        0        0     1152 2023-07-04 11:19:04.015372 gtfs_parser-0.1.1/README.md
--rw-r--r--   0        0        0       54 2023-07-04 11:19:04.015372 gtfs_parser-0.1.1/gtfs_parser/__init__.py
--rw-r--r--   0        0        0     4198 2023-07-04 11:19:04.015372 gtfs_parser-0.1.1/gtfs_parser/__main__.py
--rw-r--r--   0        0        0    17228 2023-07-04 11:19:04.015372 gtfs_parser-0.1.1/gtfs_parser/aggregate.py
--rw-r--r--   0        0        0     1178 2023-07-04 11:19:04.015372 gtfs_parser-0.1.1/gtfs_parser/gtfs.py
--rw-r--r--   0        0        0     6135 2023-07-04 11:19:04.015372 gtfs_parser-0.1.1/gtfs_parser/parse.py
--rw-r--r--   0        0        0      529 2023-07-04 11:19:04.015372 gtfs_parser-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1732 1970-01-01 00:00:00.000000 gtfs_parser-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1051 2023-07-04 11:22:39.037953 gtfs_parser-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1152 2023-07-04 11:22:39.037953 gtfs_parser-0.1.2/README.md
+-rw-r--r--   0        0        0       54 2023-07-04 11:22:39.037953 gtfs_parser-0.1.2/gtfs_parser/__init__.py
+-rw-r--r--   0        0        0     4198 2023-07-04 11:22:39.037953 gtfs_parser-0.1.2/gtfs_parser/__main__.py
+-rw-r--r--   0        0        0    17228 2023-07-04 11:22:39.037953 gtfs_parser-0.1.2/gtfs_parser/aggregate.py
+-rw-r--r--   0        0        0     1178 2023-07-04 11:22:39.037953 gtfs_parser-0.1.2/gtfs_parser/gtfs.py
+-rw-r--r--   0        0        0     6135 2023-07-04 11:22:39.037953 gtfs_parser-0.1.2/gtfs_parser/parse.py
+-rw-r--r--   0        0        0      529 2023-07-04 11:22:39.037953 gtfs_parser-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1732 1970-01-01 00:00:00.000000 gtfs_parser-0.1.2/PKG-INFO
```

### Comparing `gtfs_parser-0.1.1/LICENSE` & `gtfs_parser-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.1/README.md` & `gtfs_parser-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.1/gtfs_parser/__main__.py` & `gtfs_parser-0.1.2/gtfs_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.1/gtfs_parser/aggregate.py` & `gtfs_parser-0.1.2/gtfs_parser/aggregate.py`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.1/gtfs_parser/gtfs.py` & `gtfs_parser-0.1.2/gtfs_parser/gtfs.py`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.1/gtfs_parser/parse.py` & `gtfs_parser-0.1.2/gtfs_parser/parse.py`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.1/pyproject.toml` & `gtfs_parser-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gtfs_parser"
-version = "0.1.1"
+version = "0.1.2"
 description = "parse and aggregate GTFS"
 authors = ["MIERUNE Inc.", "Kanahiro IGUCHI"]
 license = "MIT"
 homepage = "https://github.com/MIERUNE"
 repository = "https://github.com/MIERUNE/{project-name}"
 readme = "README.md"
 packages = [{include = "gtfs_parser"}]
@@ -15,8 +15,8 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-gtfs-parser = "gtfs_parser.__main__:main"
+gtfs_parser = "gtfs_parser.__main__:main"
```

### Comparing `gtfs_parser-0.1.1/PKG-INFO` & `gtfs_parser-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtfs-parser
-Version: 0.1.1
+Version: 0.1.2
 Summary: parse and aggregate GTFS
 Home-page: https://github.com/MIERUNE
 License: MIT
 Author: MIERUNE Inc.
 Requires-Python: >=3.7.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

