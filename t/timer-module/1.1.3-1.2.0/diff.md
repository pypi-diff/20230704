# Comparing `tmp/timer-module-1.1.3.tar.gz` & `tmp/timer-module-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timer-module-1.1.3.tar", last modified: Sun Jul  2 20:42:22 2023, max compression
+gzip compressed data, was "timer-module-1.2.0.tar", last modified: Mon Jul  3 22:10:19 2023, max compression
```

## Comparing `timer-module-1.1.3.tar` & `timer-module-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 20:42:22.233569 timer-module-1.1.3/
--rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     2428 2023-07-02 20:42:22.233569 timer-module-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 20:42:22.234570 timer-module-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-07-02 20:41:15.000000 timer-module-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 20:42:22.211543 timer-module-1.1.3/timer_module/
--rw-rw-rw-   0        0        0      127 2023-05-20 04:38:26.000000 timer-module-1.1.3/timer_module/__init__.py
--rw-rw-rw-   0        0        0     6019 2023-07-02 20:34:07.000000 timer-module-1.1.3/timer_module/metrics.py
--rw-rw-rw-   0        0        0     7032 2023-07-02 20:35:17.000000 timer-module-1.1.3/timer_module/profiler.py
--rw-rw-rw-   0        0        0     1358 2023-06-29 22:39:56.000000 timer-module-1.1.3/timer_module/terminal.py
--rw-rw-rw-   0        0        0     1459 2023-05-20 04:38:26.000000 timer-module-1.1.3/timer_module/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-02 20:42:22.232569 timer-module-1.1.3/timer_module.egg-info/
--rw-rw-rw-   0        0        0     2428 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 22:10:19.649897 timer-module-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2428 2023-07-03 22:10:19.648897 timer-module-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 22:10:19.649897 timer-module-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-07-03 22:04:41.000000 timer-module-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 22:10:19.624860 timer-module-1.2.0/timer_module/
+-rw-rw-rw-   0        0        0      120 2023-07-02 20:41:30.000000 timer-module-1.2.0/timer_module/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-07-03 21:10:46.000000 timer-module-1.2.0/timer_module/hasher.py
+-rw-rw-rw-   0        0        0     3797 2023-07-03 22:06:14.000000 timer-module-1.2.0/timer_module/logger.py
+-rw-rw-rw-   0        0        0     6332 2023-07-03 21:14:38.000000 timer-module-1.2.0/timer_module/metrics.py
+-rw-rw-rw-   0        0        0     7070 2023-07-03 22:07:45.000000 timer-module-1.2.0/timer_module/profiler.py
+-rw-rw-rw-   0        0        0     1296 2023-07-02 20:41:30.000000 timer-module-1.2.0/timer_module/terminal.py
+-rw-rw-rw-   0        0        0     1405 2023-07-02 20:41:30.000000 timer-module-1.2.0/timer_module/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-03 22:10:19.647897 timer-module-1.2.0/timer_module.egg-info/
+-rw-rw-rw-   0        0        0     2428 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 22:10:19.000000 timer-module-1.2.0/timer_module.egg-info/top_level.txt
```

### Comparing `timer-module-1.1.3/LICENSE` & `timer-module-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.3/PKG-INFO` & `timer-module-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.1.3
+Version: 1.2.0
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `timer-module-1.1.3/README.md` & `timer-module-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.3/setup.py` & `timer-module-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
-VERSION = "1.1.3"
+VERSION = "1.2.0"
 DESCRIPTION = "Timer Module with performance profiling features"
 
 root = Path(__file__).parent
 long_description = (root / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="timer-module",
```

### Comparing `timer-module-1.1.3/timer_module/metrics.py` & `timer-module-1.2.0/timer_module/metrics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,172 +1,187 @@
-from .terminal import Terminal
-from .terminal import ANSICode, GreenANSI, YellowANSI, WhiteANSI, CyanANSI
-
-
-class TimeFormatterNs:
-    def __init__(self, nanos: float):
-        self.nanos = nanos
-
-    def format_seconds(self) -> str:
-        secs = self.nanos / 1e9
-        return f"{secs:.2f}s"
-
-    def format_milliseconds(self) -> str:
-        millis = self.nanos / 1e6
-        return f"{millis:.2f}ms"
-
-    def format_microseconds(self) -> str:
-        micros = self.nanos / 1e3
-        return f"{micros:.2f}μs"
-
-    def format_nanoseconds(self) -> str:
-        return f"{self.nanos:.2f}ns"
-
-    def auto_format(self) -> str:
-        nanos = self.nanos
-        if nanos >= 1e9:
-            return self.format_seconds()
-
-        elif nanos >= 1e6:
-            return self.format_milliseconds()
-
-        elif nanos >= 1e3:
-            return self.format_microseconds()
-
-        return self.format_nanoseconds()
-
-
-class CallableMetrics:
-    __slots__ = ("name", "module", "call_hash", "ncalls", "time_ns")
-
-    def __init__(
-        self,
-        name: str,
-        module: str,
-        call_hash: int,
-        ncalls: int,
-        time_ns: float,
-    ):
-        self.name = name
-        self.module = module
-        self.call_hash = call_hash
-        self.ncalls = ncalls
-        self.time_ns = time_ns
-
-    def __hash__(self) -> int:
-        return self.call_hash
-
-    def clone_and_reset(self) -> "CallableMetrics":
-        call_metrics = CallableMetrics(
-            name=self.name,
-            module=self.module,
-            call_hash=self.call_hash,
-            ncalls=0,
-            time_ns=0.0,
-        )
-        return call_metrics
-
-    def get_percall_time(self) -> float:
-        if self.ncalls > 0:
-            percall_time_ns = self.time_ns / self.ncalls
-            return percall_time_ns
-        return 0.0
-
-
-class ProfileMetricsReport:
-    def __init__(self, realtime: bool = False):
-        self.realtime = realtime
-        self.terminal = Terminal()
-        self.header_color = self.get_header_color()
-        self.call_color = self.get_call_color()
-        self.total_time_color = self.get_total_time_color()
-
-    def get_header_color(self) -> ANSICode:
-        if self.realtime:
-            return YellowANSI()
-        return GreenANSI()
-
-    def get_call_color(self) -> ANSICode:
-        if self.realtime:
-            return CyanANSI()
-        return WhiteANSI()
-
-    def get_total_time_color(self) -> ANSICode:
-        if self.realtime:
-            return YellowANSI()
-        return GreenANSI()
-
-    def get_relative_percentage(self, pcall_ns: float, call_ns: float) -> float:
-        percentage = 0.0
-        if pcall_ns > 0.0 and call_ns > 0.0:
-            percentage = (call_ns / pcall_ns) * 100
-        return percentage
-
-    def write_primary_call_header(self, call_metrics: CallableMetrics):
-        pcall_name = call_metrics.name
-        profile_header = "█ PROFILE: {} █"
-        profile_header = profile_header.format(pcall_name)
-        separator = "=" * len(profile_header)
-        string = "\n{}\n{}"
-        string = string.format(profile_header, separator)
-        self.terminal.set_ansi_color(self.header_color)
-        self.terminal.write(string)
-
-    def write_primary_call_report(self, pcall_metrics: CallableMetrics):
-        pcall_time_ns = pcall_metrics.time_ns
-        pcall_ncalls = pcall_metrics.ncalls
-        percall_time_ns = pcall_metrics.get_percall_time()
-
-        pcall_time = TimeFormatterNs(pcall_time_ns).auto_format()
-        percall_time = TimeFormatterNs(percall_time_ns).auto_format()
-        string = "Profile Time: [{}]\nNCalls: [{}] — PerCall: [{}]\n——————\n"
-        string = string.format(pcall_time, pcall_ncalls, percall_time)
-        self.terminal.set_ansi_color(self.call_color)
-        self.terminal.write(string)
-
-    def write_call_report(self, call_metrics: CallableMetrics, pcall_time: float):
-        call_name = call_metrics.name
-        call_time_ns = call_metrics.time_ns
-        call_ncalls = call_metrics.ncalls
-        percall_time_ns = call_metrics.get_percall_time()
-
-        prc = self.get_relative_percentage(pcall_time, call_time_ns)
-        call_time = TimeFormatterNs(call_time_ns).auto_format()
-        percall_time = TimeFormatterNs(percall_time_ns).auto_format()
-
-        string = "Name: {}\nTime: [{}] — T%: {:.2f}%\nNCalls: [{}] — PerCall: [{}]\n——"
-        string = string.format(call_name, call_time, prc, call_ncalls, percall_time)
-        self.terminal.set_ansi_color(self.call_color)
-        self.terminal.write(string)
-
-    def get_total_time(
-        self,
-        callable_refs: dict[int, CallableMetrics],
-        timing_refs: dict[int, dict[int, CallableMetrics]],
-    ):
-        total_time = 0.0
-        for pcall_hash, _ in timing_refs.items():
-            total_time += callable_refs[pcall_hash].time_ns
-        return total_time
-
-    def write_report(
-        self,
-        callable_refs: dict[int, CallableMetrics],
-        timing_refs: dict[int, dict[int, CallableMetrics]],
-    ):
-        for pcall_hash, subcalls in timing_refs.items():
-            pcall_metrics = callable_refs[pcall_hash]
-            self.write_primary_call_header(pcall_metrics)
-            pcall_time = pcall_metrics.time_ns
-            for _, subcall_metrics in subcalls.items():
-                if subcall_metrics == pcall_metrics:
-                    continue
-                self.write_call_report(subcall_metrics, pcall_time)
-            self.write_primary_call_report(pcall_metrics)
-
-        total_time_ns = self.get_total_time(callable_refs, timing_refs)
-        total_time = TimeFormatterNs(total_time_ns).auto_format()
-
-        string = "――― Total Time: [{}] ―――\n\n\n"
-        string = string.format(f"{total_time}")
-        self.terminal.set_ansi_color(self.total_time_color)
-        self.terminal.write(string)
+from copy import copy
+
+from .hasher import Hasher
+from .terminal import Terminal
+from .terminal import ANSICode, GreenANSI, YellowANSI, WhiteANSI, CyanANSI
+
+
+class TimeFormatterNs:
+    def __init__(self, nanos: float):
+        self.nanos = nanos
+
+    def format_seconds(self) -> str:
+        secs = self.nanos / 1e9
+        return f"{secs:.2f}s"
+
+    def format_milliseconds(self) -> str:
+        millis = self.nanos / 1e6
+        return f"{millis:.2f}ms"
+
+    def format_microseconds(self) -> str:
+        micros = self.nanos / 1e3
+        return f"{micros:.2f}μs"
+
+    def format_nanoseconds(self) -> str:
+        return f"{self.nanos:.2f}ns"
+
+    def auto_format(self) -> str:
+        nanos = self.nanos
+        if nanos >= 1e9:
+            return self.format_seconds()
+
+        elif nanos >= 1e6:
+            return self.format_milliseconds()
+
+        elif nanos >= 1e3:
+            return self.format_microseconds()
+
+        return self.format_nanoseconds()
+
+
+class CallableMetrics:
+    __slots__ = ("name", "module", "suffix", "call_hash", "ncalls", "time_ns")
+
+    def __init__(
+        self,
+        name: str,
+        module: str,
+        suffix: str,
+        ncalls: int,
+        time_ns: float,
+    ):
+        self.name = name
+        self.module = module
+        self.suffix = suffix
+        self.ncalls = ncalls
+        self.time_ns = time_ns
+        self.call_hash = self.get_hash()
+
+    def __hash__(self) -> int:
+        return self.call_hash
+
+    def get_hash(self) -> int:
+        call_identifier = self.get_call_identifier()
+        return Hasher(call_identifier).hash_sha1()
+
+    def get_call_identifier(self) -> str:
+        call_identifier = f"{self.module}.{self.name}"
+        return call_identifier
+
+    def get_percall_time(self) -> float:
+        if self.ncalls > 0:
+            percall_time_ns = self.time_ns / self.ncalls
+            return percall_time_ns
+        return 0.0
+
+    def fresh_copy(self) -> "CallableMetrics":
+        call_metrics = copy(self)
+        call_metrics.ncalls = 0
+        call_metrics.time_ns = 0.0
+        return call_metrics
+
+
+class ProfileMetricsReport:
+    def __init__(self, realtime: bool = False):
+        self.realtime = realtime
+        self.terminal = Terminal()
+        self.header_color = self.get_header_color()
+        self.call_color = self.get_call_color()
+        self.total_time_color = self.get_total_time_color()
+
+    def get_header_color(self) -> ANSICode:
+        if self.realtime:
+            return YellowANSI()
+        return GreenANSI()
+
+    def get_call_color(self) -> ANSICode:
+        if self.realtime:
+            return CyanANSI()
+        return WhiteANSI()
+
+    def get_total_time_color(self) -> ANSICode:
+        if self.realtime:
+            return YellowANSI()
+        return GreenANSI()
+
+    def get_relative_percentage(self, pcall_ns: float, call_ns: float) -> float:
+        percentage = 0.0
+        if pcall_ns > 0.0 and call_ns > 0.0:
+            percentage = (call_ns / pcall_ns) * 100
+        return percentage
+
+    def write_primary_call_header(self, call_metrics: CallableMetrics):
+        pcall_name = call_metrics.name
+        pcall_suffix = call_metrics.suffix
+        if pcall_suffix:
+            pcall_name += f" ({pcall_suffix})"
+
+        profile_header = "█ PROFILE: {} █"
+        profile_header = profile_header.format(pcall_name)
+        separator = "=" * len(profile_header)
+        string = "\n{}\n{}"
+        string = string.format(profile_header, separator)
+        self.terminal.set_ansi_color(self.header_color)
+        self.terminal.write(string)
+
+    def write_primary_call_report(self, pcall_metrics: CallableMetrics):
+        pcall_time_ns = pcall_metrics.time_ns
+        pcall_ncalls = pcall_metrics.ncalls
+        percall_time_ns = pcall_metrics.get_percall_time()
+
+        pcall_time = TimeFormatterNs(pcall_time_ns).auto_format()
+        percall_time = TimeFormatterNs(percall_time_ns).auto_format()
+        string = "Profile Time: [{}]\nNCalls: [{}] — PerCall: [{}]\n——————\n"
+        string = string.format(pcall_time, pcall_ncalls, percall_time)
+        self.terminal.set_ansi_color(self.call_color)
+        self.terminal.write(string)
+
+    def write_call_report(self, call_metrics: CallableMetrics, pcall_time: float):
+        call_name = call_metrics.name
+        call_suffix = call_metrics.suffix
+        if call_suffix:
+            call_name += f" ({call_suffix})"
+        call_time_ns = call_metrics.time_ns
+        call_ncalls = call_metrics.ncalls
+        percall_time_ns = call_metrics.get_percall_time()
+
+        prc = self.get_relative_percentage(pcall_time, call_time_ns)
+        call_time = TimeFormatterNs(call_time_ns).auto_format()
+        percall_time = TimeFormatterNs(percall_time_ns).auto_format()
+
+        string = "Name: {}\nTime: [{}] — T%: {:.2f}%\nNCalls: [{}] — PerCall: [{}]\n——"
+        string = string.format(call_name, call_time, prc, call_ncalls, percall_time)
+        self.terminal.set_ansi_color(self.call_color)
+        self.terminal.write(string)
+
+    def get_total_time(
+        self,
+        callable_refs: dict[int, CallableMetrics],
+        timing_refs: dict[int, dict[int, CallableMetrics]],
+    ):
+        total_time = 0.0
+        for pcall_hash, _ in timing_refs.items():
+            total_time += callable_refs[pcall_hash].time_ns
+        return total_time
+
+    def write_report(
+        self,
+        callable_refs: dict[int, CallableMetrics],
+        timing_refs: dict[int, dict[int, CallableMetrics]],
+    ):
+        for pcall_hash, subcalls in timing_refs.items():
+            pcall_metrics = callable_refs[pcall_hash]
+            self.write_primary_call_header(pcall_metrics)
+            pcall_time = pcall_metrics.time_ns
+            for _, subcall_metrics in subcalls.items():
+                if subcall_metrics == pcall_metrics:
+                    continue
+                self.write_call_report(subcall_metrics, pcall_time)
+            self.write_primary_call_report(pcall_metrics)
+
+        total_time_ns = self.get_total_time(callable_refs, timing_refs)
+        total_time = TimeFormatterNs(total_time_ns).auto_format()
+
+        string = "――― Total Time: [{}] ―――\n\n\n"
+        string = string.format(f"{total_time}")
+        self.terminal.set_ansi_color(self.total_time_color)
+        self.terminal.write(string)
```

### Comparing `timer-module-1.1.3/timer_module/profiler.py` & `timer-module-1.2.0/timer_module/profiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,182 +1,180 @@
-import hashlib
-
-from time import perf_counter_ns
-from functools import lru_cache
-from typing import Callable, Awaitable
-from typing import Union, Optional, Type, TypeVar, ParamSpec
-from inspect import getmembers, ismethod, isfunction, iscoroutinefunction
-
-from .metrics import CallableMetrics, ProfileMetricsReport
-
-P = ParamSpec("P")
-RT = TypeVar("RT")
-CT = TypeVar("CT")
-
-
-class TimeProfilerBase:
-    def __init__(self, realtime: bool = False) -> None:
-        self._realtime: bool = realtime
-
-    def __new__(cls, *args, **kwargs):
-        if not hasattr(cls, "instance") or not isinstance(cls.instance, cls):
-            cls.instance = super(TimeProfilerBase, cls).__new__(cls)
-            cls._callable_refs: dict[int, CallableMetrics] = {}
-            cls._timing_refs: dict[int, dict[int, CallableMetrics]] = {}
-            cls._pcall_hash: Optional[int] = None
-        return cls.instance
-
-    def __del__(self) -> None:
-        self._print_report()
-
-    def _print_report(self, realtime: bool = False):
-        metrics_report = ProfileMetricsReport(realtime)
-        callable_refs = self._callable_refs
-        timing_refs = self._timing_refs
-        metrics_report.write_report(callable_refs, timing_refs)
-
-    @staticmethod
-    def _set_attribute(instance: CT, name: str, method: Callable) -> CT:
-        try:
-            instance.__setattr__(name, method)
-        except AttributeError:
-            print(f"Class Method ({name}) is read-only and cannot be timed.")
-        return instance
-
-    def _append_metrics(self, call_hash: int, time_ns: float) -> None:
-        callable_refs = self._callable_refs
-        pcall_hash = self._pcall_hash
-
-        if pcall_hash is not None:
-            if call_hash == pcall_hash:
-                call_metrics = callable_refs[call_hash]
-                call_metrics.time_ns += time_ns
-                call_metrics.ncalls += 1
-                self._pcall_hash = None
-
-                if self._realtime:
-                    self._print_report(realtime=True)
-            else:
-                call_metrics = self._timing_refs[pcall_hash][call_hash]
-                call_metrics.time_ns += time_ns
-                call_metrics.ncalls += 1
-
-    @staticmethod
-    def _create_callable_metrics(call: Callable, call_hash: int) -> CallableMetrics:
-        name = call.__qualname__
-        module = call.__module__
-        if isinstance(call, type):
-            name += " (Initialization)"
-
-        call_metrics = CallableMetrics(
-            name=name,
-            module=module,
-            call_hash=call_hash,
-            ncalls=0,
-            time_ns=0.0,
-        )
-        return call_metrics
-
-    @staticmethod
-    @lru_cache(maxsize=None)
-    def hash_type_id(type_id: Type) -> int:
-        hasher = hashlib.sha1()
-        hasher.update(str(type_id).encode())
-        hash_result = int(hasher.hexdigest(), 16)
-        return hash_result
-
-    def _set_pcall_hash(self, call_hash: int):
-        pcall_hash = self._pcall_hash
-
-        if pcall_hash is None:
-            pcall_hash = call_hash
-            self._pcall_hash = pcall_hash
-            if pcall_hash not in self._timing_refs:
-                self._timing_refs[pcall_hash] = {}
-            return
-
-        pcall_timing = self._timing_refs[pcall_hash]
-        if call_hash not in pcall_timing:
-            call_metrics = self._callable_refs[call_hash]
-            new_metrics = call_metrics.clone_and_reset()
-            pcall_timing.update({call_hash: new_metrics})
-
-    def _add_call_ref(self, call: Callable) -> int:
-        call_hash = self.hash_type_id(call)
-        call_metrics = self._create_callable_metrics(call, call_hash)
-        self._callable_refs[call_hash] = call_metrics
-        return call_hash
-
-    def _get_method_wrapper(
-        self, method: Callable[P, RT], method_hash: int
-    ) -> Union[Callable[P, RT], Callable[P, Awaitable[RT]]]:
-        is_coroutine = iscoroutinefunction(method)
-        if is_coroutine:
-            return self._async_function_wrapper(method, method_hash)
-        return self._function_wrapper(method, method_hash)
-
-    def _class_wrapper(
-        self, cls_obj: Type[Callable[P, CT]], pcall_hash: int
-    ) -> Type[CT]:
-        class ClassWrapper(cls_obj):  # type: ignore
-            def __init__(_self, *args: P.args, **kwargs: P.kwargs) -> None:
-                self._set_pcall_hash(pcall_hash)
-                start_time = perf_counter_ns()
-                super().__init__(*args, **kwargs)
-                elapsed_time = perf_counter_ns() - start_time
-                self._append_metrics(pcall_hash, elapsed_time)
-
-            def __new__(_cls: cls_obj, *args: P.args, **kwargs: P.kwargs) -> CT:
-                cls_instance = super().__new__(_cls)
-                methods = getmembers(cls_instance, predicate=ismethod)
-                functions = getmembers(cls_instance, predicate=isfunction)
-                members = methods + functions
-                for name, member in members:
-                    member_ref = self._add_call_ref(member)
-                    member = self._get_method_wrapper(member, member_ref)
-                    cls_instance = self._set_attribute(cls_instance, name, member)
-
-                return cls_instance
-
-        return ClassWrapper
-
-    def _function_wrapper(
-        self, func: Callable[P, RT], pcall_hash: int
-    ) -> Callable[P, RT]:
-        def function_wrapper(*args: P.args, **kwargs: P.kwargs) -> RT:
-            self._set_pcall_hash(pcall_hash)
-            start_time = perf_counter_ns()
-            result = func(*args, **kwargs)
-            elapsed_time = perf_counter_ns() - start_time
-            self._append_metrics(pcall_hash, elapsed_time)
-            return result
-
-        return function_wrapper
-
-    def _async_function_wrapper(
-        self, func: Callable[P, Awaitable[RT]], pcall_hash: int
-    ) -> Callable[P, Awaitable[RT]]:
-        async def function_wrapper(*args: P.args, **kwargs: P.kwargs) -> RT:
-            self._set_pcall_hash(pcall_hash)
-            start_time = perf_counter_ns()
-            result = await func(*args, **kwargs)
-            elapsed_time = perf_counter_ns() - start_time
-            self._append_metrics(pcall_hash, elapsed_time)
-            return result
-
-        return function_wrapper
-
-
-class TimeProfiler(TimeProfilerBase):
-    def class_profiler(self, cls_obj: Type[Callable[P, CT]]) -> Type[CT]:
-        main_ref = self._add_call_ref(cls_obj)
-        return self._class_wrapper(cls_obj, main_ref)
-
-    def function_profiler(self, func: Callable[P, RT]) -> Callable[P, RT]:
-        main_ref = self._add_call_ref(func)
-        return self._function_wrapper(func, main_ref)
-
-    def async_function_profiler(
-        self, func: Callable[P, Awaitable[RT]]
-    ) -> Callable[P, Awaitable[RT]]:
-        main_ref = self._add_call_ref(func)
-        return self._async_function_wrapper(func, main_ref)
+from time import perf_counter_ns
+from typing import Callable, Awaitable, Self
+from typing import Union, Optional, Type, TypeVar, ParamSpec
+from inspect import getmembers, ismethod, isfunction, iscoroutinefunction
+
+from .metrics import CallableMetrics, ProfileMetricsReport
+from .logger import TimeProfilerLogger
+
+P = ParamSpec("P")
+RT = TypeVar("RT")
+CT = TypeVar("CT")
+
+
+class TimeProfilerBase:
+    def __init__(self, realtime: bool = False, verbose: bool = False) -> None:
+        self._realtime: bool = realtime
+        self._verbose: bool = verbose
+        self._profiler_logger: TimeProfilerLogger = TimeProfilerLogger()
+
+    def __new__(cls, *args, **kwargs) -> Self:
+        if not hasattr(cls, "instance") or not isinstance(cls.instance, cls):
+            cls.instance = super(TimeProfilerBase, cls).__new__(cls)
+            cls._callable_refs: dict[int, CallableMetrics] = {}
+            cls._timing_refs: dict[int, dict[int, CallableMetrics]] = {}
+            cls._pcall_hash: Optional[int] = None
+        return cls.instance
+
+    def __del__(self) -> None:
+        self._print_report()
+
+    def _print_report(self, realtime: bool = False):
+        metrics_report = ProfileMetricsReport(realtime)
+        callable_refs = self._callable_refs
+        timing_refs = self._timing_refs
+        metrics_report.write_report(callable_refs, timing_refs)
+
+    @staticmethod
+    def _set_attribute(instance: CT, name: str, method: Callable) -> CT:
+        try:
+            instance.__setattr__(name, method)
+        except AttributeError:
+            print(f"Class Method ({name}) is read-only and cannot be timed.")
+        return instance
+
+    def _append_metrics(self, call_hash: int, time_ns: float) -> None:
+        pcall_hash = self._pcall_hash
+
+        if pcall_hash is not None:
+            if call_hash == pcall_hash:
+                call_metrics = self._callable_refs[call_hash]
+                call_metrics.time_ns += time_ns
+                call_metrics.ncalls += 1
+                self._pcall_hash = None
+
+                if self._realtime:
+                    self._print_report(realtime=True)
+            else:
+                call_metrics = self._timing_refs[pcall_hash][call_hash]
+                call_metrics.time_ns += time_ns
+                call_metrics.ncalls += 1
+                if self._verbose:
+                    self._profiler_logger.subcall_event(call_metrics)
+
+    @staticmethod
+    def _create_callable_metrics(call: Callable, suffix: str) -> CallableMetrics:
+        name = call.__qualname__
+        module = call.__module__
+
+        call_metrics = CallableMetrics(
+            name=name,
+            module=module,
+            suffix=suffix,
+            ncalls=0,
+            time_ns=0.0,
+        )
+        return call_metrics
+
+    def _set_pcall_hash(self, call_hash: int):
+        pcall_hash = self._pcall_hash
+
+        if pcall_hash is None:
+            pcall_hash = call_hash
+            self._pcall_hash = pcall_hash
+            if pcall_hash not in self._timing_refs:
+                self._timing_refs[pcall_hash] = {}
+
+            call_metrics = self._callable_refs[pcall_hash]
+            if self._verbose:
+                self._profiler_logger.set_primary_call(call_metrics)
+            return
+
+        pcall_timing = self._timing_refs[pcall_hash]
+        if call_hash not in pcall_timing:
+            call_metrics = self._callable_refs[call_hash]
+            new_metrics = call_metrics.fresh_copy()
+            pcall_timing.update({call_hash: new_metrics})
+
+    def _add_call_ref(self, call: Callable, suffix: str = "") -> int:
+        call_metrics = self._create_callable_metrics(call, suffix)
+        call_hash = call_metrics.call_hash
+        self._callable_refs[call_hash] = call_metrics
+        if self._verbose:
+            self._profiler_logger.add_call_reference(call_metrics)
+        return call_hash
+
+    def _get_method_wrapper(
+        self, method: Callable[P, RT], method_hash: int
+    ) -> Union[Callable[P, RT], Callable[P, Awaitable[RT]]]:
+        is_coroutine = iscoroutinefunction(method)
+        if is_coroutine:
+            return self._async_function_wrapper(method, method_hash)
+        return self._function_wrapper(method, method_hash)
+
+    def _class_wrapper(
+        self, cls_obj: Type[Callable[P, CT]], pcall_hash: int
+    ) -> Type[CT]:
+        class ClassWrapper(cls_obj):  # type: ignore
+            def __init__(_self, *args: P.args, **kwargs: P.kwargs) -> None:
+                self._set_pcall_hash(pcall_hash)
+                start_time = perf_counter_ns()
+                super().__init__(*args, **kwargs)
+                elapsed_time = perf_counter_ns() - start_time
+                self._append_metrics(pcall_hash, elapsed_time)
+
+            def __new__(_cls: cls_obj, *args: P.args, **kwargs: P.kwargs) -> CT:
+                cls_instance = super().__new__(_cls)
+                methods = getmembers(cls_instance, predicate=ismethod)
+                functions = getmembers(cls_instance, predicate=isfunction)
+                members = methods + functions
+                for name, member in members:
+                    if member.__module__ != __name__:
+                        member_ref = self._add_call_ref(member)
+                        member = self._get_method_wrapper(member, member_ref)
+                        cls_instance = self._set_attribute(cls_instance, name, member)
+
+                return cls_instance
+
+        return ClassWrapper
+
+    def _function_wrapper(
+        self, func: Callable[P, RT], pcall_hash: int
+    ) -> Callable[P, RT]:
+        def function_wrapper(*args: P.args, **kwargs: P.kwargs) -> RT:
+            self._set_pcall_hash(pcall_hash)
+            start_time = perf_counter_ns()
+            result = func(*args, **kwargs)
+            elapsed_time = perf_counter_ns() - start_time
+            self._append_metrics(pcall_hash, elapsed_time)
+            return result
+
+        return function_wrapper
+
+    def _async_function_wrapper(
+        self, func: Callable[P, Awaitable[RT]], pcall_hash: int
+    ) -> Callable[P, Awaitable[RT]]:
+        async def function_wrapper(*args: P.args, **kwargs: P.kwargs) -> RT:
+            self._set_pcall_hash(pcall_hash)
+            start_time = perf_counter_ns()
+            result = await func(*args, **kwargs)
+            elapsed_time = perf_counter_ns() - start_time
+            self._append_metrics(pcall_hash, elapsed_time)
+            return result
+
+        return function_wrapper
+
+
+class TimeProfiler(TimeProfilerBase):
+    def class_profiler(self, cls_obj: Type[Callable[P, CT]]) -> Type[CT]:
+        main_ref = self._add_call_ref(cls_obj, "Initialization")
+        return self._class_wrapper(cls_obj, main_ref)
+
+    def function_profiler(self, func: Callable[P, RT]) -> Callable[P, RT]:
+        main_ref = self._add_call_ref(func)
+        return self._function_wrapper(func, main_ref)
+
+    def async_function_profiler(
+        self, func: Callable[P, Awaitable[RT]]
+    ) -> Callable[P, Awaitable[RT]]:
+        main_ref = self._add_call_ref(func)
+        return self._async_function_wrapper(func, main_ref)
```

### Comparing `timer-module-1.1.3/timer_module.egg-info/PKG-INFO` & `timer-module-1.2.0/timer_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.1.3
+Version: 1.2.0
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

