# Comparing `tmp/zeugvars-0.2.1.tar.gz` & `tmp/zeugvars-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.2.1.tar", max compression
+gzip compressed data, was "zeugvars-0.2.3.tar", max compression
```

## Comparing `zeugvars-0.2.1.tar` & `zeugvars-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.1/LICENSE
--rw-r--r--   0        0        0     3450 2023-07-04 18:28:40.653623 zeugvars-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4168 2023-07-04 18:28:28.612770 zeugvars-0.2.1/README.md
--rw-r--r--   0        0        0    10695 2023-07-04 18:21:07.559831 zeugvars-0.2.1/zeugvars.py
--rw-r--r--   0        0        0     4511 1970-01-01 00:00:00.000000 zeugvars-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3450 2023-07-04 18:30:24.122118 zeugvars-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4169 2023-07-04 18:29:59.436921 zeugvars-0.2.3/README.md
+-rw-r--r--   0        0        0    10695 2023-07-04 18:21:07.559831 zeugvars-0.2.3/zeugvars.py
+-rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 zeugvars-0.2.3/PKG-INFO
```

### Comparing `zeugvars-0.2.1/LICENSE` & `zeugvars-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zeugvars-0.2.1/pyproject.toml` & `zeugvars-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeugvars"
-version = "0.2.1"
+version = "0.2.3"
 description = "A simple & straight-forward Python module for creating context-dependent proxy objects."
 authors = ["bswck <bswck.dev@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/bswck/zeugvars"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `zeugvars-0.2.1/README.md` & `zeugvars-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 `Manager.get()` and `Manage.set()` are called.
 This might be useful when there is the need to keep track of the tokens
 returned by `ContextVar.set()`, if using `ContextVar` as the manager.
 
 ## When would you use `zeugvars`?
 
 You could use `zeugvars` when...
-* ...writing a thread-safe application that operates on fixed resource that are different per thread.
+* ...writing a thread-safe application that operates on fixed resources specific for separate threads.
 * ...improving code readability by avoiding passing around the same object to every function.
 * ...writing a web application that operates on fixed resources per request.
 * ...writing an asynchronous application that operates on fixed resources between tasks.
 * ...having any other case where you could use global variables that are context-dependent!
 
 ## Why does it have such a weird name?
```

### Comparing `zeugvars-0.2.1/zeugvars.py` & `zeugvars-0.2.3/zeugvars.py`

 * *Files identical despite different names*

### Comparing `zeugvars-0.2.1/PKG-INFO` & `zeugvars-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeugvars
-Version: 0.2.1
+Version: 0.2.3
 Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
 Home-page: https://github.com/bswck/zeugvars
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -75,15 +75,15 @@
 `Manager.get()` and `Manage.set()` are called.
 This might be useful when there is the need to keep track of the tokens
 returned by `ContextVar.set()`, if using `ContextVar` as the manager.
 
 ## When would you use `zeugvars`?
 
 You could use `zeugvars` when...
-* ...writing a thread-safe application that operates on fixed resource that are different per thread.
+* ...writing a thread-safe application that operates on fixed resources specific for separate threads.
 * ...improving code readability by avoiding passing around the same object to every function.
 * ...writing a web application that operates on fixed resources per request.
 * ...writing an asynchronous application that operates on fixed resources between tasks.
 * ...having any other case where you could use global variables that are context-dependent!
 
 ## Why does it have such a weird name?
```

