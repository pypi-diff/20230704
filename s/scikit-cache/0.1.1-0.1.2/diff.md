# Comparing `tmp/scikit-cache-0.1.1.tar.gz` & `tmp/scikit-cache-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-cache-0.1.1.tar", last modified: Tue Jan 31 10:41:17 2023, max compression
+gzip compressed data, was "scikit-cache-0.1.2.tar", last modified: Tue Jul  4 12:28:49 2023, max compression
```

## Comparing `scikit-cache-0.1.1.tar` & `scikit-cache-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/scikit_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/scikit_cache/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/scikit_cache/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/scikit_cache/components/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/scikit_cache/components/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-01-31 10:40:47.204649 scikit-cache-0.1.1/scikit_cache/components/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/components/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/components/internal_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/components/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/utils/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/scikit_cache/utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_func_cache_set_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_object_cache_set_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-01-31 10:40:47.208649 scikit-cache-0.1.1/tests/test_utils.py
--rw-------   0 runner    (1001) docker     (123)     2054 2023-01-31 10:41:17.392453 scikit-cache-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1389 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/README.md
+-rw-r--r--   0        0        0     2752 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/__version__.py
+-rw-r--r--   0        0        0      267 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/components/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/components/cleanup.py
+-rw-r--r--   0        0        0    10305 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/components/decorators.py
+-rw-r--r--   0        0        0     4021 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/components/estimators.py
+-rw-r--r--   0        0        0     3933 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/components/file_handler.py
+-rw-r--r--   0        0        0     2913 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/components/internal_cache.py
+-rw-r--r--   0        0        0     1549 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/components/logging.py
+-rw-r--r--   0        0        0    21811 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/controller.py
+-rw-r--r--   0        0        0        0 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/py.typed
+-rw-r--r--   0        0        0     8734 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/resources.py
+-rw-r--r--   0        0        0      157 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/utils/__init__.py
+-rw-r--r--   0        0        0     2780 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/utils/base.py
+-rw-r--r--   0        0        0     1683 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/utils/estimators.py
+-rw-r--r--   0        0        0      661 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/utils/file_utils.py
+-rw-r--r--   0        0        0     3306 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/utils/hashing.py
+-rw-r--r--   0        0        0      718 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/utils/output.py
+-rw-r--r--   0        0        0     1652 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/scikit_cache/utils/versioning.py
+-rw-r--r--   0        0        0     1627 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     7570 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_cleanup.py
+-rw-r--r--   0        0        0     7973 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_controller.py
+-rw-r--r--   0        0        0     8991 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_decorators.py
+-rw-r--r--   0        0        0     3091 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_estimators.py
+-rw-r--r--   0        0        0     1655 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_file_handler.py
+-rw-r--r--   0        0        0     2838 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_func_cache_set_get.py
+-rw-r--r--   0        0        0     4386 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_hashing.py
+-rw-r--r--   0        0        0     3385 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_object_cache_set_get.py
+-rw-r--r--   0        0        0     7247 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_resources.py
+-rw-r--r--   0        0        0     4158 2023-07-04 12:28:08.075136 scikit-cache-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 scikit-cache-0.1.2/PKG-INFO
```

### Comparing `scikit-cache-0.1.1/LICENSE` & `scikit-cache-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/pyproject.toml` & `scikit-cache-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "pydantic",
+    "pydantic <= 1.10.10",
     "joblib",
     "pyyaml",
 ]
-version = "0.1.1"
+version = "0.1.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/deniskrumko/scikit-cache"
```

### Comparing `scikit-cache-0.1.1/scikit_cache/components/cleanup.py` & `scikit-cache-0.1.2/scikit_cache/components/cleanup.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/components/decorators.py` & `scikit-cache-0.1.2/scikit_cache/components/decorators.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/components/estimators.py` & `scikit-cache-0.1.2/scikit_cache/components/estimators.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/components/file_handler.py` & `scikit-cache-0.1.2/scikit_cache/components/file_handler.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/components/internal_cache.py` & `scikit-cache-0.1.2/scikit_cache/components/internal_cache.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/components/logging.py` & `scikit-cache-0.1.2/scikit_cache/components/logging.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/controller.py` & `scikit-cache-0.1.2/scikit_cache/controller.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/resources.py` & `scikit-cache-0.1.2/scikit_cache/resources.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/utils/base.py` & `scikit-cache-0.1.2/scikit_cache/utils/base.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/utils/estimators.py` & `scikit-cache-0.1.2/scikit_cache/utils/estimators.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/utils/file_utils.py` & `scikit-cache-0.1.2/scikit_cache/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/utils/hashing.py` & `scikit-cache-0.1.2/scikit_cache/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/utils/output.py` & `scikit-cache-0.1.2/scikit_cache/utils/output.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/scikit_cache/utils/versioning.py` & `scikit-cache-0.1.2/scikit_cache/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/conftest.py` & `scikit-cache-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_cleanup.py` & `scikit-cache-0.1.2/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_controller.py` & `scikit-cache-0.1.2/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_decorators.py` & `scikit-cache-0.1.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_estimators.py` & `scikit-cache-0.1.2/tests/test_estimators.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_file_handler.py` & `scikit-cache-0.1.2/tests/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_func_cache_set_get.py` & `scikit-cache-0.1.2/tests/test_func_cache_set_get.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_hashing.py` & `scikit-cache-0.1.2/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_object_cache_set_get.py` & `scikit-cache-0.1.2/tests/test_object_cache_set_get.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_resources.py` & `scikit-cache-0.1.2/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/tests/test_utils.py` & `scikit-cache-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-cache-0.1.1/PKG-INFO` & `scikit-cache-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_cache
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pickle-based caching library with SKLearn estimators supports
 License: MIT
 Author-email: Denis Krumko <dkrumko@gmail.ru>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -19,14 +19,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Provides-Extra: dev
 Project-URL: repository, https://github.com/deniskrumko/scikit-cache
 Description-Content-Type: text/markdown
 
+[![pypi](https://img.shields.io/pypi/v/scikit-cache.svg)](https://pypi.org/project/scikit-cache/)
+[![pypi](https://img.shields.io/pypi/pyversions/scikit-cache.svg)](https://pypi.org/project/scikit-cache/)
+[![pypi](https://img.shields.io/pypi/l/scikit-cache.svg)](https://raw.githubusercontent.com/deniskrumko/scikit-cache/master/LICENSE)
+
 # Scikit Cache
 
 Pickle-based caching library. Supports file-system caching only.
 
 ## Installation
 
 ```
```

