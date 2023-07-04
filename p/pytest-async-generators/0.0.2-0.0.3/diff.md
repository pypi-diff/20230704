# Comparing `tmp/pytest_async_generators-0.0.2.tar.gz` & `tmp/pytest_async_generators-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_async_generators-0.0.2.tar", max compression
+gzip compressed data, was "pytest_async_generators-0.0.3.tar", max compression
```

## Comparing `pytest_async_generators-0.0.2.tar` & `pytest_async_generators-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      876 2023-07-04 19:46:34.473668 pytest_async_generators-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 19:20:46.368349 pytest_async_generators-0.0.2/pytest_async_generators/__init__.py
--rw-r--r--   0        0        0     1053 2023-07-04 19:44:00.152309 pytest_async_generators-0.0.2/pytest_async_generators/subscribe_to_messages.py
--rw-r--r--   0        0        0     1036 2023-07-04 19:11:43.775589 pytest_async_generators-0.0.2/readme.md
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 pytest_async_generators-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      876 2023-07-04 20:42:46.975820 pytest_async_generators-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 19:20:46.368349 pytest_async_generators-0.0.3/pytest_async_generators/__init__.py
+-rw-r--r--   0        0        0     1919 2023-07-04 20:41:21.927064 pytest_async_generators-0.0.3/pytest_async_generators/subscribe_to_messages.py
+-rw-r--r--   0        0        0     1036 2023-07-04 19:11:43.775589 pytest_async_generators-0.0.3/readme.md
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 pytest_async_generators-0.0.3/PKG-INFO
```

### Comparing `pytest_async_generators-0.0.2/pyproject.toml` & `pytest_async_generators-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-async-generators"
-version = "0.0.2"
+version = "0.0.3"
 description = "Pytest fixtures for async generators"
 repository = "https://github.com/possibilities/pytest-async-generators"
 authors = ["Mike Bannister <notimpossiblemike@gmail.com>"]
 readme = "readme.md"
 packages = [{include = "pytest_async_generators"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pytest_async_generators-0.0.2/readme.md` & `pytest_async_generators-0.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `pytest_async_generators-0.0.2/PKG-INFO` & `pytest_async_generators-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-async-generators
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pytest fixtures for async generators
 Home-page: https://github.com/possibilities/pytest-async-generators
 Author: Mike Bannister
 Author-email: notimpossiblemike@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

