# Comparing `tmp/autopack_tools-0.2.3.tar.gz` & `tmp/autopack_tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.2.3.tar", max compression
+gzip compressed data, was "autopack_tools-0.2.4.tar", max compression
```

## Comparing `autopack_tools-0.2.3.tar` & `autopack_tools-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.3/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.3/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.3/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.3/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.3/autopack/__main__.py
--rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.3/autopack/api.py
--rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.3/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.3/autopack/errors.py
--rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.3/autopack/get_pack.py
--rw-r--r--   0        0        0     3877 2023-07-04 01:58:56.151275 autopack_tools-0.2.3/autopack/installation.py
--rw-r--r--   0        0        0     2921 2023-07-03 23:58:49.932953 autopack_tools-0.2.3/autopack/pack.py
--rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.3/autopack/pack_response.py
--rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.3/autopack/search.py
--rw-r--r--   0        0        0     2094 2023-07-04 01:58:55.758062 autopack_tools-0.2.3/autopack/selection.py
--rw-r--r--   0        0        0     4405 2023-07-04 01:58:56.161504 autopack_tools-0.2.3/autopack/utils.py
--rw-r--r--   0        0        0      910 2023-07-04 01:59:16.152339 autopack_tools-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 autopack_tools-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.4/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.4/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.4/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.4/autopack/__main__.py
+-rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.4/autopack/api.py
+-rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.4/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.4/autopack/errors.py
+-rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.4/autopack/get_pack.py
+-rw-r--r--   0        0        0     3877 2023-07-04 01:58:56.151275 autopack_tools-0.2.4/autopack/installation.py
+-rw-r--r--   0        0        0     2921 2023-07-03 23:58:49.932953 autopack_tools-0.2.4/autopack/pack.py
+-rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.4/autopack/pack_response.py
+-rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.4/autopack/search.py
+-rw-r--r--   0        0        0     2094 2023-07-04 01:58:55.758062 autopack_tools-0.2.4/autopack/selection.py
+-rw-r--r--   0        0        0     4405 2023-07-04 01:58:56.161504 autopack_tools-0.2.4/autopack/utils.py
+-rw-r--r--   0        0        0      911 2023-07-04 03:52:06.435379 autopack_tools-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 autopack_tools-0.2.4/PKG-INFO
```

### Comparing `autopack_tools-0.2.3/LICENSE` & `autopack_tools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/README.md` & `autopack_tools-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/autopack/api.py` & `autopack_tools-0.2.4/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/autopack/cli.py` & `autopack_tools-0.2.4/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/autopack/get_pack.py` & `autopack_tools-0.2.4/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/autopack/installation.py` & `autopack_tools-0.2.4/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/autopack/pack.py` & `autopack_tools-0.2.4/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/autopack/pack_response.py` & `autopack_tools-0.2.4/autopack/pack_response.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/autopack/selection.py` & `autopack_tools-0.2.4/autopack/selection.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/autopack/utils.py` & `autopack_tools-0.2.4/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.3/pyproject.toml` & `autopack_tools-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.2.3"
+version = "0.2.4"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 requests = "^2.31.0"
 dataclasses-json = "^0.5.8"
 urllib3 = "^1.26.16"
 gitpython = "^3.1.31"
-langchain = "^0.0.215"
+langchain = ">=0.0.222"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.4.0"
 isort = "^5.12.0"
 pytest = "^7.3.2"
```

### Comparing `autopack_tools-0.2.3/PKG-INFO` & `autopack_tools-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.2.3
+Version: 0.2.4
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.8,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
-Requires-Dist: langchain (>=0.0.215,<0.0.216)
+Requires-Dist: langchain (>=0.0.222)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/AutoPackAI/autopack
 Description-Content-Type: text/markdown
 
 # AutoPack
```

