# Comparing `tmp/qps_limit-1.0.6-py3-none-any.whl.zip` & `tmp/qps_limit-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5252 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jul-04 03:01 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     5269 b- defN 23-Jul-04 03:01 qps_limit/limiter.py
--rw-rw-r--  2.0 unx     5474 b- defN 23-Jul-04 03:01 qps_limit/run.py
--rw-rw-r--  2.0 unx     2609 b- defN 23-Jul-04 03:03 qps_limit-1.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 03:03 qps_limit-1.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-04 03:03 qps_limit-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-04 03:03 qps_limit-1.0.6.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-04 03:03 qps_limit-1.0.6.dist-info/RECORD
-8 files, 14241 bytes uncompressed, 4168 bytes compressed:  70.7%
+Zip file size: 5217 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jul-04 04:58 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     5206 b- defN 23-Jul-04 04:58 qps_limit/limiter.py
+-rw-rw-r--  2.0 unx     5474 b- defN 23-Jul-04 04:55 qps_limit/run.py
+-rw-rw-r--  2.0 unx     2552 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-04 04:58 qps_limit-1.0.7.dist-info/RECORD
+8 files, 14121 bytes uncompressed, 4133 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.6.dist-info/METADATA
+Filename: qps_limit-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.6.dist-info/WHEEL
+Filename: qps_limit-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.6.dist-info/top_level.txt
+Filename: qps_limit-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.6.dist-info/zip-safe
+Filename: qps_limit-1.0.7.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.0.6.dist-info/RECORD
+Filename: qps_limit-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.6'
+__version__ = '1.0.7'
 
 from .run import batch_run, async_batch_run
 from .limiter import Limiter
 
 __all__ = [
     'batch_run',
     'async_batch_run',
```

## qps_limit/limiter.py

```diff
@@ -11,37 +11,35 @@
 
 class Limiter():
 
     def __init__(
         self,
         func: Callable[..., Coroutine[Any, Any, Any]],
         params: Callable,
+        callback: Optional[Callable] = None,
         num_workers: int = 1,
         worker_max_qps: Optional[float] = None,
         streaming: bool = False,
-        callback: Optional[Callable] = None,
-        progress: bool = True,
         ordered: bool = True,
         verbose: bool = False,
         warmup_steps: int = 1,
         max_coroutines: int = 128
     ) -> Callable:
         try:
             multiprocessing.set_start_method('fork')
         except RuntimeError:
             if self.verbose:
                 print("multiprocessing set_start_method error")
 
         self.func = func
         self.params = params
+        self.callback = callback
         self.num_workers = num_workers
         self.worker_max_qps = worker_max_qps
         self.streaming = streaming
-        self.callback = callback
-        self.progress = progress
         self.ordered = ordered
         self.verbose = verbose
 
         if self.verbose:
             print("warmup worker nodes with {} data".format(warmup_steps))
         warmup_param_iterator = itertools.islice(self.params(), warmup_steps)
         warmup_start_time = time.time()
@@ -64,23 +62,21 @@
             self.res_dict = multiprocessing.Manager().dict()
         else:
             self.res_queue = multiprocessing.Queue()
 
         self.job_value = multiprocessing.Value('i', 0)
         self.worker_value = multiprocessing.Value('i', 0)
         self.worker_event = multiprocessing.Event()
-        self.job_queue = multiprocessing.Queue() if self.progress else None
+        self.job_queue = multiprocessing.Queue()
 
         self.workers = []
         for mod in range(self.num_workers):
             self.workers.append(multiprocessing.Process(target=self._worker, args=(mod, )))
 
     def _progress_worker(self):
-        if self.job_queue is None:
-            return
         progress_bar = tqdm(total=self.job_count, desc=self.func.__name__)
         progress_cnt = 0
         while progress_cnt < self.job_count:
             progress_bar.update(self.job_queue.get())
             progress_cnt += 1
 
     def _worker(self, mod: int):
@@ -89,17 +85,17 @@
                 if idx % self.num_workers == mod:
                     yield args, kwargs
 
         batch_run_func = batch_run if not self.streaming else streaming_batch_run
         for idx, res in batch_run_func(
             func=self.func,
             params=make_worker_iterator(),
+            callback=self.callback,
             max_qps=self.worker_max_qps,
             max_coroutines=self.max_coroutines,
-            callback=self.callback,
             job_queue=self.job_queue,
             job_value=self.job_value,
             worker_value=self.worker_value,
             worker_event=self.worker_event
         ):
             real_idx = idx * self.num_workers + mod
             if self.ordered:
@@ -107,36 +103,43 @@
             else:
                 self.res_queue.put((real_idx, res))
 
     def __call__(self):
         start_time = time.time()
         for worker in self.workers:
             worker.start()
+
+        if self.verbose:
+            data_bar = tqdm(desc='data')
         while True:
             if self.verbose:
-                print("receive {} data ...".format(self.job_value.value), end='\r')
+                data_bar.update(self.job_value.value - data_bar.n)
             if self.worker_value.value == self.num_workers:
                 break
         if self.verbose:
+            data_bar.close()
             print("receive {} data from {} worker nodes".format(self.job_value.value, self.worker_value.value))
+
         self.job_count = self.job_value.value
         progress_worker = multiprocessing.Process(target=self._progress_worker)
         progress_worker.start()
         self.worker_event.set()
+
         job_done = 0
         while job_done < self.job_count:
             if self.ordered:
                 while job_done not in self.res_dict:
                     pass
                 yield (job_done, self.res_dict[job_done])
                 del self.res_dict[job_done]
             else:
                 yield self.res_queue.get()
             job_done += 1
         assert job_done == self.job_count
+
         for worker in self.workers:
             worker.join()
         progress_worker.join()
         end_time = time.time()
         if self.verbose:
             print('elapsed time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
                 end_time - start_time,
```

## qps_limit/run.py

 * *Ordering differences only*

```diff
@@ -14,17 +14,17 @@
     return AsyncLimiter(max_rate=max_rate, time_period=time_period)
 
 
 async def async_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
+    callback: Optional[Callable] = None,
     max_qps: Optional[float] = None,
     max_coroutines: int = 128,
-    callback: Optional[Callable] = None,
     job_queue: Optional[multiprocessing.Queue] = None,
     job_value: Optional[multiprocessing.Value] = None,
     worker_value: Optional[multiprocessing.Value] = None,
     worker_event: Optional[multiprocessing.Event] = None
 ):
     if max_qps is not None:
         limiter = get_limiter(max_qps)
@@ -71,32 +71,32 @@
     return result
 
 
 def batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
+    callback: Optional[Callable] = None,
     max_qps: Optional[float] = None,
     max_coroutines: int = 128,
-    callback: Optional[Callable] = None,
     job_queue: Optional[multiprocessing.Queue] = None,
     job_value: Optional[multiprocessing.Value] = None,
     worker_value: Optional[multiprocessing.Value] = None,
     worker_event: Optional[multiprocessing.Event] = None
 ):
     return asyncio.new_event_loop().run_until_complete(async_batch_run(**locals()))
 
 
 async def async_streaming_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
+    callback: Optional[Callable] = None,
     max_qps: Optional[float] = None,
     max_coroutines: int = 128,
-    callback: Optional[Callable] = None,
     job_queue: Optional[multiprocessing.Queue] = None,
     job_value: Optional[multiprocessing.Value] = None,
     worker_value: Optional[multiprocessing.Value] = None,
     worker_event: Optional[multiprocessing.Event] = None
 ):
     if max_qps is not None:
         limiter = get_limiter(max_qps)
@@ -147,17 +147,17 @@
     assert job_consume == job_cnt
 
 
 def streaming_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
+    callback: Optional[Callable] = None,
     max_qps: Optional[float] = None,
     max_coroutines: int = 128,
-    callback: Optional[Callable] = None,
     job_queue: Optional[multiprocessing.Queue] = None,
     job_value: Optional[multiprocessing.Value] = None,
     worker_value: Optional[multiprocessing.Value] = None,
     worker_event: Optional[multiprocessing.Event] = None
 ):
     async_generator = async_streaming_batch_run(**locals())
```

## Comparing `qps_limit-1.0.6.dist-info/METADATA` & `qps_limit-1.0.7.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.6
+Version: 1.0.7
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -44,19 +44,18 @@
 
 ```python
 from qps_limit import Limiter
 
 f = Limiter(
     func="an asynchronous function",
     params="a generator function yields args and kwargs",
+    callback="a callback function that handles the return values of func",
     num_workers="number of processes, recommended <= number of CPUs",
     worker_max_qps="maximum qps per process, None means unlimited",
     streaming="stream data processing, useful when the memory is limited",
-    callback="a callback function that handles the return values of func",
-    progress="display a progress bar",
     ordered="return ordered results or not"
 )
 ```
 
 BTW: The wrapped function returns a structure `(idx, res)` consisting of an index of the data and the function return value. If `ordered=False` is set, the order of the returned values may be randomized for better performance.
 
 ### Example
@@ -66,14 +65,15 @@
 > Assuming that `func` is a time-consuming function, it takes 1.0 seconds to execute
 
 ```python
 import asyncio
 
 from qps_limit import Limiter
 
+
 async def func(n: int):
     await asyncio.sleep(1.0)
     return 1 + 1 / n, n
 
 
 def params():
     for n in range(1, 1001):
@@ -83,18 +83,17 @@
 def callback(r):
     return r[0] ** r[1]
 
 
 f = Limiter(
     func=func,
     params=params,
+    callback=callback,
     num_workers=10,
     worker_max_qps=10,
     streaming=False,
-    callback=callback,
-    progress=True,
     ordered=True
 )
 
 for idx, r in f():
     print(idx, r)
 ```
```

