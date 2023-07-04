# Comparing `tmp/jorun-0.2.0.tar.gz` & `tmp/jorun-0.2.1.tar.gz`

## Comparing `jorun-0.2.0.tar` & `jorun-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,42 @@
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 jorun-0.2.0/jorun.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/configuration.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/constants.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/errors.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/logger.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/main.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/runner.py
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/runner_process.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/base.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/docker.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/group.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/shell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/palette/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/palette/base.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/palette/darcula.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/types/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/types/options.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/types/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/__init__.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/application.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/data_signals.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/main_window.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/pane.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/task_panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.2.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.2.0/LICENSE
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jorun-0.2.0/README.md
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 jorun-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 jorun-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 jorun-0.2.1/jorun.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/configuration.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/constants.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/errors.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/logger.py
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/main.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/runner.py
+-rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/runner_process.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/scanner.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/handler/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/handler/base.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/handler/docker.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/handler/group.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/handler/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/messaging/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/messaging/message.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/palette/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/palette/base.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/palette/darcula.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/palette/hacker.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/palette/kimbie_dark.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/palette/monokai.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/palette/solarized_dark.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/types/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/types/options.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/types/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/ui/__init__.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/ui/application.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/ui/command_handler.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/ui/data_signals.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/ui/main_window.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/ui/pane.py
+-rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/ui/task_panel.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 jorun-0.2.1/src/jorun/ui/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.2.1/LICENSE
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 jorun-0.2.1/README.md
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 jorun-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9740 2020-02-02 00:00:00.000000 jorun-0.2.1/PKG-INFO
```

### Comparing `jorun-0.2.0/jorun.yml` & `jorun-0.2.1/jorun.yml`

 * *Files identical despite different names*

### Comparing `jorun-0.2.0/src/jorun/configuration.py` & `jorun-0.2.1/src/jorun/configuration.py`

 * *Files identical despite different names*

### Comparing `jorun-0.2.0/src/jorun/logger.py` & `jorun-0.2.1/src/jorun/logger.py`

 * *Files identical despite different names*

### Comparing `jorun-0.2.0/src/jorun/runner.py` & `jorun-0.2.1/src/jorun/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,42 +6,42 @@
 import time
 from asyncio.subprocess import Process
 from datetime import datetime
 from logging import Logger
 from typing import Optional, Callable, List, Union
 
 import psutil
-from tinyioc import inject
+from tinyioc import get_service
 
+from . import constants
 from .handler.base import BaseTaskHandler
 from .logger import logger
 from .scanner import AsyncScanner
 from .types.options import TaskOptions
 from .types.task import Task
 from .configuration import AppConfiguration
 
-OUTPUT_READ_INTERVAL = 0.015
-
 
 class TaskRunner:
     _handlers: List[BaseTaskHandler]
     _handler: BaseTaskHandler
 
     _task: Task
     _process: Optional[Process]
     _completion_callback: Optional[Callable]
     _scanner: AsyncScanner
     _log_handler: logging.Handler
 
     _logger: Logger
     _err_logger: Logger
 
-    @inject()
     def __init__(self, task: Task, file_output_dir: Optional[str], log_level: Union[int, str],
-                 log_handler: logging.Handler, configuration: AppConfiguration):
+                 log_handler: logging.Handler):
+        configuration: AppConfiguration = get_service(AppConfiguration)
+
         self._task = task
         self._handlers = configuration.handlers
         self._process = None
         self._running = True
         self._completion_callback = None
         self._log_handler = log_handler
 
@@ -68,47 +68,48 @@
             self._err_logger.addHandler(file_handler)
 
     @property
     def name(self):
         return self._task["name"]
 
     def _on_stop(self):
+        # noinspection PyTypedDict
         self._handler.on_exit(self._task[self._handler.task_type], self._process)
 
     def stop(self, timeout=1):
         if self._process and self._process.returncode is None:
             logger.debug(f"Process {self.name} is alive. Killing it")
 
             self._on_stop()
             pid = self._process.pid
 
             if platform.system() == "Windows":
                 os.kill(pid, signal.CTRL_C_EVENT)
             else:
                 os.kill(pid, signal.SIGTERM)
 
-            timeout_left = timeout
-            while timeout_left > 0 and psutil.pid_exists(pid):
-                time.sleep(0.2)
-                timeout_left -= 0.2
+            init_time = time.time()
+            while psutil.pid_exists(pid) and time.time() < init_time + timeout:
+                time.sleep(constants.PROCESS_KILL_POLLING_INTERVAL)
 
             if psutil.pid_exists(pid):
                 logger.debug(f"Process {self.name} still alive after {timeout}s timeout. Sending SIGKILL")
                 if platform.system() == "Windows":
                     os.kill(pid, signal.CTRL_BREAK_EVENT)
                 else:
                     os.kill(pid, signal.SIGKILL)
 
-    async def start(self, completion_callback: Callable):
+    async def start(self, completion_callback: Optional[Callable]):
         try:
             self._completion_callback = completion_callback
             t = self._task
 
             stderr_redirect = t.get('pattern_in_stderr', False)
 
+            # noinspection PyTypedDict
             task_options: Optional[TaskOptions] = t.get(self._handler.task_type)
 
             self._process = await self._handler.execute(task_options, self._completion_callback,
                                                         stderr_redirect)
             if not self._process:
                 self._running = False
                 return
```

### Comparing `jorun-0.2.0/src/jorun/scanner.py` & `jorun-0.2.1/src/jorun/scanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,30 +49,34 @@
         try:
             while self._process.returncode is None:
                 line_b = await self._readline(self._process.stdout, self._read_timeout)
 
                 if line_b is not None:
                     line = line_b.decode('utf-8', errors='ignore')
                     self._logger.info(line, extra={'subprocess': task_name})
-                    if reg.match(line) and self._completion_callback:
+                    if reg.match(line):
                         pattern_matched = True
 
-                        self._completion_callback()
-                        self._completion_callback = None
+                        if self._completion_callback:
+                            self._completion_callback()
+                            self._completion_callback = None
+
                         return await self._print_stdout(task_name)
 
             if not pattern_matched:
                 while line_b := await self._process.stdout.readline():
                     line = line_b.decode('utf-8', errors='ignore')
                     self._logger.info(line, extra={'subprocess': task_name})
-                    if reg.match(line) and self._completion_callback:
+                    if reg.match(line):
                         pattern_matched = True
 
-                        self._completion_callback()
-                        self._completion_callback = None
+                        if self._completion_callback:
+                            self._completion_callback()
+                            self._completion_callback = None
+
                         return await self._print_stdout(task_name)
         except Exception:
             pass
 
         if not pattern_matched:
             raise TaskRunException(f"Could not match given pattern on '{task_name}' before process exit")
```

### Comparing `jorun-0.2.0/src/jorun/handler/base.py` & `jorun-0.2.1/src/jorun/handler/base.py`

 * *Files identical despite different names*

### Comparing `jorun-0.2.0/src/jorun/handler/docker.py` & `jorun-0.2.1/src/jorun/handler/docker.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import subprocess
 from asyncio.subprocess import Process
 from typing import Callable, Optional, Dict, List
 
 from ..handler.base import BaseTaskHandler
 from ..logger import logger
 from ..types.options import TaskOptions
+from ..utils import get_process_group_args
 
 
 class DockerTask(TaskOptions):
     container_name: str
     image: str
     docker_arguments: Optional[List[str]]
     docker_command: Optional[List[str]]
@@ -47,19 +48,22 @@
 
         process = await asyncio.create_subprocess_exec(
             command[0],
             *command[1:],
             cwd=options.get("working_directory"),
             stdout=subprocess.PIPE,
             stderr=stderr_file,
-            stdin=subprocess.DEVNULL)
+            stdin=subprocess.DEVNULL,
+            **get_process_group_args())
 
         self._stop_on_exit = options.get("stop_at_exit", False)
         return process
 
     def on_exit(self, options: DockerTask, process: Process):
         if self._stop_on_exit:
+            logger.info(f"Stopping docker container {options['container_name']}")
+            logger.debug(f"Stop command: {' '.join(['docker','stop', options['container_name']])}")
             subprocess.run([
                 "docker",
                 "stop",
                 options['container_name']
             ])
```

### Comparing `jorun-0.2.0/src/jorun/handler/group.py` & `jorun-0.2.1/src/jorun/handler/group.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 class GroupTaskHandler(BaseTaskHandler):
     @property
     def task_type(self) -> str:
         return "group"
 
     async def execute(self, options: Optional[TaskOptions], completion_callback: Callable, stderr_redirect: bool) \
             -> Optional[Process]:
-        completion_callback()
+        if completion_callback:
+            completion_callback()
         return None
 
     def on_exit(self, options: TaskOptions, process: Process):
         pass
```

### Comparing `jorun-0.2.0/src/jorun/handler/shell.py` & `jorun-0.2.1/src/jorun/handler/shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 from asyncio.subprocess import Process
 from typing import Callable, Optional, List, Union, Dict
 
 from ..types.options import TaskOptions
 from .base import BaseTaskHandler
 from ..logger import logger
+from ..utils import get_process_group_args
 
 
 class ShellTask(TaskOptions):
     command: Union[str, List[str]]
     working_directory: Optional[str]
     environment: Optional[Dict[str, str]]
 
@@ -39,22 +40,24 @@
         if not isinstance(options["command"], list):
             process = await asyncio.create_subprocess_shell(
                 options["command"],
                 cwd=options.get("working_directory"),
                 env=env_vars,
                 stdout=subprocess.PIPE,
                 stderr=stderr_file,
-                stdin=subprocess.DEVNULL)
+                stdin=subprocess.DEVNULL,
+                **get_process_group_args())
         else:
             process = await asyncio.create_subprocess_exec(
                 options["command"][0],
                 *options["command"][1:],
                 cwd=options.get("working_directory"),
                 env=env_vars,
                 stdout=subprocess.PIPE,
                 stderr=stderr_file,
-                stdin=subprocess.DEVNULL)
+                stdin=subprocess.DEVNULL,
+                **get_process_group_args())
 
         return process
 
     def on_exit(self, options: TaskOptions, process: Process):
         pass
```

### Comparing `jorun-0.2.0/src/jorun/types/task.py` & `jorun-0.2.1/src/jorun/types/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,22 @@
 
 
 class PaneConfiguration(TypedDict):
     columns: int
     tasks: List[str]
 
 
+class GuiConfiguration(TypedDict):
+    panes: Optional[Dict[str, PaneConfiguration]]
+    palette: Optional[str]
+
+
 class TasksConfiguration(TypedDict):
     tasks: Dict[str, Task]
-    gui: Optional[Dict[str, PaneConfiguration]]
+    gui: Optional[GuiConfiguration]
 
 
 @dataclass
 class TaskNode:
     task: Task
     dependencies: List["TaskNode"]
```

### Comparing `jorun-0.2.0/src/jorun/ui/main_window.py` & `jorun-0.2.1/src/jorun/ui/main_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from logging import LogRecord
 from typing import Dict, List, Optional
 
 from PySide6.QtCore import Slot
 from PySide6.QtWidgets import QMainWindow, QTabWidget
-from tinyioc import inject
+from tinyioc import get_service
 
 from .data_signals import DataUpdateSignalEmitter, MainWindowSignals
 from .pane import TasksPane
 from .. import constants
+from ..messaging.message import TaskStatusMessage
 from ..palette.base import BaseColorPalette
 from ..types.task import PaneConfiguration
 
 
 class MainWindow(QMainWindow, DataUpdateSignalEmitter):
     _tab_widget: QTabWidget
     _panes: List[TasksPane]
     signals = MainWindowSignals()
 
-    @inject()
-    def __init__(self, tasks: List[str], palette: BaseColorPalette, gui_config: Optional[Dict[str, PaneConfiguration]]):
+    def __init__(self, tasks: List[str], gui_config: Optional[Dict[str, PaneConfiguration]]):
         super(MainWindow, self).__init__()
 
+        palette: BaseColorPalette = get_service(BaseColorPalette)
+
         self.signals.app_terminated.connect(self.close)
         self._panes = []
 
         self.setStyleSheet(f"""
             background-color: {palette.background};
         """)
         self.setMinimumSize(300, 300)
@@ -69,19 +71,28 @@
         if len(tasks_bucket) > 0:
             extra_pane = TasksPane(None, list(tasks_bucket))
             extra_pane.setAutoFillBackground(True)
             self._tab_widget.addTab(extra_pane, "-")
             self._panes.append(extra_pane)
 
         self.signals.data_received.connect(self._handle_stream_record)
+        self.signals.task_status_received.connect(self._handle_task_status)
 
-    @Slot()
+    @Slot(LogRecord)
     def _handle_stream_record(self, record: LogRecord):
         for p in self._panes:
             p.dispatch_log_record(record)
 
+    @Slot(TaskStatusMessage)
+    def _handle_task_status(self, status: TaskStatusMessage):
+        for p in self._panes:
+            p.dispatch_task_status(status)
+
     # noinspection PyUnresolvedReferences
     def dispatch_stream_record(self, record: LogRecord):
         self.signals.data_received.emit(record)
 
+    def dispatch_task_status(self, status: TaskStatusMessage):
+        self.signals.task_status_received.emit(status)
+
     def dispatch_app_termination(self):
         self.signals.app_terminated.emit()
```

### Comparing `jorun-0.2.0/src/jorun/ui/pane.py` & `jorun-0.2.1/src/jorun/ui/pane.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from logging import LogRecord
 from typing import Optional, List, Dict
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QSplitter
-from tinyioc import inject
+from tinyioc import get_service
 
+from ..logger import logger
+from ..messaging.message import TaskStatusMessage
 from ..palette.base import BaseColorPalette
 from .task_panel import TaskPanel
 
 
 class TasksPane(QWidget):
     _layout: QVBoxLayout
     _central_widget: QSplitter
     _tasks: List[str]
     _total_columns: int
     _task_widgets: Dict[str, TaskPanel]
     _splitters: List[QSplitter]
 
-    @inject()
-    def __init__(self, parent: Optional[QWidget], tasks: List[str], palette: BaseColorPalette, columns: int = 3):
+    def __init__(self, parent: Optional[QWidget], tasks: List[str], columns: int = 3):
         super(TasksPane, self).__init__(parent)
 
+        palette: BaseColorPalette = get_service(BaseColorPalette)
+
         self._tasks = tasks
         self._total_columns = columns
         self._task_widgets = {}
         self._splitters = []
 
         self._central_widget = QSplitter(Qt.Orientation.Vertical, self)
         self._central_widget.setStyleSheet(f"""
@@ -53,7 +56,11 @@
 
             col += 1
 
     # noinspection PyUnresolvedReferences
     def dispatch_log_record(self, record: LogRecord):
         if record.subprocess in self._task_widgets:
             self._task_widgets[record.subprocess].append_text(record)
+
+    def dispatch_task_status(self, status: TaskStatusMessage):
+        if status.task in self._task_widgets:
+            self._task_widgets[status.task].update_status(status.status)
```

### Comparing `jorun-0.2.0/LICENSE` & `jorun-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jorun-0.2.0/README.md` & `jorun-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -29,23 +29,25 @@
 jorun ./conf.yml
 ```
 
 ## Configuration
 
 ```yml
 gui:
-  services:
-    tasks:
-      - db
-      - redis
-  terminals:
-    tasks:
-      - test_1
-      - test_2
-      - test_3
+  panes:
+    services:
+      tasks:
+        - db
+        - redis
+    terminals:
+      tasks:
+        - test_1
+        - test_2
+        - test_3
+  palette: hacker
 tasks:
   db:
     type: docker
     docker:
       container_name: test
       image: postgres
       docker_arguments:
@@ -87,51 +89,92 @@
     type: shell
     shell:
       command: echo TEST 3
     depends:
       - test
 ```
 
-This sample YML file shows two task types you can run:
+This sample YML file shows three task types you can run:
 
 - **Shell**: a task launching a shell command
 - **Docker**: a task optimized for docker containers
-- **Group**: a task that groups other tasks (for parallel execution)
+- **Group**: a task that groups other tasks. Used when you have a lot of tasks with the same dependencies, to avoid writing all of them every time 
 
 The task runner supports searching for a pattern in the task output to
 signal its completion. This way you can start a dependent task after the pattern
 shows up in the task output.
 
-Tasks are chained through dependencies. 
+Tasks are chained through dependencies.
 The first tasks to run are the ones without dependencies.
 If you declare one or more dependencies, the task will not run until all the dependencies are either:
 
-- *completed* (i.e. the task finished executing), by default
-- _the completion pattern is matched_ (the regex pattern matched a line of the task output), if you set a **completion_pattern**
-- _launched_, if you set the **run_mode** to `indefinite`
+- **completed** (i.e. the task finished executing), by default
+- **the completion pattern is matched** (the regex pattern matched a line of the task output), if you set a
+  **completion_pattern**
+- **launched**, if you set the **run_mode** to `indefinite`
 
 ## GUI
 
 If you run **Jorun** with the `--gui` command line option, or if you specify the **gui** option
 in the yaml configuration you can start the tool with a graphical interface.
 The GUI is still a prototype, but will let you keep track of the task logs individually and
 even filter the log rows.
 
 The **gui** section in the YML configuration is where you can specify the panes you want displayed,
 and for each pane you can set the tasks that belong to it and the maximum number of columns visible in the pane.
 
+For instance, let's say you have 10 tasks in which you have 4 databases, 4 REST services, and 2 queues.
+You then have this GUI configuration:
+
+```yml
+gui:
+  panes:
+    databases:
+      tasks:
+        - postgres
+        - redis
+        - mongo
+        - cassandra
+      columns: 2
+    services:
+      tasks:
+        - auth
+        - orders
+        - customers
+        - shipments
+      columns: 4
+    pubsub:
+      tasks:
+        - rabbitmq
+        - kafka
+      columns: 1
+  palette: hacker
+```
+
+The first pane will display the 4 databases in a resizable grid of 2 rows and 2 columns. The second
+pane will display the services in a single row of 4 columns. The last pane will
+display the two services in a single column of 2 rows.
+
 ## Reference
 
 The options in **bold** are mandatory, while the others can be omitted.
 
 ### YAML Configuration file
+
 | Option               | Description                                                                    |
 |----------------------|--------------------------------------------------------------------------------|
 | **tasks** _(object)_ | a mapping between task names and the [task configuration](#task_configuration) |
-| **gui** _(object)_   | a mapping between pane names and the [pane configuration](#pane_configuration) |
+| gui _(object)_       | the [gui configuration](#gui_configuration)                                    |
+
+#### <a name="gui_configuration"></a> GUI configuration
+
+| Option             | Description                                                                    |
+|--------------------|--------------------------------------------------------------------------------|
+| palette _(string)_ | apply a specific color palette (see [available palettes](#color_palettes))     |
+| panes _(object)_   | a mapping between pane names and the [pane configuration](#pane_configuration) |
 
 #### <a name="pane_configuration"></a> Pane configuration
 
 | Option                  | Description                                          |
 |-------------------------|------------------------------------------------------|
 | **tasks** _(array)_     | the tasks that will be displayed in this pane        |
 | **columns** _(integer)_ | the number of columns you want the pane divided into |
@@ -163,7 +206,15 @@
 | **container_name** _(string)_ | the name to give to the container                                                           |
 | **image** _(string)_          | the docker image to run                                                                     |
 | docker_arguments _(array)_    | any additional arguments for the *docker run* command, to be inserted before the image name |
 | docker_command _(array)_      | any arguments to be appended after the image name                                           |
 | environment _(object)_        | env variables to be passed to the docker container                                          |
 | working_directory _(string)_  | a working directory for the docker command to be run from                                   |
 | stop_at_exit _(boolean)_      | will stop the container when the task is closed                                             |
+
+### <a name="color_palettes"></a> Available color palettes
+
+- darcula (default)
+- monokai
+- kimbie-dark
+- solarized-dark
+- hacker
```

### Comparing `jorun-0.2.0/pyproject.toml` & `jorun-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jorun"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Paolo Infante", email="info@paoloinfante.it" },
 ]
 description = "A customizable task runner"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jorun-0.2.0/PKG-INFO` & `jorun-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jorun
-Version: 0.2.0
+Version: 0.2.1
 Summary: A customizable task runner
 Project-URL: Homepage, https://github.com/paolo-projects/jorun
 Project-URL: Bug Tracker, https://github.com/paolo-projects/jorun/issues
 Author-email: Paolo Infante <info@paoloinfante.it>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,23 +47,25 @@
 jorun ./conf.yml
 ```
 
 ## Configuration
 
 ```yml
 gui:
-  services:
-    tasks:
-      - db
-      - redis
-  terminals:
-    tasks:
-      - test_1
-      - test_2
-      - test_3
+  panes:
+    services:
+      tasks:
+        - db
+        - redis
+    terminals:
+      tasks:
+        - test_1
+        - test_2
+        - test_3
+  palette: hacker
 tasks:
   db:
     type: docker
     docker:
       container_name: test
       image: postgres
       docker_arguments:
@@ -105,51 +107,92 @@
     type: shell
     shell:
       command: echo TEST 3
     depends:
       - test
 ```
 
-This sample YML file shows two task types you can run:
+This sample YML file shows three task types you can run:
 
 - **Shell**: a task launching a shell command
 - **Docker**: a task optimized for docker containers
-- **Group**: a task that groups other tasks (for parallel execution)
+- **Group**: a task that groups other tasks. Used when you have a lot of tasks with the same dependencies, to avoid writing all of them every time 
 
 The task runner supports searching for a pattern in the task output to
 signal its completion. This way you can start a dependent task after the pattern
 shows up in the task output.
 
-Tasks are chained through dependencies. 
+Tasks are chained through dependencies.
 The first tasks to run are the ones without dependencies.
 If you declare one or more dependencies, the task will not run until all the dependencies are either:
 
-- *completed* (i.e. the task finished executing), by default
-- _the completion pattern is matched_ (the regex pattern matched a line of the task output), if you set a **completion_pattern**
-- _launched_, if you set the **run_mode** to `indefinite`
+- **completed** (i.e. the task finished executing), by default
+- **the completion pattern is matched** (the regex pattern matched a line of the task output), if you set a
+  **completion_pattern**
+- **launched**, if you set the **run_mode** to `indefinite`
 
 ## GUI
 
 If you run **Jorun** with the `--gui` command line option, or if you specify the **gui** option
 in the yaml configuration you can start the tool with a graphical interface.
 The GUI is still a prototype, but will let you keep track of the task logs individually and
 even filter the log rows.
 
 The **gui** section in the YML configuration is where you can specify the panes you want displayed,
 and for each pane you can set the tasks that belong to it and the maximum number of columns visible in the pane.
 
+For instance, let's say you have 10 tasks in which you have 4 databases, 4 REST services, and 2 queues.
+You then have this GUI configuration:
+
+```yml
+gui:
+  panes:
+    databases:
+      tasks:
+        - postgres
+        - redis
+        - mongo
+        - cassandra
+      columns: 2
+    services:
+      tasks:
+        - auth
+        - orders
+        - customers
+        - shipments
+      columns: 4
+    pubsub:
+      tasks:
+        - rabbitmq
+        - kafka
+      columns: 1
+  palette: hacker
+```
+
+The first pane will display the 4 databases in a resizable grid of 2 rows and 2 columns. The second
+pane will display the services in a single row of 4 columns. The last pane will
+display the two services in a single column of 2 rows.
+
 ## Reference
 
 The options in **bold** are mandatory, while the others can be omitted.
 
 ### YAML Configuration file
+
 | Option               | Description                                                                    |
 |----------------------|--------------------------------------------------------------------------------|
 | **tasks** _(object)_ | a mapping between task names and the [task configuration](#task_configuration) |
-| **gui** _(object)_   | a mapping between pane names and the [pane configuration](#pane_configuration) |
+| gui _(object)_       | the [gui configuration](#gui_configuration)                                    |
+
+#### <a name="gui_configuration"></a> GUI configuration
+
+| Option             | Description                                                                    |
+|--------------------|--------------------------------------------------------------------------------|
+| palette _(string)_ | apply a specific color palette (see [available palettes](#color_palettes))     |
+| panes _(object)_   | a mapping between pane names and the [pane configuration](#pane_configuration) |
 
 #### <a name="pane_configuration"></a> Pane configuration
 
 | Option                  | Description                                          |
 |-------------------------|------------------------------------------------------|
 | **tasks** _(array)_     | the tasks that will be displayed in this pane        |
 | **columns** _(integer)_ | the number of columns you want the pane divided into |
@@ -181,7 +224,15 @@
 | **container_name** _(string)_ | the name to give to the container                                                           |
 | **image** _(string)_          | the docker image to run                                                                     |
 | docker_arguments _(array)_    | any additional arguments for the *docker run* command, to be inserted before the image name |
 | docker_command _(array)_      | any arguments to be appended after the image name                                           |
 | environment _(object)_        | env variables to be passed to the docker container                                          |
 | working_directory _(string)_  | a working directory for the docker command to be run from                                   |
 | stop_at_exit _(boolean)_      | will stop the container when the task is closed                                             |
+
+### <a name="color_palettes"></a> Available color palettes
+
+- darcula (default)
+- monokai
+- kimbie-dark
+- solarized-dark
+- hacker
```

