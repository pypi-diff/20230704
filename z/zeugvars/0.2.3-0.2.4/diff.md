# Comparing `tmp/zeugvars-0.2.3.tar.gz` & `tmp/zeugvars-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.2.3.tar", max compression
+gzip compressed data, was "zeugvars-0.2.4.tar", max compression
```

## Comparing `zeugvars-0.2.3.tar` & `zeugvars-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.3/LICENSE
--rw-r--r--   0        0        0     3450 2023-07-04 18:30:24.122118 zeugvars-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4169 2023-07-04 18:29:59.436921 zeugvars-0.2.3/README.md
--rw-r--r--   0        0        0    10695 2023-07-04 18:21:07.559831 zeugvars-0.2.3/zeugvars.py
--rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 zeugvars-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3450 2023-07-04 18:31:39.281981 zeugvars-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4159 2023-07-04 18:31:16.683894 zeugvars-0.2.4/README.md
+-rw-r--r--   0        0        0    10695 2023-07-04 18:21:07.559831 zeugvars-0.2.4/zeugvars.py
+-rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 zeugvars-0.2.4/PKG-INFO
```

### Comparing `zeugvars-0.2.3/LICENSE` & `zeugvars-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zeugvars-0.2.3/pyproject.toml` & `zeugvars-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeugvars"
-version = "0.2.3"
+version = "0.2.4"
 description = "A simple & straight-forward Python module for creating context-dependent proxy objects."
 authors = ["bswck <bswck.dev@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/bswck/zeugvars"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `zeugvars-0.2.3/README.md` & `zeugvars-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## `zeugvars`
 
 A simple & straight-forward Python module for creating type-safe, context-dependent proxy objects.
 
 ## Example
 
-The following example shows how to use `zeugvar` with `contextvars.ContextVar`:
+The following example shows how to use `zeugvars` with `contextvars`:
 
 ```python
 >>> from contextvars import ContextVar
 >>> from zeugvars import proxy
 ...
 >>> count_var = ContextVar("count_var")
 >>> count = proxy(counter, int)
```

### Comparing `zeugvars-0.2.3/zeugvars.py` & `zeugvars-0.2.4/zeugvars.py`

 * *Files identical despite different names*

### Comparing `zeugvars-0.2.3/PKG-INFO` & `zeugvars-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeugvars
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
 Home-page: https://github.com/bswck/zeugvars
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 
 ## `zeugvars`
 
 A simple & straight-forward Python module for creating type-safe, context-dependent proxy objects.
 
 ## Example
 
-The following example shows how to use `zeugvar` with `contextvars.ContextVar`:
+The following example shows how to use `zeugvars` with `contextvars`:
 
 ```python
 >>> from contextvars import ContextVar
 >>> from zeugvars import proxy
 ...
 >>> count_var = ContextVar("count_var")
 >>> count = proxy(counter, int)
```

