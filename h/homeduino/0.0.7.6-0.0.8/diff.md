# Comparing `tmp/homeduino-0.0.7.6.tar.gz` & `tmp/homeduino-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeduino-0.0.7.6.tar", last modified: Sat May 27 10:13:24 2023, max compression
+gzip compressed data, was "homeduino-0.0.8.tar", last modified: Mon Jul  3 22:27:15 2023, max compression
```

## Comparing `homeduino-0.0.7.6.tar` & `homeduino-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/homeduino/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/homeduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/homeduino/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/homeduino/homeduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/homeduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:27:15.891523 homeduino-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-07-03 22:27:03.000000 homeduino-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 22:27:15.891523 homeduino-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:27:15.891523 homeduino-0.0.8/homeduino/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-03 22:27:03.000000 homeduino-0.0.8/homeduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-03 22:27:03.000000 homeduino-0.0.8/homeduino/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-03 22:27:03.000000 homeduino-0.0.8/homeduino/homeduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:27:15.891523 homeduino-0.0.8/homeduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 22:27:15.000000 homeduino-0.0.8/homeduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 22:27:15.000000 homeduino-0.0.8/homeduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:27:15.000000 homeduino-0.0.8/homeduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 22:27:15.000000 homeduino-0.0.8/homeduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 22:27:15.000000 homeduino-0.0.8/homeduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-03 22:27:03.000000 homeduino-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:27:15.891523 homeduino-0.0.8/setup.cfg
```

### Comparing `homeduino-0.0.7.6/LICENSE` & `homeduino-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7.6/PKG-INFO` & `homeduino-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7.6
+Version: 0.0.8
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7.6/homeduino/__main__.py` & `homeduino-0.0.8/homeduino/__main__.py`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7.6/homeduino/homeduino.py` & `homeduino-0.0.8/homeduino/homeduino.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,21 +139,21 @@
                 for rf_receive_callback in self.rf_receive_callbacks:
                     rf_receive_callback(protocol)
 
     def handle_key_press(self, line: str) -> None:
         logger.debug(line)
         # Ignoring key presses for now
 
-    async def send(self, packet: str) -> str:
+    async def send(self, packet: str, ignore_ready: bool = False) -> str:
         """Encode and put packet string onto write buffer."""
 
         if not self.transport:
             raise DisconnectedError("Homeduino is not connected")
 
-        if not self.ready:
+        if not ignore_ready and not self.ready:
             logger.error("Not ready")
             raise NotReadyError("Homeduino is not ready")
 
         while self.busy():
             if (datetime.now() - self._tx_busy_since).total_seconds() > _BUSY_TIMEOUT:
                 logger.error("Too busy to send %s", packet)
                 raise TooBusyError("Homeduino is too busy to send a command")
@@ -247,22 +247,28 @@
                     parity=serial_asyncio.serial.PARITY_NONE,
                     stopbits=serial_asyncio.serial.STOPBITS_ONE,
                 )
 
                 start_time = datetime.now()
                 while not self.protocol.ready:
                     if (datetime.now() - start_time).total_seconds() > _READY_TIMEOUT:
-                        logger.error(
-                            "Timeout while waiting for Homeduino to become ready"
-                        )
+                        break
+                    logger.debug("Waiting for Homeduino to become ready")
+                    await asyncio.sleep(0.01)
+
+                if not self.protocol.ready:
+                    logger.error(
+                        "Timeout while waiting for Homeduino to become ready, trying to ping instead"
+                    )
+                    if self._ping(True):
+                        self.protocol.handle_ready()
+                    else:
                         raise ResponseTimeoutError(
                             "Timeout while waiting for Homeduino to become ready"
                         )
-                    logger.debug("Waiting for Homeduino to become ready")
-                    await asyncio.sleep(0.01)
 
                 await self.protocol.set_receive_interrupt(self.receive_interrupt)
 
                 for rf_receive_callback in self.rf_receive_callbacks:
                     self.protocol.add_rf_receive_callback(rf_receive_callback)
 
                 return True
@@ -294,31 +300,34 @@
 
             self.protocol = None
             logger.debug("Homeduino disconnected")
             return True
 
         return False
 
-    async def ping(self) -> bool:
-        if not self.connected():
-            raise DisconnectedError("Homeduino is not connected")
-
-        if self.protocol.busy():
-            return True
-
+    async def _ping(self, ignore_ready: bool = False) -> bool:
         logger.debug("Pinging Homeduino")
         message = f"PING {time.time()}"
-        response = await self.protocol.send(message)
+        response = await self.protocol.send(message, ignore_ready)
         if response == message:
             logger.debug("Pinging Homeduino successful")
             return True
 
         logger.error("Pinging Homeduino failed")
         return False
 
+    async def ping(self) -> bool:
+        if not self.connected():
+            raise DisconnectedError("Homeduino is not connected")
+
+        if self.protocol.busy():
+            return True
+
+        return await self._ping()
+
     def add_rf_receive_callback(self, rf_receive_callback) -> None:
         self.rf_receive_callbacks.append(rf_receive_callback)
         if self.connected():
             self.protocol.add_rf_receive_callback(rf_receive_callback)
 
     async def rf_send(self, rf_protocol: str, values) -> bool:
         if not self.connected():
```

### Comparing `homeduino-0.0.7.6/homeduino.egg-info/PKG-INFO` & `homeduino-0.0.8/homeduino.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7.6
+Version: 0.0.8
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7.6/pyproject.toml` & `homeduino-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "homeduino"
-version = "0.0.7.6"
+version = "0.0.8"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Homeduino library"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pyserial-asyncio==0.6",
-    "rfcontrolpy==0.0.4"
+    "rfcontrolpy==0.0.5"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/rrooggiieerr/homeduino.py"
 "Bug Tracker" = "https://github.com/rrooggiieerr/homeduino.py/issues"
 
 [tool.black]
```

