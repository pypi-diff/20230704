# Comparing `tmp/qps_limit-1.0.7-py3-none-any.whl.zip` & `tmp/qps_limit-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5217 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jul-04 04:58 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     5206 b- defN 23-Jul-04 04:58 qps_limit/limiter.py
+Zip file size: 5357 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jul-04 08:29 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     5742 b- defN 23-Jul-04 08:28 qps_limit/limiter.py
 -rw-rw-r--  2.0 unx     5474 b- defN 23-Jul-04 04:55 qps_limit/run.py
--rw-rw-r--  2.0 unx     2552 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/RECORD
-8 files, 14121 bytes uncompressed, 4133 bytes compressed:  70.7%
+-rw-rw-r--  2.0 unx     2552 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/RECORD
+8 files, 14657 bytes uncompressed, 4273 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.7.dist-info/METADATA
+Filename: qps_limit-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.7.dist-info/WHEEL
+Filename: qps_limit-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.7.dist-info/top_level.txt
+Filename: qps_limit-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.7.dist-info/zip-safe
+Filename: qps_limit-1.0.8.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.0.7.dist-info/RECORD
+Filename: qps_limit-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.7'
+__version__ = '1.0.8'
 
 from .run import batch_run, async_batch_run
 from .limiter import Limiter
 
 __all__ = [
     'batch_run',
     'async_batch_run',
```

## qps_limit/limiter.py

```diff
@@ -1,8 +1,9 @@
 import itertools
+import logging
 import math
 import multiprocessing
 import time
 from typing import Any, Callable, Coroutine, Optional
 
 from tqdm import tqdm
 
@@ -20,31 +21,42 @@
         worker_max_qps: Optional[float] = None,
         streaming: bool = False,
         ordered: bool = True,
         verbose: bool = False,
         warmup_steps: int = 1,
         max_coroutines: int = 128
     ) -> Callable:
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(logging.INFO)
+        handler = logging.StreamHandler()
+        handler.setLevel(logging.INFO)
+        formatter = logging.Formatter(
+            fmt="%(asctime)s - %(levelname)s - %(message)s",
+            datefmt="%m/%d/%Y %H:%M:%S"
+        )
+        handler.setFormatter(formatter)
+        self.logger.addHandler(handler)
+
         try:
             multiprocessing.set_start_method('fork')
         except RuntimeError:
             if self.verbose:
-                print("multiprocessing set_start_method error")
+                self.logger.error("multiprocessing set_start_method error")
 
         self.func = func
         self.params = params
         self.callback = callback
         self.num_workers = num_workers
         self.worker_max_qps = worker_max_qps
         self.streaming = streaming
         self.ordered = ordered
         self.verbose = verbose
 
         if self.verbose:
-            print("warmup worker nodes with {} data".format(warmup_steps))
+            self.logger.info("warmup worker nodes with {} data".format(warmup_steps))
         warmup_param_iterator = itertools.islice(self.params(), warmup_steps)
         warmup_start_time = time.time()
         batch_run(
             func=self.func,
             params=warmup_param_iterator,
             max_qps=None,
             max_coroutines=1
@@ -52,15 +64,17 @@
         warmup_end_time = time.time()
         avg_worker_time = (warmup_end_time - warmup_start_time) / warmup_steps
         if self.worker_max_qps is None:
             self.max_coroutines = max_coroutines
         else:
             self.max_coroutines = min(max_coroutines, self.worker_max_qps * math.ceil(avg_worker_time))
         if self.verbose:
-            print("avg worker time: {:.2f}s -> set coroutine num: {}".format(avg_worker_time, self.max_coroutines))
+            self.logger.info(
+                "avg worker time: {:.2f}s -> set coroutine num: {}".format(avg_worker_time, self.max_coroutines)
+            )
 
         if self.ordered:
             self.res_dict = multiprocessing.Manager().dict()
         else:
             self.res_queue = multiprocessing.Queue()
 
         self.job_value = multiprocessing.Value('i', 0)
@@ -113,15 +127,17 @@
         while True:
             if self.verbose:
                 data_bar.update(self.job_value.value - data_bar.n)
             if self.worker_value.value == self.num_workers:
                 break
         if self.verbose:
             data_bar.close()
-            print("receive {} data from {} worker nodes".format(self.job_value.value, self.worker_value.value))
+            self.logger.info(
+                "receive {} data from {} worker nodes".format(self.job_value.value, self.worker_value.value)
+            )
 
         self.job_count = self.job_value.value
         progress_worker = multiprocessing.Process(target=self._progress_worker)
         progress_worker.start()
         self.worker_event.set()
 
         job_done = 0
@@ -137,12 +153,12 @@
         assert job_done == self.job_count
 
         for worker in self.workers:
             worker.join()
         progress_worker.join()
         end_time = time.time()
         if self.verbose:
-            print('elapsed time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
+            self.logger.info('elapsed time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
                 end_time - start_time,
                 self.job_count / (end_time - start_time),
                 self.worker_max_qps * self.num_workers if self.worker_max_qps else float("inf"))
             )
```

## Comparing `qps_limit-1.0.7.dist-info/METADATA` & `qps_limit-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.7
+Version: 1.0.8
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

## Comparing `qps_limit-1.0.7.dist-info/RECORD` & `qps_limit-1.0.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-qps_limit/__init__.py,sha256=1vkSBhY4iqUNYMOZOiIljEgsH2Y1HtN2IrDdcRjZHDo,165
-qps_limit/limiter.py,sha256=87uGi7b_PGI35cHYckHCMCkvvEpQ1mklsmYH78E7Djw,5206
+qps_limit/__init__.py,sha256=C8s-LOIrzYOUt9wOS2bhMGqYmDvUEnIQ11e6XSyWqg4,165
+qps_limit/limiter.py,sha256=d2JkuvHv6jcuZiasicHS9Y4ZrkhkxQIIa_ruJcfFAiA,5742
 qps_limit/run.py,sha256=mqmPou-88VcnDqjg4dcjn5eYYyslJUGm79gblWnmVZQ,5474
-qps_limit-1.0.7.dist-info/METADATA,sha256=PXeH_iUhHCMYfJMM0GudKsJwBEQQljPlpZbRZp-OwiI,2552
-qps_limit-1.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-qps_limit-1.0.7.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
-qps_limit-1.0.7.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-qps_limit-1.0.7.dist-info/RECORD,,
+qps_limit-1.0.8.dist-info/METADATA,sha256=t29Lf6I9XfVIJHpCnxgLGdoq6pZAX7zy5dQYk6b9rmI,2552
+qps_limit-1.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+qps_limit-1.0.8.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
+qps_limit-1.0.8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+qps_limit-1.0.8.dist-info/RECORD,,
```

