# Comparing `tmp/scratchattach-1.2.6.tar.gz` & `tmp/scratchattach-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.2.6.tar", last modified: Sun Jun 18 14:34:21 2023, max compression
+gzip compressed data, was "scratchattach-1.2.7.tar", last modified: Tue Jul  4 18:53:41 2023, max compression
```

## Comparing `scratchattach-1.2.6.tar` & `scratchattach-1.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 14:34:21.491949 scratchattach-1.2.6/
--rw-rw-rw-   0        0        0    21960 2023-06-18 14:34:21.490952 scratchattach-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    20641 2023-06-18 14:23:06.000000 scratchattach-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 14:34:21.438093 scratchattach-1.2.6/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.6/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    13982 2023-06-18 14:33:57.000000 scratchattach-1.2.6/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    18499 2023-06-18 14:33:59.000000 scratchattach-1.2.6/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.6/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.6/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.6/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.6/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.6/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.6/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.6/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-06-18 14:34:21.487960 scratchattach-1.2.6/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    21960 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 14:34:21.492946 scratchattach-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-06-18 14:23:24.000000 scratchattach-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:53:41.479739 scratchattach-1.2.7/
+-rw-rw-rw-   0        0        0    22121 2023-07-04 18:53:41.478742 scratchattach-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    20795 2023-07-04 18:52:48.000000 scratchattach-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 18:53:41.441054 scratchattach-1.2.7/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.7/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    15465 2023-07-04 18:39:44.000000 scratchattach-1.2.7/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    18499 2023-06-18 14:33:59.000000 scratchattach-1.2.7/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.7/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.7/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.7/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.7/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.7/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.7/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.7/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:53:41.476264 scratchattach-1.2.7/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22121 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 18:53:41.479739 scratchattach-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-07-04 18:52:57.000000 scratchattach-1.2.7/setup.py
```

### Comparing `scratchattach-1.2.6/PKG-INFO` & `scratchattach-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.6
+Version: 1.2.7
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -91,43 +91,50 @@
 
 ```python
 conn = scratch3.CloudConnection(project_id = "project_id", username="username", session_id="sessionId")
 ```
 
 **Connect to the TurboWarp cloud:**
 
-Does not require a session.
-
 ```python
+conn = scratch3.connect_tw_cloud("project_id")
+```
+
+Alternative ways to do connect to the TurboWarp cloud:
+
+```py
+conn = session.connect_tw_cloud("project_id")
 conn = scratch3.TwCloudConnection(project_id = "project_id", username="username")  
 # Optional argument: cloud_host="wss://clouddata.turbowarp.org"
 # To connect to forkphorus's cloud server, use cloud_host="wss://stratus.turbowarp.org"
 ```
 
 **Set a cloud var:**
 
-New Scratchers can set Scratch cloud variables too.
-
 ```python
 conn.set_var("variable", "value") #the variable name is specified without the cloud emoji
 ```
 
-**Get a Scratch cloud var from the clouddata logs:**
+**Get a cloud var:**
 
-Does not require a connection / session.
+Get Scratch cloud variables:
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 variables = scratch3.get_cloud("project_id") #Returns a dict with all cloud var values
 logs = scratch3.get_cloud_logs("project_id") #Returns the cloud logs as list
 ```
 
-**Get a Scratch / TurboWarp cloud var from the websocket:**
+Get TurboWarp cloud variables:
+*Do not spam these methods, they create a new cloud connection on every run*
 
-This feature is not working at the moment.
+```python
+value = scratch3.get_tw_var("project_id", "variable")
+variables = scratch3.get_tw_cloud("project_id")
+```
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
 
@@ -155,15 +162,15 @@
 ```python
 import scratchattach as scratch3
 
 events = scratch3.CloudEvents("project_id")
 
 @events.event
 def on_set(event): #Called when a cloud var is set
-    print(f"{event.user} set the variable {event.var} to the valuee {event.value} at {event.timestamp}")
+    print(f"{event.user} set the variable {event.var} to the value {event.value} at {event.timestamp}")
 
 @events.event
 def on_del(event):
     print(f"{event.user} deleted variable {event.var}")
 
 @events.event
 def on_create(event):
```

### Comparing `scratchattach-1.2.6/README.md` & `scratchattach-1.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,43 +75,50 @@
 
 ```python
 conn = scratch3.CloudConnection(project_id = "project_id", username="username", session_id="sessionId")
 ```
 
 **Connect to the TurboWarp cloud:**
 
-Does not require a session.
-
 ```python
+conn = scratch3.connect_tw_cloud("project_id")
+```
+
+Alternative ways to do connect to the TurboWarp cloud:
+
+```py
+conn = session.connect_tw_cloud("project_id")
 conn = scratch3.TwCloudConnection(project_id = "project_id", username="username")  
 # Optional argument: cloud_host="wss://clouddata.turbowarp.org"
 # To connect to forkphorus's cloud server, use cloud_host="wss://stratus.turbowarp.org"
 ```
 
 **Set a cloud var:**
 
-New Scratchers can set Scratch cloud variables too.
-
 ```python
 conn.set_var("variable", "value") #the variable name is specified without the cloud emoji
 ```
 
-**Get a Scratch cloud var from the clouddata logs:**
+**Get a cloud var:**
 
-Does not require a connection / session.
+Get Scratch cloud variables:
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 variables = scratch3.get_cloud("project_id") #Returns a dict with all cloud var values
 logs = scratch3.get_cloud_logs("project_id") #Returns the cloud logs as list
 ```
 
-**Get a Scratch / TurboWarp cloud var from the websocket:**
+Get TurboWarp cloud variables:
+*Do not spam these methods, they create a new cloud connection on every run*
 
-This feature is not working at the moment.
+```python
+value = scratch3.get_tw_var("project_id", "variable")
+variables = scratch3.get_tw_cloud("project_id")
+```
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
 
@@ -139,15 +146,15 @@
 ```python
 import scratchattach as scratch3
 
 events = scratch3.CloudEvents("project_id")
 
 @events.event
 def on_set(event): #Called when a cloud var is set
-    print(f"{event.user} set the variable {event.var} to the valuee {event.value} at {event.timestamp}")
+    print(f"{event.user} set the variable {event.var} to the value {event.value} at {event.timestamp}")
 
 @events.event
 def on_del(event):
     print(f"{event.user} deleted variable {event.var}")
 
 @events.event
 def on_create(event):
```

### Comparing `scratchattach-1.2.6/scratchattach/_cloud.py` & `scratchattach-1.2.7/scratchattach/_cloud.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,88 +6,84 @@
 import time
 from . import _exceptions
 import traceback
 import warnings
 
 class _CloudMixin:
 
-    def __init__(self, *, project_id, username="python", session_id=None, cloud_host=None, _allow_non_numeric=False, _no_reconnect=False):
+    def __init__(self, *, project_id, username="python", session_id=None, cloud_host=None, _allow_non_numeric=False, _ws_timeout=None):
         self._session_id = session_id
         self._username = username
         try:
             self.project_id = int(project_id)
         except ValueError: #non-numeric project id (possible on turbowarp's cloud server)
             self.project_id = str(project_id)
         self._ratelimited_until = 0 #deals with the 0.1 second rate limit for cloud variable sets
         self._connect_timestamp = 0 #timestamp of when the cloud connection was opened
+        self._ws_timeout = _ws_timeout
         self.websocket = websocket.WebSocket()
-        self._no_reconnect = False
         self._connect(cloud_host=cloud_host)
         self._handshake()
-        self._no_reconnect = _no_reconnect
         self.cloud_host = cloud_host
         self.allow_non_numeric = _allow_non_numeric #TurboWarp only. If this is true, turbowarp cloud variables can be set to non-numeric values (if) the cloud_host wss allows it)
-        self._clouddata = []
 
     def _send_packet(self, packet):
         self.websocket.send(json.dumps(packet) + "\n")
 
     def disconnect(self):
         self.websocket.close()
 
     def _handshake(self):
-        if self._no_reconnect is True:
-            return
         try:
             self._send_packet(
                 {"method": "handshake", "user": self._username, "project_id": self.project_id}
             )
         except Exception:
             self._connect(cloud_host=self.cloud_host)
             self._handshake()
 
-    def get_var(self, variable):
-        try:
-            variable = "☁ " + str(variable)
-            self.set_var('@scratchattach','0')
+    # ---
 
-            result = []
-            for i in self._clouddata:
-                try:
-                    result.append(json.loads(i))
-                except Exception: pass
-            if result == []:
-                return None
-            else:
-                for i in result:
-                    if i['name'] == variable:
-                        return i['value']
-                return None
-        except Exception as e:
-            raise _exceptions.FetchError
+    def get_cloud(self):
+        # DEPRECATED: On Scratch's cloud variables, this method of getting a cloud variable does not work. On TurboWarp's cloud variables it does work, but there's the scratchattach.get_tw_cloud function for that now
+        print("Warning: scratchattach.CloudConnection.get_cloud and scratchattach.TwCloudConnection.get_cloud are deprecated. Use scratchattach.get_cloud or scratchattach.get_tw_cloud instead")
+        warnings.warn(
+            "scratchattach.CloudConnection.get_cloud and scratchattach.TwCloudConnection.get_cloud are deprecated. Use scratchattach.get_cloud or scratchattach.get_tw_cloud instead", DeprecationWarning
+        )
+        return []
+
+    def get_var(self, variable):
+        # DEPRECATED: On Scratch's cloud variables, this method of getting a cloud variable does not work. On TurboWarp's cloud variables it does work, but there's the scratchattach.get_tw_var function for that now
+        print("Warning: scratchattach.CloudConnection.get_var and scratchattach.TwCloudConnection.get_var are deprecated. Use scratchattach.get_var or scratchattach.get_tw_var instead")
+        warnings.warn(
+            "scratchattach.CloudConnection.get_var and scratchattach.TwCloudConnection.get_var are deprecated. Use scratchattach.get_var or scratchattach.get_tw_var instead", DeprecationWarning
+        )
+        return None
 
 class CloudConnection(_CloudMixin):
 
     def _connect(self, *, cloud_host):
         try:
             self.websocket = websocket.WebSocket()
             self.websocket.connect(
                 "wss://clouddata.scratch.mit.edu",
                 cookie="scratchsessionsid=" + self._session_id + ";",
                 origin="https://scratch.mit.edu",
                 enable_multithread=True,
+                timeout=self._ws_timeout
             )
         except Exception:
             try:
                 self.websocket = websocket.WebSocket()
                 self.websocket.connect(
                     "wss://clouddata.scratch.mit.edu",
                     cookie="scratchsessionsid=" + self._session_id + ";",
                     origin="https://scratch.mit.edu",
                     enable_multithread=True,
+                    timeout=timeout
                 )
             except Exception:
                 raise(_exceptions.ConnectionError)
         self._connect_timestamp = time.time()
 
     def set_var(self, variable, value):
         variable = variable.replace("☁ ", "")
@@ -109,16 +105,14 @@
                     "method": "set",
                     "name": "☁ " + variable,
                     "value": value,
                     "user": self._username,
                     "project_id": self.project_id,
                 }
             )
-            if variable == "@scratchattach":
-                self._clouddata = self.websocket.recv().split('\n')
         except Exception as e:
             try:
                 self._handshake()
             except Exception:
                 try:
                     self._connect(cloud_host=self.cloud_host)
                     self._handshake()
@@ -127,49 +121,28 @@
 
             time.sleep(0.1)
             self.set_var(variable, value)
         self._ratelimited_until = time.time()
 
 class TwCloudConnection(_CloudMixin):
 
-    def _connect(self, *, cloud_host):
-        if self._no_reconnect is True:
-            return
+    def _connect(self, *, cloud_host, timeout=None):
         try:
             if cloud_host is None:
                 cloud_host = "wss://clouddata.turbowarp.org/"
                 self.cloud_host = "wss://clouddata.turbowarp.org/"
             self.websocket.connect(
                 cloud_host,
-                enable_multithread=True
+                enable_multithread=True,
+                timeout = self._ws_timeout
             )
         except Exception:
             raise(_exceptions.ConnectionError)
         self._connect_timestamp = time.time()
 
-    def get_cloud(self, variable):
-        try:
-            variable = "☁ " + str(variable)
-            self.set_var('@scratchattach','0')
-
-            result = []
-            for i in self._clouddata:
-                try:
-                    result.append(json.loads(i))
-                except Exception: pass
-            data = {}
-            if result == []:
-                return {}
-            else:
-                for item in result:
-                    data[item["name"]] = item["value"]
-                return data
-        except Exception as e:
-            raise _exceptions.FetchError
-
 
     def set_var(self, variable, value):
         variable = variable.replace("☁ ", "")
         if not (value is True or value is False or value in [float('inf'), -float('inf')]):
             value = str(value)
             x = value.replace(".", "")
             x = x.replace("-", "")
@@ -185,16 +158,14 @@
                     "method": "set",
                     "name": "☁ " + variable,
                     "value": value,
                     "user": self._username,
                     "project_id": self.project_id,
                 }
             )
-            if variable == "@scratchattach":
-                self._clouddata = self.websocket.recv().split('\n') + self._clouddata
         except Exception as e:
             try:
                 self._handshake()
                 time.sleep(0.1)
                 self.set_var(variable, value)
             except Exception:
                 try:
@@ -337,37 +308,84 @@
                     self.connection._connect(cloud_host=self.connection.cloud_host)
                     self.connection._handshake()
                 except Exception:
                     if "on_disconnect" in self._events:
                         self._events["on_disconnect"]()
 # -----
 
+
 def get_cloud(project_id):
+    #Gets the Scratch clouddata of a project from the Scratch cloud log
     try:
         response = json.loads(requests.get(f"https://clouddata.scratch.mit.edu/logs?projectid={project_id}&limit=100&offset=0").text)
         response.reverse()
         clouddata = {}
         for activity in response:
             clouddata[activity["name"][2:]] = activity["value"]
         return clouddata
     except Exception:
         return []
 
 def get_var(project_id, variable):
+    #Gets the value of a Scratch cloud variable from the Scratch cloud log
     try:
         response = json.loads(requests.get(f"https://clouddata.scratch.mit.edu/logs?projectid={project_id}&limit=100&offset=0").text)
         response = list(filter(lambda k: k["name"] == "☁ "+variable, response))
         if response == []:
             return None
         else:
             return response[0]["value"]
     except Exception:
         return None
 
+def get_tw_cloud(project_id):
+    #Gets the clouddata of a TurboWarp project from the TurboWarp websocket
+    #Do not spam this method, it creates a new connection to the TW cloud on every run
+    try:
+        conn = TwCloudConnection(project_id=project_id, _ws_timeout=1)
+        data = conn.websocket.recv().split("\n")
+        conn.disconnect()
+
+        result = []
+        for i in data:
+            try:
+                result.append(json.loads(i))
+            except Exception: pass
+        return result
+    except websocket._exceptions.WebSocketTimeoutException:
+        return []
+    except Exception:
+        raise _exceptions.FetchError
+
+def get_tw_var(project_id, variable):
+    #Gets the value of a Turbowarp cloud variable from the TW websocket
+    #Do not spam this method, it creates a new connection to the TW cloud on every run
+    try:
+        variable = "☁ " + str(variable)
+        result = get_tw_cloud(project_id)
+        if result == []:
+            return None
+        else:
+            for i in result:
+                if i['name'] == variable:
+                    return i['value']
+            else:
+                return None
+    except Exception as e:
+        raise _exceptions.FetchError
+
 def get_cloud_logs(project_id, *, filter_by_var_named =None, limit=25, offset=0, log_url="https://clouddata.scratch.mit.edu/logs"):
     try:
         response = json.loads(requests.get(f"{log_url}?projectid={project_id}&limit={limit}&offset={offset}").text)
         if filter_by_var_named is None: return response
         else:
             return list(filter(lambda k: k["name"] == "☁ "+filter_by_var_named, response))
     except Exception:
         return []
+
+def connect_tw_cloud(project_id_arg=None, *, project_id=None):
+    if project_id is None:
+        project_id = project_id_arg
+    if project_id is None:
+        return None
+
+    return TwCloudConnection(project_id = int(project_id))
```

### Comparing `scratchattach-1.2.6/scratchattach/_cloud_requests.py` & `scratchattach-1.2.7/scratchattach/_cloud_requests.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.6/scratchattach/_encoder.py` & `scratchattach-1.2.7/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.6/scratchattach/_exceptions.py` & `scratchattach-1.2.7/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.6/scratchattach/_forum.py` & `scratchattach-1.2.7/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.6/scratchattach/_project.py` & `scratchattach-1.2.7/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.6/scratchattach/_session.py` & `scratchattach-1.2.7/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.6/scratchattach/_studio.py` & `scratchattach-1.2.7/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.6/scratchattach/_user.py` & `scratchattach-1.2.7/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.6/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.2.7/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.6
+Version: 1.2.7
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -91,43 +91,50 @@
 
 ```python
 conn = scratch3.CloudConnection(project_id = "project_id", username="username", session_id="sessionId")
 ```
 
 **Connect to the TurboWarp cloud:**
 
-Does not require a session.
-
 ```python
+conn = scratch3.connect_tw_cloud("project_id")
+```
+
+Alternative ways to do connect to the TurboWarp cloud:
+
+```py
+conn = session.connect_tw_cloud("project_id")
 conn = scratch3.TwCloudConnection(project_id = "project_id", username="username")  
 # Optional argument: cloud_host="wss://clouddata.turbowarp.org"
 # To connect to forkphorus's cloud server, use cloud_host="wss://stratus.turbowarp.org"
 ```
 
 **Set a cloud var:**
 
-New Scratchers can set Scratch cloud variables too.
-
 ```python
 conn.set_var("variable", "value") #the variable name is specified without the cloud emoji
 ```
 
-**Get a Scratch cloud var from the clouddata logs:**
+**Get a cloud var:**
 
-Does not require a connection / session.
+Get Scratch cloud variables:
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 variables = scratch3.get_cloud("project_id") #Returns a dict with all cloud var values
 logs = scratch3.get_cloud_logs("project_id") #Returns the cloud logs as list
 ```
 
-**Get a Scratch / TurboWarp cloud var from the websocket:**
+Get TurboWarp cloud variables:
+*Do not spam these methods, they create a new cloud connection on every run*
 
-This feature is not working at the moment.
+```python
+value = scratch3.get_tw_var("project_id", "variable")
+variables = scratch3.get_tw_cloud("project_id")
+```
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
 
@@ -155,15 +162,15 @@
 ```python
 import scratchattach as scratch3
 
 events = scratch3.CloudEvents("project_id")
 
 @events.event
 def on_set(event): #Called when a cloud var is set
-    print(f"{event.user} set the variable {event.var} to the valuee {event.value} at {event.timestamp}")
+    print(f"{event.user} set the variable {event.var} to the value {event.value} at {event.timestamp}")
 
 @events.event
 def on_del(event):
     print(f"{event.user} deleted variable {event.var}")
 
 @events.event
 def on_create(event):
```

### Comparing `scratchattach-1.2.6/setup.py` & `scratchattach-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.2.6'
+VERSION = '1.2.7'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

