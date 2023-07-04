# Comparing `tmp/xanadu-cloud-client-0.3.0.tar.gz` & `tmp/xanadu-cloud-client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/xanadu-cloud-client/xanadu-cloud-client/dist/tmpk3r0l_6k/xanadu-cloud-client-0.3.0.tar", last modified: Tue Dec  6 21:28:19 2022, max compression
+gzip compressed data, was "/home/runner/work/xanadu-cloud-client/xanadu-cloud-client/dist/tmpk39rvdp1/xanadu-cloud-client-0.3.1.tar", last modified: Tue Jul  4 19:31:45 2023, max compression
```

## Comparing `xanadu-cloud-client-0.3.0.tar` & `xanadu-cloud-client-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/xanadu_cloud_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/xanadu_cloud_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/xanadu_cloud_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/xanadu_cloud_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/xanadu_cloud_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/xanadu_cloud_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/xanadu_cloud_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 21:28:19.000000 xanadu-cloud-client-0.3.0/xcc/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/xcc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/xcc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/xcc/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13615 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/xcc/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/xcc/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13399 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/xcc/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/xcc/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2022-12-06 21:27:57.000000 xanadu-cloud-client-0.3.0/xcc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15980 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/xanadu_cloud_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/xanadu_cloud_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/xanadu_cloud_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/xanadu_cloud_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/xanadu_cloud_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/xanadu_cloud_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/xanadu_cloud_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:45.000000 xanadu-cloud-client-0.3.1/xcc/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/xcc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/xcc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/xcc/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-07-04 19:31:26.000000 xanadu-cloud-client-0.3.1/xcc/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-07-04 19:31:27.000000 xanadu-cloud-client-0.3.1/xcc/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-07-04 19:31:27.000000 xanadu-cloud-client-0.3.1/xcc/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-04 19:31:27.000000 xanadu-cloud-client-0.3.1/xcc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-04 19:31:27.000000 xanadu-cloud-client-0.3.1/xcc/util.py
```

### Comparing `xanadu-cloud-client-0.3.0/LICENSE` & `xanadu-cloud-client-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xanadu-cloud-client-0.3.0/PKG-INFO` & `xanadu-cloud-client-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xanadu-cloud-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: XCC is a Python API and CLI for the Xanadu Cloud.
 Home-page: https://github.com/XanaduAI/xanadu-cloud-client
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Description: .. image:: https://raw.githubusercontent.com/XanaduAI/xanadu-cloud-client/main/docs/_static/xcc_title.svg
             :alt: XCC
```

### Comparing `xanadu-cloud-client-0.3.0/README.rst` & `xanadu-cloud-client-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `xanadu-cloud-client-0.3.0/setup.py` & `xanadu-cloud-client-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("xcc/_version.py") as f:
     version = f.readlines()[-1].split()[-1].strip("\"'")
 
 requirements = [
     "appdirs",
     "fire",
     "numpy",
-    "pydantic[dotenv]",
+    "pydantic[dotenv]<2",
     "python-dateutil",
     "requests",
 ]
 
 info = {
     "description": "XCC is a Python API and CLI for the Xanadu Cloud.",
     "entry_points": {"console_scripts": ["xcc=xcc.commands:main"]},
```

### Comparing `xanadu-cloud-client-0.3.0/xanadu_cloud_client.egg-info/PKG-INFO` & `xanadu-cloud-client-0.3.1/xanadu_cloud_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xanadu-cloud-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: XCC is a Python API and CLI for the Xanadu Cloud.
 Home-page: https://github.com/XanaduAI/xanadu-cloud-client
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Description: .. image:: https://raw.githubusercontent.com/XanaduAI/xanadu-cloud-client/main/docs/_static/xcc_title.svg
             :alt: XCC
```

### Comparing `xanadu-cloud-client-0.3.0/xcc/__init__.py` & `xanadu-cloud-client-0.3.1/xcc/__init__.py`

 * *Files identical despite different names*

### Comparing `xanadu-cloud-client-0.3.0/xcc/commands.py` & `xanadu-cloud-client-0.3.1/xcc/commands.py`

 * *Files identical despite different names*

### Comparing `xanadu-cloud-client-0.3.0/xcc/connection.py` & `xanadu-cloud-client-0.3.1/xcc/connection.py`

 * *Files identical despite different names*

### Comparing `xanadu-cloud-client-0.3.0/xcc/device.py` & `xanadu-cloud-client-0.3.1/xcc/device.py`

 * *Files identical despite different names*

### Comparing `xanadu-cloud-client-0.3.0/xcc/job.py` & `xanadu-cloud-client-0.3.1/xcc/job.py`

 * *Files identical despite different names*

### Comparing `xanadu-cloud-client-0.3.0/xcc/settings.py` & `xanadu-cloud-client-0.3.1/xcc/settings.py`

 * *Files identical despite different names*

### Comparing `xanadu-cloud-client-0.3.0/xcc/util.py` & `xanadu-cloud-client-0.3.1/xcc/util.py`

 * *Files identical despite different names*

