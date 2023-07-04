# Comparing `tmp/minty-3.0.8.tar.gz` & `tmp/minty-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minty-3.0.8.tar", last modified: Tue Nov 22 13:13:52 2022, max compression
+gzip compressed data, was "minty-3.0.9.tar", last modified: Tue Jul  4 07:09:39 2023, max compression
```

## Comparing `minty-3.0.8.tar` & `minty-3.0.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.989261 minty-3.0.8/
--rw-r--r--   0 root         (0) root         (0)     1980 2022-11-22 13:13:52.989261 minty-3.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1409 2022-11-22 13:13:33.000000 minty-3.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.985261 minty-3.0.8/minty/
--rw-rw-rw-   0 root         (0) root         (0)     1652 2022-11-22 13:13:33.000000 minty-3.0.8/minty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.985261 minty-3.0.8/minty/config/
--rw-rw-rw-   0 root         (0) root         (0)       82 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.989261 minty-3.0.8/minty/config/parser/
--rw-rw-rw-   0 root         (0) root         (0)      273 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      919 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/parser/apache.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/parser/base.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/parser/json_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.989261 minty-3.0.8/minty/config/store/
--rw-rw-rw-   0 root         (0) root         (0)      305 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/store/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/store/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/store/filestore.py
--rw-rw-rw-   0 root         (0) root         (0)     1382 2022-11-22 13:13:33.000000 minty-3.0.8/minty/config/store/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.989261 minty-3.0.8/minty/cqrs/
--rw-rw-rw-   0 root         (0) root         (0)    25866 2022-11-22 13:13:33.000000 minty-3.0.8/minty/cqrs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5471 2022-11-22 13:13:33.000000 minty-3.0.8/minty/cqrs/events.py
--rw-rw-rw-   0 root         (0) root         (0)     5584 2022-11-22 13:13:33.000000 minty-3.0.8/minty/cqrs/test.py
--rw-rw-rw-   0 root         (0) root         (0)     2790 2022-11-22 13:13:33.000000 minty-3.0.8/minty/date_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)    11015 2022-11-22 13:13:33.000000 minty-3.0.8/minty/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2022-11-22 13:13:33.000000 minty-3.0.8/minty/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.989261 minty-3.0.8/minty/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)     7994 2022-11-22 13:13:33.000000 minty-3.0.8/minty/infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2022-11-22 13:13:33.000000 minty-3.0.8/minty/infrastructure/mime_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.989261 minty-3.0.8/minty/logging/
--rw-rw-rw-   0 root         (0) root         (0)       82 2022-11-22 13:13:33.000000 minty-3.0.8/minty/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2022-11-22 13:13:33.000000 minty-3.0.8/minty/logging/mdc.py
--rw-rw-rw-   0 root         (0) root         (0)     3391 2022-11-22 13:13:33.000000 minty-3.0.8/minty/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-11-22 13:13:33.000000 minty-3.0.8/minty/object.py
--rw-rw-rw-   0 root         (0) root         (0)     3583 2022-11-22 13:13:33.000000 minty-3.0.8/minty/repository.py
--rw-rw-rw-   0 root         (0) root         (0)     2406 2022-11-22 13:13:33.000000 minty-3.0.8/minty/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 13:13:52.985261 minty-3.0.8/minty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1980 2022-11-22 13:13:52.000000 minty-3.0.8/minty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      818 2022-11-22 13:13:52.000000 minty-3.0.8/minty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 13:13:52.000000 minty-3.0.8/minty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 13:13:52.000000 minty-3.0.8/minty.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      119 2022-11-22 13:13:52.000000 minty-3.0.8/minty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-11-22 13:13:52.000000 minty-3.0.8/minty.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      558 2022-11-22 13:13:33.000000 minty-3.0.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      228 2022-11-22 13:13:52.993261 minty-3.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1373 2022-11-22 13:13:33.000000 minty-3.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.468438 minty-3.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-07-04 07:09:39.468438 minty-3.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-07-04 07:00:04.000000 minty-3.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.464438 minty-3.0.9/minty/
+-rw-rw-rw-   0 root         (0) root         (0)     1652 2023-07-04 07:00:04.000000 minty-3.0.9/minty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.468438 minty-3.0.9/minty/config/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.468438 minty-3.0.9/minty/config/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/parser/apache.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/parser/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/parser/json_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.468438 minty-3.0.9/minty/config/store/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/store/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/store/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/store/filestore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-07-04 07:00:04.000000 minty-3.0.9/minty/config/store/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.468438 minty-3.0.9/minty/cqrs/
+-rw-rw-rw-   0 root         (0) root         (0)    25866 2023-07-04 07:00:04.000000 minty-3.0.9/minty/cqrs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-07-04 07:00:04.000000 minty-3.0.9/minty/cqrs/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     5584 2023-07-04 07:00:04.000000 minty-3.0.9/minty/cqrs/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-07-04 07:00:04.000000 minty-3.0.9/minty/date_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)    11015 2023-07-04 07:00:04.000000 minty-3.0.9/minty/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-07-04 07:00:04.000000 minty-3.0.9/minty/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.468438 minty-3.0.9/minty/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)     7994 2023-07-04 07:00:04.000000 minty-3.0.9/minty/infrastructure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-07-04 07:00:04.000000 minty-3.0.9/minty/infrastructure/mime_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.468438 minty-3.0.9/minty/logging/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-07-04 07:00:04.000000 minty-3.0.9/minty/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-07-04 07:00:04.000000 minty-3.0.9/minty/logging/mdc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2023-07-04 07:00:04.000000 minty-3.0.9/minty/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-04 07:00:04.000000 minty-3.0.9/minty/object.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 07:00:04.000000 minty-3.0.9/minty/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3583 2023-07-04 07:00:04.000000 minty-3.0.9/minty/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     2406 2023-07-04 07:00:04.000000 minty-3.0.9/minty/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:09:39.468438 minty-3.0.9/minty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-07-04 07:09:39.000000 minty-3.0.9/minty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2023-07-04 07:09:39.000000 minty-3.0.9/minty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 07:09:39.000000 minty-3.0.9/minty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 07:09:39.000000 minty-3.0.9/minty.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      129 2023-07-04 07:09:39.000000 minty-3.0.9/minty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-04 07:09:39.000000 minty-3.0.9/minty.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-04 07:00:04.000000 minty-3.0.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-04 07:09:39.472438 minty-3.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-07-04 07:08:23.000000 minty-3.0.9/setup.py
```

### Comparing `minty-3.0.8/PKG-INFO` & `minty-3.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: minty
-Version: 3.0.8
+Version: 3.0.9
 Summary: Minty Command and Query based on DDD
 Home-page: https://gitlab.com/minty-python/minty
 Author: Michiel Ootjers
 Author-email: michiel@mintlab.nl
 License: EUPL license
 Keywords: minty
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 
@@ -63,9 +62,7 @@
 
 This project is licensed under the EUPL, v1.2. See the `EUPL-1.2.txt` in the
 `LICENSES` directory for details.
 
 .. SPDX-FileCopyrightText: 2020 Mintlab B.V.
 ..
 .. SPDX-License-Identifier: EUPL-1.2
-
-
```

### Comparing `minty-3.0.8/README.rst` & `minty-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/__init__.py` & `minty-3.0.9/minty/__init__.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/config/parser/apache.py` & `minty-3.0.9/minty/config/parser/apache.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/config/parser/base.py` & `minty-3.0.9/minty/config/parser/base.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/config/parser/json_parser.py` & `minty-3.0.9/minty/config/parser/json_parser.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/config/store/base.py` & `minty-3.0.9/minty/config/store/base.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/config/store/filestore.py` & `minty-3.0.9/minty/config/store/filestore.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/config/store/redis.py` & `minty-3.0.9/minty/config/store/redis.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/cqrs/__init__.py` & `minty-3.0.9/minty/cqrs/__init__.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/cqrs/events.py` & `minty-3.0.9/minty/cqrs/events.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/cqrs/test.py` & `minty-3.0.9/minty/cqrs/test.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/date_calculation.py` & `minty-3.0.9/minty/date_calculation.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/entity.py` & `minty-3.0.9/minty/entity.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/exceptions.py` & `minty-3.0.9/minty/exceptions.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/infrastructure/__init__.py` & `minty-3.0.9/minty/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/infrastructure/mime_utils.py` & `minty-3.0.9/minty/infrastructure/mime_utils.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/logging/mdc.py` & `minty-3.0.9/minty/logging/mdc.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/middleware.py` & `minty-3.0.9/minty/middleware.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/repository.py` & `minty-3.0.9/minty/repository.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty/validation.py` & `minty-3.0.9/minty/validation.py`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/minty.egg-info/PKG-INFO` & `minty-3.0.9/minty.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: minty
-Version: 3.0.8
+Version: 3.0.9
 Summary: Minty Command and Query based on DDD
 Home-page: https://gitlab.com/minty-python/minty
 Author: Michiel Ootjers
 Author-email: michiel@mintlab.nl
 License: EUPL license
 Keywords: minty
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 
@@ -63,9 +62,7 @@
 
 This project is licensed under the EUPL, v1.2. See the `EUPL-1.2.txt` in the
 `LICENSES` directory for details.
 
 .. SPDX-FileCopyrightText: 2020 Mintlab B.V.
 ..
 .. SPDX-License-Identifier: EUPL-1.2
-
-
```

### Comparing `minty-3.0.8/minty.egg-info/SOURCES.txt` & `minty-3.0.9/minty.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 minty/__init__.py
 minty/date_calculation.py
 minty/entity.py
 minty/exceptions.py
 minty/middleware.py
 minty/object.py
+minty/py.typed
 minty/repository.py
 minty/validation.py
 minty.egg-info/PKG-INFO
 minty.egg-info/SOURCES.txt
 minty.egg-info/dependency_links.txt
 minty.egg-info/not-zip-safe
 minty.egg-info/requires.txt
```

### Comparing `minty-3.0.8/pyproject.toml` & `minty-3.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `minty-3.0.8/setup.py` & `minty-3.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     keywords="minty",
     name="minty",
     package_data={"minty": ["py.typed"]},
     packages=find_packages(include=["minty", "minty.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://gitlab.com/minty-python/minty",
-    version="3.0.8",
+    version="3.0.9",
     zip_safe=False,
 )
```

