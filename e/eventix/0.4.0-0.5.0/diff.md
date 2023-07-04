# Comparing `tmp/eventix-0.4.0.tar.gz` & `tmp/eventix-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventix-0.4.0.tar", max compression
+gzip compressed data, was "eventix-0.5.0.tar", max compression
```

## Comparing `eventix-0.4.0.tar` & `eventix-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/__init__.py
--rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.4.0/eventix/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/functions/__init__.py
--rw-r--r--   0        0        0     4402 2023-07-04 12:48:26.939576 eventix-0.4.0/eventix/functions/core.py
--rw-r--r--   0        0        0      709 2023-07-03 12:35:26.910564 eventix-0.4.0/eventix/functions/errors.py
--rw-r--r--   0        0        0      801 2023-07-04 06:52:56.282299 eventix-0.4.0/eventix/functions/eventix_client.py
--rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.4.0/eventix/functions/fastapi.py
--rw-r--r--   0        0        0     6125 2023-07-04 08:38:43.486260 eventix-0.4.0/eventix/functions/task.py
--rw-r--r--   0        0        0      990 2023-07-03 12:36:06.494329 eventix-0.4.0/eventix/functions/task_scheduler.py
--rw-r--r--   0        0        0     5482 2023-07-04 11:52:40.153974 eventix-0.4.0/eventix/functions/task_worker.py
--rw-r--r--   0        0        0      322 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/functions/tools.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/pydantic/__init__.py
--rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/pydantic/event.py
--rw-r--r--   0        0        0     1987 2023-07-04 12:48:48.055369 eventix-0.4.0/eventix/pydantic/task.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/router/__init__.py
--rw-r--r--   0        0        0      517 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/router/event.py
--rw-r--r--   0        0        0      236 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/router/metrics.py
--rw-r--r--   0        0        0     1201 2023-07-03 12:25:39.726933 eventix-0.4.0/eventix/router/task.py
--rw-r--r--   0        0        0      954 2023-07-04 13:10:17.297703 eventix-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 eventix-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-04 15:24:17.141091 eventix-0.5.0/eventix/contexts/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.5.0/eventix/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/functions/__init__.py
+-rw-r--r--   0        0        0     3500 2023-07-04 15:24:17.133091 eventix-0.5.0/eventix/functions/core.py
+-rw-r--r--   0        0        0      709 2023-07-03 12:35:26.910564 eventix-0.5.0/eventix/functions/errors.py
+-rw-r--r--   0        0        0      801 2023-07-04 06:52:56.282299 eventix-0.5.0/eventix/functions/eventix_client.py
+-rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.5.0/eventix/functions/fastapi.py
+-rw-r--r--   0        0        0     5982 2023-07-04 21:08:43.049808 eventix-0.5.0/eventix/functions/task.py
+-rw-r--r--   0        0        0     1155 2023-07-04 15:24:17.145091 eventix-0.5.0/eventix/functions/task_scheduler.py
+-rw-r--r--   0        0        0     5469 2023-07-04 15:24:17.137091 eventix-0.5.0/eventix/functions/task_worker.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/functions/tools.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/pydantic/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/pydantic/event.py
+-rw-r--r--   0        0        0     1987 2023-07-04 12:48:48.055369 eventix-0.5.0/eventix/pydantic/task.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/router/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/router/event.py
+-rw-r--r--   0        0        0      236 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/router/metrics.py
+-rw-r--r--   0        0        0     1201 2023-07-03 12:25:39.726933 eventix-0.5.0/eventix/router/task.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:28:16.696215 eventix-0.5.0/eventix/tasks/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-04 21:10:00.620848 eventix-0.5.0/eventix/tasks/cleanup.py
+-rw-r--r--   0        0        0      974 2023-07-04 21:15:38.476803 eventix-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 eventix-0.5.0/PKG-INFO
```

### Comparing `eventix-0.4.0/eventix/exceptions/__init__.py` & `eventix-0.5.0/eventix/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.4.0/eventix/functions/errors.py` & `eventix-0.5.0/eventix/functions/errors.py`

 * *Files identical despite different names*

### Comparing `eventix-0.4.0/eventix/functions/eventix_client.py` & `eventix-0.5.0/eventix/functions/eventix_client.py`

 * *Files identical despite different names*

### Comparing `eventix-0.4.0/eventix/functions/fastapi.py` & `eventix-0.5.0/eventix/functions/fastapi.py`

 * *Files identical despite different names*

### Comparing `eventix-0.4.0/eventix/functions/task.py` & `eventix-0.5.0/eventix/functions/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,21 +67,20 @@
             log.debug(f"updated task {updated_task.uid}")
             # noinspection PyTypeChecker
             return updated_task  # update worked
         except RevisionConflict as e:
             continue  # try again.
 
 
-def task_clean_expired_workers(namespace: str):
+def task_clean_expired_workers():
     params = dict(
         model=TaskModel,
         skip=0,
         limit=1,
         query_filter=dict(
-            namespace=namespace,  # namespace has to match
             worker_expires={
                 "$and": [
                     {"$ne": None},
                     {"$lt": utcnow()},
                 ]
             }  # no worker assigned
         ),
@@ -110,17 +109,14 @@
         except RevisionConflict as e:
             continue
 
 
 def task_next_scheduled(worker_id: str, namespace: str, expires: int = 300) -> TaskModel | None:
     log.debug(f"[{worker_id}] Worker getting next scheduled task...")
 
-    # clean worker expires
-
-    task_clean_expired_workers(namespace)
 
     # looking up possible tasks in right order
     # take first one
     # try to set worker_id and expiration
 
     eta = utcnow().isoformat()  # eta has to be now or in the past
```

### Comparing `eventix-0.4.0/eventix/functions/task_scheduler.py` & `eventix-0.5.0/eventix/functions/task_scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import logging
 
+from eventix.contexts import namespace_context
 from eventix.exceptions import backend_exceptions
 from eventix.functions.errors import raise_errors
 from eventix.functions.eventix_client import EventixClient
 from eventix.pydantic.task import TaskModel
 
 log = logging.getLogger(__name__)
 
 
 class TaskScheduler(EventixClient):
 
     @classmethod
     def schedule(cls, task: TaskModel) -> TaskModel:
-        log.debug(f"scheduling task: {task.task} uid: {task.uid} eta: {task.eta} unique_key: {task.unique_key}")
-        task.namespace = cls.namespace
+        if task.namespace is None:
+            with namespace_context() as namespace:
+                task.namespace = namespace
+        log.debug(f"scheduling task: {task.task} namespace: {task.namespace} uid: {task.uid} eta: {task.eta} unique_key: {task.unique_key}")
         return cls.task_post(task)
 
     @classmethod
     def task_get(cls, uid: str) -> TaskModel:
         r = cls.interface.get(f'/task/{uid}')
         with raise_errors(r, backend_exceptions):
             return TaskModel.parse_raw(r.content)
```

### Comparing `eventix-0.4.0/eventix/functions/task_worker.py` & `eventix-0.5.0/eventix/functions/task_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 import sys
 import time
 from typing import List
 
 import dotenv
 from pydantic_db_backend.utils import utcnow
 
+from eventix.contexts import worker_id_context, namespace_provider
 from eventix.exceptions import TaskNotRegistered, backend_exceptions
-from eventix.functions.core import EventflowTaskBase, namespace_context, worker_id_context, namespace_provider
+from eventix.functions.core import EventixTaskBase, namespace_context
 from eventix.functions.errors import raise_errors
 from eventix.functions.eventix_client import EventixClient
 from eventix.functions.task import task_set_error, task_set_result
 from eventix.pydantic.task import TaskModel
 
 log = logging.getLogger(__name__)
 
@@ -55,23 +56,24 @@
         if "namespace" in config:
             cls.namespace = config['namespace']
 
         namespace = os.environ.get("EVENTIX_NAMESPACE", "")
         if namespace != "":
             cls.namespace = namespace
 
+
     @classmethod
     def register_tasks(cls, paths=List[str]):
         log.info("registering tasks...")
         # noinspection PyTypeChecker
         for path in paths:
             try:
                 imported_module = importlib.import_module(path)
                 for f in filter(
-                    lambda x: isinstance(x, EventflowTaskBase),
+                    lambda x: isinstance(x, EventixTaskBase),
                     [getattr(imported_module, x) for x in dir(imported_module)]
                 ):
                     log.info(f"registered '{f.func_name}' from {path}")
                     cls._tasks[f.func_name] = f
             except ImportError as e:
                 print(e)
 
@@ -113,16 +115,15 @@
             log.info(f"Executing task: {task.task} uid: {task.uid} ...")
 
             if task.task not in cls._tasks:
                 raise TaskNotRegistered(task=task.task)  # Task not registered in worker
 
             f = cls._tasks[task.task]
             r = f.run(*task.args, **task.kwargs)
-            if task.store_result:
-                task_set_result(task, r)
+            task_set_result(task, r)
 
         except TaskNotRegistered as e:
             log.exception(e)
             task_set_error(
                 task,
                 TaskNotRegistered(task=task.task)
             )
```

### Comparing `eventix-0.4.0/eventix/pydantic/task.py` & `eventix-0.5.0/eventix/pydantic/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.4.0/eventix/router/event.py` & `eventix-0.5.0/eventix/router/event.py`

 * *Files identical despite different names*

### Comparing `eventix-0.4.0/eventix/router/task.py` & `eventix-0.5.0/eventix/router/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.4.0/pyproject.toml` & `eventix-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventix"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.99.1"
@@ -12,14 +12,15 @@
 python-dotenv = "^0.15.0"
 pydash = "*"
 pydantic-db-backend = {version = "^0.4.3", extras = ["couchdb"]}
 psutil = "^5.9.5"
 requests = "^2.31.0"
 toml = "^0.10.2"
 webexception = "^1.0.2"
+croniter = "^1.4.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 httpx = "^0.24.1"
 freezegun = "^1.2.2"
 coverage = "^7.2.7"
```

### Comparing `eventix-0.4.0/PKG-INFO` & `eventix-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: eventix
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: croniter (>=1.4.1,<2.0.0)
 Requires-Dist: fastapi (>=0.99.1,<0.100.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pydantic-db-backend[couchdb] (>=0.4.3,<0.5.0)
 Requires-Dist: pydash
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

