# Comparing `tmp/parking-env-0.0.2.tar.gz` & `tmp/parking-env-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parking-env-0.0.2.tar", last modified: Fri May  5 06:59:28 2023, max compression
+gzip compressed data, was "parking-env-0.0.3.tar", last modified: Tue Jul  4 07:47:09 2023, max compression
```

## Comparing `parking-env-0.0.2.tar` & `parking-env-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kexian    (1000) sozne     (1000)        0 2023-05-05 06:59:28.381409 parking-env-0.0.2/
--rw-r--r--   0 kexian    (1000) sozne     (1000)     1067 2023-05-05 06:44:08.000000 parking-env-0.0.2/LICENSE
--rw-r--r--   0 kexian    (1000) sozne     (1000)     1705 2023-05-05 06:59:28.381409 parking-env-0.0.2/PKG-INFO
--rw-r--r--   0 kexian    (1000) sozne     (1000)     1245 2023-05-05 05:24:46.000000 parking-env-0.0.2/README.md
-drwxr-xr-x   0 kexian    (1000) sozne     (1000)        0 2023-05-05 06:59:28.381409 parking-env-0.0.2/parking_env/
--rw-r--r--   0 kexian    (1000) sozne     (1000)      167 2023-05-05 05:29:47.000000 parking-env-0.0.2/parking_env/__init__.py
--rw-r--r--   0 kexian    (1000) sozne     (1000)    13861 2023-05-05 05:29:53.000000 parking-env-0.0.2/parking_env/parking.py
-drwxr-xr-x   0 kexian    (1000) sozne     (1000)        0 2023-05-05 06:59:28.381409 parking-env-0.0.2/parking_env.egg-info/
--rw-r--r--   0 kexian    (1000) sozne     (1000)     1705 2023-05-05 06:59:28.000000 parking-env-0.0.2/parking_env.egg-info/PKG-INFO
--rw-r--r--   0 kexian    (1000) sozne     (1000)      295 2023-05-05 06:59:28.000000 parking-env-0.0.2/parking_env.egg-info/SOURCES.txt
--rw-r--r--   0 kexian    (1000) sozne     (1000)        1 2023-05-05 06:59:28.000000 parking-env-0.0.2/parking_env.egg-info/dependency_links.txt
--rw-r--r--   0 kexian    (1000) sozne     (1000)       62 2023-05-05 06:59:28.000000 parking-env-0.0.2/parking_env.egg-info/entry_points.txt
--rw-r--r--   0 kexian    (1000) sozne     (1000)       35 2023-05-05 06:59:28.000000 parking-env-0.0.2/parking_env.egg-info/requires.txt
--rw-r--r--   0 kexian    (1000) sozne     (1000)       12 2023-05-05 06:59:28.000000 parking-env-0.0.2/parking_env.egg-info/top_level.txt
--rw-r--r--   0 kexian    (1000) sozne     (1000)      650 2023-05-05 06:59:28.381409 parking-env-0.0.2/setup.cfg
--rw-r--r--   0 kexian    (1000) sozne     (1000)      311 2023-04-12 10:57:25.000000 parking-env-0.0.2/setup.py
+drwxr-xr-x   0 kexian    (1000) sozne     (1000)        0 2023-07-04 07:47:09.908387 parking-env-0.0.3/
+-rw-r--r--   0 kexian    (1000) sozne     (1000)     1067 2023-07-04 07:03:14.000000 parking-env-0.0.3/LICENSE
+-rw-r--r--   0 kexian    (1000) sozne     (1000)     2983 2023-07-04 07:47:09.908387 parking-env-0.0.3/PKG-INFO
+-rw-r--r--   0 kexian    (1000) sozne     (1000)     2524 2023-07-04 07:18:12.000000 parking-env-0.0.3/README.md
+drwxr-xr-x   0 kexian    (1000) sozne     (1000)        0 2023-07-04 07:47:09.908387 parking-env-0.0.3/parking_env/
+-rw-r--r--   0 kexian    (1000) sozne     (1000)      167 2023-07-04 07:05:10.000000 parking-env-0.0.3/parking_env/__init__.py
+-rw-r--r--   0 kexian    (1000) sozne     (1000)    13616 2023-07-04 07:31:13.000000 parking-env-0.0.3/parking_env/parking.py
+drwxr-xr-x   0 kexian    (1000) sozne     (1000)        0 2023-07-04 07:47:09.908387 parking-env-0.0.3/parking_env.egg-info/
+-rw-r--r--   0 kexian    (1000) sozne     (1000)     2983 2023-07-04 07:47:09.000000 parking-env-0.0.3/parking_env.egg-info/PKG-INFO
+-rw-r--r--   0 kexian    (1000) sozne     (1000)      295 2023-07-04 07:47:09.000000 parking-env-0.0.3/parking_env.egg-info/SOURCES.txt
+-rw-r--r--   0 kexian    (1000) sozne     (1000)        1 2023-07-04 07:47:09.000000 parking-env-0.0.3/parking_env.egg-info/dependency_links.txt
+-rw-r--r--   0 kexian    (1000) sozne     (1000)       62 2023-07-04 07:47:09.000000 parking-env-0.0.3/parking_env.egg-info/entry_points.txt
+-rw-r--r--   0 kexian    (1000) sozne     (1000)       35 2023-07-04 07:47:09.000000 parking-env-0.0.3/parking_env.egg-info/requires.txt
+-rw-r--r--   0 kexian    (1000) sozne     (1000)       12 2023-07-04 07:47:09.000000 parking-env-0.0.3/parking_env.egg-info/top_level.txt
+-rw-r--r--   0 kexian    (1000) sozne     (1000)      650 2023-07-04 07:47:09.908387 parking-env-0.0.3/setup.cfg
+-rw-r--r--   0 kexian    (1000) sozne     (1000)      311 2023-07-04 07:05:10.000000 parking-env-0.0.3/setup.py
```

### Comparing `parking-env-0.0.2/LICENSE` & `parking-env-0.0.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Kexian Shen
+Copyright (c) 2023 KexianShen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `parking-env-0.0.2/parking_env/parking.py` & `parking-env-0.0.3/parking_env/parking.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,24 +209,21 @@
         self.clock = None
 
     def step(self, action: Union[np.ndarray, int]):
         if action is not None:
             if self.multidiscrete:
                 action = np.array([LON_ACTIONS[action[0]], LAT_ACTIONS[action[1]]])
             elif self.continuous:
-                # action = np.tanh(action)  # C63
-                # action *= STEERING_LIMIT
-                action = np.clip(action, -STEERING_LIMIT, STEERING_LIMIT)
+                action = np.clip(action, -1, 1) * STEERING_LIMIT
                 action = np.array([SPEED_LIMIT, action.item()])
             elif self.multicontinuous:
-                # action = np.tanh(action)  # C63
-                # action[0] *= SPEED_LIMIT
-                # action[1] *= STEERING_LIMIT
-                action[0] = np.clip(action[0], -SPEED_LIMIT, SPEED_LIMIT)
-                action[1] = np.clip(action[1], -STEERING_LIMIT, STEERING_LIMIT)
+                action = np.clip(action, [-1, -1], [1, 1]) * [
+                    SPEED_LIMIT,
+                    STEERING_LIMIT,
+                ]
             else:
                 action = np.array([SPEED_LIMIT, LAT_ACTIONS[action]])
             kinematic_act(action, self.movable[0], DT)
             self.movable_vertices = compute_vertices(self.movable[0])
 
         self.state_rgb_array = self._render("state_rgb_array")
         reward = self._reward()
```

### Comparing `parking-env-0.0.2/setup.cfg` & `parking-env-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = parking-env
-version = 0.0.2
+version = 0.0.3
 author = Kexian Shen
 author_email = shenkexian@gmail.com
 description = An environment for simulated parking lot tasks.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/kexianshen/parking-env
 license = MIT
```

