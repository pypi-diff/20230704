# Comparing `tmp/performancetest-0.0.14.tar.gz` & `tmp/performancetest-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "performancetest-0.0.14.tar", last modified: Tue Jul  4 04:48:58 2023, max compression
+gzip compressed data, was "performancetest-0.0.15.tar", last modified: Tue Jul  4 06:22:07 2023, max compression
```

## Comparing `performancetest-0.0.14.tar` & `performancetest-0.0.15.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 04:48:58.627357 performancetest-0.0.14/
--rw-rw-rw-   0        0        0      516 2023-07-04 04:48:58.627357 performancetest-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.14/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 04:48:58.583474 performancetest-0.0.14/performancetest/
--rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.14/performancetest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 04:48:58.614392 performancetest-0.0.14/performancetest/core/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.14/performancetest/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 04:48:58.618385 performancetest-0.0.14/performancetest/core/base/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.14/performancetest/core/base/__init__.py
--rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.14/performancetest/core/base/actuator.py
--rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.14/performancetest/core/base/monitor.py
--rw-rw-rw-   0        0        0     3562 2023-06-21 12:46:09.000000 performancetest-0.0.14/performancetest/core/command.py
--rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.14/performancetest/core/cpu.py
--rw-rw-rw-   0        0        0     6451 2023-07-04 03:26:18.000000 performancetest-0.0.14/performancetest/core/device.py
--rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.14/performancetest/core/devicebattery.py
--rw-rw-rw-   0        0        0    19366 2023-07-03 10:04:25.000000 performancetest-0.0.14/performancetest/core/fps.py
--rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.14/performancetest/core/global_data.py
--rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.14/performancetest/core/gpu.py
--rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.14/performancetest/core/iosperf.py
--rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.14/performancetest/core/memory.py
--rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.14/performancetest/core/snapshot.py
--rw-rw-rw-   0        0        0     4254 2023-07-03 09:44:21.000000 performancetest-0.0.14/performancetest/core/task_handle.py
-drwxrwxrwx   0        0        0        0 2023-07-04 04:48:58.620377 performancetest-0.0.14/performancetest/test/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.14/performancetest/test/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.14/performancetest/test/all_property_test.py
-drwxrwxrwx   0        0        0        0 2023-07-04 04:48:58.625363 performancetest-0.0.14/performancetest/web/
--rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.14/performancetest/web/__init__.py
--rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.14/performancetest/web/dao.py
--rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.14/performancetest/web/entity.py
--rw-rw-rw-   0        0        0     9209 2023-07-03 11:29:59.000000 performancetest-0.0.14/performancetest/web/main.py
--rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.14/performancetest/web/util.py
-drwxrwxrwx   0        0        0        0 2023-07-04 04:48:58.601424 performancetest-0.0.14/performancetest.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-04 04:48:58.000000 performancetest-0.0.14/performancetest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-07-04 04:48:58.000000 performancetest-0.0.14/performancetest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 04:48:58.000000 performancetest-0.0.14/performancetest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 04:48:58.000000 performancetest-0.0.14/performancetest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-04 04:48:58.000000 performancetest-0.0.14/performancetest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 04:48:58.627357 performancetest-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-07-04 04:48:34.000000 performancetest-0.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:22:07.415559 performancetest-0.0.15/
+-rw-rw-rw-   0        0        0      516 2023-07-04 06:22:07.414559 performancetest-0.0.15/PKG-INFO
+-rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.15/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 06:22:07.352723 performancetest-0.0.15/performancetest/
+-rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.15/performancetest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:22:07.394612 performancetest-0.0.15/performancetest/core/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.15/performancetest/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:22:07.399602 performancetest-0.0.15/performancetest/core/base/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.15/performancetest/core/base/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.15/performancetest/core/base/actuator.py
+-rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.15/performancetest/core/base/monitor.py
+-rw-rw-rw-   0        0        0     3562 2023-06-21 12:46:09.000000 performancetest-0.0.15/performancetest/core/command.py
+-rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.15/performancetest/core/cpu.py
+-rw-rw-rw-   0        0        0     6451 2023-07-04 03:26:18.000000 performancetest-0.0.15/performancetest/core/device.py
+-rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.15/performancetest/core/devicebattery.py
+-rw-rw-rw-   0        0        0    19366 2023-07-03 10:04:25.000000 performancetest-0.0.15/performancetest/core/fps.py
+-rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.15/performancetest/core/global_data.py
+-rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.15/performancetest/core/gpu.py
+-rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.15/performancetest/core/iosperf.py
+-rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.15/performancetest/core/memory.py
+-rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.15/performancetest/core/snapshot.py
+-rw-rw-rw-   0        0        0     4254 2023-07-03 09:44:21.000000 performancetest-0.0.15/performancetest/core/task_handle.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:22:07.402615 performancetest-0.0.15/performancetest/test/
+-rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.15/performancetest/test/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.15/performancetest/test/all_property_test.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:22:07.412564 performancetest-0.0.15/performancetest/web/
+-rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.15/performancetest/web/__init__.py
+-rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.15/performancetest/web/dao.py
+-rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.15/performancetest/web/entity.py
+-rw-rw-rw-   0        0        0     9209 2023-07-03 11:29:59.000000 performancetest-0.0.15/performancetest/web/main.py
+-rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.15/performancetest/web/util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:22:07.375663 performancetest-0.0.15/performancetest.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-04 06:22:07.000000 performancetest-0.0.15/performancetest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-07-04 06:22:07.000000 performancetest-0.0.15/performancetest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 06:22:07.000000 performancetest-0.0.15/performancetest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-07-04 06:22:07.000000 performancetest-0.0.15/performancetest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-04 06:22:07.000000 performancetest-0.0.15/performancetest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 06:22:07.416560 performancetest-0.0.15/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-07-04 06:20:42.000000 performancetest-0.0.15/setup.py
```

### Comparing `performancetest-0.0.14/PKG-INFO` & `performancetest-0.0.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.14
+Version: 0.0.15
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.14/README.md` & `performancetest-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/command.py` & `performancetest-0.0.15/performancetest/core/command.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/cpu.py` & `performancetest-0.0.15/performancetest/core/cpu.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/device.py` & `performancetest-0.0.15/performancetest/core/device.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/devicebattery.py` & `performancetest-0.0.15/performancetest/core/devicebattery.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/fps.py` & `performancetest-0.0.15/performancetest/core/fps.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/global_data.py` & `performancetest-0.0.15/performancetest/core/global_data.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/gpu.py` & `performancetest-0.0.15/performancetest/core/gpu.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/iosperf.py` & `performancetest-0.0.15/performancetest/core/iosperf.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/memory.py` & `performancetest-0.0.15/performancetest/core/memory.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/snapshot.py` & `performancetest-0.0.15/performancetest/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/core/task_handle.py` & `performancetest-0.0.15/performancetest/core/task_handle.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/test/all_property_test.py` & `performancetest-0.0.15/performancetest/test/all_property_test.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/web/dao.py` & `performancetest-0.0.15/performancetest/web/dao.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/web/main.py` & `performancetest-0.0.15/performancetest/web/main.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest/web/util.py` & `performancetest-0.0.15/performancetest/web/util.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/performancetest.egg-info/PKG-INFO` & `performancetest-0.0.15/performancetest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.14
+Version: 0.0.15
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.14/performancetest.egg-info/SOURCES.txt` & `performancetest-0.0.15/performancetest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.14/setup.py` & `performancetest-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # # _*_ coding: utf-8 _*_
 from setuptools import setup, find_packages
 
 setup(
        name='performancetest',
-       version='0.0.14',
+       version='0.0.15',
        url='https://github.com/1033866383/perf-orange-cat',
        author='bozhou.fan',
        author_email='15525730080@163.com',
        description='Android, IOS app_performance',
        packages=find_packages(),
        install_requires=[
            "psutil", "airtest", "fastapi", "tidevice", "func-timeout", "sqlalchemy", "sqlalchemy-serializer", "uvicorn"
```

