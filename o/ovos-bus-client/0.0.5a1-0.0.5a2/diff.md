# Comparing `tmp/ovos-bus-client-0.0.5a1.tar.gz` & `tmp/ovos-bus-client-0.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.5a1.tar", last modified: Wed Jun 21 01:30:16 2023, max compression
+gzip compressed data, was "ovos-bus-client-0.0.5a2.tar", last modified: Tue Jun 27 17:18:36 2023, max compression
```

## Comparing `ovos-bus-client-0.0.5a1.tar` & `ovos-bus-client-0.0.5a2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    22546 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 01:30:16.000000 ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:30:16.236145 ovos-bus-client-0.0.5a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-21 01:30:15.000000 ovos-bus-client-0.0.5a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:18:36.557006 ovos-bus-client-0.0.5a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-27 17:18:36.557006 ovos-bus-client-0.0.5a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:18:36.553006 ovos-bus-client-0.0.5a2/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:18:36.557006 ovos-bus-client-0.0.5a2/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:18:36.557006 ovos-bus-client-0.0.5a2/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:18:36.553006 ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-27 17:18:36.000000 ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-27 17:18:36.000000 ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:18:36.000000 ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 17:18:36.000000 ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 17:18:36.000000 ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 17:18:36.000000 ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:18:36.557006 ovos-bus-client-0.0.5a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-27 17:18:35.000000 ovos-bus-client-0.0.5a2/setup.py
```

### Comparing `ovos-bus-client-0.0.5a1/LICENSE.md` & `ovos-bus-client-0.0.5a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/PKG-INFO` & `ovos-bus-client-0.0.5a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/client/client.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/conf.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/conf.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/message.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,15 @@
         return response_message
 
 
 class GUIMessage(Message):
     def __init__(self, msg_type, **kwargs):
         super().__init__(msg_type, data=kwargs)
 
-    def serialize(self):
+    def serialize(self) -> str:
         """This returns a string of the message info.
 
         This makes it easy to send over a websocket. This uses
         json dumps to generate the string with type, data and context
 
         Returns:
             str: a json string representation of the message.
@@ -447,11 +447,11 @@
         msg = json.dumps({'type': self.msg_type, **data})
         if self._secret_key:
             payload = encrypt_as_dict(self._secret_key, msg)
             return json.dumps(payload)
         return msg
 
     @staticmethod
-    def deserialize(value):
+    def deserialize(value: str):
         value = Message._json_load(value)
         msg_type = value.pop("type")
         return GUIMessage(msg_type, **value)
```

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/scripts.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/send_func.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/session.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class UtteranceState(str, enum.Enum):
     INTENT = "intent"  # includes converse
     RESPONSE = "response"
 
 
 def _get_valid_langs() -> List[str]:
     return list(set([get_default_lang()] +
-                    Configuration().get("secondary_langs'", [])))
+                    Configuration().get("secondary_langs", [])))
 
 
 class IntentContextManagerFrame:
     def __init__(self, entities: List[dict] = None, metadata: dict = None):
         """
         Manages entities and context for a single frame of conversation.
         Provides simple equality querying.
```

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/util/scheduler.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.5a2/ovos_bus_client/util/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.5a1/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.5a2/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.5a1/setup.py` & `ovos-bus-client-0.0.5a2/setup.py`

 * *Files identical despite different names*

