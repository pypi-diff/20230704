# Comparing `tmp/bondzai.gateway-sdk-0.0.4.tar.gz` & `tmp/bondzai.gateway-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-sdk-0.0.4.tar", last modified: Wed Jun 21 16:31:54 2023, max compression
+gzip compressed data, was "bondzai.gateway-sdk-0.0.5.tar", last modified: Tue Jul  4 09:34:26 2023, max compression
```

## Comparing `bondzai.gateway-sdk-0.0.4.tar` & `bondzai.gateway-sdk-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:31:54.049295 bondzai.gateway-sdk-0.0.4/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      604 2023-06-21 16:31:54.049514 bondzai.gateway-sdk-0.0.4/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      155 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:31:54.034375 bondzai.gateway-sdk-0.0.4/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:31:54.041872 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/
--rw-r--r--   0 theo       (501) staff       (20)      139 2023-06-21 16:30:18.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     9552 2023-06-21 16:29:54.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/agent.py
--rw-r--r--   0 theo       (501) staff       (20)     2494 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/commands.py
--rw-r--r--   0 theo       (501) staff       (20)      257 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/config.py
--rw-r--r--   0 theo       (501) staff       (20)     6243 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/enums.py
--rw-r--r--   0 theo       (501) staff       (20)     3983 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/events.py
--rw-r--r--   0 theo       (501) staff       (20)     4384 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/gateway.py
--rw-r--r--   0 theo       (501) staff       (20)     3318 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/message.py
--rw-r--r--   0 theo       (501) staff       (20)      812 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/request.py
--rw-r--r--   0 theo       (501) staff       (20)        0 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/responses.py
--rw-r--r--   0 theo       (501) staff       (20)      570 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/timer.py
--rw-r--r--   0 theo       (501) staff       (20)      738 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-21 16:31:54.048769 bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      604 2023-06-21 16:31:54.000000 bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      735 2023-06-21 16:31:54.000000 bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 16:31:54.000000 bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-21 16:31:54.000000 bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       61 2023-06-21 16:31:54.000000 bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-06-21 16:31:54.000000 bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-21 16:31:53.000000 bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)    21241 2023-06-21 15:39:37.000000 bondzai.gateway-sdk-0.0.4/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      775 2023-06-21 16:31:54.050670 bondzai.gateway-sdk-0.0.4/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:26.751649 bondzai.gateway-sdk-0.0.5/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 09:32:39.000000 bondzai.gateway-sdk-0.0.5/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-04 09:34:26.751843 bondzai.gateway-sdk-0.0.5/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      155 2023-07-04 09:32:39.000000 bondzai.gateway-sdk-0.0.5/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:26.741476 bondzai.gateway-sdk-0.0.5/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:26.748043 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/
+-rw-r--r--   0 theo       (501) staff       (20)      139 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)    10180 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/agent.py
+-rw-r--r--   0 theo       (501) staff       (20)     2497 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/commands.py
+-rw-r--r--   0 theo       (501) staff       (20)      255 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/config.py
+-rw-r--r--   0 theo       (501) staff       (20)     6661 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)     6937 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/events.py
+-rw-r--r--   0 theo       (501) staff       (20)     4380 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/gateway.py
+-rw-r--r--   0 theo       (501) staff       (20)     3288 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/message.py
+-rw-r--r--   0 theo       (501) staff       (20)      810 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/request.py
+-rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-04 09:32:39.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/responses.py
+-rw-r--r--   0 theo       (501) staff       (20)      771 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/timer.py
+-rw-r--r--   0 theo       (501) staff       (20)     1415 2023-07-04 09:34:17.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/transcode.py
+-rw-r--r--   0 theo       (501) staff       (20)      738 2023-07-04 09:32:39.000000 bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:26.751280 bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-04 09:34:26.000000 bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      770 2023-07-04 09:34:26.000000 bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:34:26.000000 bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 09:34:26.000000 bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       61 2023-07-04 09:34:26.000000 bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 09:34:26.000000 bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:34:26.000000 bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)    21241 2023-07-04 09:32:39.000000 bondzai.gateway-sdk-0.0.5/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-04 09:34:26.753438 bondzai.gateway-sdk-0.0.5/setup.cfg
```

### Comparing `bondzai.gateway-sdk-0.0.4/NOTICE` & `bondzai.gateway-sdk-0.0.5/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.4/PKG-INFO` & `bondzai.gateway-sdk-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/agent.py` & `bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from __future__ import annotations
 from collections.abc import Callable
 
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from .gateway import Gateway
+
 from .request import Request, RequestActions
 from .message import EventMessage, Message, MessageModule, MessageType, CommandMessage
-from .enums import EventOperationID, AgentAIMode, AgentTriggerType, CommandOperationID, \
-                LogCommand, DBMCommandParameter, DBMTable, DBMCommand
+from .enums import EventOperationID, AgentAIMode, AgentAIType, AgentTriggerType, CommandOperationID, \
+    LogCommand, DBMCommandParameter, DBMTable, DBMCommand, LogCommandParameter
 from .utils import unpack_buffer_to_list, b642b
 from .timer import Timer
 
+from .transcode import transcode
+
 
-class Agent():
-    def __init__(self, gateway: "Gateway", device_name: str) -> None:
+class Agent:
+    def __init__(self, gateway: Gateway, device_name: str) -> None:
         self.device_name = device_name
         self.gateway = gateway
 
         self._active_label = None
 
         self._wait_response = {}
 
@@ -31,93 +37,95 @@
             typ = MessageType(msg['header']['typ'])
             msg_id = msg["header"]["id"]
 
             data: dict = None
             if "payloads" in msg and len(msg["payloads"]):
                 data = msg["payloads"][0]['data']
 
-            if msg_id in self._wait_response:
-                self._wait_response[msg_id] = data
+            if typ == MessageType.RESPONSE:
+                if msg_id in self._wait_response:
+                    self._wait_response[msg_id] = data
 
             if typ == MessageType.EVENT:
                 operation = EventOperationID(msg['header']['op'])
                 if mod == MessageModule.LOG:
                     if operation == EventOperationID.EVT_EXT_LOG:
                         content = data.get("msg", "")
                         if content == "EVT_INT_TRAIN_DONE":
                             for callback in self._on_train_done_handlers.values():
                                 callback(self, data)
                         else:
                             for callback in self._on_log_handlers.values():
                                 callback(self, content)
                 else:
-                    if operation == EventOperationID.EVT_INT_INFER_DONE:
+                    data_transcode = transcode(operation, data)
+                    if operation == EventOperationID.EVT_EXT_VM_RESULT:
                         for callback in self._on_infer_done_handlers.values():
-                            callback(self, data)
-                    elif operation == EventOperationID.EVT_INT_FINAL:
+                            callback(self, data_transcode)
+                    elif operation == EventOperationID.EVT_EXT_ASL_RESULT:
                         for callback in self._on_final_process_done.values():
-                            callback(self, data)
+                            callback(self, data_transcode)
                     for callback in self._on_event_handlers.values():
                         callback(self, operation, data)
 
     def remove_observer(self, dict_obj_name, idx):
         if not hasattr(self, dict_obj_name):
-            return 
+            return
         dict_obj = getattr(self, dict_obj_name)
         if hasattr(dict_obj, idx):
             delattr(getattr(self, dict_obj_name), idx)
 
     def set_active_label(self, label_id: int) -> None:
         self._active_label = label_id
 
-    def on_log(self, callback: Callable[["Agent", str], None]) -> None:
+    def on_log(self, callback: Callable[[Agent, str], None]) -> callable:
         cb_id = f"onlog-{len(self._on_log_handlers.keys())}"
         self._on_log_handlers[cb_id] = callback
         return lambda: self.remove_observer("_on_log_handlers", cb_id)
 
-    def on_event(self, callback: Callable[["Agent", EventOperationID, dict], None]) -> None:
+    def on_event(self, callback: Callable[[Agent, EventOperationID, dict], None]) -> callable:
         cb_id = f"onevent-{len(self._on_log_handlers.keys())}"
         self._on_event_handlers[cb_id] = callback
         return lambda: self.remove_observer("_on_event_handlers", cb_id)
 
-    def on_training_done(self, callback: Callable[["Agent", dict], None]) -> None:
+    def on_training_done(self, callback: Callable[[Agent, dict], None]) -> callable:
         cb_id = f"ontraindone-{len(self._on_log_handlers.keys())}"
         self._on_train_done_handlers[cb_id] = callback
         return lambda: self.remove_observer("_on_train_handlers", cb_id)
 
-    def on_inference_done(self, callback: Callable[["Agent", dict], None]) -> None:
+    def on_inference_done(self, callback: Callable[[Agent, dict], None]) -> callable:
         cb_id = f"oninferdone-{len(self._on_log_handlers.keys())}"
         self._on_infer_done_handlers[cb_id] = callback
         return lambda: self.remove_observer("_on_infer_done_handlers", cb_id)
 
-    def on_final_process_done(self, callback: Callable[["Agent", dict], None]) -> None:
+    def on_final_process_done(self, callback: Callable[[Agent, dict], None]) -> callable:
         cb_id = f"onfinaldone-{len(self._on_log_handlers.keys())}"
         self._on_final_process_done[cb_id] = callback
         return lambda: self.remove_observer("_on_final_process_done", cb_id)
 
     def send_message(self, message: Message, sync: bool = False):
         self.gateway.send(Request(
-            RequestActions.ACT_SEND_TO_DEVICE, 
-            self.device_name, 
+            RequestActions.ACT_SEND_TO_DEVICE,
+            self.device_name,
             message.to_dict()
         ))
 
         if sync:
             return self.wait_command_response(message)
-        
+
         return None
 
     def subscribe(self):
         self.gateway.send(Request(
-            RequestActions.ACT_SUB_TO_DEVICE, 
+            RequestActions.ACT_SUB_TO_DEVICE,
             self.device_name
-        ))        
+        ))
 
     def send_chunk(self, source_id: int, chunk: list[float]) -> None:
-        msg = EventMessage(EventOperationID.EVT_EXT_DATA_IN)\
+        msg = EventMessage(EventOperationID.EVT_EXT_DATA_IN) \
             .add_payload(source_id, "<f", chunk)
         self.send_message(msg)
 
     def send_data(self, source_id: int, data: list[float], chunk_size: int, chunk_rate: int) -> None:
         sent_data = 0
         start_idx = 0
         end_idx = chunk_size
@@ -127,42 +135,49 @@
             time_1 = Timer.get_elapsed_time()
             self.send_chunk(source_id, data[start_idx:end_idx])
             sent_data += chunk_size
             send_time = Timer.get_elapsed_time() - time_1
             start_idx += chunk_size
             end_idx += chunk_size
             if end_idx > data_len:
-                end_idx = data_len - 1
+                end_idx = data_len
             Timer.wait(chunk_period - send_time)
 
-    def set_ai_mode(self, mode: AgentAIMode, active_label: int = None) -> None:
-        data = [mode.value]
-        if mode == AgentAIMode.APP_AI_MODE_ENROLLEMENT:
-            data += [1, active_label]
-        msg = EventMessage(EventOperationID.EVT_EXT_CUSTOM_2)\
-            .add_payload(data)
+    def set_ai_mode(self, mode: AgentAIMode, ground_truth: list = []) -> None:
+        ai_type = AgentAIType.APP_AI_TYPE_CLASSIFICATION
+        if len(ground_truth) > 0 and isinstance(ground_truth[0], float):
+            ai_type = AgentAIType.APP_AI_TYPE_REGRESSION
+
+        msg = EventMessage(EventOperationID.EVT_EXT_SET_MODE) \
+            .add_payload(mode.value, ai_type.value, ground_truth)
         self.send_message(msg)
 
     def trigger(self, trigger_type: AgentTriggerType) -> None:
-        msg = EventMessage(EventOperationID.EVT_EXT_CUSTOM_1)\
-            .add_payload([trigger_type.value])
+        msg = EventMessage(EventOperationID.EVT_EXT_TRIGGER) \
+            .add_payload(trigger_type.value, 0)
         self.send_message(msg)
 
     def kill(self) -> None:
         self.trigger(AgentTriggerType.TRIGGER_KILL)
 
-    def correct(self, ground_truth: float | int, position: int = 0, remove: bool = False):
-        msg = EventMessage(EventOperationID.EVT_EXT_CUSTOM_2)\
-            .add_payload([3, remove, position, ground_truth])
+    def correct(self, ground_truth: list, position: int = 0, remove: bool = False):
+        ai_type = AgentAIType.APP_AI_TYPE_CLASSIFICATION
+        if remove:
+            ground_truth = []
+        if len(ground_truth) > 0 and isinstance(ground_truth[0], float):
+            ai_type = AgentAIType.APP_AI_TYPE_REGRESSION
+        msg = EventMessage(EventOperationID.EVT_EXT_CORRECTION) \
+            .add_payload(position, ai_type.value, ground_truth)
         self.send_message(msg)
 
-    def wait_command_response(self, msg: Message, timeout: int = 10000):
+    def wait_command_response(self, msg: Message, timeout_ms: int = 10000):
         msg_id = msg.header.id
         self._wait_response[msg_id] = None
 
+        timeout = timeout_ms / 1000.0
         sleeptime = 0.001
         start_time = Timer.get_elapsed_time()
         while msg_id in self._wait_response and self._wait_response[msg_id] is None:
             elapsed_time = Timer.get_elapsed_time() - start_time
             if elapsed_time > timeout:
                 raise Exception("Command message Timeout")
             Timer.wait(sleeptime)
@@ -170,65 +185,64 @@
         return_value = self._wait_response[msg_id]
         del self._wait_response[msg_id]
         return return_value
 
     # OTA 
     def get_kpi(self):
         msg = CommandMessage(CommandOperationID.CMD_GET, MessageModule.LOG)
-        msg.add_payload(LogCommand.LOG_GET_KPI.value)
+        msg.add_payload(LogCommandParameter.LOG_NB_KPIS.value)
         data: dict = self.send_message(msg, sync=True)
 
         if "number" not in data:
             raise Exception("Missing number in data")
-        
+
         nbkpis = data.get("number")
         kpi_list = []
         for i in range(nbkpis):
             msg = CommandMessage(CommandOperationID.CMD_START, MessageModule.LOG)
             msg.add_payload(LogCommand.LOG_GET_KPI.value, i)
             kpi = self.send_message(msg, sync=True)
             kpi_list.append({
                 "id": kpi.get("id", 0),
                 "description": kpi["description"],
                 "value": kpi["value"],
                 "type": kpi["typ"]
             })
 
         return kpi_list
-    
+
     def export_dataset(self) -> list:
         datasets = []
-        for data in self.export_table_data(DBMTable.DBM_DAT): 
+        for data in self.export_table_data(DBMTable.DBM_DAT):
             val = data.get("record")
             if val is not None:
                 data["record"] = unpack_buffer_to_list(
                     b642b(val),
 
                 )
             datasets.append(data)
         return datasets
 
     def export_vm_list(self) -> list:
         return self.export_table_data(DBMTable.DBM_VM)
-    
+
     def export_tables(self) -> list:
         msg = CommandMessage(CommandOperationID.CMD_GET, MessageModule.DBM)
         msg.add_payload(DBMCommandParameter.DBM_PARAM_INFO.value)
         data = self.send_message(msg, sync=True)
 
         return data.get("tables", [])
-    
+
     def export_table_data(self, data_type: DBMTable) -> list:
         tables = self.export_tables()
         results = []
 
         for table in tables:
             if table.get("typ") != data_type.value:
                 continue
-
             for i in range(table.get("count", 0)):
                 msg = CommandMessage(CommandOperationID.CMD_START, MessageModule.DBM)
                 msg.add_payload(DBMCommand.DBM_EXPORT_ROW.value, table.get("handle"), "", i)
                 data = self.send_message(msg, sync=True)
                 attr = data.get("attributes")
                 if attr is not None:
                     results.append(attr)
```

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/commands.py` & `bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @dataclass
 class CommandGet:
     itemid: int
 
     def get_size(self) -> int:
         return 2
 
-    def to_dict(self) -> str:
+    def to_dict(self) -> dict:
         return {
             "itemid": self.itemid,
         }
 
     def to_array(self) -> list:
         return [
             self.itemid,
@@ -25,15 +25,15 @@
 class CommandStartLogGetKpi:
     itemid: int
     index: int
 
     def get_size(self) -> int:
         return 6
 
-    def to_dict(self) -> str:
+    def to_dict(self) -> dict:
         return {
             "itemid": self.itemid,
             "index": self.index,
         }
 
     def to_array(self) -> list:
         return [
@@ -48,15 +48,15 @@
     handle: int
     key: str
     index: int = -1
 
     def get_size(self) -> int:
         return 4 + (4 if len(self.key) == 0 else len(self.key))
 
-    def to_dict(self) -> str:
+    def to_dict(self) -> dict:
         return {
             "itemid": self.itemid,
             "handle": self.handle,
             "key": self.key,
             "index": self.index,
         }
```

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/enums.py` & `bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/enums.py`

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

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/gateway.py` & `bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .request import Request, RequestActions
 from .config import Configuration
 from .agent import Agent
 from .timer import Timer
 
 
-class Gateway():
+class Gateway:
     def __init__(self, host: str, port: int, config: Configuration = None) -> None: 
         self.config = config if config is not None else Configuration()
         
         self._host = host
         self._port = port
 
         host_parts = host.split("/")
@@ -30,15 +30,15 @@
             on_message=self._on_message,
             on_error=self._on_error
         )
 
         self.is_connected = False
         self.thread = None
 
-        self._on_connect_callbacks: list[Callable[[None], None]] = []
+        self._on_connect_callbacks: list[Callable[None, None]] = []
         self._on_close_callbacks: list[Callable[[int, str], None]] = []
         self._on_error_callbacks: list[Callable[[Exception], None]] = []
 
         self._agents: dict[str, Agent] = {}
 
     def _on_connection_open(self, _: WebSocketApp):
         self.is_connected = True
@@ -61,17 +61,17 @@
             if "action" in data:
                 if data["action"] == RequestActions.ACT_GET_DEVICES_LIST.value:
                     device_list = data.get("devices", [])
 
                     # Adding new agents
                     for d_name in device_list:
                         if d_name not in self._agents:
-                            self._agents[d_name] = Agent(self,d_name)
+                            self._agents[d_name] = Agent(self, d_name)
 
-                    # Removing mnissing agents
+                    # Removing missing agents
                     for agent in self._agents.values():
                         if agent.device_name not in device_list:
                             del self._agents[agent.device_name]
 
                 elif data["action"] == RequestActions.EVT_ON_DEVICE_MSG.value:
                     device_name = data.get("device_name")
                     msg = data.get("message", "")
```

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/message.py` & `bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,51 +6,52 @@
 from .timer import Timer
 from .enums import MessageModule, EventOperationID, CommandOperationID
 from .events import EventHeader, get_event_class
 from .commands import get_command_class
 
 
 class MessageType(Enum):
-    COMMAND     = 0
-    RESPONSE    = 1
-    ERR         = 2
-    EVENT       = 3
+    COMMAND = 0
+    RESPONSE = 1
+    ERR = 2
+    EVENT = 3
 
 
-class MessageHeader():
+class MessageHeader:
     current_id: int = 0
 
-    def __init__(self, 
-        msg_type: MessageType,
-        mod: MessageModule,
+    def __init__(
+        self, 
+        msg_type: MessageType, 
+        mod: MessageModule, 
         operation: EventOperationID,
-        session: bytes = Configuration.session, 
+        session: bytes = Configuration.session,
         id_num: int = None
     ) -> None:
         self.session = session
         self.operation = operation
         self.mod = mod
         self.type = msg_type
         if id_num is None:
             self.id = MessageHeader.current_id
             MessageHeader.current_id = (MessageHeader.current_id + 1) % 255
-        else:            
+        else:
             self.id = id_num
 
     def to_dict(self):
         return {
             "session": b2b64(self.session),
             "id": self.id,
             "op": self.operation.value,
             "typ": self.type.value,
             "mod": self.mod.value
         }
 
 
-class Message():
+class Message:
     def __init__(self) -> None:
         self.header: MessageHeader = None
         self.payloads: list[Any] = []
 
     def to_dict(self) -> dict:
         raise NotImplementedError()
 
@@ -64,17 +65,17 @@
     def add_payload(self, *args):
         event_class = get_event_class(self.header.operation)
         if event_class is None:
             raise Exception(f"Operation {self.header.operation} has no type associated")
 
         event = event_class(*args)
         header = EventHeader(
-            self.header.mod.value, 
-            Configuration.app_id, 
-            Timer.get_timestamp(), 
+            self.header.mod.value,
+            Configuration.app_id,
+            Timer.get_timestamp(),
             event.get_size()
         )
 
         self.payloads.append({
             "header": header,
             "event": event
         })
```

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/request.py` & `bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/request.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     EVT_ON_DEVICE_MSG = "on-device-msg"
 
     def __repr__(self) -> str:
         return self.value
 
 
-class Request():
+class Request:
     def __init__(self, action: RequestActions, device_name: str = "", data: Any = None) -> None:
         self.action: RequestActions = action
         self.device_name: str = device_name
         self.message: str = json.dumps(data) if data else ""
 
     def to_json(self):
         return json.dumps({
```

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai/gateway_sdk/utils.py` & `bondzai.gateway-sdk-0.0.5/bondzai/gateway_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/PKG-INFO` & `bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.4/bondzai.gateway_sdk.egg-info/SOURCES.txt` & `bondzai.gateway-sdk-0.0.5/bondzai.gateway_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ./bondzai/gateway_sdk/enums.py
 ./bondzai/gateway_sdk/events.py
 ./bondzai/gateway_sdk/gateway.py
 ./bondzai/gateway_sdk/message.py
 ./bondzai/gateway_sdk/request.py
 ./bondzai/gateway_sdk/responses.py
 ./bondzai/gateway_sdk/timer.py
+./bondzai/gateway_sdk/transcode.py
 ./bondzai/gateway_sdk/utils.py
 bondzai.gateway_sdk.egg-info/PKG-INFO
 bondzai.gateway_sdk.egg-info/SOURCES.txt
 bondzai.gateway_sdk.egg-info/dependency_links.txt
 bondzai.gateway_sdk.egg-info/namespace_packages.txt
 bondzai.gateway_sdk.egg-info/requires.txt
 bondzai.gateway_sdk.egg-info/top_level.txt
```

### Comparing `bondzai.gateway-sdk-0.0.4/pyproject.toml` & `bondzai.gateway-sdk-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.4/setup.cfg` & `bondzai.gateway-sdk-0.0.5/setup.cfg`

 * *Files identical despite different names*

