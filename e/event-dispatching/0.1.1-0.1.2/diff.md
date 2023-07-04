# Comparing `tmp/event_dispatching-0.1.1.tar.gz` & `tmp/event_dispatching-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_dispatching-0.1.1.tar", max compression
+gzip compressed data, was "event_dispatching-0.1.2.tar", max compression
```

## Comparing `event_dispatching-0.1.1.tar` & `event_dispatching-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-04 03:29:41.012953 event_dispatching-0.1.1/LICENSE
--rw-r--r--   0        0        0     1528 2023-07-04 05:31:13.781657 event_dispatching-0.1.1/README.md
--rw-r--r--   0        0        0      238 2023-07-04 04:50:41.069619 event_dispatching-0.1.1/event_dispatcher/__init__.py
--rw-r--r--   0        0        0     1876 2023-07-04 04:49:27.706489 event_dispatching-0.1.1/event_dispatcher/_dispatcher.py
--rw-r--r--   0        0        0      922 2023-07-04 04:49:27.706489 event_dispatching-0.1.1/event_dispatcher/async_dispatcher.py
--rw-r--r--   0        0        0      786 2023-07-04 04:49:27.706489 event_dispatching-0.1.1/event_dispatcher/sync_dispatcher.py
--rw-r--r--   0        0        0      203 2023-07-04 03:02:26.831669 event_dispatching-0.1.1/event_dispatcher/types.py
--rw-r--r--   0        0        0     1252 2023-07-04 05:35:33.682403 event_dispatching-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2114 1970-01-01 00:00:00.000000 event_dispatching-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1528 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/README.md
+-rw-r--r--   0        0        0      238 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/__init__.py
+-rw-r--r--   0        0        0     1876 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/_dispatcher.py
+-rw-r--r--   0        0        0      922 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/async_dispatcher.py
+-rw-r--r--   0        0        0      786 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/sync_dispatcher.py
+-rw-r--r--   0        0        0      237 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/event_dispatcher/types.py
+-rw-r--r--   0        0        0     1252 2023-07-04 05:54:22.121150 event_dispatching-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2114 1970-01-01 00:00:00.000000 event_dispatching-0.1.2/PKG-INFO
```

### Comparing `event_dispatching-0.1.1/LICENSE` & `event_dispatching-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.1/README.md` & `event_dispatching-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.1/event_dispatcher/_dispatcher.py` & `event_dispatching-0.1.2/event_dispatcher/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.1/event_dispatcher/async_dispatcher.py` & `event_dispatching-0.1.2/event_dispatcher/async_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.1/event_dispatcher/sync_dispatcher.py` & `event_dispatching-0.1.2/event_dispatcher/sync_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.1/pyproject.toml` & `event_dispatching-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-dispatching"
-version = "0.1.1"
+version = "0.1.2"
 description = "Pure python implementation of event dispatcher"
 authors = ["Ruslan Saiko <ruslan.saiko.dev@gmail.com>"]
 repository = "https://github.com/trabem/event-dispatcher"
 readme = "README.md"
 packages = [{ include = "event_dispatcher" }]
 license = "MIT"
```

### Comparing `event_dispatching-0.1.1/PKG-INFO` & `event_dispatching-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-dispatching
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pure python implementation of event dispatcher
 Home-page: https://github.com/trabem/event-dispatcher
 License: MIT
 Author: Ruslan Saiko
 Author-email: ruslan.saiko.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

