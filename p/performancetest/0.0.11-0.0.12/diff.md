# Comparing `tmp/performancetest-0.0.11.tar.gz` & `tmp/performancetest-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "performancetest-0.0.11.tar", last modified: Mon Jul  3 10:15:28 2023, max compression
+gzip compressed data, was "performancetest-0.0.12.tar", last modified: Tue Jul  4 03:41:17 2023, max compression
```

## Comparing `performancetest-0.0.11.tar` & `performancetest-0.0.12.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 10:15:28.330161 performancetest-0.0.11/
--rw-rw-rw-   0        0        0      516 2023-07-03 10:15:28.330161 performancetest-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 10:15:28.167663 performancetest-0.0.11/performancetest/
--rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.11/performancetest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:15:28.287607 performancetest-0.0.11/performancetest/core/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.11/performancetest/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:15:28.290598 performancetest-0.0.11/performancetest/core/base/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.11/performancetest/core/base/__init__.py
--rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.11/performancetest/core/base/actuator.py
--rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.11/performancetest/core/base/monitor.py
--rw-rw-rw-   0        0        0     3562 2023-06-21 12:46:09.000000 performancetest-0.0.11/performancetest/core/command.py
--rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.11/performancetest/core/cpu.py
--rw-rw-rw-   0        0        0     6413 2023-06-23 08:54:45.000000 performancetest-0.0.11/performancetest/core/device.py
--rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.11/performancetest/core/devicebattery.py
--rw-rw-rw-   0        0        0    19366 2023-07-03 10:04:25.000000 performancetest-0.0.11/performancetest/core/fps.py
--rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.11/performancetest/core/global_data.py
--rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.11/performancetest/core/gpu.py
--rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.11/performancetest/core/iosperf.py
--rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.11/performancetest/core/memory.py
--rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.11/performancetest/core/snapshot.py
--rw-rw-rw-   0        0        0     4254 2023-07-03 09:44:21.000000 performancetest-0.0.11/performancetest/core/task_handle.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:15:28.300259 performancetest-0.0.11/performancetest/test/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.11/performancetest/test/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.11/performancetest/test/all_property_test.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:15:28.328165 performancetest-0.0.11/performancetest/web/
--rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.11/performancetest/web/__init__.py
--rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.11/performancetest/web/dao.py
--rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.11/performancetest/web/entity.py
--rw-rw-rw-   0        0        0     9224 2023-07-03 09:44:21.000000 performancetest-0.0.11/performancetest/web/main.py
--rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.11/performancetest/web/util.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:15:28.190600 performancetest-0.0.11/performancetest.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-03 10:15:28.000000 performancetest-0.0.11/performancetest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2023-07-03 10:15:28.000000 performancetest-0.0.11/performancetest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 10:15:28.000000 performancetest-0.0.11/performancetest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-03 10:15:28.000000 performancetest-0.0.11/performancetest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 10:15:28.331159 performancetest-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-07-03 10:09:20.000000 performancetest-0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:41:17.250066 performancetest-0.0.12/
+-rw-rw-rw-   0        0        0      516 2023-07-04 03:41:17.249103 performancetest-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 03:41:17.208917 performancetest-0.0.12/performancetest/
+-rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.12/performancetest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:41:17.236104 performancetest-0.0.12/performancetest/core/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.12/performancetest/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:41:17.240096 performancetest-0.0.12/performancetest/core/base/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.12/performancetest/core/base/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.12/performancetest/core/base/actuator.py
+-rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.12/performancetest/core/base/monitor.py
+-rw-rw-rw-   0        0        0     3562 2023-06-21 12:46:09.000000 performancetest-0.0.12/performancetest/core/command.py
+-rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.12/performancetest/core/cpu.py
+-rw-rw-rw-   0        0        0     6451 2023-07-04 03:26:18.000000 performancetest-0.0.12/performancetest/core/device.py
+-rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.12/performancetest/core/devicebattery.py
+-rw-rw-rw-   0        0        0    19366 2023-07-03 10:04:25.000000 performancetest-0.0.12/performancetest/core/fps.py
+-rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.12/performancetest/core/global_data.py
+-rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.12/performancetest/core/gpu.py
+-rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.12/performancetest/core/iosperf.py
+-rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.12/performancetest/core/memory.py
+-rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.12/performancetest/core/snapshot.py
+-rw-rw-rw-   0        0        0     4254 2023-07-03 09:44:21.000000 performancetest-0.0.12/performancetest/core/task_handle.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:41:17.242086 performancetest-0.0.12/performancetest/test/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.12/performancetest/test/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.12/performancetest/test/all_property_test.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:41:17.248072 performancetest-0.0.12/performancetest/web/
+-rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.12/performancetest/web/__init__.py
+-rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.12/performancetest/web/dao.py
+-rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.12/performancetest/web/entity.py
+-rw-rw-rw-   0        0        0     9209 2023-07-03 11:29:59.000000 performancetest-0.0.12/performancetest/web/main.py
+-rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.12/performancetest/web/util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:41:17.221881 performancetest-0.0.12/performancetest.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-04 03:41:17.000000 performancetest-0.0.12/performancetest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2023-07-04 03:41:17.000000 performancetest-0.0.12/performancetest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 03:41:17.000000 performancetest-0.0.12/performancetest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-04 03:41:17.000000 performancetest-0.0.12/performancetest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 03:41:17.250066 performancetest-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-07-04 03:41:06.000000 performancetest-0.0.12/setup.py
```

### Comparing `performancetest-0.0.11/PKG-INFO` & `performancetest-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.11
+Version: 0.0.12
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.11/README.md` & `performancetest-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/command.py` & `performancetest-0.0.12/performancetest/core/command.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/cpu.py` & `performancetest-0.0.12/performancetest/core/cpu.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/device.py` & `performancetest-0.0.12/performancetest/core/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,20 +121,21 @@
     def get_battery(self):
         res = self.device.get_io_power()
         res_text = {"CurrentCapacity": (res['Diagnostics']['IORegistry']['CurrentCapacity']), "Temperature": (
             res['Diagnostics']['IORegistry']['Temperature'])}
         return res_text
 
     def get_perf(self):
-        perf = tidevice.Performance(self.device, [DataType.CPU, DataType.MEMORY, DataType.FPS, DataType.GPU])
-        _rp = RunningProcess(self.device, self.package)
-        perf._rp = _rp
         if not self.perf_dict_iter.get(self.package):
+            perf = tidevice.Performance(self.device, [DataType.CPU, DataType.MEMORY, DataType.FPS, DataType.GPU])
+            _rp = RunningProcess(self.device, self.package)
+            perf._rp = _rp
             self.perf_dict_iter[self.package] = {"cm": iter_cpu_memory(self.device, _rp), "fps": iter_fps(self.device),
                                                  "gpu": iter_gpu(self.device)}
+        perf_info = None
         try:
             perf_info = self.gen_perf_info(self.package)
         except:
             traceback.print_exc()
             del self.perf_dict_iter[self.package]
         return perf_info
```

### Comparing `performancetest-0.0.11/performancetest/core/devicebattery.py` & `performancetest-0.0.12/performancetest/core/devicebattery.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/fps.py` & `performancetest-0.0.12/performancetest/core/fps.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/global_data.py` & `performancetest-0.0.12/performancetest/core/global_data.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/gpu.py` & `performancetest-0.0.12/performancetest/core/gpu.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/iosperf.py` & `performancetest-0.0.12/performancetest/core/iosperf.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/memory.py` & `performancetest-0.0.12/performancetest/core/memory.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/snapshot.py` & `performancetest-0.0.12/performancetest/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/core/task_handle.py` & `performancetest-0.0.12/performancetest/core/task_handle.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/test/all_property_test.py` & `performancetest-0.0.12/performancetest/test/all_property_test.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/web/dao.py` & `performancetest-0.0.12/performancetest/web/dao.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest/web/main.py` & `performancetest-0.0.12/performancetest/web/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         task_item.status = 2
         task_item.end_time = datetime.datetime.now()
         try:
             if task_item.platform == "ios":
                 t = Device(task_item.serialno)
                 with t.connect_instruments() as ts:
                     logger.info('Stop...')
-                    ts.stop_iter_cpu_memory()
+                    ts.close()
         except:
             traceback.print_exc()
     return {"code": 200}
 
 
 @app.get("/delete_task/")
 async def delete_task(request: Request, id: int):
```

### Comparing `performancetest-0.0.11/performancetest/web/util.py` & `performancetest-0.0.12/performancetest/web/util.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/performancetest.egg-info/PKG-INFO` & `performancetest-0.0.12/performancetest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.11
+Version: 0.0.12
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.11/performancetest.egg-info/SOURCES.txt` & `performancetest-0.0.12/performancetest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.11/setup.py` & `performancetest-0.0.12/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # # _*_ coding: utf-8 _*_
 from setuptools import setup, find_packages
 
 setup(
        name='performancetest',
-       version='0.0.11',
+       version='0.0.12',
        url='https://github.com/1033866383/perf-orange-cat',
        author='bozhou.fan',
        author_email='15525730080@163.com',
        description='Android, IOS app_performance',
        packages=find_packages(),
        install_requires=[],
        include_package_data=True,  # 这里添加 include_package_data 参数
```

