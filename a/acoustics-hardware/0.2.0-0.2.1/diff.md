# Comparing `tmp/acoustics-hardware-0.2.0.tar.gz` & `tmp/acoustics-hardware-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acoustics-hardware-0.2.0.tar", last modified: Fri Jul 22 12:52:27 2022, max compression
+gzip compressed data, was "acoustics-hardware-0.2.1.tar", last modified: Tue Jul  4 08:04:08 2023, max compression
```

## Comparing `acoustics-hardware-0.2.0.tar` & `acoustics-hardware-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-07-22 12:52:27.051720 acoustics-hardware-0.2.0/
--rw-rw-rw-   0        0        0     1092 2022-03-28 14:01:16.000000 acoustics-hardware-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       15 2022-03-28 14:01:16.000000 acoustics-hardware-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      885 2022-07-22 12:52:27.050721 acoustics-hardware-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      511 2022-03-28 14:01:16.000000 acoustics-hardware-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-07-22 12:52:27.008909 acoustics-hardware-0.2.0/acoustics_hardware/
--rw-rw-rw-   0        0        0      299 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/__init__.py
--rw-rw-rw-   0        0        0    11035 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/_core.py
--rw-rw-rw-   0        0        0      353 2022-07-22 12:52:24.000000 acoustics-hardware-0.2.0/acoustics_hardware/_version.py
--rw-rw-rw-   0        0        0     9339 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/analysis.py
--rw-rw-rw-   0        0        0    10304 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/generators.py
--rw-rw-rw-   0        0        0    28913 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/interfaces.py
--rw-rw-rw-   0        0        0     6612 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/recorders.py
--rw-rw-rw-   0        0        0     7511 2022-04-01 07:52:43.000000 acoustics-hardware-0.2.0/acoustics_hardware/serial.py
--rw-rw-rw-   0        0        0     3379 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/signal_tools.py
--rw-rw-rw-   0        0        0     2609 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/timestamps.py
--rw-rw-rw-   0        0        0    10644 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/acoustics_hardware/triggers.py
-drwxrwxrwx   0        0        0        0 2022-07-22 12:52:27.045848 acoustics-hardware-0.2.0/acoustics_hardware.egg-info/
--rw-rw-rw-   0        0        0      885 2022-07-22 12:52:25.000000 acoustics-hardware-0.2.0/acoustics_hardware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2022-07-22 12:52:26.000000 acoustics-hardware-0.2.0/acoustics_hardware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-22 12:52:26.000000 acoustics-hardware-0.2.0/acoustics_hardware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2022-07-22 12:52:26.000000 acoustics-hardware-0.2.0/acoustics_hardware.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-07-22 12:52:26.000000 acoustics-hardware-0.2.0/acoustics_hardware.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-22 12:52:27.051720 acoustics-hardware-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1035 2022-07-22 12:43:54.000000 acoustics-hardware-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:04:08.388247 acoustics-hardware-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-04 08:04:08.388247 acoustics-hardware-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:04:08.388247 acoustics-hardware-0.2.1/acoustics_hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-04 08:04:08.000000 acoustics-hardware-0.2.1/acoustics_hardware/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28188 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/recorders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/signal_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/acoustics_hardware/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:04:08.388247 acoustics-hardware-0.2.1/acoustics_hardware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-04 08:04:08.000000 acoustics-hardware-0.2.1/acoustics_hardware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-04 08:04:08.000000 acoustics-hardware-0.2.1/acoustics_hardware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:04:08.000000 acoustics-hardware-0.2.1/acoustics_hardware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 08:04:08.000000 acoustics-hardware-0.2.1/acoustics_hardware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 08:04:08.000000 acoustics-hardware-0.2.1/acoustics_hardware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:04:08.388247 acoustics-hardware-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-04 08:03:55.000000 acoustics-hardware-0.2.1/setup.py
```

### Comparing `acoustics-hardware-0.2.0/LICENSE` & `acoustics-hardware-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 Carl Andersson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2018 Carl Andersson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `acoustics-hardware-0.2.0/PKG-INFO` & `acoustics-hardware-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1
-Name: acoustics-hardware
-Version: 0.2.0
-Summary: Controlling hardware used in acoustic measurement systems
-Home-page: https://github.com/AppliedAcousticsChalmers/acoustics-hardware
-Author: Carl Andersson
-Author-email: carl.andersson@chalmers.se
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-Acoustics Hardware
-==================
-
-This Python package provides a unified interface to serveral hardware platforms used in acoustic measurements, e.g. audio interfaces.
-The purpose of this package is twofold, both to enable cross-hardware interactions with a consistent interface, and to simplify scripting of advanced measurement setups.
-
-Documentation:
-    http://acoustics-hardware.readthedocs.io/
-Source code and issue tracker:
-    https://github.com/AppliedAcousticsChalmers/acoustics-hardware
-
+Metadata-Version: 2.1
+Name: acoustics-hardware
+Version: 0.2.1
+Summary: Controlling hardware used in acoustic measurement systems
+Home-page: https://github.com/AppliedAcousticsChalmers/acoustics-hardware
+Author: Carl Andersson
+Author-email: carl.andersson@chalmers.se
+License: MIT
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Acoustics Hardware
+==================
+
+This Python package provides a unified interface to serveral hardware platforms used in acoustic measurements, e.g. audio interfaces.
+The purpose of this package is twofold, both to enable cross-hardware interactions with a consistent interface, and to simplify scripting of advanced measurement setups.
+
+Documentation:
+    http://acoustics-hardware.readthedocs.io/
+Source code and issue tracker:
+    https://github.com/AppliedAcousticsChalmers/acoustics-hardware
```

### Comparing `acoustics-hardware-0.2.0/acoustics_hardware/_core.py` & `acoustics-hardware-0.2.1/acoustics_hardware/_core.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,320 +1,320 @@
-class Packet:
-    ...
-
-
-class Request(Packet):
-    ...
-
-
-class FrameRequest(Request):
-    def __init__(self, framesize):
-        self.framesize = framesize
-
-
-class Frame(Packet):
-    def __init__(self, frame):
-        self.frame = frame
-
-
-class LastFrame(Frame):
-    def __init__(self, frame, valid_samples):
-        self.frame = frame
-        self.valid_samples = valid_samples
-
-
-class TriggerFrame(Frame):
-    def __init__(self, frame, indices):
-        self.frame = frame
-        self.indices = indices
-
-
-class GateOpenFrame(Frame):
-    ...
-
-
-class GateCloseFrame(Frame):
-    ...
-
-
-class GateOpenCloseFrame(GateOpenFrame, GateCloseFrame):
-    ...
-
-
-class Pipeline:
-    def __init__(self, *nodes):
-        self.nodes = nodes
-        for node in self:
-            node._pipeline = self
-
-    def __str__(self):
-        return str([node.__class__.__name__ for node in self])
-
-    def __iter__(self):
-        return iter(self.nodes)
-
-    def to_dict(self):
-        from . import __version_info__
-        return dict(
-            package_version=__version_info__,
-            nodes=[node.to_dict() for node in self]
-        )
-
-    @property
-    def samplerate_decider(self):
-        for node in self:
-            if isinstance(node, SamplerateDecider):
-                return node
-
-    def run(self):
-        self.samplerate_decider.run()
-
-    def setup(self):
-        for node in self:
-            node.setup()
-
-    def reset(self):
-        for node in self:
-            node.reset()
-
-    def __or__(self, other):
-        if isinstance(other, Pipeline):
-            self.nodes[-1]._downstream = other.nodes[0]
-            other.nodes[0]._upstream = self.nodes[-1]
-            return Pipeline(*self.nodes, *other.nodes)
-        if isinstance(other, Node):
-            self.nodes[-1]._downstream = other
-            other._upstream = self.nodes[-1]
-            return Pipeline(*self.nodes, other)
-        return NotImplemented
-
-    def __ror__(self, other):
-        if isinstance(other, Pipeline):
-            self.nodes[0]._upstream = other.nodes[-1]
-            other.nodes[-1]._downstream = self.nodes[0]
-            return Pipeline(*other.nodes, *self.nodes)
-        if isinstance(other, Node):
-            self.nodes[0]._upstream = other
-            other._downstream = self.nodes[0]
-            return Pipeline(other, *self.nodes)
-        return NotImplemented
-
-
-class Node:
-    """Generic pipeline Node."""
-
-    def __init__(self):
-        self._pipeline = None
-        self._is_ready = False
-        self.__upstream = None
-        self.__downstream = None
-
-    def __or__(self, other):
-        if isinstance(other, Node):
-            self._downstream = other
-            other._upstream = self
-            return Pipeline(self, other)
-        return NotImplemented
-
-    def to_dict(self):
-        return dict(type=self.__class__.__name__)
-
-    def setup(self):
-        """Run setup for this Node."""
-        self._is_ready = True
-
-    def reset(self):
-        """Reset this Node."""
-        self._is_ready = False
-
-    def process(self, frame):
-        """Process one frame of data."""
-        return frame
-
-    @property
-    def _upstream(self):
-        """Wrap for the upstream node object."""
-        return self.__upstream
-
-    @_upstream.setter
-    def _upstream(self, node):
-        """Set the upstream node, running update code."""
-        self.__upstream = node
-        self._upstream_changed()
-
-    def _upstream_changed(self):
-        """Code to run when the upstream is changed."""
-        pass
-
-    @property
-    def _downstream(self):
-        """Wrap for the downstream node object."""
-        return self.__downstream
-
-    @_downstream.setter
-    def _downstream(self, node):
-        """Set the downstream node, running update code."""
-        self.__downstream = node
-        self._downstream_changed()
-
-    def _downstream_changed(self):
-        """Code to run when the downstream is changed."""
-        pass
-
-    def push(self, packet):
-        """Give a packet of data as the input to this node.
-
-        Processes a frame and passes it along down the pipeline.
-        """
-        if isinstance(packet, Frame):
-            packet = self.process(packet)
-
-        if packet is None:
-            return
-
-        if self._downstream is not None:
-            # We should push the frame down the pipeline, and return the final result.
-            return self._downstream.push(packet)
-        else:
-            # This is the end of the pipeline, so return the frame.
-            return packet
-
-    def request(self, packet):
-        """Request one frame of output from this object.
-
-        Requests a frame from the upstream or this node, process it,
-        then return the frame.
-        """
-        if self._upstream is not None:
-            # There's an upstream node, ask it to handle the packet first.
-            packet = self._upstream.request(packet)
-
-        if isinstance(packet, Request):
-            if isinstance(packet, FrameRequest):
-                # Either there's no upstream node, or it could not handle the request.
-                # Process this request here, then return the generated frame.
-                return self.process(packet)
-
-
-class SamplerateDecider(Node):
-    """Base class for nodes that have an externally defined samplerate.
-
-    Instances of this type will decide the samplerate for an entire pipeline,
-    by telling the SamplerateFollowers what samplerate they are operating at.
-    """
-    def __init__(self, samplerate, **kwargs):
-        super().__init__(**kwargs)
-        self.samplerate = samplerate
-
-    def to_dict(self):
-        return super().to_dict() | dict(
-            samplerate=self.samplerate,
-        )
-
-    def _upstream_changed(self):
-        super()._upstream_changed()
-        if isinstance(self._upstream, SamplerateFollower):
-            self._upstream._set_samplerate_direction('downstream')
-
-    def _downstream_changed(self):
-        super()._downstream_changed()
-        if isinstance(self._downstream, SamplerateFollower):
-            self._downstream._set_samplerate_direction('upstream')
-
-
-class SamplerateFollower(Node):
-    """Base class for nodes which have no external samplerate.
-
-    Instances of this class will look for a samplerate elsewhere in the pipeline.
-    This can be found either upstream when the instance is receiving data from
-    a SamperateDecider, or downstream when the instance will send data to a SamplerateDecider.
-    This is managed automatically when assembling the pipeline, no user interaction required.
-    """
-    def __init__(self, **kwargs):
-        self._samplerate_direction = None
-        super().__init__(**kwargs)
-
-    def _upstream_changed(self):
-        """Clear any stored samplerate direction since it might no longer be valid."""
-        super()._upstream_changed()
-        self._samplerate_direction = None
-
-    def _downstream_changed(self):
-        """Clear any stored samplerate direction since it might no longer be valid."""
-        super()._downstream_changed()
-        self._samplerate_direction = None
-
-    @property
-    def samplerate(self):
-        direction = self._get_samplerate_direction()
-        if direction == 'upstream':
-            samplerate = self._upstream.samplerate
-            try:
-                _, samplerate = samplerate
-            except TypeError:
-                pass
-            return samplerate
-        if direction == 'downstream':
-            samplerate = self._downstream.samplerate
-            try:
-                samplerate, _ = samplerate
-            except TypeError:
-                pass
-            return samplerate
-
-    def _get_samplerate_direction(self, direction='both'):
-        """Check if the samplerate can be found along the pipeline.
-
-        This will run along the pipeline and see if there's a SamplerateDecider
-        somewhere. If a direction is specified, it will only look in the given direction.
-        If found, all other SamplerateFollowers will be updated.
-
-        This is a complicated getter for the samplerate direction, parameterized with a
-        search direction to allow recursive searches. Additionally, when the value is found
-        it will be updated for all the relevant SamplerateFollowers.
-        """
-        if self._samplerate_direction is not None:
-            return self._samplerate_direction
-
-        if direction == 'both':
-            self._samplerate_direction = self._get_samplerate_direction('upstream') or self._get_samplerate_direction('downstream')
-            return self._samplerate_direction
-
-        if direction == 'upstream':
-            if isinstance(self._upstream, SamplerateDecider):
-                self._set_samplerate_direction('upstream')
-                return 'upstream'
-            elif isinstance(self._upstream, SamplerateFollower):
-                return self._upstream._get_samplerate_direction('upstream')
-        elif direction == 'downstream':
-            if isinstance(self._downstream, SamplerateDecider):
-                self._set_samplerate_direction('downstream')
-                return 'downstream'
-            elif isinstance(self._downstream, SamplerateFollower):
-                return self._downstream._get_samplerate_direction('downstream')
-        else:
-            raise ValueError(f"Search direction should be one of 'upstream' or 'downstream', got {direction}")
-        return False
-
-    def _set_samplerate_direction(self, direction):
-        """Update the pipeline samplerate direction.
-
-        This will go through the pipeline in one direction and update
-        the samplerate search direction.
-        It will always go through the pipeline in the opposite direction to the
-        search direction. I.e., if diretcion='upstream', this will go downstream
-        set all the samplerate directions to 'upstream', and vice versa.
-        """
-        if direction == 'upstream':
-            self._samplerate_direction = 'upstream'
-            if isinstance(self._downstream, SamplerateFollower):
-                if self._downstream._samplerate_direction is None:
-                    self._downstream._set_samplerate_direction('upstream')
-                elif self._downstream._samplerate_direction == 'downstream':
-                    raise ValueError('Conflicting pipeline samplerates!')
-        elif direction == 'downstream':
-            self._samplerate_direction = 'downstream'
-            if isinstance(self._upstream, SamplerateFollower):
-                if self._upstream._samplerate_direction is None:
-                    self._upstream._set_samplerate_direction('downstream')
-                elif self._upstream._samplerate_direction == 'upstream':
-                    raise ValueError('Conflicting pipeline samplerates!')
+class Packet:
+    ...
+
+
+class Request(Packet):
+    ...
+
+
+class FrameRequest(Request):
+    def __init__(self, framesize):
+        self.framesize = framesize
+
+
+class Frame(Packet):
+    def __init__(self, frame):
+        self.frame = frame
+
+
+class LastFrame(Frame):
+    def __init__(self, frame, valid_samples):
+        self.frame = frame
+        self.valid_samples = valid_samples
+
+
+class TriggerFrame(Frame):
+    def __init__(self, frame, indices):
+        self.frame = frame
+        self.indices = indices
+
+
+class GateOpenFrame(Frame):
+    ...
+
+
+class GateCloseFrame(Frame):
+    ...
+
+
+class GateOpenCloseFrame(GateOpenFrame, GateCloseFrame):
+    ...
+
+
+class Pipeline:
+    def __init__(self, *nodes):
+        self.nodes = nodes
+        for node in self:
+            node._pipeline = self
+
+    def __str__(self):
+        return str([node.__class__.__name__ for node in self])
+
+    def __iter__(self):
+        return iter(self.nodes)
+
+    def to_dict(self):
+        from . import __version_info__
+        return dict(
+            package_version=__version_info__,
+            nodes=[node.to_dict() for node in self]
+        )
+
+    @property
+    def samplerate_decider(self):
+        for node in self:
+            if isinstance(node, SamplerateDecider):
+                return node
+
+    def run(self):
+        self.samplerate_decider.run()
+
+    def setup(self):
+        for node in self:
+            node.setup()
+
+    def reset(self):
+        for node in self:
+            node.reset()
+
+    def __or__(self, other):
+        if isinstance(other, Pipeline):
+            self.nodes[-1]._downstream = other.nodes[0]
+            other.nodes[0]._upstream = self.nodes[-1]
+            return Pipeline(*self.nodes, *other.nodes)
+        if isinstance(other, Node):
+            self.nodes[-1]._downstream = other
+            other._upstream = self.nodes[-1]
+            return Pipeline(*self.nodes, other)
+        return NotImplemented
+
+    def __ror__(self, other):
+        if isinstance(other, Pipeline):
+            self.nodes[0]._upstream = other.nodes[-1]
+            other.nodes[-1]._downstream = self.nodes[0]
+            return Pipeline(*other.nodes, *self.nodes)
+        if isinstance(other, Node):
+            self.nodes[0]._upstream = other
+            other._downstream = self.nodes[0]
+            return Pipeline(other, *self.nodes)
+        return NotImplemented
+
+
+class Node:
+    """Generic pipeline Node."""
+
+    def __init__(self):
+        self._pipeline = None
+        self._is_ready = False
+        self.__upstream = None
+        self.__downstream = None
+
+    def __or__(self, other):
+        if isinstance(other, Node):
+            self._downstream = other
+            other._upstream = self
+            return Pipeline(self, other)
+        return NotImplemented
+
+    def to_dict(self):
+        return dict(type=self.__class__.__name__)
+
+    def setup(self):
+        """Run setup for this Node."""
+        self._is_ready = True
+
+    def reset(self):
+        """Reset this Node."""
+        self._is_ready = False
+
+    def process(self, frame):
+        """Process one frame of data."""
+        return frame
+
+    @property
+    def _upstream(self):
+        """Wrap for the upstream node object."""
+        return self.__upstream
+
+    @_upstream.setter
+    def _upstream(self, node):
+        """Set the upstream node, running update code."""
+        self.__upstream = node
+        self._upstream_changed()
+
+    def _upstream_changed(self):
+        """Code to run when the upstream is changed."""
+        pass
+
+    @property
+    def _downstream(self):
+        """Wrap for the downstream node object."""
+        return self.__downstream
+
+    @_downstream.setter
+    def _downstream(self, node):
+        """Set the downstream node, running update code."""
+        self.__downstream = node
+        self._downstream_changed()
+
+    def _downstream_changed(self):
+        """Code to run when the downstream is changed."""
+        pass
+
+    def push(self, packet):
+        """Give a packet of data as the input to this node.
+
+        Processes a frame and passes it along down the pipeline.
+        """
+        if isinstance(packet, Frame):
+            packet = self.process(packet)
+
+        if packet is None:
+            return
+
+        if self._downstream is not None:
+            # We should push the frame down the pipeline, and return the final result.
+            return self._downstream.push(packet)
+        else:
+            # This is the end of the pipeline, so return the frame.
+            return packet
+
+    def request(self, packet):
+        """Request one frame of output from this object.
+
+        Requests a frame from the upstream or this node, process it,
+        then return the frame.
+        """
+        if self._upstream is not None:
+            # There's an upstream node, ask it to handle the packet first.
+            packet = self._upstream.request(packet)
+
+        if isinstance(packet, Request):
+            if isinstance(packet, FrameRequest):
+                # Either there's no upstream node, or it could not handle the request.
+                # Process this request here, then return the generated frame.
+                return self.process(packet)
+
+
+class SamplerateDecider(Node):
+    """Base class for nodes that have an externally defined samplerate.
+
+    Instances of this type will decide the samplerate for an entire pipeline,
+    by telling the SamplerateFollowers what samplerate they are operating at.
+    """
+    def __init__(self, samplerate, **kwargs):
+        super().__init__(**kwargs)
+        self.samplerate = samplerate
+
+    def to_dict(self):
+        return super().to_dict() | dict(
+            samplerate=self.samplerate,
+        )
+
+    def _upstream_changed(self):
+        super()._upstream_changed()
+        if isinstance(self._upstream, SamplerateFollower):
+            self._upstream._set_samplerate_direction('downstream')
+
+    def _downstream_changed(self):
+        super()._downstream_changed()
+        if isinstance(self._downstream, SamplerateFollower):
+            self._downstream._set_samplerate_direction('upstream')
+
+
+class SamplerateFollower(Node):
+    """Base class for nodes which have no external samplerate.
+
+    Instances of this class will look for a samplerate elsewhere in the pipeline.
+    This can be found either upstream when the instance is receiving data from
+    a SamperateDecider, or downstream when the instance will send data to a SamplerateDecider.
+    This is managed automatically when assembling the pipeline, no user interaction required.
+    """
+    def __init__(self, **kwargs):
+        self._samplerate_direction = None
+        super().__init__(**kwargs)
+
+    def _upstream_changed(self):
+        """Clear any stored samplerate direction since it might no longer be valid."""
+        super()._upstream_changed()
+        self._samplerate_direction = None
+
+    def _downstream_changed(self):
+        """Clear any stored samplerate direction since it might no longer be valid."""
+        super()._downstream_changed()
+        self._samplerate_direction = None
+
+    @property
+    def samplerate(self):
+        direction = self._get_samplerate_direction()
+        if direction == 'upstream':
+            samplerate = self._upstream.samplerate
+            try:
+                _, samplerate = samplerate
+            except TypeError:
+                pass
+            return samplerate
+        if direction == 'downstream':
+            samplerate = self._downstream.samplerate
+            try:
+                samplerate, _ = samplerate
+            except TypeError:
+                pass
+            return samplerate
+
+    def _get_samplerate_direction(self, direction='both'):
+        """Check if the samplerate can be found along the pipeline.
+
+        This will run along the pipeline and see if there's a SamplerateDecider
+        somewhere. If a direction is specified, it will only look in the given direction.
+        If found, all other SamplerateFollowers will be updated.
+
+        This is a complicated getter for the samplerate direction, parameterized with a
+        search direction to allow recursive searches. Additionally, when the value is found
+        it will be updated for all the relevant SamplerateFollowers.
+        """
+        if self._samplerate_direction is not None:
+            return self._samplerate_direction
+
+        if direction == 'both':
+            self._samplerate_direction = self._get_samplerate_direction('upstream') or self._get_samplerate_direction('downstream')
+            return self._samplerate_direction
+
+        if direction == 'upstream':
+            if isinstance(self._upstream, SamplerateDecider):
+                self._set_samplerate_direction('upstream')
+                return 'upstream'
+            elif isinstance(self._upstream, SamplerateFollower):
+                return self._upstream._get_samplerate_direction('upstream')
+        elif direction == 'downstream':
+            if isinstance(self._downstream, SamplerateDecider):
+                self._set_samplerate_direction('downstream')
+                return 'downstream'
+            elif isinstance(self._downstream, SamplerateFollower):
+                return self._downstream._get_samplerate_direction('downstream')
+        else:
+            raise ValueError(f"Search direction should be one of 'upstream' or 'downstream', got {direction}")
+        return False
+
+    def _set_samplerate_direction(self, direction):
+        """Update the pipeline samplerate direction.
+
+        This will go through the pipeline in one direction and update
+        the samplerate search direction.
+        It will always go through the pipeline in the opposite direction to the
+        search direction. I.e., if diretcion='upstream', this will go downstream
+        set all the samplerate directions to 'upstream', and vice versa.
+        """
+        if direction == 'upstream':
+            self._samplerate_direction = 'upstream'
+            if isinstance(self._downstream, SamplerateFollower):
+                if self._downstream._samplerate_direction is None:
+                    self._downstream._set_samplerate_direction('upstream')
+                elif self._downstream._samplerate_direction == 'downstream':
+                    raise ValueError('Conflicting pipeline samplerates!')
+        elif direction == 'downstream':
+            self._samplerate_direction = 'downstream'
+            if isinstance(self._upstream, SamplerateFollower):
+                if self._upstream._samplerate_direction is None:
+                    self._upstream._set_samplerate_direction('downstream')
+                elif self._upstream._samplerate_direction == 'upstream':
+                    raise ValueError('Conflicting pipeline samplerates!')
```

### Comparing `acoustics-hardware-0.2.0/acoustics_hardware/analysis.py` & `acoustics-hardware-0.2.1/acoustics_hardware/analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,245 +1,263 @@
-import numpy as np
-import scipy.signal
-from . import signal_tools
-
-
-def dB(x, power=False, safe_zeros=True):
-    if safe_zeros:
-        x = signal_tools.nonzero_signals(x)
-    if power:
-        if np.any(x < 0):
-            return 10 * np.log10(x + 0j)
-        return 10 * np.log10(x)
-    else:
-        return 20 * np.log10(np.abs(x))
-
-
-def sweep_deconvolution(
-    reference_signal,
-    measured_signal,
-    samplerate=None,
-    lower_cutoff=None,
-    upper_cutoff=None,
-    truncation_length=None,
-    output_length=None,
-    fade_in=None,
-    fade_out=None,
-    ir_orders=1,
-    inversion_method='regularized',
-    **kwargs
-):
-    if isinstance(inversion_method, str):
-        if inversion_method.lower() == 'filtering':
-            inversion_method = _filtered_deconvolution
-        elif inversion_method.lower() == 'regularized':
-            inversion_method = _regularized_deconvolution
-        elif inversion_method.lower() == 'analytic':
-            inversion_method = _exponential_sweep_analytical_deconvolution
-        elif inversion_method.lower() == 'time-reversal':
-            inversion_method = _exponential_sweep_time_reversal_deconvolution
-        else:
-            raise ValueError(f'Unknown inverse filtering method {inversion_method}')
-
-    impulse_response = inversion_method(
-        reference_signal=reference_signal,
-        measured_signal=measured_signal,
-        samplerate=samplerate,
-        lower_cutoff=lower_cutoff,
-        upper_cutoff=upper_cutoff,
-        **kwargs
-    )
-
-    if ir_orders == 'whole':
-        return impulse_response
-
-    num_samples = impulse_response.shape[-1] // 2
-
-    irs = [impulse_response[..., :num_samples]]
-    if ir_orders > 1:
-        phase_rate = reference_signal.size / np.log(upper_cutoff / lower_cutoff)
-        lags = np.log(np.arange(1, ir_orders + 1)) * phase_rate  # How much each impulse response is before the linear one
-        indices = num_samples - np.ceil(lags).astype(int)  # The index where each of the impulse responses start
-        for order in range(1, ir_orders):  # Starts with order 1, corresponding to the first harmonic.
-            irs.append(impulse_response[indices[order]:indices[order - 1]])
-
-    irs = signal_tools.truncate_signals(irs, length=truncation_length, samplerate=samplerate)
-    irs = signal_tools.extend_signals(irs, length=output_length, samplerate=samplerate)
-    irs = signal_tools.fade_signals(irs, fade_in=fade_in, fade_out=fade_out, samplerate=samplerate)
-
-    if len(irs) == 1:
-        return irs[0]
-    return irs
-
-
-def _filtered_deconvolution(
-    reference_signal,
-    measured_signal,
-    samplerate=None,
-    lower_cutoff=None,
-    upper_cutoff=None,
-    **kwargs
-):
-    measured_signal = np.asarray(measured_signal)
-    num_samples = measured_signal.shape[-1]
-    impulse_response = np.fft.irfft(
-        np.fft.rfft(measured_signal, 2 * num_samples)
-        / np.fft.rfft(reference_signal, 2 * num_samples)
-    )
-
-    filter_args = kwargs or {}
-    if lower_cutoff is not None and upper_cutoff is not None:
-        filter_args.setdefault('Wn', (lower_cutoff, upper_cutoff))
-        filter_args['btype'] = 'bandpass'
-    elif lower_cutoff is not None:
-        filter_args.setdefault('Wn', lower_cutoff)
-        filter_args['btype'] = 'highpass'
-    elif upper_cutoff is not None:
-        filter_args.setdefault('Wn', upper_cutoff)
-        filter_args['btype'] = 'lowpass'
-    else:
-        return impulse_response
-
-    filter_args.setdefault('N', 8)
-    filter_args.setdefault('fs', samplerate)
-    filter_args.setdefault('ftype', 'butter')
-    filter_args['output'] = 'sos'
-
-    sos = scipy.signal.iirfilter(**filter_args)
-    impulse_response = scipy.signal.sosfilt(sos, impulse_response)
-    return impulse_response
-
-
-def _regularized_deconvolution(
-    reference_signal,
-    measured_signal,
-    samplerate=None,
-    lower_cutoff=None,
-    upper_cutoff=None,
-    transition_width=1 / 12,
-    interior_regularization=0.01,
-    exterior_regularization=1,
-):
-    measured_signal = np.asarray(measured_signal)
-    num_samples = measured_signal.shape[-1]
-
-    reference_spectrum = np.fft.rfft(reference_signal, 2 * num_samples)
-    samplerate = samplerate or 2  # No given samplerate -> frequencies normalized to Nyquist as in iirfilter
-    f = np.fft.rfftfreq(2 * num_samples, 1 / samplerate)
-    if lower_cutoff is None:
-        lower_cutoff = f[1]
-    if upper_cutoff is None:
-        upper_cutoff = f[-1]
-    lower_cutoff_interior = lower_cutoff * 2**transition_width
-    upper_cutoff_interior = upper_cutoff / 2**transition_width
-
-    regularization = np.zeros(reference_spectrum.shape)
-    interior_idx = (lower_cutoff_interior <= f) & (f <= upper_cutoff_interior)
-    regularization[interior_idx] = 1 / f[interior_idx] * interior_regularization
-    regularization[0] = 0
-
-    regularization[f <= lower_cutoff] = exterior_regularization / lower_cutoff
-    slope_idx = (lower_cutoff < f) & (f < lower_cutoff_interior)
-    regularization[slope_idx] = np.geomspace(exterior_regularization / lower_cutoff, interior_regularization / lower_cutoff_interior, np.sum(slope_idx))
-
-    slope_idx = (upper_cutoff_interior < f) & (f < upper_cutoff)
-    regularization[upper_cutoff <= f] = exterior_regularization / upper_cutoff
-    regularization[slope_idx] = np.geomspace(interior_regularization / upper_cutoff_interior, exterior_regularization / upper_cutoff, np.sum(slope_idx))
-
-    regularization *= np.mean(np.abs(reference_spectrum[interior_idx])**2 / regularization[interior_idx]) * interior_regularization
-    inverse_spectrum = reference_spectrum.conj() / (reference_spectrum.conj() * reference_spectrum + regularization)
-
-    impulse_response = np.fft.irfft(np.fft.rfft(measured_signal, n=2 * num_samples) * inverse_spectrum)
-    return impulse_response
-
-
-def _exponential_sweep_analytical_deconvolution(
-    reference_signal,
-    measured_signal,
-    samplerate,
-    lower_cutoff,
-    upper_cutoff,
-):
-    num_samples = reference_signal.size
-    phase_rate = num_samples / samplerate / np.log(upper_cutoff / lower_cutoff)
-    f = np.fft.rfftfreq(num_samples, 1 / samplerate)
-    with np.errstate(divide='ignore', invalid='ignore'):
-        inverse_spectrum = 2 * (f / phase_rate)**0.5 * np.exp(-2j * np.pi * f * phase_rate * (1 - np.log(f / lower_cutoff)) + 1j * np.pi / 4)
-    inverse_spectrum[0] = 0
-    # We have to go back to time to zero pad.
-    # It's much easier to generate the correct spectrum with the original reference length.
-    inverse_filter = np.fft.irfft(inverse_spectrum) / samplerate
-
-    measured_signal = np.asarray(measured_signal)
-    num_samples = measured_signal.shape[-1]
-
-    impulse_response = np.fft.irfft(
-        np.fft.rfft(measured_signal, n=2 * num_samples)
-        * np.fft.rfft(inverse_filter, n=2 * num_samples),
-    )
-    impulse_response = np.roll(impulse_response, -reference_signal.size, axis=-1)
-
-    return impulse_response
-
-
-def _exponential_sweep_time_reversal_deconvolution(
-    reference_signal,
-    measured_signal,
-    lower_cutoff,
-    upper_cutoff,
-    samplerate=None,
-):
-    amplitude_correction = 10**(np.linspace(0, -6 * np.log2(upper_cutoff / lower_cutoff), reference_signal.size) / 20)
-    inverse_filter = reference_signal[-1::-1] * amplitude_correction
-
-    measured_signal = np.asarray(measured_signal)
-    num_samples = measured_signal.shape[-1]
-
-    impulse_response = np.fft.irfft(
-        np.fft.rfft(measured_signal, n=2 * num_samples, axis=-1)
-        * np.fft.rfft(inverse_filter, n=2 * num_samples),
-        axis=-1
-    )
-    impulse_response = np.roll(impulse_response, -reference_signal.size, axis=-1)
-
-    return impulse_response
-
-
-def mls_analysis(reference, output):
-    output = np.atleast_2d(output)
-    seq_len = len(reference)
-    order = np.round(np.log2(seq_len + 1)).astype(int)
-    reps = int(output.shape[1] / seq_len)
-
-    if reps > 1:
-        response = output[:, seq_len:reps * seq_len].reshape((-1, reps - 1, seq_len)).mean(axis=1)
-    else:
-        response = output[:, :seq_len]
-
-    if order <= 8:
-        dtype = np.uint8
-    elif order <= 16:
-        dtype = np.uint16
-    elif order <= 32:
-        dtype = np.uint32
-    elif order <= 64:
-        dtype = np.uint64
-    else:
-        assert False, "You would need at least one zettabyte memory to store this array..."
-
-    ps = np.zeros(seq_len, dtype=dtype)
-    idx = np.arange(seq_len)  # Cannot be uint since it will be subtracted to be negative!
-    ref = reference.astype(dtype)
-    for s in range(order):
-        ps[idx] += ref[(idx - s) % seq_len] << (order - 1 - s)
-
-    indices = np.argsort(ps)[2**np.arange(order - 1, -1, -1, dtype=dtype) - 1]  # This also will not be uint.
-    pl = np.zeros(seq_len, dtype=dtype)
-    for s in range(order):
-        pl += ref[(indices[s] - idx) % seq_len] << (order - s - 1)
-
-    transform = np.zeros((output.shape[0], seq_len + 1))
-    transform[:, ps] = response
-    for _ in range(order):
-        transform = np.concatenate((transform[:, ::2] + transform[:, 1::2], transform[:, ::2] - transform[:, 1::2]), axis=1)
-    ir = transform[:, pl] / (seq_len + 1)
-    return np.squeeze(ir)
+import numpy as np
+import scipy.signal
+from . import signal_tools
+
+
+def dB(x, power=False, safe_zeros=True):
+    if safe_zeros and np.size(x) > 1:
+        x = signal_tools.nonzero_signals(x)
+    if power:
+        if np.any(x < 0):
+            if power == 'imag':
+                return 10 * np.log10(x + 0j)
+            if power == 'nan':
+                return 10 * np.log10(np.where(x > 0, x, np.nan))
+        return 10 * np.log10(x)
+    else:
+        return 20 * np.log10(np.abs(x))
+
+
+def sweep_deconvolution(
+    reference_signal,
+    measured_signal,
+    samplerate=None,
+    lower_cutoff=None,
+    upper_cutoff=None,
+    truncation_length=None,
+    output_length=None,
+    fade_in=None,
+    fade_out=None,
+    ir_orders=1,
+    inversion_method='regularized',
+    **kwargs
+):
+    if isinstance(inversion_method, str):
+        if inversion_method.lower() == 'filtering':
+            inversion_method = _filtered_deconvolution
+        elif inversion_method.lower() == 'regularized':
+            inversion_method = _regularized_deconvolution
+        elif inversion_method.lower() == 'analytic':
+            inversion_method = _exponential_sweep_analytical_deconvolution
+        elif inversion_method.lower() == 'time-reversal':
+            inversion_method = _exponential_sweep_time_reversal_deconvolution
+        else:
+            raise ValueError(f'Unknown inverse filtering method {inversion_method}')
+
+    impulse_response = inversion_method(
+        reference_signal=reference_signal,
+        measured_signal=measured_signal,
+        samplerate=samplerate,
+        lower_cutoff=lower_cutoff,
+        upper_cutoff=upper_cutoff,
+        **kwargs
+    )
+
+    if ir_orders == 'whole':
+        return impulse_response
+
+    num_samples = impulse_response.shape[-1] // 2
+
+    irs = [impulse_response[..., :num_samples]]
+    if ir_orders > 1:
+        phase_rate = reference_signal.size / np.log(upper_cutoff / lower_cutoff)
+        lags = np.log(np.arange(1, ir_orders + 1)) * phase_rate  # How much each impulse response is before the linear one
+        indices = num_samples - np.ceil(lags).astype(int)  # The index where each of the impulse responses start
+        for order in range(1, ir_orders):  # Starts with order 1, corresponding to the first harmonic.
+            irs.append(impulse_response[indices[order]:indices[order - 1]])
+
+    irs = signal_tools.truncate_signals(irs, length=truncation_length, samplerate=samplerate)
+    irs = signal_tools.extend_signals(irs, length=output_length, samplerate=samplerate)
+    irs = signal_tools.fade_signals(irs, fade_in=fade_in, fade_out=fade_out, samplerate=samplerate)
+
+    if len(irs) == 1:
+        return irs[0]
+    return irs
+
+
+def _filtered_deconvolution(
+    reference_signal,
+    measured_signal,
+    samplerate=None,
+    lower_cutoff=None,
+    upper_cutoff=None,
+    **kwargs
+):
+    measured_signal = np.asarray(measured_signal)
+    num_samples = measured_signal.shape[-1]
+    impulse_response = np.fft.irfft(
+        np.fft.rfft(measured_signal, 2 * num_samples)
+        / np.fft.rfft(reference_signal, 2 * num_samples)
+    )
+
+    filter_args = kwargs or {}
+    if lower_cutoff is not None and upper_cutoff is not None:
+        filter_args.setdefault('Wn', (lower_cutoff, upper_cutoff))
+        filter_args['btype'] = 'bandpass'
+    elif lower_cutoff is not None:
+        filter_args.setdefault('Wn', lower_cutoff)
+        filter_args['btype'] = 'highpass'
+    elif upper_cutoff is not None:
+        filter_args.setdefault('Wn', upper_cutoff)
+        filter_args['btype'] = 'lowpass'
+    else:
+        return impulse_response
+
+    filter_args.setdefault('N', 8)
+    filter_args.setdefault('fs', samplerate)
+    filter_args.setdefault('ftype', 'butter')
+    filter_args['output'] = 'sos'
+
+    sos = scipy.signal.iirfilter(**filter_args)
+    impulse_response = scipy.signal.sosfilt(sos, impulse_response)
+    return impulse_response
+
+
+def _regularized_deconvolution(
+    reference_signal,
+    measured_signal,
+    samplerate=None,
+    lower_cutoff=None,
+    upper_cutoff=None,
+    transition_width=1 / 12,
+    interior_regularization=0.01,
+    exterior_regularization=1,
+):
+    measured_signal = np.asarray(measured_signal)
+    num_samples = measured_signal.shape[-1]
+
+    reference_spectrum = np.fft.rfft(reference_signal, 2 * num_samples)
+    samplerate = samplerate or 2  # No given samplerate -> frequencies normalized to Nyquist as in iirfilter
+    f = np.fft.rfftfreq(2 * num_samples, 1 / samplerate)
+    if lower_cutoff is None:
+        lower_cutoff = f[1]
+    if upper_cutoff is None:
+        upper_cutoff = f[-1]
+    lower_cutoff_interior = lower_cutoff * 2**transition_width
+    upper_cutoff_interior = upper_cutoff / 2**transition_width
+
+    regularization = np.zeros(reference_spectrum.shape)
+    interior_idx = (lower_cutoff_interior <= f) & (f <= upper_cutoff_interior)
+    regularization[interior_idx] = 1 / f[interior_idx] * interior_regularization
+    regularization[0] = 0
+
+    regularization[f <= lower_cutoff] = exterior_regularization / lower_cutoff
+    slope_idx = (lower_cutoff < f) & (f < lower_cutoff_interior)
+    regularization[slope_idx] = np.geomspace(exterior_regularization / lower_cutoff, interior_regularization / lower_cutoff_interior, np.sum(slope_idx))
+
+    slope_idx = (upper_cutoff_interior < f) & (f < upper_cutoff)
+    regularization[upper_cutoff <= f] = exterior_regularization / upper_cutoff
+    regularization[slope_idx] = np.geomspace(interior_regularization / upper_cutoff_interior, exterior_regularization / upper_cutoff, np.sum(slope_idx))
+
+    regularization *= np.mean(np.abs(reference_spectrum[interior_idx])**2 / regularization[interior_idx]) * interior_regularization
+    inverse_spectrum = reference_spectrum.conj() / (reference_spectrum.conj() * reference_spectrum + regularization)
+
+    impulse_response = np.fft.irfft(np.fft.rfft(measured_signal, n=2 * num_samples) * inverse_spectrum)
+    return impulse_response
+
+
+def _exponential_sweep_analytical_deconvolution(
+    reference_signal,
+    measured_signal,
+    samplerate,
+    lower_cutoff,
+    upper_cutoff,
+):
+    num_samples = reference_signal.size
+    phase_rate = num_samples / samplerate / np.log(upper_cutoff / lower_cutoff)
+    f = np.fft.rfftfreq(num_samples, 1 / samplerate)
+    with np.errstate(divide='ignore', invalid='ignore'):
+        inverse_spectrum = 2 * (f / phase_rate)**0.5 * np.exp(-2j * np.pi * f * phase_rate * (1 - np.log(f / lower_cutoff)) + 1j * np.pi / 4)
+    inverse_spectrum[0] = 0
+    # We have to go back to time to zero pad.
+    # It's much easier to generate the correct spectrum with the original reference length.
+    inverse_filter = np.fft.irfft(inverse_spectrum) / samplerate
+
+    measured_signal = np.asarray(measured_signal)
+    num_samples = measured_signal.shape[-1]
+
+    impulse_response = np.fft.irfft(
+        np.fft.rfft(measured_signal, n=2 * num_samples)
+        * np.fft.rfft(inverse_filter, n=2 * num_samples),
+    )
+    impulse_response = np.roll(impulse_response, -reference_signal.size, axis=-1)
+
+    return impulse_response
+
+
+def _exponential_sweep_time_reversal_deconvolution(
+    reference_signal,
+    measured_signal,
+    lower_cutoff,
+    upper_cutoff,
+    samplerate=None,
+):
+    amplitude_correction = 10**(np.linspace(0, -6 * np.log2(upper_cutoff / lower_cutoff), reference_signal.size) / 20)
+    inverse_filter = reference_signal[-1::-1] * amplitude_correction
+
+    measured_signal = np.asarray(measured_signal)
+    num_samples = measured_signal.shape[-1]
+
+    impulse_response = np.fft.irfft(
+        np.fft.rfft(measured_signal, n=2 * num_samples, axis=-1)
+        * np.fft.rfft(inverse_filter, n=2 * num_samples),
+        axis=-1
+    )
+    impulse_response = np.roll(impulse_response, -reference_signal.size, axis=-1)
+
+    return impulse_response
+
+
+def mls_analysis(reference, output):
+    output = np.atleast_2d(output)
+    seq_len = len(reference)
+    order = np.round(np.log2(seq_len + 1)).astype(int)
+    reps = int(output.shape[1] / seq_len)
+
+    # Handle different reference mappings
+    ref_check = np.sum(reference)
+    if ref_check == 1:
+        # Mapped with (0, 1) -> (-1, 1)
+        reference = (reference + 1) / 2
+    elif ref_check == -1:
+        # Mapped with (0, 1) -> (1, -1)
+        reference = (1 - reference) / 2
+    elif ref_check == 2**(order - 1) - 1:
+        # Mapped with (0, 1) -> (1, 0)
+        reference = 1 - reference
+
+    if np.sum(reference) != 2**(order - 1):
+        raise ValueError('MLS reference sequence is not a single iteration of a valid MLS')
+
+    if reps > 1:
+        response = output[:, seq_len:reps * seq_len].reshape((-1, reps - 1, seq_len)).mean(axis=1)
+    else:
+        response = output[:, :seq_len]
+
+    if order <= 8:
+        dtype = np.uint8
+    elif order <= 16:
+        dtype = np.uint16
+    elif order <= 32:
+        dtype = np.uint32
+    elif order <= 64:
+        dtype = np.uint64
+    else:
+        assert False, "You would need at least one zettabyte memory to store this array..."
+
+    ps = np.zeros(seq_len, dtype=dtype)
+    idx = np.arange(seq_len)  # Cannot be uint since it will be subtracted to be negative!
+    ref = reference.astype(dtype)
+    for s in range(order):
+        ps[idx] += ref[(idx - s) % seq_len] << (order - 1 - s)
+
+    indices = np.argsort(ps)[2**np.arange(order - 1, -1, -1, dtype=dtype) - 1]  # This also will not be uint.
+    pl = np.zeros(seq_len, dtype=dtype)
+    for s in range(order):
+        pl += ref[(indices[s] - idx) % seq_len] << (order - s - 1)
+
+    transform = np.zeros((output.shape[0], seq_len + 1))
+    transform[:, ps] = response
+    for _ in range(order):
+        transform = np.concatenate((transform[:, ::2] + transform[:, 1::2], transform[:, ::2] - transform[:, 1::2]), axis=1)
+    ir = transform[:, pl] / (seq_len + 1)
+    return np.squeeze(ir)
```

### Comparing `acoustics-hardware-0.2.0/acoustics_hardware/interfaces.py` & `acoustics-hardware-0.2.1/acoustics_hardware/interfaces.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,742 +1,742 @@
-from . import _core, signal_tools
-import numpy as np
-import sounddevice as sd
-import time
-import functools
-import warnings
-
-try:
-    import nidaqmx
-    import nidaqmx.stream_readers
-    import nidaqmx.stream_writers
-except ImportError:
-    pass
-
-
-def _channel_collection(channel_class, **default_channel_kwargs):
-    @functools.wraps(channel_class, updated=())
-    class ChannelCollection:
-        default_channel_settings = default_channel_kwargs
-        def __init__(self, channels=None):
-            self.channels = []
-            if channels is None:
-                return
-
-            if isinstance(channels, int):
-                # Channels given as number of channels to use
-                channels = range(channels)
-            if isinstance(channels, dict):
-                # Channels given as a single dict defining one channel
-                channels = [channels]
-
-            try:
-                # Channels given as a single pair of (int, dict) for a single channel
-                ch, configs = channels
-            except (ValueError, TypeError):
-                pass
-            else:
-                if isinstance(ch, int) and isinstance(configs, dict):
-                    # This extra check is needed in case channels is given as e.g. [0, 1]
-                    # which defines two channels, not one.
-                    channels = [channels]
-
-            for channel in channels:
-                try:
-                    # This channel is a single dict defining the channel
-                    self.append(**channel)
-                except TypeError:
-                    pass
-                else:
-                    continue
-
-                try:
-                    # Channel is an (int, dict) pair
-                    ch, configs = channel
-                except (ValueError, TypeError):
-                    pass
-                else:
-                    if isinstance(ch, int) and isinstance(configs, dict):
-                        self.append(channel=ch, **configs)
-                        continue
-
-                if isinstance(channel, int):
-                    # This channel i s just defined by its index, with no settings
-                    self.append(channel)
-                    continue
-                raise ValueError(f'Cannot add channel with definition {channel}')
-
-
-        def append(self, channel, **kwargs):
-            self.channels.append(channel_class(channel, **self.default_channel_settings | kwargs))
-
-        def __getitem__(self, key):
-            return self.channels[key]
-
-        def __len__(self):
-            return len(self.channels)
-
-        def __repr__(self):
-            return repr(self.channels)
-
-    return ChannelCollection
-
-
-class SimpleChannel:
-    """A single channel without settings.
-
-    Parameters
-    -----------
-    channel : int
-        The index of the channel, zero based.
-    label : string, default none
-        An optional label to assign to the channel.
-    """
-
-    def __init__(self, channel, label=None):
-        self.channel = channel
-        self.label = label
-
-    def __repr__(self):
-        label = '' if self.label is None else f", '{self.label}'"
-        return f'{self.__class__.__name__}({self.channel}{label})'
-
-
-class _StreamedInterface(_core.SamplerateDecider):
-    _input_channels = _channel_collection(SimpleChannel)
-    _output_channels = _channel_collection(SimpleChannel)
-
-    def __init__(self, input_channels=None, output_channels=None, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.input_channels = self._input_channels(input_channels)
-        self.output_channels = self._output_channels(output_channels)
-
-    def to_dict(self):
-        return super().to_dict() | dict(
-            input_channels=repr(self.input_channels),
-            output_channels=repr(self.output_channels),
-        )
-
-    def process(self, packet):
-        frame = framesize = None
-        if isinstance(packet, _core.Frame):
-            frame = packet.frame
-        elif isinstance(packet, _core.FrameRequest):
-            framesize = packet.framesize
-        elif not isinstance(packet, _core.Packet):
-            if np.ndim(packet) == 0:
-                framesize = packet
-            else:
-                frame = packet
-        return _core.Frame(self.playrec(frame=frame, framesize=framesize))
-
-
-class DummyInterface(_StreamedInterface):
-    def __init__(self, framesize=None, maxframes=np.inf, realtime=False, threaded=True, **kwargs):
-        super().__init__(**kwargs)
-        self.framesize = framesize
-        self.maxframes = maxframes
-        self.realtime = realtime
-        self.threaded = threaded
-
-    def run(self):
-        if self.threaded:
-            import threading
-            self._running = threading.Event()
-            self._thread = threading.Thread(target=self._passthrough_target)
-            self._thread.start()
-        else:
-            frames = 0
-            while frames < self.maxframes:
-                frames += 1
-                frame = self._upstream.request(_core.FrameRequest(self.framesize))
-                if self.realtime:
-                    time.sleep(self.framesize / self.samplerate)
-                self._downstream.push(frame)
-                if isinstance(frame, _core.LastFrame):
-                    break
-
-    def _passthrough_target(self):
-        self._running.set()
-        frames = 0
-        while self._running.is_set() and frames < self.maxframes:
-            frames += 1
-            frame = self._upstream.request(self.framesize)
-            if self.realtime:
-                time.sleep(self.framesize / self.samplerate)
-            self._downstream.push(frame)
-            if isinstance(frame, _core.LastFrame):
-                self._running.clear()
-                break
-
-    def playrec(self, frame=None, framesize=None):
-        if frame is not None:
-            return frame
-        return np.zeros((1, framesize))
-
-    def stop(self):
-        self._running.clear()
-
-
-class AudioInterface(_StreamedInterface):
-    @classmethod
-    def list_interfaces(cls):
-        """Check which audio interfaces can be interacted with.
-
-        This is just a wrapper around `sounddevice.query_devices`.
-
-        Returns
-        -------
-        interfaces : list
-            A list of all interfaces found.
-        """
-        return sd.query_devices()
-
-    def __init__(self, name=None, input_name=None, output_name=None, framesize=None, **kwargs):
-        super().__init__(**kwargs)
-        self.framesize = framesize
-        input_name = input_name or name
-        output_name = output_name or name
-        input_name = sd.default.device[0] if input_name is None else input_name
-        output_name = sd.default.device[1] if output_name is None else output_name
-
-        device_list = sd.query_devices()
-        self._input_device = sd.query_devices(input_name)
-        self._input_device['index'] = device_list.index(self._input_device)
-        self._output_device = sd.query_devices(output_name)
-        self._output_device['index'] = device_list.index(self._output_device)
-
-    def to_dict(self):
-        return super().to_dict() | dict(
-            input_device=self._input_device['name'],
-            output_device=self._output_device['name'],
-            framesize=self.framesize,
-        )
-
-    def run(self):
-        outputs = [ch.channel for ch in self.output_channels]
-        inputs = [ch.channel for ch in self.input_channels]
-        num_input_ch = max(inputs, default=-1) + 1
-        num_output_ch = max(outputs, default=-1) + 1
-        if num_output_ch == 1 and self.max_outputs > 1:
-            # PortAudio by default duplicates mono channels over all channels.
-            # This is not what the rest of this package is doing.
-            num_output_ch = 2
-        silent_ch = [ch for ch in range(num_output_ch) if ch not in outputs]
-
-        def process_input(frame):
-            # Take the frame read from hardware and push it downstream in the pipeline.
-            frame = _core.Frame(frame.T[inputs])
-            self._downstream.push(frame)
-
-        def process_output(buffer):
-            # Get a frame from upstream in the pipeline and write it to the buffer.
-            frame = self._upstream.request(_core.FrameRequest(buffer.shape[0]))
-            buffer[:, outputs] = frame.frame.T
-            buffer[:, silent_ch] = 0
-            if isinstance(frame, _core.LastFrame):
-                raise sd.CallbackStop()
-
-        if num_input_ch and num_output_ch:
-            def callback(indata, outdata, frames, time, status):
-                process_input(indata)
-                process_output(outdata)
-            self._stream = sd.Stream(
-                samplerate=self.samplerate,
-                blocksize=self.framesize,
-                device=(self._input_device['index'], self._output_device['index']),
-                channels=(num_input_ch, num_output_ch),
-                callback=callback,
-            )
-        elif num_input_ch:
-            def callback(indata, frames, time, status):
-                process_input(indata)
-            self._stream = sd.InputStream(
-                samplerate=self.samplerate,
-                blocksize=self.framesize,
-                device=self._input_device['name'],
-                channels=num_input_ch,
-                callback=callback,
-            )
-        elif num_output_ch:
-            def callback(outdata, frames, time, status):
-                process_output(outdata)
-            self._stream = sd.OutputStream(
-                samplerate=self.samplerate,
-                blocksize=self.framesize,
-                device=self._output_device['name'],
-                channels=num_output_ch,
-                callback=callback,
-            )
-
-        self._stream.start()
-
-    def stop(self):
-        self._stream.stop()
-
-    def playrec(self, frame=None, framesize=None):
-        outputs = [ch.channel + 1 for ch in self.output_channels]
-        inputs = [ch.channel + 1 for ch in self.input_channels]
-
-        if len(inputs) and len(outputs):
-            return sd.playrec(
-                data=frame.T,
-                samplerate=self.samplerate,
-                device=(self._input_device['index'], self._output_device['index']),
-                input_mapping=inputs,
-                output_mapping=outputs,
-                blocking=True,
-            )
-        elif len(inputs):
-            return sd.rec(
-                frames=framesize,
-                samplerate=self.samplerate,
-                device=self._input_device['index'],
-                mapping=inputs,
-                blocking=True,
-            )
-        elif len(outputs):
-            return sd.play(
-                data=frame.T,
-                samplerate=self.samplerate,
-                device=self._output_device['index'],
-                mapping=outputs,
-                blocking=True,
-            )
-
-    @property
-    def max_inputs(self):
-        return self._input_device['max_input_channels']
-
-    @property
-    def max_outputs(self):
-        return self._output_device['max_output_channels']
-
-
-class NationalInstrumentsConfigurableChannel(SimpleChannel):
-    """A configurable National instruments channel
-
-    Parameters
-    ----------
-    channel : int
-        The index of the channel, zero based.
-    label : str, default None
-        Optional label to assign the channel
-    voltage_range : numeric
-        The range in which to configure the channel.
-        Give a two values (min, max) or a single amplitude value.
-    terminal_config : str, default None
-        How to configure the terminals for the channel. Leave as None to use device default configuration.
-        Should be one of
-        - Differential: for a differential input
-        - Single ended: for a single ended measurement
-    """
-    def __init__(self, channel, label=None, voltage_range=None, terminal_config=None):
-        super().__init__(channel=channel, label=label)
-        self.voltage_range = voltage_range
-        self.terminal_config = terminal_config
-
-    def config(self, interface):
-        configs = {}
-        if self.voltage_range is not None:
-            try:
-                min_val, max_val = self.voltage_range
-            except TypeError:
-                min_val = -self.voltage_range
-                max_val = self.voltage_range
-            configs['min_val'] = min_val
-            configs['max_val'] = max_val
-        if self.terminal_config is not None:
-            if 'diff' in self.terminal_config.lower():
-                configs['terminal_config'] = nidaqmx.constants.TerminalConfiguration.BAL_DIFF
-            elif 'single' in self.terminal_config.lower():
-                configs['terminal_config'] = nidaqmx.constants.TerminalConfiguration.RSE
-            else:
-                raise ValueError(f'Unknown terminal configuration {self.terminal_config}')
-        return configs
-
-    def __repr__(self):
-        s = super().__repr__()[:-1]
-        voltage_range = '' if self.voltage_range is None else f', voltage_range={self.voltage_range}'
-        terminal_config = '' if self.terminal_config is None else f', terminal_config={self.terminal_config}'
-        return s + voltage_range + terminal_config + ')'
-
-
-class NationalInstrumentsInputChannel(NationalInstrumentsConfigurableChannel):
-    def config(self, interface):
-        return super().config(interface) | dict(physical_channel=f'{interface.name}/ai{self.channel}')
-
-
-class NationalInstrumentsOutputChannel(NationalInstrumentsConfigurableChannel):
-    def config(self, interface):
-        return super().config(interface) | dict(physical_channel=f'{interface.name}/ao{self.channel}')
-
-
-class NationalInstrumentsDaqmx(_StreamedInterface):
-    @classmethod
-    def list_interfaces(cls):
-        """Check what National Instruments hardware is available.
-
-        Returns
-        -------
-        interfaces : list
-            A list of all devices.
-        """
-        try:
-            system = nidaqmx.system.System.local()
-        except NameError as e:
-            if e.args[0] == "name 'nidaqmx' is not defined":
-                raise ModuleNotFoundError("Windows-only module 'nidaqmx' is not installed")
-            else:
-                raise e
-        name_list = [dev.name for dev in system.devices]
-        return name_list
-
-    def __init__(self, name=None, framesize=None, buffer_n_frames=25, **kwargs):
-        self.name = name or self.list_interfaces()[0]
-        self._device = nidaqmx.system.Device(self.name)
-        self._input_channels = _channel_collection(
-            NationalInstrumentsInputChannel,
-            terminal_config='single ended',
-            voltage_range=(min(self._device.ai_voltage_rngs), max(self._device.ai_voltage_rngs))
-        )
-        self._output_channels = _channel_collection(
-            NationalInstrumentsOutputChannel,
-            voltage_range=(min(self._device.ao_voltage_rngs), max(self._device.ao_voltage_rngs))
-        )
-        super().__init__(**kwargs)
-        self.framesize = framesize
-        self.buffer_n_frames = buffer_n_frames
-
-    def to_dict(self):
-        return super().to_dict() | dict(
-            name=self.name,
-            framesize=self.framesize,
-        )
-
-    @property
-    def samplerate(self):
-        return self._samplerate
-
-    @samplerate.setter
-    def samplerate(self, val):
-        has_in = self.max_inputs > 0
-        has_out = self.max_outputs > 0
-
-        if val is None:
-            if has_in and has_out:
-                fs_in = self._device.ai_max_multi_chan_rate
-                fs_out = self._device.ao_max_rate
-            elif has_in:
-                fs_in = fs_out = self._device.ai_max_multi_chan_rate
-            elif has_out:
-                fs_in = fs_out = self._device.ao_max_rate
-            else:
-                raise ValueError(f'National Instruments interface {self.name} seems to have neither inputs nor outputs')
-        else:
-            try:
-                fs_out, fs_in = val
-            except TypeError:
-                fs_out = fs_in = val
-
-        if has_in:
-            task = nidaqmx.Task()
-            task.ai_channels.add_ai_voltage_chan(self._device.ai_physical_chans[0].name)
-            task.timing.cfg_samp_clk_timing(rate=fs_in)
-            if not fs_in == task.timing.samp_clk_rate:
-                warnings.warn(f'Target input samplerate {fs_in} not available on device, using {task.timing.samp_clk_rate}', stacklevel=2)
-                fs_in = task.timing.samp_clk_rate
-            task.close()
-
-        if has_out:
-            task = nidaqmx.Task()
-            task.ao_channels.add_ao_voltage_chan(self._device.ao_physical_chans[0].name)
-            task.timing.cfg_samp_clk_timing(rate=fs_out)
-            if not fs_out == task.timing.samp_clk_rate:
-                warnings.warn(f'Target output samplerate {fs_out} not available on device, using {task.timing.samp_clk_rate}', stacklevel=3)
-                fs_out = task.timing.samp_clk_rate
-            task.close()
-
-        if fs_out == fs_in:
-            self._samplerate = fs_in
-        else:
-            self._samplerate = (fs_out, fs_in)
-
-    @property
-    def framesize(self):
-        return self._framesize
-
-    @framesize.setter
-    def framesize(self, val):
-        if val is None:
-            fs = self.samplerate
-            try:
-                fs_out, fs_in = fs
-            except TypeError:
-                fs_in = fs_out = fs
-            N_in = fs_in // 50
-            N_out = fs_out // 50
-        else:
-            try:
-                N_out, N_in = val
-            except TypeError:
-                N_out = N_in = val
-
-        if N_out == N_in:
-            self._framesize = N_out
-        else:
-            self._framesize = (N_out, N_in)
-
-    def reset(self, **kwargs):
-        super().reset(**kwargs)
-        try:
-            self._device.reset_device()
-        except (AttributeError, nidaqmx.DaqError):
-            pass
-
-    @property
-    def max_inputs(self):
-        return len(self._device.ai_physical_chans)
-
-    @property
-    def max_outputs(self):
-        return len(self._device.ao_physical_chans)
-
-    def setup(self, finite_samples=False, **kwargs):
-        super().setup(**kwargs)
-
-        if len(self.input_channels):
-            self._input_task = nidaqmx.Task()
-            for ch in self.input_channels:
-                self._input_task.ai_channels.add_ai_voltage_chan(**ch.config(self))
-
-        if len(self.output_channels):
-            self._output_task = nidaqmx.Task()
-            for ch in self.output_channels:
-                self._output_task.ao_channels.add_ao_voltage_chan(**ch.config(self))
-
-        try:
-            samplerate_upstream, samplerate_downstream = self.samplerate
-        except TypeError:
-            samplerate_upstream = samplerate_downstream = self.samplerate
-
-        if finite_samples is False:
-            try:
-                framesize_upstream, framesize_downstream = self.framesize
-            except TypeError:
-                framesize_upstream = framesize_downstream = self.framesize
-            samps_per_chan_read = self.buffer_n_frames * framesize_downstream
-            samps_per_chan_write = self.buffer_n_frames * framesize_upstream
-            sample_mode = nidaqmx.constants.AcquisitionType.CONTINUOUS
-        else:
-            try:
-                samps_per_chan_write, samps_per_chan_read = finite_samples
-            except TypeError:
-                samps_per_chan_write = samps_per_chan_read = finite_samples
-            sample_mode = nidaqmx.constants.AcquisitionType.FINITE
-
-        if len(self.input_channels):
-            self._input_task.timing.cfg_samp_clk_timing(
-                rate=samplerate_downstream,
-                samps_per_chan=samps_per_chan_read,
-                sample_mode=sample_mode
-            )
-            if finite_samples is False:
-                self._databuffer = np.empty((self._input_task.in_stream.num_chans, framesize_downstream))
-                self._read = nidaqmx.stream_readers.AnalogMultiChannelReader(self._input_task.in_stream).read_many_sample
-                self._samples_read = 0
-                self._input_task.in_stream.input_buf_size = framesize_downstream * self.buffer_n_frames
-                self._input_task.register_every_n_samples_acquired_into_buffer_event(framesize_downstream, self._read_callback)
-
-        if len(self.output_channels):
-            self._output_task.timing.cfg_samp_clk_timing(
-                rate=samplerate_upstream,
-                samps_per_chan=samps_per_chan_write,
-                sample_mode=sample_mode
-            )
-
-            if finite_samples is False:
-                self._write = nidaqmx.stream_writers.AnalogMultiChannelWriter(self._output_task.out_stream).write_many_sample
-                self._output_task.out_stream.regen_mode = nidaqmx.constants.RegenerationMode.DONT_ALLOW_REGENERATION
-                self._samples_written = 0
-                self._output_task.out_stream.output_buf_size = framesize_upstream * self.buffer_n_frames
-                self._write_callback(None, None, self.buffer_n_frames * framesize_upstream, None)
-                self._output_task.register_every_n_samples_transferred_from_buffer_event(framesize_upstream, self._write_callback)
-
-        if len(self.output_channels) and len(self.input_channels):
-            self._input_task.triggers.start_trigger.cfg_dig_edge_start_trig(f'/{self.name}/ao/StartTrigger')
-
-
-    def run(self):
-        if not self._is_ready:
-            self.setup()
-
-        if len(self.input_channels):
-            self._input_task.start()
-        if len(self.output_channels):
-            self._output_task.start()
-
-    def stop(self):
-        self._is_ready = False  # The tasks are single use!
-
-        if len(self.output_channels):
-            try:
-                self._output_task.stop()
-                self._output_task.wait_until_done(timeout=10)
-                self._output_task.close()
-            except nidaqmx.DaqError:
-                pass
-
-        if len(self.input_channels):
-            if len(self.output_channels):
-                while self._samples_read < self._samples_written:
-                    time.sleep(self._input_task.in_stream.sleep_time)
-            try:
-                self._input_task.stop()
-                self._input_task.wait_until_done(timeout=10)
-                self._input_task.close()
-            except nidaqmx.DaqError:
-                pass
-
-    def _read_callback(self, task_handle, every_n_samples_event_type, number_of_samples, callback_data):
-        try:
-            self._read(self._databuffer, number_of_samples)
-        except nidaqmx.DaqError:
-            self.stop()
-            raise
-        self._samples_read += number_of_samples
-        self._downstream.push(_core.Frame(self._databuffer.copy()))
-        return 0
-
-    def _write_callback(self, task_handle, every_n_samples_event_type, number_of_samples, callback_data):
-        frame = self._upstream.request(_core.FrameRequest(number_of_samples))
-        self._write(frame.frame)
-        self._samples_written += number_of_samples
-        if isinstance(frame, _core.LastFrame):
-            self._samples_written -= number_of_samples
-            self._samples_written += frame.valid_samples
-            frame = self._write(np.zeros((len(self.output_channels), number_of_samples)))
-            while self._output_task.out_stream.total_samp_per_chan_generated < self._samples_written:
-                time.sleep(self._output_task.out_stream.sleep_time)
-            self.stop()
-        return 0
-
-    def playrec(self, frame=None, framesize=None):
-        if frame is not None:
-            padded_frame = signal_tools.pad_signals(frame, post_pad=1)
-        if framesize is None and len(self.input_channels):
-            try:
-                samplerate_upstream, samplerate_downstream = self.samplerate
-            except TypeError:
-                samplerate_upstream = samplerate_downstream = self.samplerate
-            framesize = np.math.ceil(padded_frame.shape[-1] * samplerate_downstream / samplerate_upstream)
-        self.setup(finite_samples=(padded_frame.shape[-1], framesize), pipeline=True)
-
-        if len(self.input_channels):
-            self._input_task.start()
-
-        if len(self.output_channels):
-            timeout = frame.shape[-1] / samplerate_upstream * 1.2 + 5
-            self._output_task.write(padded_frame.squeeze())
-            self._output_task.start()
-            self._output_task.wait_until_done(timeout=timeout)
-            self._output_task.close()
-
-        if len(self.input_channels):
-            timeout = framesize / samplerate_downstream * 1.2 + 5
-            read_frame = self._input_task.read(framesize, timeout=timeout)
-            read_frame = np.asarray(read_frame)
-            self._input_task.close()
-            return read_frame[..., 1:]
-
-
-class NationalInstrumentsMultimoduleInputChannel(NationalInstrumentsConfigurableChannel):
-    def __init__(self, module, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.module = module
-
-    def __repr__(self):
-        s = super().__repr__()
-        pre, post = s.split('(')
-        return f'{pre}(module={self.module}, {post}'
-
-    def config(self, interface):
-        return interface.input_modules[self.module].ai_physical_chans[self.channel].name
-
-
-class NationalInstrumentsMultimoduleOutputChannel(NationalInstrumentsMultimoduleInputChannel):
-    def config(self, interface):
-        return interface.output_modules[self.module].ao_physical_chans[self.channel].name
-
-
-class CompactDaqmxMultimodule(NationalInstrumentsDaqmx):
-    @classmethod
-    def get_chassis(cls, name=None):
-        devices = cls.list_interfaces()
-        chassis = [dev for dev in devices if 'cDAQ' in dev and 'Mod' not in dev]
-        if name is None:
-            return chassis
-        if name not in chassis:
-            name = [dev for dev in chassis if str(name) in dev][0]
-        return nidaqmx.system.Device(name)
-
-    @classmethod
-    def get_modules(cls, chassis):
-        try:
-            chassis = chassis.name
-        except AttributeError:
-            pass
-        chassis = cls.get_chassis(chassis)
-        devs = cls.list_interfaces()
-        return [nidaqmx.system.Device(dev) for dev in devs if chassis in dev and 'Mod' in dev]
-
-    @classmethod
-    def reset_chassis_modules(cls, chassis):
-        for module in cls.get_modules(chassis):
-            nidaqmx.system.Device(module).reset_device()
-
-    _input_channels = _channel_collection(NationalInstrumentsMultimoduleInputChannel)
-    _output_channels = _channel_collection(NationalInstrumentsMultimoduleOutputChannel)
-
-    def __init__(self, name=None, **kwargs):
-        if name is None:
-            name = self.list_devices()[0]
-        self.chassis = self.get_chassis(name)
-        self.modules = self.get_modules(self.chassis)
-
-        # We need to set a default name for the NIDAQ class to initialize properly
-        if len(self.input_modules) > 0:
-            self.name = self.input_modules[0]
-        elif len(self.output_modules) > 0:
-            self.name = self.output_modules[0]
-        super().__init__(**kwargs)
-        del self.name
-
-        self.input_modules = [module for module in self.modules if len(module.ai_physical_chans) > 0]
-        self.output_modules = [module for module in self.modules if len(module.ao_physical_chans) > 0]
-
-    @property
-    def max_inputs(self):
-        inputs = 0
-        for module in self.input_modules:
-            inputs += len(module.ai_physical_chans)
-        return inputs
-
-    @property
-    def max_outputs(self):
-        outputs = 0
-        for module in self.output_modules:
-            outputs += len(module.ao_physical_chans)
-        return outputs
-
-    def setup(self, **kwargs):
-        super().setup(**kwargs)
-        if len(self.input_channels) and len(self.output_channels):
-            self._output_task.timing.samp_clk_timebase_src = self._input_task.timing.samp_clk_timebase_src
-            self._output_task.timing.samp_clk_timebase_rate = self._input_task.timing.samp_clk_timebase_rate
-
-    def reset(self, **kwargs):
-        super().reset(**kwargs)
-        for module in self.input_modules:
-            module.reset_device()
-        for module in self.output_modules:
-            module.reset_device()
+from . import _core, signal_tools
+import numpy as np
+import sounddevice as sd
+import time
+import functools
+import warnings
+
+try:
+    import nidaqmx
+    import nidaqmx.stream_readers
+    import nidaqmx.stream_writers
+except ImportError:
+    pass
+
+
+def _channel_collection(channel_class, **default_channel_kwargs):
+    @functools.wraps(channel_class, updated=())
+    class ChannelCollection:
+        default_channel_settings = default_channel_kwargs
+        def __init__(self, channels=None):
+            self.channels = []
+            if channels is None:
+                return
+
+            if isinstance(channels, int):
+                # Channels given as number of channels to use
+                channels = range(channels)
+            if isinstance(channels, dict):
+                # Channels given as a single dict defining one channel
+                channels = [channels]
+
+            try:
+                # Channels given as a single pair of (int, dict) for a single channel
+                ch, configs = channels
+            except (ValueError, TypeError):
+                pass
+            else:
+                if isinstance(ch, int) and isinstance(configs, dict):
+                    # This extra check is needed in case channels is given as e.g. [0, 1]
+                    # which defines two channels, not one.
+                    channels = [channels]
+
+            for channel in channels:
+                try:
+                    # This channel is a single dict defining the channel
+                    self.append(**channel)
+                except TypeError:
+                    pass
+                else:
+                    continue
+
+                try:
+                    # Channel is an (int, dict) pair
+                    ch, configs = channel
+                except (ValueError, TypeError):
+                    pass
+                else:
+                    if isinstance(ch, int) and isinstance(configs, dict):
+                        self.append(channel=ch, **configs)
+                        continue
+
+                if isinstance(channel, int):
+                    # This channel i s just defined by its index, with no settings
+                    self.append(channel)
+                    continue
+                raise ValueError(f'Cannot add channel with definition {channel}')
+
+
+        def append(self, channel, **kwargs):
+            self.channels.append(channel_class(channel, **self.default_channel_settings | kwargs))
+
+        def __getitem__(self, key):
+            return self.channels[key]
+
+        def __len__(self):
+            return len(self.channels)
+
+        def __repr__(self):
+            return repr(self.channels)
+
+    return ChannelCollection
+
+
+class SimpleChannel:
+    """A single channel without settings.
+
+    Parameters
+    -----------
+    channel : int
+        The index of the channel, zero based.
+    label : string, default none
+        An optional label to assign to the channel.
+    """
+
+    def __init__(self, channel, label=None):
+        self.channel = channel
+        self.label = label
+
+    def __repr__(self):
+        label = '' if self.label is None else f", '{self.label}'"
+        return f'{self.__class__.__name__}({self.channel}{label})'
+
+
+class _StreamedInterface(_core.SamplerateDecider):
+    _input_channels = _channel_collection(SimpleChannel)
+    _output_channels = _channel_collection(SimpleChannel)
+
+    def __init__(self, input_channels=None, output_channels=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.input_channels = self._input_channels(input_channels)
+        self.output_channels = self._output_channels(output_channels)
+
+    def to_dict(self):
+        return super().to_dict() | dict(
+            input_channels=repr(self.input_channels),
+            output_channels=repr(self.output_channels),
+        )
+
+    def process(self, packet):
+        frame = framesize = None
+        if isinstance(packet, _core.Frame):
+            frame = packet.frame
+        elif isinstance(packet, _core.FrameRequest):
+            framesize = packet.framesize
+        elif not isinstance(packet, _core.Packet):
+            if np.ndim(packet) == 0:
+                framesize = packet
+            else:
+                frame = packet
+        return _core.Frame(self.playrec(frame=frame, framesize=framesize))
+
+
+class DummyInterface(_StreamedInterface):
+    def __init__(self, framesize=None, maxframes=np.inf, realtime=False, threaded=True, **kwargs):
+        super().__init__(**kwargs)
+        self.framesize = framesize
+        self.maxframes = maxframes
+        self.realtime = realtime
+        self.threaded = threaded
+
+    def run(self):
+        if self.threaded:
+            import threading
+            self._running = threading.Event()
+            self._thread = threading.Thread(target=self._passthrough_target)
+            self._thread.start()
+        else:
+            frames = 0
+            while frames < self.maxframes:
+                frames += 1
+                frame = self._upstream.request(_core.FrameRequest(self.framesize))
+                if self.realtime:
+                    time.sleep(self.framesize / self.samplerate)
+                self._downstream.push(frame)
+                if isinstance(frame, _core.LastFrame):
+                    break
+
+    def _passthrough_target(self):
+        self._running.set()
+        frames = 0
+        while self._running.is_set() and frames < self.maxframes:
+            frames += 1
+            frame = self._upstream.request(_core.FrameRequest(self.framesize))
+            if self.realtime:
+                time.sleep(self.framesize / self.samplerate)
+            self._downstream.push(frame)
+            if isinstance(frame, _core.LastFrame):
+                self._running.clear()
+                break
+
+    def playrec(self, frame=None, framesize=None):
+        if frame is not None:
+            return frame
+        return np.zeros((1, framesize))
+
+    def stop(self):
+        self._running.clear()
+
+
+class AudioInterface(_StreamedInterface):
+    @classmethod
+    def list_interfaces(cls):
+        """Check which audio interfaces can be interacted with.
+
+        This is just a wrapper around `sounddevice.query_devices`.
+
+        Returns
+        -------
+        interfaces : list
+            A list of all interfaces found.
+        """
+        return sd.query_devices()
+
+    def __init__(self, name=None, input_name=None, output_name=None, framesize=None, **kwargs):
+        super().__init__(**kwargs)
+        self.framesize = framesize
+        input_name = input_name or name
+        output_name = output_name or name
+        input_name = sd.default.device[0] if input_name is None else input_name
+        output_name = sd.default.device[1] if output_name is None else output_name
+
+        device_list = sd.query_devices()
+        self._input_device = sd.query_devices(input_name)
+        self._input_device['index'] = device_list.index(self._input_device)
+        self._output_device = sd.query_devices(output_name)
+        self._output_device['index'] = device_list.index(self._output_device)
+
+    def to_dict(self):
+        return super().to_dict() | dict(
+            input_device=self._input_device['name'],
+            output_device=self._output_device['name'],
+            framesize=self.framesize,
+        )
+
+    def run(self):
+        outputs = [ch.channel for ch in self.output_channels]
+        inputs = [ch.channel for ch in self.input_channels]
+        num_input_ch = max(inputs, default=-1) + 1
+        num_output_ch = max(outputs, default=-1) + 1
+        if num_output_ch == 1 and self.max_outputs > 1:
+            # PortAudio by default duplicates mono channels over all channels.
+            # This is not what the rest of this package is doing.
+            num_output_ch = 2
+        silent_ch = [ch for ch in range(num_output_ch) if ch not in outputs]
+
+        def process_input(frame):
+            # Take the frame read from hardware and push it downstream in the pipeline.
+            frame = _core.Frame(frame.T[inputs])
+            self._downstream.push(frame)
+
+        def process_output(buffer):
+            # Get a frame from upstream in the pipeline and write it to the buffer.
+            frame = self._upstream.request(_core.FrameRequest(buffer.shape[0]))
+            buffer[:, outputs] = frame.frame.T
+            buffer[:, silent_ch] = 0
+            if isinstance(frame, _core.LastFrame):
+                raise sd.CallbackStop()
+
+        if num_input_ch and num_output_ch:
+            def callback(indata, outdata, frames, time, status):
+                process_input(indata)
+                process_output(outdata)
+            self._stream = sd.Stream(
+                samplerate=self.samplerate,
+                blocksize=self.framesize,
+                device=(self._input_device['index'], self._output_device['index']),
+                channels=(num_input_ch, num_output_ch),
+                callback=callback,
+            )
+        elif num_input_ch:
+            def callback(indata, frames, time, status):
+                process_input(indata)
+            self._stream = sd.InputStream(
+                samplerate=self.samplerate,
+                blocksize=self.framesize,
+                device=self._input_device['name'],
+                channels=num_input_ch,
+                callback=callback,
+            )
+        elif num_output_ch:
+            def callback(outdata, frames, time, status):
+                process_output(outdata)
+            self._stream = sd.OutputStream(
+                samplerate=self.samplerate,
+                blocksize=self.framesize,
+                device=self._output_device['index'],
+                channels=num_output_ch,
+                callback=callback,
+            )
+
+        self._stream.start()
+
+    def stop(self):
+        self._stream.stop()
+
+    def playrec(self, frame=None, framesize=None):
+        outputs = [ch.channel + 1 for ch in self.output_channels]
+        inputs = [ch.channel + 1 for ch in self.input_channels]
+
+        if len(inputs) and len(outputs):
+            return sd.playrec(
+                data=frame.T,
+                samplerate=self.samplerate,
+                device=(self._input_device['index'], self._output_device['index']),
+                input_mapping=inputs,
+                output_mapping=outputs,
+                blocking=True,
+            )
+        elif len(inputs):
+            return sd.rec(
+                frames=framesize,
+                samplerate=self.samplerate,
+                device=self._input_device['index'],
+                mapping=inputs,
+                blocking=True,
+            )
+        elif len(outputs):
+            return sd.play(
+                data=frame.T,
+                samplerate=self.samplerate,
+                device=self._output_device['index'],
+                mapping=outputs,
+                blocking=True,
+            )
+
+    @property
+    def max_inputs(self):
+        return self._input_device['max_input_channels']
+
+    @property
+    def max_outputs(self):
+        return self._output_device['max_output_channels']
+
+
+class NationalInstrumentsConfigurableChannel(SimpleChannel):
+    """A configurable National instruments channel
+
+    Parameters
+    ----------
+    channel : int
+        The index of the channel, zero based.
+    label : str, default None
+        Optional label to assign the channel
+    voltage_range : numeric
+        The range in which to configure the channel.
+        Give a two values (min, max) or a single amplitude value.
+    terminal_config : str, default None
+        How to configure the terminals for the channel. Leave as None to use device default configuration.
+        Should be one of
+        - Differential: for a differential input
+        - Single ended: for a single ended measurement
+    """
+    def __init__(self, channel, label=None, voltage_range=None, terminal_config=None):
+        super().__init__(channel=channel, label=label)
+        self.voltage_range = voltage_range
+        self.terminal_config = terminal_config
+
+    def config(self, interface):
+        configs = {}
+        if self.voltage_range is not None:
+            try:
+                min_val, max_val = self.voltage_range
+            except TypeError:
+                min_val = -self.voltage_range
+                max_val = self.voltage_range
+            configs['min_val'] = min_val
+            configs['max_val'] = max_val
+        if self.terminal_config is not None:
+            if 'diff' in self.terminal_config.lower():
+                configs['terminal_config'] = nidaqmx.constants.TerminalConfiguration.DIFF
+            elif 'single' in self.terminal_config.lower():
+                configs['terminal_config'] = nidaqmx.constants.TerminalConfiguration.RSE
+            else:
+                raise ValueError(f'Unknown terminal configuration {self.terminal_config}')
+        return configs
+
+    def __repr__(self):
+        s = super().__repr__()[:-1]
+        voltage_range = '' if self.voltage_range is None else f', voltage_range={self.voltage_range}'
+        terminal_config = '' if self.terminal_config is None else f', terminal_config={self.terminal_config}'
+        return s + voltage_range + terminal_config + ')'
+
+
+class NationalInstrumentsInputChannel(NationalInstrumentsConfigurableChannel):
+    def config(self, interface):
+        return super().config(interface) | dict(physical_channel=f'{interface.name}/ai{self.channel}')
+
+
+class NationalInstrumentsOutputChannel(NationalInstrumentsConfigurableChannel):
+    def config(self, interface):
+        return super().config(interface) | dict(physical_channel=f'{interface.name}/ao{self.channel}')
+
+
+class NationalInstrumentsDaqmx(_StreamedInterface):
+    @classmethod
+    def list_interfaces(cls):
+        """Check what National Instruments hardware is available.
+
+        Returns
+        -------
+        interfaces : list
+            A list of all devices.
+        """
+        try:
+            system = nidaqmx.system.System.local()
+        except NameError as e:
+            if e.args[0] == "name 'nidaqmx' is not defined":
+                raise ModuleNotFoundError("Windows-only module 'nidaqmx' is not installed")
+            else:
+                raise e
+        name_list = [dev.name for dev in system.devices]
+        return name_list
+
+    def __init__(self, name=None, framesize=None, buffer_n_frames=25, **kwargs):
+        self.name = name or self.list_interfaces()[0]
+        self._device = nidaqmx.system.Device(self.name)
+        self._input_channels = _channel_collection(
+            NationalInstrumentsInputChannel,
+            terminal_config='single ended',
+            voltage_range=(min(self._device.ai_voltage_rngs), max(self._device.ai_voltage_rngs))
+        )
+        self._output_channels = _channel_collection(
+            NationalInstrumentsOutputChannel,
+            voltage_range=(min(self._device.ao_voltage_rngs), max(self._device.ao_voltage_rngs))
+        )
+        super().__init__(**kwargs)
+        self.framesize = framesize
+        self.buffer_n_frames = buffer_n_frames
+
+    def to_dict(self):
+        return super().to_dict() | dict(
+            name=self.name,
+            framesize=self.framesize,
+        )
+
+    @property
+    def samplerate(self):
+        return self._samplerate
+
+    @samplerate.setter
+    def samplerate(self, val):
+        has_in = self.max_inputs > 0
+        has_out = self.max_outputs > 0
+
+        if val is None:
+            if has_in and has_out:
+                fs_in = self._device.ai_max_multi_chan_rate
+                fs_out = self._device.ao_max_rate
+            elif has_in:
+                fs_in = fs_out = self._device.ai_max_multi_chan_rate
+            elif has_out:
+                fs_in = fs_out = self._device.ao_max_rate
+            else:
+                raise ValueError(f'National Instruments interface {self.name} seems to have neither inputs nor outputs')
+        else:
+            try:
+                fs_out, fs_in = val
+            except TypeError:
+                fs_out = fs_in = val
+
+        if has_in:
+            task = nidaqmx.Task()
+            task.ai_channels.add_ai_voltage_chan(self._device.ai_physical_chans[0].name)
+            task.timing.cfg_samp_clk_timing(rate=fs_in)
+            if not fs_in == task.timing.samp_clk_rate:
+                warnings.warn(f'Target input samplerate {fs_in} not available on device, using {task.timing.samp_clk_rate}', stacklevel=2)
+                fs_in = task.timing.samp_clk_rate
+            task.close()
+
+        if has_out:
+            task = nidaqmx.Task()
+            task.ao_channels.add_ao_voltage_chan(self._device.ao_physical_chans[0].name)
+            task.timing.cfg_samp_clk_timing(rate=fs_out)
+            if not fs_out == task.timing.samp_clk_rate:
+                warnings.warn(f'Target output samplerate {fs_out} not available on device, using {task.timing.samp_clk_rate}', stacklevel=3)
+                fs_out = task.timing.samp_clk_rate
+            task.close()
+
+        if fs_out == fs_in:
+            self._samplerate = fs_in
+        else:
+            self._samplerate = (fs_out, fs_in)
+
+    @property
+    def framesize(self):
+        return self._framesize
+
+    @framesize.setter
+    def framesize(self, val):
+        if val is None:
+            fs = self.samplerate
+            try:
+                fs_out, fs_in = fs
+            except TypeError:
+                fs_in = fs_out = fs
+            N_in = fs_in // 50
+            N_out = fs_out // 50
+        else:
+            try:
+                N_out, N_in = val
+            except TypeError:
+                N_out = N_in = val
+
+        if N_out == N_in:
+            self._framesize = N_out
+        else:
+            self._framesize = (N_out, N_in)
+
+    def reset(self, **kwargs):
+        super().reset(**kwargs)
+        try:
+            self._device.reset_device()
+        except (AttributeError, nidaqmx.DaqError):
+            pass
+
+    @property
+    def max_inputs(self):
+        return len(self._device.ai_physical_chans)
+
+    @property
+    def max_outputs(self):
+        return len(self._device.ao_physical_chans)
+
+    def setup(self, finite_samples=False, **kwargs):
+        super().setup(**kwargs)
+
+        if len(self.input_channels):
+            self._input_task = nidaqmx.Task()
+            for ch in self.input_channels:
+                self._input_task.ai_channels.add_ai_voltage_chan(**ch.config(self))
+
+        if len(self.output_channels):
+            self._output_task = nidaqmx.Task()
+            for ch in self.output_channels:
+                self._output_task.ao_channels.add_ao_voltage_chan(**ch.config(self))
+
+        try:
+            samplerate_upstream, samplerate_downstream = self.samplerate
+        except TypeError:
+            samplerate_upstream = samplerate_downstream = self.samplerate
+
+        if finite_samples is False:
+            try:
+                framesize_upstream, framesize_downstream = self.framesize
+            except TypeError:
+                framesize_upstream = framesize_downstream = self.framesize
+            samps_per_chan_read = self.buffer_n_frames * framesize_downstream
+            samps_per_chan_write = self.buffer_n_frames * framesize_upstream
+            sample_mode = nidaqmx.constants.AcquisitionType.CONTINUOUS
+        else:
+            try:
+                samps_per_chan_write, samps_per_chan_read = finite_samples
+            except TypeError:
+                samps_per_chan_write = samps_per_chan_read = finite_samples
+            sample_mode = nidaqmx.constants.AcquisitionType.FINITE
+
+        if len(self.input_channels):
+            self._input_task.timing.cfg_samp_clk_timing(
+                rate=samplerate_downstream,
+                samps_per_chan=samps_per_chan_read,
+                sample_mode=sample_mode
+            )
+            if finite_samples is False:
+                self._databuffer = np.empty((self._input_task.in_stream.num_chans, framesize_downstream))
+                self._read = nidaqmx.stream_readers.AnalogMultiChannelReader(self._input_task.in_stream).read_many_sample
+                self._samples_read = 0
+                self._input_task.in_stream.input_buf_size = framesize_downstream * self.buffer_n_frames
+                self._input_task.register_every_n_samples_acquired_into_buffer_event(framesize_downstream, self._read_callback)
+
+        if len(self.output_channels):
+            self._output_task.timing.cfg_samp_clk_timing(
+                rate=samplerate_upstream,
+                samps_per_chan=samps_per_chan_write,
+                sample_mode=sample_mode
+            )
+
+            if finite_samples is False:
+                self._write = nidaqmx.stream_writers.AnalogMultiChannelWriter(self._output_task.out_stream).write_many_sample
+                self._output_task.out_stream.regen_mode = nidaqmx.constants.RegenerationMode.DONT_ALLOW_REGENERATION
+                self._samples_written = 0
+                self._output_task.out_stream.output_buf_size = framesize_upstream * self.buffer_n_frames
+                self._write_callback(None, None, self.buffer_n_frames * framesize_upstream, None)
+                self._output_task.register_every_n_samples_transferred_from_buffer_event(framesize_upstream, self._write_callback)
+
+        if len(self.output_channels) and len(self.input_channels):
+            self._input_task.triggers.start_trigger.cfg_dig_edge_start_trig(f'/{self.name}/ao/StartTrigger')
+
+
+    def run(self):
+        if not self._is_ready:
+            self.setup()
+
+        if len(self.input_channels):
+            self._input_task.start()
+        if len(self.output_channels):
+            self._output_task.start()
+
+    def stop(self):
+        self._is_ready = False  # The tasks are single use!
+
+        if len(self.output_channels):
+            try:
+                self._output_task.stop()
+                self._output_task.wait_until_done(timeout=10)
+                self._output_task.close()
+            except nidaqmx.DaqError:
+                pass
+
+        if len(self.input_channels):
+            if len(self.output_channels):
+                while self._samples_read < self._samples_written:
+                    time.sleep(self._input_task.in_stream.sleep_time)
+            try:
+                self._input_task.stop()
+                self._input_task.wait_until_done(timeout=10)
+                self._input_task.close()
+            except nidaqmx.DaqError:
+                pass
+
+    def _read_callback(self, task_handle, every_n_samples_event_type, number_of_samples, callback_data):
+        try:
+            self._read(self._databuffer, number_of_samples)
+        except nidaqmx.DaqError:
+            self.stop()
+            raise
+        self._samples_read += number_of_samples
+        self._downstream.push(_core.Frame(self._databuffer.copy()))
+        return 0
+
+    def _write_callback(self, task_handle, every_n_samples_event_type, number_of_samples, callback_data):
+        frame = self._upstream.request(_core.FrameRequest(number_of_samples))
+        self._write(frame.frame)
+        self._samples_written += number_of_samples
+        if isinstance(frame, _core.LastFrame):
+            self._samples_written -= number_of_samples
+            self._samples_written += frame.valid_samples
+            frame = self._write(np.zeros((len(self.output_channels), number_of_samples)))
+            while self._output_task.out_stream.total_samp_per_chan_generated < self._samples_written:
+                time.sleep(self._output_task.out_stream.sleep_time)
+            self.stop()
+        return 0
+
+    def playrec(self, frame=None, framesize=None):
+        if frame is not None:
+            padded_frame = signal_tools.pad_signals(frame, post_pad=1)
+        if framesize is None and len(self.input_channels):
+            try:
+                samplerate_upstream, samplerate_downstream = self.samplerate
+            except TypeError:
+                samplerate_upstream = samplerate_downstream = self.samplerate
+            framesize = np.math.ceil(padded_frame.shape[-1] * samplerate_downstream / samplerate_upstream)
+        self.setup(finite_samples=(padded_frame.shape[-1], framesize), pipeline=True)
+
+        if len(self.input_channels):
+            self._input_task.start()
+
+        if len(self.output_channels):
+            timeout = frame.shape[-1] / samplerate_upstream * 1.2 + 5
+            self._output_task.write(padded_frame.squeeze())
+            self._output_task.start()
+            self._output_task.wait_until_done(timeout=timeout)
+            self._output_task.close()
+
+        if len(self.input_channels):
+            timeout = framesize / samplerate_downstream * 1.2 + 5
+            read_frame = self._input_task.read(framesize, timeout=timeout)
+            read_frame = np.asarray(read_frame)
+            self._input_task.close()
+            return read_frame[..., 1:]
+
+
+class NationalInstrumentsMultimoduleInputChannel(NationalInstrumentsConfigurableChannel):
+    def __init__(self, module, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.module = module
+
+    def __repr__(self):
+        s = super().__repr__()
+        pre, post = s.split('(')
+        return f'{pre}(module={self.module}, {post}'
+
+    def config(self, interface):
+        return interface.input_modules[self.module].ai_physical_chans[self.channel].name
+
+
+class NationalInstrumentsMultimoduleOutputChannel(NationalInstrumentsMultimoduleInputChannel):
+    def config(self, interface):
+        return interface.output_modules[self.module].ao_physical_chans[self.channel].name
+
+
+class CompactDaqmxMultimodule(NationalInstrumentsDaqmx):
+    @classmethod
+    def get_chassis(cls, name=None):
+        devices = cls.list_interfaces()
+        chassis = [dev for dev in devices if 'cDAQ' in dev and 'Mod' not in dev]
+        if name is None:
+            return chassis
+        if name not in chassis:
+            name = [dev for dev in chassis if str(name) in dev][0]
+        return nidaqmx.system.Device(name)
+
+    @classmethod
+    def get_modules(cls, chassis):
+        try:
+            chassis = chassis.name
+        except AttributeError:
+            pass
+        chassis = cls.get_chassis(chassis)
+        devs = cls.list_interfaces()
+        return [nidaqmx.system.Device(dev) for dev in devs if chassis in dev and 'Mod' in dev]
+
+    @classmethod
+    def reset_chassis_modules(cls, chassis):
+        for module in cls.get_modules(chassis):
+            nidaqmx.system.Device(module).reset_device()
+
+    _input_channels = _channel_collection(NationalInstrumentsMultimoduleInputChannel)
+    _output_channels = _channel_collection(NationalInstrumentsMultimoduleOutputChannel)
+
+    def __init__(self, name=None, **kwargs):
+        if name is None:
+            name = self.list_devices()[0]
+        self.chassis = self.get_chassis(name)
+        self.modules = self.get_modules(self.chassis)
+
+        # We need to set a default name for the NIDAQ class to initialize properly
+        if len(self.input_modules) > 0:
+            self.name = self.input_modules[0]
+        elif len(self.output_modules) > 0:
+            self.name = self.output_modules[0]
+        super().__init__(**kwargs)
+        del self.name
+
+        self.input_modules = [module for module in self.modules if len(module.ai_physical_chans) > 0]
+        self.output_modules = [module for module in self.modules if len(module.ao_physical_chans) > 0]
+
+    @property
+    def max_inputs(self):
+        inputs = 0
+        for module in self.input_modules:
+            inputs += len(module.ai_physical_chans)
+        return inputs
+
+    @property
+    def max_outputs(self):
+        outputs = 0
+        for module in self.output_modules:
+            outputs += len(module.ao_physical_chans)
+        return outputs
+
+    def setup(self, **kwargs):
+        super().setup(**kwargs)
+        if len(self.input_channels) and len(self.output_channels):
+            self._output_task.timing.samp_clk_timebase_src = self._input_task.timing.samp_clk_timebase_src
+            self._output_task.timing.samp_clk_timebase_rate = self._input_task.timing.samp_clk_timebase_rate
+
+    def reset(self, **kwargs):
+        super().reset(**kwargs)
+        for module in self.input_modules:
+            module.reset_device()
+        for module in self.output_modules:
+            module.reset_device()
```

### Comparing `acoustics-hardware-0.2.0/acoustics_hardware/signal_tools.py` & `acoustics-hardware-0.2.1/acoustics_hardware/signal_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,111 @@
-import numpy as np
-import fractions
-
-
-def _apply_to_signals(func, signals):
-    if isinstance(signals, np.ndarray):
-        return func(signals)
-    return tuple(func(signal) for signal in signals)
-
-
-def _length_parser(length, samplerate):
-    if isinstance(length, str):
-        if '%' in length:
-            length = float(length.strip('%')) / 100
-            def parser(signal):
-                return round(signal.shape[-1] * length)
-        else:
-            length = fractions.Fraction(length)
-            def parser(signal):
-                return round(signal.shape[-1] * length)
-    else:
-        length = length or 0
-        if samplerate is not None:
-            length = round(samplerate * length)
-        def parser(signal):
-            return length
-    return parser
-
-
-def truncate_signals(signals, length=None, samplerate=None):
-    """Cut signals down to a specified length."""
-    if length is None:
-        return signals
-    if samplerate is not None:
-        length = round(samplerate * length)
-
-    def truncation(signal):
-        return signal[..., :length]
-
-    return _apply_to_signals(truncation, signals)
-
-
-def extend_signals(signals, length=None, samplerate=None):
-    """Zero-pad signals to a certain length.
-
-    Note that this will not shorten signals, so if they are longer
-    than the requested length they will be unchanged.
-    """
-    if length is None:
-        return signals
-    if samplerate is not None:
-        length = round(samplerate * length)
-
-    def extend(signal):
-        padding = length - signal.shape[-1]
-        if padding < 1:
-            return signal.copy()
-        padding = np.zeros(signal.shape[:-1] + (padding,))
-        padded = np.concatenate([signal, padding], axis=-1)
-        return padded
-
-    return _apply_to_signals(extend, signals)
-
-
-def pad_signals(signals, pre_pad=None, post_pad=None, samplerate=None):
-    if pre_pad is None and post_pad is None:
-        return signals
-
-    pre_pad = _length_parser(pre_pad, samplerate)
-    post_pad = _length_parser(post_pad, samplerate)
-    def pad(signal):
-        pre = np.zeros(signal.shape[:-1] + (pre_pad(signal),))
-        post = np.zeros(signal.shape[:-1] + (post_pad(signal),))
-        return np.concatenate([pre, signal, post], axis=-1)
-
-    return _apply_to_signals(pad, signals)
-
-
-def fade_signals(signals, fade_in=None, fade_out=None, samplerate=None, inplace=False):
-    if fade_in is None and fade_out is None:
-        return signals
-
-    fade_in = _length_parser(fade_in, samplerate)
-    fade_out = _length_parser(fade_out, samplerate)
-
-    def fade(signal):
-        if not inplace:
-            signal = signal.copy()
-        in_samples = fade_in(signal)
-        out_samples = fade_out(signal)
-        signal[..., :in_samples] *= np.sin(np.linspace(0, np.pi / 2, in_samples))**2
-        signal[..., -out_samples:] *= np.sin(np.linspace(np.pi / 2, 0, out_samples))**2
-        return signal
-
-    return _apply_to_signals(fade, signals)
-
-
-def nonzero_signals(signals, inplace=False):
-    def nonzero(signal):
-        if not inplace:
-            signal = signal.copy()
-        zero_indices = signal == 0
-        signal[zero_indices] = np.min(np.abs(signal[np.invert(zero_indices)]))
-        return signal
-    return _apply_to_signals(nonzero, signals)
+import numpy as np
+import fractions
+
+
+def _apply_to_signals(func, signals):
+    if isinstance(signals, np.ndarray):
+        return func(signals)
+    try:
+        return tuple(func(signal) for signal in signals)
+    except TypeError as err:
+        if str(err).endswith('object is not iterable'):
+            return func(signals)
+        else:
+            raise
+
+
+def _length_parser(length, samplerate):
+    if isinstance(length, str):
+        if '%' in length:
+            length = float(length.strip('%')) / 100
+            def parser(signal):
+                return round(signal.shape[-1] * length)
+        else:
+            length = fractions.Fraction(length)
+            def parser(signal):
+                return round(signal.shape[-1] * length)
+    else:
+        length = length or 0
+        if samplerate is not None:
+            length = round(samplerate * length)
+        def parser(signal):
+            return length
+    return parser
+
+
+def truncate_signals(signals, length=None, samplerate=None):
+    """Cut signals down to a specified length."""
+    if length is None:
+        return signals
+    if samplerate is not None:
+        length = round(samplerate * length)
+
+    def truncation(signal):
+        return signal[..., :length]
+
+    return _apply_to_signals(truncation, signals)
+
+
+def extend_signals(signals, length=None, samplerate=None):
+    """Zero-pad signals to a certain length.
+
+    Note that this will not shorten signals, so if they are longer
+    than the requested length they will be unchanged.
+    """
+    if length is None:
+        return signals
+    if samplerate is not None:
+        length = round(samplerate * length)
+
+    def extend(signal):
+        padding = length - signal.shape[-1]
+        if padding < 1:
+            return signal.copy()
+        padding = np.zeros(signal.shape[:-1] + (padding,))
+        padded = np.concatenate([signal, padding], axis=-1)
+        return padded
+
+    return _apply_to_signals(extend, signals)
+
+
+def pad_signals(signals, pre_pad=None, post_pad=None, samplerate=None):
+    if pre_pad is None and post_pad is None:
+        return signals
+
+    pre_pad = _length_parser(pre_pad, samplerate)
+    post_pad = _length_parser(post_pad, samplerate)
+    def pad(signal):
+        pre = np.zeros(signal.shape[:-1] + (pre_pad(signal),))
+        post = np.zeros(signal.shape[:-1] + (post_pad(signal),))
+        return np.concatenate([pre, signal, post], axis=-1)
+
+    return _apply_to_signals(pad, signals)
+
+
+def fade_signals(signals, fade_in=None, fade_out=None, samplerate=None, inplace=False):
+    if fade_in is None and fade_out is None:
+        return signals
+
+    fade_in = _length_parser(fade_in, samplerate)
+    fade_out = _length_parser(fade_out, samplerate)
+
+    def fade(signal):
+        if not inplace:
+            signal = signal.copy()
+        in_samples = fade_in(signal)
+        out_samples = fade_out(signal)
+        signal[..., :in_samples] *= np.sin(np.linspace(0, np.pi / 2, in_samples))**2
+        signal[..., -out_samples:] *= np.sin(np.linspace(np.pi / 2, 0, out_samples))**2
+        return signal
+
+    return _apply_to_signals(fade, signals)
+
+
+def nonzero_signals(signals, inplace=False):
+    def nonzero(signal):
+        if not inplace:
+            signal = signal.copy()
+        zero_indices = signal == 0
+        signal[zero_indices] = np.min(np.abs(signal[np.invert(zero_indices)]))
+        return signal
+    return _apply_to_signals(nonzero, signals)
```

### Comparing `acoustics-hardware-0.2.0/acoustics_hardware/timestamps.py` & `acoustics-hardware-0.2.1/acoustics_hardware/timestamps.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import datetime
-import re
-import os
-
-# TODO: make a timestamper class instead of functions?
-
-
-def parse_timestamp(ts):
-    sep = r'[-,_,:,T, ]?'
-
-    year = r'(?P<year>\d{4})'
-    month = r'(?P<month>\d{2})'
-    day = r'(?P<day>\d{2})'
-    hour = r'(?P<hour>\d{2})?'
-    minute = r'(?P<minute>\d{2})?'
-    second = r'(?P<second>\d{2})?'
-    fraction = r'\.?(?P<fraction>\d+)?'
-
-    pattern = sep.join([year, month, day, hour, minute, second]) + fraction
-    regex = re.compile(pattern)
-    match = regex.search(ts)
-    if match is None:
-        raise ValueError(f'Count not parse timestamp {ts}')
-
-    #     raise ValueError(f'Count not parse timestamp {ts}')
-
-    args = []
-    for arg in match.groups():
-        if arg is not None:
-            args.append(int(arg))
-        else:
-            break
-    return datetime.datetime(*args)
-    # TODO: convert the matched strings to ints
-    # TODO: fill two digit year to four digit year
-    # TODO: raise something meaningful on missing info
-    return datetime.datetime(
-        int(groups['year']),
-        int(groups['month']),
-        int(groups['day']),
-        int(groups['hour']),
-        int(groups['minute']),
-        int(groups['second']),
-        int(groups['fraction']),
-    )
-
-
-def timestamp(format='ISO', microseconds=False, utc=False):
-    now = datetime.datetime.now(datetime.timezone.utc)
-    if not utc:
-        now = now.astimezone()
-    if format.lower() == 'iso':
-        return now.isoformat(timespec='microseconds' if microseconds else 'seconds')
-    if format.lower() == 'filename':
-        return now.strftime('%Y-%m-%d_%H-%M-%S' + ('.%f' if microseconds else ''))
-    if format.lower() == 'epoch':
-        return now.timestamp() if microseconds else int(now.timestamp())
-    raise ValueError(f"Unknown timestamp format {format}")
-
-
-def newest_timestamed_filename(directory, n_files=1):
-    return_files = []
-    files = os.listdir(directory)
-    for _ in range(n_files):
-        newest = None
-        for file in files:
-            try:
-                stamp = parse_timestamp(file)
-            except ValueError:
-                continue
-            if newest is None:
-                newest = (file, stamp)
-            elif stamp > newest[1]:
-                newest = (file, stamp)
-        if newest is not None:
-            return_files.append(newest[0])
-            files.remove(file)
-    if len(return_files) < n_files:
-        raise ValueError('No matching files found')
-    if n_files == 1:
-        return return_files[0]
-    return return_files
+import datetime
+import re
+import os
+
+# TODO: make a timestamper class instead of functions?
+
+
+def parse_timestamp(ts):
+    sep = r'[-,_,:,T, ]?'
+
+    year = r'(?P<year>\d{4})'
+    month = r'(?P<month>\d{2})'
+    day = r'(?P<day>\d{2})'
+    hour = r'(?P<hour>\d{2})?'
+    minute = r'(?P<minute>\d{2})?'
+    second = r'(?P<second>\d{2})?'
+    fraction = r'\.?(?P<fraction>\d+)?'
+
+    pattern = sep.join([year, month, day, hour, minute, second]) + fraction
+    regex = re.compile(pattern)
+    match = regex.search(ts)
+    if match is None:
+        raise ValueError(f'Count not parse timestamp {ts}')
+
+    #     raise ValueError(f'Count not parse timestamp {ts}')
+
+    args = []
+    for arg in match.groups():
+        if arg is not None:
+            args.append(int(arg))
+        else:
+            break
+    return datetime.datetime(*args)
+    # TODO: convert the matched strings to ints
+    # TODO: fill two digit year to four digit year
+    # TODO: raise something meaningful on missing info
+    return datetime.datetime(
+        int(groups['year']),
+        int(groups['month']),
+        int(groups['day']),
+        int(groups['hour']),
+        int(groups['minute']),
+        int(groups['second']),
+        int(groups['fraction']),
+    )
+
+
+def timestamp(format='ISO', microseconds=False, utc=False):
+    now = datetime.datetime.now(datetime.timezone.utc)
+    if not utc:
+        now = now.astimezone()
+    if format.lower() == 'iso':
+        return now.isoformat(timespec='microseconds' if microseconds else 'seconds')
+    if format.lower() == 'filename':
+        return now.strftime('%Y-%m-%d_%H-%M-%S' + ('.%f' if microseconds else ''))
+    if format.lower() == 'epoch':
+        return now.timestamp() if microseconds else int(now.timestamp())
+    raise ValueError(f"Unknown timestamp format {format}")
+
+
+def newest_timestamed_filename(directory, n_files=1):
+    return_files = []
+    files = os.listdir(directory)
+    for _ in range(n_files):
+        newest = None
+        for file in files:
+            try:
+                stamp = parse_timestamp(file)
+            except ValueError:
+                continue
+            if newest is None:
+                newest = (file, stamp)
+            elif stamp > newest[1]:
+                newest = (file, stamp)
+        if newest is not None:
+            return_files.append(newest[0])
+            files.remove(file)
+    if len(return_files) < n_files:
+        raise ValueError('No matching files found')
+    if n_files == 1:
+        return return_files[0]
+    return return_files
```

### Comparing `acoustics-hardware-0.2.0/acoustics_hardware.egg-info/PKG-INFO` & `acoustics-hardware-0.2.1/acoustics_hardware.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1
-Name: acoustics-hardware
-Version: 0.2.0
-Summary: Controlling hardware used in acoustic measurement systems
-Home-page: https://github.com/AppliedAcousticsChalmers/acoustics-hardware
-Author: Carl Andersson
-Author-email: carl.andersson@chalmers.se
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-Acoustics Hardware
-==================
-
-This Python package provides a unified interface to serveral hardware platforms used in acoustic measurements, e.g. audio interfaces.
-The purpose of this package is twofold, both to enable cross-hardware interactions with a consistent interface, and to simplify scripting of advanced measurement setups.
-
-Documentation:
-    http://acoustics-hardware.readthedocs.io/
-Source code and issue tracker:
-    https://github.com/AppliedAcousticsChalmers/acoustics-hardware
-
+Metadata-Version: 2.1
+Name: acoustics-hardware
+Version: 0.2.1
+Summary: Controlling hardware used in acoustic measurement systems
+Home-page: https://github.com/AppliedAcousticsChalmers/acoustics-hardware
+Author: Carl Andersson
+Author-email: carl.andersson@chalmers.se
+License: MIT
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Acoustics Hardware
+==================
+
+This Python package provides a unified interface to serveral hardware platforms used in acoustic measurements, e.g. audio interfaces.
+The purpose of this package is twofold, both to enable cross-hardware interactions with a consistent interface, and to simplify scripting of advanced measurement setups.
+
+Documentation:
+    http://acoustics-hardware.readthedocs.io/
+Source code and issue tracker:
+    https://github.com/AppliedAcousticsChalmers/acoustics-hardware
```

### Comparing `acoustics-hardware-0.2.0/acoustics_hardware.egg-info/SOURCES.txt` & `acoustics-hardware-0.2.1/acoustics_hardware.egg-info/SOURCES.txt`

 * *Files identical despite different names*

