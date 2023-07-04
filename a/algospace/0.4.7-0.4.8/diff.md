# Comparing `tmp/algospace-0.4.7.tar.gz` & `tmp/algospace-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algospace-0.4.7.tar", last modified: Mon Jul  3 18:20:22 2023, max compression
+gzip compressed data, was "algospace-0.4.8.tar", last modified: Tue Jul  4 05:38:14 2023, max compression
```

## Comparing `algospace-0.4.7.tar` & `algospace-0.4.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.813934 algospace-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-03 18:20:13.000000 algospace-0.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-03 18:20:13.000000 algospace-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-03 18:20:22.813934 algospace-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-03 18:20:13.000000 algospace-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace/customer/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/customer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/customer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/customer/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/customer/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/docker_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/enroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/param_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    41688 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/stdio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.813934 algospace-0.4.7/algospace/provider/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/algospace-config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.813934 algospace-0.4.7/algospace/provider/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-docker-logs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-docker-start.sh
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-docker-stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 18:20:22.813934 algospace-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-03 18:20:13.000000 algospace-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:14.795346 algospace-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-04 05:38:06.000000 algospace-0.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 05:38:06.000000 algospace-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-04 05:38:14.795346 algospace-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-04 05:38:06.000000 algospace-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:14.791346 algospace-0.4.8/algospace/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:14.791346 algospace-0.4.8/algospace/customer/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/customer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/customer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/customer/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/customer/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:14.791346 algospace-0.4.8/algospace/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:14.791346 algospace-0.4.8/algospace/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/docker_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/enroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/param_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41687 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/stdio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:14.791346 algospace-0.4.8/algospace/provider/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/templates/algospace-config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:14.795346 algospace-0.4.8/algospace/provider/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/templates/docker/algospace-docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/templates/docker/algospace-docker-logs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/templates/docker/algospace-docker-start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/templates/docker/algospace-docker-stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/provider/templates/docker/algospace-dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 05:38:06.000000 algospace-0.4.8/algospace/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:38:14.791346 algospace-0.4.8/algospace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-04 05:38:14.000000 algospace-0.4.8/algospace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-04 05:38:14.000000 algospace-0.4.8/algospace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:38:14.000000 algospace-0.4.8/algospace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-04 05:38:14.000000 algospace-0.4.8/algospace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 05:38:14.000000 algospace-0.4.8/algospace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 05:38:14.000000 algospace-0.4.8/algospace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 05:38:14.795346 algospace-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-04 05:38:06.000000 algospace-0.4.8/setup.py
```

### Comparing `algospace-0.4.7/PKG-INFO` & `algospace-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.7
+Version: 0.4.8
 Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
```

### Comparing `algospace-0.4.7/README.md` & `algospace-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/__init__.py` & `algospace-0.4.8/algospace/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/__main__.py` & `algospace-0.4.8/algospace/__main__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/customer/fn.py` & `algospace-0.4.8/algospace/customer/fn.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/customer/service.py` & `algospace-0.4.8/algospace/customer/service.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/exceptions/__init__.py` & `algospace-0.4.8/algospace/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/logger.py` & `algospace-0.4.8/algospace/logger.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/login.py` & `algospace-0.4.8/algospace/login.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/provider/cloud.py` & `algospace-0.4.8/algospace/provider/cloud.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/provider/config.py` & `algospace-0.4.8/algospace/provider/config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/provider/config_generator.py` & `algospace-0.4.8/algospace/provider/config_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/provider/config_loader.py` & `algospace-0.4.8/algospace/provider/config_loader.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/provider/docker_generator.py` & `algospace-0.4.8/algospace/provider/docker_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/provider/enroll.py` & `algospace-0.4.8/algospace/provider/enroll.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/provider/param_validator.py` & `algospace-0.4.8/algospace/provider/param_validator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace/provider/service.py` & `algospace-0.4.8/algospace/provider/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -841,16 +841,14 @@
         fn_process = create_fn_process()
         service_process = create_service_process()
         gradio_process = create_gradio_process()
         process_exit_code = None
 
         self.algo_logger.info(f'Waiting for service launched...')
 
-        after_cancel_tasks = []
-
         async def join_task(process: multiprocessing.Process):
             nonlocal process_exit_code
             try:
                 await asyncio.get_event_loop().run_in_executor(None, process.join)
                 process_exit_code = process.exitcode
             except:
                 if process.is_alive():
@@ -875,40 +873,40 @@
                     traceback.print_exc()
                     self.algo_logger.error(f'Heartbeat error: {str(e)}')
 
         async def subprocess_stdio_task():
             queue_stdio_exec = QueueStdIOExec(stdio_queue)
             stdio_exec = queue_stdio_exec.exec
             stdio_exec_all = queue_stdio_exec.exec_all
-            after_cancel_tasks.append(stdio_exec_all)
             is_execed = True
             while True:
                 try:
                     if not is_execed:
                         await asyncio.sleep(0.1)
                     is_execed = await asyncio.get_event_loop().run_in_executor(None, stdio_exec)
                 except concurrent.futures._base.CancelledError:
+                    stdio_exec_all()
                     break
                 except asyncio.CancelledError:
+                    stdio_exec_all()
                     break
                 except Exception as e:
                     traceback.print_exc()
                     self.algo_logger.error(f'Handle subprocess stdio error: {str(e)}')
 
         # 当有任务抛出异常时，停止所有任务
         tasks = [join_task(fn_process),
                  join_task(service_process),
                  join_task(gradio_process),
                  heartbeat_task(),
                  subprocess_stdio_task()]
         done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
         for task in pending:
             task.cancel()
-        for task in after_cancel_tasks:
-            task()
+        await asyncio.wait(pending, return_when=asyncio.ALL_COMPLETED)
         for task in done:
             task.result()
         return process_exit_code
 
 
 def run_service(config_path: str, fetch_mode: str = 'listen') -> None:
     loop = asyncio.get_event_loop()
```

### Comparing `algospace-0.4.7/algospace/provider/stdio.py` & `algospace-0.4.8/algospace/provider/stdio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: 标准输入输出处理
 @Author: Kermit
 @Date: 2022-11-07 14:56:36
-@LastEditors: Kermit
-@LastEditTime: 2023-04-10 16:37:02
 '''
 
 import sys
 import os
 from typing import Callable
 import time
 from multiprocessing import Queue
```

### Comparing `algospace-0.4.7/algospace/provider/templates/algospace-config.py` & `algospace-0.4.8/algospace/provider/templates/algospace-config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/algospace.egg-info/PKG-INFO` & `algospace-0.4.8/algospace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.7
+Version: 0.4.8
 Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
```

### Comparing `algospace-0.4.7/algospace.egg-info/SOURCES.txt` & `algospace-0.4.8/algospace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algospace-0.4.7/setup.py` & `algospace-0.4.8/setup.py`

 * *Files identical despite different names*

