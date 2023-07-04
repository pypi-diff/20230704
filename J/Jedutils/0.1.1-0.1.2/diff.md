# Comparing `tmp/Jedutils-0.1.1.tar.gz` & `tmp/Jedutils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jedutils-0.1.1.tar", last modified: Mon Jun 26 04:16:36 2023, max compression
+gzip compressed data, was "Jedutils-0.1.2.tar", last modified: Tue Jul  4 07:34:53 2023, max compression
```

## Comparing `Jedutils-0.1.1.tar` & `Jedutils-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:36.526326 Jedutils-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:36.522326 Jedutils-0.1.1/Jedutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-26 04:16:36.000000 Jedutils-0.1.1/Jedutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 04:16:36.000000 Jedutils-0.1.1/Jedutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:16:36.000000 Jedutils-0.1.1/Jedutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 04:16:36.000000 Jedutils-0.1.1/Jedutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 04:16:35.000000 Jedutils-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 04:16:35.000000 Jedutils-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-26 04:16:36.526326 Jedutils-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 04:16:35.000000 Jedutils-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:36.522326 Jedutils-0.1.1/jedutils/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 04:16:35.000000 Jedutils-0.1.1/jedutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:36.526326 Jedutils-0.1.1/jedutils/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 04:16:35.000000 Jedutils-0.1.1/jedutils/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-26 04:16:35.000000 Jedutils-0.1.1/jedutils/asyncio/_async_redis_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 04:16:35.000000 Jedutils-0.1.1/jedutils/asyncio/_run_async.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:16:36.526326 Jedutils-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-26 04:16:35.000000 Jedutils-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:34:53.504208 Jedutils-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:34:53.504208 Jedutils-0.1.2/Jedutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 07:34:53.000000 Jedutils-0.1.2/Jedutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 07:34:53.000000 Jedutils-0.1.2/Jedutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:34:53.000000 Jedutils-0.1.2/Jedutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 07:34:53.000000 Jedutils-0.1.2/Jedutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-04 07:34:52.000000 Jedutils-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-04 07:34:52.000000 Jedutils-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 07:34:53.504208 Jedutils-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-04 07:34:52.000000 Jedutils-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:34:53.504208 Jedutils-0.1.2/jedutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 07:34:52.000000 Jedutils-0.1.2/jedutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:34:53.504208 Jedutils-0.1.2/jedutils/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-04 07:34:52.000000 Jedutils-0.1.2/jedutils/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-04 07:34:52.000000 Jedutils-0.1.2/jedutils/asyncio/_async_redis_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-04 07:34:52.000000 Jedutils-0.1.2/jedutils/asyncio/_run_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:34:53.504208 Jedutils-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-04 07:34:52.000000 Jedutils-0.1.2/setup.py
```

### Comparing `Jedutils-0.1.1/Jedutils.egg-info/PKG-INFO` & `Jedutils-0.1.2/Jedutils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
```

### Comparing `Jedutils-0.1.1/LICENSE` & `Jedutils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.1/PKG-INFO` & `Jedutils-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
```

### Comparing `Jedutils-0.1.1/README.md` & `Jedutils-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.1/jedutils/asyncio/_async_redis_pipe.py` & `Jedutils-0.1.2/jedutils/asyncio/_async_redis_pipe.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.1/setup.py` & `Jedutils-0.1.2/setup.py`

 * *Files identical despite different names*

