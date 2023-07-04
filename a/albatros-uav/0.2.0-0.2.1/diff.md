# Comparing `tmp/albatros_uav-0.2.0.tar.gz` & `tmp/albatros_uav-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albatros_uav-0.2.0.tar", max compression
+gzip compressed data, was "albatros_uav-0.2.1.tar", max compression
```

## Comparing `albatros_uav-0.2.0.tar` & `albatros_uav-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0      251 2023-06-28 21:11:22.663227 albatros_uav-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-09 15:52:27.239088 albatros_uav-0.2.0/albatros/__init__.py
--rw-r--r--   0        0        0     5944 2023-06-11 08:27:47.442808 albatros_uav-0.2.0/albatros/commands.py
--rw-r--r--   0        0        0     7312 2023-06-11 08:27:47.443808 albatros_uav-0.2.0/albatros/enums.py
--rw-r--r--   0        0        0        0 2023-06-14 12:38:56.434756 albatros_uav-0.2.0/albatros/nav/__init__.py
--rw-r--r--   0        0        0     1410 2023-06-14 15:16:21.197023 albatros_uav-0.2.0/albatros/nav/position.py
--rw-r--r--   0        0        0     1814 2023-07-03 21:45:33.471753 albatros_uav-0.2.0/albatros/telemetry_source.py
--rw-r--r--   0        0        0     6455 2023-07-03 21:45:33.472753 albatros_uav-0.2.0/albatros/uav.py
--rw-r--r--   0        0        0      757 2023-07-03 21:50:32.664560 albatros_uav-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 albatros_uav-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2023-06-28 21:11:22.663227 albatros_uav-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 15:52:27.239088 albatros_uav-0.2.1/albatros/__init__.py
+-rw-r--r--   0        0        0     5944 2023-06-11 08:27:47.442808 albatros_uav-0.2.1/albatros/commands.py
+-rw-r--r--   0        0        0     7312 2023-06-11 08:27:47.443808 albatros_uav-0.2.1/albatros/enums.py
+-rw-r--r--   0        0        0    10188 2023-07-04 16:27:13.774291 albatros_uav-0.2.1/albatros/message_models.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:38:56.434756 albatros_uav-0.2.1/albatros/nav/__init__.py
+-rw-r--r--   0        0        0     1410 2023-06-14 15:16:21.197023 albatros_uav-0.2.1/albatros/nav/position.py
+-rw-r--r--   0        0        0     1492 2023-07-04 16:27:13.775291 albatros_uav-0.2.1/albatros/receive_loop.py
+-rw-r--r--   0        0        0      175 2023-07-04 16:27:13.775291 albatros_uav-0.2.1/albatros/setup_logging.py
+-rw-r--r--   0        0        0     2037 2023-07-04 16:27:13.776291 albatros_uav-0.2.1/albatros/telemetry.py
+-rw-r--r--   0        0        0     7031 2023-07-04 16:27:13.777291 albatros_uav-0.2.1/albatros/uav.py
+-rw-r--r--   0        0        0     3249 2023-07-04 16:27:13.777291 albatros_uav-0.2.1/albatros/uav_data.py
+-rw-r--r--   0        0        0      778 2023-07-04 16:27:53.056225 albatros_uav-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 albatros_uav-0.2.1/PKG-INFO
```

### Comparing `albatros_uav-0.2.0/albatros/commands.py` & `albatros_uav-0.2.1/albatros/commands.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.0/albatros/enums.py` & `albatros_uav-0.2.1/albatros/enums.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.0/albatros/nav/position.py` & `albatros_uav-0.2.1/albatros/nav/position.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.2.0/albatros/telemetry_source.py` & `albatros_uav-0.2.1/albatros/telemetry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 import logging
 from enum import Enum
 
 import pika
 from pika.adapters.blocking_connection import BlockingChannel
 from pymavlink import mavutil
 
+from .receive_loop import ReceiveLoop
+from .uav_data import UAVData
+
 logger = logging.getLogger(__name__)
 
 
 class ConnectionType(Enum):
     DIRECT = 1
     RABBITMQ = 2
 
 
-MY_SRC_ID = 1
-MY_CMP_ID = 191
-
-
-class TelemetrySource:
+class Telemetry:
     def __init__(
         self,
         connection_type: ConnectionType = ConnectionType.DIRECT,
         device: str = "udpin:0.0.0.0:14550",
         baud_rate: int = 115200,
         host: str = "localhost",
     ) -> None:
         self.direct_connection: mavutil.mavudp
         self.rabbit_connection: BlockingChannel
         self.connection_type = connection_type
         self.device = device
         self.baud_rate = baud_rate
         self.host = host
+        self.data = UAVData()
 
     def __post_init__(self) -> None:
         if self.connection_type == ConnectionType.DIRECT:
             self.make_direct_connection()
 
         if self.connection_type == ConnectionType.RABBITMQ:
             self.make_rabbitmq_connection()
 
     def make_direct_connection(self) -> None:
         self.direct_connection = mavutil.mavlink_connection(self.device, self.baud_rate)
         self.direct_connection.wait_heartbeat()
         logger.info("heartbeat recived")
 
+        # starts a thread that receives telemetry
+        receive_telem_loop = ReceiveLoop(self.direct_connection, self.data)
+        receive_telem_loop.start()
+
     def make_rabbitmq_connection(self) -> None:
         connection = pika.BlockingConnection(pika.ConnectionParameters(self.host))
         self.rabbit_connection = connection.channel()
         self.rabbit_connection.queue_declare(queue="commands")
 
     def send(self, message: bytes) -> None:
         if self.connection_type == ConnectionType.DIRECT:
```

### Comparing `albatros_uav-0.2.0/albatros/uav.py` & `albatros_uav-0.2.1/albatros/uav.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,92 @@
 import logging
+from time import sleep, time
 from typing import Optional, Union
 
 from pymavlink.dialects.v20.ardupilotmega import (
     MAV_CMD_COMPONENT_ARM_DISARM,
     MAV_CMD_DO_REPOSITION,
     MAV_CMD_DO_SET_MODE,
     MAV_CMD_DO_SET_SERVO,
     MAV_CMD_NAV_RETURN_TO_LAUNCH,
     MAV_CMD_NAV_WAYPOINT,
+    MAV_MODE_FLAG_SAFETY_ARMED,
     MAVLink,
 )
 
 from .commands import (
     get_command_int_message,
     get_command_long_message,
     get_mission_count_message,
     get_mission_item_int,
 )
 from .enums import CopterFlightModes, PlaneFlightModes
-from .telemetry_source import TelemetrySource
+from .telemetry import Telemetry
 
 logger = logging.getLogger(__name__)
 
 MY_SRC_ID = 1
 MY_CMP_ID = 191
 
 
 class UAV:
     def __init__(self, target_system: int = 1, target_component: int = 1) -> None:
         self.target_system = target_system
         self.target_component = target_component
         self.mav = MAVLink(0, MY_SRC_ID, MY_CMP_ID)
 
-        self.telem_source = TelemetrySource()
-        self.telem_source.make_direct_connection()
+        self.telem = Telemetry()
+        self.telem.make_direct_connection()
 
-    def arm(self) -> None:
+    def wait_gps_fix(self) -> None:
+        while (
+            self.telem.data.gps_raw_int.fix_type < 3
+            or self.telem.data.gps_raw_int.lat == 0
+        ):
+            sleep(0.1)
+
+    def is_armed(self) -> bool:
+        armed_flag = self.telem.data.heartbeat.base_mode & MAV_MODE_FLAG_SAFETY_ARMED
+        return bool(armed_flag)
+
+    def wait_heartbeat(self) -> None:
+        while time() * 1000 - self.telem.data.heartbeat.timestamp_ms > 100:
+            sleep(0.1)
+        sleep(0.1)
+
+    def arm(self) -> bool:
         """
         Arms motors.
         """
         msg = get_command_long_message(
             target_system=self.target_system,
             target_component=self.target_component,
             command=MAV_CMD_COMPONENT_ARM_DISARM,
             param1=1,
         )
 
-        self.telem_source.send(msg.pack(self.mav))
+        self.telem.send(msg.pack(self.mav))
         logger.info("Arm command sent.")
+        self.wait_heartbeat()
+        logger.info("heartbeat received")
+
+        return self.is_armed()
 
     def disarm(self) -> None:
         """
         Disarms motors.
         """
         msg = get_command_long_message(
             target_system=self.target_system,
             target_component=self.target_component,
             command=MAV_CMD_COMPONENT_ARM_DISARM,
             param1=0,
         )
 
-        self.telem_source.send(msg.pack(self.mav))
+        self.telem.send(msg.pack(self.mav))
         logger.info("Disarm command sent.")
 
     def set_mode(self, mode: Union[PlaneFlightModes, CopterFlightModes]) -> None:
         """
         Set system mode.
 
         Args:
@@ -74,15 +96,15 @@
             target_system=self.target_system,
             target_component=self.target_component,
             command=MAV_CMD_DO_SET_MODE,
             param1=1,
             param2=mode.value,
         )
 
-        self.telem_source.send(msg.pack(self.mav))
+        self.telem.send(msg.pack(self.mav))
         logger.info("Set mode command sent")
 
     def set_servo(self, instance_number: int, pwm: int) -> None:
         """
         Set a servo to a desired PWM value.
 
         Args:
@@ -93,15 +115,15 @@
             target_system=self.target_system,
             target_component=self.target_component,
             command=MAV_CMD_DO_SET_SERVO,
             param1=instance_number,
             param2=pwm,
         )
 
-        self.telem_source.send(msg.pack(self.mav))
+        self.telem.send(msg.pack(self.mav))
         logger.info("Set servo command sent.")
 
     def flight_to_gps_position(self, lat_int: int, lon_int: int, alt_m: float) -> None:
         """
         Works only in Guided mode. Reposition the vehicle to a specific WGS84 global position.
         """
         msg = get_command_int_message(
@@ -109,15 +131,15 @@
             target_component=self.target_component,
             command=MAV_CMD_DO_REPOSITION,
             x=lat_int,
             y=lon_int,
             z=alt_m,
         )
 
-        self.telem_source.send(msg.pack(self.mav))
+        self.telem.send(msg.pack(self.mav))
         logger.info("Flight to point command sent.")
 
     def send_mission_count(self, mission_elements_count: int) -> None:
         """
         Send the number of items in a mission. This is used to initiate mission upload.
 
         Args:
@@ -125,15 +147,15 @@
         """
         msg = get_mission_count_message(
             target_system=self.target_system,
             target_component=self.target_component,
             count=mission_elements_count,
         )
 
-        self.telem_source.send(msg.pack(self.mav))
+        self.telem.send(msg.pack(self.mav))
         logger.info("mission_count message sent.")
 
     def send_mission_waypoint_item(
         self,
         seq: int,
         lat_int: int,
         lon_int: int,
@@ -170,15 +192,15 @@
             param3=pass_radius_m,
             param4=yaw_deg,
             x=lat_int,
             y=lon_int,
             z=alt_m,
         )
 
-        self.telem_source.send(msg.pack(self.mav))
+        self.telem.send(msg.pack(self.mav))
         logger.info("mission_waypoint message sent.")
 
     def send_mission_rtl_item(
         self,
         seq: int,
     ) -> None:
         """
@@ -192,9 +214,9 @@
         msg = get_mission_item_int(
             target_system=self.target_system,
             target_component=self.target_component,
             seq=seq,
             command=MAV_CMD_NAV_RETURN_TO_LAUNCH,
         )
 
-        self.telem_source.send(msg.pack(self.mav))
+        self.telem.send(msg.pack(self.mav))
         logger.info("mission_rtl message sent.")
```

### Comparing `albatros_uav-0.2.0/pyproject.toml` & `albatros_uav-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "albatros-uav"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Jędrzej Stasik <sjedrzej58@gmail.com>"]
 readme = "README.md"
 packages = [{include = "albatros"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pika = "^1.3.2"
 pymavlink = "^2.4.39"
+pydantic = "^1.10.9"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pylint = "^2.17.4"
 flake8 = "^6.0.0"
```

### Comparing `albatros_uav-0.2.0/PKG-INFO` & `albatros_uav-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: albatros-uav
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Jędrzej Stasik
 Author-email: sjedrzej58@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pika (>=1.3.2,<2.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: pymavlink (>=2.4.39,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Albatros - Python libary handling mavlink commands
 
 ## Run examples
```

