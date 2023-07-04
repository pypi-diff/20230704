# Comparing `tmp/ailola-0.9.8.tar.gz` & `tmp/ailola-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailola-0.9.8.tar", last modified: Mon Jul  3 11:56:05 2023, max compression
+gzip compressed data, was "ailola-0.9.9.tar", last modified: Mon Jul  3 11:56:42 2023, max compression
```

## Comparing `ailola-0.9.8.tar` & `ailola-0.9.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:56:05.488985 ailola-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 11:56:05.488985 ailola-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-03 11:55:53.000000 ailola-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:56:05.484985 ailola-0.9.8/ailola/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:56:05.488985 ailola-0.9.8/ailola/ailola.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 11:56:05.000000 ailola-0.9.8/ailola/ailola.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 11:56:05.000000 ailola-0.9.8/ailola/ailola.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:56:05.000000 ailola-0.9.8/ailola/ailola.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:56:05.000000 ailola-0.9.8/ailola/ailola.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 11:56:05.000000 ailola-0.9.8/ailola/ailola.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 11:56:05.000000 ailola-0.9.8/ailola/ailola.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-03 11:55:53.000000 ailola-0.9.8/ailola/ailola.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 11:56:05.488985 ailola-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-03 11:55:53.000000 ailola-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:56:42.012022 ailola-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 11:56:42.012022 ailola-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-03 11:56:32.000000 ailola-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:56:42.012022 ailola-0.9.9/ailola/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:56:42.012022 ailola-0.9.9/ailola/ailola.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 11:56:41.000000 ailola-0.9.9/ailola/ailola.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 11:56:41.000000 ailola-0.9.9/ailola/ailola.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:56:41.000000 ailola-0.9.9/ailola/ailola.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:56:41.000000 ailola-0.9.9/ailola/ailola.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 11:56:41.000000 ailola-0.9.9/ailola/ailola.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 11:56:41.000000 ailola-0.9.9/ailola/ailola.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-03 11:56:32.000000 ailola-0.9.9/ailola/ailola.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 11:56:42.016022 ailola-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-03 11:56:32.000000 ailola-0.9.9/setup.py
```

### Comparing `ailola-0.9.8/README.md` & `ailola-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ailola-0.9.8/ailola/ailola.py` & `ailola-0.9.9/ailola/ailola.py`

 * *Files identical despite different names*

### Comparing `ailola-0.9.8/setup.py` & `ailola-0.9.9/setup.py`

 * *Files identical despite different names*

