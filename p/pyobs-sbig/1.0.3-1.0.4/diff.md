# Comparing `tmp/pyobs_sbig-1.0.3.tar.gz` & `tmp/pyobs_sbig-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_sbig-1.0.3.tar", max compression
+gzip compressed data, was "pyobs_sbig-1.0.4.tar", max compression
```

## Comparing `pyobs_sbig-1.0.3.tar` & `pyobs_sbig-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1099 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/LICENSE
--rw-r--r--   0        0        0     1219 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/build.py
--rw-r--r--   0        0        0      121 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/pyobs_sbig/__init__.py
--rw-r--r--   0        0        0     1592 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/pyobs_sbig/sbig6303e.py
--rw-r--r--   0        0        0    10011 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/pyobs_sbig/sbigcamera.py
--rw-r--r--   0        0        0     7661 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/pyobs_sbig/sbigfiltercamera.py
--rw-r--r--   0        0        0     9399 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/pyobs_sbig/sbigudrv.pxd
--rw-r--r--   0        0        0    11096 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/pyobs_sbig/sbigudrv.pyx
--rw-r--r--   0        0        0      715 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    46914 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/src/csbigcam.cpp
--rw-r--r--   0        0        0     6041 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/src/csbigcam.h
--rw-r--r--   0        0        0    60914 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/src/csbigimg.cpp
--rw-r--r--   0        0        0    10777 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/src/csbigimg.h
--rw-r--r--   0        0        0      850 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/src/lpardrv.h
--rw-r--r--   0        0        0    28066 2023-07-03 09:54:28.575608 pyobs_sbig-1.0.3/src/sbigudrv.h
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 pyobs_sbig-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1219 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/build.py
+-rw-r--r--   0        0        0      121 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/__init__.py
+-rw-r--r--   0        0        0     1592 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbig6303e.py
+-rw-r--r--   0        0        0    10011 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbigcamera.py
+-rw-r--r--   0        0        0     7661 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbigfiltercamera.py
+-rw-r--r--   0        0        0     9399 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbigudrv.pxd
+-rw-r--r--   0        0        0     9472 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbigudrv.pyx
+-rw-r--r--   0        0        0      715 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    46914 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/src/csbigcam.cpp
+-rw-r--r--   0        0        0     6041 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/src/csbigcam.h
+-rw-r--r--   0        0        0    60914 2023-07-04 18:33:27.886204 pyobs_sbig-1.0.4/src/csbigimg.cpp
+-rw-r--r--   0        0        0    10777 2023-07-04 18:33:27.886204 pyobs_sbig-1.0.4/src/csbigimg.h
+-rw-r--r--   0        0        0      850 2023-07-04 18:33:27.886204 pyobs_sbig-1.0.4/src/lpardrv.h
+-rw-r--r--   0        0        0    28066 2023-07-04 18:33:27.886204 pyobs_sbig-1.0.4/src/sbigudrv.h
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 pyobs_sbig-1.0.4/PKG-INFO
```

### Comparing `pyobs_sbig-1.0.3/LICENSE` & `pyobs_sbig-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/build.py` & `pyobs_sbig-1.0.4/build.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/pyobs_sbig/sbig6303e.py` & `pyobs_sbig-1.0.4/pyobs_sbig/sbig6303e.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/pyobs_sbig/sbigcamera.py` & `pyobs_sbig-1.0.4/pyobs_sbig/sbigcamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/pyobs_sbig/sbigfiltercamera.py` & `pyobs_sbig-1.0.4/pyobs_sbig/sbigfiltercamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/pyobs_sbig/sbigudrv.pxd` & `pyobs_sbig-1.0.4/pyobs_sbig/sbigudrv.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/pyobs_sbig/sbigudrv.pyx` & `pyobs_sbig-1.0.4/pyobs_sbig/sbigudrv.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -7,22 +7,14 @@
 import numpy as np
 cimport numpy as np
 np.import_array()
 
 from .sbigudrv cimport *
 
 
-@contextmanager
-def acquire_lock(lock):
-    if not lock.acquire(timeout=5):
-        raise ValueError('Could not acquire exclusive lock on camera.')
-    yield
-    lock.release()
-
-
 class FilterWheelModel(Enum):
     UNKNOWN = CFW_MODEL_SELECT.CFWSEL_UNKNOWN
     CFW2 = CFW_MODEL_SELECT.CFWSEL_CFW2
     CFW5 = CFW_MODEL_SELECT.CFWSEL_CFW5
     CFW8 = CFW_MODEL_SELECT.CFWSEL_CFW8
     CFWL = CFW_MODEL_SELECT.CFWSEL_CFWL
     CFW402 = CFW_MODEL_SELECT.CFWSEL_CFW402
@@ -120,237 +112,203 @@
     def establish_link(self):
         res = self.obj.EstablishLink()
         if res != 0:
             raise ValueError(self.obj.GetErrorString(res))
 
     @property
     def sensor(self) -> ActiveSensor:
-        with acquire_lock(self.lock):
-            return ActiveSensor(self.obj.GetActiveCCD())
+        return ActiveSensor(self.obj.GetActiveCCD())
 
     @sensor.setter
     def sensor(self, camera: ActiveSensor):
-        with acquire_lock(self.lock):
-            self.obj.SetActiveCCD(camera.value)
+        self.obj.SetActiveCCD(camera.value)
 
     @property
     def readout_mode(self):
-        with acquire_lock(self.lock):
-            return self.obj.GetReadoutMode()
+        return self.obj.GetReadoutMode()
 
     @readout_mode.setter
     def readout_mode(self, rm):
-        with acquire_lock(self.lock):
-            self.obj.SetReadoutMode(rm)
+        self.obj.SetReadoutMode(rm)
 
     @property
     def full_frame(self) -> Tuple[int, int, int, int]:
         # define width and height
         cdef int width = 0
         cdef int height = 0
 
-        # acquire lock
-        with acquire_lock(self.lock):
-            # call library
-            res = self.obj.GetFullFrame(width, height)
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
-            return 0, 0, width, height
+        # call library
+        res = self.obj.GetFullFrame(width, height)
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
+        return 0, 0, width, height
 
     @property
     def window(self):
         # define left, top, width and height
         cdef int left = 0
         cdef int top = 0
         cdef int width = 0
         cdef int height = 0
 
-        # acquire lock
-        with acquire_lock(self.lock):
-            # call library
-            self.obj.GetSubFrame(left, top, width, height)
-            return left, top, width, height
+        # call library
+        self.obj.GetSubFrame(left, top, width, height)
+        return left, top, width, height
 
     @window.setter
     def window(self, wnd):
         # set window
-        with acquire_lock(self.lock):
-            self.obj.SetSubFrame(wnd[0], wnd[1], wnd[2], wnd[3])
+        self.obj.SetSubFrame(wnd[0], wnd[1], wnd[2], wnd[3])
 
     @property
     def binning(self):
-        # acquire lock
-        with acquire_lock(self.lock):
-            # get readout mode
-            mode = self.obj.GetReadoutMode()
-
-            # return it
-            # 0 = No binning, high resolution
-            # 1 = 2x2 on-chip binning, medium resolution
-            # 2 = 3x3 on-chip binning, low resolution (ST-7/8/etc/237 only)
-            if mode in [0, 1, 2]:
-                return mode + 1, mode + 1
-            else:
-                raise ValueError('Unknown readout mode.')
+        # get readout mode
+        mode = self.obj.GetReadoutMode()
+
+        # return it
+        # 0 = No binning, high resolution
+        # 1 = 2x2 on-chip binning, medium resolution
+        # 2 = 3x3 on-chip binning, low resolution (ST-7/8/etc/237 only)
+        if mode in [0, 1, 2]:
+            return mode + 1, mode + 1
+        else:
+            raise ValueError('Unknown readout mode.')
 
     @binning.setter
     def binning(self, binning):
         # check
         if binning[0] != binning[1] or binning[0] < 1 or binning[0] > 3:
             raise ValueError('Only 1x1, 2x2, and 3x3 binnings supported.')
 
         # set it
-        with acquire_lock(self.lock):
-            self.obj.SetReadoutMode(binning[0] - 1)
+        self.obj.SetReadoutMode(binning[0] - 1)
 
     @property
     def exposure_time(self):
-        with acquire_lock(self.lock):
-            return self.obj.GetExposureTime()
+        return self.obj.GetExposureTime()
 
     @exposure_time.setter
     def exposure_time(self, exp):
-        with acquire_lock(self.lock):
-            self.obj.SetExposureTime(exp)
+        self.obj.SetExposureTime(exp)
 
     @property
     def temperature(self):
         cdef double temp = 0
 
-        # acquire lock
-        with acquire_lock(self.lock):
-            # get temp
-            res = self.obj.GetCCDTemperature(temp)
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
-            return temp
+        # get temp
+        res = self.obj.GetCCDTemperature(temp)
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
+        return temp
 
     def set_cooling(self, enable: bool, setpoint: float):
-        # acquire lock
-        with acquire_lock(self.lock):
-            res = self.obj.SetTemperatureRegulation(enable, setpoint)
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
+        res = self.obj.SetTemperatureRegulation(enable, setpoint)
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
 
     def get_cooling(self):
         # define vars
         cdef MY_LOGICAL enabled = 0
         cdef double temp = 0.
         cdef double setpoint = 0.
         cdef double power = 0.
 
-        # acquire lock
-        with acquire_lock(self.lock):
-            # get it
-            res = self.obj.QueryTemperatureStatus(enabled, temp, setpoint, power)
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
-            return enabled == 1, temp, setpoint, power
+        # get it
+        res = self.obj.QueryTemperatureStatus(enabled, temp, setpoint, power)
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
+        return enabled == 1, temp, setpoint, power
 
     def abort(self):
         # abort exposure
         self.aborted = True
 
     def was_aborted(self):
         return self.aborted
 
     def start_exposure(self, img: SBIGImg, shutter: bool):
          # define vars
         cdef MY_LOGICAL complete = 0
 
-        # acquire lock
-        with acquire_lock(self.lock):
-            # not aborted
-            self.aborted = False
-
-            # get mode
-            mode = SBIG_DARK_FRAME.SBDF_LIGHT_ONLY if shutter else SBIG_DARK_FRAME.SBDF_DARK_ONLY
-
-            # do setup
-            res = self.obj.GrabSetup(img.obj, mode)
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
-
-            # end current exposure, if any
-            res = self.obj.EndExposure()
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
-
-            # start exposure
-            shutter_cmd = SHUTTER_COMMAND.SC_OPEN_SHUTTER if shutter else  SHUTTER_COMMAND.SC_CLOSE_SHUTTER
-            res = self.obj.StartExposure(shutter_cmd)
-            if res != 0:
-                raise ValueError('Could not start exposure: ' + str(self.obj.GetErrorString(res)))
+        # not aborted
+        self.aborted = False
+
+        # get mode
+        mode = SBIG_DARK_FRAME.SBDF_LIGHT_ONLY if shutter else SBIG_DARK_FRAME.SBDF_DARK_ONLY
+
+        # do setup
+        res = self.obj.GrabSetup(img.obj, mode)
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
+
+        # end current exposure, if any
+        res = self.obj.EndExposure()
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
+
+        # start exposure
+        shutter_cmd = SHUTTER_COMMAND.SC_OPEN_SHUTTER if shutter else  SHUTTER_COMMAND.SC_CLOSE_SHUTTER
+        res = self.obj.StartExposure(shutter_cmd)
+        if res != 0:
+            raise ValueError('Could not start exposure: ' + str(self.obj.GetErrorString(res)))
 
     def has_exposure_finished(self):
          # define vars
         cdef MY_LOGICAL complete = 0
 
-        # acquire lock
-        with acquire_lock(self.lock):
-            # is complete?
-            res = self.obj.IsExposureComplete(complete)
-            if res != 0:
-                raise ValueError('Could not get exposure status: ' + self.obj.GetErrorString(res))
+        # is complete?
+        res = self.obj.IsExposureComplete(complete)
+        if res != 0:
+            raise ValueError('Could not get exposure status: ' + self.obj.GetErrorString(res))
 
-            # break on error or if complete or aborted
-            return res != 0 or complete
+        # break on error or if complete or aborted
+        return res != 0 or complete
 
     def end_exposure(self):
-        # acquire lock
-        with acquire_lock(self.lock):
-            res = self.obj.EndExposure()
-            if res != 0:
-                raise ValueError('Could not end exposure: ' + str(self.obj.GetErrorString(res)))
+        res = self.obj.EndExposure()
+        if res != 0:
+            raise ValueError('Could not end exposure: ' + str(self.obj.GetErrorString(res)))
 
     @staticmethod
     cdef int _readout(CSBIGCam *cam, CSBIGImg *img, SBIG_DARK_FRAME mode) nogil:
         cdef int res = cam.Readout(img, mode)
         return res
 
     def readout(self, img: SBIGImg, shutter: bool):
         # get mode
         cdef SBIG_DARK_FRAME mode = SBIG_DARK_FRAME.SBDF_LIGHT_ONLY if shutter else SBIG_DARK_FRAME.SBDF_DARK_ONLY
         cdef int res = 0
 
-        # acquire lock
-        with acquire_lock(self.lock):
-            # do readout
-            with nogil:
-                res = int(SBIGCam._readout(self.obj, img.obj, mode))
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(int(res)))
+        # do readout
+        with nogil:
+            res = int(SBIGCam._readout(self.obj, img.obj, mode))
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(int(res)))
 
     def set_filter_wheel(self, wheel: FilterWheelModel, com_port: FilterWheelComPort = FilterWheelComPort.COM1):
-        # acquire lock
-        with acquire_lock(self.lock):
-            res = self.obj.SetCFWModel(wheel.value, com_port.value)
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
+        res = self.obj.SetCFWModel(wheel.value, com_port.value)
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
 
     def set_filter(self, position: FilterWheelPosition):
-        # acquire lock
-        with acquire_lock(self.lock):
-            res = self.obj.SetCFWPosition(position.value)
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
+        res = self.obj.SetCFWPosition(position.value)
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
 
     def get_filter_position_and_status(self):
         # define vars
         cdef CFW_POSITION position = CFW_POSITION.CFWP_UNKNOWN
         cdef CFW_STATUS status = CFW_STATUS.CFWS_UNKNOWN
 
-        # acquire lock
-        with acquire_lock(self.lock):
-            # request from driver
-            res = self.obj.GetCFWPositionAndStatus(position, status)
-            if res != 0:
-                raise ValueError(self.obj.GetErrorString(res))
-
-            # parse it, since for whatever reason, position can be a value not defined in CFW_POSITION...
-            try:
-                pos = FilterWheelPosition(position)
-            except ValueError:
-                pos = FilterWheelPosition.UNKNOWN
+        # request from driver
+        res = self.obj.GetCFWPositionAndStatus(position, status)
+        if res != 0:
+            raise ValueError(self.obj.GetErrorString(res))
+
+        # parse it, since for whatever reason, position can be a value not defined in CFW_POSITION...
+        try:
+            pos = FilterWheelPosition(position)
+        except ValueError:
+            pos = FilterWheelPosition.UNKNOWN
 
-            # return it
-            return pos, FilterWheelStatus(status)
+        # return it
+        return pos, FilterWheelStatus(status)
```

### Comparing `pyobs_sbig-1.0.3/pyproject.toml` & `pyobs_sbig-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobs-sbig"
-version = "1.0.3"
+version = "1.0.4"
 description = "pyobs module for SBIG cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['src']
 #build = 'build.py'
 
 [tool.poetry.build]
```

### Comparing `pyobs_sbig-1.0.3/src/csbigcam.cpp` & `pyobs_sbig-1.0.4/src/csbigcam.cpp`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/src/csbigcam.h` & `pyobs_sbig-1.0.4/src/csbigcam.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/src/csbigimg.cpp` & `pyobs_sbig-1.0.4/src/csbigimg.cpp`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/src/csbigimg.h` & `pyobs_sbig-1.0.4/src/csbigimg.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/src/lpardrv.h` & `pyobs_sbig-1.0.4/src/lpardrv.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/src/sbigudrv.h` & `pyobs_sbig-1.0.4/src/sbigudrv.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.3/PKG-INFO` & `pyobs_sbig-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobs-sbig
-Version: 1.0.3
+Version: 1.0.4
 Summary: pyobs module for SBIG cameras
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

