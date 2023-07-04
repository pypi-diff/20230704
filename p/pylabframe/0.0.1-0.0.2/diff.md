# Comparing `tmp/pylabframe-0.0.1.tar.gz` & `tmp/pylabframe-0.0.2.tar.gz`

## Comparing `pylabframe-0.0.1.tar` & `pylabframe-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,27 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pylabframe-0.0.1/pylabframe/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pylabframe-0.0.1/pylabframe/general.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pylabframe-0.0.1/pylabframe/data/__init__.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pylabframe-0.0.1/pylabframe/data/general.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylabframe-0.0.1/pylabframe/hardware/__init__.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pylabframe-0.0.1/pylabframe/hardware/device.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 pylabframe-0.0.1/pylabframe/hardware/drivers.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 pylabframe-0.0.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pylabframe-0.0.1/LICENSE
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pylabframe-0.0.1/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pylabframe-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pylabframe-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/__init__.py
+-rwxr-xr-x   0        0        0     3741 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/config.py
+-rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/general.py
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/util.py
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/data/__init__.py
+-rwxr-xr-x   0        0        0    22026 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/data/core.py
+-rwxr-xr-x   0        0        0     6610 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/data/fitters.py
+-rwxr-xr-x   0        0        0     6991 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/data/path.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/data/loaders/__init__.py
+-rwxr-xr-x   0        0        0     2926 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/data/loaders/keysight_loader.py
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/hw/__init__.py
+-rwxr-xr-x   0        0        0     2473 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/hw/device.py
+-rwxr-xr-x   0        0        0     4675 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/hw/visadevice.py
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/hw/drivers/__init__.py
+-rwxr-xr-x   0        0        0     8233 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/hw/drivers/keysightvisa.py
+-rwxr-xr-x   0        0        0     1363 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/hw/drivers/santecvisa.py
+-rwxr-xr-x   0        0        0     4229 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pylabframe/hw/drivers/tekvisa.py
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 pylabframe-0.0.2/test/config_test.py
+-rwxr-xr-x   0        0        0     1420 2020-02-02 00:00:00.000000 pylabframe-0.0.2/test/data_test.py
+-rwxr-xr-x   0        0        0     3646 2020-02-02 00:00:00.000000 pylabframe-0.0.2/test/restack.npz
+-rwxr-xr-x   0        0        0     1580 2020-02-02 00:00:00.000000 pylabframe-0.0.2/test/tarr1.npz
+-rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 pylabframe-0.0.2/test/testconf.toml
+-rwxr-xr-x   0        0        0     3253 2020-02-02 00:00:00.000000 pylabframe-0.0.2/.gitignore
+-rwxr-xr-x   0        0        0     1088 2020-02-02 00:00:00.000000 pylabframe-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 pylabframe-0.0.2/README.md
+-rwxr-xr-x   0        0        0      729 2020-02-02 00:00:00.000000 pylabframe-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pylabframe-0.0.2/PKG-INFO
```

### Comparing `pylabframe-0.0.1/pylabframe/hardware/device.py` & `pylabframe-0.0.2/pylabframe/hw/visadevice.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,158 @@
 import pyvisa
-import pylabframe
-from enum import Enum
-
-_visa_rm = pyvisa.ResourceManager()
-_connected_devices = {}
+from . import device
 
+from enum import Enum, IntEnum
 
-def get_device(id):
-    if id in _connected_devices:
-        return _connected_devices[id]
-    else:
-        dev = _connect_device(id)
-        _connected_devices[id] = dev
-        return dev
+_visa_rm = pyvisa.ResourceManager()
 
 
-def _connect_device(id):
-    from . import drivers
-    hw_conf = read_hw_config()
-    device_parts = hw_conf[id].split("@")
-    device_class = device_parts[0]
-    device_address = "@".join(device_parts[1:])
+class EventStatusRegister:
+    class Functions(IntEnum):
+        OPC = 0
+        RQC = 1
+        QYE = 2
+        DDE = 3
+        EXE = 4
+        CME = 5
+        URQ = 6
+        PON = 7
+    ERROR_MASK = 0b00111100
+
+    def __init__(self, val):
+        self.esr = int(val)
+
+    def function_value(self, func):
+        return bool(self.esr & (1 << func))
+
+    @property
+    def is_error(self):
+        return bool(self.esr & self.ERROR_MASK)
+
+    @property
+    def command_error(self):
+        return self.function_value(self.Functions.CME)
+
+    @property
+    def execution_error(self):
+        return self.function_value(self.Functions.EXE)
+
+    @property
+    def device_error(self):
+        return self.function_value(self.Functions.DDE)
+
+    @property
+    def query_error(self):
+        return self.function_value(self.Functions.QYE)
+
+    def __repr__(self):
+        bits_set = []
+        for i in range(8):
+            if self.function_value(i):
+                bits_set.append(self.Functions(i))
+
+        bits_set = [b.name for b in bits_set]
+        return f"EventStatusRegister([{', '.join(bits_set)}])"
+
+
+DTYPE_CONVERTERS = {
+    bool: (device.intbool_conv, int),
+}
+
+
+def visa_property(visa_cmd: str, dtype=None, read_only=False, read_conv=str, write_conv=str, rw_conv=None, access_guard=None):
+    if rw_conv is not None:
+        read_conv = rw_conv
+        write_conv = rw_conv
+
+    if dtype is not None:
+        if dtype in DTYPE_CONVERTERS:
+            read_conv, write_conv = DTYPE_CONVERTERS[dtype]
+        else:
+            read_conv, write_conv = dtype, dtype
+            if issubclass(dtype, device.SettingEnum):
+                write_conv = str
+
+    def visa_getter(self: "VisaDevice"):
+        if access_guard is not None:
+            access_guard(self)
 
-    device_class = eval(f"drivers.{device_class}")
+        fmt_visa_cmd = visa_cmd
+        if hasattr(self, "query_params"):
+            # doing this gives us access to object properties (eg channel id) that can be put in the command string
+            fmt_visa_cmd = fmt_visa_cmd.format(**self.query_params)
+        response = self.instr.query(f"{fmt_visa_cmd}?")
+        response = read_conv(response.strip())
+        return response
 
-    dev = device_class(id, device_address)
+    if not read_only:
+        def visa_setter(self: "VisaDevice", value):
+            if access_guard is not None:
+                access_guard(self)
 
-    return dev
+            fmt_visa_cmd = visa_cmd
+            if hasattr(self, "query_params"):
+                fmt_visa_cmd = fmt_visa_cmd.format(**self.query_params)
+            cmd = f"{fmt_visa_cmd} {write_conv(value)}"
+            self.instr.write(cmd)
+    else:
+        visa_setter = None
 
+    prop = property(visa_getter, visa_setter)
 
-def read_hw_config(computer_name=None):
-    if computer_name is None:
-        computer_name = pylabframe.general.get_computer_name()
+    return prop
 
-    return pylabframe.general.load_config_file(f"hardware/{computer_name}")
 
+def visa_command(visa_cmd, wait_until_done=False):
+    def visa_executer(self: "VisaDevice", **kw):
+        if hasattr(self, "query_params"):
+            kw.update(self.query_params)
 
-class Device:
-    def __init__(self, id, error_on_double_connect=True, **kw):
-        if id in _connected_devices and error_on_double_connect:
-            raise RuntimeError(f"Device {id} already connected")
+        fmt_visa_cmd = visa_cmd.format(**kw)
+        if wait_until_done:
+            return self.wait_until_done(fmt_visa_cmd)
+        else:
+            return self.instr.write(fmt_visa_cmd)
 
-    @classmethod
-    def list_available(cls):
-        return []
+    return visa_executer
 
 
-class VisaDevice(Device):
+class VisaDevice(device.Device):
     def __init__(self, id, address, **kw):
         super().__init__(id, **kw)
         self.address = address
-        self.visa_instr: pyvisa.resources.messagebased.MessageBasedResource = _visa_rm.open_resource(address)
+        self.instr: pyvisa.resources.messagebased.MessageBasedResource = _visa_rm.open_resource(address)
 
     def __del__(self):
-        self.visa_instr.close()
-        del self.visa_instr
+        self.instr.close()
+        del self.instr
 
     @classmethod
     def list_available(cls):
         return list(_visa_rm.list_resources())
 
     def get_identifier(self, sanitize=True):
-        response = self.visa_instr.query("*IDN?")
+        response = self.instr.query("*IDN?")
         if sanitize:
             response = response.strip()
         return response
 
-    def wait_until_done(self):
-        self.visa_instr.write("*OPC?")
+    def wait_until_done(self, visa_cmd=None):
+        if visa_cmd is not None:
+            cmd_string = f"{visa_cmd};*OPC?"
+        else:
+            cmd_string = "*OPC?"
+        self.instr.write(cmd_string)
         is_done = False
         while not is_done:
             try:
-                self.visa_instr.read()
+                result_code = self.instr.read()
                 is_done = True
             except pyvisa.VisaIOError as e:
                 if e.error_code != pyvisa.constants.StatusCode.error_timeout:
                     # re-raise anything other than a time-out
                     raise e
+        return result_code
 
-    @classmethod
-    def visa_property(cls, visa_cmd: str, read_only=False, read_conv=str, write_conv=str):
-        def visa_getter(self: VisaDevice):
-            # doing this gives us access to object properties (eg channel id) that can be put in the command string
-            fmt_visa_cmd = visa_cmd
-            if hasattr(self, "query_params"):
-                fmt_visa_cmd = fmt_visa_cmd.format(**self.query_params)
-            response = self.visa_instr.query(f"{fmt_visa_cmd}?")
-            response = read_conv(response.strip())
-            return response
-
-        if not read_only:
-            def visa_setter(self: VisaDevice, value):
-                fmt_visa_cmd = visa_cmd
-                if hasattr(self, "query_params"):
-                    fmt_visa_cmd = fmt_visa_cmd.format(**self.query_params)
-                cmd = f"{fmt_visa_cmd} {write_conv(value)}"
-                self.visa_instr.write(cmd)
-        else:
-            visa_setter = None
-
-        prop = property(visa_getter, visa_setter)
-        return prop
-
-
-def enum_conv(e, allow_other_types=True):
-    if isinstance(e, Enum):
-        return e.value
-    elif allow_other_types:
-        return e
-    else:
-        raise ValueError(f"{e} is not an enum type")
-
-def str_conv(s):
-    return s.replace('"', '')
+    ## standard SCPI commands
+    clear_status_register = visa_command("*cls")
+    status_register = visa_property("*esr", dtype=EventStatusRegister, read_only=True)
```

### Comparing `pylabframe-0.0.1/pylabframe/hardware/drivers.py` & `pylabframe-0.0.2/pylabframe/hw/drivers/tekvisa.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 import numpy as np
-
-from . import device
 from enum import Enum
-from .device import enum_conv, str_conv
-import pylabframe.data
 
-# helper definition
-visa_property = device.VisaDevice.visa_property
+from pylabframe.hw import device, visadevice
+from pylabframe.hw.device import str_conv, SettingEnum, intbool_conv
+from pylabframe.hw.visadevice import visa_property, visa_command
+import pylabframe.data
 
 
-class TektronixScope(device.VisaDevice):
+class TektronixScope(visadevice.VisaDevice):
     NUM_CHANNELS = 2
 
-    class RunModes(Enum):
+    class RunModes(SettingEnum):
         CONTINUOUS = "RUNST"
         SINGLE = "SEQ"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # initialize channels
         self.channels: list[TektronixScope.Channel] = [self.Channel(i+1, self) for i in range(self.NUM_CHANNELS)]
 
     # global scpi properties
-    record_length = visa_property("horizontal:recordlength", read_conv=int, write_conv=int)
-    run_mode = visa_property("acquire:stopafter", read_conv=RunModes, write_conv=enum_conv)
-    run_state = visa_property("acquire:state", read_conv=bool, write_conv=int)
-    x_scale = visa_property("horizontal:scale", read_conv=float, write_conv=float)
+    trace_points = visa_property("horizontal:recordlength", rw_conv=int)
+    run_mode = visa_property("acquire:stopafter", read_conv=RunModes)
+    running = visa_property("acquire:state", read_conv=intbool_conv, write_conv=int)
+    x_scale = visa_property("horizontal:scale", rw_conv=float)
+
+    def trigger_single_acquisition(self):
+        # (I think there are better/more specific commands to do this, but it works)
+        self.instr.write("fpanel:press single")
+        self.instr.write("fpanel:press forcetrig")
 
     # waveform transfer properties
     waveform_points = visa_property("wfmoutpre:nr_pt", read_only=True, read_conv=int)
     waveform_y_multiplier = visa_property("wfmoutpre:ymult", read_only=True, read_conv=float)
     waveform_y_offset_levels = visa_property("wfmoutpre:yoff", read_only=True, read_conv=float)
     waveform_y_zero = visa_property("wfmoutpre:yzero", read_only=True, read_conv=float)
     waveform_y_unit = visa_property("wfmoutpre:yunit", read_only=True, read_conv=str_conv)
 
     waveform_x_increment = visa_property("wfmoutpre:xincr", read_only=True, read_conv=float)
     waveform_x_zero = visa_property("wfmoutpre:xzero", read_only=True, read_conv=float)
     waveform_x_unit = visa_property("wfmoutpre:xunit", read_only=True, read_conv=str_conv)
 
     def initialize_waveform_transfer(self, channel_id, start=1, stop=None):
-        self.visa_instr.write(f"data:source ch{channel_id}")
-        self.visa_instr.write(f"data:start {start}")
+        self.instr.write(f"data:source ch{channel_id}")
+        self.instr.write(f"data:start {start}")
         if stop is None:
             # default to full waveform
-            stop = self.record_length
-        self.visa_instr.write(f"data:stop {stop}")
-        self.visa_instr.write("data:encdg fast")
-        self.visa_instr.write("data:width 2")
-        self.visa_instr.write("header 0")
+            stop = self.trace_points
+        self.instr.write(f"data:stop {stop}")
+        self.instr.write("data:encdg fast")
+        self.instr.write("data:width 2")
+        self.instr.write("header 0")
 
     def do_waveform_transfer(self):
-        wfm_raw = self.visa_instr.query_binary_values("curve?", datatype='h', is_big_endian=True, container=np.array)
-        wfm_converted = (wfm_raw * self.waveform_y_multiplier) + self.waveform_y_zero
+        wfm_raw = self.instr.query_binary_values("curve?", datatype='h', is_big_endian=True, container=np.array)
+        wfm_converted = ((wfm_raw - self.waveform_y_offset_levels) * self.waveform_y_multiplier) + self.waveform_y_zero
         time_axis = (np.arange(self.waveform_points) * self.waveform_x_increment) + self.waveform_x_zero
 
         metadata = {
             "x_unit": self.waveform_x_unit,
             "x_label": f"time",
             "y_unit": self.waveform_y_unit,
             "y_label": f"signal",
         }
         data_obj = pylabframe.data.NumericalData(wfm_converted, x_axis=time_axis, metadata=metadata)
         return data_obj
 
-    def get_channel_waveform(self, channel_id, start=1, stop=None):
+    def acquire_channel_waveform(self, channel_id, start=1, stop=None):
         self.initialize_waveform_transfer(channel_id, start=start, stop=stop)
         wfm = self.do_waveform_transfer()
         return wfm
 
     # channel properties
     class Channel:
         def __init__(self, channel, device):
             self.channel_id = channel
             self.query_params = {'channel_id':  channel}
             self.device: "TektronixScope" = device
-            self.visa_instr = self.device.visa_instr
+            self.instr = self.device.instr
 
-        y_scale = visa_property("ch{channel_id}:scale", read_conv=float, write_conv=float)
-        offset = visa_property("ch{channel_id}:offset", read_conv=float, write_conv=float)
-        termination = visa_property("ch{channel_id}:termination", read_conv=float, write_conv=float)
-        inverted = visa_property("ch{channel_id}:invert", read_conv=bool, write_conv=int)
+        y_scale = visa_property("ch{channel_id}:scale", rw_conv=float)
+        offset = visa_property("ch{channel_id}:offset", rw_conv=float)
+        termination = visa_property("ch{channel_id}:termination", rw_conv=float)
+        inverted = visa_property("ch{channel_id}:invert", read_conv=intbool_conv, write_conv=int)
 
         mean = visa_property("measu:meas{channel_id}:mean", read_only=True, read_conv=float)
 
-        def get_waveform(self, start=1, stop=None):
-            return self.device.get_channel_waveform(self.channel_id, start=start, stop=stop)
-
+        def acquire_waveform(self, start=1, stop=None):
+            return self.device.acquire_channel_waveform(self.channel_id, start=start, stop=stop)
```

### Comparing `pylabframe-0.0.1/.gitignore` & `pylabframe-0.0.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -154,7 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
+
+test/internal/
```

### Comparing `pylabframe-0.0.1/LICENSE` & `pylabframe-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylabframe-0.0.1/pyproject.toml` & `pylabframe-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pylabframe"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jesse Slim", email="jesse.j.slim@gmail.com" },
 ]
 description = "Python package to interact with laboratory devices and measurement data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
+    "tomli; python_version < '3.11'",
+    "matplotlib",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/JesseSlim/pylabframe"
-"Bug Tracker" = "https://github.com/JesseSlim/pylabframe/issues"
+"Bug Tracker" = "https://github.com/JesseSlim/pylabframe/issues"
```

### Comparing `pylabframe-0.0.1/PKG-INFO` & `pylabframe-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pylabframe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package to interact with laboratory devices and measurement data
 Project-URL: Homepage, https://github.com/JesseSlim/pylabframe
 Project-URL: Bug Tracker, https://github.com/JesseSlim/pylabframe/issues
 Author-email: Jesse Slim <jesse.j.slim@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: tomli; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # pyLabFrame
 
 pyLabFrame is a Python package to interact with laboratory devices and measurement data.
```

