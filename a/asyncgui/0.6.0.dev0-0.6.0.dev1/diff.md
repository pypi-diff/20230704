# Comparing `tmp/asyncgui-0.6.0.dev0.tar.gz` & `tmp/asyncgui-0.6.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncgui-0.6.0.dev0.tar", max compression
+gzip compressed data, was "asyncgui-0.6.0.dev1.tar", max compression
```

## Comparing `asyncgui-0.6.0.dev0.tar` & `asyncgui-0.6.0.dev1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1055 2023-06-28 01:11:59.000000 asyncgui-0.6.0.dev0/LICENSE
--rw-r--r--   0        0        0     4268 2023-06-30 01:07:19.587907 asyncgui-0.6.0.dev0/README.md
--rw-r--r--   0        0        0     1213 2023-06-30 01:07:19.587907 asyncgui-0.6.0.dev0/pyproject.toml
--rw-r--r--   0        0        0    21326 2023-06-30 01:07:19.587907 asyncgui-0.6.0.dev0/src/asyncgui.py
--rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 asyncgui-0.6.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-28 01:11:59.000000 asyncgui-0.6.0.dev1/LICENSE
+-rw-r--r--   0        0        0     4268 2023-07-02 23:02:42.911629 asyncgui-0.6.0.dev1/README.md
+-rw-r--r--   0        0        0     1353 2023-07-04 01:57:38.832614 asyncgui-0.6.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0    26997 2023-07-04 01:56:51.481127 asyncgui-0.6.0.dev1/src/asyncgui.py
+-rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 asyncgui-0.6.0.dev1/PKG-INFO
```

### Comparing `asyncgui-0.6.0.dev0/LICENSE` & `asyncgui-0.6.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncgui-0.6.0.dev0/README.md` & `asyncgui-0.6.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `asyncgui-0.6.0.dev0/pyproject.toml` & `asyncgui-0.6.0.dev1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncgui"
-version = "0.6.0.dev0"
+version = "0.6.0.dev1"
 description = "async/await without event-loop"
 authors = ["Nattōsai Mitō <flow4re2c@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/gottadiveintopython/asyncgui'
 homepage = 'https://github.com/gottadiveintopython/asyncgui'
 keywords = ['async', ]
@@ -26,15 +26,21 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 exceptiongroup = {version = "^1.0.4", python = "<3.11"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.1"
-flake8 = "^4.0.1"
+flake8 = "^6.0.0"
+
+[tool.poetry.group.doc.dependencies]
+Sphinx = "^6.0.0"
+sphinx-tabs = "^3.4.1"
+sphinx-book-theme = "^1.0.1"
+sphinx-autobuild = "^2021.3.14"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 xfail_strict = true
```

### Comparing `asyncgui-0.6.0.dev0/src/asyncgui.py` & `asyncgui-0.6.0.dev1/src/asyncgui.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'Event',
 
     # utils (structured concurrency)
     'wait_all', 'wait_any', 'wait_all_cm', 'wait_any_cm', 'run_as_secondary', 'run_as_primary',
     'open_nursery', 'Nursery',
 
     # utils (for async library developer)
-    'IBox', 'ISignal',
+    'IBox', 'ISignal', '_current_task', '_sleep_forever',
 
     # aliases
     'run_as_daemon', 'TaskGroup', 'and_', 'or_',
 )
 import types
 import typing as T
 from inspect import getcoroutinestate, CORO_CREATED, CORO_SUSPENDED, isawaitable
@@ -31,101 +31,139 @@
 # -----------------------------------------------------------------------------
 # Core
 # -----------------------------------------------------------------------------
 
 if sys.version_info < (3, 11):
     from exceptiongroup import BaseExceptionGroup, ExceptionGroup
 else:
-    BaseExceptionGroup = BaseExceptionGroup
-    ExceptionGroup = ExceptionGroup
+    BaseExceptionGroup = BaseExceptionGroup  #: :meta private:
+    ExceptionGroup = ExceptionGroup  #: :meta private:
 
-potential_bug_msg = '''
-This may be a bug of this library. Please make a minimal code that reproduces the bug, and open an issue at the GitHub
-repository, and post that code. (https://github.com/gottadiveintopython/asyncgui).
-'''
+potential_bug_msg = \
+    r"This may be a bug of this library. Please make a minimal code that reproduces the bug, and open an issue at " \
+    r"the GitHub repository, then post the code there. (https://github.com/gottadiveintopython/asyncgui)."
 
 
 class InvalidStateError(Exception):
     """The operation is not allowed in the current state."""
 
 
 class _Cancelled(BaseException):
     @cached_property
     def level(self) -> int:
         return self.args[0]
 
 
 Cancelled = (_Cancelled, GeneratorExit, )
+'''
+Exception class that represents cancellation.
+See dealing-with-cancellation_ .
+
+:meta hide-value:
+'''
 
 
 class TaskState(enum.Enum):
+    '''
+    Enum class that represents the Task state.
+    '''
+
     CREATED = enum.auto()
-    '''CORO_CREATED'''
+    '''
+    Waiting to start execution.
+
+    :meta hide-value:
+    '''
 
     STARTED = enum.auto()
-    '''CORO_RUNNING or CORO_SUSPENDED'''
+    '''
+    Currently running or suspended.
+
+    :meta hide-value:
+    '''
 
     CANCELLED = enum.auto()
-    '''CORO_CLOSED by 'Task.cancel()' or an unhandled exception'''
+    '''
+    The execution has been cancelled.
+    The cause of cancellation can be either :meth:`Task.cancel` or an unhandled exception.
+
+    :meta hide-value:
+    '''
 
     FINISHED = enum.auto()
-    '''CORO_CLOSED (finished)'''
+    '''
+    The execution has been completed.
+
+    :meta hide-value:
+    '''
 
 
 class Task:
     __slots__ = (
         'name', '_uid', '_root_coro', '_state', '_result', '_on_end',
         '_exc_caught', '_suppresses_exc',
         '_cancel_disabled', '_cancel_depth', '_cancel_level',
     )
 
     _uid_iter = itertools.count()
 
-    def __init__(self, awaitable: T.Awaitable, /):
-        if not isawaitable(awaitable):
-            raise ValueError(str(awaitable) + " is not awaitable.")
+    def __init__(self, aw: T.Awaitable, /):
+        if not isawaitable(aw):
+            raise ValueError(str(aw) + " is not awaitable.")
         self._uid = next(self._uid_iter)
-        self.name = ""
+        self.name = ""  #: :meta private:
         self._cancel_disabled = 0
-        self._root_coro = self._wrapper(awaitable)
+        self._root_coro = self._wrapper(aw)
         self._state = TaskState.CREATED
         self._on_end = None
         self._cancel_depth = 0
         self._cancel_level = None
         self._exc_caught = None
         self._suppresses_exc = False
 
     def __str__(self):
         return f'Task(state={self._state.name}, uid={self._uid}, name={self.name!r})'
 
     @property
     def uid(self) -> int:
+        '''
+        An unique integer assigned to the task.
+        This exists solely for inspection purposes.
+        '''
         return self._uid
 
     @property
     def root_coro(self) -> T.Coroutine:
+        '''
+        The starting point of the coroutine chain for the task.
+        This exists solely for inspection purposes.
+        '''
         return self._root_coro
 
     @property
     def state(self) -> TaskState:
+        '''
+        The current state of the task.
+        This exists solely for inspection purposes.
+        '''
         return self._state
 
     @property
     def finished(self) -> bool:
+        '''Whether the task has been completed..'''
         return self._state is TaskState.FINISHED
 
     @property
     def cancelled(self) -> bool:
+        '''Whether the task has been cancelled.'''
         return self._state is TaskState.CANCELLED
 
     @property
     def result(self) -> T.Any:
-        '''Result of the task. If the task hasn't finished yet,
-        InvalidStateError will be raised.
-        '''
+        '''Result of the task. If the task is not finished, :exc:`InvalidStateError` will be raised. '''
         state = self._state
         if state is TaskState.FINISHED:
             return self._result
         elif state is TaskState.CANCELLED:
             raise InvalidStateError(f"{self} was cancelled")
         else:
             raise InvalidStateError(f"Result of {self} is not ready")
@@ -150,15 +188,15 @@
             self._state = TaskState.FINISHED
         finally:
             assert self._cancel_depth == 0, potential_bug_msg
             if (on_end := self._on_end) is not None:
                 on_end(self)
 
     def cancel(self, _level=0, /):
-        '''Cancel the task as soon as possible'''
+        '''Cancel the task as soon as possible.'''
         if self._cancel_level is None:
             self._cancel_level = _level
             state = getcoroutinestate(self._root_coro)
             if state is CORO_SUSPENDED:
                 if not self._cancel_disabled:
                     self._actual_cancel()
             elif state is CORO_CREATED:
@@ -172,24 +210,24 @@
             # NOTE: _cancel_levelが0の時は末尾の関数呼び出し (self) は省いても良いかもしれない
             self._root_coro.throw(_Cancelled(self._cancel_level))(self)
         except StopIteration:
             pass
         else:
             self._cancel_if_needed()
 
-    # give 'cancel()' an alias so that we can pass a Task instance to `contextlib.closing`
     close = cancel
+    '''An alias for :meth:`cancel`.'''
 
     @property
     def _cancel_requested(self) -> bool:
         return self._cancel_level is not None
 
     @property
     def _is_cancellable(self) -> bool:
-        '''Whether the task can immediately be cancelled.'''
+        '''Whether the task can be cancelled immediately.'''
         return (not self._cancel_disabled) and getcoroutinestate(self._root_coro) is CORO_SUSPENDED
 
     def _cancel_if_needed(self, getcoroutinestate=getcoroutinestate, CORO_SUSPENDED=CORO_SUSPENDED):
         if (self._cancel_level is None) or self._cancel_disabled or \
                 (getcoroutinestate(self._root_coro) is not CORO_SUSPENDED):
             pass
         else:
@@ -219,18 +257,25 @@
             self._cancel_if_needed()
 
 
 Aw_or_Task = T.Union[T.Awaitable, Task]
 
 
 def start(aw: Aw_or_Task, /) -> Task:
-    '''Starts an asyncgui-flavored awaitable or a Task.
+    '''*Immediately* start a Task/Awaitable.
+
+    If the argument is a :class:`Task`, itself will be returned. If it's a :class:`typing.Awaitable`,
+    it will be wrapped in a Task, and that Task will be returned.
+
+    .. code-block::
 
-    If the argument is a Task, itself will be returned. If it's an awaitable,
-    it will be wrapped in a Task, and the Task will be returned.
+        async def async_func():
+            ...
+
+        task = start(async_func())
     '''
     if isawaitable(aw):
         task = Task(aw)
     elif isinstance(aw, Task):
         task = aw
         if task._state is not TaskState.CREATED:
             raise ValueError(f"{task} has already started")
@@ -245,22 +290,23 @@
         task._cancel_if_needed()
 
     return task
 
 
 class CancelScope:
     '''
-    You should not directly instantiate this. Use :func:`open_cancel_scope`.
+    Equivalent of :class:`trio.CancelScope`.
+    You should not directly instantiate this, use :func:`open_cancel_scope`.
     '''
     __slots__ = ('_task', '_depth', 'cancelled_caught', 'cancel_called', )
 
     def __init__(self, task: Task, /):
         self._task = task
-        self.cancelled_caught = False
-        self.cancel_called = False
+        self.cancelled_caught = False  #: Whether the scope caught a corresponding :class:`Cancelled` instance.
+        self.cancel_called = False  #: Whether the :meth:`cancel` has been called.
 
     def __enter__(self) -> 'CancelScope':
         t = self._task
         t._cancel_depth = self._depth = t._cancel_depth + 1
         return self
 
     def __exit__(self, exc_type, exc, __):
@@ -283,27 +329,32 @@
             self.cancelled_caught = True
             return True
         else:
             assert level < depth, potential_bug_msg
 
     @property
     def closed(self) -> bool:
+        '''
+        Whether this scope has been closed.
+        The cause of the closure of the scope can be either an exception occurred or the scope exited gracefully,
+        '''
         return self._task is None
 
     def cancel(self):
+        '''Cancel the execution inside this scope as soon as possible. '''
         if self.cancel_called:
             return
         self.cancel_called = True
         if not self.closed:
             self._task.cancel(self._depth)
 
 
 class open_cancel_scope:
     '''
-    Same as :class:`trio.CancelScope` except this one is an async context manager.
+    Same as :class:`trio.CancelScope` except this one returns an async context manager.
 
     .. code-block::
 
         async with open_cancel_scope() as scope:
             ...
     '''
     __slots__ = ('_scope', )
@@ -312,23 +363,32 @@
         self._scope = CancelScope(await current_task())
         return self._scope.__enter__()
 
     async def __aexit__(self, *args):
         return self._scope.__exit__(*args)
 
 
+def _current_task(task):
+    return task._step(task)
+
+
 @types.coroutine
-def current_task(_f=lambda task: task._step(task)) -> T.Awaitable[Task]:
-    '''Returns the Task instance corresponding to the caller.'''
+def current_task(_f=_current_task) -> T.Awaitable[Task]:
+    '''Returns the Task instance corresponding to the caller.
+
+    .. code-block::
+
+        task = await current_task()
+    '''
     return (yield _f)[0][0]
 
 
 class disable_cancellation:
     '''
-    Async context manager that protects its code-block from cancellation.
+    Return an async context manager that protects its code-block from cancellation.
 
     .. code-block::
 
         async with disable_cancellation():
             await something  # <- never gets cancelled
     '''
 
@@ -338,48 +398,97 @@
         self._task = task = await current_task()
         task._cancel_disabled += 1
 
     async def __aexit__(self, *__):
         self._task._cancel_disabled -= 1
 
 
-async def check_cancellation():
+@types.coroutine
+def check_cancellation():
     '''
-    (experimental) If the ``.cancel()`` method of the current task has been
-    called and the task is not protected from cancellation, cancels the task
-    immediately. Otherwise, does nothing.
+    If the current task has been requested to be cancelled, and the task is not protected from cancellation,
+    cancel the task immediately. Otherwise, do nothing.
+
+    .. code-block::
+
+        await check_cancellation()
     '''
-    task = await current_task()
+    task = (yield _current_task)[0][0]
     if task._cancel_requested and not task._cancel_disabled:
-        await sleep_forever()
+        yield _sleep_forever
+
+
+def _sleep_forever(task):
+    pass
 
 
 @types.coroutine
-def sleep_forever(_f=lambda task: None) -> T.Awaitable:
+def sleep_forever(_f=_sleep_forever) -> T.Awaitable:
+    '''
+    .. code-block::
+
+        await sleep_forever()
+    '''
     yield _f
 
 
 dummy_task = Task(sleep_forever())
+'''
+An already closed task.
+This can be utilized to prevent the need for the common null validation mentioned below.
+
+*Before:*
+
+.. code-block::
+    :emphasize-lines: 3, 6,7
+
+    class MyClass:
+        def __init__(self):
+            self._task = None
+
+        def restart(self):
+            if self._task is not None:
+                self._task.cancel()
+            self._task = asyncgui.start(self.main())
+
+        async def main(self):
+            ...
+
+*After:*
+
+.. code-block::
+    :emphasize-lines: 3, 6
+
+    class MyClass:
+        def __init__(self):
+            self._task = asyncgui.dummy_task
+
+        def restart(self):
+            self._task.cancel()
+            self._task = asyncgui.start(self.main())
+
+        async def main(self):
+            ...
+'''
 dummy_task.cancel()
 dummy_task.name = r"asyncgui.dummy_task"
 
 # -----------------------------------------------------------------------------
 # Utilities
 # -----------------------------------------------------------------------------
 
 
 class Event:
     '''
-    Equivalent of :class:`asyncio.Event`.
+    Similar to :class:`asyncio.Event`.
+    The differences are:
 
-    Difference
-    ----------
-
-    :meth:`set` accepts any number of arguments but doesn't use them at all so it can be used as a callback function
-    of any library.
+    * :meth:`set` accepts any number of arguments but doesn't use them at all so it can be used as a callback function
+      in any library.
+    * :attr:`is_set` is a property not a function.
 
     .. code-block::
 
         e = Event()
         any_library.register_callback(e.set)
     '''
 
@@ -390,28 +499,37 @@
         self._waiting_tasks = []
 
     @property
     def is_set(self) -> bool:
         return self._flag
 
     def set(self, *args, **kwargs):
+        '''
+        Set the event.
+        Unlike asyncio's, all tasks waiting for this event to be set will be resumed *immediately*.
+        '''
         if self._flag:
             return
         self._flag = True
         tasks = self._waiting_tasks
         self._waiting_tasks = []
         for t in tasks:
             if t is not None:
                 t._step()
 
     def clear(self):
+        '''Unset the event.'''
         self._flag = False
 
     @types.coroutine
     def wait(self) -> T.Awaitable:
+        '''
+        Wait for the event to be set.
+        Return *immediately* if it's already set.
+        '''
         if self._flag:
             return
         try:
             tasks = self._waiting_tasks
             idx = len(tasks)
             yield self._waiting_tasks.append
         finally:
@@ -421,42 +539,58 @@
 class ISignal:
     '''
     Same as :class:`Event` except:
 
     * This one doesn't have ``clear()`` and ``is_set``.
     * Only one task can :meth:`wait` at a time.
 
-    The reason this is introduced
-    -----------------------------
+    It's quite common that only one task waits for an event to be set.
+    Using :class:`Event` may be over-kill in that situation because it is designed to allow multiple tasks to
+    ``wait()`` simultaneously.
+
+    .. code-block::
+
+        sig = ISignal()
+        any_library.register_callback(sig.set)
+
+        async def async_func():
+            await sig.wait()
 
-    It's quite common that only one task waits for an event to be fired,
-    and :class:`Event` may be over-kill in that situation because it is designed to accept multiple tasks.
+    .. seealso:: wrapping-a-callback-based-api_
     '''
 
     __slots__ = ('_flag', '_task', )
 
     def __init__(self):
         self._flag = False
         self._task = None
 
     def set(self, *args, **kwargs):
+        '''
+        Set the event.
+        The task waiting for this signal to be set will be resumed *immediately* if there is one.
+        '''
         if self._flag:
             return
         self._flag = True
         if (t := self._task) is not None:
             t._step()
 
     _decrease_or_set = set
 
     @types.coroutine
     def wait(self) -> T.Awaitable:
+        '''
+        Wait for the signal to be set. Return *immediately* if it's already set.
+        Raise :exc:`InvalidStateError` if there is already a task waiting for it.
+        '''
         if self._flag:
             return
         if self._task is not None:
-            raise InvalidStateError("There is already a task waiting for this signal to set.")
+            raise InvalidStateError("There is already a task waiting for this signal to be set.")
         try:
             yield self._store_task
         finally:
             self._task = None
 
     def _store_task(self, task):
         self._task = task
@@ -493,15 +627,15 @@
             sig._flag = False
             await sig.wait()
 
     def __bool__(self):
         return not not self._n_tasks  # 'not not' is not a typo
 
 
-async def _wait_xxx(debug_msg, on_child_end, *aws: T.Iterable[Aw_or_Task]):
+async def _wait_xxx(debug_msg, on_child_end, *aws: T.Iterable[Aw_or_Task]) -> T.Awaitable[T.Sequence[Task]]:
     children = tuple(v if isinstance(v, Task) else Task(v) for v in aws)
     if not children:
         return children
     counter = TaskCounter(len(children))
     parent = await current_task()
 
     try:
@@ -541,15 +675,36 @@
     counter_or_signal._decrease_or_set()
     if child._exc_caught is not None or child.finished:
         scope.cancel()
 
 
 _wait_xxx_type = T.Callable[..., T.Awaitable[T.Sequence[Task]]]
 wait_all: _wait_xxx_type = partial(_wait_xxx, "wait_all()", _on_child_end__ver_all)
+'''
+Run multiple tasks concurrently, and wait for **all** of them to **end**. When any of them raises an exception, the others
+will be cancelled, and the exception will be propagated to the caller, like :class:`trio.Nursery`.
+
+.. code-block::
+
+    tasks = await wait_all(async_fn1(), async_fn2(), async_fn3())
+    if tasks[0].finished:
+        print("The return value of async_fn1() :", tasks[0].result)
+'''
 wait_any: _wait_xxx_type = partial(_wait_xxx, "wait_any()", _on_child_end__ver_any)
+'''
+Run multiple tasks concurrently, and wait for **any** of them to **finish**. As soon as that happens, the others will be
+cancelled. When any of them raises an exception, the others will be cancelled, and the exception will be propagated to
+the caller, like :class:`trio.Nursery`.
+
+.. code-block::
+
+    tasks = await wait_any(async_fn1(), async_fn2(), async_fn3())
+    if tasks[0].finished:
+        print("The return value of async_fn1() :", tasks[0].result)
+'''
 
 
 @asynccontextmanager
 async def _wait_xxx_cm(debug_msg, on_child_end, wait_bg, aw: Aw_or_Task):
     signal = ISignal()
     fg_task = await current_task()
     bg_task = aw if isinstance(aw, Task) else Task(aw)
@@ -581,22 +736,27 @@
         if (fg_task._cancel_level is not None) and (not fg_task._cancel_disabled):
             await sleep_forever()
             assert False, potential_bug_msg
 
 
 _wait_xxx_cm_type = T.Callable[[Aw_or_Task], T.AsyncContextManager[Task]]
 wait_all_cm: _wait_xxx_cm_type = partial(_wait_xxx_cm, "wait_all_cm()", _on_child_end__ver_all, True)
+'''See :doc:`structured-concurrency`.'''
 wait_any_cm: _wait_xxx_cm_type = partial(_wait_xxx_cm, "wait_any_cm()", _on_child_end__ver_any, False)
+'''See :doc:`structured-concurrency`.'''
 run_as_primary: _wait_xxx_cm_type = partial(_wait_xxx_cm, "run_as_primary()", _on_child_end__ver_any, True)
+'''See :doc:`structured-concurrency`.'''
 run_as_secondary: _wait_xxx_cm_type = partial(_wait_xxx_cm, "run_as_secondary()", _on_child_end__ver_all, False)
+'''See :doc:`structured-concurrency`.'''
 
 
 class Nursery:
     '''
-    You should not directly instantiate this. Use :func:`open_nursery`.
+    Similar to :class:`trio.Nursery`.
+    You should not directly instantiate this, use :func:`open_nursery`.
     '''
 
     __slots__ = ('_closed', '_children', '_scope', '_counters', '_callbacks', )
 
     def __init__(self, children, scope, counter, daemon_counter):
         self._closed = False
         self._children = children
@@ -604,39 +764,52 @@
         self._counters = (daemon_counter, counter, )
         self._callbacks = (
             partial(_on_child_end__ver_all, scope, daemon_counter),
             partial(_on_child_end__ver_all, scope, counter),
         )
 
     def start(self, aw: Aw_or_Task, /, *, daemon=False) -> Task:
+        '''
+        *Immediately* start a Task/Awaitable under the supervision of the nursery.
+
+        If the argument is a :class:`Task`, itself will be returned. If it's a :class:`typing.Awaitable`,
+        it will be wrapped in a Task, and that Task will be returned.
+
+        The ``daemon`` parameter acts like the one in the :mod:`threading` module.
+        When only daemon tasks are left, they get cancelled, and the nursery closes.
+        '''
         if self._closed:
             raise InvalidStateError("Nursery has been already closed")
         child = aw if isinstance(aw, Task) else Task(aw)
         child._suppresses_exc = True
         child._on_end = self._callbacks[not daemon]
         self._counters[not daemon].increase()
         self._children.append(child)
         return start(child)
 
     def close(self):
-        '''
-        Cancel all the child tasks inside the nursery.
-        '''
+        '''Cancel all the child tasks in the nursery as soon as possible. '''
         self._closed = True
         self._scope.cancel()
 
     @property
     def closed(self) -> bool:
         return self._closed
 
 
 @asynccontextmanager
 async def open_nursery() -> T.AsyncIterator[Nursery]:
     '''
     Equivalent of :func:`trio.open_nursery`.
+
+    .. code-block::
+
+        async with open_nursery() as nursery:
+            nursery.start(other_async_func1())
+            nursery.start(other_async_func2())
     '''
     children = []
     exc = None
     parent = await current_task()
     counter = TaskCounter()
     daemon_counter = TaskCounter()
 
@@ -666,40 +839,53 @@
         if (parent._cancel_level is not None) and (not parent._cancel_disabled):
             await sleep_forever()
             assert False, potential_bug_msg
 
 
 class IBox:
     '''
-    An item box with the following limitations.
+    :class:`ISignal` + the capability to transfer values.
+
+    .. code-block::
 
-    * You can :meth:`put` an item in it only once. Doing it more than once will be ignored.
-    * Only one task can :meth:`get` an item from it at a time.
+        box = IBox()
+        ...
+        box.put(1, 2, key='value')
+
+        async def async_func():
+            args, kwargs = await box.get()
+            assert args == (1, 2, )
+            assert kwargs == {'key': 'value', }
 
     .. note::
 
-        This exists for the purpose of wrapping a callback-based api in an async/await-based api.
-        Using it for any other purpose is not recommended.
+        This is not a generic item storage, but is designed for a specific purpose.
+        See wrapping-a-callback-based-api_ for details.
     '''
 
     __slots__ = ('_item', '_getter', )
 
     def __init__(self):
         self._item = None
         self._getter = None
 
     def put(self, *args, **kwargs):
+        '''Put an item into the box. This has an effect only on the first call; subsequent calls will be ignored. '''
         if self._item is not None:
             return
         self._item = (args, kwargs, )
         if (getter := self._getter) is not None:
             getter._step(*args, **kwargs)
 
     @types.coroutine
     def get(self) -> T.Awaitable[T.Tuple[tuple, dict]]:
+        '''
+        Get an item inside the box. If the box is empty, wait until one is available.
+        Raise :exc:`InvalidStateError` if there is already a task waiting for it.
+        '''
         if self._getter is not None:
             raise InvalidStateError("There is already a task trying to get an item from this box.")
         if self._item is None:
             try:
                 return (yield self._store_getter)
             finally:
                 self._getter = None
@@ -709,12 +895,11 @@
     def _store_getter(self, task):
         self._getter = task
 
 
 # -----------------------------------------------------------------------------
 # Aliases
 # -----------------------------------------------------------------------------
-
-run_as_daemon = run_as_secondary
-TaskGroup = open_nursery
-and_ = wait_all
-or_ = wait_any
+run_as_daemon = run_as_secondary  #: An alias for :func:`run_as_secondary`.
+TaskGroup = open_nursery  #: An alias for :func:`open_nursery`.
+and_ = wait_all  #: An alias for :func:`wait_all`. This exists solely for backward compatibility.
+or_ = wait_any  #: An alias for :func:`wait_any`. This exists solely for backward compatibility.
```

### Comparing `asyncgui-0.6.0.dev0/PKG-INFO` & `asyncgui-0.6.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncgui
-Version: 0.6.0.dev0
+Version: 0.6.0.dev1
 Summary: async/await without event-loop
 Home-page: https://github.com/gottadiveintopython/asyncgui
 License: MIT
 Keywords: async
 Author: Nattōsai Mitō
 Author-email: flow4re2c@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

