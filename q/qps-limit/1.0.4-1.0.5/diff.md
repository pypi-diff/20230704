# Comparing `tmp/qps_limit-1.0.4-py3-none-any.whl.zip` & `tmp/qps_limit-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5253 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jul-03 12:54 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     5244 b- defN 23-Jul-03 12:53 qps_limit/limiter.py
+Zip file size: 5237 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jul-03 13:02 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     5145 b- defN 23-Jul-03 13:02 qps_limit/limiter.py
 -rw-rw-r--  2.0 unx     5459 b- defN 23-Jul-03 12:36 qps_limit/run.py
--rw-rw-r--  2.0 unx     2609 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-03 12:54 qps_limit-1.0.4.dist-info/RECORD
-8 files, 14201 bytes uncompressed, 4169 bytes compressed:  70.6%
+-rw-rw-r--  2.0 unx     2609 b- defN 23-Jul-03 13:02 qps_limit-1.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-03 13:02 qps_limit-1.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-03 13:02 qps_limit-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-03 13:02 qps_limit-1.0.5.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-03 13:02 qps_limit-1.0.5.dist-info/RECORD
+8 files, 14102 bytes uncompressed, 4153 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.4.dist-info/METADATA
+Filename: qps_limit-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.4.dist-info/WHEEL
+Filename: qps_limit-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.4.dist-info/top_level.txt
+Filename: qps_limit-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.4.dist-info/zip-safe
+Filename: qps_limit-1.0.5.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.0.4.dist-info/RECORD
+Filename: qps_limit-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 
 from .run import batch_run, async_batch_run
 from .limiter import Limiter
 
 __all__ = [
     'batch_run',
     'async_batch_run',
```

## qps_limit/limiter.py

```diff
@@ -40,16 +40,15 @@
         self.callback = callback
         self.progress = progress
         self.ordered = ordered
         self.verbose = verbose
 
         if self.verbose:
             print("warmup worker nodes with {} data".format(warmup_steps))
-        self.param_iterator, warmup_param_iterator = itertools.tee(self.params(), 2)
-        warmup_param_iterator = itertools.islice(warmup_param_iterator, warmup_steps)
+        warmup_param_iterator = itertools.islice(self.params(), warmup_steps)
         warmup_start_time = time.time()
         batch_run(
             func=self.func,
             params=warmup_param_iterator,
             max_qps=None,
             max_workers=1
         )
@@ -83,15 +82,15 @@
         progress_cnt = 0
         while progress_cnt < self.job_count:
             progress_bar.update(self.job_queue.get())
             progress_cnt += 1
 
     def _worker(self, mod: int):
         def make_worker_iterator():
-            for idx, (args, kwargs) in enumerate(self.param_iterator):
+            for idx, (args, kwargs) in enumerate(self.params()):
                 if idx % self.num_workers == mod:
                     yield args, kwargs
 
         batch_run_func = batch_run if not self.streaming else streaming_batch_run
         for idx, res in batch_run_func(
             func=self.func,
             params=make_worker_iterator(),
```

## Comparing `qps_limit-1.0.4.dist-info/METADATA` & `qps_limit-1.0.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.4
+Version: 1.0.5
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

