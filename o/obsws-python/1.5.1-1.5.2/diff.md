# Comparing `tmp/obsws_python-1.5.1.tar.gz` & `tmp/obsws_python-1.5.2.tar.gz`

## Comparing `obsws_python-1.5.1.tar` & `obsws_python-1.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/__init__.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/baseclient.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/callback.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/error.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/events.py
--rw-r--r--   0        0        0    58004 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/reqs.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/subs.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/version.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 obsws_python-1.5.1/.gitignore
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 obsws_python-1.5.1/LICENSE
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 obsws_python-1.5.1/README.md
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 obsws_python-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4702 2020-02-02 00:00:00.000000 obsws_python-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/__init__.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/baseclient.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/callback.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/error.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/events.py
+-rw-r--r--   0        0        0    58224 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/reqs.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/subs.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 obsws_python-1.5.2/obsws_python/version.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 obsws_python-1.5.2/.gitignore
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 obsws_python-1.5.2/LICENSE
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 obsws_python-1.5.2/README.md
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 obsws_python-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 obsws_python-1.5.2/PKG-INFO
```

### Comparing `obsws_python-1.5.1/obsws_python/baseclient.py` & `obsws_python-1.5.2/obsws_python/baseclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         try:
             self.ws = websocket.WebSocket()
             self.ws.connect(f"ws://{self.host}:{self.port}", timeout=self.timeout)
             self.server_hello = json.loads(self.ws.recv())
         except ValueError as e:
             self.logger.error(f"{type(e).__name__}: {e}")
             raise
-        except (ConnectionRefusedError, WebSocketTimeoutException) as e:
+        except (ConnectionRefusedError, TimeoutError, WebSocketTimeoutException) as e:
             self.logger.exception(f"{type(e).__name__}: {e}")
             raise
 
     def _conn_from_toml(self) -> dict:
         try:
             import tomllib
         except ModuleNotFoundError:
@@ -104,17 +104,23 @@
             ).decode()
 
             payload["d"]["authentication"] = auth
 
         self.ws.send(json.dumps(payload))
         try:
             response = json.loads(self.ws.recv())
-            return response["op"] == 2
+            if response["op"] != 2:
+                raise OBSSDKError(
+                    "failed to identify client with the server, expected response with OpCode 2 Identified"
+                )
+            return response["d"]
         except json.decoder.JSONDecodeError:
-            raise OBSSDKError("failed to identify client with the server")
+            raise OBSSDKError(
+                "failed to identify client with the server, please check connection settings"
+            )
 
     def req(self, req_type, req_data=None):
         payload = {
             "op": 6,
             "d": {"requestType": req_type, "requestId": randint(1, 1000)},
         }
         if req_data:
```

### Comparing `obsws_python-1.5.1/obsws_python/callback.py` & `obsws_python-1.5.2/obsws_python/callback.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.1/obsws_python/events.py` & `obsws_python-1.5.2/obsws_python/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from threading import Thread
 
 from websocket import WebSocketTimeoutException
 
 from .baseclient import ObsClient
 from .callback import Callback
-from .error import OBSSDKTimeoutError
+from .error import OBSSDKError, OBSSDKTimeoutError
 from .subs import Subs
 
 """
 A class to interact with obs-websocket events
 defined in official github repo
 https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md#events
 """
@@ -23,16 +23,22 @@
     DELAY = 0.001
 
     def __init__(self, **kwargs):
         self.logger = logger.getChild(self.__class__.__name__)
         defaultkwargs = {"subs": Subs.LOW_VOLUME}
         kwargs = defaultkwargs | kwargs
         self.base_client = ObsClient(**kwargs)
-        if self.base_client.authenticate():
-            self.logger.info(f"Successfully identified {self} with the server")
+        try:
+            success = self.base_client.authenticate()
+            self.logger.info(
+                f"Successfully identified {self} with the server using RPC version:{success['negotiatedRpcVersion']}"
+            )
+        except OBSSDKError as e:
+            self.logger.error(f"{type(e).__name__}: {e}")
+            raise
         self.callback = Callback()
         self.subscribe()
 
     def __repr__(self):
         return type(
             self
         ).__name__ + "(host='{host}', port={port}, password='{password}', subs={subs}, timeout={timeout})".format(
```

### Comparing `obsws_python-1.5.1/obsws_python/reqs.py` & `obsws_python-1.5.2/obsws_python/reqs.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,22 @@
 logger = logging.getLogger(__name__)
 
 
 class ReqClient:
     def __init__(self, **kwargs):
         self.logger = logger.getChild(self.__class__.__name__)
         self.base_client = ObsClient(**kwargs)
-        if self.base_client.authenticate():
-            self.logger.info(f"Successfully identified {self} with the server")
+        try:
+            success = self.base_client.authenticate()
+            self.logger.info(
+                f"Successfully identified {self} with the server using RPC version:{success['negotiatedRpcVersion']}"
+            )
+        except OBSSDKError as e:
+            self.logger.error(f"{type(e).__name__}: {e}")
+            raise
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.base_client.ws.close()
```

### Comparing `obsws_python-1.5.1/obsws_python/subs.py` & `obsws_python-1.5.2/obsws_python/subs.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.1/obsws_python/util.py` & `obsws_python-1.5.2/obsws_python/util.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.1/.gitignore` & `obsws_python-1.5.2/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -41,13 +41,18 @@
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 .hatch
 
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+.python-version
+
 # Test/config
 quick.py
 config.toml
 obsws.log
 
 .vscode/
```

### Comparing `obsws_python-1.5.1/LICENSE` & `obsws_python-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.1/README.md` & `obsws_python-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.1/pyproject.toml` & `obsws_python-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.1/PKG-INFO` & `obsws_python-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: obsws-python
-Version: 1.5.1
+Version: 1.5.2
 Summary: A Python SDK for OBS Studio WebSocket v5.0
 Project-URL: Homepage, https://github.com/aatikturk/obsws-python
 Author-email: Adem Atikturk <aatikturk@gmail.com>
+License-Expression: GPL-3.0-only
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Requires-Dist: websocket-client
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
```

