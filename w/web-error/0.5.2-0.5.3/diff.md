# Comparing `tmp/web_error-0.5.2.tar.gz` & `tmp/web_error-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_error-0.5.2.tar", max compression
+gzip compressed data, was "web_error-0.5.3.tar", max compression
```

## Comparing `web_error-0.5.2.tar` & `web_error-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11307 2020-10-05 08:06:50.313394 web_error-0.5.2/LICENSE
--rw-r--r--   0        0        0     3068 2023-04-25 17:11:29.892937 web_error-0.5.2/README.md
--rw-r--r--   0        0        0     1772 2023-04-25 17:11:29.892937 web_error-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-04-25 17:11:29.892937 web_error-0.5.2/web_error/__init__.py
--rw-r--r--   0        0        0       76 2023-02-19 13:27:57.835626 web_error-0.5.2/web_error/constant.py
--rw-r--r--   0        0        0     1700 2023-02-19 13:32:08.909713 web_error-0.5.2/web_error/error.py
--rw-r--r--   0        0        0        0 2020-10-05 09:05:22.710518 web_error-0.5.2/web_error/handler/__init__.py
--rw-r--r--   0        0        0     1268 2023-02-19 13:23:27.856394 web_error-0.5.2/web_error/handler/aiohttp.py
--rw-r--r--   0        0        0     2521 2023-04-25 17:03:40.700398 web_error-0.5.2/web_error/handler/fastapi.py
--rw-r--r--   0        0        0     1116 2023-02-19 13:20:25.477898 web_error-0.5.2/web_error/handler/flask.py
--rw-r--r--   0        0        0     1528 2023-02-19 13:19:46.823583 web_error-0.5.2/web_error/handler/pyramid.py
--rw-r--r--   0        0        0     3725 2023-02-19 13:25:07.941219 web_error-0.5.2/web_error/handler/starlette.py
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 web_error-0.5.2/setup.py
--rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 web_error-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11307 2020-10-05 08:06:50.313394 web_error-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3068 2023-07-04 14:30:04.309661 web_error-0.5.3/README.md
+-rw-r--r--   0        0        0     1772 2023-07-04 14:30:04.309661 web_error-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-04 14:30:04.309661 web_error-0.5.3/web_error/__init__.py
+-rw-r--r--   0        0        0       76 2023-02-19 13:27:57.835626 web_error-0.5.3/web_error/constant.py
+-rw-r--r--   0        0        0     1700 2023-02-19 13:32:08.909713 web_error-0.5.3/web_error/error.py
+-rw-r--r--   0        0        0        0 2020-10-05 09:05:22.710518 web_error-0.5.3/web_error/handler/__init__.py
+-rw-r--r--   0        0        0     1268 2023-02-19 13:23:27.856394 web_error-0.5.3/web_error/handler/aiohttp.py
+-rw-r--r--   0        0        0     2731 2023-07-04 14:29:08.091382 web_error-0.5.3/web_error/handler/fastapi.py
+-rw-r--r--   0        0        0     1116 2023-02-19 13:20:25.477898 web_error-0.5.3/web_error/handler/flask.py
+-rw-r--r--   0        0        0     1528 2023-02-19 13:19:46.823583 web_error-0.5.3/web_error/handler/pyramid.py
+-rw-r--r--   0        0        0     3725 2023-02-19 13:25:07.941219 web_error-0.5.3/web_error/handler/starlette.py
+-rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 web_error-0.5.3/PKG-INFO
```

### Comparing `web_error-0.5.2/LICENSE` & `web_error-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `web_error-0.5.2/README.md` & `web_error-0.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Web Errors v0.5.2
+# Web Errors v0.5.3
 [![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)
 ![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)
 ![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)
 [![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)
```

### Comparing `web_error-0.5.2/pyproject.toml` & `web_error-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web_error"
-version = "0.5.2"
+version = "0.5.3"
 description = "Web based error utils"
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/EdgyEdgemond/web-error/"
 homepage="https://github.com/EdgyEdgemond/web-error/"
 readme = "README.md"
```

### Comparing `web_error-0.5.2/web_error/error.py` & `web_error-0.5.3/web_error/error.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.2/web_error/handler/aiohttp.py` & `web_error-0.5.3/web_error/handler/aiohttp.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.2/web_error/handler/fastapi.py` & `web_error-0.5.3/web_error/handler/fastapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from web_error import constant
 from web_error.error import HttpException
 from web_error.handler import starlette
 
 logger = logging.getLogger(__name__)
 
 
-def _handle_exception(exc: Exception) -> Tuple[dict, str]:
+def _handle_exception(exc: Exception, *, debug_enabled: bool = True) -> Tuple[dict, str]:
     status = constant.SERVER_ERROR
     message = "Unhandled exception occurred."
     response = {
         "message": message,
         "debug_message": str(exc),
         "code": None,
     }
@@ -33,24 +33,28 @@
     if isinstance(exc, HttpException):
         response = exc.marshal()
         status = exc.status
 
     if status >= constant.SERVER_ERROR:
         logger.exception(message, exc_info=(type(exc), exc, exc.__traceback__))
 
+    if not debug_enabled:
+        response.pop("debug_message", None)
+
     return response, status
 
 
 class ExceptionHandler:
-    def __init__(self, unhandled_code: str, request_validation_code: str) -> None:
+    def __init__(self, unhandled_code: str, request_validation_code: str, *, debug_enabled: bool = True) -> None:
         self.unhandled_code = unhandled_code
         self.request_validation_code = request_validation_code
+        self.debug_enabled = debug_enabled
 
     def __call__(self, request: starlette.Request, exc: Exception) -> starlette.JSONResponse:  # noqa: ARG002
-        response, status = _handle_exception(exc)
+        response, status = _handle_exception(exc, debug_enabled=self.debug_enabled)
 
         if response["code"] is None:
             response["code"] = self.request_validation_code if status == 422 else self.unhandled_code  # noqa: PLR2004
 
         return starlette.JSONResponse(
             status_code=status,
             content=response,
```

### Comparing `web_error-0.5.2/web_error/handler/flask.py` & `web_error-0.5.3/web_error/handler/flask.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.2/web_error/handler/pyramid.py` & `web_error-0.5.3/web_error/handler/pyramid.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.2/web_error/handler/starlette.py` & `web_error-0.5.3/web_error/handler/starlette.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.2/setup.py` & `web_error-0.5.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,128 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: web-error
+Version: 0.5.3
+Summary: Web based error utils
+Home-page: https://github.com/EdgyEdgemond/web-error/
+License: Apache-2.0
+Author: Daniel Edgecombe
+Author-email: edgy.edgemond@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/EdgyEdgemond/web-error/
+Description-Content-Type: text/markdown
 
-packages = \
-['web_error', 'web_error.handler']
+# Web Errors v0.5.3
+[![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)
+[![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)
+[![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)
+![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)
+![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)
+[![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)
 
-package_data = \
-{'': ['*']}
+`web_error` is a set of exceptions and handlers for use in web apis to support easy error management and responses
 
-setup_kwargs = {
-    'name': 'web-error',
-    'version': '0.5.2',
-    'description': 'Web based error utils',
-    'long_description': '# Web Errors v0.5.2\n[![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)\n[![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)\n[![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)\n![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)\n![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)\n[![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)\n\n`web_error` is a set of exceptions and handlers for use in web apis to support easy error management and responses\n\nEach exception easily marshals to JSON for use in api errors. Handlers for different web frameworks are provided.\n\n\n## Errors\n\nThe base `web_error.error.HttpException` accepts a `message`, `debug_message`, `code` and `status` (default 500)\n\nAnd will render a response with status as the status code:\n\n```json\n{\n    "code": "code",\n    "message": "message",\n    "debug_message": "debug_message",\n}\n```\n\nSome convenience Exceptions are provided, to create custom error subclass these\nand define `message` and `code` attributes.\n\n* `web_error.error.ServerException` provides status 500 errors\n* `web_error.error.BadRequestException` provides status 400 errors\n* `web_error.error.UnauthorisedException` provides status 401 errors\n* `web_error.error.NotFoundException` provides status 404 errors\n\n### Custom Errors\n\nSubclassing the convenience classes provide a simple way to consistently raise the same error\nand message.\n\nCode is an optional attribute to provide a unique value to parse in a frontend/client instead of\nmatching against messages.\n\n```python\nfrom web_error.error import NotFoundException\n\n\nclass UserNotFoundError(NotFoundException):\n    message = "User not found."\n    code = "E001"\n```\n\n\n## FastAPI\n\nInclude the `exception_handler` in your app.\n\n```python\n    exception_handler = web_error.handler.fastapi.exception_handler\n\n    return FastAPI(\n        exception_handlers={\n            Exception: exception_handler,\n            RequestValidationError: exception_handler,\n            HTTPException: exception_handler,\n        },\n    )\n```\n## Pyramid\n\nInclude the pyramid exception handlers in your config.\n\n```python\ndef main(global_config, **config_blob):\n    config = Configurator(settings=config_blob)\n\n    ...\n\n    config.scan("web_error.handler.pyramid")\n\n    return config.make_wsgi_app()\n```\n\nThis will handle all unexpected errors, and any app specific errors.\n\n```python\n@view_config(route_name="test", renderer="json")\ndef test(request):\n    raise UserNotFoundError("debug message")\n```\n\n\n## Flask\n\nRegister the error handler with your application\n\n```python\napp.register_error_handler(Exception, web_error.handler.flask.exception_handler)\n```\n\n## Aiohttp\n\nDecorate your views with the error handler.\n\n```python\n@web_error.handler.aiohttp.view_error_handler\nasync def user(self):\n    raise UserNotFoundError("debug message")\n```\n',
-    'author': 'Daniel Edgecombe',
-    'author_email': 'edgy.edgemond@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/EdgyEdgemond/web-error/',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+Each exception easily marshals to JSON for use in api errors. Handlers for different web frameworks are provided.
+
+
+## Errors
+
+The base `web_error.error.HttpException` accepts a `message`, `debug_message`, `code` and `status` (default 500)
+
+And will render a response with status as the status code:
+
+```json
+{
+    "code": "code",
+    "message": "message",
+    "debug_message": "debug_message",
 }
+```
+
+Some convenience Exceptions are provided, to create custom error subclass these
+and define `message` and `code` attributes.
+
+* `web_error.error.ServerException` provides status 500 errors
+* `web_error.error.BadRequestException` provides status 400 errors
+* `web_error.error.UnauthorisedException` provides status 401 errors
+* `web_error.error.NotFoundException` provides status 404 errors
+
+### Custom Errors
+
+Subclassing the convenience classes provide a simple way to consistently raise the same error
+and message.
+
+Code is an optional attribute to provide a unique value to parse in a frontend/client instead of
+matching against messages.
+
+```python
+from web_error.error import NotFoundException
+
+
+class UserNotFoundError(NotFoundException):
+    message = "User not found."
+    code = "E001"
+```
+
+
+## FastAPI
+
+Include the `exception_handler` in your app.
+
+```python
+    exception_handler = web_error.handler.fastapi.exception_handler
+
+    return FastAPI(
+        exception_handlers={
+            Exception: exception_handler,
+            RequestValidationError: exception_handler,
+            HTTPException: exception_handler,
+        },
+    )
+```
+## Pyramid
+
+Include the pyramid exception handlers in your config.
+
+```python
+def main(global_config, **config_blob):
+    config = Configurator(settings=config_blob)
+
+    ...
+
+    config.scan("web_error.handler.pyramid")
+
+    return config.make_wsgi_app()
+```
+
+This will handle all unexpected errors, and any app specific errors.
+
+```python
+@view_config(route_name="test", renderer="json")
+def test(request):
+    raise UserNotFoundError("debug message")
+```
+
+
+## Flask
+
+Register the error handler with your application
+
+```python
+app.register_error_handler(Exception, web_error.handler.flask.exception_handler)
+```
+
+## Aiohttp
+
+Decorate your views with the error handler.
 
+```python
+@web_error.handler.aiohttp.view_error_handler
+async def user(self):
+    raise UserNotFoundError("debug message")
+```
 
-setup(**setup_kwargs)
```

