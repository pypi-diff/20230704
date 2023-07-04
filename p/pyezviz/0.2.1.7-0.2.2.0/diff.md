# Comparing `tmp/pyezviz-0.2.1.7.tar.gz` & `tmp/pyezviz-0.2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.1.7.tar", last modified: Sat Jul  1 18:05:02 2023, max compression
+gzip compressed data, was "pyezviz-0.2.2.0.tar", last modified: Tue Jul  4 05:42:08 2023, max compression
```

## Comparing `pyezviz-0.2.1.7.tar` & `pyezviz-0.2.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    61784 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62664 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 05:42:07.000000 pyezviz-0.2.2.0/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 05:42:08.004020 pyezviz-0.2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-04 05:41:57.000000 pyezviz-0.2.2.0/setup.py
```

### Comparing `pyezviz-0.2.1.7/LICENSE.md` & `pyezviz-0.2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.7/README.md` & `pyezviz-0.2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.7/pyezviz/__init__.py` & `pyezviz-0.2.2.0/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.7/pyezviz/__main__.py` & `pyezviz-0.2.2.0/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.7/pyezviz/api_endpoints.py` & `pyezviz-0.2.2.0/pyezviz/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.7/pyezviz/camera.py` & `pyezviz-0.2.2.0/pyezviz/camera.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, Any
 
 from .constants import DeviceSwitchType, SoundMode
 from .exceptions import PyEzvizError
+from .utils import fetch_nested_value, string_to_list
 
 if TYPE_CHECKING:
     from .client import EzvizClient
 
 
 class EzvizCamera:
     """Initialize Ezviz camera object."""
@@ -25,37 +26,40 @@
             "timepassed": None,
         }
         self._device = (
             device_obj if device_obj else self._client.get_device_infos(self._serial)
         )
         self._last_alarm: dict[str, Any] = {}
         self._switch: dict[int, bool] = {
-            switch["type"]: switch["enable"]
-            for switch in self._device.get("SWITCH", {})
+            switch["type"]: switch["enable"] for switch in self._device["SWITCH"]
         }
 
+    def fetch_key(self, keys: list, default_value: Any = None) -> Any:
+        """Fetch dictionary key."""
+        return fetch_nested_value(self._device, keys, default_value)
+
     def _alarm_list(self) -> None:
         """Get last alarm info for this camera's self._serial."""
         _alarmlist = self._client.get_alarminfo(self._serial)
 
-        if _alarmlist["page"].get("totalResults") > 0:
+        if fetch_nested_value(_alarmlist, ["page", "totalResults"], 0) > 0:
             self._last_alarm = _alarmlist["alarms"][0]
             return self._motion_trigger()
 
     def _local_ip(self) -> Any:
         """Fix empty ip value for certain cameras."""
         if (
-            self._device["WIFI"].get("address")
+            self.fetch_key(["WIFI", "address"])
             and self._device["WIFI"]["address"] != "0.0.0.0"
         ):
             return self._device["WIFI"]["address"]
 
         # Seems to return none or 0.0.0.0 on some.
         if (
-            self._device["CONNECTION"].get("localIp")
+            self.fetch_key(["CONNECTION", "localIp"])
             and self._device["CONNECTION"]["localIp"] != "0.0.0.0"
         ):
             return self._device["CONNECTION"]["localIp"]
 
         return "0.0.0.0"
 
     def _motion_trigger(self) -> None:
@@ -78,97 +82,93 @@
             "alarm_trigger_active": bool(timepassed < datetime.timedelta(seconds=60)),
             "timepassed": timepassed.total_seconds(),
         }
 
     def _is_alarm_schedules_enabled(self) -> bool:
         """Check if alarm schedules enabled."""
         _alarm_schedules = [
-            item for item in self._device.get("TIME_PLAN", {}) if item.get("type") == 2
+            item for item in self._device["TIME_PLAN"] if item.get("type") == 2
         ]
 
         if _alarm_schedules:
             return bool(_alarm_schedules[0].get("enable"))
 
         return False
 
     def status(self) -> dict[Any, Any]:
         """Return the status of the camera."""
         self._alarm_list()
 
         return {
             "serial": self._serial,
-            "name": self._device["deviceInfos"].get("name"),
-            "version": self._device["deviceInfos"].get("version"),
+            "name": self.fetch_key(["deviceInfos", "name"]),
+            "version": self.fetch_key(["deviceInfos", "version"]),
             "upgrade_available": bool(
-                self._device["UPGRADE"].get("isNeedUpgrade") == 3
+                self.fetch_key(["UPGRADE", "isNeedUpgrade"]) == 3
             ),
-            "status": self._device["deviceInfos"].get("status"),
-            "device_category": self._device["deviceInfos"].get("deviceCategory"),
-            "device_sub_category": self._device["deviceInfos"].get("deviceSubCategory"),
-            "sleep": self._switch.get(DeviceSwitchType.SLEEP.value)
-            or self._switch.get(DeviceSwitchType.AUTO_SLEEP.value),
-            "privacy": self._switch.get(DeviceSwitchType.PRIVACY.value),
-            "audio": self._switch.get(DeviceSwitchType.SOUND.value),
-            "ir_led": self._switch.get(DeviceSwitchType.INFRARED_LIGHT.value),
-            "state_led": self._switch.get(DeviceSwitchType.LIGHT.value),
-            "upgrade_percent": self._device["STATUS"].get("upgradeProcess"),
+            "status": self.fetch_key(["deviceInfos", "status"]),
+            "device_category": self.fetch_key(["deviceInfos", "deviceCategory"]),
+            "device_sub_category": self.fetch_key(["deviceInfos", "deviceSubCategory"]),
+            "upgrade_percent": self.fetch_key(["STATUS", "upgradeProcess"]),
             "upgrade_in_progress": bool(
-                self._device["STATUS"].get("upgradeStatus") == 0
+                self.fetch_key(["STATUS", "upgradeStatus"]) == 0
             ),
-            "latest_firmware_info": self._device["UPGRADE"].get("upgradePackageInfo"),
-            "follow_move": self._switch.get(DeviceSwitchType.MOBILE_TRACKING.value),
-            "alarm_notify": bool(self._device["STATUS"].get("globalStatus")),
+            "latest_firmware_info": self.fetch_key(["UPGRADE", "upgradePackageInfo"]),
+            "alarm_notify": bool(self.fetch_key(["STATUS", "globalStatus"])),
             "alarm_schedules_enabled": self._is_alarm_schedules_enabled(),
             "alarm_sound_mod": SoundMode(
-                self._device["STATUS"].get("alarmSoundMode", -1)
+                self.fetch_key(["STATUS", "alarmSoundMode"], -1)
             ).name,
-            "encrypted": bool(self._device["STATUS"].get("isEncrypt")),
-            "encrypted_pwd_hash": self._device["STATUS"].get("encryptPwd"),
+            "encrypted": bool(self.fetch_key(["STATUS", "isEncrypt"])),
+            "encrypted_pwd_hash": self.fetch_key(["STATUS", "encryptPwd"]),
             "local_ip": self._local_ip(),
-            "wan_ip": self._device["CONNECTION"].get("netIp"),
-            "mac_address": self._device["deviceInfos"].get("mac"),
-            "local_rtsp_port": self._device["CONNECTION"].get("localRtspPort", "554")
-            if self._device["CONNECTION"].get("localRtspPort", "554") != 0
+            "wan_ip": self.fetch_key(["CONNECTION", "netIp"]),
+            "mac_address": self.fetch_key(["deviceInfos", "mac"]),
+            "local_rtsp_port": self.fetch_key(["CONNECTION", "localRtspPort"], "554")
+            if self.fetch_key(["CONNECTION", "localRtspPort"], "554") != 0
             else "554",
-            "supported_channels": self._device["deviceInfos"].get("channelNumber"),
-            "battery_level": self._device["STATUS"]
-            .get("optionals", {})
-            .get("powerRemaining"),
-            "battery_camera_work_mode": self._device["STATUS"]
-            .get("optionals", {})
-            .get("batteryCameraWorkMode"),
-            "Alarm_DetectHumanCar": self._device["STATUS"]
-            .get("optionals", {})
-            .get("Alarm_DetectHumanCar"),
-            "NightVision_Model": self._device["STATUS"]
-            .get("optionals", {})
-            .get("NightVision_Model"),
-            "PIR_Status": self._device["STATUS"].get("pirStatus"),
-            "Motion_Trigger": self._alarmmotiontrigger.get("alarm_trigger_active"),
-            "Seconds_Last_Trigger": self._alarmmotiontrigger.get("timepassed"),
-            "last_alarm_time": self._last_alarm.get("alarmStartTimeStr"),
+            "supported_channels": self.fetch_key(["deviceInfos", "channelNumber"]),
+            "battery_level": self.fetch_key(["STATUS", "optionals", "powerRemaining"]),
+            "PIR_Status": self.fetch_key(["STATUS", "pirStatus"]),
+            "Motion_Trigger": self._alarmmotiontrigger["alarm_trigger_active"],
+            "Seconds_Last_Trigger": self._alarmmotiontrigger["timepassed"],
+            "last_alarm_time": self._last_alarm.get(
+                "alarmStartTimeStr", "2000-01-01 00:00:00"
+            ),
             "last_alarm_pic": self._last_alarm.get(
                 "picUrl",
                 "https://eustatics.ezvizlife.com/ovs_mall/web/img/index/EZVIZ_logo.png?ver=3007907502",
             ),
             "last_alarm_type_code": self._last_alarm.get("alarmType", "0000"),
             "last_alarm_type_name": self._last_alarm.get("sampleName", "NoAlarm"),
-            "alarm_light_luminance": int(
-                "".join(
-                    filter(
-                        str.isdigit,
-                        self._device["STATUS"]
-                        .get("optionals", {})
-                        .get("Alarm_Light", "0"),
-                    )
-                )
-            ),  # extract the value from the string and cater for the case where the value is not set.
-            "wifiInfos": self._device.get("WIFI"),
+            "cam_timezone": self.fetch_key(["STATUS", "optionals", "timeZone"]),
+            "push_notify_alarm": not bool(self.fetch_key(["NODISTURB", "alarmEnable"])),
+            "push_notify_call": not bool(
+                self.fetch_key(["NODISTURB", "callingEnable"])
+            ),
+            "alarm_light_luminance": self.fetch_key(
+                ["STATUS", "optionals", "Alarm_Light", "luminance"]
+            ),
+            "Alarm_DetectHumanCar": self.fetch_key(
+                ["STATUS", "optionals", "Alarm_DetectHumanCar", "type"]
+            ),
+            "diskCapacity": string_to_list(
+                self.fetch_key(["STATUS", "optionals", "diskCapacity"])
+            ),
+            "NightVision_Model": self.fetch_key(
+                ["STATUS", "optionals", "NightVision_Model"]
+            ),
+            "batteryCameraWorkMode": self.fetch_key(
+                ["STATUS", "optionals", "workMode"]
+            ),
+            "wifiInfos": self._device["WIFI"],
             "switches": self._switch,
+            "optionals": self.fetch_key(["STATUS", "optionals"]),
             "supportExt": self._device["deviceInfos"]["supportExt"],
+            "ezDeviceCapability": self.fetch_key(["deviceInfos", "ezDeviceCapability"]),
         }
 
     def move(self, direction: str, speed: int = 5) -> bool:
         """Move camera."""
         if direction not in ["right", "left", "down", "up"]:
             raise PyEzvizError(f"Invalid direction: {direction} ")
```

### Comparing `pyezviz-0.2.1.7/pyezviz/cas.py` & `pyezviz-0.2.2.0/pyezviz/cas.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,30 @@
         xor_msg = bytes(a ^ b for a, b in zip(stream.read(), cycle(xor_key)))
     return xor_msg
 
 
 class EzvizCAS:
     """Ezviz CAS server client."""
 
-    def __init__(self, token):
+    def __init__(self, token) -> None:
         """Initialize the client object."""
         self._session = None
         self._token = token or {
             "session_id": None,
             "rf_session_id": None,
             "username": None,
             "api_url": "apiieu.ezvizlife.com",
         }
         self._service_urls = token["service_urls"]
 
     def cas_get_encryption(self, devserial):
         """Fetch encryption code from ezviz cas server."""
 
         # Random hex 64 characters long.
-        rand_hex = random.randrange(10 ** 80)
+        rand_hex = random.randrange(10**80)
         rand_hex = "%064x" % rand_hex
         rand_hex = rand_hex[:64]
 
         payload = (
             f"\x9e\xba\xac\xe9\x01\x00\x00\x00\x00\x00"
             f"\x00\x02"  # Check or order?
             f"\x00\x00\x00\x00\x00\x00 "
@@ -90,15 +90,15 @@
 
         return response
 
     def set_camera_defence_state(self, serial, enable=1):
         """Enable alarm notifications."""
 
         # Random hex 64 characters long.
-        rand_hex = random.randrange(10 ** 80)
+        rand_hex = random.randrange(10**80)
         rand_hex = "%064x" % rand_hex
         rand_hex = rand_hex[:64]
 
         payload = (
             f"\x9e\xba\xac\xe9\x01\x00\x00\x00\x00\x00"
             f"\x00\x14"  # Check or order?
             f"\x00\x00\x00\x00\x00\x00 "
```

### Comparing `pyezviz-0.2.1.7/pyezviz/client.py` & `pyezviz-0.2.2.0/pyezviz/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 from .exceptions import (
     EzvizAuthTokenExpired,
     EzvizAuthVerificationCode,
     HTTPError,
     InvalidURL,
     PyEzvizError,
 )
+from .utils import convert_to_dict
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class EzvizClient:
     """Initialize api client object."""
 
@@ -729,15 +730,19 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
-                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                _LOGGER.warning(
+                    "Can't get storage status from device %s, retrying %s",
+                    serial,
+                    max_retries,
+                )
                 return self.get_storage_status(serial, max_retries + 1)
             raise PyEzvizError(
                 f"Could not get device storage status: Got {json_output})"
             )
 
         return json_output["storageStatus"]
 
@@ -944,15 +949,19 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
-                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                _LOGGER.warning(
+                    "Unable to reboot camera, camera %s is unreachable, retrying %s",
+                    serial,
+                    max_retries,
+                )
                 return self.reboot_camera(serial, delay, operation, max_retries + 1)
             raise PyEzvizError(f"Could not reboot device {json_output})")
 
         return True
 
     def get_group_defence_mode(self, max_retries: int = 0) -> Any:
         """Get group arm status. The alarm arm/disarm concept on 1st page of app."""
@@ -1108,14 +1117,15 @@
                 "WIFI": devices.get("WIFI", {}).get(_serial, {}),
                 "deviceInfos": device,
             }
             # Nested keys are still encoded as JSON strings
             result[_serial]["deviceInfos"]["supportExt"] = json.loads(
                 result[_serial]["deviceInfos"]["supportExt"]
             )
+            convert_to_dict(result[_serial]["STATUS"].get("optionals"))
 
         if not serial:
             return result
 
         return result.get(serial, {})
 
     def ptz_control(
@@ -1210,15 +1220,19 @@
             ) from err
 
         if json_output["resultCode"] == "20002":
             raise EzvizAuthVerificationCode(f"MFA code required: Got {json_output})")
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
-                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                _LOGGER.warning(
+                    "Camera %s encryption key not found, retrying %s",
+                    serial,
+                    max_retries,
+                )
                 return self.get_cam_key(serial, smscode, max_retries + 1)
             raise PyEzvizError(
                 f"Could not get camera encryption key: Got {json_output})"
             )
 
         return json_output
 
@@ -1254,15 +1268,19 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
-                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                _LOGGER.warning(
+                    "Create panoramic failed on device %s retrying %s",
+                    serial,
+                    max_retries,
+                )
                 return self.create_panoramic(serial, max_retries + 1)
             raise PyEzvizError(
                 f"Could not send command to create panoramic photo: Got {json_output})"
             )
 
         return json_output
 
@@ -1298,15 +1316,17 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
-                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                _LOGGER.warning(
+                    "Camera %s busy or unreachable, retrying %s", serial, max_retries
+                )
                 return self.return_panoramic(serial, max_retries + 1)
             raise PyEzvizError(f"Could retrieve panoramic photo: Got {json_output})")
 
         return json_output
 
     def ptz_control_coordinates(
         self, serial: str, x_axis: float, y_axis: float
@@ -1503,15 +1523,17 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
-                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                _LOGGER.warning(
+                    "Camara %s offline or unreachable, retrying %s", serial, max_retries
+                )
                 return self.api_set_defence_schedule(
                     serial, schedule, enable, max_retries + 1
                 )
             raise PyEzvizError(f"Could not set the schedule: Got {json_output})")
 
         return True
 
@@ -1558,15 +1580,15 @@
 
     def do_not_disturb(
         self,
         serial: str,
         enable: int = 1,
         channelno: int = 1,
         max_retries: int = 0,
-    ) -> bool | str:
+    ) -> bool:
         """Set do not disturb on camera with specified serial."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
         try:
             req = self._session.put(
                 "https://"
@@ -1581,26 +1603,26 @@
             )
             req.raise_for_status()
 
         except requests.HTTPError as err:
             if err.response.status_code == 401:
                 # session is wrong, need to re-log-in
                 self.login()
-                return self.do_not_disturb(serial, enable, max_retries + 1)
+                return self.do_not_disturb(serial, enable, channelno, max_retries + 1)
 
             raise HTTPError from err
 
         try:
             json_output = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(f"Could not set defence mode: Got {json_output})")
+            raise PyEzvizError(f"Could not set do not disturb: Got {json_output})")
 
         return True
 
     def set_floodlight_brightness(
         self,
         serial: str,
         luminance: int = 50,
@@ -1700,15 +1722,19 @@
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["resultCode"] != "0":
             if response_json["resultCode"] == "-1":
-                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                _LOGGER.warning(
+                    "Camera %s is offline, can't set sensitivity, retrying %s",
+                    serial,
+                    max_retries,
+                )
                 return self.detection_sensibility(
                     serial, sensibility, type_value, max_retries + 1
                 )
             raise PyEzvizError(
                 f"Unable to set detection sensibility. Got: {response_json}"
             )
 
@@ -1748,15 +1774,17 @@
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["resultCode"] != "0":
             if response_json["resultCode"] == "-1":
-                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                _LOGGER.warning(
+                    "Camera %s is offline, retrying %s", serial, max_retries
+                )
                 return self.get_detection_sensibility(
                     serial, type_value, max_retries + 1
                 )
             raise PyEzvizError(
                 f"Unable to get detection sensibility. Got: {response_json}"
             )
```

### Comparing `pyezviz-0.2.1.7/pyezviz/constants.py` & `pyezviz-0.2.2.0/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.7/pyezviz/exceptions.py` & `pyezviz-0.2.2.0/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.7/pyezviz/mqtt.py` & `pyezviz-0.2.2.0/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.7/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.2.0/pyezviz/test_cam_rtsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def __init__(
         self,
         ip_addr,
         username=None,
         password=None,
         test_uri="",
-    ):
+    ) -> None:
         """Initialize RTSP credential test."""
         self._rtsp_details = {
             "bufLen": 1024,
             "defaultServerIp": ip_addr,
             "defaultServerPort": 554,
             "defaultTestUri": test_uri,
             "defaultUserAgent": "RTSP Client",
```

### Comparing `pyezviz-0.2.1.7/setup.py` & `pyezviz-0.2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.1.7",
+    version="0.2.2.0",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

