# Comparing `tmp/pytest-persistence-0.1.8.tar.gz` & `tmp/pytest-persistence-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-persistence-0.1.8.tar", last modified: Wed Jun 14 08:30:22 2023, max compression
+gzip compressed data, was "pytest-persistence-0.1.9.tar", last modified: Tue Jul  4 10:03:53 2023, max compression
```

## Comparing `pytest-persistence-0.1.8.tar` & `pytest-persistence-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-06-14 08:30:22.607442 pytest-persistence-0.1.8/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1077 2021-12-07 17:34:12.000000 pytest-persistence-0.1.8/LICENSE
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1033 2023-06-14 08:30:22.606442 pytest-persistence-0.1.8/PKG-INFO
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      570 2023-06-14 08:29:26.000000 pytest-persistence-0.1.8/README.md
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-06-14 08:30:22.605442 pytest-persistence-0.1.8/pytest_persistence/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1428 2023-03-28 16:41:44.000000 pytest-persistence-0.1.8/pytest_persistence/XDistScheduling.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       22 2023-06-14 08:29:52.000000 pytest-persistence-0.1.8/pytest_persistence/__init__.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     8275 2023-06-14 08:29:26.000000 pytest-persistence-0.1.8/pytest_persistence/plugin.py
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-06-14 08:30:22.606442 pytest-persistence-0.1.8/pytest_persistence.egg-info/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1033 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/PKG-INFO
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      396 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/SOURCES.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)        1 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/dependency_links.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       51 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/entry_points.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       19 2023-06-14 08:30:22.000000 pytest-persistence-0.1.8/pytest_persistence.egg-info/top_level.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       38 2023-06-14 08:30:22.607442 pytest-persistence-0.1.8/setup.cfg
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      969 2021-12-07 17:34:12.000000 pytest-persistence-0.1.8/setup.py
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-06-14 08:30:22.606442 pytest-persistence-0.1.8/tests/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      111 2023-05-16 08:13:42.000000 pytest-persistence-0.1.8/tests/test_mock.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1980 2022-06-27 12:07:26.000000 pytest-persistence-0.1.8/tests/test_plugin.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1367 2022-06-27 12:28:20.000000 pytest-persistence-0.1.8/tests/test_unit.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-07-04 10:03:53.720554 pytest-persistence-0.1.9/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1077 2021-12-07 17:34:12.000000 pytest-persistence-0.1.9/LICENSE
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1033 2023-07-04 10:03:53.720554 pytest-persistence-0.1.9/PKG-INFO
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      570 2023-06-14 08:29:26.000000 pytest-persistence-0.1.9/README.md
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-07-04 10:03:53.719554 pytest-persistence-0.1.9/pytest_persistence/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1428 2023-03-28 16:41:44.000000 pytest-persistence-0.1.9/pytest_persistence/XDistScheduling.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       22 2023-07-04 10:02:44.000000 pytest-persistence-0.1.9/pytest_persistence/__init__.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     8135 2023-07-04 10:02:39.000000 pytest-persistence-0.1.9/pytest_persistence/plugin.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-07-04 10:03:53.719554 pytest-persistence-0.1.9/pytest_persistence.egg-info/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1033 2023-07-04 10:03:53.000000 pytest-persistence-0.1.9/pytest_persistence.egg-info/PKG-INFO
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      396 2023-07-04 10:03:53.000000 pytest-persistence-0.1.9/pytest_persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)        1 2023-07-04 10:03:53.000000 pytest-persistence-0.1.9/pytest_persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       51 2023-07-04 10:03:53.000000 pytest-persistence-0.1.9/pytest_persistence.egg-info/entry_points.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       19 2023-07-04 10:03:53.000000 pytest-persistence-0.1.9/pytest_persistence.egg-info/top_level.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       38 2023-07-04 10:03:53.720554 pytest-persistence-0.1.9/setup.cfg
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      969 2021-12-07 17:34:12.000000 pytest-persistence-0.1.9/setup.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-07-04 10:03:53.720554 pytest-persistence-0.1.9/tests/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      111 2023-05-16 08:13:42.000000 pytest-persistence-0.1.9/tests/test_mock.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1980 2022-06-27 12:07:26.000000 pytest-persistence-0.1.9/tests/test_plugin.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1367 2022-06-27 12:28:20.000000 pytest-persistence-0.1.9/tests/test_unit.py
```

### Comparing `pytest-persistence-0.1.8/LICENSE` & `pytest-persistence-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.8/PKG-INFO` & `pytest-persistence-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-persistence
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pytest tool for persistent objects
 Home-page: https://github.com/JaurbanRH/pytest-persistence
 Author: Jakub Urban
 Author-email: kubo.urban@gmail.com
 Maintainer: Jakub Urban
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-persistence-0.1.8/README.md` & `pytest-persistence-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.8/pytest_persistence/XDistScheduling.py` & `pytest-persistence-0.1.9/pytest_persistence/XDistScheduling.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.8/pytest_persistence/plugin.py` & `pytest-persistence-0.1.9/pytest_persistence/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,20 +202,17 @@
                     continue
                 for cell in fin.__closure__:
                     if hasattr(cell.cell_contents, "cached_result"):
                         yield cell.cell_contents
 
         for k in list(stack.keys()):
             if k not in needed:
-                indexes = []
-                for i, v in enumerate(fixtures(stack[k][0])):
-                    v.cached_result = None
-                    indexes.append(i)
-                for i in sorted(indexes, reverse=True):
-                    del stack[k][0][i]
+                for i in fixtures(stack[k][0]):
+                    i.cached_result = None
+                stack[k][0].clear()
 
 
 def pytest_configure(config):
     """
     Hook ensures that plugin works only when the --load or --store option is present.
     """
     if config.getoption("--load") or config.getoption("--store"):
```

### Comparing `pytest-persistence-0.1.8/pytest_persistence.egg-info/PKG-INFO` & `pytest-persistence-0.1.9/pytest_persistence.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-persistence
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pytest tool for persistent objects
 Home-page: https://github.com/JaurbanRH/pytest-persistence
 Author: Jakub Urban
 Author-email: kubo.urban@gmail.com
 Maintainer: Jakub Urban
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-persistence-0.1.8/setup.py` & `pytest-persistence-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.8/tests/test_plugin.py` & `pytest-persistence-0.1.9/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.8/tests/test_unit.py` & `pytest-persistence-0.1.9/tests/test_unit.py`

 * *Files identical despite different names*

