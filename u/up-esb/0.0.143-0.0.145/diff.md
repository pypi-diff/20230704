# Comparing `tmp/up_esb-0.0.143.tar.gz` & `tmp/up_esb-0.0.145.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_esb-0.0.143.tar", last modified: Mon Jul  3 13:32:34 2023, max compression
+gzip compressed data, was "up_esb-0.0.145.tar", last modified: Tue Jul  4 15:13:31 2023, max compression
```

## Comparing `up_esb-0.0.143.tar` & `up_esb-0.0.145.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.797967 up_esb-0.0.143/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.789967 up_esb-0.0.143/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.789967 up_esb-0.0.143/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-03 13:32:14.000000 up_esb-0.0.143/.github/scripts/update_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.789967 up_esb-0.0.143/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-03 13:32:14.000000 up_esb-0.0.143/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 13:32:14.000000 up_esb-0.0.143/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-03 13:32:14.000000 up_esb-0.0.143/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 13:32:14.000000 up_esb-0.0.143/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 13:32:14.000000 up_esb-0.0.143/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-03 13:32:34.797967 up_esb-0.0.143/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-03 13:32:14.000000 up_esb-0.0.143/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.789967 up_esb-0.0.143/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-03 13:32:14.000000 up_esb-0.0.143/docs/callable_interface.md
--rw-r--r--   0 runner    (1001) docker     (123)    37750 2023-07-03 13:32:14.000000 up_esb-0.0.143/docs/create_action_interface.drawio.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.793967 up_esb-0.0.143/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-03 13:32:14.000000 up_esb-0.0.143/examples/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-03 13:32:14.000000 up_esb-0.0.143/examples/partialorderplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-03 13:32:14.000000 up_esb-0.0.143/examples/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-03 13:32:14.000000 up_esb-0.0.143/examples/time_triggered.py
--rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-07-03 13:32:14.000000 up_esb-0.0.143/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:32:34.797967 up_esb-0.0.143/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-03 13:32:14.000000 up_esb-0.0.143/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.793967 up_esb-0.0.143/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-03 13:32:14.000000 up_esb-0.0.143/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.793967 up_esb-0.0.143/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:14.000000 up_esb-0.0.143/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-03 13:32:14.000000 up_esb-0.0.143/tests/components/test_expression_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-07-03 13:32:14.000000 up_esb-0.0.143/tests/test_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-03 13:32:14.000000 up_esb-0.0.143/tests/test_create_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-03 13:32:14.000000 up_esb-0.0.143/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-03 13:32:14.000000 up_esb-0.0.143/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-03 13:32:14.000000 up_esb-0.0.143/tests/test_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.793967 up_esb-0.0.143/up_esb/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.793967 up_esb-0.0.143/up_esb/components/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/components/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/components/expression_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/components/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.797967 up_esb-0.0.143/up_esb/plexmo/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/plexmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/plexmo/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-03 13:32:14.000000 up_esb-0.0.143/up_esb/plexmo/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:32:34.793967 up_esb-0.0.143/up_esb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-03 13:32:34.000000 up_esb-0.0.143/up_esb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-03 13:32:34.000000 up_esb-0.0.143/up_esb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:32:34.000000 up_esb-0.0.143/up_esb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 13:32:34.000000 up_esb-0.0.143/up_esb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 13:32:34.000000 up_esb-0.0.143/up_esb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.490395 up_esb-0.0.145/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.482395 up_esb-0.0.145/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.482395 up_esb-0.0.145/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-04 15:13:14.000000 up_esb-0.0.145/.github/scripts/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.482395 up_esb-0.0.145/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-04 15:13:14.000000 up_esb-0.0.145/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 15:13:14.000000 up_esb-0.0.145/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 15:13:14.000000 up_esb-0.0.145/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-04 15:13:14.000000 up_esb-0.0.145/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 15:13:14.000000 up_esb-0.0.145/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-04 15:13:31.490395 up_esb-0.0.145/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-04 15:13:14.000000 up_esb-0.0.145/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.482395 up_esb-0.0.145/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-04 15:13:14.000000 up_esb-0.0.145/docs/callable_interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37750 2023-07-04 15:13:14.000000 up_esb-0.0.145/docs/create_action_interface.drawio.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.486395 up_esb-0.0.145/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-04 15:13:14.000000 up_esb-0.0.145/examples/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-04 15:13:14.000000 up_esb-0.0.145/examples/partialorderplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-04 15:13:14.000000 up_esb-0.0.145/examples/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-04 15:13:14.000000 up_esb-0.0.145/examples/time_triggered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-07-04 15:13:14.000000 up_esb-0.0.145/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:13:31.490395 up_esb-0.0.145/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 15:13:14.000000 up_esb-0.0.145/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.486395 up_esb-0.0.145/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-04 15:13:14.000000 up_esb-0.0.145/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.486395 up_esb-0.0.145/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:14.000000 up_esb-0.0.145/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-04 15:13:14.000000 up_esb-0.0.145/tests/components/test_expression_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-07-04 15:13:14.000000 up_esb-0.0.145/tests/test_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-04 15:13:14.000000 up_esb-0.0.145/tests/test_create_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-04 15:13:14.000000 up_esb-0.0.145/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-04 15:13:14.000000 up_esb-0.0.145/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-04 15:13:14.000000 up_esb-0.0.145/tests/test_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.486395 up_esb-0.0.145/up_esb/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.486395 up_esb-0.0.145/up_esb/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/components/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/components/expression_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/components/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.490395 up_esb-0.0.145/up_esb/plexmo/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/plexmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/plexmo/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-04 15:13:14.000000 up_esb-0.0.145/up_esb/plexmo/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:13:31.486395 up_esb-0.0.145/up_esb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-04 15:13:31.000000 up_esb-0.0.145/up_esb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 15:13:31.000000 up_esb-0.0.145/up_esb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:13:31.000000 up_esb-0.0.145/up_esb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-04 15:13:31.000000 up_esb-0.0.145/up_esb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 15:13:31.000000 up_esb-0.0.145/up_esb.egg-info/top_level.txt
```

### Comparing `up_esb-0.0.143/.github/scripts/update_version.py` & `up_esb-0.0.145/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/.github/workflows/deploy.yml` & `up_esb-0.0.145/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/.github/workflows/main.yml` & `up_esb-0.0.145/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/.gitignore` & `up_esb-0.0.145/.gitignore`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/.pre-commit-config.yaml` & `up_esb-0.0.145/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/LICENSE` & `up_esb-0.0.145/LICENSE`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/PKG-INFO` & `up_esb-0.0.145/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up_esb
-Version: 0.0.143
+Version: 0.0.145
 Summary: General functionalities for using unified-planning in robotic applications
 License: Apache-2.0 License
 Project-URL: Repository, https://github.com/aiplan4eu/embedded-systems-bridge
 Project-URL: Homepage, https://www.aiplan4eu-project.eu/
 Keywords: unified-planning,embedded-systems-bridge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `up_esb-0.0.143/README.md` & `up_esb-0.0.145/README.md`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/docs/callable_interface.md` & `up_esb-0.0.145/docs/callable_interface.md`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/docs/create_action_interface.drawio.png` & `up_esb-0.0.145/docs/create_action_interface.drawio.png`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/examples/parallel.py` & `up_esb-0.0.145/examples/parallel.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Example for parallel plan execution."""
 import time
 
-import matplotlib.pyplot as plt
-import networkx as nx
 import unified_planning as up
 from unified_planning.model import EndTiming, StartTiming
 
 from up_esb.bridge import Bridge
 from up_esb.executor import Executor
 
 
@@ -49,93 +47,89 @@
 
 
 class Robot:
     """Robot class."""
 
     location = "l1"
 
-    def __init__(self):
-        self.l_from = ""
-        self.l_to = ""
-
-    def move(self, l_from: Location, l_to: Location):
+    @classmethod
+    def move(cls, l_from: Location, l_to: Location):
         """Move the robot from one location to another."""
 
-        self.l_from, self.l_to = l_from, l_to
-        print(f"Moving from {self.l_from} to {self.l_to}")
+        print(f"Moving from {l_from} to {l_to}")
+        Robot.location = l_to
         time.sleep(2)
 
-    def survey(self, area: Area):
+    @classmethod
+    def survey(cls, area: Area):
         """Survey the area."""
         print(f"Surveying area {area}")
         time.sleep(5)
 
-    def send_info(self, location: Location):
+    @classmethod
+    def send_info(cls, location: Location):
         """Send info about the location."""
         print(f"Sending info about {location}")
-        self.l_to = location
+        Robot.l_to = location
 
 
-def robot_at_fun(l: Location):  # pylint: disable=unused-argument
+def robot_at_fun(l: Location):
     """Check if the robot is at the location."""
     return Robot.location == l
 
 
-def visited_fun(l: Location):  # pylint: disable=unused-argument
+def visited_fun(l: Location):
     """Check if the location is visited."""
     return Robot.location == l
 
 
 def is_surveyed_fun():
     """Check if the area is surveyed."""
     return True
 
 
-def info_sent_fun(l: Location):  # pylint: disable=unused-argument
+def info_sent_fun(_: Location):
     """Send info about the location."""
     return True
 
 
 #################### 2. Define the problem ####################
 
 
 def define_problem():
     """Define the problem."""
     bridge = Bridge()
-    robot = Robot()
 
     bridge.create_types([Location, Area, Robot])
 
     robot_at = bridge.create_fluent_from_function(robot_at_fun)
     visited = bridge.create_fluent_from_function(visited_fun)
     is_surveyed = bridge.create_fluent_from_function(is_surveyed_fun)
     info_sent = bridge.create_fluent_from_function(info_sent_fun)
 
     l1 = bridge.create_object("l1", Location("l1"))
     l2 = bridge.create_object("l2", Location("l2"))
     l3 = bridge.create_object("l3", Location("l3"))
     l4 = bridge.create_object("l4", Location("l4"))
-    area = bridge.create_object("area", Area(0, 10, 0, 10))  # pylint: disable=unused-variable
+    _ = bridge.create_object("area", Area(0, 10, 0, 10))
 
     move, [l_from, l_to] = bridge.create_action(
-        "Move", _callable=robot.move, l_from=Location, l_to=Location, duration=5
+        "Move", _callable=Robot.move, l_from=Location, l_to=Location, duration=5
     )
     move.add_condition(StartTiming(), info_sent(l_from))
     move.add_condition(StartTiming(), info_sent(l_to))
     move.add_condition(StartTiming(), robot_at(l_from))
     move.add_effect(StartTiming(), robot_at(l_from), False)
     move.add_effect(EndTiming(), robot_at(l_to), True)
     move.add_effect(EndTiming(), visited(l_to), True)
 
-    survey, [a] = bridge.create_action(  # pylint: disable=unused-variable
-        "Survey", _callable=robot.survey, area=Area, duration=5
-    )
+    survey, [_] = bridge.create_action("Survey", _callable=Robot.survey, area=Area, duration=5)
     survey.add_effect(EndTiming(), is_surveyed(), True)
 
-    send_info, [l] = bridge.create_action("SendInfo", _callable=robot.send_info, location=Location)
+    send_info, [l] = bridge.create_action("SendInfo", _callable=Robot.send_info, location=Location)
     send_info.add_precondition(is_surveyed())
     send_info.add_effect(info_sent(l), True)
 
     problem = bridge.define_problem()
     problem.set_initial_value(is_surveyed(), False)
     problem.set_initial_value(robot_at(l1), True)
     problem.set_initial_value(robot_at(l2), False)
@@ -169,29 +163,12 @@
     for action in plan.timed_actions:
         print(action)
     print("*" * 10)
 
     graph_executor = bridge.get_executable_graph(plan)
     executor.execute(graph_executor)
 
-    # draw graph
-    plt.figure(figsize=(10, 10))
-
-    labels = {}
-    for node in graph_executor.nodes(data=True):
-        labels[node[0]] = node[1]["node_name"]
-
-    pos = nx.nx_pydot.pydot_layout(graph_executor, prog="dot")
-    nx.draw(
-        graph_executor,
-        pos,
-        with_labels=True,
-        labels=labels,
-        node_size=2000,
-        node_color="skyblue",
-        font_size=20,
-    )
-    plt.show()
+    # TODO: Add visualization
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `up_esb-0.0.143/examples/partialorderplan.py` & `up_esb-0.0.145/examples/partialorderplan.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 #
 # Authors:
 # - Sebastian Stock, DFKI
 # - Selvakumar H S, LAAS-CNRS
 """Example for parallel execution of a partial order plan."""
 from pprint import pprint
 
-import matplotlib.pyplot as plt
-import networkx as nx
 import unified_planning as up
 from parallel import (
     Area,
     Location,
     Robot,
     info_sent_fun,
     is_surveyed_fun,
@@ -38,39 +36,36 @@
 
 # Define the problem. The domain is re-used from examples/parallel.py
 
 
 def define_problem():
     """Define the problem."""
     bridge = Bridge()
-    robot = Robot()
     bridge.create_types([Location, Area, Robot])
 
     robot_at = bridge.create_fluent_from_function(robot_at_fun)
     visited = bridge.create_fluent_from_function(visited_fun)
     is_surveyed = bridge.create_fluent_from_function(is_surveyed_fun)
     info_sent = bridge.create_fluent_from_function(info_sent_fun)
 
     # Instead of the example in paralle.py, we use instantanious actions
     move, [l_from, l_to] = bridge.create_action(
-        "Move", _callable=robot.move, l_from=Location, l_to=Location
+        "Move", _callable=Robot.move, l_from=Location, l_to=Location
     )
     move.add_precondition(info_sent(l_from))
     move.add_precondition(info_sent(l_to))
     move.add_precondition(robot_at(l_from))
     move.add_effect(robot_at(l_from), False)
     move.add_effect(robot_at(l_to), True)
     move.add_effect(visited(l_to), True)
 
-    survey, [a] = bridge.create_action(  # pylint: disable=unused-variable
-        "Survey", _callable=robot.survey, area=Area
-    )
+    survey, [_] = bridge.create_action("Survey", _callable=Robot.survey, area=Area)
     survey.add_effect(is_surveyed(), True)
 
-    send_info, [l] = bridge.create_action("SendInfo", _callable=robot.send_info, location=Location)
+    send_info, [l] = bridge.create_action("SendInfo", _callable=Robot.send_info, location=Location)
     # send_info.add_precondition(is_surveyed())
     send_info.add_effect(info_sent(l), True)
 
     l1 = bridge.create_object("l1", Location("l1"))
     l2 = bridge.create_object("l2", Location("l2"))
     l3 = bridge.create_object("l3", Location("l3"))
     l4 = bridge.create_object("l4", Location("l4"))
@@ -97,15 +92,15 @@
 
 
 def main():
     """Main function."""
     up.shortcuts.get_environment().credits_stream = None
     bridge, problem = define_problem()
 
-    plan = bridge.solve(problem)  # By default, choses a planner based on its problemkind
+    plan = bridge.solve(problem)  # By default, chooses a planner based on its problem.kind
     print("*" * 10)
     print("* Plan *")
     for action in plan.actions:
         print(action)
     print("*" * 10)
 
     if plan.kind == PlanKind.SEQUENTIAL_PLAN:
@@ -117,29 +112,12 @@
     else:
         raise ValueError("Plan is not a SequentialPlan")
 
     dependency_graph = bridge.get_executable_graph(plan)
     executor = Executor()
     executor.execute(dependency_graph)
 
-    # draw graph
-    plt.figure(figsize=(10, 10))
-
-    labels = {}
-    for node in dependency_graph.nodes(data=True):
-        labels[node[0]] = node[1]["node_name"]
-
-    pos = nx.nx_pydot.pydot_layout(dependency_graph, prog="dot")
-    nx.draw(
-        dependency_graph,
-        pos,
-        with_labels=True,
-        labels=labels,
-        node_size=2000,
-        node_color="skyblue",
-        font_size=20,
-    )
-    plt.show()
+    # TODO: Add visualization
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `up_esb-0.0.143/examples/sequential.py` & `up_esb-0.0.145/examples/sequential.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Example for sequential plan execution."""
-import matplotlib.pyplot as plt
-import networkx as nx
 import unified_planning as up
 
 from up_esb.bridge import Bridge
 from up_esb.plexmo import PlanDispatcher
 
 
 #################### 1. Define the domain ####################
@@ -35,58 +33,53 @@
 
 
 class Robot:
     """Robot class."""
 
     location = Location("l1")
 
-    def __init__(self):
-        self.l_from = ""
-        self.l_to = ""
-
-    def move(self, l_from: Location, l_to: Location):
+    @classmethod
+    def move(cls, l_from: Location, l_to: Location):
         """Move the robot from one location to another."""
 
-        self.l_from, self.l_to = l_from, l_to
-        print(f"Moving from {self.l_from} to {self.l_to}")
-        Robot.location = self.l_to
+        print(f"Moving from {l_from} to {l_to}")
+        Robot.location = l_to
 
         return True
 
 
 def robot_at_fun(l: Location):
     """Check if the robot is at a location."""
-    return Robot().location == l
+    return Robot.location == l
 
 
 def visited_fun(l: Location):
     """Check if the location is visited."""
-    return Robot().location == l
+    return Robot.location == l
 
 
 #################### 2. Define the problem ####################
 
 
 def define_problem():
     """Define the problem."""
     bridge = Bridge()
-    robot = Robot()
 
     bridge.create_types([Location, Robot])
 
     robot_at = bridge.create_fluent_from_function(robot_at_fun)
     visited = bridge.create_fluent_from_function(visited_fun)
 
     l1 = bridge.create_object("l1", Location("l1"))
     l2 = bridge.create_object("l2", Location("l2"))
     l3 = bridge.create_object("l3", Location("l3"))
     l4 = bridge.create_object("l4", Location("l4"))
 
     move, [l_from, l_to] = bridge.create_action(
-        "Move", _callable=robot.move, l_from=Location, l_to=Location
+        "Move", _callable=Robot.move, l_from=Location, l_to=Location
     )
     move.add_precondition(robot_at(l_from))
     move.add_effect(robot_at(l_from), False)
     move.add_effect(robot_at(l_to), True)
     move.add_effect(visited(l_to), True)
 
     problem = bridge.define_problem()
@@ -119,29 +112,12 @@
     for action in plan.actions:
         print(action)
     print("*" * 10)
 
     graph_executor = bridge.get_executable_graph(plan)
     dispatcher.execute_plan(graph_executor)
 
-    # draw graph
-    plt.figure(figsize=(10, 10))
-
-    labels = {}
-    for node in graph_executor.nodes(data=True):
-        labels[node[0]] = node[1]["node_name"]
-
-    pos = nx.nx_pydot.pydot_layout(graph_executor, prog="dot")
-    nx.draw(
-        graph_executor,
-        pos,
-        with_labels=True,
-        labels=labels,
-        node_size=2000,
-        node_color="skyblue",
-        font_size=20,
-    )
-    plt.show()
+    # TODO: Add visualization
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `up_esb-0.0.143/examples/time_triggered.py` & `up_esb-0.0.145/examples/time_triggered.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Example for time triggered plan execution."""
 
 import time
 
-import matplotlib.pyplot as plt
-import networkx as nx
 import unified_planning as up
 from unified_planning.model import EndTiming, StartTiming
 from unified_planning.shortcuts import ClosedTimeInterval, Not
 
 from up_esb.bridge import Bridge
 from up_esb.plexmo import PlanDispatcher
 
@@ -45,64 +43,65 @@
     def __repr__(self) -> str:
         return self.name
 
 
 class TemporalActions:
     """Class for temporal actions."""
 
-    m = None
-    f = None
+    match = None
+    fuse = None
 
-    def light_match(self, m: Match):
+    @classmethod
+    def light_match(cls, m: Match):
         """Light match action."""
-        TemporalActions.m = m
+        TemporalActions.match = m
 
         print(f"Lighting match {m}")
         time.sleep(5)
         return True
 
-    def mend_fuse(self, f: Fuse):
+    @classmethod
+    def mend_fuse(cls, f: Fuse):
         """Mend fuse action."""
-        TemporalActions.f = f
+        TemporalActions.fuse = f
 
         print(f"Mending fuse {f}")
         time.sleep(3)
         return True
 
 
 def handsfree_fun():
     """Check if hands are free."""
-    return TemporalActions().m is None and TemporalActions().f is None
+    return TemporalActions.match is None and TemporalActions.fuse is None
 
 
 def light_fun():
     """Check if lighted."""
-    return TemporalActions().m is not None
+    return TemporalActions.match is not None
 
 
-def match_used_fun(m: Match):  # pylint: disable=unused-argument
+def match_used_fun(m: Match):
     """Check if match is used."""
-    return TemporalActions().m == m
+    return TemporalActions.match == m
 
 
-def fuse_mended_fun(f: Fuse):  # pylint: disable=unused-argument
+def fuse_mended_fun(f: Fuse):
     """Fuse mended?"""
-    return TemporalActions().f == f
+    return TemporalActions.fuse == f
 
 
-def light_match_fun(m: Match):  # pylint: disable=unused-argument
+def light_match_fun(m: Match):
     """Light match?"""
-    return TemporalActions().m == m
+    return TemporalActions.match == m
 
 
 #################### 2. Define the problem ####################
 def define_problem():
     """Define the problem."""
     bridge = Bridge()
-    actions = TemporalActions()
 
     bridge.create_types([Match, Fuse])
 
     handsfree = bridge.create_fluent_from_function(handsfree_fun)
     light = bridge.create_fluent_from_function(light_fun)
     match_used = bridge.create_fluent_from_function(match_used_fun)
     fuse_mended = bridge.create_fluent_from_function(fuse_mended_fun)
@@ -111,23 +110,23 @@
     f2 = bridge.create_object("f2", Fuse("f2"))
     f3 = bridge.create_object("f3", Fuse("f3"))
     m1 = bridge.create_object("m1", Match("m1"))
     m2 = bridge.create_object("m2", Match("m2"))
     m3 = bridge.create_object("m3", Match("m3"))
 
     light_match, [m] = bridge.create_action(
-        "LightMatch", _callable=actions.light_match, m=Match, duration=5
+        "LightMatch", _callable=TemporalActions.light_match, m=Match, duration=5
     )
     light_match.add_condition(StartTiming(), Not(match_used(m)))
     light_match.add_effect(StartTiming(), match_used(m), True)
     light_match.add_effect(StartTiming(), light, True)
     light_match.add_effect(EndTiming(), light, False)
 
     mend_fuse, [f] = bridge.create_action(
-        "MendFuse", _callable=actions.mend_fuse, f=Fuse, duration=3
+        "MendFuse", _callable=TemporalActions.mend_fuse, f=Fuse, duration=3
     )
     mend_fuse.add_condition(StartTiming(), handsfree)
     mend_fuse.add_condition(ClosedTimeInterval(StartTiming(), EndTiming()), light)
     mend_fuse.add_effect(StartTiming(), handsfree, False)
     mend_fuse.add_effect(EndTiming(), fuse_mended(f), True)
     mend_fuse.add_effect(EndTiming(), handsfree, True)
 
@@ -161,29 +160,12 @@
     print("*" * 10)
 
     graph_executor = bridge.get_executable_graph(plan)
     dispatcher.execute_plan(
         graph_executor, dry_run=True
     )  # Dry run condition checks since temporal evaluation is not supported yet
 
-    # draw graph
-    plt.figure(figsize=(10, 10))
-
-    labels = {}
-    for node in graph_executor.nodes(data=True):
-        labels[node[0]] = node[1]["node_name"]
-
-    pos = nx.nx_pydot.pydot_layout(graph_executor, prog="dot")
-    nx.draw(
-        graph_executor,
-        pos,
-        with_labels=True,
-        labels=labels,
-        node_size=1000,
-        node_color="skyblue",
-        font_size=20,
-    )
-    plt.show()
+    # TODO: Add visualization
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `up_esb-0.0.143/pyproject.toml` & `up_esb-0.0.145/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 description = "General functionalities for using unified-planning in robotic applications"
 keywords = ["unified-planning", "embedded-systems-bridge"]
 license = {text = "Apache-2.0 License"}
 name = "up_esb"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.0.143"
+version = "0.0.145"
 
 [project.urls]
 Repository = "https://github.com/aiplan4eu/embedded-systems-bridge"
 Homepage = "https://www.aiplan4eu-project.eu/"
 
 [project.optional-dependencies]
 dev = ["black", "pylint", "pytest", "pre-commit"]
```

### Comparing `up_esb-0.0.143/tests/__init__.py` & `up_esb-0.0.145/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/tests/components/test_expression_manager.py` & `up_esb-0.0.145/tests/components/test_expression_manager.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/tests/test_bridge.py` & `up_esb-0.0.145/tests/test_bridge.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/tests/test_create_action.py` & `up_esb-0.0.145/tests/test_create_action.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/tests/test_dispatcher.py` & `up_esb-0.0.145/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/tests/test_graph.py` & `up_esb-0.0.145/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/tests/test_monitor.py` & `up_esb-0.0.145/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/__init__.py` & `up_esb-0.0.145/up_esb/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/bridge.py` & `up_esb-0.0.145/up_esb/bridge.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/components/__init__.py` & `up_esb-0.0.145/up_esb/components/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/components/actions.py` & `up_esb-0.0.145/up_esb/components/actions.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/components/expression_manager.py` & `up_esb-0.0.145/up_esb/components/expression_manager.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/components/graph.py` & `up_esb-0.0.145/up_esb/components/graph.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/executor.py` & `up_esb-0.0.145/up_esb/executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,23 +41,25 @@
 
                 # Fetch complete node data
                 for s in successors:
                     successors[successors.index(s)] = (s, graph.nodes[s])
                 self._execute_coroutines(successors)
             else:
                 parameters = node[1]["parameters"]
-                result = node[1]["executor"](*parameters)
+                executor = node[1]["context"][node[1]["action"]]
+                result = executor(**parameters)
 
         return result
 
     async def _execute_concurrent_action(self, action):
         # TODO: Better implementation
         # FIXME: Duplicate execution of actions
         parameters = action[1]["parameters"]
-        result = action[1]["executor"](*parameters)
+        executor = action[1]["context"][action[1]["action"]]
+        result = executor(**parameters)
 
         return result
 
     async def _run_concurrent_tasks(self, tasks):
         # TODO: add await on parallel actions
         await asyncio.gather(*tasks)
```

### Comparing `up_esb-0.0.143/up_esb/plexmo/__init__.py` & `up_esb-0.0.145/up_esb/plexmo/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/plexmo/dispatcher.py` & `up_esb-0.0.145/up_esb/plexmo/dispatcher.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb/plexmo/monitor.py` & `up_esb-0.0.145/up_esb/plexmo/monitor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.143/up_esb.egg-info/PKG-INFO` & `up_esb-0.0.145/up_esb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up-esb
-Version: 0.0.143
+Version: 0.0.145
 Summary: General functionalities for using unified-planning in robotic applications
 License: Apache-2.0 License
 Project-URL: Repository, https://github.com/aiplan4eu/embedded-systems-bridge
 Project-URL: Homepage, https://www.aiplan4eu-project.eu/
 Keywords: unified-planning,embedded-systems-bridge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `up_esb-0.0.143/up_esb.egg-info/SOURCES.txt` & `up_esb-0.0.145/up_esb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

