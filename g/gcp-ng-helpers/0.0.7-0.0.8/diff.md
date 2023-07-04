# Comparing `tmp/gcp_ng_helpers-0.0.7.tar.gz` & `tmp/gcp_ng_helpers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_ng_helpers-0.0.7.tar", last modified: Tue Jul  4 10:56:27 2023, max compression
+gzip compressed data, was "gcp_ng_helpers-0.0.8.tar", last modified: Tue Jul  4 14:58:33 2023, max compression
```

## Comparing `gcp_ng_helpers-0.0.7.tar` & `gcp_ng_helpers-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_helpers/cloud_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/cloud_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/cloud_tasks/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_helpers/firestore/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/firestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/firestore/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_helpers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/functions/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/gcp_helpers/functions/routers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 10:56:27.000000 gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 10:56:15.000000 gcp_ng_helpers-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-04 10:56:27.393393 gcp_ng_helpers-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-04 14:58:33.593765 gcp_ng_helpers-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_helpers/cloud_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/cloud_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/cloud_tasks/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_helpers/firestore/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/firestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/firestore/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_helpers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/functions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/gcp_helpers/functions/routers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:33.589765 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 14:58:33.000000 gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 14:58:22.000000 gcp_ng_helpers-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-04 14:58:33.593765 gcp_ng_helpers-0.0.8/setup.cfg
```

### Comparing `gcp_ng_helpers-0.0.7/LICENSE` & `gcp_ng_helpers-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.7/PKG-INFO` & `gcp_ng_helpers-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp_ng_helpers
-Version: 0.0.7
+Version: 0.0.8
 Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,30 @@
 def hello_route(request: Request) -> Response:
     return make_response('Hello', 200)
 
 
 router = HttpRouter()
 router.register(hello_route, '/hello', 'GET')
 
+
+def main(request):
+    return router.response(request)
+```
+or
+```python
+from flask import Request, Response, make_response
+from gcp_helpers.functions.routers import HttpRouter
+
+router = HttpRouter()
+
+@router.route("/hello", 'GET')
+def hello_route(request: Request) -> Response:
+    return make_response('Hello', 200)
+
+
 def main(request):
     return router.response(request)
 ```
 # Tasks submodule
 ## Manager
 CloudTasksManager class is wrapper for cloud task api. Allows to shorten task creation.
 Currently, supports only http task creation
```

### Comparing `gcp_ng_helpers-0.0.7/README.md` & `gcp_ng_helpers-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,30 @@
 def hello_route(request: Request) -> Response:
     return make_response('Hello', 200)
 
 
 router = HttpRouter()
 router.register(hello_route, '/hello', 'GET')
 
+
+def main(request):
+    return router.response(request)
+```
+or
+```python
+from flask import Request, Response, make_response
+from gcp_helpers.functions.routers import HttpRouter
+
+router = HttpRouter()
+
+@router.route("/hello", 'GET')
+def hello_route(request: Request) -> Response:
+    return make_response('Hello', 200)
+
+
 def main(request):
     return router.response(request)
 ```
 # Tasks submodule
 ## Manager
 CloudTasksManager class is wrapper for cloud task api. Allows to shorten task creation.
 Currently, supports only http task creation
```

### Comparing `gcp_ng_helpers-0.0.7/gcp_helpers/cloud_tasks/manager.py` & `gcp_ng_helpers-0.0.8/gcp_helpers/cloud_tasks/manager.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.7/gcp_helpers/firestore/collections.py` & `gcp_ng_helpers-0.0.8/gcp_helpers/firestore/collections.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.7/gcp_helpers/functions/decorators.py` & `gcp_ng_helpers-0.0.8/gcp_helpers/functions/decorators.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.7/gcp_helpers/functions/routers.py` & `gcp_ng_helpers-0.0.8/gcp_helpers/functions/routers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import json
+from collections import defaultdict
 from typing import Callable
 
 from flask import Request, make_response, Response
 
 
 class HttpRouter:
     def __init__(self, prefix=''):
         self.__route_prefix = self._strip_path(prefix)
-        self._routes = {}
+        self._routes = defaultdict(dict)
+
+    def route(self, path: str, method: str = 'GET') -> Callable:
+        def decorator(func: Callable) -> Callable:
+            formatted_path = self._format_path(path)
+            self.register(func, formatted_path, method)
+            return func
+
+        return decorator
 
     @staticmethod
     def _strip_path(path: str):
         return path.strip().strip('/').strip()
 
     def _format_path(self, path: str):
         if self.__route_prefix != '':
             return f'/{self.__route_prefix}/{self._strip_path(path)}'
         else:
             return f'/{self._strip_path(path)}'
 
-    def register(self, handler: Callable, path: str, method: str = 'GET'):
-        if method not in self._routes:
-            self._routes.update({method: {self._format_path(path): handler}})
-        else:
-            self._routes[method].update({self._format_path(path): handler})
+    def register(self, handler: Callable[[Request], Response], path: str, method: str = 'GET'):
+        self._routes[method][path] = handler
 
     def _list_routes(self):
         print(json.dumps(self._routes, indent=2, default=str))
 
     def response(self, request: Request) -> Response:
-        if request.method not in self._routes.keys():
+        if request.method not in self._routes:
             return make_response("Method not allowed", 405)
 
         if request.path not in self._routes[request.method]:
             return make_response("Not found", 404)
 
         return self._routes[request.method][request.path](request)
-
-
-
-
-
```

### Comparing `gcp_ng_helpers-0.0.7/gcp_ng_helpers.egg-info/PKG-INFO` & `gcp_ng_helpers-0.0.8/gcp_ng_helpers.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-ng-helpers
-Version: 0.0.7
+Version: 0.0.8
 Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,30 @@
 def hello_route(request: Request) -> Response:
     return make_response('Hello', 200)
 
 
 router = HttpRouter()
 router.register(hello_route, '/hello', 'GET')
 
+
+def main(request):
+    return router.response(request)
+```
+or
+```python
+from flask import Request, Response, make_response
+from gcp_helpers.functions.routers import HttpRouter
+
+router = HttpRouter()
+
+@router.route("/hello", 'GET')
+def hello_route(request: Request) -> Response:
+    return make_response('Hello', 200)
+
+
 def main(request):
     return router.response(request)
 ```
 # Tasks submodule
 ## Manager
 CloudTasksManager class is wrapper for cloud task api. Allows to shorten task creation.
 Currently, supports only http task creation
```

### Comparing `gcp_ng_helpers-0.0.7/setup.cfg` & `gcp_ng_helpers-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_file = LICENSE
 name = gcp_ng_helpers
-version = 0.0.7
+version = 0.0.8
 author = Dmitriy Tischenko aka NGhost
 author_email = nghostik@gmail.com
 description = Various helper functions for Google Cloud services
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/NGhostClub/gcp-helpers
 project_urls =
```

