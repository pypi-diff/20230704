# Comparing `tmp/threed_optix-1.0.7.tar.gz` & `tmp/threed_optix-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-1.0.7.tar", last modified: Tue Jul  4 17:24:28 2023, max compression
+gzip compressed data, was "threed_optix-1.0.8.tar", last modified: Tue Jul  4 17:26:58 2023, max compression
```

## Comparing `threed_optix-1.0.7.tar` & `threed_optix-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:24:28.725541 threed_optix-1.0.7/
--rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-29 16:13:48.000000 threed_optix-1.0.7/LICENSE.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)      206 2023-07-04 17:24:28.725541 threed_optix-1.0.7/PKG-INFO
--rw-rw-r--   0 elika     (1000) elika     (1000)      731 2023-07-04 17:18:02.000000 threed_optix-1.0.7/README.md
--rw-rw-r--   0 elika     (1000) elika     (1000)      107 2023-07-04 17:24:28.725541 threed_optix-1.0.7/setup.cfg
--rw-rw-r--   0 elika     (1000) elika     (1000)      433 2023-07-04 17:24:18.000000 threed_optix-1.0.7/setup.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:24:28.725541 threed_optix-1.0.7/src/
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:24:28.725541 threed_optix-1.0.7/src/threed_optix/
--rw-rw-r--   0 elika     (1000) elika     (1000)       22 2023-06-26 17:19:19.000000 threed_optix-1.0.7/src/threed_optix/__init__.py
--rw-rw-r--   0 elika     (1000) elika     (1000)     5757 2023-07-01 14:22:21.000000 threed_optix-1.0.7/src/threed_optix/api.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:24:28.725541 threed_optix-1.0.7/src/threed_optix/examples/
--rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-24 18:01:59.000000 threed_optix-1.0.7/src/threed_optix/examples/__init__.py
--rw-rw-r--   0 elika     (1000) elika     (1000)     2152 2023-07-01 14:44:27.000000 threed_optix-1.0.7/src/threed_optix/examples/example_0.py
--rwxrwxr-x   0 elika     (1000) elika     (1000)     2374 2023-07-01 11:27:04.000000 threed_optix-1.0.7/src/threed_optix/examples/simple.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:24:28.725541 threed_optix-1.0.7/src/threed_optix.egg-info/
--rw-rw-r--   0 elika     (1000) elika     (1000)      206 2023-07-04 17:24:28.000000 threed_optix-1.0.7/src/threed_optix.egg-info/PKG-INFO
--rw-rw-r--   0 elika     (1000) elika     (1000)      405 2023-07-04 17:24:28.000000 threed_optix-1.0.7/src/threed_optix.egg-info/SOURCES.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)        1 2023-07-04 17:24:28.000000 threed_optix-1.0.7/src/threed_optix.egg-info/dependency_links.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)       27 2023-07-04 17:24:28.000000 threed_optix-1.0.7/src/threed_optix.egg-info/requires.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)       13 2023-07-04 17:24:28.000000 threed_optix-1.0.7/src/threed_optix.egg-info/top_level.txt
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:26:58.887298 threed_optix-1.0.8/
+-rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-29 16:13:48.000000 threed_optix-1.0.8/LICENSE.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)      938 2023-07-04 17:26:58.887298 threed_optix-1.0.8/PKG-INFO
+-rw-rw-r--   0 elika     (1000) elika     (1000)      731 2023-07-04 17:18:02.000000 threed_optix-1.0.8/README.md
+-rw-rw-r--   0 elika     (1000) elika     (1000)      107 2023-07-04 17:26:58.887298 threed_optix-1.0.8/setup.cfg
+-rw-rw-r--   0 elika     (1000) elika     (1000)      535 2023-07-04 17:26:52.000000 threed_optix-1.0.8/setup.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:26:58.883298 threed_optix-1.0.8/src/
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:26:58.883298 threed_optix-1.0.8/src/threed_optix/
+-rw-rw-r--   0 elika     (1000) elika     (1000)       22 2023-06-26 17:19:19.000000 threed_optix-1.0.8/src/threed_optix/__init__.py
+-rw-rw-r--   0 elika     (1000) elika     (1000)     5757 2023-07-01 14:22:21.000000 threed_optix-1.0.8/src/threed_optix/api.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:26:58.887298 threed_optix-1.0.8/src/threed_optix/examples/
+-rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-24 18:01:59.000000 threed_optix-1.0.8/src/threed_optix/examples/__init__.py
+-rw-rw-r--   0 elika     (1000) elika     (1000)     2152 2023-07-01 14:44:27.000000 threed_optix-1.0.8/src/threed_optix/examples/example_0.py
+-rwxrwxr-x   0 elika     (1000) elika     (1000)     2374 2023-07-01 11:27:04.000000 threed_optix-1.0.8/src/threed_optix/examples/simple.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-04 17:26:58.887298 threed_optix-1.0.8/src/threed_optix.egg-info/
+-rw-rw-r--   0 elika     (1000) elika     (1000)      938 2023-07-04 17:26:58.000000 threed_optix-1.0.8/src/threed_optix.egg-info/PKG-INFO
+-rw-rw-r--   0 elika     (1000) elika     (1000)      405 2023-07-04 17:26:58.000000 threed_optix-1.0.8/src/threed_optix.egg-info/SOURCES.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)        1 2023-07-04 17:26:58.000000 threed_optix-1.0.8/src/threed_optix.egg-info/dependency_links.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)       27 2023-07-04 17:26:58.000000 threed_optix-1.0.8/src/threed_optix.egg-info/requires.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)       13 2023-07-04 17:26:58.000000 threed_optix-1.0.8/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-1.0.7/README.md` & `threed_optix-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `threed_optix-1.0.7/src/threed_optix/api.py` & `threed_optix-1.0.8/src/threed_optix/api.py`

 * *Files identical despite different names*

### Comparing `threed_optix-1.0.7/src/threed_optix/examples/example_0.py` & `threed_optix-1.0.8/src/threed_optix/examples/example_0.py`

 * *Files identical despite different names*

### Comparing `threed_optix-1.0.7/src/threed_optix/examples/simple.py` & `threed_optix-1.0.8/src/threed_optix/examples/simple.py`

 * *Files identical despite different names*

