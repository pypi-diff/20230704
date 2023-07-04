# Comparing `tmp/arpreq-0.3.3.tar.gz` & `tmp/arpreq-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arpreq-0.3.3.tar", last modified: Tue Jun  6 10:30:26 2017, max compression
+gzip compressed data, was "arpreq-0.3.4.tar", last modified: Tue Jul  4 16:02:36 2023, max compression
```

## Comparing `arpreq-0.3.3.tar` & `arpreq-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 shreyder  (1000) users      (100)        0 2017-06-06 10:30:26.000000 arpreq-0.3.3/
-drwxr-xr-x   0 shreyder  (1000) users      (100)        0 2017-06-06 10:30:26.000000 arpreq-0.3.3/src/
-drwxr-xr-x   0 shreyder  (1000) users      (100)        0 2017-06-06 10:30:26.000000 arpreq-0.3.3/src/arpreq.egg-info/
--rw-r--r--   0 shreyder  (1000) users      (100)     5291 2017-06-06 10:30:26.000000 arpreq-0.3.3/src/arpreq.egg-info/PKG-INFO
--rw-r--r--   0 shreyder  (1000) users      (100)      258 2017-06-06 10:30:26.000000 arpreq-0.3.3/src/arpreq.egg-info/SOURCES.txt
--rw-r--r--   0 shreyder  (1000) users      (100)        1 2017-06-06 10:30:26.000000 arpreq-0.3.3/src/arpreq.egg-info/dependency_links.txt
--rw-r--r--   0 shreyder  (1000) users      (100)        7 2017-06-06 10:30:26.000000 arpreq-0.3.3/src/arpreq.egg-info/top_level.txt
--rw-r--r--   0 shreyder  (1000) users      (100)    11460 2017-06-06 10:25:46.000000 arpreq-0.3.3/src/arpreq.c
-drwxr-xr-x   0 shreyder  (1000) users      (100)        0 2017-06-06 10:30:26.000000 arpreq-0.3.3/tests/
--rw-r--r--   0 shreyder  (1000) users      (100)        0 2016-06-09 15:42:58.000000 arpreq-0.3.3/tests/__init__.py
--rw-r--r--   0 shreyder  (1000) users      (100)     2086 2017-06-05 15:51:07.000000 arpreq-0.3.3/tests/test_arpreq.py
--rw-r--r--   0 shreyder  (1000) users      (100)     1086 2015-11-24 20:12:20.000000 arpreq-0.3.3/LICENSE
--rw-r--r--   0 shreyder  (1000) users      (100)       77 2016-06-26 19:34:00.000000 arpreq-0.3.3/MANIFEST.in
--rw-r--r--   0 shreyder  (1000) users      (100)     3223 2017-06-06 10:25:46.000000 arpreq-0.3.3/README.rst
--rw-r--r--   0 shreyder  (1000) users      (100)      100 2017-05-03 11:07:12.000000 arpreq-0.3.3/dev-requirements.txt
--rw-r--r--   0 shreyder  (1000) users      (100)       63 2017-06-06 10:30:26.000000 arpreq-0.3.3/setup.cfg
--rw-r--r--   0 shreyder  (1000) users      (100)     2403 2017-06-06 10:25:46.000000 arpreq-0.3.3/setup.py
--rw-r--r--   0 shreyder  (1000) users      (100)     5291 2017-06-06 10:30:26.000000 arpreq-0.3.3/PKG-INFO
+drwxr-xr-x   0 scs       (1000) scs       (1000)        0 2023-07-04 16:02:36.741229 arpreq-0.3.4/
+-rw-r--r--   0 scs       (1000) scs       (1000)     1086 2020-01-14 14:29:55.000000 arpreq-0.3.4/LICENSE
+-rw-r--r--   0 scs       (1000) scs       (1000)       77 2020-01-14 14:29:55.000000 arpreq-0.3.4/MANIFEST.in
+-rw-r--r--   0 scs       (1000) scs       (1000)     7274 2023-07-04 16:02:36.744563 arpreq-0.3.4/PKG-INFO
+-rw-r--r--   0 scs       (1000) scs       (1000)     5889 2022-04-09 19:57:02.000000 arpreq-0.3.4/README.rst
+-rw-r--r--   0 scs       (1000) scs       (1000)       74 2021-12-21 10:48:13.000000 arpreq-0.3.4/dev-requirements.txt
+-rw-r--r--   0 scs       (1000) scs       (1000)       63 2023-07-04 16:02:36.744563 arpreq-0.3.4/setup.cfg
+-rw-r--r--   0 scs       (1000) scs       (1000)     2297 2022-04-09 19:55:07.000000 arpreq-0.3.4/setup.py
+drwxr-xr-x   0 scs       (1000) scs       (1000)        0 2023-07-04 16:02:36.741229 arpreq-0.3.4/src/
+-rw-r--r--   0 scs       (1000) scs       (1000)    15006 2022-04-09 19:55:07.000000 arpreq-0.3.4/src/arpreq.c
+drwxr-xr-x   0 scs       (1000) scs       (1000)        0 2023-07-04 16:02:36.741229 arpreq-0.3.4/src/arpreq.egg-info/
+-rw-r--r--   0 scs       (1000) scs       (1000)     7274 2023-07-04 16:02:36.000000 arpreq-0.3.4/src/arpreq.egg-info/PKG-INFO
+-rw-r--r--   0 scs       (1000) scs       (1000)      258 2023-07-04 16:02:36.000000 arpreq-0.3.4/src/arpreq.egg-info/SOURCES.txt
+-rw-r--r--   0 scs       (1000) scs       (1000)        1 2023-07-04 16:02:36.000000 arpreq-0.3.4/src/arpreq.egg-info/dependency_links.txt
+-rw-r--r--   0 scs       (1000) scs       (1000)        7 2023-07-04 16:02:36.000000 arpreq-0.3.4/src/arpreq.egg-info/top_level.txt
+drwxr-xr-x   0 scs       (1000) scs       (1000)        0 2023-07-04 16:02:36.741229 arpreq-0.3.4/tests/
+-rw-r--r--   0 scs       (1000) scs       (1000)        0 2020-01-14 14:29:55.000000 arpreq-0.3.4/tests/__init__.py
+-rw-r--r--   0 scs       (1000) scs       (1000)     5204 2022-04-09 19:55:07.000000 arpreq-0.3.4/tests/test_arpreq.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `arpreq-0.3.3/LICENSE` & `arpreq-0.3.4/LICENSE`

 * *Files identical despite different names*

