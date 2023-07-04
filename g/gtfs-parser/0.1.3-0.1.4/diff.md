# Comparing `tmp/gtfs_parser-0.1.3.tar.gz` & `tmp/gtfs_parser-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfs_parser-0.1.3.tar", max compression
+gzip compressed data, was "gtfs_parser-0.1.4.tar", max compression
```

## Comparing `gtfs_parser-0.1.3.tar` & `gtfs_parser-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1051 2023-07-04 13:21:36.031730 gtfs_parser-0.1.3/LICENSE
--rw-r--r--   0        0        0     1183 2023-07-04 13:21:36.031730 gtfs_parser-0.1.3/README.md
--rw-r--r--   0        0        0       54 2023-07-04 13:21:36.031730 gtfs_parser-0.1.3/gtfs_parser/__init__.py
--rw-r--r--   0        0        0     4198 2023-07-04 13:21:36.035730 gtfs_parser-0.1.3/gtfs_parser/__main__.py
--rw-r--r--   0        0        0    17228 2023-07-04 13:21:36.035730 gtfs_parser-0.1.3/gtfs_parser/aggregate.py
--rw-r--r--   0        0        0     1178 2023-07-04 13:21:36.035730 gtfs_parser-0.1.3/gtfs_parser/gtfs.py
--rw-r--r--   0        0        0     6135 2023-07-04 13:21:36.035730 gtfs_parser-0.1.3/gtfs_parser/parse.py
--rw-r--r--   0        0        0      529 2023-07-04 13:21:36.035730 gtfs_parser-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 gtfs_parser-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1051 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1143 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/README.md
+-rw-r--r--   0        0        0       54 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/__init__.py
+-rw-r--r--   0        0        0     4198 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/__main__.py
+-rw-r--r--   0        0        0    17228 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/aggregate.py
+-rw-r--r--   0        0        0     1178 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/gtfs.py
+-rw-r--r--   0        0        0     6135 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/parse.py
+-rw-r--r--   0        0        0      529 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 gtfs_parser-0.1.4/PKG-INFO
```

### Comparing `gtfs_parser-0.1.3/LICENSE` & `gtfs_parser-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.3/README.md` & `gtfs_parser-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## API
 
 TODO
 
 ## CLI
 
 ```
-usage: __main__.py [-h] [--parse_ignoreshapes] [--parse_ignorenoroute]
+usage: gtfs-parser [-h] [--parse_ignoreshapes] [--parse_ignorenoroute]
                    [--aggregate_yyyymmdd AGGREGATE_YYYYMMDD]
                    [--aggregate_nounifystops]
                    [--aggregate_delimiter AGGREGATE_DELIMITER]
                    [--aggregate_begintime AGGREGATE_BEGINTIME]
                    [--aggregate_endtime AGGREGATE_ENDTIME]
                    mode src dst
 
@@ -40,12 +40,12 @@
   --aggregate_begintime AGGREGATE_BEGINTIME
   --aggregate_endtime AGGREGATE_ENDTIME
 ```
 
 ### Example
 
 ```sh
-python -m gtfs-parser parse gtfs.zip output
-python -m gtfs-parser parse gtfs_dir output --parse_ignoreshapes
-python -m gtfs-parser aggregate gtfs.zip output
-python -m gtfs-parser aggregate gtfs_dir output --aggregate_nounifystops
+gtfs-parser parse gtfs.zip output
+gtfs-parser parse gtfs_dir output --parse_ignoreshapes
+gtfs-parser aggregate gtfs.zip output
+gtfs-parser aggregate gtfs_dir output --aggregate_nounifystops
 ```
```

### Comparing `gtfs_parser-0.1.3/gtfs_parser/__main__.py` & `gtfs_parser-0.1.4/gtfs_parser/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     if args.src.endswith(".zip"):  # TODO: wiser checking
         print("extracting zipfile...")
         temp_dir = os.path.join(tempfile.gettempdir(), "gtfs_parser")
         if os.path.exists(temp_dir):
             shutil.rmtree(temp_dir)
         os.mkdir(temp_dir)
-        with zipfile.ZipFile(args.zip) as z:
+        with zipfile.ZipFile(args.src) as z:
             z.extractall(temp_dir)
         output_dir = temp_dir
     else:
         output_dir = args.src
 
     gtfs = GTFS(output_dir)
     print("GTFS loaded.")
```

### Comparing `gtfs_parser-0.1.3/gtfs_parser/aggregate.py` & `gtfs_parser-0.1.4/gtfs_parser/aggregate.py`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.3/gtfs_parser/gtfs.py` & `gtfs_parser-0.1.4/gtfs_parser/gtfs.py`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.3/gtfs_parser/parse.py` & `gtfs_parser-0.1.4/gtfs_parser/parse.py`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.3/pyproject.toml` & `gtfs_parser-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gtfs_parser"
-version = "0.1.3"
+version = "0.1.4"
 description = "parse and aggregate GTFS"
 authors = ["MIERUNE Inc.", "Kanahiro IGUCHI"]
 license = "MIT"
 homepage = "https://github.com/MIERUNE"
 repository = "https://github.com/MIERUNE/{project-name}"
 readme = "README.md"
 packages = [{include = "gtfs_parser"}]
```

### Comparing `gtfs_parser-0.1.3/PKG-INFO` & `gtfs_parser-0.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtfs-parser
-Version: 0.1.3
+Version: 0.1.4
 Summary: parse and aggregate GTFS
 Home-page: https://github.com/MIERUNE
 License: MIT
 Author: MIERUNE Inc.
 Requires-Python: >=3.7.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 ## API
 
 TODO
 
 ## CLI
 
 ```
-usage: __main__.py [-h] [--parse_ignoreshapes] [--parse_ignorenoroute]
+usage: gtfs-parser [-h] [--parse_ignoreshapes] [--parse_ignorenoroute]
                    [--aggregate_yyyymmdd AGGREGATE_YYYYMMDD]
                    [--aggregate_nounifystops]
                    [--aggregate_delimiter AGGREGATE_DELIMITER]
                    [--aggregate_begintime AGGREGATE_BEGINTIME]
                    [--aggregate_endtime AGGREGATE_ENDTIME]
                    mode src dst
 
@@ -58,12 +58,12 @@
   --aggregate_begintime AGGREGATE_BEGINTIME
   --aggregate_endtime AGGREGATE_ENDTIME
 ```
 
 ### Example
 
 ```sh
-python -m gtfs-parser parse gtfs.zip output
-python -m gtfs-parser parse gtfs_dir output --parse_ignoreshapes
-python -m gtfs-parser aggregate gtfs.zip output
-python -m gtfs-parser aggregate gtfs_dir output --aggregate_nounifystops
+gtfs-parser parse gtfs.zip output
+gtfs-parser parse gtfs_dir output --parse_ignoreshapes
+gtfs-parser aggregate gtfs.zip output
+gtfs-parser aggregate gtfs_dir output --aggregate_nounifystops
 ```
```

