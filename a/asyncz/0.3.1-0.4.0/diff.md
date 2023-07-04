# Comparing `tmp/asyncz-0.3.1.tar.gz` & `tmp/asyncz-0.4.0.tar.gz`

## Comparing `asyncz-0.3.1.tar` & `asyncz-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/_mapping.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/datastructures.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/enums.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/py.typed
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/state.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/typing.py
--rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/contrib/esmerald/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/contrib/esmerald/decorator.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/contrib/esmerald/scheduler.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/events/__init__.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/events/base.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/events/constants.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/executors/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/executors/asyncio.py
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/executors/base.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/executors/debug.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/executors/pool.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/executors/types.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/schedulers/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/schedulers/asyncio.py
--rw-r--r--   0        0        0    39976 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/schedulers/base.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/schedulers/datastructures.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/schedulers/types.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/schedulers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/stores/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/stores/base.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/stores/memory.py
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/stores/mongo.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/stores/redis.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/stores/types.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/tasks/__init__.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/tasks/base.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/tasks/types.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/__init__.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/base.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/combination.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/date.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/interval.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/types.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/cron/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/cron/constants.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/cron/expressions.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/cron/fields.py
--rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/cron/trigger.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 asyncz-0.3.1/asyncz/triggers/cron/types.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 asyncz-0.3.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 asyncz-0.3.1/LICENSE
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 asyncz-0.3.1/README.md
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 asyncz-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 asyncz-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/_mapping.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/datastructures.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/enums.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/py.typed
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/state.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/typing.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/contrib/esmerald/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/contrib/esmerald/decorator.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/contrib/esmerald/scheduler.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/events/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/events/base.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/events/constants.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/asyncio.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/base.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/debug.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/pool.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/types.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/__init__.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/asyncio.py
+-rw-r--r--   0        0        0    39886 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/base.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/datastructures.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/types.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/__init__.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/base.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/memory.py
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/mongo.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/redis.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/types.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/tasks/__init__.py
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/tasks/base.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/tasks/types.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/__init__.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/base.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/combination.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/date.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/interval.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/types.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/constants.py
+-rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/expressions.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/fields.py
+-rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/trigger.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/types.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 asyncz-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 asyncz-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 asyncz-0.4.0/README.md
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 asyncz-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 asyncz-0.4.0/PKG-INFO
```

### Comparing `asyncz-0.3.1/asyncz/_mapping.py` & `asyncz-0.4.0/asyncz/_mapping.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/exceptions.py` & `asyncz-0.4.0/asyncz/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/utils.py` & `asyncz-0.4.0/asyncz/utils.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/contrib/esmerald/decorator.py` & `asyncz-0.4.0/asyncz/contrib/esmerald/decorator.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/contrib/esmerald/scheduler.py` & `asyncz-0.4.0/asyncz/contrib/esmerald/scheduler.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/events/base.py` & `asyncz-0.4.0/asyncz/events/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from datetime import datetime
 from typing import Any, List, Optional, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 
 class SchedulerEvent(BaseModel):
     """
     The event itself.
 
     Args:
         code: The code type for the event
         alias: The alias given to store or executor.
     """
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
     code: Union[int, int]
-    alias: Optional[str]
-
-    class Config:
-        arbitrary_types_allowed = True
+    alias: Optional[str] = None
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} (code={self.code})>"
 
 
 class TaskEvent(SchedulerEvent):
     """
@@ -29,15 +27,15 @@
 
     Args:
         task_id: The identifier given to a task.
         store: The alias given to a store.
     """
 
     task_id: Union[str, int]
-    store: Union[str, Any]
+    store: Union[str, Any] = None
 
 
 class TaskSubmissionEvent(TaskEvent):
     """
     Event related to the submission of a task.
 
     Args:
@@ -55,10 +53,10 @@
         scheduled_run_times: The time when the task was scheduled to be run.
         return_value: The return value of the task successfully executed.
         exception: The exception raised by the task.
         traceback: A formated traceback for the exception.
     """
 
     scheduled_run_time: Union[int, str, Any]
-    return_value: Any
-    exception: Optional[Exception]
-    traceback: Optional[str]
+    return_value: Any = None
+    exception: Optional[Exception] = None
+    traceback: Optional[str] = None
```

### Comparing `asyncz-0.3.1/asyncz/events/constants.py` & `asyncz-0.4.0/asyncz/events/constants.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/executors/asyncio.py` & `asyncz-0.4.0/asyncz/executors/asyncio.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/executors/base.py` & `asyncz-0.4.0/asyncz/executors/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/executors/debug.py` & `asyncz-0.4.0/asyncz/executors/debug.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/executors/pool.py` & `asyncz-0.4.0/asyncz/executors/pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import concurrent.futures
 from abc import abstractmethod
 from concurrent.futures.process import BrokenProcessPool
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, List, Optional
 
+from pydantic import ConfigDict
+
 from asyncz.executors.base import BaseExecutor, run_task
-from asyncz.typing import DictAny
 
 if TYPE_CHECKING:
     from asyncz.tasks.types import TaskType
 
 
 class BasePoolExecutor(BaseExecutor):
+    model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True, populate_by_name=True)
+
     @abstractmethod
-    def __init__(self, pool: Any, **kwargs: "DictAny"):
+    def __init__(self, pool: Any, **kwargs: Any):
         super().__init__(**kwargs)
         self.pool = pool
 
     def do_send_task(self, task: "TaskType", run_times: List[datetime]) -> Any:
         def callback(fn):
             exc, _ = (
                 fn.exception_info()
@@ -37,31 +40,25 @@
             fn = self.pool.submit(run_task, task, task.store_alias, run_times, self.logger)
 
         fn.add_done_callback(callback)
 
     def shutdown(self, wait=True):
         self.pool.shutdown(wait)
 
-    class Config(BaseExecutor.Config):
-        allow_population_by_field_name = True
-
 
 class ThreadPoolExecutor(BasePoolExecutor):
     """
     An executor that runs tasks in a concurrent.futures thread pool.
 
     Args:
         max_workers: The maximum number of spawned threads.
         pool_kwargs: Dict of keyword arguments to pass to the underlying ThreadPoolExecutor constructor.
     """
 
-    max_workers: Optional[int]
-    pool_kwargs: Optional["DictAny"]
-
-    def __init__(self, max_workers: int = 10, pool_kwargs: Optional["DictAny"] = None):
+    def __init__(self, max_workers: int = 10, pool_kwargs: Optional[Any] = None):
         pool_kwargs = pool_kwargs or {}
         pool = concurrent.futures.ThreadPoolExecutor(int(max_workers), **pool_kwargs)
         super().__init__(pool)
 
 
 class ProcessPoolExecutor(BasePoolExecutor):
     """
@@ -69,14 +66,11 @@
 
     Args:
         max_workers: The maximum number of spawned processes.
         pool_kwargs: Dict of keyword arguments to pass to the underlying
             ProcessPoolExecutor constructor.
     """
 
-    max_workers: Optional[int]
-    pool_kwargs: Optional["DictAny"]
-
-    def __init__(self, max_workers: int = 10, pool_kwargs: Optional["DictAny"] = None):
+    def __init__(self, max_workers: int = 10, pool_kwargs: Optional[Any] = None):
         pool_kwargs = pool_kwargs or {}
         pool = concurrent.futures.ProcessPoolExecutor(int(max_workers), **pool_kwargs)
         super().__init__(pool)
```

### Comparing `asyncz-0.3.1/asyncz/schedulers/asyncio.py` & `asyncz-0.4.0/asyncz/schedulers/asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 from typing import Any, Optional
 
 from asyncz.executors.asyncio import AsyncIOExecutor
 from asyncz.schedulers.base import BaseScheduler
 from asyncz.schedulers.utils import run_in_event_loop
-from asyncz.typing import DictAny
 from asyncz.utils import maybe_ref
 
 
 class AsyncIOScheduler(BaseScheduler):
     """
     A scheduler that runs on an asyncio event loop.
 
@@ -16,15 +15,15 @@
     use it internally if needed. For example, Esmerald and Starlette.
 
     Args:
         event_loop: AsyncOP event loop to use. Default to the global event loop.
     """
 
     def __init__(
-        self, event_loop: Optional[Any] = None, timeout: Optional[int] = None, **kwargs: "DictAny"
+        self, event_loop: Optional[Any] = None, timeout: Optional[int] = None, **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         self.event_loop = event_loop
         self.timeout = timeout
 
     def start(self, paused: bool = False):
         if not self.event_loop:
@@ -32,15 +31,15 @@
         super().start(paused)
 
     @run_in_event_loop
     def shutdown(self, wait: bool = True):
         super().shutdown(wait)
         self.stop_timer()
 
-    def _setup(self, config: "DictAny") -> None:
+    def _setup(self, config: Any) -> None:
         self.event_loop = maybe_ref(config.pop("event_loop", None))
         super()._setup(config)
 
     def start_timer(self, wait_seconds: Optional[int] = None):
         self.stop_timer()
         if wait_seconds is not None:
             self.timeout = self.event_loop.call_later(wait_seconds, self.wakeup)
```

### Comparing `asyncz-0.3.1/asyncz/schedulers/base.py` & `asyncz-0.4.0/asyncz/schedulers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             the list of due tasks.
         task_defaults: Default values for newly added tasks.
         stores: A dictionary of task store alias -> task store instance or configuration dict.
         executors: A dictionary of executor alias -> executor instance or configuration dict.
         state: current running state of the scheduler.
     """
 
-    def __init__(self, global_config: Optional["DictAny"] = None, **kwargs: "DictAny") -> None:
+    def __init__(self, global_config: Optional[Any] = None, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         mapping = AsynczObjectMapping()
         self.global_config = global_config or {}
         self.trigger_plugins = dict(mapping.triggers.items())
         self.trigger_classes = {}
         self.executor_plugins = dict(mapping.executors.items())
         self.executor_classes = {}
@@ -105,17 +105,17 @@
             "Schedulers cannot be serialized. Ensure that you are not passing a "
             "scheduler instance as an argument to a task, or scheduling an instance "
             "method where the instance contains a scheduler as an attribute."
         )
 
     def setup(
         self,
-        global_config: Optional["DictAny"] = None,
+        global_config: Optional[Any] = None,
         prefix: Optional[str] = "asyncz.",
-        **options: "DictAny",
+        **options: Any,
     ):
         """
         Reconfigures the scheduler with the given options.
         Can only be done when the scheduler isn't running.
 
         Args:
             global_config: a "global" configuration dictionary whose values can be overridden by
@@ -241,15 +241,15 @@
         """
         Return True if the scheduler has been started. This is a shortcut
         for scheduler.state != SchedulerState.STATE_STOPPED.
         """
         return self.state != SchedulerState.STATE_STOPPED
 
     def add_executor(
-        self, executor: "ExecutorType", alias: str = "default", **executor_options: "DictAny"
+        self, executor: "ExecutorType", alias: str = "default", **executor_options: Any
     ):
         with self.executor_lock:
             if alias in self.executors:
                 raise ValueError(
                     f"This scheduler already has an executor by the alias of '{alias}'."
                 )
 
@@ -278,15 +278,15 @@
             del self.executors[alias]
 
         if shutdown:
             executor.shutdown()
 
         self.dispatch_event(SchedulerEvent(code=EXECUTOR_REMOVED, alias=alias))
 
-    def add_store(self, store: "StoreType", alias: str = "default", **store_options: "DictAny"):
+    def add_store(self, store: "StoreType", alias: str = "default", **store_options: Any):
         """
         Adds a task store to this scheduler.
 
         Any extra keyword arguments will be passed to the task store plugin's constructor, assuming
         that the first argument is the name of a task store plugin.
         """
         with self.store_lock:
@@ -354,25 +354,25 @@
                     del self.listeners[index]
 
     def add_task(
         self,
         fn: Optional[Callable[..., Any]],
         trigger: Optional[Union["TriggerType", str]] = None,
         args: Optional[Any] = None,
-        kwargs: Optional["DictAny"] = None,
+        kwargs: Optional[Any] = None,
         id: Optional[str] = None,
         name: Optional[str] = None,
         mistrigger_grace_time: Optional[int] = undefined,
         coalesce: Optional[bool] = undefined,
         max_instances: Optional[int] = undefined,
         next_run_time: Optional[Union[datetime, str]] = undefined,
         store: str = "default",
         executor: str = "default",
         replace_existing: bool = False,
-        **trigger_args: "DictAny",
+        **trigger_args: Any,
     ) -> "TaskType":
         """
         Adds the given task to the task list and wakes up the scheduler if it's already running.
 
         Any option that defaults to undefined will be replaced with the corresponding default
         value when the task is scheduled (which happens when the scheduler is started, or
         immediately if the scheduler is already running).
@@ -432,24 +432,24 @@
                 self.real_add_task(task, store, replace_existing)
         return task
 
     def scheduled_task(
         self,
         trigger: Optional[Union["TriggerType", str]] = None,
         args: Optional[Any] = None,
-        kwargs: Optional["DictAny"] = None,
+        kwargs: Optional[Any] = None,
         id: Optional[str] = None,
         name: Optional[str] = None,
         mistrigger_grace_time: Optional[int] = undefined,
         coalesce: Optional[bool] = undefined,
         max_instances: Optional[int] = undefined,
         next_run_time: Optional[Union[datetime, str]] = undefined,
         store: str = "default",
         executor: str = "default",
-        **trigger_args: "DictAny",
+        **trigger_args: Any,
     ):
         """
         Functionality that can be used as a decorator for any function to schedule a task with a difference that replace_existing is always True.
 
         Args:
             trigger: Trigger that determines when fn is called.
             args: List of positional arguments to call fn with.
@@ -485,15 +485,15 @@
                 **trigger_args,
             )
             return fn
 
         return wrap
 
     def update_task(
-        self, task_id: Union[int, str], store: Optional[str] = None, **updates: "DictAny"
+        self, task_id: Union[int, str], store: Optional[str] = None, **updates: Any
     ) -> "TaskType":
         """
         Modifies the propertues of a single task.
 
         Modifications are passed to this method as extra keyword arguments.
 
         Args:
@@ -514,15 +514,15 @@
         return task
 
     def reschedule_task(
         self,
         task_id: Union[int, str],
         store: Optional[str] = None,
         trigger: Optional[str] = None,
-        **trigger_args: "DictAny",
+        **trigger_args: Any,
     ) -> "TaskType":
         """
         Constructs a new trigger for a task and updates its next run time.
 
         Extra keyword arguments are passed directly to the trigger's constructor.
 
         Args:
@@ -660,15 +660,15 @@
     def wakeup(self):
         """
         Notifies the scheduler that there may be tasks due for execution.
         Triggers process_tasks to be run in an implementation specific manner.
         """
         ...
 
-    def _setup(self, config: "DictAny") -> None:
+    def _setup(self, config: Any) -> None:
         """
         Applies initial configurations called by the Base constructor.
         """
         self.logger = maybe_ref(config.pop("logger", None)) or logger
         self.timezone = to_timezone(config.pop("timezone", None)) or get_localzone()
         self.store_retry_interval = float(config.pop("store_retry_interval", 10))
 
@@ -866,15 +866,15 @@
         module = import_module(module_path)
 
         try:
             return getattr(module, class_name)
         except AttributeError as exc:
             raise ImportError(str(exc)) from exc
 
-    def create_plugin_instance(self, _type: str, alias: str, constructor_args: "DictAny"):
+    def create_plugin_instance(self, _type: str, alias: str, constructor_args: Any):
         """
         Creates an instance of the given plugin type, loading the plugin first if necessary.
         """
         plugin_container, class_container, base_class = {
             "trigger": (self.trigger_plugins, self.trigger_classes, BaseTrigger),
             "store": (self.store_plugins, self.store_classes, BaseStore),
             "executor": (self.executor_plugins, self.executor_classes, BaseExecutor),
@@ -893,15 +893,15 @@
                         f"The {format(_type)} entry point does not point to a {format(_type)} class."
                     ) from None
             else:
                 raise LookupError(f"No {_type} by the name '{alias}' was found.") from None
 
         return plugin_cls(**constructor_args)
 
-    def create_trigger(self, trigger: "TriggerType", trigger_args: "DictAny") -> Any:
+    def create_trigger(self, trigger: "TriggerType", trigger_args: Any) -> Any:
         """
         Creates a trigger.
         """
         if isinstance(trigger, BaseTrigger):
             return trigger
         elif trigger is None:
             trigger = "date"
```

### Comparing `asyncz-0.3.1/asyncz/schedulers/datastructures.py` & `asyncz-0.4.0/asyncz/schedulers/datastructures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from datetime import datetime
 from typing import Any, Callable, Optional, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from asyncz.triggers.types import TriggerType
-from asyncz.typing import DictAny, UndefinedType
+from asyncz.typing import UndefinedType
 
 
 class BaseStruct(BaseModel):
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 class TaskStruct(BaseStruct):
     """
     fn: Callable (or a textual reference to one) to run at the given time.
     trigger: Trigger that determines when fn is called.
     args: List of positional arguments to call fn with.
@@ -31,15 +30,15 @@
     executor: Alias of the executor to run the task with.
     """
 
     trigger: Optional[TriggerType]
     executor: Optional[str]
     fn: Optional[Callable[..., Any]]
     args: Optional[Any]
-    kwargs: Optional["DictAny"]
+    kwargs: Optional[Any]
     id: Optional[str]
     name: Optional[str]
     mistrigger_grace_time: Optional[Union[int, "UndefinedType"]]
     coalesce: Optional[Union[bool, "UndefinedType"]]
     max_instances: Optional[Union[int, "UndefinedType"]]
     next_run_time: Optional[Union[datetime, str]]
```

### Comparing `asyncz-0.3.1/asyncz/stores/base.py` & `asyncz-0.4.0/asyncz/stores/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from loguru import logger
 
 from asyncz.state import BaseStateExtra
-from asyncz.typing import DictAny
 
 if TYPE_CHECKING:
     from asyncz.tasks.types import TaskType
 
 
 class BaseStore(BaseStateExtra, ABC):
     """
     Base class for all task stores.
     """
 
     def __init__(
-        self, scheduler: Optional[Any] = None, alias: Optional[str] = None, **kwargs: "DictAny"
+        self, scheduler: Optional[Any] = None, alias: Optional[str] = None, **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         self.logger = logger
         self.scheduler = scheduler
         self.alias = alias
 
     def start(self, scheduler: Any, alias: str):
```

### Comparing `asyncz-0.3.1/asyncz/stores/memory.py` & `asyncz-0.4.0/asyncz/stores/memory.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/stores/mongo.py` & `asyncz-0.4.0/asyncz/stores/mongo.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/stores/redis.py` & `asyncz-0.4.0/asyncz/stores/redis.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/tasks/base.py` & `asyncz-0.4.0/asyncz/tasks/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import inspect
 from datetime import datetime
-from typing import Any, Iterable, List, Mapping, Optional
+from typing import TYPE_CHECKING, Any, Callable, Iterable, List, Mapping, Optional, Union
 from uuid import uuid4
 
 from asyncz.datastructures import TaskState
 from asyncz.state import BaseStateExtra
 from asyncz.triggers.base import BaseTrigger
-from asyncz.typing import DictAny
 from asyncz.utils import (
     check_callable_args,
     datetime_repr,
     get_callable_name,
     obj_to_ref,
     ref_to_obj,
     repr_escape,
     to_datetime,
 )
 
 object_setattr = object.__setattr__
 
+if TYPE_CHECKING:
+    from asyncz.stores.types import StoreType
+    from asyncz.triggers.types import TriggerType
+else:
+    StoreType = Any
+    TriggerType = Any
+
 
 class Task(BaseStateExtra):
     """
     Contains the options given when scheduling callables and its current schedule and other state.
     This class should never be instantiated by the user.
 
     Args:
@@ -38,35 +44,42 @@
         mistrigger_grace_time: The time (in seconds) how much this task's execution is allowed to
             be late (`None` means "allow the task to run no matter how late it is").
         max_instances: The maximum number of concurrently executing instances allowed for this
             task.
         next_run_time: The next scheduled run time of this task.
     """
 
+    name: Optional[str] = None
+    fn: Optional[Union[Callable[..., Any], str]] = None
+    fn_reference: Optional[str] = None
+    args: Optional[Any] = None
+    kwargs: Optional[Any] = None
+    next_run_time: Optional[datetime] = None
+
     def __init__(
         self,
         scheduler: Any,
         id: Optional[str] = None,
         store_alias: Optional[str] = None,
-        **kwargs: "DictAny",
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.scheduler = scheduler
         self.store_alias = store_alias
         self._update(id=id or uuid4().hex, **kwargs)
 
     @property
     def pending(self):
         """
         Returns true if the referenced task is still waiting to be added to its designated task
         store.
         """
         return self.store_alias is None
 
-    def update(self, **updates: "DictAny") -> "Task":
+    def update(self, **updates: Any) -> "Task":
         """
         Makes the given updates to this jon and save it in the associated store.
         Accepted keyword args are the same as the class variables.
         """
         self.scheduler.update_task(self.id, self.store_alias, **updates)
         return self
 
@@ -103,15 +116,15 @@
         run_times = []
         next_run_time = self.next_run_time
         while next_run_time and next_run_time <= now:
             run_times.append(next_run_time)
             next_run_time = self.trigger.get_next_trigger_time(next_run_time, now)
         return run_times
 
-    def _update(self, **updates: "DictAny") -> None:
+    def _update(self, **updates: Any) -> None:
         """
         Validates the updates to the Task and makes the modifications if and only if all of them
         validate.
         """
         approved = {}
         if "id" in updates:
             _id = updates.pop("id")
@@ -202,15 +215,15 @@
             )
 
         for key, value in approved.items():
             setattr(self, key, value)
 
     def __setstate__(self, state):
         object_setattr(self, "__dict__", state.__dict__)
-        object_setattr(self, "__fields_set__", state.__fields_set__)
+        object_setattr(self, "__pydantic_fields_set__", state.__pydantic_fields_set__)
 
         for name, value in self.__dict__.items():
             if name == "fn":
                 self.__dict__[name] = ref_to_obj(value)
 
         for name, value in state.__private_attributes__.items():
             if name == "fn":
```

### Comparing `asyncz-0.3.1/asyncz/triggers/base.py` & `asyncz-0.4.0/asyncz/triggers/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import random
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from asyncz.datastructures import CombinationState
 from asyncz.state import BaseStateExtra
-from asyncz.typing import DictAny
 from asyncz.utils import obj_to_ref, ref_to_obj
 
 if TYPE_CHECKING:
     from asyncz.triggers.types import TriggerType
 
 
 class BaseTrigger(BaseStateExtra, ABC):
@@ -57,15 +56,15 @@
         jitter: he maximum number of second to add to the next_trigger_time.
     """
 
     def __init__(
         self,
         triggers: List["TriggerType"],
         jitter: Optional[int] = None,
-        **kwargs: "DictAny",
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.triggers = triggers
         self.jitter = jitter
 
     def __getstate__(self) -> "CombinationState":
         triggers = [
```

### Comparing `asyncz-0.3.1/asyncz/triggers/combination.py` & `asyncz-0.4.0/asyncz/triggers/combination.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/triggers/date.py` & `asyncz-0.4.0/asyncz/triggers/date.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import datetime, tzinfo
-from typing import Any, Dict, Optional, Union
+from typing import Any, Optional, Union
 
 from tzlocal import get_localzone
 
 from asyncz.datastructures import DateState
 from asyncz.triggers.base import BaseTrigger
-from asyncz.typing import DictAny
 from asyncz.utils import datetime_repr, to_datetime, to_timezone
 
 
 class DateTrigger(BaseTrigger):
     """
     Triggers once on the given datetime. If run_at is left empty then the current time is used.
 
@@ -20,15 +19,15 @@
 
     alias: str = "date"
 
     def __init__(
         self,
         run_at: Optional[Union[datetime, str]] = None,
         timezone: Optional[Union[tzinfo, str]] = None,
-        **kwargs: Dict[str, Any],
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         timezone = to_timezone(timezone) or get_localzone()
         if run_at is not None:
             self.run_at = to_datetime(run_at, timezone, "run_at")
         else:
             self.run_at = datetime.now(timezone)
@@ -36,15 +35,15 @@
     def get_next_trigger_time(
         self, previous_time: datetime, now: Optional[datetime] = None
     ) -> Union[datetime, None]:
         if previous_time is None:
             return self.run_at
         return None
 
-    def __getstate__(self) -> "DictAny":
+    def __getstate__(self) -> Any:
         """
         Handles the conversion to a dict to be able to pickle.
         """
         state = DateState(run_at=self.run_at)
         return state
 
     def __str__(self) -> str:
```

### Comparing `asyncz-0.3.1/asyncz/triggers/interval.py` & `asyncz-0.4.0/asyncz/triggers/interval.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from datetime import datetime, timedelta, tzinfo
 from math import ceil
-from typing import Any, Dict, Optional, Union
+from typing import Any, Optional, Union
 
 from tzlocal import get_localzone
 
 from asyncz.datastructures import IntervalState
 from asyncz.triggers.base import BaseTrigger
-from asyncz.typing import DictAny
 from asyncz.utils import datetime_repr, normalize, timedelta_seconds, to_datetime, to_timezone
 
 
 class IntervalTrigger(BaseTrigger):
     """
     Triggers on a specific intervals, starting on start_at if specified or datetime.now() + interval otherwise.
 
@@ -35,15 +34,15 @@
         hours: Optional[int] = 0,
         minutes: Optional[int] = 0,
         seconds: Optional[int] = 0,
         start_at: Optional[Union[datetime, str]] = None,
         end_at: Optional[Union[datetime, str]] = None,
         timezone: Optional[Union[tzinfo, str]] = None,
         jitter: Optional[int] = None,
-        **kwargs: Dict[str, Any],
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.interval = timedelta(
             weeks=weeks, days=days, hours=hours, minutes=minutes, seconds=seconds
         )
         self.interval_size = timedelta_seconds(self.interval)
 
@@ -64,15 +63,14 @@
         self.start_at = to_datetime(start_at, self.timezone, "start_at")
         self.end_at = to_datetime(end_at, self.timezone, "end_at")
         self.jitter = jitter
 
     def get_next_trigger_time(
         self, previous_time: datetime, now: datetime
     ) -> Union[datetime, None]:
-
         if previous_time:
             next_trigger_time = previous_time + self.interval
         elif self.start_at > now:
             next_trigger_time = self.start_at
         else:
             time_difference_seconds = timedelta_seconds(now - self.start_at)
             next_interval_number = int(ceil(time_difference_seconds / self.interval_size))
@@ -92,15 +90,15 @@
             start_at=self.start_at,
             end_at=self.end_at,
             interval=self.interval,
             jitter=self.jitter,
         )
         return state
 
-    def __setstate__(self, state: "DictAny") -> None:
+    def __setstate__(self, state: Any) -> None:
         trigger = super().__setstate__(state)
         trigger.interval_size = timedelta_seconds(self.interval)
 
     def __str__(self) -> str:
         return f"interval[{self.interval}]"
 
     def __repr__(self) -> str:
```

### Comparing `asyncz-0.3.1/asyncz/triggers/cron/constants.py` & `asyncz-0.4.0/asyncz/triggers/cron/constants.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/asyncz/triggers/cron/expressions.py` & `asyncz-0.4.0/asyncz/triggers/cron/expressions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import re
 from calendar import monthrange
 from datetime import date, datetime
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, ClassVar, Optional, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from asyncz.triggers.cron.constants import MAX_VALUES, MIN_VALUES, MONTHS, OPTIONS, WEEKDAYS
 from asyncz.utils import to_int
 
 if TYPE_CHECKING:
     from asyncz.triggers.cron.types import FieldType
 
 
 class BaseExpression(BaseModel):
-    class Config:
-        arbitrary_types_allowed = True
-        extra = "allow"
+    model_config = ConfigDict(arbitrary_types_allowed=True, extra="allow")
 
 
 class AllExpression(BaseExpression):
     regex: ClassVar[re.Pattern] = re.compile(r"\*(?:/(?P<step>\d+))?$")
-    step: Optional[Union[int, float]]
+    step: Optional[Union[int, float]] = None
 
-    def __init__(self, step: Optional[Union[int, float]] = None, **kwargs: Dict[str, Any]):
+    def __init__(self, step: Optional[Union[int, float]] = None, **kwargs: Any):
         super().__init__(**kwargs)
         if step:
             self.step = to_int(step)
             if self.step == 0:
                 raise ValueError("Increment must be higher than 0.")
 
     def validate_range(self, field_name: str) -> None:
@@ -64,22 +62,22 @@
         return f"{self.__class__.__name__}({self.step})"
 
 
 class RangeExpression(AllExpression):
     regex: ClassVar[re.Pattern] = re.compile(
         r"(?P<first>\d+)(?:-(?P<last>\d+))?(?:/(?P<step>\d+))?$"
     )
-    step: Optional[Union[int, float]]
+    step: Optional[Union[int, float]] = None
 
     def __init__(
         self,
         first: Union[str, float],
         last: Optional[Union[str, float]] = None,
         step: Optional[Union[int, float]] = None,
-        **kwargs: Dict[str, Any],
+        **kwargs: Any,
     ):
         super().__init__(step=step, **kwargs)
         first = to_int(first)
         last = to_int(last)  # type: ignore
 
         if last is None and self.step is None:
             last = first
@@ -151,15 +149,15 @@
         return f"{self.__class__.__name__}({', '.join(args)})"
 
 
 class MonthRangeExpression(RangeExpression):
     regex: ClassVar[re.Pattern] = re.compile(
         r"(?P<first>[a-z]+)(?:-(?P<last>[a-z]+))?", re.IGNORECASE
     )
-    step: Optional[Union[int, float]]
+    step: Optional[Union[int, float]] = None
 
     def __init__(
         self,
         first: Union[str, float],
         last: Optional[Union[str, float]] = None,
         **kwargs: Any,
     ) -> None:
@@ -240,15 +238,15 @@
 
 
 class WeekdayPositionExpression(AllExpression):
     regex: ClassVar[re.Pattern] = re.compile(
         r"(?P<option_name>%s) +(?P<weekday_name>(?:\d+|\w+))" % "|".join(OPTIONS), re.IGNORECASE
     )
 
-    def __init__(self, option_name: str, weekday_name: str, **kwargs: Dict[str, Any]):
+    def __init__(self, option_name: str, weekday_name: str, **kwargs: Any):
         super().__init__(step=None, **kwargs)
         try:
             self.option_number = OPTIONS.index(option_name.lower())
         except ValueError:
             raise ValueError(f'Invalid weekday position "{option_name}".') from None
 
         try:
@@ -289,15 +287,15 @@
             f"', '{WEEKDAYS[self.weekday]}')"
         )
 
 
 class LastDayOfMonthExpression(AllExpression):
     regex: ClassVar[re.Pattern] = re.compile(r"last", re.IGNORECASE)
 
-    def __init__(self, **kwargs: Dict[str, Any]) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         super().__init__(step=None, **kwargs)
 
     def get_next_value(self, date: Union[date, datetime], field: "FieldType"):  # type: ignore
         return monthrange(date.year, date.month)[1]
 
     def __str__(self) -> str:
         return "last"
```

### Comparing `asyncz-0.3.1/asyncz/triggers/cron/fields.py` & `asyncz-0.4.0/asyncz/triggers/cron/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from calendar import monthrange
 from datetime import datetime
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from asyncz.triggers.cron.constants import MAX_VALUES, MIN_VALUES
 from asyncz.triggers.cron.expressions import (
     AllExpression,
     LastDayOfMonthExpression,
     MonthRangeExpression,
     RangeExpression,
@@ -15,28 +15,29 @@
     WeekdayRangeExpression,
 )
 
 SEPARATOR = re.compile(" *, *")
 
 
 class BaseField(BaseModel):
-    name: Optional[str]
-    exprs: Optional[Any]
-    is_default: Optional[bool]
-    expressions: Optional[List[Any]]
-    compilers: Optional[List[Any]]
-    real: Optional[bool]
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+    name: Optional[str] = None
+    exprs: Optional[Any] = None
+    is_default: Optional[bool] = False
+    expressions: Optional[List[Any]] = None
+    compilers: Optional[List[Any]] = None
+    real: Optional[bool] = False
 
     def __init__(
         self,
         name: str,
         exprs: Any,
         is_default: Optional[bool] = False,
         compilers: Optional[List[Any]] = None,
-        **kwargs: Dict[str, Any]
+        **kwargs: Any
     ):
         super().__init__(**kwargs)
         self.name = name
         self.is_default = is_default
         self.exprs = exprs
         self.compilers = [AllExpression, RangeExpression]
 
@@ -91,51 +92,40 @@
     def __str__(self):
         expr_strings = (str(e) for e in self.expressions)
         return ",".join(expr_strings)
 
     def __repr__(self):
         return "{}('{}', '{}')".format(self.__class__.__name__, self.name, self)
 
-    class Config:
-        arbitrary_types_allowed = True
-
 
 class WeekField(BaseField):
-    def __init__(
-        self, name: str, exprs: Any, is_default: Optional[bool] = False, **kwargs: Dict[str, Any]
-    ):
+    def __init__(self, name: str, exprs: Any, is_default: Optional[bool] = False, **kwargs: Any):
         super().__init__(name, exprs, is_default, **kwargs)
         self.real: bool = False
 
     def get_value(self, dateval: datetime):
         return dateval.isocalendar()[1]
 
 
 class DayOfMonthField(BaseField):
-    def __init__(
-        self, name: str, exprs: Any, is_default: Optional[bool] = False, **kwargs: Dict[str, Any]
-    ):
+    def __init__(self, name: str, exprs: Any, is_default: Optional[bool] = False, **kwargs: Any):
         compilers = [WeekdayPositionExpression, LastDayOfMonthExpression]
         super().__init__(name, exprs, is_default, compilers=compilers, **kwargs)
 
     def get_max(self, dateval: datetime):
         return monthrange(dateval.year, dateval.month)[1]
 
 
 class DayOfWeekField(BaseField):
-    def __init__(
-        self, name: str, exprs: Any, is_default: Optional[bool] = False, **kwargs: Dict[str, Any]
-    ):
+    def __init__(self, name: str, exprs: Any, is_default: Optional[bool] = False, **kwargs: Any):
         compilers = [WeekdayRangeExpression]
         super().__init__(name, exprs, is_default, compilers=compilers, **kwargs)
         self.real: bool = False
 
     def get_value(self, dateval: datetime):
         return dateval.weekday()
 
 
 class MonthField(BaseField):
-    def __init__(
-        self, name: str, exprs: Any, is_default: Optional[bool] = False, **kwargs: Dict[str, Any]
-    ):
+    def __init__(self, name: str, exprs: Any, is_default: Optional[bool] = False, **kwargs: Any):
         compilers = [MonthRangeExpression]
         super().__init__(name, exprs, is_default, compilers=compilers, **kwargs)
```

### Comparing `asyncz-0.3.1/asyncz/triggers/cron/trigger.py` & `asyncz-0.4.0/asyncz/triggers/cron/trigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from datetime import datetime, timedelta, tzinfo
-from typing import Any, Dict, Optional, Union
+from typing import Any, Optional, Union
 
 from tzlocal import get_localzone
 
 from asyncz.datastructures import CronState
 from asyncz.triggers.base import BaseTrigger
 from asyncz.triggers.cron.constants import DEFAULT_VALUES
 from asyncz.triggers.cron.fields import (
     BaseField,
     DayOfMonthField,
     DayOfWeekField,
     MonthField,
     WeekField,
 )
-from asyncz.typing import DictAny
 from asyncz.utils import (
     datetime_ceil,
     datetime_repr,
     localize,
     normalize,
     to_datetime,
     to_timezone,
@@ -68,15 +67,15 @@
         hour: Optional[Union[int, str]] = None,
         minute: Optional[Union[int, str]] = None,
         second: Optional[Union[int, str]] = None,
         start_at: Optional[Union[datetime, str]] = None,
         end_at: Optional[Union[datetime, str]] = None,
         timezone: Optional[Union[tzinfo, str]] = None,
         jitter: Optional[int] = None,
-        **kwargs: Dict[str, Any],
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.year = year
         self.month = month
         self.day = day
         self.week = week
         self.day_of_week = day_of_week
@@ -251,25 +250,25 @@
             if self.end_at and next_date > self.end_at:
                 return None
 
         if fieldnum >= 0:
             next_date = self.apply_jitter(next_date, self.jitter, now)
             return min(next_date, self.end_at) if self.end_at else next_date
 
-    def __getstate__(self) -> "DictAny":
+    def __getstate__(self) -> Any:
         state = CronState(
             timezone=self.timezone,
             start_at=self.start_at,
             end_at=self.end_at,
             fields=self.fields,
             jitter=self.jitter,
         )
         return state
 
-    def __setstate__(self, state: "DictAny") -> Any:
+    def __setstate__(self, state: Any) -> Any:
         if isinstance(state, tuple):
             return state[1]
         super().__setstate__(state)
 
     def __str__(self):
         options = [f"{f.name}='{f}'" for f in self.fields if not f.is_default]
         return f"cron[{', '.join(options)}]"
```

### Comparing `asyncz-0.3.1/LICENSE` & `asyncz-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/README.md` & `asyncz-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `asyncz-0.3.1/pyproject.toml` & `asyncz-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "asyncio>=3.4.3,<4.0.0",
-    "loguru>=0.6.0,<0.7.0",
-    "pydantic>=1.10.9,<2.0.0",
+    "loguru>=0.7.0,<0.8.0",
+    "pydantic>=2.0.0,<3.0.0",
     "pytz>=2022.6",
     "tzlocal>=4.2,<5.0",
 ]
 keywords = [
     "api",
     "rest",
     "http",
@@ -69,15 +69,15 @@
 Documentation = "https://asyncz.tarsild.io/"
 Changelog = "https://asyncz.tarsild.io/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/tarsil/asyncz"
 
 [project.optional-dependencies]
 test = [
-    "esmerald==0.4.2",
+    # "esmerald==0.4.2",
     "mock>=4.0.3",
     "pymongo>=4.3.3,<5.0.0",
     "pytest >=7.1.3,<8.0.0",
     "pytest-cov >=2.12.0,<5.0.0",
     "pytest-asyncio >=0.19.0,<1.0.0",
     "pytest-loguru>=0.2.0,<1",
     "redis>=4.4.0,<5.0.0",
@@ -87,35 +87,29 @@
 
 dev = [
     "autoflake >=1.4.0,<3.0.0",
     "black>=22.10.0,<23.0.0",
     "flake8>=3.8.3,<7.0.0",
     "isort>=5.0.6,<6.0.0",
     "mypy>=0.982,<2.0.0",
-    "pre-commit >=2.17.0,<3.0.0",
-    "loguru>=0.6.0,<0.7.0",
+    "pre-commit>=2.17.0,<3.0.0",
     "watchfiles>=0.16.1,<0.20.0",
 ]
 
 doc = [
     "mkautodoc >=0.2.0,<0.3.0",
     "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=9.0.13,<10.0.0",
     "mdx-include >=1.4.2,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.2.5,<0.3.0",
     "mkdocstrings>=0.20.0,<0.30.0",
     "pyyaml >=6.0,<7.0.0",
 ]
 
-all = [
-    "asyncio>=3.4.3,<4.0.0",
-    "pydantic>=1.10.5,<2.0.0",
-    "pytz>=2022.6",
-    "tzlocal>=4.2,<5.0",
-]
+all = ["asyncio>=3.4.3,<4.0.0", "pytz>=2022.6", "tzlocal>=4.2,<5.0"]
 
 [tool.hatch.version]
 path = "asyncz/__init__.py"
 
 [tool.isort]
 profile = "black"
 known_third_party = ["asyncz", "pydantic", "starlette"]
```

### Comparing `asyncz-0.3.1/PKG-INFO` & `asyncz-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncz
-Version: 0.3.1
+Version: 0.4.0
 Summary: The scheduler that nobody wants but every application needs.
 Project-URL: Homepage, https://github.com/tarsil/asyncz
 Project-URL: Documentation, https://asyncz.tarsild.io/
 Project-URL: Changelog, https://asyncz.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/asyncz
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -33,42 +33,39 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: asyncio<4.0.0,>=3.4.3
-Requires-Dist: loguru<0.7.0,>=0.6.0
-Requires-Dist: pydantic<2.0.0,>=1.10.9
+Requires-Dist: loguru<0.8.0,>=0.7.0
+Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: pytz>=2022.6
 Requires-Dist: tzlocal<5.0,>=4.2
 Provides-Extra: all
 Requires-Dist: asyncio<4.0.0,>=3.4.3; extra == 'all'
-Requires-Dist: pydantic<2.0.0,>=1.10.5; extra == 'all'
 Requires-Dist: pytz>=2022.6; extra == 'all'
 Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: autoflake<3.0.0,>=1.4.0; extra == 'dev'
 Requires-Dist: black<23.0.0,>=22.10.0; extra == 'dev'
 Requires-Dist: flake8<7.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'dev'
-Requires-Dist: loguru<0.7.0,>=0.6.0; extra == 'dev'
 Requires-Dist: mypy<2.0.0,>=0.982; extra == 'dev'
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc'
 Requires-Dist: mkdocs-material<10.0.0,>=9.0.13; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc'
 Requires-Dist: mkdocstrings<0.30.0,>=0.20.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc'
 Provides-Extra: test
-Requires-Dist: esmerald==0.4.2; extra == 'test'
 Requires-Dist: mock>=4.0.3; extra == 'test'
 Requires-Dist: pymongo<5.0.0,>=4.3.3; extra == 'test'
 Requires-Dist: pytest-asyncio<1.0.0,>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest-loguru<1,>=0.2.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: redis<5.0.0,>=4.4.0; extra == 'test'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asyncz Version: 0.3.1 Summary: The scheduler that
+Metadata-Version: 2.1 Name: asyncz Version: 0.4.0 Summary: The scheduler that
 nobody wants but every application needs. Project-URL: Homepage, https://
 github.com/tarsil/asyncz Project-URL: Documentation, https://asyncz.tarsild.io/
 Project-URL: Changelog, https://asyncz.tarsild.io/release-notes/ Project-URL:
 Funding, https://github.com/sponsors/tarsil Project-URL: Source, https://
 github.com/tarsil/asyncz Author-email: Tiago Silva
 arasilva@gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 api,apscheduler,asgi,asyncz,cron,fastapi,framework,http,machine
@@ -19,34 +19,33 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Internet Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
 Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Application Frameworks Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Classifier: Typing ::
 Typed Requires-Python: >=3.8 Requires-Dist: asyncio<4.0.0,>=3.4.3 Requires-
-Dist: loguru<0.7.0,>=0.6.0 Requires-Dist: pydantic<2.0.0,>=1.10.9 Requires-
-Dist: pytz>=2022.6 Requires-Dist: tzlocal<5.0,>=4.2 Provides-Extra: all
-Requires-Dist: asyncio<4.0.0,>=3.4.3; extra == 'all' Requires-Dist:
-pydantic<2.0.0,>=1.10.5; extra == 'all' Requires-Dist: pytz>=2022.6; extra ==
-'all' Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all' Provides-Extra: dev
+Dist: loguru<0.8.0,>=0.7.0 Requires-Dist: pydantic<3.0.0,>=2.0.0 Requires-Dist:
+pytz>=2022.6 Requires-Dist: tzlocal<5.0,>=4.2 Provides-Extra: all Requires-
+Dist: asyncio<4.0.0,>=3.4.3; extra == 'all' Requires-Dist: pytz>=2022.6; extra
+== 'all' Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all' Provides-Extra: dev
 Requires-Dist: autoflake<3.0.0,>=1.4.0; extra == 'dev' Requires-Dist:
 black<23.0.0,>=22.10.0; extra == 'dev' Requires-Dist: flake8<7.0.0,>=3.8.3;
 extra == 'dev' Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'dev' Requires-
-Dist: loguru<0.7.0,>=0.6.0; extra == 'dev' Requires-Dist: mypy<2.0.0,>=0.982;
-extra == 'dev' Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
-Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev' Provides-Extra: doc
-Requires-Dist: mdx-include<2.0.0,>=1.4.2; extra == 'doc' Requires-Dist:
+Dist: mypy<2.0.0,>=0.982; extra == 'dev' Requires-Dist: pre-
+commit<3.0.0,>=2.17.0; extra == 'dev' Requires-Dist:
+watchfiles<0.20.0,>=0.16.1; extra == 'dev' Provides-Extra: doc Requires-Dist:
+mdx-include<2.0.0,>=1.4.2; extra == 'doc' Requires-Dist:
 mkautodoc<0.3.0,>=0.2.0; extra == 'doc' Requires-Dist: mkdocs-
 markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc' Requires-Dist: mkdocs-
 material<10.0.0,>=9.0.13; extra == 'doc' Requires-Dist: mkdocs<2.0.0,>=1.1.2;
 extra == 'doc' Requires-Dist: mkdocstrings<0.30.0,>=0.20.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc' Provides-Extra: test
-Requires-Dist: esmerald==0.4.2; extra == 'test' Requires-Dist: mock>=4.0.3;
-extra == 'test' Requires-Dist: pymongo<5.0.0,>=4.3.3; extra == 'test' Requires-
-Dist: pytest-asyncio<1.0.0,>=0.19.0; extra == 'test' Requires-Dist: pytest-
+Requires-Dist: mock>=4.0.3; extra == 'test' Requires-Dist:
+pymongo<5.0.0,>=4.3.3; extra == 'test' Requires-Dist: pytest-
+asyncio<1.0.0,>=0.19.0; extra == 'test' Requires-Dist: pytest-
 cov<5.0.0,>=2.12.0; extra == 'test' Requires-Dist: pytest-loguru<1,>=0.2.0;
 extra == 'test' Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test' Requires-
 Dist: redis<5.0.0,>=4.4.0; extra == 'test' Requires-Dist:
 requests<3.0.0,>=2.27.0; extra == 'test' Requires-Dist: ruff<1.0.0,>=0.0.256;
 extra == 'test' Description-Content-Type: text/markdown # Asyncz
                                    [Asyncz]
                   ð The scheduler that simply works. ð
```

