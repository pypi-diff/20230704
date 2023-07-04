# Comparing `tmp/eventix-0.3.3.tar.gz` & `tmp/eventix-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventix-0.3.3.tar", max compression
+gzip compressed data, was "eventix-0.4.0.tar", max compression
```

## Comparing `eventix-0.3.3.tar` & `eventix-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/__init__.py
--rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.3.3/eventix/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/functions/__init__.py
--rw-r--r--   0        0        0     3104 2023-07-03 12:35:26.922564 eventix-0.3.3/eventix/functions/core.py
--rw-r--r--   0        0        0      709 2023-07-03 12:35:26.910564 eventix-0.3.3/eventix/functions/errors.py
--rw-r--r--   0        0        0      900 2023-07-03 12:36:13.218289 eventix-0.3.3/eventix/functions/eventix_client.py
--rw-r--r--   0        0        0     2552 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/functions/fastapi.py
--rw-r--r--   0        0        0     6082 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/functions/task.py
--rw-r--r--   0        0        0      990 2023-07-03 12:36:06.494329 eventix-0.3.3/eventix/functions/task_scheduler.py
--rw-r--r--   0        0        0     3879 2023-07-03 12:37:58.589687 eventix-0.3.3/eventix/functions/task_worker.py
--rw-r--r--   0        0        0      322 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/functions/tools.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/pydantic/__init__.py
--rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/pydantic/event.py
--rw-r--r--   0        0        0     1951 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/pydantic/task.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/router/__init__.py
--rw-r--r--   0        0        0      517 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/router/event.py
--rw-r--r--   0        0        0      236 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/router/metrics.py
--rw-r--r--   0        0        0     1201 2023-07-03 12:25:39.726933 eventix-0.3.3/eventix/router/task.py
--rw-r--r--   0        0        0      954 2023-07-03 14:08:07.522481 eventix-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 eventix-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.4.0/eventix/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/functions/__init__.py
+-rw-r--r--   0        0        0     4402 2023-07-04 12:48:26.939576 eventix-0.4.0/eventix/functions/core.py
+-rw-r--r--   0        0        0      709 2023-07-03 12:35:26.910564 eventix-0.4.0/eventix/functions/errors.py
+-rw-r--r--   0        0        0      801 2023-07-04 06:52:56.282299 eventix-0.4.0/eventix/functions/eventix_client.py
+-rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.4.0/eventix/functions/fastapi.py
+-rw-r--r--   0        0        0     6125 2023-07-04 08:38:43.486260 eventix-0.4.0/eventix/functions/task.py
+-rw-r--r--   0        0        0      990 2023-07-03 12:36:06.494329 eventix-0.4.0/eventix/functions/task_scheduler.py
+-rw-r--r--   0        0        0     5482 2023-07-04 11:52:40.153974 eventix-0.4.0/eventix/functions/task_worker.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/functions/tools.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/pydantic/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/pydantic/event.py
+-rw-r--r--   0        0        0     1987 2023-07-04 12:48:48.055369 eventix-0.4.0/eventix/pydantic/task.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/router/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/router/event.py
+-rw-r--r--   0        0        0      236 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/router/metrics.py
+-rw-r--r--   0        0        0     1201 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/router/task.py
+-rw-r--r--   0        0        0      954 2023-07-04 13:10:17.297703 eventix-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 eventix-0.4.0/PKG-INFO
```

### Comparing `eventix-0.3.3/eventix/exceptions/__init__.py` & `eventix-0.4.0/eventix/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.3/eventix/functions/core.py` & `eventix-0.4.0/eventix/functions/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import contextlib
 import contextvars
 import functools
 import logging
 import os
-from typing import Callable
+from inspect import signature, Parameter
+from typing import Callable, Tuple, Dict, Any, List
+
+from pydantic import BaseModel
 
 from eventix.functions.task_scheduler import TaskScheduler
 from eventix.pydantic.task import TaskModel
 
 log = logging.getLogger(__name__)
 
 
@@ -51,55 +54,76 @@
     # noinspection PyTypeChecker
     worker_id = worker_id_context_var.get()
     if worker_id is None:
         worker_id = os.environ.get("EVENTFLOW_TASK_WORKER_ID", "default")
     yield worker_id
 
 
-def task(result: bool = True, unique_key_generator: Callable = None):
+def task(store_result: bool = True, unique_key_generator: Callable = None):
     # parameters suggested:
     #
-    # result: bool , wether to store or not to store results
+    # store_result: bool , wether to store or not to store results
     # unique_uid: ....  having a unique id, which leads to update the task if it is rescheduled.
 
     # retry: bool, wether to retry failed tasks
     # max_retry: int, maximum retries default 5 ... each retry doubles the time to wait, starting with 30 sec
 
     is_unique = unique_key_generator is not None
 
     def inner(f):
         class EventflowTask(EventflowTaskBase):
             def __init__(self):
                 self.func = f
                 self.func_name = f.__name__
+                self.arg_spec = list(signature(f).parameters.values())
+                self.arg_spec_args = [arg.annotation for arg in self.arg_spec]
+                self.arg_spec_kwargs = {arg.name: arg.annotation for arg in self.arg_spec}
+                assert True
+
+            def restore_pydantic_instances(self, args, kwargs) -> tuple[list[Any], Dict[str, Any]]:
+                new_args = []
+                for i, arg in enumerate(args):
+                    if isinstance(arg, dict):
+                        cls = self.arg_spec_args[i]
+                        if issubclass(cls, BaseModel):
+                            arg = cls.parse_obj(arg)
+                    new_args.append(arg)
+                new_kwargs = {}
+                for kw, arg in kwargs.items():
+                    if isinstance(arg, dict):
+                        cls = self.arg_spec_kwargs[kw]
+                        if issubclass(cls, BaseModel):
+                            arg = cls.parse_obj(arg)
+                    new_kwargs[kw] = arg
+                return new_args, new_kwargs
 
             @functools.wraps(f)
             def delay(self, *args, _priority: int | None = 0, **kwargs):
                 # priority has to be negated, needed for fixing ascending sort order
 
                 tm = self.make_task_model(args, kwargs, priority=_priority * -1)
                 # log.debug(f"scheduling {self.func.__name__} info: {tm.json()}")
                 tm = TaskScheduler.schedule(tm)
                 return tm
 
             @functools.wraps(f)
             def run(self, *args, **kwargs):
+                args, kwargs = self.restore_pydantic_instances(args, kwargs)
                 return self.func(*args, **kwargs)
 
             def make_task_model(self, args, kwargs, priority) -> TaskModel:
                 params = dict(
                     task=self.func_name,
                     args=args,
                     kwargs=kwargs,
-                    priority=priority
+                    priority=priority,
+                    store_result=store_result
                 )
                 if is_unique:
                     unique_key = unique_key_generator(*args, **kwargs)
                     params |= dict(unique_key=unique_key)
 
                 return TaskModel.parse_obj(params)
 
         return EventflowTask()
 
     return inner
-
-
```

### Comparing `eventix-0.3.3/eventix/functions/errors.py` & `eventix-0.4.0/eventix/functions/errors.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.3/eventix/functions/fastapi.py` & `eventix-0.4.0/eventix/functions/fastapi.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,17 +56,24 @@
         status_code = None
         if isinstance(e, HTTPException):
             status_code = e.status_code
             content = dict(detail=e.detail)
 
         elif isinstance(e, WebException):
             status_code = e.status_code
-            content = e.dict()
+            if status_code == 204:
+                content = None
+            else:
+                content = e.dict()
         else:
             if status_code is None:  # no status code found yet
                 status_code = 500
             content = dict(detail=await self.make_exception_detail(e))
 
         if status_code >= 500:
             log.exception(e, stacklevel=2)
 
-        return JSONResponse(status_code=status_code, content=content, headers=headers)
+        if isinstance(content, dict):
+            response = JSONResponse(status_code=status_code, content=content, headers=headers)
+        else:
+            response = Response(status_code=status_code, headers=headers, content=content)
+        return response
```

### Comparing `eventix-0.3.3/eventix/functions/task.py` & `eventix-0.4.0/eventix/functions/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+from traceback import format_tb
 from typing import List, Any
 
 from webexception.webexception import WebException
 
 from eventix.pydantic.task import TaskModel
 from pydantic_db_backend.backend import Backend
 from pydantic_db_backend.exceptions import RevisionConflict
@@ -164,15 +165,15 @@
     if isinstance(error, WebException):
         task.result = error.dict()
     elif isinstance(error, Exception):
         task.result = dict(
             error_class=error.__class__.__name__,
             error_message=str(error),
             error_status_code=500,
-            error_traceback=error.__traceback__,
+            error_traceback=format_tb(error.__traceback__),
             error_payload={}
         )
     else:
         task.result = error
 
     if task.retry and (task.max_retries is None or task.max_retries != 0):
         task.status = "retry"
```

### Comparing `eventix-0.3.3/eventix/functions/task_scheduler.py` & `eventix-0.4.0/eventix/functions/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.3/eventix/functions/task_worker.py` & `eventix-0.4.0/eventix/functions/task_worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,67 @@
+from __future__ import annotations
+
 import importlib
 import logging
+import os
+import sys
 import time
 from typing import List
 
+import dotenv
 from pydantic_db_backend.utils import utcnow
 
 from eventix.exceptions import TaskNotRegistered, backend_exceptions
-from eventix.functions.core import EventflowTaskBase, namespace_context, worker_id_context
+from eventix.functions.core import EventflowTaskBase, namespace_context, worker_id_context, namespace_provider
 from eventix.functions.errors import raise_errors
 from eventix.functions.eventix_client import EventixClient
-from eventix.functions.task import task_set_error
+from eventix.functions.task import task_set_error, task_set_result
 from eventix.pydantic.task import TaskModel
 
 log = logging.getLogger(__name__)
 
 
 class TaskWorker(EventixClient):
     _wait_interval = 10
     _tasks = {}
+    namespace: str = None
+
+    @classmethod
+    def setup_logging(cls, without_time: bool = False, level: int = logging.INFO):
+        if without_time:
+            f = "[%(levelname)8s] %(message)s"
+        else:
+            f = "%(asctime)s [%(levelname)s] %(message)s"
+        logging.basicConfig(
+            level=level,
+            format=f,
+            handlers=[
+                logging.StreamHandler()
+            ]
+        )
+
+    @classmethod
+    def config(cls, config: dict):
+
+        base_url = os.environ.get("EVENTIX_URL", "")
+        if base_url == "":
+            log.error("No EVENTIX_URL set.")
+            sys.exit()
+
+        cls.set_base_url(base_url)
+
+        if "register_tasks" in config:
+            cls.register_tasks(config['register_tasks'])
+
+        if "namespace" in config:
+            cls.namespace = config['namespace']
+
+        namespace = os.environ.get("EVENTIX_NAMESPACE", "")
+        if namespace != "":
+            cls.namespace = namespace
 
     @classmethod
     def register_tasks(cls, paths=List[str]):
         log.info("registering tasks...")
         # noinspection PyTypeChecker
         for path in paths:
             try:
@@ -46,24 +86,25 @@
                 r = cls.interface.get(f'/task/next_scheduled', params=params)
                 if r.status_code == 200:
                     tm = TaskModel.parse_raw(r.content)
                     return tm
                 else:
                     return None
 
-        # with raise_errors(r):
-        #     return TaskModel.parse_raw(r.content)
+    # with raise_errors(r):
+    #     return TaskModel.parse_raw(r.content)
 
     @classmethod
     def listen(cls, endless=True):
+        log.info("Start listening...")
         while True:
-            log.info("Start listening...")
+            log.info("Looking for tasks...")
             t = cls.task_next_scheduled()
             if t is not None:
-                pass
+                cls.execute_task(t)
             else:
                 log.info(f"Nothing to do... waiting {cls._wait_interval}s")
                 if not endless:
                     return
                 time.sleep(cls._wait_interval)
 
     @classmethod
@@ -73,34 +114,35 @@
 
             if task.task not in cls._tasks:
                 raise TaskNotRegistered(task=task.task)  # Task not registered in worker
 
             f = cls._tasks[task.task]
             r = f.run(*task.args, **task.kwargs)
             if task.store_result:
-                task.result = r
+                task_set_result(task, r)
 
         except TaskNotRegistered as e:
             log.exception(e)
             task_set_error(
                 task,
                 TaskNotRegistered(task=task.task)
             )
 
         except Exception as e:
+            log.exception(e)
             task_set_error(task, e)
 
         finally:
             cls.task_write_back(task)
 
     @classmethod
     def task_write_back(cls, task: TaskModel) -> TaskModel | None:
         try:
 
-            if task.expires < utcnow():
+            if task.expires is not None and task.expires < utcnow():  # gammel
                 # if task is already expired, delete it instead of updating
                 r = cls.interface.delete(f'/task/{task.uid}')
                 return None
             else:
                 # task not yet expired.... update
                 r = cls.interface.put(f'/task/{task.uid}', data=task.json())
 
@@ -112,7 +154,21 @@
         except Exception as e:
             log.error("Exception raised when calling eventix")
             log.exception(e)
             log.error("Exception used this task info")
             log.error(task.json())
 
         return None
+
+    @classmethod
+    def load_env(cls):
+        dotenv.load_dotenv(".env.local")
+
+    def __init__(self, config: dict) -> None:
+        self.setup_logging()
+        self.load_env()
+        self.config(config)
+
+    def start(self, endless: bool = True):
+        log.info(f"Using namespace: {self.namespace}")
+        with namespace_provider(self.namespace):
+            self.listen(endless)
```

### Comparing `eventix-0.3.3/eventix/pydantic/task.py` & `eventix-0.4.0/eventix/pydantic/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 from typing import Any, Dict, Tuple, Self, Type, Literal
 
 from pydantic import Field
 from webexception.webexception import WebException
 
 from pydantic_db_backend.backend import BackendModel
```

### Comparing `eventix-0.3.3/eventix/router/event.py` & `eventix-0.4.0/eventix/router/event.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.3/eventix/router/task.py` & `eventix-0.4.0/eventix/router/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.3.3/pyproject.toml` & `eventix-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "eventix"
-version = "0.3.3"
+version = "0.4.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-fastapi = "^0.95.1"
+fastapi = "^0.99.1"
 uvicorn = "^0.22.0"
 python-dotenv = "^0.15.0"
 pydash = "*"
-pydantic-db-backend = {version = "^0.4.2", extras = ["couchdb"]}
+pydantic-db-backend = {version = "^0.4.3", extras = ["couchdb"]}
 psutil = "^5.9.5"
 requests = "^2.31.0"
 toml = "^0.10.2"
 webexception = "^1.0.2"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `eventix-0.3.3/PKG-INFO` & `eventix-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: eventix
-Version: 0.3.3
+Version: 0.4.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: fastapi (>=0.99.1,<0.100.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: pydantic-db-backend[couchdb] (>=0.4.2,<0.5.0)
+Requires-Dist: pydantic-db-backend[couchdb] (>=0.4.3,<0.5.0)
 Requires-Dist: pydash
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: webexception (>=1.0.2,<2.0.0)
 Description-Content-Type: text/markdown
```

