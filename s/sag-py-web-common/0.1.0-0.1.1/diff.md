# Comparing `tmp/sag-py-web-common-0.1.0.tar.gz` & `tmp/sag-py-web-common-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-web-common-0.1.0.tar", last modified: Mon May  8 13:10:26 2023, max compression
+gzip compressed data, was "sag-py-web-common-0.1.1.tar", last modified: Tue Jul  4 09:11:11 2023, max compression
```

## Comparing `sag-py-web-common-0.1.0.tar` & `sag-py-web-common-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:10:26.958146 sag-py-web-common-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-08 13:10:26.958146 sag-py-web-common-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:10:26.958146 sag-py-web-common-0.1.0/sag_py_web_common/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/sag_py_web_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/sag_py_web_common/default_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/sag_py_web_common/filtered_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/sag_py_web_common/json_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/sag_py_web_common/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/sag_py_web_common/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:10:26.958146 sag-py-web-common-0.1.0/sag_py_web_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-08 13:10:26.000000 sag-py-web-common-0.1.0/sag_py_web_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-08 13:10:26.000000 sag-py-web-common-0.1.0/sag_py_web_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:10:26.000000 sag-py-web-common-0.1.0/sag_py_web_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 13:10:26.000000 sag-py-web-common-0.1.0/sag_py_web_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 13:10:26.000000 sag-py-web-common-0.1.0/sag_py_web_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 13:10:26.958146 sag-py-web-common-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:10:26.958146 sag-py-web-common-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 13:10:13.000000 sag-py-web-common-0.1.0/tests/test_build_default_route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/sag_py_web_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/default_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/filtered_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/json_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/sag_py_web_common/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 09:11:11.000000 sag-py-web-common-0.1.1/sag_py_web_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:11:11.150767 sag-py-web-common-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 09:11:00.000000 sag-py-web-common-0.1.1/tests/test_build_default_route.py
```

### Comparing `sag-py-web-common-0.1.0/LICENSE.txt` & `sag-py-web-common-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-web-common-0.1.0/PKG-INFO` & `sag-py-web-common-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-web-common
-Version: 0.1.0
+Version: 0.1.1
 Summary: Small helper functions for web projects
 Home-page: https://github.com/SamhammerAG/sag_py_web_common
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_web_common
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_web_common/issues
@@ -75,24 +75,34 @@
 )
 ```
 
 Also see this page for further configuration details: https://github.com/Kludex/asgi-logger
 
 ### Json exception handler
 
-Per default fastapi falls back to text responses if there are exceptions.
+Per default fastapi falls back to text responses if there are unknown exceptions.
 That's not the desired behaviour for json api's.
 
 This handler ensures that a json is returned. It contains the field "detail" with the exception message.
 
 ```python
-from sag_py_web_common.json_exception_handler import handle_exception
+from sag_py_web_common.json_exception_handler import handle_unknown_exception
 
-app.add_exception_handler(Exception, handle_exception)
+app.add_exception_handler(Exception, handle_unknown_exception)
 ```
+Fo logging any HHTP-Exception use log_exception funktion.
+
+```python
+from starlette.exceptions import HTTPException as StarletteHTTPException
+from sag_py_web_common.json_exception_handler import log_exception
+
+app.add_exception_handler(StarletteHTTPException, log_exception)
+```
+
+Json Exception handler uses logger "http_error_logger", what could be use for reporting concepts
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
```

### Comparing `sag-py-web-common-0.1.0/README.md` & `sag-py-web-common-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -52,24 +52,34 @@
 )
 ```
 
 Also see this page for further configuration details: https://github.com/Kludex/asgi-logger
 
 ### Json exception handler
 
-Per default fastapi falls back to text responses if there are exceptions.
+Per default fastapi falls back to text responses if there are unknown exceptions.
 That's not the desired behaviour for json api's.
 
 This handler ensures that a json is returned. It contains the field "detail" with the exception message.
 
 ```python
-from sag_py_web_common.json_exception_handler import handle_exception
+from sag_py_web_common.json_exception_handler import handle_unknown_exception
 
-app.add_exception_handler(Exception, handle_exception)
+app.add_exception_handler(Exception, handle_unknown_exception)
 ```
+Fo logging any HHTP-Exception use log_exception funktion.
+
+```python
+from starlette.exceptions import HTTPException as StarletteHTTPException
+from sag_py_web_common.json_exception_handler import log_exception
+
+app.add_exception_handler(StarletteHTTPException, log_exception)
+```
+
+Json Exception handler uses logger "http_error_logger", what could be use for reporting concepts
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
```

### Comparing `sag-py-web-common-0.1.0/sag_py_web_common/default_route.py` & `sag-py-web-common-0.1.1/sag_py_web_common/default_route.py`

 * *Files identical despite different names*

### Comparing `sag-py-web-common-0.1.0/sag_py_web_common/filtered_access_logger.py` & `sag-py-web-common-0.1.1/sag_py_web_common/filtered_access_logger.py`

 * *Files identical despite different names*

### Comparing `sag-py-web-common-0.1.0/sag_py_web_common.egg-info/PKG-INFO` & `sag-py-web-common-0.1.1/sag_py_web_common.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-web-common
-Version: 0.1.0
+Version: 0.1.1
 Summary: Small helper functions for web projects
 Home-page: https://github.com/SamhammerAG/sag_py_web_common
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_web_common
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_web_common/issues
@@ -75,24 +75,34 @@
 )
 ```
 
 Also see this page for further configuration details: https://github.com/Kludex/asgi-logger
 
 ### Json exception handler
 
-Per default fastapi falls back to text responses if there are exceptions.
+Per default fastapi falls back to text responses if there are unknown exceptions.
 That's not the desired behaviour for json api's.
 
 This handler ensures that a json is returned. It contains the field "detail" with the exception message.
 
 ```python
-from sag_py_web_common.json_exception_handler import handle_exception
+from sag_py_web_common.json_exception_handler import handle_unknown_exception
 
-app.add_exception_handler(Exception, handle_exception)
+app.add_exception_handler(Exception, handle_unknown_exception)
 ```
+Fo logging any HHTP-Exception use log_exception funktion.
+
+```python
+from starlette.exceptions import HTTPException as StarletteHTTPException
+from sag_py_web_common.json_exception_handler import log_exception
+
+app.add_exception_handler(StarletteHTTPException, log_exception)
+```
+
+Json Exception handler uses logger "http_error_logger", what could be use for reporting concepts
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
```

### Comparing `sag-py-web-common-0.1.0/setup.py` & `sag-py-web-common-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-web-common",
-    version="0.1.0",
+    version="0.1.1",
     description="Small helper functions for web projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_web_common",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

