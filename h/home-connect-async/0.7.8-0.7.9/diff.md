# Comparing `tmp/home-connect-async-0.7.8.tar.gz` & `tmp/home-connect-async-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-connect-async-0.7.8.tar", last modified: Thu Mar 23 23:00:55 2023, max compression
+gzip compressed data, was "home-connect-async-0.7.9.tar", last modified: Tue Jul  4 15:28:15 2023, max compression
```

## Comparing `home-connect-async-0.7.8.tar` & `home-connect-async-0.7.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:00:55.111979 home-connect-async-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-23 23:00:55.111979 home-connect-async-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:00:55.111979 home-connect-async-0.7.8/home_connect_async/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/home_connect_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/home_connect_async/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/home_connect_async/appliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/home_connect_async/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/home_connect_async/callback_registery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/home_connect_async/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/home_connect_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/home_connect_async/homeconnect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:00:55.111979 home-connect-async-0.7.8/home_connect_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-23 23:00:55.000000 home-connect-async-0.7.8/home_connect_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-23 23:00:55.000000 home-connect-async-0.7.8/home_connect_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 23:00:55.000000 home-connect-async-0.7.8/home_connect_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-23 23:00:55.000000 home-connect-async-0.7.8/home_connect_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-23 23:00:55.000000 home-connect-async-0.7.8/home_connect_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-23 23:00:55.111979 home-connect-async-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-23 23:00:42.000000 home-connect-async-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:15.020874 home-connect-async-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-04 15:28:15.020874 home-connect-async-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:15.020874 home-connect-async-0.7.9/home_connect_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/home_connect_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/home_connect_async/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39105 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/home_connect_async/appliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/home_connect_async/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/home_connect_async/callback_registery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/home_connect_async/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/home_connect_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/home_connect_async/homeconnect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:28:15.020874 home-connect-async-0.7.9/home_connect_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-04 15:28:15.000000 home-connect-async-0.7.9/home_connect_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-04 15:28:15.000000 home-connect-async-0.7.9/home_connect_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:28:15.000000 home-connect-async-0.7.9/home_connect_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 15:28:15.000000 home-connect-async-0.7.9/home_connect_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:28:15.000000 home-connect-async-0.7.9/home_connect_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 15:28:15.020874 home-connect-async-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-04 15:28:05.000000 home-connect-async-0.7.9/setup.py
```

### Comparing `home-connect-async-0.7.8/PKG-INFO` & `home-connect-async-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-connect-async
-Version: 0.7.8
+Version: 0.7.9
 Summary: Async SDK for BSH Home Connect API
 Home-page: https://github.com/ekutner/home-connect-async
 Author: Eran Kutner
 Author-email: eran@kutner.org
 License: MIT
 Keywords: HomeConnect,Home Connect,BSH,Async,SDK
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `home-connect-async-0.7.8/README.md` & `home-connect-async-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `home-connect-async-0.7.8/home_connect_async/api.py` & `home-connect-async-0.7.9/home_connect_async/api.py`

 * *Files identical despite different names*

### Comparing `home-connect-async-0.7.8/home_connect_async/appliance.py` & `home-connect-async-0.7.9/home_connect_async/appliance.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,15 +453,15 @@
 
         if response.error_description:
             raise HomeConnectError(response.error_description, response=response)
         raise HomeConnectError("Failed to set program ({response.status})", response=response)
 
     #endregion
 
-    
+
     async def async_set_connection_state(self, connected:bool):
         """ Update the appliance connection state when notified about a state change from the event stream """
         if connected != self.connected:
             self.connected = connected
             if connected:
                 await self.async_fetch_data(include_static_data=False)
             await self._callbacks.async_broadcast_event(self, Events.CONNECTION_CHANGED, connected)
@@ -531,65 +531,67 @@
             self._active_program_fail_count = 0
         elif ( (key == "BSH.Common.Root.ActiveProgram" and value) or
                 # apparently it is possible to get progress notifications without getting the ActiveProgram event first so we handle that
                 (key in ["BSH.Common.Option.ProgramProgress", "BSH.Common.Option.RemainingProgramTime"]) or
                 # it is also possible to get operation state Run without getting the ActiveProgram event
                 (key == "BSH.Common.Status.OperationState" and value=="BSH.Common.EnumType.OperationState.Run")
             ) and \
-            (not self.active_program or (key == "BSH.Common.Root.ActiveProgram" and self.active_program.key != value) ) :
+            (not self.active_program or (key == "BSH.Common.Root.ActiveProgram" and self.active_program.key != value) ) and \
+            self._active_program_fail_count < 3 :
             # handle program start
             self.active_program = await self._async_fetch_programs("active")
+            if self.active_program:
+                self._active_program_fail_count = 0
+            else:
+                # This is a workaround to prevent rate limiting when receiving progress events but avaialable_programs returns 404
+                self._active_program_fail_count += 1
             self.available_programs = await self._async_fetch_programs("available")
             self.settings = await self._async_fetch_settings()
             self.commands = await self._async_fetch_commands()
             await self._callbacks.async_broadcast_event(self, Events.PROGRAM_STARTED, value)
             await self._callbacks.async_broadcast_event(self, Events.DATA_CHANGED)
-            self._active_program_fail_count = 0
+
         elif ( (key == "BSH.Common.Root.ActiveProgram" and not value) or
                (key == "BSH.Common.Status.OperationState" and value in ["BSH.Common.EnumType.OperationState.Ready", "BSH.Common.EnumType.OperationState.Finished"]) or
                (key == "BSH.Common.Event.ProgramFinished")
             ) and self.active_program:
             # handle program end
             prev_prog = self.active_program.key if self.active_program else None
             self.active_program = None
+            self._active_program_fail_count = 0
             self.settings = await self._async_fetch_settings()
             self.commands = await self._async_fetch_commands()
             self.available_programs = await self._async_fetch_programs("available")
             await self._callbacks.async_broadcast_event(self, Events.PROGRAM_FINISHED, prev_prog)
             await self._callbacks.async_broadcast_event(self, Events.DATA_CHANGED)
-            self._active_program_fail_count = 0
+
         elif key == "BSH.Common.Status.OperationState" and \
              value!="BSH.Common.EnumType.OperationState.Run" and \
              self.status.get("BSH.Common.Status.OperationState") != value:  # ignore repeat notifiations of the same state
-            #await self.async_fetch_data(include_static_data=False)
             self.active_program = await self._async_fetch_programs("active")
             self.selected_program = await self._async_fetch_programs("selected")
             self.available_programs = await self._async_fetch_programs("available")
             self.settings = await self._async_fetch_settings()
             self.commands = await self._async_fetch_commands()
             await self._callbacks.async_broadcast_event(self, Events.DATA_CHANGED)
+
         elif key =="BSH.Common.Status.RemoteControlStartAllowed":
             self.available_programs = await self._async_fetch_programs("available")
             await self._callbacks.async_broadcast_event(self, Events.DATA_CHANGED)
+
         elif ( not self.available_programs or len(self.available_programs) < 2) and \
-             ( self._active_program_fail_count < 5 ) and \
              ( key in ["BSH.Common.Status.OperationState", "BSH.Common.Status.RemoteControlActive"] ) and \
              ( "BSH.Common.Status.OperationState" not in self.status or self.status["BSH.Common.Status.OperationState"].value == "BSH.Common.EnumType.OperationState.Ready" ) and \
              ( "BSH.Common.Status.RemoteControlActive" not in self.status or self.status["BSH.Common.Status.RemoteControlActive"].value):
             # Handle cases were the appliance data was loaded without getting all the programs (for example when HA is restarted while a program is active)
-            # If the state is Ready and remote control is possible and we didn"t load the available programs before then load them now
+            # If the state is Ready and remote control is possible and we didn't load the available programs before then load them now
             available_programs = await self._async_fetch_programs("available")
-            if available_programs:
-                self.available_programs = available_programs
-                await self._callbacks.async_broadcast_event(self, Events.PAIRED)
-                await self._callbacks.async_broadcast_event(self, Events.DATA_CHANGED)
-                self._active_program_fail_count = 0
-            else:
-                # This is a workaround to prevent rate limiting when receiving progress events but avaialable_programs returns 404
-                self._active_program_fail_count += 1
+            self.available_programs = available_programs
+            await self._callbacks.async_broadcast_event(self, Events.PAIRED)
+            await self._callbacks.async_broadcast_event(self, Events.DATA_CHANGED)
 
         # broadcast the specific event that was received
         await self._callbacks.async_broadcast_event(self, key, value)
 
     def register_callback(self, callback:Callable[[Appliance, str, any], None], keys:str|Sequence[str] ) -> None:
         """ Register a callback to be called when an update is received for the specified keys
             Wildcard syntax is also supported for the keys
```

### Comparing `home-connect-async-0.7.8/home_connect_async/auth.py` & `home-connect-async-0.7.9/home_connect_async/auth.py`

 * *Files identical despite different names*

### Comparing `home-connect-async-0.7.8/home_connect_async/callback_registery.py` & `home-connect-async-0.7.9/home_connect_async/callback_registery.py`

 * *Files identical despite different names*

### Comparing `home-connect-async-0.7.8/home_connect_async/common.py` & `home-connect-async-0.7.9/home_connect_async/common.py`

 * *Files identical despite different names*

### Comparing `home-connect-async-0.7.8/home_connect_async/const.py` & `home-connect-async-0.7.9/home_connect_async/const.py`

 * *Files identical despite different names*

### Comparing `home-connect-async-0.7.8/home_connect_async/homeconnect.py` & `home-connect-async-0.7.9/home_connect_async/homeconnect.py`

 * *Files identical despite different names*

### Comparing `home-connect-async-0.7.8/home_connect_async.egg-info/PKG-INFO` & `home-connect-async-0.7.9/home_connect_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-connect-async
-Version: 0.7.8
+Version: 0.7.9
 Summary: Async SDK for BSH Home Connect API
 Home-page: https://github.com/ekutner/home-connect-async
 Author: Eran Kutner
 Author-email: eran@kutner.org
 License: MIT
 Keywords: HomeConnect,Home Connect,BSH,Async,SDK
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `home-connect-async-0.7.8/setup.py` & `home-connect-async-0.7.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name = 'home-connect-async',
     packages = ['home_connect_async'],
-    version = '0.7.8',
+    version = '0.7.9',
     license='MIT',
     description = 'Async SDK for BSH Home Connect API',
     author = 'Eran Kutner',
     author_email = 'eran@kutner.org',
     url = 'https://github.com/ekutner/home-connect-async',
     keywords = ['HomeConnect', 'Home Connect', 'BSH', 'Async', 'SDK'],
     install_requires=[
```

