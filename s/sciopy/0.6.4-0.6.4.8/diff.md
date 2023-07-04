# Comparing `tmp/sciopy-0.6.4-py3-none-any.whl.zip` & `tmp/sciopy-0.6.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,22 @@
-Zip file size: 25454 bytes, number of entries: 17
+Zip file size: 28853 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx     1463 b- defN 23-May-05 08:25 sciopy/3d_mesh.py
--rw-rw-r--  2.0 unx     4256 b- defN 23-May-16 14:05 sciopy/__init__.py
+-rw-rw-r--  2.0 unx     4314 b- defN 23-Jun-27 08:45 sciopy/__init__.py
 -rw-rw-r--  2.0 unx     2314 b- defN 23-May-05 08:25 sciopy/com_handling.py
--rw-rw-r--  2.0 unx    16189 b- defN 23-May-17 07:09 sciopy/configurations.py
+-rw-rw-r--  2.0 unx    20457 b- defN 23-Jun-27 06:58 sciopy/configurations.py
 -rw-rw-r--  2.0 unx     4417 b- defN 23-May-05 08:25 sciopy/doteit.py
+-rw-rw-r--  2.0 unx      547 b- defN 23-May-25 14:34 sciopy/eth_2.py
+-rw-rw-r--  2.0 unx     1178 b- defN 23-May-25 14:34 sciopy/eth_3.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-May-25 14:34 sciopy/eth_4.py
 -rw-rw-r--  2.0 unx     4685 b- defN 23-May-05 08:25 sciopy/meshing.py
--rw-rw-r--  2.0 unx     8987 b- defN 23-May-17 07:57 sciopy/npztocsv.py
+-rw-rw-r--  2.0 unx     8987 b- defN 23-May-17 11:24 sciopy/npztocsv.py
 -rw-rw-r--  2.0 unx    11208 b- defN 23-May-05 08:25 sciopy/prepare_data.py
 -rw-rw-r--  2.0 unx     4372 b- defN 23-May-05 08:25 sciopy/print_command_info.py
--rw-rw-r--  2.0 unx     3484 b- defN 23-May-05 08:25 sciopy/sciopy_dataclasses.py
--rw-rw-r--  2.0 unx    20119 b- defN 23-May-17 07:19 sciopy/setup_m.py
+-rw-rw-r--  2.0 unx     3804 b- defN 23-Jun-28 07:17 sciopy/sciopy_dataclasses.py
+-rw-rw-r--  2.0 unx    20119 b- defN 23-Jun-28 07:21 sciopy/setup_m.py
 -rw-rw-r--  2.0 unx     7482 b- defN 23-May-05 08:25 sciopy/visualization.py
--rw-rw-r--  2.0 unx     1062 b- defN 23-May-17 08:05 sciopy-0.6.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2377 b- defN 23-May-17 08:05 sciopy-0.6.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-17 08:05 sciopy-0.6.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-17 08:05 sciopy-0.6.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1317 b- defN 23-May-17 08:05 sciopy-0.6.4.dist-info/RECORD
-17 files, 93831 bytes uncompressed, 23332 bytes compressed:  75.1%
+-rw-rw-r--  2.0 unx     1062 b- defN 23-Jul-04 11:07 sciopy-0.6.4.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3493 b- defN 23-Jul-04 11:07 sciopy-0.6.4.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 11:07 sciopy-0.6.4.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-04 11:07 sciopy-0.6.4.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1542 b- defN 23-Jul-04 11:07 sciopy-0.6.4.8.dist-info/RECORD
+20 files, 103054 bytes uncompressed, 26393 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -9,14 +9,23 @@
 
 Filename: sciopy/configurations.py
 Comment: 
 
 Filename: sciopy/doteit.py
 Comment: 
 
+Filename: sciopy/eth_2.py
+Comment: 
+
+Filename: sciopy/eth_3.py
+Comment: 
+
+Filename: sciopy/eth_4.py
+Comment: 
+
 Filename: sciopy/meshing.py
 Comment: 
 
 Filename: sciopy/npztocsv.py
 Comment: 
 
 Filename: sciopy/prepare_data.py
@@ -30,23 +39,23 @@
 
 Filename: sciopy/setup_m.py
 Comment: 
 
 Filename: sciopy/visualization.py
 Comment: 
 
-Filename: sciopy-0.6.4.dist-info/LICENSE
+Filename: sciopy-0.6.4.8.dist-info/LICENSE
 Comment: 
 
-Filename: sciopy-0.6.4.dist-info/METADATA
+Filename: sciopy-0.6.4.8.dist-info/METADATA
 Comment: 
 
-Filename: sciopy-0.6.4.dist-info/WHEEL
+Filename: sciopy-0.6.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: sciopy-0.6.4.dist-info/top_level.txt
+Filename: sciopy-0.6.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: sciopy-0.6.4.dist-info/RECORD
+Filename: sciopy-0.6.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sciopy/__init__.py

```diff
@@ -65,19 +65,20 @@
     GetBatteryControll,
     SetLEDControl,
     GetLEDControl,
     SetLED_Mode,
     DisableLED_AutoMode,
     EnableLED_AutoMode,
     PowerPlugDetect,
-    GetDevideInfo,
+    GetDeviceInfo,
     GetFirmwareIDs,
 )
 
 from .configurations import (
+    set_measurement_config,
     conf_n_el_16_adjacent,
     conf_n_el_32_adjacent,
     conf_n_el_16_opposite,
     conf_n_el_32_opposite,
 )
 
 from .npztocsv import (
@@ -139,17 +140,18 @@
     "GetBatteryControll",
     "SetLEDControl",
     "GetLEDControl",
     "SetLED_Mode",
     "DisableLED_AutoMode",
     "EnableLED_AutoMode",
     "PowerPlugDetect",
-    "GetDevideInfo",
+    "GetDeviceInfo",
     "GetFirmwareIDs",
     # .configurations
+    "set_measurement_config",
     "conf_n_el_16_adjacent",
     "conf_n_el_32_adjacent",
     "conf_n_el_16_opposite",
     "conf_n_el_32_opposite",
     # "configure_configuration",
     # .prepare_data
     "create_prep_directory",
```

## sciopy/configurations.py

```diff
@@ -1,10 +1,145 @@
 # TBD: https://stackoverflow.com/questions/3898572/what-are-the-most-common-python-docstring-formats
-from .sciopy_dataclasses import ScioSpecMeasurementConfig
+from .sciopy_dataclasses import (
+    ScioSpecMeasurementConfig,
+    ScioSpecMeasurementSetup,
+)
 from datetime import datetime
+import numpy as np
+from typing import Union
+import struct
+
+
+def set_measurement_config(serial, ssms: ScioSpecMeasurementSetup) -> None:
+    """
+    set_measurement_config sets the ScioSpec device configuration depending on the ssms configuration dataclass.
+
+    Parameters
+    ----------
+    serial : _type_
+        serial connection
+    ssms : ScioSpecMeasurementSetup
+        dataclass with the measurement setup settings.
+    """
+
+    def clTbt_sp(val: Union[int, float]) -> list:
+        """
+        clTbt_sp converts an integer or float value to a list of single precision bytes.
+
+        Parameters
+        ----------
+        val : Union[int, float]
+            Value that has to be converted
+
+        Returns
+        -------
+        list
+            list with single precision byte respresentation
+        """
+        return [int(bt) for bt in struct.pack(">f", val)]
+
+    def clTbt_dp(val: float) -> list:
+        """
+        clTbt_dp converts an integer or float value to a list of double precision bytes.
+
+        Parameters
+        ----------
+        val : float
+            value that has to be converted
+
+        Returns
+        -------
+        list
+            list with double precision byte respresentation
+        """
+        return [int(ele) for ele in struct.pack(">d", val)]
+
+    # Set measurement setup:
+    serial.write(bytearray([0xB0, 0x01, 0x01, 0xB0]))
+    # Set burst count: "B0 03 02 00 03 B0" = 3
+    serial.write(bytearray([0xB0, 0x03, 0x02, 0x00, ssms.burst_count, 0xB0]))
+
+    # Excitation amplitude double precision
+    # A_min = 100nA
+    # A_max = 10mA
+    if ssms.amplitude > 0.001:
+        print(f"Divide {ssms.amplitude}/1000. Out of available range")
+        ssms.amplitude = ssms.amplitude / 1000
+    serial.write(
+        bytearray(list(np.concatenate([[176, 9, 5], clTbt_dp(ssms.amplitude), [176]])))
+    )
+
+    # ADC range settings: [+/-1, +/-5, +/-10]
+    # ADC range = +/-1  : B0 02 0D 01 B0
+    # ADC range = +/-5  : B0 02 0D 02 B0
+    # ADC range = +/-10 : B0 02 0D 03 B0
+    if ssms.adc_range == 1:
+        serial.write(bytearray([0xB0, 0x02, 0x0D, 0x01, 0xB0]))
+    elif ssms.adc_range == 5:
+        serial.write(bytearray([0xB0, 0x02, 0x0D, 0x02, 0xB0]))
+    elif ssms.adc_range == 10:
+        serial.write(bytearray([0xB0, 0x02, 0x0D, 0x03, 0xB0]))
+
+    # Gain settings:
+    # Gain = 1     : B0 03 09 01 00 B0
+    # Gain = 10    : B0 03 09 01 01 B0
+    # Gain = 100   : B0 03 09 01 02 B0
+    # Gain = 1_000 : B0 03 09 01 03 B0
+    if ssms.gain == 1:
+        serial.write(bytearray([0xB0, 0x03, 0x09, 0x01, 0x00, 0xB0]))
+    elif ssms.gain == 10:
+        serial.write(bytearray([0xB0, 0x03, 0x09, 0x01, 0x01, 0xB0]))
+    elif ssms.gain == 100:
+        serial.write(bytearray([0xB0, 0x03, 0x09, 0x01, 0x02, 0xB0]))
+    elif ssms.gain == 1_000:
+        serial.write(bytearray([0xB0, 0x03, 0x09, 0x01, 0x03, 0xB0]))
+
+    # Single ended mode:
+    serial.write(bytearray([0xB0, 0x03, 0x08, 0x01, 0x01, 0xB0]))
+
+    # Excitation switch type:
+    serial.write(bytearray([0xB0, 0x02, 0x0C, 0x01, 0xB0]))
+
+    # Set framerate:
+    serial.write(
+        bytearray(list(np.concatenate([[176, 5, 3], clTbt_sp(ssms.framerate), [176]])))
+    )
+
+    # Set frequencies:
+    # [CT] 0C 04 [fmin] [fmax] [fcount] [ftype] [CT]
+    f_min = clTbt_sp(ssms.exc_freq)
+    f_max = clTbt_sp(ssms.exc_freq)
+    f_count = [0, 1]
+    f_type = [0]
+    # bytearray
+    serial.write(
+        bytearray(
+            list(np.concatenate([[176, 12, 4], f_min, f_max, f_count, f_type, [176]]))
+        )
+    )
+
+    # Set injection config
+
+    el_inj = np.arange(1, ssms.n_el + 1)
+    el_gnd = np.roll(el_inj, -(ssms.inj_skip + 1))
+
+    for v_el, g_el in zip(el_inj, el_gnd):
+        serial.write(bytearray([0xB0, 0x03, 0x06, v_el, g_el, 0xB0]))
+
+    # Get measurement setup
+    serial.write(bytearray([0xB1, 0x01, 0x03, 0xB1]))
+    # Set output configuration
+    serial.write(bytearray([0xB2, 0x02, 0x01, 0x01, 0xB2]))
+    serial.write(bytearray([0xB2, 0x02, 0x03, 0x01, 0xB2]))
+    serial.write(bytearray([0xB2, 0x02, 0x02, 0x01, 0xB2]))
+
+    ## start measurement
+    # serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
+    # stop measurement
+    # serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
 
 
 def conf_n_el_16_adjacent(
     serial, cnf: ScioSpecMeasurementConfig
 ) -> ScioSpecMeasurementConfig:
     """
     Amplitude 	1 mA
@@ -82,16 +217,16 @@
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x0E, 0x0F, 0xB0]))
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x0F, 0x10, 0xB0]))
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x10, 0x01, 0xB0]))
     serial.write(bytearray([0xB1, 0x01, 0x03, 0xB1]))
     serial.write(bytearray([0xB2, 0x02, 0x01, 0x01, 0xB2]))
     serial.write(bytearray([0xB2, 0x02, 0x03, 0x01, 0xB2]))
     serial.write(bytearray([0xB2, 0x02, 0x02, 0x01, 0xB2]))
-    serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
-    serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
+    # serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
+    # serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
     return ScioSpecMeasurementConfig(
         com_port=serial.name,
         burst_count=10,
         n_el=16,
         channel_group=[1],
         actual_sample=cnf.actual_sample,
         s_path=cnf.s_path,
@@ -184,16 +319,16 @@
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x0E, 0x06, 0xB0]))
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x0F, 0x07, 0xB0]))
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x10, 0x08, 0xB0]))
     serial.write(bytearray([0xB1, 0x01, 0x03, 0xB1]))
     serial.write(bytearray([0xB2, 0x02, 0x01, 0x01, 0xB2]))
     serial.write(bytearray([0xB2, 0x02, 0x03, 0x01, 0xB2]))
     serial.write(bytearray([0xB2, 0x02, 0x02, 0x01, 0xB2]))
-    serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
-    serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
+    # serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
+    # serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
     return ScioSpecMeasurementConfig(
         serial.name,
         burst_count=10,
         n_el=16,
         channel_group=[1],
         actual_sample=cnf.actual_sample,
         s_path=cnf.s_path,
@@ -302,16 +437,16 @@
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x1E, 0x1F, 0xB0]))
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x1F, 0x20, 0xB0]))
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x20, 0x01, 0xB0]))
     serial.write(bytearray([0xB1, 0x01, 0x03, 0xB1]))
     serial.write(bytearray([0xB2, 0x02, 0x01, 0x01, 0xB2]))
     serial.write(bytearray([0xB2, 0x02, 0x03, 0x01, 0xB2]))
     serial.write(bytearray([0xB2, 0x02, 0x02, 0x01, 0xB2]))
-    serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
-    serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
+    # serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
+    # serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
     return ScioSpecMeasurementConfig(
         serial.name,
         burst_count=1,
         n_el=32,
         channel_group=[1, 2],
         actual_sample=cnf.actual_sample,
         s_path=cnf.s_path,
@@ -420,16 +555,16 @@
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x1E, 0x0E, 0xB0]))
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x1F, 0x0F, 0xB0]))
     serial.write(bytearray([0xB0, 0x03, 0x06, 0x20, 0x10, 0xB0]))
     serial.write(bytearray([0xB1, 0x01, 0x03, 0xB1]))
     serial.write(bytearray([0xB2, 0x02, 0x01, 0x01, 0xB2]))
     serial.write(bytearray([0xB2, 0x02, 0x03, 0x01, 0xB2]))
     serial.write(bytearray([0xB2, 0x02, 0x02, 0x01, 0xB2]))
-    serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
-    serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
+    # serial.write(bytearray([0xB4, 0x01, 0x01, 0xB4]))
+    # serial.write(bytearray([0xB4, 0x01, 0x00, 0xB4]))
     return ScioSpecMeasurementConfig(
         serial.name,
         burst_count=1,
         n_el=32,
         channel_group=[1, 2],
         actual_sample=cnf.actual_sample,
         s_path=cnf.s_path,
```

## sciopy/sciopy_dataclasses.py

```diff
@@ -1,9 +1,25 @@
 from dataclasses import dataclass
-from typing import List, Tuple
+from typing import List, Tuple, Union
+
+
+@dataclass
+class ScioSpecMeasurementSetup:
+    burst_count: int
+    total_meas_num: int
+    n_el: int
+    channel_group: list
+    exc_freq: Union[int, float]
+    framerate: Union[int, float]
+    amplitude: Union[int, float]
+    inj_skip: str
+    gain: int
+    adc_range: int
+    notes: str
+    configured: bool
 
 
 @dataclass
 class SingleFrame:
     """
     This class is for parsing single excitation stages.
```

## sciopy/setup_m.py

```diff
@@ -784,15 +784,15 @@
     -------
     None
     """
     serial.write(bytearray([0xCC, 0x01, 0x81, 0xCC]))
     SystemMessageCallback(serial)
 
 
-def GetDevideInfo(serial) -> None:
+def GetDeviceInfo(serial) -> None:
     """
     Print device information.
 
     Parameters
     ----------
     serial :
         serial connection
```

## Comparing `sciopy-0.6.4.dist-info/LICENSE` & `sciopy-0.6.4.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sciopy-0.6.4.dist-info/RECORD` & `sciopy-0.6.4.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 sciopy/3d_mesh.py,sha256=PTGmUQXykeQjfyIdvHtmrSQmAKCimZ4KZIybpZD0BMc,1463
-sciopy/__init__.py,sha256=rw1pg5XuWhGIoeBpSa78lJblZC7Rh7--W-prp7JRbG4,4256
+sciopy/__init__.py,sha256=79GQiHhMZfE4Q4jW1HW5mhU9frFBqWjJqluwmhBTV1Q,4314
 sciopy/com_handling.py,sha256=U1ZMOKKRw65eWq1Jvrl6EnH7ogiurPkCJ4p1q96-8q4,2314
-sciopy/configurations.py,sha256=2IWVHKufzxIbRunSscUobNAccWsgJDA3vUp8dsj7cIM,16189
+sciopy/configurations.py,sha256=Cq-BhG4Oc2rrDHQpKq9w5pmURXUj1MiOTGTKx52psas,20457
 sciopy/doteit.py,sha256=WJjIWgYG_3abW848ccHxru3sHiBu9iRf98zWe2bSSxA,4417
+sciopy/eth_2.py,sha256=M9WMeG1BaKuVI_sx1Ts8licy36abFhRxUyWIJB6Bv2I,547
+sciopy/eth_3.py,sha256=yGO42YJjVwv5C5n1VvfooaK2g_TLxTNxp6A7wul6mUc,1178
+sciopy/eth_4.py,sha256=THHwPvoQzeku__AFkZB91KyOgF_kgGb2p-yr7WUCNeY,1511
 sciopy/meshing.py,sha256=jgBi9JUcOjTBn4gWgSpLsiPX3KiNqA0G4ZmJ6w1qGGs,4685
 sciopy/npztocsv.py,sha256=rAdSZO-BpiySK3gcFevkWLNoEuQNqHZVUqv3NCb3wo8,8987
 sciopy/prepare_data.py,sha256=Ad58NT1VaPZtQxGOPRhOfvVaqHk3M_de1QAYRlYKb68,11208
 sciopy/print_command_info.py,sha256=rBnZJ1Tl_-QRCQnfqfet-znl8XnN7wvXTV4Z4krbFGQ,4372
-sciopy/sciopy_dataclasses.py,sha256=Hi2X8q2RXyAiuTatI4z_2BHyKnIKYlR8trnjyo9FrGI,3484
-sciopy/setup_m.py,sha256=PlPLhDltfgPdpcX-bE0yKEDIpTeYCs7vugp9QiOtPoA,20119
+sciopy/sciopy_dataclasses.py,sha256=aAXWaUv4WgX9VmvZ0scywjvO_vyEhoArOi9aa0GotcA,3804
+sciopy/setup_m.py,sha256=2X9nBAE_S6o3dlTVxJsBewSBVdbL79eUPEN2CbKIkNE,20119
 sciopy/visualization.py,sha256=AW_cYLVrPvwArKLDeoxEDnTveZhF6HSBMdU9pqtGa2g,7482
-sciopy-0.6.4.dist-info/LICENSE,sha256=mvuu3JpofjFcd8rEvSAGR4EedNMH979iMwXp9BGi38Y,1062
-sciopy-0.6.4.dist-info/METADATA,sha256=kmM5GnL8GGJQnygj8YwCnZ4ctM3iPsf3HBXv1VxPvxQ,2377
-sciopy-0.6.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sciopy-0.6.4.dist-info/top_level.txt,sha256=Yfokv5CD23A5gda5ZEjDy0YfFwrFeo_EOXJLRv-QoEU,7
-sciopy-0.6.4.dist-info/RECORD,,
+sciopy-0.6.4.8.dist-info/LICENSE,sha256=mvuu3JpofjFcd8rEvSAGR4EedNMH979iMwXp9BGi38Y,1062
+sciopy-0.6.4.8.dist-info/METADATA,sha256=eOklcA4M49kNEBzfQJfZJ4f0c5dNC3iFxSvrD1XEcio,3493
+sciopy-0.6.4.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sciopy-0.6.4.8.dist-info/top_level.txt,sha256=Yfokv5CD23A5gda5ZEjDy0YfFwrFeo_EOXJLRv-QoEU,7
+sciopy-0.6.4.8.dist-info/RECORD,,
```

