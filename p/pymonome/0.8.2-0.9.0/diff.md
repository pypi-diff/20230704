# Comparing `tmp/pymonome-0.8.2.tar.gz` & `tmp/pymonome-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymonome-0.8.2.tar", last modified: Fri Feb 27 06:17:01 2015, max compression
+gzip compressed data, was "dist/pymonome-0.9.0.tar", last modified: Mon Oct 30 13:26:17 2017, max compression
```

## Comparing `pymonome-0.8.2.tar` & `pymonome-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 art       (1000) art       (1000)        0 2015-02-27 06:17:01.000000 pymonome-0.8.2/
-drwxrwxr-x   0 art       (1000) art       (1000)        0 2015-02-27 06:17:01.000000 pymonome-0.8.2/examples/
--rw-rw-rw-   0 art       (1000) art       (1000)     1670 2014-08-10 15:57:46.000000 pymonome-0.8.2/examples/faders.py
--rw-rw-rw-   0 art       (1000) art       (1000)      725 2015-01-25 18:28:58.000000 pymonome-0.8.2/examples/monobright.py
--rw-rw-r--   0 art       (1000) art       (1000)     1266 2015-01-25 18:29:14.000000 pymonome-0.8.2/examples/lights.py
--rw-rw-rw-   0 art       (1000) art       (1000)      365 2015-01-25 18:26:20.000000 pymonome-0.8.2/examples/hello.py
--rw-rw-rw-   0 art       (1000) art       (1000)     1523 2015-01-25 18:44:12.000000 pymonome-0.8.2/examples/pages.py
--rw-rw-rw-   0 art       (1000) art       (1000)     2623 2014-08-10 14:14:00.000000 pymonome-0.8.2/examples/bridge.py
--rw-rw-rw-   0 art       (1000) art       (1000)     2193 2015-01-25 18:39:55.000000 pymonome-0.8.2/examples/life.py
--rw-rw-r--   0 art       (1000) art       (1000)      146 2015-02-27 06:10:08.000000 pymonome-0.8.2/CHANGES.txt
-drwxrwxr-x   0 art       (1000) art       (1000)        0 2015-02-27 06:17:01.000000 pymonome-0.8.2/pymonome.egg-info/
--rw-rw-r--   0 art       (1000) art       (1000)      353 2015-02-27 06:17:01.000000 pymonome-0.8.2/pymonome.egg-info/SOURCES.txt
--rw-rw-r--   0 art       (1000) art       (1000)        7 2015-02-27 06:17:00.000000 pymonome-0.8.2/pymonome.egg-info/top_level.txt
--rw-rw-r--   0 art       (1000) art       (1000)        1 2015-02-27 06:17:00.000000 pymonome-0.8.2/pymonome.egg-info/dependency_links.txt
--rw-rw-r--   0 art       (1000) art       (1000)        6 2015-02-27 06:17:00.000000 pymonome-0.8.2/pymonome.egg-info/requires.txt
--rw-rw-r--   0 art       (1000) art       (1000)     1048 2015-02-27 06:17:00.000000 pymonome-0.8.2/pymonome.egg-info/PKG-INFO
--rw-rw-r--   0 art       (1000) art       (1000)       59 2015-02-27 06:17:01.000000 pymonome-0.8.2/setup.cfg
--rw-rw-rw-   0 art       (1000) art       (1000)    17381 2015-02-27 06:06:32.000000 pymonome-0.8.2/monome.py
--rw-rw-rw-   0 art       (1000) art       (1000)       77 2015-02-05 16:05:28.000000 pymonome-0.8.2/MANIFEST.in
--rw-rw-r--   0 art       (1000) art       (1000)      807 2015-02-27 06:09:38.000000 pymonome-0.8.2/setup.py
--rw-rw-r--   0 art       (1000) art       (1000)      393 2015-02-07 04:18:03.000000 pymonome-0.8.2/README.rst
--rw-rw-r--   0 art       (1000) art       (1000)     1048 2015-02-27 06:17:01.000000 pymonome-0.8.2/PKG-INFO
--rw-rw-r--   0 art       (1000) art       (1000)     1096 2014-07-20 12:07:47.000000 pymonome-0.8.2/LICENSE
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2017-10-30 13:26:17.000000 pymonome-0.9.0/
+-rw-r--r--   0 art       (1000) art       (1000)      807 2017-10-29 16:54:42.000000 pymonome-0.9.0/setup.py
+-rw-rw-r--   0 art       (1000) art       (1000)      393 2015-02-07 04:18:03.000000 pymonome-0.9.0/README.rst
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2017-10-30 13:26:17.000000 pymonome-0.9.0/pymonome.egg-info/
+-rw-rw-r--   0 art       (1000) art       (1000)      355 2017-10-30 13:26:17.000000 pymonome-0.9.0/pymonome.egg-info/SOURCES.txt
+-rw-rw-r--   0 art       (1000) art       (1000)        7 2017-10-30 13:26:17.000000 pymonome-0.9.0/pymonome.egg-info/top_level.txt
+-rw-rw-r--   0 art       (1000) art       (1000)        1 2017-10-30 13:26:17.000000 pymonome-0.9.0/pymonome.egg-info/dependency_links.txt
+-rw-rw-r--   0 art       (1000) art       (1000)     1048 2017-10-30 13:26:17.000000 pymonome-0.9.0/pymonome.egg-info/PKG-INFO
+-rw-rw-r--   0 art       (1000) art       (1000)        6 2017-10-30 13:26:17.000000 pymonome-0.9.0/pymonome.egg-info/requires.txt
+-rw-r--r--   0 art       (1000) art       (1000)    21836 2017-10-29 16:54:42.000000 pymonome-0.9.0/monome.py
+-rw-rw-r--   0 art       (1000) art       (1000)     1096 2014-07-20 12:07:47.000000 pymonome-0.9.0/LICENSE
+-rw-r--r--   0 art       (1000) art       (1000)       38 2017-10-30 13:26:17.000000 pymonome-0.9.0/setup.cfg
+-rw-rw-r--   0 art       (1000) art       (1000)       77 2015-02-05 16:05:28.000000 pymonome-0.9.0/MANIFEST.in
+-rw-rw-r--   0 art       (1000) art       (1000)      146 2015-02-27 06:10:08.000000 pymonome-0.9.0/CHANGES.txt
+-rw-r--r--   0 art       (1000) art       (1000)     1048 2017-10-30 13:26:17.000000 pymonome-0.9.0/PKG-INFO
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2017-10-30 13:26:17.000000 pymonome-0.9.0/examples/
+-rw-r--r--   0 art       (1000) art       (1000)      703 2017-10-09 14:40:47.000000 pymonome-0.9.0/examples/monobright.py
+-rw-r--r--   0 art       (1000) art       (1000)     1174 2017-10-29 16:54:42.000000 pymonome-0.9.0/examples/splitter.py
+-rw-r--r--   0 art       (1000) art       (1000)     2470 2017-10-29 16:54:42.000000 pymonome-0.9.0/examples/life.py
+-rw-r--r--   0 art       (1000) art       (1000)     1229 2017-10-09 14:41:41.000000 pymonome-0.9.0/examples/lights.py
+-rw-r--r--   0 art       (1000) art       (1000)     1089 2017-10-29 16:54:42.000000 pymonome-0.9.0/examples/pages.py
+-rw-r--r--   0 art       (1000) art       (1000)     1683 2017-10-29 16:54:42.000000 pymonome-0.9.0/examples/faders.py
+-rw-r--r--   0 art       (1000) art       (1000)      343 2017-10-29 16:54:42.000000 pymonome-0.9.0/examples/hello.py
```

### Comparing `pymonome-0.8.2/examples/faders.py` & `pymonome-0.9.0/examples/faders.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,51 +2,50 @@
 
 import random
 import asyncio
 import monome
 
 FADERS_MAX_VALUE = 100
 
-class Faders(monome.Monome):
+class Faders(monome.App):
     def __init__(self):
-        super().__init__('/faders')
+        super().__init__() # TODO: prefix
 
-    def ready(self):
-        self.led_all(0)
-        self.led_row(0, self.height - 1, [1] * self.width)
+    def on_grid_ready(self):
+        self.grid.led_all(0)
 
         self.row_values = []
         row_value = 0
-        for i in range(self.height):
+        for i in range(self.grid.height):
             self.row_values.append(int(round(row_value)))
-            row_value += FADERS_MAX_VALUE / (self.height - 1)
+            row_value += FADERS_MAX_VALUE / (self.grid.height - 1)
 
-        self.values = [random.randint(0, FADERS_MAX_VALUE) for f in range(self.width)]
-        self.faders = [asyncio.async(self.fade_to(f, 0)) for f in range(self.width)]
+        self.values = [random.randint(0, FADERS_MAX_VALUE) for f in range(self.grid.width)]
+        self.faders = [asyncio.async(self.fade_to(f, 0)) for f in range(self.grid.width)]
 
-    def grid_key(self, x, y, s):
+    def on_grid_key(self, x, y, s):
         if s == 1:
             self.faders[x].cancel()
             self.faders[x] = asyncio.async(self.fade_to(x, self.row_to_value(y)))
 
     def value_to_row(self, value):
-        return sorted([i for i in range(self.height)], key=lambda i: abs(self.row_values[i] - value))[0]
+        return sorted([i for i in range(self.grid.height)], key=lambda i: abs(self.row_values[i] - value))[0]
 
     def row_to_value(self, row):
-        return self.row_values[self.height - 1 - row]
+        return self.row_values[self.grid.height - 1 - row]
 
-    @asyncio.coroutine
-    def fade_to(self, x, new_value):
+    async def fade_to(self, x, new_value):
         while self.values[x] != new_value:
             if self.values[x] < new_value:
                 self.values[x] += 1
             else:
                 self.values[x] -= 1
-            col = [0 if c > self.value_to_row(self.values[x]) else 1 for c in range(self.height)]
+            col = [0 if c > self.value_to_row(self.values[x]) else 1 for c in range(self.grid.height)]
             col.reverse()
-            self.led_col(x, 0, col)
-            yield from asyncio.sleep(1/100)
+            self.grid.led_col(x, 0, col)
+            await asyncio.sleep(1/100)
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
-    asyncio.async(monome.create_serialosc_connection(Faders), loop=loop)
+    faders_app = Faders()
+    asyncio.async(monome.SerialOsc.create(loop=loop, autoconnect_app=faders_app))
     loop.run_forever()
```

### Comparing `pymonome-0.8.2/examples/monobright.py` & `pymonome-0.9.0/examples/monobright.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 import asyncio
 import monome
 
 class Monobright(monome.Monome):
     def __init__(self):
         super().__init__('/hello', varibright=False)
 
-    @asyncio.coroutine
-    def light(self, x, y):
+    async def light(self, x, y):
         for i in range(16):
             self.led_level_set(x, y, i)
-            yield from asyncio.sleep(0.1)
+            await asyncio.sleep(0.1)
 
     def grid_key(self, x, y, s):
         if s == 1:
             asyncio.async(self.light(x, y))
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
```

### Comparing `pymonome-0.8.2/examples/lights.py` & `pymonome-0.9.0/examples/lights.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,26 @@
         if s == 1:
             self.led_set(x, y, s)
 
     def disconnect(self, *args):
         self.alive = False
         super().disconnect(*args)
 
-    @asyncio.coroutine
-    def animate(self):
+    async def animate(self):
         while self.alive:
             for i in range(self.height):
                 row = [random.randint(0, 1) for i in range(self.width)]
                 for j in range(3):
                     self.led_row(0, i, [0] * self.width)
-                    yield from asyncio.sleep(1 / 30)
+                    await asyncio.sleep(1 / 30)
                     self.led_row(0, i, row)
-                    yield from asyncio.sleep(1 / 30)
+                    await asyncio.sleep(1 / 30)
             for i in reversed(range(self.height)):
                 row = [random.randint(0, 1) for i in range(self.width)]
                 self.led_row(0, i, row)
-                yield from asyncio.sleep(1 / 20)
-            yield from asyncio.sleep(2)
+                await asyncio.sleep(1 / 20)
+            await asyncio.sleep(2)
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
     asyncio.async(monome.create_serialosc_connection(Lights), loop=loop)
     loop.run_forever()
```

### Comparing `pymonome-0.8.2/pymonome.egg-info/PKG-INFO` & `pymonome-0.9.0/pymonome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pymonome
-Version: 0.8.2
+Version: 0.9.0
 Summary: a monome serialosc client in python
 Home-page: https://github.com/artfwo/pymonome
 Author: Artem Popov
 Author-email: artfwo@gmail.com
 License: MIT
 Description: ========
         pymonome
```

### Comparing `pymonome-0.8.2/setup.py` & `pymonome-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(
     name='pymonome',
     author='Artem Popov',
     author_email='artfwo@gmail.com',
     url='https://github.com/artfwo/pymonome',
     description='a monome serialosc client in python',
     long_description=long_description,
-    version='0.8.2',
+    version='0.9.0',
     py_modules=['monome'],
     include_package_data=True,
     install_requires=[
         'aiosc'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `pymonome-0.8.2/PKG-INFO` & `pymonome-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pymonome
-Version: 0.8.2
+Version: 0.9.0
 Summary: a monome serialosc client in python
 Home-page: https://github.com/artfwo/pymonome
 Author: Artem Popov
 Author-email: artfwo@gmail.com
 License: MIT
 Description: ========
         pymonome
```

### Comparing `pymonome-0.8.2/LICENSE` & `pymonome-0.9.0/LICENSE`

 * *Files identical despite different names*

