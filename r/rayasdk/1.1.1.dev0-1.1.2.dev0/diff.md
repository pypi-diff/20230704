# Comparing `tmp/rayasdk-1.1.1.dev0.tar.gz` & `tmp/rayasdk-1.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-1.1.1.dev0.tar", last modified: Thu Jun  8 21:03:00 2023, max compression
+gzip compressed data, was "rayasdk-1.1.2.dev0.tar", last modified: Tue Jul  4 20:59:55 2023, max compression
```

## Comparing `rayasdk-1.1.1.dev0.tar` & `rayasdk-1.1.2.dev0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:03:00.478422 rayasdk-1.1.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-08 21:03:00.478422 rayasdk-1.1.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:03:00.478422 rayasdk-1.1.1.dev0/rayasdk/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5706 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:03:00.478422 rayasdk-1.1.1.dev0/rayasdk/container_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/container_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/container_handlers/docker_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/executioner_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/killer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/sshKeyGen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:03:00.478422 rayasdk-1.1.1.dev0/rayasdk/template/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/template/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/template/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/template/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/template/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/rayasdk/vcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:03:00.478422 rayasdk-1.1.1.dev0/rayasdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-08 21:03:00.000000 rayasdk-1.1.1.dev0/rayasdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-08 21:03:00.000000 rayasdk-1.1.1.dev0/rayasdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:03:00.000000 rayasdk-1.1.1.dev0/rayasdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 21:03:00.000000 rayasdk-1.1.1.dev0/rayasdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-08 21:03:00.000000 rayasdk-1.1.1.dev0/rayasdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 21:03:00.000000 rayasdk-1.1.1.dev0/rayasdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 21:03:00.478422 rayasdk-1.1.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 21:02:47.000000 rayasdk-1.1.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.604219 rayasdk-1.1.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-04 20:59:55.604219 rayasdk-1.1.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.600219 rayasdk-1.1.2.dev0/rayasdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5706 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.600219 rayasdk-1.1.2.dev0/rayasdk/container_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/container_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/container_handlers/docker_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/executioner_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/killer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/sshKeyGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.604219 rayasdk-1.1.2.dev0/rayasdk/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/template/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/template/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/template/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/template/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/vcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.600219 rayasdk-1.1.2.dev0/rayasdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 20:59:55.604219 rayasdk-1.1.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/setup.py
```

### Comparing `rayasdk-1.1.1.dev0/PKG-INFO` & `rayasdk-1.1.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.1.dev0
+Version: 1.1.2.dev0
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: 
 Download-URL: 
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
```

### Comparing `rayasdk-1.1.1.dev0/README.md` & `rayasdk-1.1.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/__init__.py` & `rayasdk-1.1.2.dev0/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/__main__.py` & `rayasdk-1.1.2.dev0/rayasdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/connect.py` & `rayasdk-1.1.2.dev0/rayasdk/connect.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/constants.py` & `rayasdk-1.1.2.dev0/rayasdk/constants.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/container_handlers/docker_handler.py` & `rayasdk-1.1.2.dev0/rayasdk/container_handlers/docker_handler.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/executioner_command.py` & `rayasdk-1.1.2.dev0/rayasdk/executioner_command.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/initializer.py` & `rayasdk-1.1.2.dev0/rayasdk/initializer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/killer.py` & `rayasdk-1.1.2.dev0/rayasdk/killer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/logger.py` & `rayasdk-1.1.2.dev0/rayasdk/logger.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/messages.py` & `rayasdk-1.1.2.dev0/rayasdk/messages.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/runner.py` & `rayasdk-1.1.2.dev0/rayasdk/runner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/scanner.py` & `rayasdk-1.1.2.dev0/rayasdk/scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,36 +20,45 @@
     def __init__(self):
         pass
 
 
     def init_parser(self, subparser):
         self.parser = subparser.add_parser(
             type(self).COMMAND, help='Discover robots in the local network.')
+        self.parser.add_argument(
+            '-t','--time',
+            help='Total time that execute the scan',
+        )
 
 
     def __save_last_scan(self, path):
         global robots_info
-        if len(robots_info) > 0:
-            with open(path, 'w', encoding='utf-8') as f:
-                all_robots = dict()
-                for robot in robots_info:
-                    for index, info_robot in robots_info[robot].items():
-                        key = f'{index}_{robot}'
-                        all_robots[key] = info_robot
+        with open(path, 'w', encoding='utf-8') as f:
+            all_robots = dict()
+            if len(robots_info) == 0:
                 json.dump(all_robots, f, ensure_ascii=False, indent=4)
-                return True
-        return False
+                return False
+            
+            for robot in robots_info:
+                for index, info_robot in robots_info[robot].items():
+                    key = f'{index}_{robot}'
+                    all_robots[key] = info_robot
+            json.dump(all_robots, f, ensure_ascii=False, indent=4)
+        return True
 
 
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
         zeroconf = Zeroconf()
         listener = MyListener(print=True)
         ServiceBrowser(Zeroconf(), '_gary-robot._tcp.local.', listener)
+        seconds_to_scan = None
+        if self.args.time:
+            seconds_to_scan = int(self.args.time)
         try:
             update_table()
             while True:
                 if select.select([sys.stdin,], [], [], 0.0)[0]:
                     input_str = sys.stdin.readline().strip()
                     if input_str == '':
                         break
@@ -60,14 +69,20 @@
                         zc=zero,
                         type_='_gary-robot._tcp.local.',
                         listener=listener
                     )
                 time.sleep(1)
                 browser.cancel()
                 zero.close()
+                
+                self.__save_last_scan(path=constants.LAST_SCANNING_PATH)
+                if seconds_to_scan is not None:
+                    seconds_to_scan -= 1
+                    if seconds_to_scan <= 0:
+                        raise KeyboardInterrupt
         except KeyboardInterrupt:
             pass
         finally:
             zeroconf.close()
 
         try:
             if not self.__save_last_scan(path=constants.LAST_SCANNING_PATH):
```

### Comparing `rayasdk-1.1.1.dev0/rayasdk/simulator.py` & `rayasdk-1.1.2.dev0/rayasdk/simulator.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/sshKeyGen.py` & `rayasdk-1.1.2.dev0/rayasdk/sshKeyGen.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/template/app.py` & `rayasdk-1.1.2.dev0/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/utils.py` & `rayasdk-1.1.2.dev0/rayasdk/utils.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk/vcs.py` & `rayasdk-1.1.2.dev0/rayasdk/vcs.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/rayasdk.egg-info/PKG-INFO` & `rayasdk-1.1.2.dev0/rayasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.1.dev0
+Version: 1.1.2.dev0
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: 
 Download-URL: 
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
```

### Comparing `rayasdk-1.1.1.dev0/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.2.dev0/rayasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.1.dev0/setup.py` & `rayasdk-1.1.2.dev0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.1.dev'
+VERSION = '1.1.2.dev'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rayasdk',
     packages=find_packages(),
```

