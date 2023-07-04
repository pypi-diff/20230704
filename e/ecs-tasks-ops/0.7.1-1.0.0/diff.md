# Comparing `tmp/ecs-tasks-ops-0.7.1.tar.gz` & `tmp/ecs_tasks_ops-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs-tasks-ops-0.7.1.tar", max compression
+gzip compressed data, was "ecs_tasks_ops-1.0.0.tar", max compression
```

## Comparing `ecs-tasks-ops-0.7.1.tar` & `ecs_tasks_ops-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
--rw-r--r--   0        0        0     1092 2022-08-30 18:17:06.908965 ecs-tasks-ops-0.7.1/LICENSE.rst
--rw-r--r--   0        0        0     5655 2022-08-30 18:17:06.908965 ecs-tasks-ops-0.7.1/README.rst
--rw-r--r--   0        0        0     1923 2022-08-30 18:17:22.349009 ecs-tasks-ops-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       21 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/__init__.py
--rw-r--r--   0        0        0     6130 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/__main__.py
--rw-r--r--   0        0        0      693 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/ecs_conf.py
--rw-r--r--   0        0        0     8282 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/ecs_data.py
--rw-r--r--   0        0        0     5501 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/ecs_facade.py
--rw-r--r--   0        0        0     1497 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/ecs_ssh.py
--rw-r--r--   0        0        0      524 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/pretty_json.py
--rw-r--r--   0        0        0      948 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/pretty_table.py
--rw-r--r--   0        0        0        0 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/py.typed
--rw-r--r--   0        0        0       57 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/__init__.py
--rw-r--r--   0        0        0      285 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/__main__.py
--rw-r--r--   0        0        0     3550 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/about.py
--rw-r--r--   0        0        0     3344 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/about.ui
--rw-r--r--   0        0        0     4991 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/main_window.py
--rw-r--r--   0        0        0     4652 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/mainwindow.ui
--rw-r--r--   0        0        0    28374 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/qt5_ecs.py
--rw-r--r--   0        0        0     3282 2022-08-30 18:17:06.912966 ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/qt5_gui.py
--rw-r--r--   0        0        0     6881 2022-08-30 18:17:24.498860 ecs-tasks-ops-0.7.1/setup.py
--rw-r--r--   0        0        0     6630 2022-08-30 18:17:24.499621 ecs-tasks-ops-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2022-01-18 16:08:09.175777 ecs_tasks_ops-1.0.0/LICENSE.rst
+-rw-r--r--   0        0        0     5655 2022-01-19 18:00:54.097700 ecs_tasks_ops-1.0.0/README.rst
+-rw-r--r--   0        0        0     1921 2023-07-04 08:34:27.541346 ecs_tasks_ops-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2020-10-08 14:56:05.755072 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/__init__.py
+-rw-r--r--   0        0        0     6130 2022-05-30 15:09:52.948780 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/__main__.py
+-rw-r--r--   0        0        0      693 2020-12-15 16:28:44.258252 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/ecs_conf.py
+-rw-r--r--   0        0        0     8282 2022-05-30 15:14:54.118049 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/ecs_data.py
+-rw-r--r--   0        0        0     5501 2020-12-16 19:14:22.464997 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/ecs_facade.py
+-rw-r--r--   0        0        0     1456 2023-07-03 14:52:32.720136 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/ecs_ssh.py
+-rw-r--r--   0        0        0      524 2020-12-17 12:01:56.020152 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/pretty_json.py
+-rw-r--r--   0        0        0      948 2020-12-15 18:30:36.478526 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/pretty_table.py
+-rw-r--r--   0        0        0        0 2020-10-07 16:20:25.687882 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/py.typed
+-rw-r--r--   0        0        0       57 2020-12-15 18:22:04.964437 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/__init__.py
+-rw-r--r--   0        0        0      285 2020-12-15 18:07:17.545356 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/__main__.py
+-rw-r--r--   0        0        0     3550 2020-12-15 18:36:18.125655 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/about.py
+-rw-r--r--   0        0        0     3344 2020-12-16 12:42:15.353107 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/about.ui
+-rw-r--r--   0        0        0     4991 2022-10-08 17:15:37.007197 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/main_window.py
+-rw-r--r--   0        0        0     4652 2020-12-15 17:05:42.851873 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/mainwindow.ui
+-rw-r--r--   0        0        0    28840 2023-07-04 07:38:10.483488 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/qt5_ecs.py
+-rw-r--r--   0        0        0     3282 2020-12-15 18:40:28.965022 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/qt5_gui.py
+-rw-r--r--   0        0        0      744 2023-07-04 08:34:51.508881 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/terminal.html
+-rw-r--r--   0        0        0     2097 2023-07-04 08:48:38.229137 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/terminal.js
+-rw-r--r--   0        0        0     6550 2023-07-04 08:45:55.225152 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/terminal.py
+-rw-r--r--   0        0        0     3318 2023-07-04 08:34:53.998902 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/xterm-addon-fit.js
+-rw-r--r--   0        0        0     6082 2023-07-04 08:34:51.728883 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/xterm-addon-web-links.js
+-rw-r--r--   0        0        0     4246 2023-07-04 08:34:51.497881 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/xterm.css
+-rw-r--r--   0        0        0   863113 2023-07-04 08:34:53.972901 ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/xterm.js
+-rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 ecs_tasks_ops-1.0.0/PKG-INFO
```

### Comparing `ecs-tasks-ops-0.7.1/LICENSE.rst` & `ecs_tasks_ops-1.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/README.rst` & `ecs_tasks_ops-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/pyproject.toml` & `ecs_tasks_ops-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 [tool.poetry]
 name = "ecs-tasks-ops"
-version = "0.7.1"
+version = "1.0.0"
 description = "Ecs Tasks Ops"
 authors = ["Pablo Palazon <ppalazon@antara.ws>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ppalazon/ecs-tasks-ops"
 repository = "https://github.com/ppalazon/ecs-tasks-ops"
 documentation = "https://ecs-tasks-ops.readthedocs.io"
 classifiers = [
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 packages = [
     { include = "ecs_tasks_ops", from = 'src' },
     { include = "ecs_tasks_ops_qt5", from = 'src' },
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/ppalazon/ecs-tasks-ops/releases"
 
 [tool.poetry.dependencies]
-python = "^3.6.1"
-click = ">=7,<9"
-boto3 = "^1.15.13"
-tabulate = "^0.8.7"
-PyQt5 = "^5.15.1"
-moto = {extras = ["ecs", "ec2"], version = ">=3.0.3,<5.0.0"}
+python = "^3.11.4"
+click = "^8.1.3"
+boto3 = "^1.27.0"
+tabulate = "^0.9.0"
+PyQt5 = "^5.15.9"
+PyQtWebEngine = "^5.15.6"
+moto = {extras = ["ec2", "ecs"], version = "^4.1.12"}
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.0.0"
-coverage = {extras = ["toml"], version = "^6.0.2"}
-safety = "^2.1.0"
-mypy = "^0.971"
-typeguard = "^2.9.1"
-xdoctest = {extras = ["colors"], version = "^1.0.0"}
-sphinx = "^4.2.0"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+coverage = {extras = ["toml"], version = "^7.2.7"}
+safety = "^2.3.5"
+mypy = "^1.4.1"
+typeguard = "^4.0.0"
+xdoctest = {extras = ["colors"], version = "^1.1.1"}
+sphinx = "^7.0.1"
 sphinx-autobuild = "^2021.3.14"
-pre-commit = "^2.8.2"
-flake8 = "^4.0.1"
-black = "^20.8b1"
-flake8-bandit = "^2.1.2"
-flake8-bugbear = "^22.1.11"
-flake8-docstrings = "^1.5.0"
-flake8-rst-docstrings = "^0.2.3"
-pep8-naming = "^0.13.0"
-darglint = "^1.5.5"
-reorder-python-imports = "^2.3.6"
-pre-commit-hooks = "^4.0.1"
-sphinx-rtd-theme = "^1.0.0"
-sphinx-click = "^3.0.1"
-Pygments = "^2.7.2"
-nox-poetry = "^0.8.6"
-rope = "^1.0.0"
-pytest-cov = "^3.0.0"
-rstcheck = "^3.3.1"
-sphinx-autodoc-typehints = "^1.12.0"
-codecov = "^2.1.12"
+pre-commit = "^3.3.3"
+flake8 = "^6.0.0"
+black = "^23.3.0"
+flake8-bandit = "^4.1.1"
+flake8-bugbear = "^23.6.5"
+flake8-docstrings = "^1.7.0"
+flake8-rst-docstrings = "^0.3.0"
+pep8-naming = "^0.13.3"
+darglint = "^1.8.1"
+reorder-python-imports = "^3.10.0"
+pre-commit-hooks = "^4.4.0"
+sphinx-click = "^4.4.0"
+Pygments = "^2.15.1"
+nox-poetry = "^1.0.2"
+rope = "^1.9.0"
+pytest-cov = "^4.1.0"
+rstcheck = "^6.1.2"
+sphinx-autodoc-typehints = "^1.23.3"
+codecov = "^2.1.13"
 
 [tool.poetry.scripts]
 ecs-tasks-ops = "ecs_tasks_ops.__main__:main"
 ecs-tasks-ops-qt5 = "ecs_tasks_ops_qt5.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/__main__.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/__main__.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/ecs_conf.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/ecs_conf.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/ecs_data.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/ecs_data.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/ecs_facade.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/ecs_facade.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/ecs_ssh.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/ecs_ssh.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """Generate ssh commands to access to ECS resources."""
 
 
 def ssh_cmd_container_instance(detail) -> str:
     """SSH command to access a ecs2 instance by id."""
-    return f"TERM=xterm ssh {detail['ec2InstanceId']}"
+    return f"ssh -tt {detail['ec2InstanceId']}"
 
 
 def ssh_cmd_task_log(detail) -> str:
     """SSH command to access the first docker instance logs of a task."""
-    return f"TERM=xterm ssh {detail['ec2InstanceId']} docker logs -f --tail=100 {detail['containers'][0]['runtimeId']}"
+    return f"ssh -tt {detail['ec2InstanceId']} docker logs -f --tail=100 {detail['containers'][0]['runtimeId']}"
 
 
 def ssh_cmd_task_exec(detail, command_on_docker, wait_press_key=None) -> str:
     """SSH command to execute a command inside the first docker containter of a task."""
     wait_cmd = ""
     if wait_press_key:
         wait_cmd = "; echo 'Press a key'; read q"
     return (
-        f"TERM=xterm ssh -t {detail['ec2InstanceId']} docker exec -ti {detail['containers'][0]['runtimeId']} {command_on_docker}"
+        f"ssh -tt {detail['ec2InstanceId']} docker exec -ti {detail['containers'][0]['runtimeId']} {command_on_docker}"
         + wait_cmd
     )
 
 
 def ssh_cmd_docker_container_log(detail) -> str:
     """SSH command to access a docker instance logs."""
-    return f"TERM=xterm ssh {detail['ec2InstanceId']} docker logs -f --tail=100 {detail['runtimeId']}"
+    return f"ssh -tt {detail['ec2InstanceId']} docker logs -f --tail=100 {detail['runtimeId']}"
 
 
 def ssh_cmd_docker_container_exec(
     detail, command_on_docker, wait_press_key=None
 ) -> str:
     """SSH command to execute a command inside a docker containter."""
     wait_cmd = ""
     if wait_press_key:
         wait_cmd = "; echo 'Press a key'; read q"
     return (
-        f"TERM=xterm ssh -t {detail['ec2InstanceId']} docker exec -ti {detail['runtimeId']} {command_on_docker}"
+        f"ssh -tt {detail['ec2InstanceId']} docker exec -ti {detail['runtimeId']} {command_on_docker}"
         + wait_cmd
     )
```

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/pretty_json.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/pretty_json.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops/pretty_table.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops/pretty_table.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/about.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/about.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/about.ui` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/about.ui`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/main_window.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/main_window.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/mainwindow.ui` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/qt5_ecs.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/qt5_ecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from PyQt5 import QtWidgets
 
 from ecs_tasks_ops import ecs_conf
 from ecs_tasks_ops import ecs_data
 from ecs_tasks_ops import ecs_facade
 from ecs_tasks_ops import ecs_ssh
 from ecs_tasks_ops import pretty_json
+from ecs_tasks_ops_qt5 import terminal
 
 
 class ECSTreeItem(QtWidgets.QTreeWidgetItem):
     """Tree Widgets Item for ECS elements."""
 
     def __init__(self, name, identifier, detail_type, detail, parent=None):
         """Initialization of basic ECS element, with name, arn_id, type and json data."""
@@ -84,15 +85,15 @@
 
 class ECSListServicesClusterTreeItem(ECSTreeItem):
     """Tree Widgets Item for List of Services of a cluster."""
 
     def __init__(self, detail, parent=None):
         """Initilize info to get a list of services for a cluster."""
         super(ECSListServicesClusterTreeItem, self).__init__(
-            name=f"Services on '{detail['clusterName']}'",
+            name=f"Services on '{detail['clusterName']!r}'",
             identifier=detail["clusterName"],
             detail_type="list_services",
             detail=detail,
             parent=parent,
         )
 
     def refresh_children(self):
@@ -104,15 +105,15 @@
 
 class ECSListTasksClusterTreeItem(ECSTreeItem):
     """Tree Widgets Item for List of Tasks of a cluster."""
 
     def __init__(self, detail, parent=None):
         """Initialize info to get a list of tasks for a cluster."""
         super(ECSListTasksClusterTreeItem, self).__init__(
-            name=f"Tasks on '{detail['clusterName']}'",
+            name=f"Tasks on '{detail['clusterName']!r}'",
             identifier=detail["clusterName"],
             detail_type="list_services",
             detail=detail,
             parent=parent,
         )
 
     def refresh_children(self):
@@ -124,15 +125,15 @@
 
 class ECSListContainersClusterTreeItem(ECSTreeItem):
     """Tree Widgets Item for List of Containers Instances of a cluster."""
 
     def __init__(self, detail, parent=None):
         """Initialize info to get a list of container instances for a cluster."""
         super(ECSListContainersClusterTreeItem, self).__init__(
-            name=f"Containers on '{detail['clusterName']}'",
+            name=f"Containers on '{detail['clusterName']!r}'",
             identifier=detail["clusterName"],
             detail_type="list_services",
             detail=detail,
             parent=parent,
         )
 
     def refresh_children(self):
@@ -668,41 +669,52 @@
 
 class EmbTerminal(QtWidgets.QWidget):
     """Open a embedded terminal widget."""
 
     def __init__(self, bash_command, parent=None):
         """Initilize parameters and open a terminal."""
         super(EmbTerminal, self).__init__(parent)
-        self.process = QtCore.QProcess(self)
-        self.terminal = QtWidgets.QWidget(self)
+
+        terminal_args = []
+        if bash_command:
+            terminal_args = ["-c", bash_command] + terminal_args
+            # terminal_args = ["-e", "bash", "-c", bash_command] + terminal_args
+        # self.process.start(
+        #     "urxvt", ["-embed", str(int(self.terminal.winId()))] + terminal_args
+        # )
+
+        self.terminal = terminal.TerminalWidget(self)
+        # self.terminal = QtWidgets.QWidget(self)
         self.command = QtWidgets.QLineEdit(self)
         self.command.setReadOnly(True)
         self.command.setText(bash_command)
         layout = QtWidgets.QVBoxLayout(self)
         layout.addWidget(self.command)
         layout.addWidget(self.terminal)
 
+        self.terminal.start("/bin/bash", ["--norc", "-r"] + terminal_args)
+
         # env = QtCore.QProcessEnvironment.systemEnvironment()
         # env.insert("TERM", "xterm")
         # self.process.setProcessEnvironment(env)
 
         # Log errors
         # self.process.error.connect(self.log_error)
 
         # Works also with urxvt:
-        terminal_args = []
-        if bash_command:
-            terminal_args = ["-e", "bash", "-c", bash_command] + terminal_args
-        self.process.start(
-            "urxvt", ["-embed", str(int(self.terminal.winId()))] + terminal_args
-        )
+        # terminal_args = []
+        # if bash_command:
+        #     terminal_args = ["-e", "bash", "-c", bash_command] + terminal_args
+        # self.process.start(
+        #     "urxvt", ["-embed", str(int(self.terminal.winId()))] + terminal_args
+        # )
 
     def closeEvent(self, event):
         """Close terminal and process."""
-        self.process.terminate()
+        self.terminal.close()
 
     def log_error(self, error):
         """Show log error information."""
         print(error)
 
 
 class ShowServiceEvents(QtWidgets.QWidget):
```

### Comparing `ecs-tasks-ops-0.7.1/src/ecs_tasks_ops_qt5/qt5_gui.py` & `ecs_tasks_ops-1.0.0/src/ecs_tasks_ops_qt5/qt5_gui.py`

 * *Files identical despite different names*

### Comparing `ecs-tasks-ops-0.7.1/setup.py` & `ecs_tasks_ops-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,219 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ecs-tasks-ops
+Version: 1.0.0
+Summary: Ecs Tasks Ops
+Home-page: https://github.com/ppalazon/ecs-tasks-ops
+License: MIT
+Author: Pablo Palazon
+Author-email: ppalazon@antara.ws
+Requires-Python: >=3.11.4,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyQt5 (>=5.15.9,<6.0.0)
+Requires-Dist: PyQtWebEngine (>=5.15.6,<6.0.0)
+Requires-Dist: boto3 (>=1.27.0,<2.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: moto[ec2,ecs] (>=4.1.12,<5.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Project-URL: Changelog, https://github.com/ppalazon/ecs-tasks-ops/releases
+Project-URL: Documentation, https://ecs-tasks-ops.readthedocs.io
+Project-URL: Repository, https://github.com/ppalazon/ecs-tasks-ops
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+ECS Tasks Ops
+=============
 
-packages = \
-['ecs_tasks_ops', 'ecs_tasks_ops_qt5']
+|PyPI| |Python Version| |License|
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyQt5>=5.15.1,<6.0.0',
- 'boto3>=1.15.13,<2.0.0',
- 'click>=7,<9',
- 'moto[ec2,ecs]>=3.0.3,<5.0.0',
- 'tabulate>=0.8.7,<0.9.0']
-
-entry_points = \
-{'console_scripts': ['ecs-tasks-ops = ecs_tasks_ops.__main__:main',
-                     'ecs-tasks-ops-qt5 = ecs_tasks_ops_qt5.__main__:main']}
-
-setup_kwargs = {
-    'name': 'ecs-tasks-ops',
-    'version': '0.7.1',
-    'description': 'Ecs Tasks Ops',
-    'long_description': 'ECS Tasks Ops\n=============\n\n|PyPI| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/ecs-tasks-ops.svg\n   :target: https://pypi.org/project/ecs-tasks-ops/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/ecs-tasks-ops\n   :target: https://pypi.org/project/ecs-tasks-ops\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/ecs-tasks-ops\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/ecs-tasks-ops/latest.svg?label=Read%20the%20Docs\n   :target: https://ecs-tasks-ops.readthedocs.io/\n   :alt: Read the documentation at https://ecs-tasks-ops.readthedocs.io/\n.. |Tests| image:: https://github.com/ppalazon/ecs-tasks-ops/workflows/Tests/badge.svg\n   :target: https://github.com/ppalazon/ecs-tasks-ops/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/ppalazon/ecs-tasks-ops/branch/main/graph/badge.svg?token=zaz1KPR73Q\n   :target: https://codecov.io/gh/ppalazon/ecs-tasks-ops\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n\nFeatures\n--------\n\n* Application GUI to manage ECS resources\n* Use your home aws credentials from ~/.aws/credentials\n* Get information and attributes for each task, service or instance container\n* Connect through SSH to container instances or docker container\n* Show logs for each docker container\n* Show ECS events for a service\n* Force restart for a service\n\nRequirements\n------------\n\n* Python 3.10\n* `boto3 <https://pypi.org/project/boto3/>`_\n* `click <https://pypi.org/project/click/>`_\n* `tabulate <https://pypi.org/project/tabulate/>`_\n* `PyQt5 <https://pypi.org/project/PyQt5/>`_\n* `moto <https://pypi.org/project/moto/>`_\n* uxrvt\n\n\nInstallation\n------------\n\nYou can install *Ecs Tasks Ops* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install ecs-tasks-ops\n\n\nConfiguration\n-------------\n\nAWS Access\n^^^^^^^^^^\n\nThis application uses your aws credentials to connect to your ECS, so you need to configure your credentials.\n\nSet up credentials (in e.g. ``~/.aws/credentials``)\n\n.. code:: ini\n\n   [default]\n   aws_access_key_id = YOUR_KEY\n   aws_secret_access_key = YOUR_SECRET\n\nThen, you set up a default region (in e.g. ``~/.aws/config``)\n\n.. code:: ini\n\n   [default]\n   region=us-east-1\n\nYou can read more about it in `boto3 <https://pypi.org/project/boto3/>`_\n\n``ssh`` over ``ssm``\n^^^^^^^^^^^^^^^^^^^^\n\nIf you want to access to containers instances or docker container through ``ssh``, you must configurate ``ssm`` in your EC2 machines.\nThat\'s because ``ecs-tasks-ops`` use its instance id as machine identifier on ``ssh`` command. For example, ``ssh i-0123456789ABCDE``.\nI use `ssh-over-ssm <https://github.com/elpy1/ssh-over-ssm>`_ tool to configure ``ssh`` over ``ssm`` to connect to instances.\n\nPredefined Commands\n^^^^^^^^^^^^^^^^^^^\n\nYou can set multiples predefined commands to execute on docker containers. You can set them in a configuration file called ``ecs-tasks-ops.json``.\nThis file can be located on ``~``, ``~/.config/ecs-tasks-ops``, ``/etc/ecs-tasks-ops``, or any directory configured in the enviromental variable\n``ECS_TASKS_OPS_CONF``\n\nSample configuration\n\n.. code-block:: json\n\n   {\n      "commands": [\n         "/bin/sh",\n         "/bin/bash",\n         "mongo admin -u root -p $(pass mongo/root)"\n      ]\n   }\n\nGUI Usage\n---------\n\nYou can open the ``qt5`` application, using the following command\n\n.. code:: console\n\n   ecs-tasks-ops-qt5\n\nCLI Usage\n---------\n\nYou can open the command line with ``ecs-tasks-ops`` command. This is the help menu:\n\n.. code::\n\n   Usage: ecs-tasks-ops [OPTIONS] COMMAND [ARGS]...\n\n      Ecs Tasks Ops.\n\n   Options:\n      -x, --debug / --no-debug\n      -j, --output-json\n      --version                 Show the version and exit.\n      --help                    Show this message and exit.\n\n   Commands:\n      clusters             Clusters information.\n      container-instances  Container instances defined in a cluster.\n      containers           Get docker containers defined in a cluster.\n      services             Services defined in a cluster.\n      tasks                Set tasks defined in a cluster.\n\nBy default, the output format is in a table, but you can get original ``json`` format with ``-j`` option.\nYou can filter json output with `jq <https://stedolan.github.io/jq/>`_ tool:\n\n.. code:: console\n\n   $ ecs-tasks-ops -j clusters | jq "."\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the MIT_ license,\n*Ecs Tasks Ops* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\n\nCredits\n-------\n\nThis project was generated from `@cjolowicz`_\'s `Hypermodern Python Cookiecutter`_ template.\n\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _MIT: http://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _file an issue: https://github.com/ppalazon/ecs-tasks-ops/issues\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n',
-    'author': 'Pablo Palazon',
-    'author_email': 'ppalazon@antara.ws',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ppalazon/ecs-tasks-ops',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6.1,<4.0.0',
-}
+|Read the Docs| |Tests| |Codecov|
 
+|pre-commit| |Black|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/ecs-tasks-ops.svg
+   :target: https://pypi.org/project/ecs-tasks-ops/
+   :alt: PyPI
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/ecs-tasks-ops
+   :target: https://pypi.org/project/ecs-tasks-ops
+   :alt: Python Version
+.. |License| image:: https://img.shields.io/pypi/l/ecs-tasks-ops
+   :target: https://opensource.org/licenses/MIT
+   :alt: License
+.. |Read the Docs| image:: https://img.shields.io/readthedocs/ecs-tasks-ops/latest.svg?label=Read%20the%20Docs
+   :target: https://ecs-tasks-ops.readthedocs.io/
+   :alt: Read the documentation at https://ecs-tasks-ops.readthedocs.io/
+.. |Tests| image:: https://github.com/ppalazon/ecs-tasks-ops/workflows/Tests/badge.svg
+   :target: https://github.com/ppalazon/ecs-tasks-ops/actions?workflow=Tests
+   :alt: Tests
+.. |Codecov| image:: https://codecov.io/gh/ppalazon/ecs-tasks-ops/branch/main/graph/badge.svg?token=zaz1KPR73Q
+   :target: https://codecov.io/gh/ppalazon/ecs-tasks-ops
+   :alt: Codecov
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Black
+
+
+Features
+--------
+
+* Application GUI to manage ECS resources
+* Use your home aws credentials from ~/.aws/credentials
+* Get information and attributes for each task, service or instance container
+* Connect through SSH to container instances or docker container
+* Show logs for each docker container
+* Show ECS events for a service
+* Force restart for a service
+
+Requirements
+------------
+
+* Python 3.10
+* `boto3 <https://pypi.org/project/boto3/>`_
+* `click <https://pypi.org/project/click/>`_
+* `tabulate <https://pypi.org/project/tabulate/>`_
+* `PyQt5 <https://pypi.org/project/PyQt5/>`_
+* `moto <https://pypi.org/project/moto/>`_
+* uxrvt
+
+
+Installation
+------------
+
+You can install *Ecs Tasks Ops* via pip_ from PyPI_:
+
+.. code:: console
+
+   $ pip install ecs-tasks-ops
+
+
+Configuration
+-------------
+
+AWS Access
+^^^^^^^^^^
+
+This application uses your aws credentials to connect to your ECS, so you need to configure your credentials.
+
+Set up credentials (in e.g. ``~/.aws/credentials``)
+
+.. code:: ini
+
+   [default]
+   aws_access_key_id = YOUR_KEY
+   aws_secret_access_key = YOUR_SECRET
+
+Then, you set up a default region (in e.g. ``~/.aws/config``)
+
+.. code:: ini
+
+   [default]
+   region=us-east-1
+
+You can read more about it in `boto3 <https://pypi.org/project/boto3/>`_
+
+``ssh`` over ``ssm``
+^^^^^^^^^^^^^^^^^^^^
+
+If you want to access to containers instances or docker container through ``ssh``, you must configurate ``ssm`` in your EC2 machines.
+That's because ``ecs-tasks-ops`` use its instance id as machine identifier on ``ssh`` command. For example, ``ssh i-0123456789ABCDE``.
+I use `ssh-over-ssm <https://github.com/elpy1/ssh-over-ssm>`_ tool to configure ``ssh`` over ``ssm`` to connect to instances.
+
+Predefined Commands
+^^^^^^^^^^^^^^^^^^^
+
+You can set multiples predefined commands to execute on docker containers. You can set them in a configuration file called ``ecs-tasks-ops.json``.
+This file can be located on ``~``, ``~/.config/ecs-tasks-ops``, ``/etc/ecs-tasks-ops``, or any directory configured in the enviromental variable
+``ECS_TASKS_OPS_CONF``
+
+Sample configuration
+
+.. code-block:: json
+
+   {
+      "commands": [
+         "/bin/sh",
+         "/bin/bash",
+         "mongo admin -u root -p $(pass mongo/root)"
+      ]
+   }
+
+GUI Usage
+---------
+
+You can open the ``qt5`` application, using the following command
+
+.. code:: console
+
+   ecs-tasks-ops-qt5
+
+CLI Usage
+---------
+
+You can open the command line with ``ecs-tasks-ops`` command. This is the help menu:
+
+.. code::
+
+   Usage: ecs-tasks-ops [OPTIONS] COMMAND [ARGS]...
+
+      Ecs Tasks Ops.
+
+   Options:
+      -x, --debug / --no-debug
+      -j, --output-json
+      --version                 Show the version and exit.
+      --help                    Show this message and exit.
+
+   Commands:
+      clusters             Clusters information.
+      container-instances  Container instances defined in a cluster.
+      containers           Get docker containers defined in a cluster.
+      services             Services defined in a cluster.
+      tasks                Set tasks defined in a cluster.
+
+By default, the output format is in a table, but you can get original ``json`` format with ``-j`` option.
+You can filter json output with `jq <https://stedolan.github.io/jq/>`_ tool:
+
+.. code:: console
+
+   $ ecs-tasks-ops -j clusters | jq "."
+
+Contributing
+------------
+
+Contributions are very welcome.
+To learn more, see the `Contributor Guide`_.
+
+
+License
+-------
+
+Distributed under the terms of the MIT_ license,
+*Ecs Tasks Ops* is free and open source software.
+
+
+Issues
+------
+
+If you encounter any problems,
+please `file an issue`_ along with a detailed description.
+
+
+Credits
+-------
+
+This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.
+
+
+.. _@cjolowicz: https://github.com/cjolowicz
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _MIT: http://opensource.org/licenses/MIT
+.. _PyPI: https://pypi.org/
+.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+.. _file an issue: https://github.com/ppalazon/ecs-tasks-ops/issues
+.. _pip: https://pip.pypa.io/
+.. github-only
+.. _Contributor Guide: CONTRIBUTING.rst
 
-setup(**setup_kwargs)
```

