# Comparing `tmp/curl_cffi-0.5.6.tar.gz` & `tmp/curl_cffi-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_cffi-0.5.6.tar", last modified: Tue May 23 08:48:07 2023, max compression
+gzip compressed data, was "curl_cffi-0.5.7.tar", last modified: Tue Jul  4 10:50:13 2023, max compression
```

## Comparing `curl_cffi-0.5.6.tar` & `curl_cffi-0.5.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.463091 curl_cffi-0.5.6/curl_cffi/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/curl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/curl_cffi/ffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/ffi/cdef.c
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/ffi/shim.c
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/ffi/shim.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/curl_cffi/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/curl_cffi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/curl_cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/curl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/curl_cffi/ffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/ffi/cdef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/ffi/shim.c
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/ffi/shim.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/curl_cffi/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18640 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/curl_cffi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/setup.py
```

### Comparing `curl_cffi-0.5.6/LICENSE` & `curl_cffi-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/PKG-INFO` & `curl_cffi-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl_cffi
-Version: 0.5.6
+Version: 0.5.7
 Summary: libcurl ffi bindings for Python, with impersonation support
 Author-email: Yifei Kong <kong@yifei.me>
 License: MIT License
         
         Copyright (c) 2018 multippt
         Copyright (c) 2022 Yifei Kong
```

### Comparing `curl_cffi-0.5.6/README.md` & `curl_cffi-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/aio.py` & `curl_cffi-0.5.7/curl_cffi/aio.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/build.py` & `curl_cffi-0.5.7/curl_cffi/build.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/const.py` & `curl_cffi-0.5.7/curl_cffi/const.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/curl.py` & `curl_cffi-0.5.7/curl_cffi/curl.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/ffi/cdef.c` & `curl_cffi-0.5.7/curl_cffi/ffi/cdef.c`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/ffi/shim.c` & `curl_cffi-0.5.7/curl_cffi/ffi/shim.c`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/requests/__init__.py` & `curl_cffi-0.5.7/curl_cffi/requests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,7 +67,8 @@
 
 head = partial(request, "HEAD")
 get = partial(request, "GET")
 post = partial(request, "POST")
 put = partial(request, "PUT")
 patch = partial(request, "PATCH")
 delete = partial(request, "DELETE")
+options = partial(request, "OPTIONS")
```

### Comparing `curl_cffi-0.5.6/curl_cffi/requests/cookies.py` & `curl_cffi-0.5.7/curl_cffi/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/requests/headers.py` & `curl_cffi-0.5.7/curl_cffi/requests/headers.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi/requests/session.py` & `curl_cffi-0.5.7/curl_cffi/requests/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import sys
 import re
 import threading
 import warnings
 from enum import Enum
 from functools import partialmethod
 from io import BytesIO
 from json import dumps
@@ -21,14 +22,19 @@
 
 try:
     import eventlet.tpool
 except ImportError:
     pass
 
 
+WINDOWS_WARN = """
+WindowsProactorEventLoopPolicy is not supported, you can use the selector loop by:
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+"""
+
 class BrowserType(str, Enum):
     edge99 = "edge99"
     edge101 = "edge101"
     chrome99 = "chrome99"
     chrome100 = "chrome100"
     chrome101 = "chrome101"
     chrome104 = "chrome104"
@@ -182,15 +188,15 @@
         elif isinstance(data, bytes):
             body = data
         elif data is None:
             body = b""
         else:
             raise TypeError("data must be dict, str, BytesIO or bytes")
         if json:
-            body = dumps(json).encode()
+            body = dumps(json, separators=(",", ":")).encode()
         if body:
             c.setopt(CurlOpt.POSTFIELDS, body)
             # necessary if body contains '\0'
             c.setopt(CurlOpt.POSTFIELDSIZE, len(body))
 
         # headers
         h = Headers(self.headers)
@@ -342,15 +348,17 @@
         return rsp
 
 
 # ThreadType = Literal["eventlet", "gevent", None]
 
 
 class Session(BaseSession):
-    def __init__(self, curl: Optional[Curl] = None, thread: Optional[str] = None, **kwargs):
+    def __init__(
+        self, curl: Optional[Curl] = None, thread: Optional[str] = None, **kwargs
+    ):
         super().__init__(**kwargs)
         self._thread = thread
         self._local = threading.local()
         if curl:
             self._is_customized_curl = True
             self._local.curl = curl
         else:
@@ -435,14 +443,15 @@
 
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
     post = partialmethod(request, "POST")
     put = partialmethod(request, "PUT")
     patch = partialmethod(request, "PATCH")
     delete = partialmethod(request, "DELETE")
+    options = partialmethod(request, "OPTIONS")
 
 
 class AsyncSession(BaseSession):
     def __init__(
         self,
         *,
         loop=None,
@@ -451,14 +460,19 @@
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.loop = loop if loop is not None else asyncio.get_running_loop()
         self.acurl = async_curl if async_curl is not None else AsyncCurl(loop=self.loop)
         self.max_clients = max_clients
         self.reset()
+        if sys.version_info >= (3, 8) and sys.platform.lower().startswith("win"):
+            if isinstance(
+                asyncio.get_event_loop_policy(), asyncio.WindowsProactorEventLoopPolicy
+            ):
+                warnings.warn(WINDOWS_WARN)
 
     def reset(self):
         self.pool = asyncio.LifoQueue(self.max_clients)
         while True:
             try:
                 self.pool.put_nowait(None)
             except asyncio.QueueFull:
@@ -545,7 +559,8 @@
 
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
     post = partialmethod(request, "POST")
     put = partialmethod(request, "PUT")
     patch = partialmethod(request, "PATCH")
     delete = partialmethod(request, "DELETE")
+    options = partialmethod(request, "OPTIONS")
```

### Comparing `curl_cffi-0.5.6/curl_cffi.egg-info/PKG-INFO` & `curl_cffi-0.5.7/curl_cffi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl-cffi
-Version: 0.5.6
+Version: 0.5.7
 Summary: libcurl ffi bindings for Python, with impersonation support
 Author-email: Yifei Kong <kong@yifei.me>
 License: MIT License
         
         Copyright (c) 2018 multippt
         Copyright (c) 2022 Yifei Kong
```

### Comparing `curl_cffi-0.5.6/curl_cffi.egg-info/SOURCES.txt` & `curl_cffi-0.5.7/curl_cffi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/curl_cffi.egg-info/requires.txt` & `curl_cffi-0.5.7/curl_cffi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.6/pyproject.toml` & `curl_cffi-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curl_cffi"
-version = "0.5.6"
+version = "0.5.7"
 authors = [{ name = "Yifei Kong", email = "kong@yifei.me" }]
 description = "libcurl ffi bindings for Python, with impersonation support"
 license = { file = "LICENSE" }
 dependencies = ["cffi>=1.12.0"]
 readme = "README.md"
 requires-python = ">=3.7"
 urls = { "repository" = "https://github.com/yifeikong/curl_cffi" }
```

### Comparing `curl_cffi-0.5.6/setup.py` & `curl_cffi-0.5.7/setup.py`

 * *Files identical despite different names*

