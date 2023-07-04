# Comparing `tmp/fastapi_throttling-0.1.8.tar.gz` & `tmp/fastapi_throttling-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_throttling-0.1.8.tar", max compression
+gzip compressed data, was "fastapi_throttling-0.1.9.tar", max compression
```

## Comparing `fastapi_throttling-0.1.8.tar` & `fastapi_throttling-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/LICENSE
--rw-r--r--   0        0        0     1347 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/README.md
--rw-r--r--   0        0        0     1753 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       79 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/src/fastapi_throttling/__init__.py
--rw-r--r--   0        0        0     4435 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/src/fastapi_throttling/throttle.py
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-07-04 21:10:17.581446 fastapi_throttling-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1347 2023-07-04 21:10:17.581446 fastapi_throttling-0.1.9/README.md
+-rw-r--r--   0        0        0     1778 2023-07-04 21:10:17.581446 fastapi_throttling-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-07-04 21:10:17.581446 fastapi_throttling-0.1.9/src/fastapi_throttling/__init__.py
+-rw-r--r--   0        0        0     4495 2023-07-04 21:10:17.581446 fastapi_throttling-0.1.9/src/fastapi_throttling/throttle.py
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.9/PKG-INFO
```

### Comparing `fastapi_throttling-0.1.8/LICENSE` & `fastapi_throttling-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.8/README.md` & `fastapi_throttling-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.8/pyproject.toml` & `fastapi_throttling-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-throttling"
-version = "0.1.8"
+version = "0.1.9"
 description = "Limit amount of requests to your FastAPI."
 authors = ["wwnbb <wwnbb1@gmail.com>"]
 license = "GPLv2"
 readme = "README.md"
 packages = [{include = "fastapi_throttling", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -18,14 +18,15 @@
 mypy = "^1.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 httpx = "^0.24.1"
 debugpy = "^1.6.7"
 types-redis = "^4.5.5.2"
 pytest-asyncio = "^0.21.0"
+asgi-lifespan = "^2.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
```

### Comparing `fastapi_throttling-0.1.8/src/fastapi_throttling/throttle.py` & `fastapi_throttling-0.1.9/src/fastapi_throttling/throttle.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,19 +83,20 @@
         if scope["type"] != "http":
             await self.app(scope, receive, send)
             return
 
         try:
             client_ip = self.get_client_ip(scope)
         except Exception as e:
-            logger.exception(e)
+            logger.debug(e)
+            logger.info("cannot retrieve user ip Address")
             client_ip = None
 
         # Throttle by IP
-        if client_ip and await self.has_exceeded_rate_limit(client_ip):
+        if client_ip and await self.has_exceeded_rate_limit(str(client_ip)):
             response = ThrottlingResponse()
             await response(scope, receive, send)
             return
 
         token = self.get_client_token(scope)
         # Throttle by Token
         if token and await self.has_exceeded_rate_limit(token):
```

### Comparing `fastapi_throttling-0.1.8/PKG-INFO` & `fastapi_throttling-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-throttling
-Version: 0.1.8
+Version: 0.1.9
 Summary: Limit amount of requests to your FastAPI.
 License: GPLv2
 Author: wwnbb
 Author-email: wwnbb1@gmail.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

