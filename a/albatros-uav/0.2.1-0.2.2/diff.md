# Comparing `tmp/albatros_uav-0.2.1.tar.gz` & `tmp/albatros_uav-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albatros_uav-0.2.1.tar", max compression
+gzip compressed data, was "albatros_uav-0.2.2.tar", max compression
```

## Comparing `albatros_uav-0.2.1.tar` & `albatros_uav-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      251 2023-06-28 21:11:22.663227 albatros_uav-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-09 15:52:27.239088 albatros_uav-0.2.1/albatros/__init__.py
--rw-r--r--   0        0        0     5944 2023-06-11 08:27:47.442808 albatros_uav-0.2.1/albatros/commands.py
--rw-r--r--   0        0        0     7312 2023-06-11 08:27:47.443808 albatros_uav-0.2.1/albatros/enums.py
--rw-r--r--   0        0        0    10188 2023-07-04 16:27:13.774291 albatros_uav-0.2.1/albatros/message_models.py
--rw-r--r--   0        0        0        0 2023-06-14 12:38:56.434756 albatros_uav-0.2.1/albatros/nav/__init__.py
--rw-r--r--   0        0        0     1410 2023-06-14 15:16:21.197023 albatros_uav-0.2.1/albatros/nav/position.py
--rw-r--r--   0        0        0     1492 2023-07-04 16:27:13.775291 albatros_uav-0.2.1/albatros/receive_loop.py
--rw-r--r--   0        0        0      175 2023-07-04 16:27:13.775291 albatros_uav-0.2.1/albatros/setup_logging.py
--rw-r--r--   0        0        0     2037 2023-07-04 16:27:13.776291 albatros_uav-0.2.1/albatros/telemetry.py
--rw-r--r--   0        0        0     7031 2023-07-04 16:27:13.777291 albatros_uav-0.2.1/albatros/uav.py
--rw-r--r--   0        0        0     3249 2023-07-04 16:27:13.777291 albatros_uav-0.2.1/albatros/uav_data.py
--rw-r--r--   0        0        0      778 2023-07-04 16:27:53.056225 albatros_uav-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 albatros_uav-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    12379 2023-07-04 18:39:58.388051 albatros_uav-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 15:52:27.239088 albatros_uav-0.2.2/albatros/__init__.py
+-rw-r--r--   0        0        0     5944 2023-06-11 08:27:47.442808 albatros_uav-0.2.2/albatros/commands.py
+-rw-r--r--   0        0        0     7312 2023-06-11 08:27:47.443808 albatros_uav-0.2.2/albatros/enums.py
+-rw-r--r--   0        0        0    10188 2023-07-04 16:27:13.774291 albatros_uav-0.2.2/albatros/message_models.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:38:56.434756 albatros_uav-0.2.2/albatros/nav/__init__.py
+-rw-r--r--   0        0        0     1410 2023-06-14 15:16:21.197023 albatros_uav-0.2.2/albatros/nav/position.py
+-rw-r--r--   0        0        0     1492 2023-07-04 16:27:13.775291 albatros_uav-0.2.2/albatros/receive_loop.py
+-rw-r--r--   0        0        0      175 2023-07-04 16:27:13.775291 albatros_uav-0.2.2/albatros/setup_logging.py
+-rw-r--r--   0        0        0     2037 2023-07-04 16:27:13.776291 albatros_uav-0.2.2/albatros/telemetry.py
+-rw-r--r--   0        0        0     7292 2023-07-04 17:30:56.796692 albatros_uav-0.2.2/albatros/uav.py
+-rw-r--r--   0        0        0     3249 2023-07-04 16:27:13.777291 albatros_uav-0.2.2/albatros/uav_data.py
+-rw-r--r--   0        0        0      778 2023-07-04 18:40:15.724018 albatros_uav-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    12847 1970-01-01 00:00:00.000000 albatros_uav-0.2.2/PKG-INFO
```

### Comparing `albatros_uav-0.2.1/albatros/commands.py` & `albatros_uav-0.2.2/albatros/commands.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.1/albatros/enums.py` & `albatros_uav-0.2.2/albatros/enums.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.1/albatros/message_models.py` & `albatros_uav-0.2.2/albatros/message_models.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.1/albatros/nav/position.py` & `albatros_uav-0.2.2/albatros/nav/position.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.1/albatros/receive_loop.py` & `albatros_uav-0.2.2/albatros/receive_loop.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.1/albatros/telemetry.py` & `albatros_uav-0.2.2/albatros/telemetry.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.1/albatros/uav.py` & `albatros_uav-0.2.2/albatros/uav.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 from .commands import (
     get_command_int_message,
     get_command_long_message,
     get_mission_count_message,
     get_mission_item_int,
 )
 from .enums import CopterFlightModes, PlaneFlightModes
-from .telemetry import Telemetry
+from .telemetry import ConnectionType, Telemetry
 
 logger = logging.getLogger(__name__)
 
-MY_SRC_ID = 1
-MY_CMP_ID = 191
-
 
 class UAV:
-    def __init__(self, target_system: int = 1, target_component: int = 1) -> None:
-        self.target_system = target_system
-        self.target_component = target_component
-        self.mav = MAVLink(0, MY_SRC_ID, MY_CMP_ID)
-
-        self.telem = Telemetry()
-        self.telem.make_direct_connection()
+    def __init__(
+        self,
+        vehicle_system_id: int = 1,
+        vehicle_component_id: int = 1,
+        my_sys_id: int = 1,
+        my_cmp_id: int = 191,
+        connection_type: ConnectionType = ConnectionType.DIRECT,
+        device: str = "udpin:0.0.0.0:14550",
+        baud_rate: int = 115200,
+        host: str = "localhost",
+    ) -> None:
+        self.target_system = vehicle_system_id
+        self.target_component = vehicle_component_id
+        self.mav = MAVLink(0, my_sys_id, my_cmp_id)
+        self.telem = Telemetry(connection_type, device, baud_rate, host)
 
     def wait_gps_fix(self) -> None:
         while (
             self.telem.data.gps_raw_int.fix_type < 3
             or self.telem.data.gps_raw_int.lat == 0
         ):
             sleep(0.1)
```

### Comparing `albatros_uav-0.2.1/albatros/uav_data.py` & `albatros_uav-0.2.2/albatros/uav_data.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.1/pyproject.toml` & `albatros_uav-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "albatros-uav"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Jędrzej Stasik <sjedrzej58@gmail.com>"]
 readme = "README.md"
 packages = [{include = "albatros"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

