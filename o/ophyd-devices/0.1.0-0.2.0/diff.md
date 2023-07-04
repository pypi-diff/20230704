# Comparing `tmp/ophyd_devices-0.1.0.tar.gz` & `tmp/ophyd_devices-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_devices-0.1.0.tar", last modified: Wed Jun 28 11:44:38 2023, max compression
+gzip compressed data, was "ophyd_devices-0.2.0.tar", last modified: Tue Jul  4 15:35:52 2023, max compression
```

## Comparing `ophyd_devices-0.1.0.tar` & `ophyd_devices-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.638876 ophyd_devices-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-28 11:44:38.638876 ophyd_devices-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.632876 ophyd_devices-0.1.0/ophyd_devices/
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-05-30 09:30:33.000000 ophyd_devices-0.1.0/ophyd_devices/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.632876 ophyd_devices-0.1.0/ophyd_devices/epics/
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/DeviceFactory.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.634876 ophyd_devices-0.1.0/ophyd_devices/epics/devices/
--rw-rw-rw-   0 root         (0) root         (0)     7222 2023-06-28 09:12:00.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/DelayGeneratorDG645.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/InsertionDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     3809 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/SpmBase.py
--rw-rw-rw-   0 root         (0) root         (0)    10676 2023-06-28 09:12:00.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/X07MADevices.py
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/XbpmBase.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/cSaxsVirtualMotors.py
--rw-rw-rw-   0 root         (0) root         (0)     4440 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/mono_dccm.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/slits.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-01 17:30:23.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/slsDetector.py
--rw-rw-rw-   0 root         (0) root         (0)     9182 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/epics/devices/specMotors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.634876 ophyd_devices-0.1.0/ophyd_devices/galil/
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-30 09:30:33.000000 ophyd_devices-0.1.0/ophyd_devices/galil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19024 2023-06-28 09:12:00.000000 ophyd_devices-0.1.0/ophyd_devices/galil/galil_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.635876 ophyd_devices-0.1.0/ophyd_devices/npoint/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/npoint/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16790 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/npoint/npoint.py
--rw-rw-rw-   0 root         (0) root         (0)    13172 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/npoint/npoint_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.635876 ophyd_devices-0.1.0/ophyd_devices/rt_lamni/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/rt_lamni/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31617 2023-06-28 09:12:00.000000 ophyd_devices-0.1.0/ophyd_devices/rt_lamni/rt_lamni_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.636876 ophyd_devices-0.1.0/ophyd_devices/sim/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-03 16:27:08.000000 ophyd_devices-0.1.0/ophyd_devices/sim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28877 2023-06-28 09:12:00.000000 ophyd_devices-0.1.0/ophyd_devices/sim/sim.py
--rw-rw-rw-   0 root         (0) root         (0)     7018 2023-05-09 16:42:37.000000 ophyd_devices-0.1.0/ophyd_devices/sim/sim_xtreme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.636876 ophyd_devices-0.1.0/ophyd_devices/smaract/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/smaract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/smaract/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)    19903 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/smaract/smaract_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     5212 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/smaract/smaract_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10338 2023-06-28 09:12:00.000000 ophyd_devices-0.1.0/ophyd_devices/smaract/smaract_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.637876 ophyd_devices-0.1.0/ophyd_devices/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/utils/controller.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-04-24 16:29:59.000000 ophyd_devices-0.1.0/ophyd_devices/utils/re_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7014 2023-06-28 09:12:00.000000 ophyd_devices-0.1.0/ophyd_devices/utils/socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:44:38.638876 ophyd_devices-0.1.0/ophyd_devices.egg-info/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-28 11:44:38.000000 ophyd_devices-0.1.0/ophyd_devices.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1506 2023-06-28 11:44:38.000000 ophyd_devices-0.1.0/ophyd_devices.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 11:44:38.000000 ophyd_devices-0.1.0/ophyd_devices.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-28 11:44:38.000000 ophyd_devices-0.1.0/ophyd_devices.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-28 11:44:38.000000 ophyd_devices-0.1.0/ophyd_devices.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-06-28 11:44:38.638876 ophyd_devices-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-28 11:44:36.000000 ophyd_devices-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.644825 ophyd_devices-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-04 15:35:52.644825 ophyd_devices-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-06-28 12:25:42.000000 ophyd_devices-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.634825 ophyd_devices-0.2.0/ophyd_devices/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-04 15:35:41.000000 ophyd_devices-0.2.0/ophyd_devices/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.635825 ophyd_devices-0.2.0/ophyd_devices/epics/
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/DeviceFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.638825 ophyd_devices-0.2.0/ophyd_devices/epics/devices/
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-04 15:35:41.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/DelayGeneratorDG645.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/InsertionDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/SpmBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    10676 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/X07MADevices.py
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/XbpmBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/cSaxsVirtualMotors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4440 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/mono_dccm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/slits.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/slsDetector.py
+-rw-rw-rw-   0 root         (0) root         (0)     9182 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/specMotors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.638825 ophyd_devices-0.2.0/ophyd_devices/galil/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-04 15:35:41.000000 ophyd_devices-0.2.0/ophyd_devices/galil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19024 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/galil/galil_ophyd.py
+-rw-r--r--   0 root         (0) root         (0)    19824 2023-07-04 15:35:41.000000 ophyd_devices-0.2.0/ophyd_devices/galil/sgalil_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.639825 ophyd_devices-0.2.0/ophyd_devices/npoint/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/npoint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16790 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/npoint/npoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    13172 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/npoint/npoint_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.640825 ophyd_devices-0.2.0/ophyd_devices/rt_lamni/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/rt_lamni/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    31617 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/rt_lamni/rt_lamni_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.640825 ophyd_devices-0.2.0/ophyd_devices/sim/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/sim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28877 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/sim/sim.py
+-rw-rw-rw-   0 root         (0) root         (0)     7018 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/sim/sim_xtreme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.642825 ophyd_devices-0.2.0/ophyd_devices/smaract/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)    19903 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     5212 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10338 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.643825 ophyd_devices-0.2.0/ophyd_devices/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3269 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/utils/controller.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/utils/re_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/utils/socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.643825 ophyd_devices-0.2.0/ophyd_devices.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-04 15:35:52.644825 ophyd_devices-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-04 15:35:50.000000 ophyd_devices-0.2.0/setup.py
```

### Comparing `ophyd_devices-0.1.0/LICENSE` & `ophyd_devices-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/DeviceFactory.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/DeviceFactory.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/__init__.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/DelayGeneratorDG645.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/DelayGeneratorDG645.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Created on Tue Nov  9 16:12:47 2021
 
 @author: mohacsi_i
 """
 
 from ophyd import Device, Component, EpicsSignal, EpicsSignalRO, Kind
-from ophyd import PositionerBase
+from ophyd import PositionerBase, PVPositioner, Signal
 from ophyd.pseudopos import (
     pseudo_position_argument,
     real_position_argument,
     PseudoSingle,
     PseudoPositioner,
 )
 
@@ -36,30 +36,33 @@
         EpicsSignal, "OutputAmpAI", write_pv="OutputAmpAO", name="amplitude", kind=Kind.config
     )
     polarity = Component(
         EpicsSignal, "OutputOffsetAI", write_pv="OutputOffsetAO", name="offset", kind=Kind.config
     )
 
 
-class DummyPositioner(Device, PositionerBase):
-    setpoint = Component(EpicsSignal, "DelayAO", kind=Kind.config)
+class DummyPositioner(PVPositioner):
+    setpoint = Component(EpicsSignal, "DelayAO", put_complete=True, kind=Kind.config)
     readback = Component(EpicsSignalRO, "DelayAI", kind=Kind.config)
+    done = Component(Signal, value=1)
 
 
 class DelayPair(PseudoPositioner):
     """Delay pair interface for DG645
 
     Virtual motor interface to a pair of signals (on the frontpanel).
     It offers a simple delay and pulse width interface for scanning.
     """
 
     # The pseudo positioner axes
     delay = Component(PseudoSingle, limits=(0, 2000.0), name="delay")
     width = Component(PseudoSingle, limits=(0, 2000.0), name="pulsewidth")
     # The real delay axes
+    # ch1 = Component(EpicsSignal, "DelayAI", write_pv="DelayAO", name="ch1", put_complete=True, kind=Kind.config)
+    # ch2 = Component(EpicsSignal, "DelayAI", write_pv="DelayAO", name="ch2", put_complete=True, kind=Kind.config)
     ch1 = Component(DummyPositioner, name="ch1")
     ch2 = Component(DummyPositioner, name="ch2")
 
     def __init__(self, *args, **kwargs):
         # Change suffix names before connecting (a bit of dynamic connections)
         self.__class__.__dict__["ch1"].suffix = kwargs["channel"][0]
         self.__class__.__dict__["ch2"].suffix = kwargs["channel"][1]
@@ -146,17 +149,15 @@
         "TriggerRateAI",
         write_pv="TriggerRateAO",
         name="trigger_rate",
         kind=Kind.config,
     )
 
     # Command PVs
-    arm = Component(
-        EpicsSignal, "TriggerDelayBI", write_pv="TriggerDelayBO", name="arm", kind=Kind.omitted
-    )
+    arm = Component(EpicsSignal, "TriggerDelayBO", name="arm", kind=Kind.omitted)
 
     # Burst mode
     burstMode = Component(
         EpicsSignal, "BurstModeBI", write_pv="BurstModeBO", name="burstmode", kind=Kind.config
     )
     burstConfig = Component(
         EpicsSignal, "BurstConfigBI", write_pv="BurstConfigBO", name="burstconfig", kind=Kind.config
```

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/InsertionDevice.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/InsertionDevice.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/SpmBase.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/SpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/X07MADevices.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/X07MADevices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/XbpmBase.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/XbpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/__init__.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/cSaxsVirtualMotors.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/cSaxsVirtualMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/mono_dccm.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/mono_dccm.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/slits.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/slits.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/slsDetector.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/slsDetector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/epics/devices/specMotors.py` & `ophyd_devices-0.2.0/ophyd_devices/epics/devices/specMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/galil/galil_ophyd.py` & `ophyd_devices-0.2.0/ophyd_devices/galil/galil_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/npoint/npoint.py` & `ophyd_devices-0.2.0/ophyd_devices/npoint/npoint.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/npoint/npoint_ophyd.py` & `ophyd_devices-0.2.0/ophyd_devices/npoint/npoint_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/rt_lamni/rt_lamni_ophyd.py` & `ophyd_devices-0.2.0/ophyd_devices/rt_lamni/rt_lamni_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/sim/sim.py` & `ophyd_devices-0.2.0/ophyd_devices/sim/sim.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/sim/sim_xtreme.py` & `ophyd_devices-0.2.0/ophyd_devices/sim/sim_xtreme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/smaract/serializer.py` & `ophyd_devices-0.2.0/ophyd_devices/smaract/serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/smaract/smaract_controller.py` & `ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/smaract/smaract_errors.py` & `ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_errors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/smaract/smaract_ophyd.py` & `ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/utils/controller.py` & `ophyd_devices-0.2.0/ophyd_devices/utils/controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices/utils/socket.py` & `ophyd_devices-0.2.0/ophyd_devices/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.1.0/ophyd_devices.egg-info/SOURCES.txt` & `ophyd_devices-0.2.0/ophyd_devices.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ./ophyd_devices/epics/devices/cSaxsVirtualMotors.py
 ./ophyd_devices/epics/devices/mono_dccm.py
 ./ophyd_devices/epics/devices/slits.py
 ./ophyd_devices/epics/devices/slsDetector.py
 ./ophyd_devices/epics/devices/specMotors.py
 ./ophyd_devices/galil/__init__.py
 ./ophyd_devices/galil/galil_ophyd.py
+./ophyd_devices/galil/sgalil_ophyd.py
 ./ophyd_devices/npoint/__init__.py
 ./ophyd_devices/npoint/npoint.py
 ./ophyd_devices/npoint/npoint_ophyd.py
 ./ophyd_devices/rt_lamni/__init__.py
 ./ophyd_devices/rt_lamni/rt_lamni_ophyd.py
 ./ophyd_devices/sim/__init__.py
 ./ophyd_devices/sim/sim.py
```

### Comparing `ophyd_devices-0.1.0/setup.cfg` & `ophyd_devices-0.2.0/setup.cfg`

 * *Files identical despite different names*

