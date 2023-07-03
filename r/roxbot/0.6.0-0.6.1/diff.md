# Comparing `tmp/roxbot-0.6.0.tar.gz` & `tmp/roxbot-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.6.0.tar", last modified: Mon Jul  3 19:39:03 2023, max compression
+gzip compressed data, was "roxbot-0.6.1.tar", last modified: Mon Jul  3 21:54:13 2023, max compression
```

## Comparing `roxbot-0.6.0.tar` & `roxbot-0.6.1.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:39:03.326428 roxbot-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-03 19:38:52.000000 roxbot-0.6.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-03 19:39:03.326428 roxbot-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-03 19:38:52.000000 roxbot-0.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-03 19:39:03.326428 roxbot-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-03 19:38:52.000000 roxbot-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:39:03.319428 roxbot-0.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:39:03.322428 roxbot-0.6.0/src/roxbot/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/base_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:39:03.324428 roxbot-0.6.0/src/roxbot/bridges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/bridges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/bridges/web_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/gps.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     8990 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:39:03.324428 roxbot-0.6.0/src/roxbot/simulators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/simulators/trike.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-03 19:38:52.000000 roxbot-0.6.0/src/roxbot/vectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:39:03.323428 roxbot-0.6.0/src/roxbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-03 19:39:03.000000 roxbot-0.6.0/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-03 19:39:03.000000 roxbot-0.6.0/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 19:39:03.000000 roxbot-0.6.0/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-03 19:39:03.000000 roxbot-0.6.0/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 19:38:55.000000 roxbot-0.6.0/src/roxbot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-03 19:39:03.000000 roxbot-0.6.0/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-03 19:39:03.000000 roxbot-0.6.0/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 19:39:03.326428 roxbot-0.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-03 19:38:52.000000 roxbot-0.6.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-03 19:38:52.000000 roxbot-0.6.0/tests/test_gps.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-03 19:38:52.000000 roxbot-0.6.0/tests/test_interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-03 19:38:52.000000 roxbot-0.6.0/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-03 19:38:52.000000 roxbot-0.6.0/tests/test_trike.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-03 19:38:52.000000 roxbot-0.6.0/tests/test_trike_sim.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-03 19:38:52.000000 roxbot-0.6.0/tests/test_vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-03 19:38:52.000000 roxbot-0.6.0/tests/test_ws_bridge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:54:13.150726 roxbot-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-03 21:54:02.000000 roxbot-0.6.1/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-03 21:54:13.150726 roxbot-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-03 21:54:02.000000 roxbot-0.6.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-03 21:54:13.151726 roxbot-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-03 21:54:02.000000 roxbot-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:54:13.144726 roxbot-0.6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:54:13.147726 roxbot-0.6.1/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/base_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:54:13.149726 roxbot-0.6.1/src/roxbot/bridges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/bridges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/bridges/web_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     8920 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:54:13.149726 roxbot-0.6.1/src/roxbot/simulators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/simulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-03 21:54:02.000000 roxbot-0.6.1/src/roxbot/vectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:54:13.148726 roxbot-0.6.1/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-03 21:54:13.000000 roxbot-0.6.1/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-03 21:54:13.000000 roxbot-0.6.1/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:54:13.000000 roxbot-0.6.1/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-03 21:54:13.000000 roxbot-0.6.1/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:54:05.000000 roxbot-0.6.1/src/roxbot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-03 21:54:13.000000 roxbot-0.6.1/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-03 21:54:13.000000 roxbot-0.6.1/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:54:13.150726 roxbot-0.6.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-03 21:54:02.000000 roxbot-0.6.1/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-03 21:54:02.000000 roxbot-0.6.1/tests/test_gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-03 21:54:02.000000 roxbot-0.6.1/tests/test_interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-03 21:54:02.000000 roxbot-0.6.1/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-03 21:54:02.000000 roxbot-0.6.1/tests/test_trike.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-03 21:54:02.000000 roxbot-0.6.1/tests/test_vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-03 21:54:02.000000 roxbot-0.6.1/tests/test_ws_bridge.py
```

### Comparing `roxbot-0.6.0/LICENCE` & `roxbot-0.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/README.md` & `roxbot-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/setup.py` & `roxbot-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/src/roxbot/base_classes.py` & `roxbot-0.6.1/src/roxbot/base_classes.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/src/roxbot/bridges/web_bridge.py` & `roxbot-0.6.1/src/roxbot/bridges/web_bridge.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/src/roxbot/gps.py` & `roxbot-0.6.1/src/roxbot/gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/src/roxbot/models.py` & `roxbot-0.6.1/src/roxbot/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,18 +290,15 @@
 
         # update steering wheel
         self.steer.step(dt)
 
         # update driving wheel targets
         for wheel, target in zip(self.wheels, self.wheel_targets):
             wheel.set_velocity_ms(target)
-
-        # update driving wheels
-        self.wheels[0].step(dt)
-        self.wheels[1].step(dt)
+            wheel.step(dt)
 
         # update position
 
         # linear distance travelled
         dS = (self.wheels[0].ds + self.wheels[1].ds) / 2
 
         # update heading
```

### Comparing `roxbot-0.6.0/src/roxbot/vectors.py` & `roxbot-0.6.1/src/roxbot/vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/src/roxbot.egg-info/SOURCES.txt` & `roxbot-0.6.1/src/roxbot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 src/roxbot.egg-info/entry_points.txt
 src/roxbot.egg-info/not-zip-safe
 src/roxbot.egg-info/requires.txt
 src/roxbot.egg-info/top_level.txt
 src/roxbot/bridges/__init__.py
 src/roxbot/bridges/web_bridge.py
 src/roxbot/simulators/__init__.py
-src/roxbot/simulators/trike.py
 tests/test_cli.py
 tests/test_gps.py
 tests/test_interfaces.py
 tests/test_models.py
 tests/test_trike.py
-tests/test_trike_sim.py
 tests/test_vectors.py
 tests/test_ws_bridge.py
```

### Comparing `roxbot-0.6.0/tests/test_gps.py` & `roxbot-0.6.1/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/tests/test_models.py` & `roxbot-0.6.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/tests/test_trike.py` & `roxbot-0.6.1/tests/test_trike.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/tests/test_vectors.py` & `roxbot-0.6.1/tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.6.0/tests/test_ws_bridge.py` & `roxbot-0.6.1/tests/test_ws_bridge.py`

 * *Files identical despite different names*

