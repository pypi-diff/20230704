# Comparing `tmp/bondzai.gateway-0.0.4.tar.gz` & `tmp/bondzai.gateway-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-0.0.4.tar", last modified: Wed Jun 21 16:07:31 2023, max compression
+gzip compressed data, was "bondzai.gateway-0.0.5.tar", last modified: Tue Jul  4 09:34:06 2023, max compression
```

## Comparing `bondzai.gateway-0.0.4.tar` & `bondzai.gateway-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.212741 bondzai.gateway-0.0.4/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      596 2023-06-21 16:07:31.212947 bondzai.gateway-0.0.4/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      195 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.188564 bondzai.gateway-0.0.4/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.191439 bondzai.gateway-0.0.4/bondzai/gateway/
--rw-r--r--   0 theo       (501) staff       (20)      775 2023-06-21 16:07:13.000000 bondzai.gateway-0.0.4/bondzai/gateway/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)      843 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/config.yml
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.196559 bondzai.gateway-0.0.4/bondzai/gateway/core/
--rw-r--r--   0 theo       (501) staff       (20)     7995 2023-06-21 16:06:07.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/application.py
--rw-r--r--   0 theo       (501) staff       (20)      328 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/device.py
--rw-r--r--   0 theo       (501) staff       (20)      577 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/events.py
--rw-r--r--   0 theo       (501) staff       (20)      833 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/fsm.py
--rw-r--r--   0 theo       (501) staff       (20)     2127 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/logger.py
--rw-r--r--   0 theo       (501) staff       (20)     2590 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/manager.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.202196 bondzai.gateway-0.0.4/bondzai/gateway/core/message/
--rw-r--r--   0 theo       (501) staff       (20)     5283 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/message/base.py
--rw-r--r--   0 theo       (501) staff       (20)     4968 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/message/command.py
--rw-r--r--   0 theo       (501) staff       (20)     6243 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/message/enums.py
--rw-r--r--   0 theo       (501) staff       (20)     3942 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/message/event.py
--rw-r--r--   0 theo       (501) staff       (20)      337 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/message/payload.py
--rw-r--r--   0 theo       (501) staff       (20)     6376 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/message/process_dbm.py
--rw-r--r--   0 theo       (501) staff       (20)     7864 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/message/response.py
--rw-r--r--   0 theo       (501) staff       (20)      942 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/message/utils.py
--rw-r--r--   0 theo       (501) staff       (20)     2276 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/observer.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.204751 bondzai.gateway-0.0.4/bondzai/gateway/core/websocket/
--rw-r--r--   0 theo       (501) staff       (20)     1768 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/websocket/client.py
--rw-r--r--   0 theo       (501) staff       (20)     2652 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/websocket/connector.py
--rw-r--r--   0 theo       (501) staff       (20)     1731 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/websocket/request.py
--rw-r--r--   0 theo       (501) staff       (20)      171 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/core/websocket/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.206610 bondzai.gateway-0.0.4/bondzai/gateway/device_connectors/
--rw-r--r--   0 theo       (501) staff       (20)      201 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/device_connectors/base.py
--rw-r--r--   0 theo       (501) staff       (20)     4426 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/device_connectors/serial.py
--rw-r--r--   0 theo       (501) staff       (20)     7630 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/device_connectors/socket_server.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.207563 bondzai.gateway-0.0.4/bondzai/gateway/tests/
--rw-r--r--   0 theo       (501) staff       (20)        0 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/tests/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2280 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/bondzai/gateway/tests/test_observer.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:07:31.212186 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      596 2023-06-21 16:07:31.000000 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1382 2023-06-21 16:07:31.000000 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 16:07:31.000000 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)       57 2023-06-21 16:07:31.000000 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/entry_points.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-21 16:07:31.000000 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)      117 2023-06-21 16:07:31.000000 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-06-21 16:07:31.000000 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 16:07:30.000000 bondzai.gateway-0.0.4/bondzai.gateway.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-06-21 15:39:32.000000 bondzai.gateway-0.0.4/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      913 2023-06-21 16:07:31.214531 bondzai.gateway-0.0.4/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.763127 bondzai.gateway-0.0.5/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-04 09:34:06.763260 bondzai.gateway-0.0.5/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      195 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.747844 bondzai.gateway-0.0.5/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.750706 bondzai.gateway-0.0.5/bondzai/gateway/
+-rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)      843 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/config.yml
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.752849 bondzai.gateway-0.0.5/bondzai/gateway/core/
+-rw-r--r--   0 theo       (501) staff       (20)     7995 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/application.py
+-rw-r--r--   0 theo       (501) staff       (20)      328 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/device.py
+-rw-r--r--   0 theo       (501) staff       (20)      577 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/events.py
+-rw-r--r--   0 theo       (501) staff       (20)      833 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/fsm.py
+-rw-r--r--   0 theo       (501) staff       (20)     2127 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/logger.py
+-rw-r--r--   0 theo       (501) staff       (20)     2590 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/manager.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.755313 bondzai.gateway-0.0.5/bondzai/gateway/core/message/
+-rw-r--r--   0 theo       (501) staff       (20)     5391 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/base.py
+-rw-r--r--   0 theo       (501) staff       (20)     4968 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/command.py
+-rw-r--r--   0 theo       (501) staff       (20)     6661 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)     6771 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/event.py
+-rw-r--r--   0 theo       (501) staff       (20)      337 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/payload.py
+-rw-r--r--   0 theo       (501) staff       (20)     6821 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/process_dbm.py
+-rw-r--r--   0 theo       (501) staff       (20)     7864 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/response.py
+-rw-r--r--   0 theo       (501) staff       (20)      942 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/utils.py
+-rw-r--r--   0 theo       (501) staff       (20)     2276 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/observer.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.756542 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/
+-rw-r--r--   0 theo       (501) staff       (20)     1768 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/client.py
+-rw-r--r--   0 theo       (501) staff       (20)     2652 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/connector.py
+-rw-r--r--   0 theo       (501) staff       (20)     1731 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/request.py
+-rw-r--r--   0 theo       (501) staff       (20)      171 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.758214 bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/
+-rw-r--r--   0 theo       (501) staff       (20)      201 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/base.py
+-rw-r--r--   0 theo       (501) staff       (20)     4426 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/serial.py
+-rw-r--r--   0 theo       (501) staff       (20)     7630 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/socket_server.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.759113 bondzai.gateway-0.0.5/bondzai/gateway/tests/
+-rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/tests/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2280 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/tests/test_observer.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.762886 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)     1382 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)       57 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/entry_points.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)      117 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      913 2023-07-04 09:34:06.764018 bondzai.gateway-0.0.5/setup.cfg
```

### Comparing `bondzai.gateway-0.0.4/NOTICE` & `bondzai.gateway-0.0.5/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/PKG-INFO` & `bondzai.gateway-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/__init__.py` & `bondzai.gateway-0.0.5/bondzai/gateway/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 from pathlib import Path
 
 from .core.application import Application, CONFIG_DEFAULT_PATH
 
 
 CMD_NAME = "bondzai.gateway"
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 def run():
     parser = argparse.ArgumentParser(
         prog=CMD_NAME,
         description="Davinsy Gateway"
     )
```

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/config.yml` & `bondzai.gateway-0.0.5/bondzai/gateway/config.yml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/application.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/application.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/events.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/fsm.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/fsm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/logger.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/logger.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/manager.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/manager.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/message/base.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/message/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,39 +48,44 @@
 
 class Message(object):
     def __init__(self, raw_data: list = None) -> None:
         self.header: MsgHeader = MsgHeader(*raw_data[:5]) if raw_data is not None else None
         self.payloads: list[MessagePayload] = []
 
         if raw_data is not None:
+            payload = None
             if self.header.typ == MSG_TYP.EVENT.value:
-                self.payloads.append(EventMessagePayload.from_array(
+                payload = EventMessagePayload.from_array(
                     self.header.op, 
                     raw_data[5:]
-                ))
+                )
             elif self.header.typ == MSG_TYP.COMMAND.value:
-                self.payloads.append(CommandMessagePayload.from_array(
+                payload = CommandMessagePayload.from_array(
                     self.header.mod,
                     self.header.op, 
                     raw_data[5:]
-                ))
+                )
             elif self.header.typ == MSG_TYP.RESPONSE.value:
-                self.payloads.append(ResponseMessagePayload.from_array(
+                payload = ResponseMessagePayload.from_array(
                     self.header.mod,
                     self.header.op, 
                     raw_data[5:]
-                ))
+                )
             else:
                 log(f"Unknown type {str(self.header.typ)}", logger_level="ERROR")
+                
+            if payload is not None:
+                self.payloads.append(payload)
 
     def to_dict(self) -> dict:
-        return {
+        res = {
             "header": self.header.to_dict(),
             "payloads": [p.to_dict() for p in self.payloads]
         }
+        return res
 
     def to_json(self) -> str:
         return msg_serialize(self.to_dict())
 
     @classmethod
     def from_json(cls, json_data: str) -> "Message":
         try:
```

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/message/command.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/message/command.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/message/enums.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/message/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,29 @@
 
 
 class EventOperationID(Enum):
     EVT_EXT_EXCEPTION = 0x00
     EVT_EXT_DATA_IN = 0x01
     EVT_EXT_CMD_STATUS = 0x100
     EVT_EXT_LOG = 0x101
-    EVT_EXT_POSTPROC = 0x200
+    EVT_EXT_VM_RESULT = 0x200
+    EVT_EXT_ASL_RESULT = 0x201
+    EVT_EXT_SET_MODE = 0x300
+    EVT_EXT_CORRECTION = 0x301
+    EVT_EXT_TRIGGER = 0x302
     EVT_EXT_CUSTOM_1 = 0xF00
     EVT_EXT_CUSTOM_2 = 0xF01
     EVT_EXT_CUSTOM_3 = 0xF02
     EVT_EXT_CUSTOM_4 = 0xF03
+    EVT_EXT_CUSTOM_5 = 0xF04
+    EVT_EXT_CUSTOM_6 = 0xF05
+    EVT_EXT_CUSTOM_7 = 0xF06
+    EVT_EXT_CUSTOM_8 = 0xF07
+    EVT_EXT_CUSTOM_9 = 0xF08
+    EVT_EXT_CUSTOM_10 = 0xF09
     EVT_INT_EXCEPTION = 0x1000
     EVT_INT_DATA_STORED = 0x1001
     EVT_INT_DISCOVERY = 0x1002
     EVT_INT_TRANSPORT = 0x1003
     EVT_INT_DATA_UPDATED = 0x1100
     EVT_INT_READY_TO_PREPROC_BATCH = 0x1101
     EVT_INT_PREPROC_BATCH_DONE = 0x1102
@@ -59,14 +69,20 @@
 class AgentAIMode(Enum):
     APP_AI_MODE_NOT_INIT = -1
     APP_AI_MODE_STANDBY = 0
     APP_AI_MODE_ENROLLEMENT = 1
     APP_AI_MODE_INFERENCE = 2
 
 
+class AgentAIType(Enum):
+    APP_AI_TYPE_NOT_INIT = -1
+    APP_AI_TYPE_CLASSIFICATION = 0
+    APP_AI_TYPE_REGRESSION = 1
+
+
 class PPOperationUID(Enum):
     OPS_ID_EXT = 0x80000000
     OPS_ID = 0x00000000
     OPS_MISC = 0x00000000
     OPS_MATH = 0x01000000
     OPS_DSP = 0x02000000
     OPS_IMG = 0x03000000
```

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/message/process_dbm.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/message/process_dbm.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,16 +61,24 @@
                         "row" : el[0] if len(el[0]) else el[1],
                         "labels": [
                             lbl for lbl in (el[1] if len(el[0]) else el[2]) 
                         ]                        
                     }
                     self.attributes["desc"]["filter"]["filters"].append(filt)            
             elif att in [DBM_ATT_VM.PREPROC_GRAPH_TRAIN.value, DBM_ATT_VM.PREPROC_GRAPH_INFER.value, DBM_ATT_VM.PREPROC_GRAPH_OTHER.value]:
-                nodes = []
-                for n in raw_data[att]:
+                graph = {
+                    "memneed": {
+                        "outlen": raw_data[att][0],
+                        "templen": raw_data[att][1],
+                    },
+                    "sizeout": raw_data[att][2],
+                }
+                
+                nodes = []                
+                for n in raw_data[att][3]:
                     nodes.append({
                         "op_id": n[0],
                         "memneed": {
                             "outlen": n[1],
                             "templen": n[2]
                         },
                         "mem_policy": n[3],
@@ -83,15 +91,16 @@
 
                     k = "preproc_other"
                     if att == DBM_ATT_VM.PREPROC_GRAPH_TRAIN.value:
                         k = "preproc_train"
                     elif att==DBM_ATT_VM.PREPROC_GRAPH_INFER.value:
                         k = "preproc_infer" 
 
-                    self.attributes[k] = nodes
+                    graph["nodes"] = nodes
+                    self.attributes[k] = graph
             elif att == DBM_ATT_VM.DEEPLOMATH.value :
                 self.attributes["deeplomath"] = {
                     "mode": raw_data[att][0],
                     "rejection": raw_data[att][1],
                     "dim_in": raw_data[att][2],
                     "dim_out": raw_data[att][3],
                     "max_layers": raw_data[att][4]
@@ -128,15 +137,18 @@
                     self.attributes["label"]["labels"] = [{
                         "type":     l[0] if len(l[0]) else l[1],
                         "label":    l[2] if not len(l[0]) else l[1]
                     } for l in raw_data[att][2]]
                 else:
                     self.attributes["label"]["values"] = raw_data[att][2]                
             elif att == DBM_ATT_DAT.DATA.value:
-                self.attributes["record"] = B2B64(b"".join(raw_data[att]))\
+
+                raw_data_l = raw_data[att][0]
+                raw_data_bytes = raw_data[att][1]
+                self.attributes["record"] = B2B64(b"".join(raw_data_bytes))\
 
     def to_dict(self):
         return self.attributes
 
 
 class DbmExportKey(object):
     pass
@@ -165,14 +177,15 @@
 }
 
 
 class DbmProcesser(object):
     @classmethod
     def from_msgpack(cls, data: bytearray) -> "DbmProcesser":
         try:
+
             stream = BytesIO(data)
             unpacker = msgpack.Unpacker(stream, raw=False, strict_map_key=False)
 
             table_type = unpacker.unpack()
 
             nb_attributes = unpacker.read_map_header()
```

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/message/response.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/message/response.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/message/utils.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/message/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/observer.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/websocket/client.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/client.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/websocket/connector.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/connector.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/core/websocket/request.py` & `bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/request.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/device_connectors/serial.py` & `bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/serial.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/device_connectors/socket_server.py` & `bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/socket_server.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai/gateway/tests/test_observer.py` & `bondzai.gateway-0.0.5/bondzai/gateway/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/bondzai.gateway.egg-info/PKG-INFO` & `bondzai.gateway-0.0.5/bondzai.gateway.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.4/bondzai.gateway.egg-info/SOURCES.txt` & `bondzai.gateway-0.0.5/bondzai.gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.4/setup.cfg` & `bondzai.gateway-0.0.5/setup.cfg`

 * *Files identical despite different names*

