# Comparing `tmp/roxbot-0.6.2.tar.gz` & `tmp/roxbot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.6.2.tar", last modified: Mon Jul  3 21:58:37 2023, max compression
+gzip compressed data, was "roxbot-0.7.0.tar", last modified: Tue Jul  4 12:03:20 2023, max compression
```

## Comparing `roxbot-0.6.2.tar` & `roxbot-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:58:37.825610 roxbot-0.6.2/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-03 21:58:25.000000 roxbot-0.6.2/LICENCE
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-03 21:58:37.826610 roxbot-0.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-03 21:58:25.000000 roxbot-0.6.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-03 21:58:37.826610 roxbot-0.6.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-03 21:58:25.000000 roxbot-0.6.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:58:37.817610 roxbot-0.6.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:58:37.821610 roxbot-0.6.2/src/roxbot/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/base_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:58:37.823610 roxbot-0.6.2/src/roxbot/bridges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/bridges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/bridges/web_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/gps.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     9063 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:58:37.824610 roxbot-0.6.2/src/roxbot/simulators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-03 21:58:25.000000 roxbot-0.6.2/src/roxbot/vectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:58:37.823610 roxbot-0.6.2/src/roxbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-03 21:58:37.000000 roxbot-0.6.2/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      715 2023-07-03 21:58:37.000000 roxbot-0.6.2/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:58:37.000000 roxbot-0.6.2/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-03 21:58:37.000000 roxbot-0.6.2/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:58:29.000000 roxbot-0.6.2/src/roxbot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-03 21:58:37.000000 roxbot-0.6.2/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-03 21:58:37.000000 roxbot-0.6.2/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:58:37.825610 roxbot-0.6.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-03 21:58:25.000000 roxbot-0.6.2/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-03 21:58:25.000000 roxbot-0.6.2/tests/test_gps.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-03 21:58:25.000000 roxbot-0.6.2/tests/test_interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-03 21:58:25.000000 roxbot-0.6.2/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-03 21:58:25.000000 roxbot-0.6.2/tests/test_trike.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-03 21:58:25.000000 roxbot-0.6.2/tests/test_vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-03 21:58:25.000000 roxbot-0.6.2/tests/test_ws_bridge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.177186 roxbot-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-04 12:03:08.000000 roxbot-0.7.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-04 12:03:20.177186 roxbot-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-04 12:03:08.000000 roxbot-0.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-04 12:03:20.178187 roxbot-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-04 12:03:08.000000 roxbot-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.170186 roxbot-0.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.173186 roxbot-0.7.0/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/base_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.175186 roxbot-0.7.0/src/roxbot/bridges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/bridges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/bridges/web_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9200 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.175186 roxbot-0.7.0/src/roxbot/simulators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/simulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-04 12:03:08.000000 roxbot-0.7.0/src/roxbot/vectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.175186 roxbot-0.7.0/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 12:03:11.000000 roxbot-0.7.0/src/roxbot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 12:03:20.000000 roxbot-0.7.0/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 12:03:20.177186 roxbot-0.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_trike.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-04 12:03:08.000000 roxbot-0.7.0/tests/test_ws_bridge.py
```

### Comparing `roxbot-0.6.2/LICENCE` & `roxbot-0.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/README.md` & `roxbot-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/setup.py` & `roxbot-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/src/roxbot/base_classes.py` & `roxbot-0.7.0/src/roxbot/base_classes.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/src/roxbot/bridges/web_bridge.py` & `roxbot-0.7.0/src/roxbot/bridges/web_bridge.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/src/roxbot/gps.py` & `roxbot-0.7.0/src/roxbot/gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/src/roxbot/models.py` & `roxbot-0.7.0/src/roxbot/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,17 +240,22 @@
         return (self.wheels[0].velocity_ms + self.wheels[1].velocity_ms) / 2
 
     @property
     def steering_angle(self) -> float:
         """steering angle in radians"""
         return self.steer.val
 
-    @steering_angle.setter
-    def steering_angle(self, angle: float) -> None:
-        """set steering angle in radians"""
+    @property
+    def target_steer(self) -> float:
+        """target steering angle in radians"""
+        return self.steer.setpoint
+
+    @target_steer.setter
+    def target_steer(self, angle: float) -> None:
+        """set target steering angle in radians"""
         self.steer.setpoint = angle
 
     @property
     def curvature(self) -> float:
         """driving curvature"""
         return math.tan(self.steering_angle) / self.L
```

### Comparing `roxbot-0.6.2/src/roxbot/vectors.py` & `roxbot-0.7.0/src/roxbot/vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/src/roxbot.egg-info/SOURCES.txt` & `roxbot-0.7.0/src/roxbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/tests/test_gps.py` & `roxbot-0.7.0/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/tests/test_models.py` & `roxbot-0.7.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/tests/test_trike.py` & `roxbot-0.7.0/tests/test_trike.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,74 +16,74 @@
     return TrikeModel(-1.0, 1.0, wheel_accel=1e6, steer_speed=1e6)
 
 
 def test_curvature_calc():
     m = create_trike()
 
     # straight line
-    m.steering_angle = 0.0
+    m.target_steer = 0.0
     m.step(DT)
     assert m.steering_angle == 0.0
     assert m.curvature == 0.0
 
     # 45 deg turn
-    m.steering_angle = radians(45)
+    m.target_steer = radians(45)
     m.step(DT)
     assert m.curvature == approx(-1)
 
     # -45 deg turn
-    m.steering_angle = radians(-45)
+    m.target_steer = radians(-45)
     m.step(DT)
     assert m.curvature == approx(1)
 
 
 def test_velocity_calc():
     m = create_trike()
 
     # straight line
-    m.steering_angle = 0.0
+    m.target_steer = 0.0
     m.target_velocity = 1.0
     m.step(DT)
     assert m.velocity == 1.0
 
     vels = m.wheel_targets
     assert vels[0] == approx(1.0)
     assert vels[1] == approx(1.0)
 
     # 45 deg turn
-    m.steering_angle = radians(45)
+    m.target_steer = radians(45)
     m.step(DT)
     vl, vr = m.wheel_targets
     assert vl == approx(1.5)
     assert vr == approx(0.5)
 
     # other angle
-    m.steering_angle = radians(30.07)
+    m.target_steer = radians(30.07)
     m.step(DT)
     vl, vr = m.wheel_targets
     assert vl == approx(1.289, abs=0.01)
     assert vr == approx(0.711, abs=0.01)
 
     # other angle
-    m.steering_angle = radians(-20.025)
+    m.target_steer = radians(-20.025)
     m.step(DT)
     vl, vr = m.wheel_targets
     assert vl == approx(0.818, abs=0.01)
     assert vr == approx(1.182, abs=0.01)
 
     # slow down
     m.target_velocity = 0.5
-    m.steering_angle = radians(-45)
+    m.target_steer = radians(-45)
     m.step(DT)
     assert m.curvature == approx(1, abs=0.001)
     vl, vr = m.wheel_targets
     assert vl == approx(0.25)
     assert vr == approx(0.75)
 
 
 def test_steering_angle():
     m = create_trike()
 
     m.target_velocity = 1.0
-    m.steering_angle = 0.5
+    m.target_steer = 0.5
     m.step(DT)
     assert m.steering_angle == 0.5
```

### Comparing `roxbot-0.6.2/tests/test_vectors.py` & `roxbot-0.7.0/tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.2/tests/test_ws_bridge.py` & `roxbot-0.7.0/tests/test_ws_bridge.py`

 * *Files identical despite different names*

