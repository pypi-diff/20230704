# Comparing `tmp/torch_compose-0.1.0.tar.gz` & `tmp/torch_compose-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_compose-0.1.0.tar", max compression
+gzip compressed data, was "torch_compose-0.1.1.tar", max compression
```

## Comparing `torch_compose-0.1.0.tar` & `torch_compose-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-01 01:44:51.699904 torch_compose-0.1.0/README.md
--rw-r--r--   0        0        0      627 2023-07-04 00:27:55.473464 torch_compose-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 01:44:51.699904 torch_compose-0.1.0/torch_compose/__init__.py
--rw-r--r--   0        0        0   248026 2023-07-04 00:25:48.880921 torch_compose-0.1.0/torch_compose/demo.ipynb
--rw-r--r--   0        0        0    10395 2023-07-04 00:25:08.508748 torch_compose-0.1.0/torch_compose/module.py
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 torch_compose-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-04 00:41:28.256948 torch_compose-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-01 01:44:51.699904 torch_compose-0.1.1/README.md
+-rw-r--r--   0        0        0      627 2023-07-04 05:27:44.274922 torch_compose-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 01:44:51.699904 torch_compose-0.1.1/torch_compose/__init__.py
+-rw-r--r--   0        0        0   248026 2023-07-04 00:25:48.880921 torch_compose-0.1.1/torch_compose/demo.ipynb
+-rw-r--r--   0        0        0    10395 2023-07-04 00:25:08.508748 torch_compose-0.1.1/torch_compose/module.py
+-rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 torch_compose-0.1.1/PKG-INFO
```

### Comparing `torch_compose-0.1.0/pyproject.toml` & `torch_compose-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "torch-compose"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Alex Naka <alex.naka@gmail.com>"]
 readme = "README.md"
 packages = [{include = "torch_compose"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-graphlib = "^0.9.5"
+python = "^3.9"
 networkx = "^3.1"
 torch = {version= "^1.7.0 || >=2.0.0", source="torch"}
 matplotlib = "^3.7.1"
+graphlib = "^0.9.5"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
 black = "^23.3.0"
 
 [build-system]
```

### Comparing `torch_compose-0.1.0/torch_compose/demo.ipynb` & `torch_compose-0.1.1/torch_compose/demo.ipynb`

 * *Files identical despite different names*

### Comparing `torch_compose-0.1.0/torch_compose/module.py` & `torch_compose-0.1.1/torch_compose/module.py`

 * *Files identical despite different names*

### Comparing `torch_compose-0.1.0/PKG-INFO` & `torch_compose-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: torch-compose
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Alex Naka
 Author-email: alex.naka@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: graphlib (>=0.9.5,<0.10.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: torch (>=1.7.0)
```

