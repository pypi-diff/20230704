# Comparing `tmp/replicate-0.8.3.tar.gz` & `tmp/replicate-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate-0.8.3.tar", last modified: Tue May 23 09:20:52 2023, max compression
+gzip compressed data, was "replicate-0.8.4.tar", last modified: Tue Jul  4 11:35:43 2023, max compression
```

## Comparing `replicate-0.8.3.tar` & `replicate-0.8.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:52.181595 replicate-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-23 09:20:41.000000 replicate-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-05-23 09:20:52.181595 replicate-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-23 09:20:41.000000 replicate-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-23 09:20:41.000000 replicate-0.8.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:52.177595 replicate-0.8.3/replicate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-23 09:20:41.000000 replicate-0.8.3/replicate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:52.177595 replicate-0.8.3/replicate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-05-23 09:20:52.000000 replicate-0.8.3/replicate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 09:20:52.000000 replicate-0.8.3/replicate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:20:52.000000 replicate-0.8.3/replicate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 09:20:52.000000 replicate-0.8.3/replicate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:20:52.000000 replicate-0.8.3/replicate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:20:52.181595 replicate-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:52.181595 replicate-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-05-23 09:20:41.000000 replicate-0.8.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-23 09:20:41.000000 replicate-0.8.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-23 09:20:41.000000 replicate-0.8.3/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-23 09:20:41.000000 replicate-0.8.3/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-23 09:20:41.000000 replicate-0.8.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:35:43.235792 replicate-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-04 11:35:31.000000 replicate-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-07-04 11:35:43.231792 replicate-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-04 11:35:31.000000 replicate-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-04 11:35:31.000000 replicate-0.8.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:35:43.231792 replicate-0.8.4/replicate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-04 11:35:31.000000 replicate-0.8.4/replicate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:35:43.231792 replicate-0.8.4/replicate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-07-04 11:35:43.000000 replicate-0.8.4/replicate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 11:35:43.000000 replicate-0.8.4/replicate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:35:43.000000 replicate-0.8.4/replicate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 11:35:43.000000 replicate-0.8.4/replicate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 11:35:43.000000 replicate-0.8.4/replicate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:35:43.235792 replicate-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:35:43.231792 replicate-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-07-04 11:35:31.000000 replicate-0.8.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-04 11:35:31.000000 replicate-0.8.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-07-04 11:35:31.000000 replicate-0.8.4/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-04 11:35:31.000000 replicate-0.8.4/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-04 11:35:31.000000 replicate-0.8.4/tests/test_version.py
```

### Comparing `replicate-0.8.3/LICENSE` & `replicate-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/PKG-INFO` & `replicate-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python client for Replicate
 Author: Replicate, Inc.
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `replicate-0.8.3/README.md` & `replicate-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/pyproject.toml` & `replicate-0.8.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "replicate"
-version = "0.8.3"
+version = "0.8.4"
 description = "Python client for Replicate"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Replicate, Inc." }]
 requires-python = ">=3.8"
-dependencies = ["packaging", "pydantic>1", "requests>2"]
+dependencies = ["packaging", "pydantic>1,<2", "requests>2"]
 optional-dependencies = { dev = [
     "black",
     "mypy",
     "pytest",
     "responses",
     "ruff",
 ] }
```

### Comparing `replicate-0.8.3/replicate/base_model.py` & `replicate-0.8.4/replicate/base_model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/client.py` & `replicate-0.8.4/replicate/client.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/collection.py` & `replicate-0.8.4/replicate/collection.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/files.py` & `replicate-0.8.4/replicate/files.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/json.py` & `replicate-0.8.4/replicate/json.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/model.py` & `replicate-0.8.4/replicate/model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/prediction.py` & `replicate-0.8.4/replicate/prediction.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/schema.py` & `replicate-0.8.4/replicate/schema.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/training.py` & `replicate-0.8.4/replicate/training.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate/version.py` & `replicate-0.8.4/replicate/version.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/replicate.egg-info/PKG-INFO` & `replicate-0.8.4/replicate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python client for Replicate
 Author: Replicate, Inc.
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `replicate-0.8.3/replicate.egg-info/SOURCES.txt` & `replicate-0.8.4/replicate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/tests/test_client.py` & `replicate-0.8.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/tests/test_model.py` & `replicate-0.8.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/tests/test_prediction.py` & `replicate-0.8.4/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/tests/test_training.py` & `replicate-0.8.4/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.3/tests/test_version.py` & `replicate-0.8.4/tests/test_version.py`

 * *Files identical despite different names*

