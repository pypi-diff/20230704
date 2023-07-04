# Comparing `tmp/event_dispatching-0.1.2.tar.gz` & `tmp/event_dispatching-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_dispatching-0.1.2.tar", max compression
+gzip compressed data, was "event_dispatching-0.1.3.tar", max compression
```

## Comparing `event_dispatching-0.1.2.tar` & `event_dispatching-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/LICENSE
--rw-r--r--   0        0        0     1528 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/README.md
--rw-r--r--   0        0        0      238 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/__init__.py
--rw-r--r--   0        0        0     1876 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/_dispatcher.py
--rw-r--r--   0        0        0      922 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/async_dispatcher.py
--rw-r--r--   0        0        0      786 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/sync_dispatcher.py
--rw-r--r--   0        0        0      237 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/types.py
--rw-r--r--   0        0        0     1252 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2114 1970-01-01 00:00:00.000000 event_dispatching-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1627 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/README.md
+-rw-r--r--   0        0        0      238 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/__init__.py
+-rw-r--r--   0        0        0     1876 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/_dispatcher.py
+-rw-r--r--   0        0        0      922 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/async_dispatcher.py
+-rw-r--r--   0        0        0      786 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/sync_dispatcher.py
+-rw-r--r--   0        0        0      237 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/event_dispatcher/types.py
+-rw-r--r--   0        0        0     1718 2023-07-04 06:20:42.250633 event_dispatching-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 event_dispatching-0.1.3/PKG-INFO
```

### Comparing `event_dispatching-0.1.2/LICENSE` & `event_dispatching-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.2/README.md` & `event_dispatching-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,23 @@
 - Simple API: Easy to understand and use.
 - Lightweight: Minimal impact on your application's performance.
 - Flexible: Can be used in any Python application.
 - Asyncio Support: Compatible with Python's built-in asyncio library.
 
 ## Installation
 
-You can install the Event Dispatcher using pip:
+You can install the Event Dispatcher using [pip](https://pypi.org/project/event-dispatching/):
 
 ```bash
 pip install event-dispatching
 ```
+or using poetry
+```bash
+poetry add event-dispatching
+```
 
 ## Usage
 
 Here is a basic example of how to use the Event Dispatcher:
 
 ```python
 import event_dispatcher
@@ -40,15 +44,15 @@
 ```
 
 When you run this code, it will print:
 
 ```
 Event received: Hello, World!
 ```
-For more examples, please see [examples](https://github.com/trabem/event-dispatcher/tree/main/examples)
+More usage examples provided [here](https://github.com/trabem/event-dispatcher/tree/main/examples)
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `event_dispatching-0.1.2/event_dispatcher/_dispatcher.py` & `event_dispatching-0.1.3/event_dispatcher/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.2/event_dispatcher/async_dispatcher.py` & `event_dispatching-0.1.3/event_dispatcher/async_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.2/event_dispatcher/sync_dispatcher.py` & `event_dispatching-0.1.3/event_dispatcher/sync_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.2/pyproject.toml` & `event_dispatching-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,35 @@
 [tool.poetry]
 name = "event-dispatching"
-version = "0.1.2"
+version = "0.1.3"
 description = "Pure python implementation of event dispatcher"
 authors = ["Ruslan Saiko <ruslan.saiko.dev@gmail.com>"]
 repository = "https://github.com/trabem/event-dispatcher"
 readme = "README.md"
 packages = [{ include = "event_dispatcher" }]
 license = "MIT"
+classifiers = [
+    "Topic :: Software Development",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3"
+]
+keywords = [
+    "event-dispatcher",
+    "event-dispatching",
+    "events",
+    "event handling",
+    "python",
+    "asynchronous",
+    "event-driven",
+    "event management"
+]
+
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
```

### Comparing `event_dispatching-0.1.2/PKG-INFO` & `event_dispatching-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: event-dispatching
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pure python implementation of event dispatcher
 Home-page: https://github.com/trabem/event-dispatcher
 License: MIT
+Keywords: event-dispatcher,event-dispatching,events,event handling,python,asynchronous,event-driven,event management
 Author: Ruslan Saiko
 Author-email: ruslan.saiko.dev@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/trabem/event-dispatcher
 Description-Content-Type: text/markdown
 
 # Event Dispatcher
 
 This repository contains a pure Python implementation of an event dispatcher. The event dispatcher allows you to create a simple event-driven architecture in your Python applications. It allows you to decouple your application components, making your code cleaner and easier to maintain.
 
@@ -24,19 +29,23 @@
 - Simple API: Easy to understand and use.
 - Lightweight: Minimal impact on your application's performance.
 - Flexible: Can be used in any Python application.
 - Asyncio Support: Compatible with Python's built-in asyncio library.
 
 ## Installation
 
-You can install the Event Dispatcher using pip:
+You can install the Event Dispatcher using [pip](https://pypi.org/project/event-dispatching/):
 
 ```bash
 pip install event-dispatching
 ```
+or using poetry
+```bash
+poetry add event-dispatching
+```
 
 ## Usage
 
 Here is a basic example of how to use the Event Dispatcher:
 
 ```python
 import event_dispatcher
@@ -56,15 +65,15 @@
 ```
 
 When you run this code, it will print:
 
 ```
 Event received: Hello, World!
 ```
-For more examples, please see [examples](https://github.com/trabem/event-dispatcher/tree/main/examples)
+More usage examples provided [here](https://github.com/trabem/event-dispatcher/tree/main/examples)
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
```

