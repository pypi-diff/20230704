# Comparing `tmp/hawkflow-0.0.9.tar.gz` & `tmp/hawkflow-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/felbus/github/hawkflow-py/dist/.tmp-o91vzij7/hawkflow-0.0.9.tar", last modified: Wed Mar 15 18:46:00 2023, max compression
+gzip compressed data, was "/Users/felbus/github/hawkflow-py/dist/.tmp-mag3eo2z/hawkflow-0.0.91.tar", last modified: Tue Jul  4 08:31:22 2023, max compression
```

## Comparing `hawkflow-0.0.9.tar` & `hawkflow-0.0.91.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-03-15 18:46:00.000000 hawkflow-0.0.9/
--rw-r--r--   0 felbus     (501) staff       (20)     1054 2023-02-20 15:32:46.000000 hawkflow-0.0.9/LICENSE
--rw-r--r--   0 felbus     (501) staff       (20)     1257 2023-03-15 18:46:00.000000 hawkflow-0.0.9/PKG-INFO
--rw-r--r--   0 felbus     (501) staff       (20)      566 2023-02-20 15:32:46.000000 hawkflow-0.0.9/README.md
--rw-r--r--   0 felbus     (501) staff       (20)      842 2023-03-15 18:45:34.000000 hawkflow-0.0.9/pyproject.toml
--rw-r--r--   0 felbus     (501) staff       (20)       38 2023-03-15 18:46:00.000000 hawkflow-0.0.9/setup.cfg
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/hawkflow.egg-info/
--rw-r--r--   0 felbus     (501) staff       (20)     1257 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/hawkflow.egg-info/PKG-INFO
--rw-r--r--   0 felbus     (501) staff       (20)      556 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/hawkflow.egg-info/SOURCES.txt
--rw-r--r--   0 felbus     (501) staff       (20)        1 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/hawkflow.egg-info/dependency_links.txt
--rw-r--r--   0 felbus     (501) staff       (20)       17 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/hawkflow.egg-info/requires.txt
--rw-r--r--   0 felbus     (501) staff       (20)       15 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/hawkflow.egg-info/top_level.txt
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/hawkflowclient/
--rw-r--r--   0 felbus     (501) staff       (20)      199 2023-03-03 15:13:44.000000 hawkflow-0.0.9/src/hawkflowclient/__init__.py
--rw-r--r--   0 felbus     (501) staff       (20)      879 2023-02-27 16:57:39.000000 hawkflow-0.0.9/src/hawkflowclient/_endpoints.py
--rw-r--r--   0 felbus     (501) staff       (20)     1045 2023-02-20 15:32:46.000000 hawkflow-0.0.9/src/hawkflowclient/_hawkflow_exceptions.py
--rw-r--r--   0 felbus     (501) staff       (20)     3444 2023-03-15 18:44:25.000000 hawkflow-0.0.9/src/hawkflowclient/_validation.py
--rw-r--r--   0 felbus     (501) staff       (20)     2714 2023-03-03 15:36:38.000000 hawkflow-0.0.9/src/hawkflowclient/hawkflow_api.py
--rw-r--r--   0 felbus     (501) staff       (20)     1816 2023-02-20 15:32:46.000000 hawkflow-0.0.9/src/hawkflowclient/hawkflow_decorators.py
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-03-15 18:46:00.000000 hawkflow-0.0.9/src/hawkflowclient/tests/
--rw-r--r--   0 felbus     (501) staff       (20)        0 2023-02-20 15:32:46.000000 hawkflow-0.0.9/src/hawkflowclient/tests/__init__.py
--rw-r--r--   0 felbus     (501) staff       (20)     3276 2023-02-20 15:32:46.000000 hawkflow-0.0.9/src/hawkflowclient/tests/test_hawkflow_api.py
--rw-r--r--   0 felbus     (501) staff       (20)     3980 2023-03-15 18:43:00.000000 hawkflow-0.0.9/src/hawkflowclient/tests/test_validation.py
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/
+-rw-r--r--   0 felbus     (501) staff       (20)     1054 2023-02-20 15:32:46.000000 hawkflow-0.0.91/LICENSE
+-rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-04 08:31:22.000000 hawkflow-0.0.91/PKG-INFO
+-rw-r--r--   0 felbus     (501) staff       (20)     1264 2023-03-15 18:47:38.000000 hawkflow-0.0.91/README.md
+-rw-r--r--   0 felbus     (501) staff       (20)      843 2023-07-04 08:30:57.000000 hawkflow-0.0.91/pyproject.toml
+-rw-r--r--   0 felbus     (501) staff       (20)       38 2023-07-04 08:31:22.000000 hawkflow-0.0.91/setup.cfg
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/
+-rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/PKG-INFO
+-rw-r--r--   0 felbus     (501) staff       (20)      556 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 felbus     (501) staff       (20)        1 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 felbus     (501) staff       (20)       17 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/requires.txt
+-rw-r--r--   0 felbus     (501) staff       (20)       15 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflow.egg-info/top_level.txt
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflowclient/
+-rw-r--r--   0 felbus     (501) staff       (20)      199 2023-03-03 15:13:44.000000 hawkflow-0.0.91/src/hawkflowclient/__init__.py
+-rw-r--r--   0 felbus     (501) staff       (20)      879 2023-02-27 16:57:39.000000 hawkflow-0.0.91/src/hawkflowclient/_endpoints.py
+-rw-r--r--   0 felbus     (501) staff       (20)     1045 2023-02-20 15:32:46.000000 hawkflow-0.0.91/src/hawkflowclient/_hawkflow_exceptions.py
+-rw-r--r--   0 felbus     (501) staff       (20)     3459 2023-07-04 08:28:09.000000 hawkflow-0.0.91/src/hawkflowclient/_validation.py
+-rw-r--r--   0 felbus     (501) staff       (20)     2714 2023-03-03 15:36:38.000000 hawkflow-0.0.91/src/hawkflowclient/hawkflow_api.py
+-rw-r--r--   0 felbus     (501) staff       (20)     1816 2023-02-20 15:32:46.000000 hawkflow-0.0.91/src/hawkflowclient/hawkflow_decorators.py
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-04 08:31:22.000000 hawkflow-0.0.91/src/hawkflowclient/tests/
+-rw-r--r--   0 felbus     (501) staff       (20)        0 2023-02-20 15:32:46.000000 hawkflow-0.0.91/src/hawkflowclient/tests/__init__.py
+-rw-r--r--   0 felbus     (501) staff       (20)     3276 2023-02-20 15:32:46.000000 hawkflow-0.0.91/src/hawkflowclient/tests/test_hawkflow_api.py
+-rw-r--r--   0 felbus     (501) staff       (20)     3980 2023-07-04 08:17:17.000000 hawkflow-0.0.91/src/hawkflowclient/tests/test_validation.py
```

### Comparing `hawkflow-0.0.9/LICENSE` & `hawkflow-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.9/pyproject.toml` & `hawkflow-0.0.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="hawkflow"
-version="0.0.9"
+version="0.0.91"
 description="HawkFlow.ai"
 readme = "README.md"
 keywords=["hawkflow", "hawkflowclient", "monitoring"]
 license = {text = "LICENSE"}
 requires-python = ">=3.7"
 dependencies=[
     "requests>=2.25.1"
```

### Comparing `hawkflow-0.0.9/src/hawkflow.egg-info/SOURCES.txt` & `hawkflow-0.0.91/src/hawkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.9/src/hawkflowclient/_endpoints.py` & `hawkflow-0.0.91/src/hawkflowclient/_endpoints.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.9/src/hawkflowclient/_hawkflow_exceptions.py` & `hawkflow-0.0.91/src/hawkflowclient/_hawkflow_exceptions.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.9/src/hawkflowclient/_validation.py` & `hawkflow-0.0.91/src/hawkflowclient/_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from ._hawkflow_exceptions import *
 
 
 PROCESS_REGEX = r'^[a-zA-Z\d\s_-]*$'
 META_REGEX = r'^[\w\s\\/\-\_\*\&\=\.\+\?\@\:]*$'
 API_KEY_REGEX = r'^[a-zA-Z0-9_-]+$'
-METRIC_KEY_REGEX = r'^[a-zA-Z\d\s_-]*$'
+METRIC_KEY_REGEX = r'^[\w\s\\/\-\_\*\&\=\.\+\?\@\:]*$'
 UID_REGEX = r'^[a-zA-Z0-9_-]*$'
 
 
 def _validate_timed_data(process: str, meta: str, uid: str):
     _validate_core(process, meta)
     _validate_uid(uid)
```

### Comparing `hawkflow-0.0.9/src/hawkflowclient/hawkflow_api.py` & `hawkflow-0.0.91/src/hawkflowclient/hawkflow_api.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.9/src/hawkflowclient/hawkflow_decorators.py` & `hawkflow-0.0.91/src/hawkflowclient/hawkflow_decorators.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.9/src/hawkflowclient/tests/test_hawkflow_api.py` & `hawkflow-0.0.91/src/hawkflowclient/tests/test_hawkflow_api.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.9/src/hawkflowclient/tests/test_validation.py` & `hawkflow-0.0.91/src/hawkflowclient/tests/test_validation.py`

 * *Files identical despite different names*

