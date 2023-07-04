# Comparing `tmp/funix-0.4.3.tar.gz` & `tmp/funix-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funix-0.4.3.tar", last modified: Mon Jul  3 05:40:36 2023, max compression
+gzip compressed data, was "funix-0.4.4.tar", last modified: Tue Jul  4 15:06:11 2023, max compression
```

## Comparing `funix-0.4.3.tar` & `funix-0.4.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.216102 funix-0.4.3/
--rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.4.3/LICENSE
--rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.4.3/MANIFEST.in
--rw-r--r--   0 yazawazi   (501) staff       (20)     8629 2023-07-03 05:40:36.216215 funix-0.4.3/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)     6748 2023-05-08 21:04:14.000000 funix-0.4.3/README.md
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.195273 funix-0.4.3/backend/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.197441 funix-0.4.3/backend/funix/
--rw-r--r--   0 yazawazi   (501) staff       (20)    12587 2023-07-03 05:14:28.000000 funix-0.4.3/backend/funix/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4171 2023-05-23 06:01:29.000000 funix-0.4.3/backend/funix/__main__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.198693 funix-0.4.3/backend/funix/app/
--rw-r--r--   0 yazawazi   (501) staff       (20)      178 2023-05-26 11:05:26.000000 funix-0.4.3/backend/funix/app/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.200505 funix-0.4.3/backend/funix/build/
--rw-r--r--   0 yazawazi   (501) staff       (20)      240 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/asset-manifest.json
--rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2023-05-27 08:54:36.000000 funix-0.4.3/backend/funix/build/favicon.ico
--rw-r--r--   0 yazawazi   (501) staff       (20)      806 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/index.html
--rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2023-05-27 08:54:36.000000 funix-0.4.3/backend/funix/build/logo192.png
--rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2023-05-27 08:54:36.000000 funix-0.4.3/backend/funix/build/logo512.png
--rw-r--r--   0 yazawazi   (501) staff       (20)      492 2023-05-27 08:54:36.000000 funix-0.4.3/backend/funix/build/manifest.json
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.195598 funix-0.4.3/backend/funix/build/static/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.200743 funix-0.4.3/backend/funix/build/static/css/
--rw-r--r--   0 yazawazi   (501) staff       (20)     9350 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/static/css/main.521e60ca.css
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.205871 funix-0.4.3/backend/funix/build/static/js/
--rw-r--r--   0 yazawazi   (501) staff       (20)  6555220 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/static/js/main.ef806516.js
--rw-r--r--   0 yazawazi   (501) staff       (20)     4231 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.206185 funix-0.4.3/backend/funix/config/
--rw-r--r--   0 yazawazi   (501) staff       (20)      928 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/config/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.212606 funix-0.4.3/backend/funix/decorator/
--rw-r--r--   0 yazawazi   (501) staff       (20)    53592 2023-06-01 23:35:40.000000 funix-0.4.3/backend/funix/decorator/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3113 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/decorator/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    10936 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/decorator/magic.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.212861 funix-0.4.3/backend/funix/frontend/
--rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-05-23 09:37:53.000000 funix-0.4.3/backend/funix/frontend/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.213396 funix-0.4.3/backend/funix/hint/
--rw-r--r--   0 yazawazi   (501) staff       (20)    10668 2023-06-01 23:31:16.000000 funix-0.4.3/backend/funix/hint/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3823 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/hint/layout.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.213759 funix-0.4.3/backend/funix/prep/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.4.3/backend/funix/prep/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     7547 2023-05-26 10:41:26.000000 funix-0.4.3/backend/funix/prep/global_to_session.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.214094 funix-0.4.3/backend/funix/session/
--rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2023-05-26 11:04:02.000000 funix-0.4.3/backend/funix/session/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.214427 funix-0.4.3/backend/funix/test/
--rw-r--r--   0 yazawazi   (501) staff       (20)     5327 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/test/test_magic.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.214714 funix-0.4.3/backend/funix/theme/
--rw-r--r--   0 yazawazi   (501) staff       (20)    10204 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/theme/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.215675 funix-0.4.3/backend/funix/util/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      456 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      771 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/module.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4268 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/network.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      467 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/uri.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.215939 funix-0.4.3/backend/funix/widget/
--rw-r--r--   0 yazawazi   (501) staff       (20)     4602 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/widget/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4689 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/widget/builtin.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.198581 funix-0.4.3/backend/funix.egg-info/
--rw-r--r--   0 yazawazi   (501) staff       (20)     8629 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)     1323 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/SOURCES.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        1 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/dependency_links.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)       50 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/entry_points.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)      143 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/requires.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        6 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/top_level.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)      938 2023-07-03 05:32:42.000000 funix-0.4.3/pyproject.toml
--rw-r--r--   0 yazawazi   (501) staff       (20)      114 2023-07-03 05:40:36.216547 funix-0.4.3/setup.cfg
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.905564 funix-0.4.4/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.4.4/LICENSE
+-rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.4.4/MANIFEST.in
+-rw-r--r--   0 yazawazi   (501) staff       (20)     8669 2023-07-04 15:06:11.905652 funix-0.4.4/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)     6748 2023-05-08 21:04:14.000000 funix-0.4.4/README.md
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.886555 funix-0.4.4/backend/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.888396 funix-0.4.4/backend/funix/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    12895 2023-07-04 15:03:42.000000 funix-0.4.4/backend/funix/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4171 2023-05-23 06:01:29.000000 funix-0.4.4/backend/funix/__main__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.890925 funix-0.4.4/backend/funix/app/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      178 2023-05-26 11:05:26.000000 funix-0.4.4/backend/funix/app/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.892492 funix-0.4.4/backend/funix/build/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      240 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/asset-manifest.json
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2023-05-27 08:54:36.000000 funix-0.4.4/backend/funix/build/favicon.ico
+-rw-r--r--   0 yazawazi   (501) staff       (20)      806 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/index.html
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2023-05-27 08:54:36.000000 funix-0.4.4/backend/funix/build/logo192.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2023-05-27 08:54:36.000000 funix-0.4.4/backend/funix/build/logo512.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)      492 2023-05-27 08:54:36.000000 funix-0.4.4/backend/funix/build/manifest.json
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.886823 funix-0.4.4/backend/funix/build/static/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.892919 funix-0.4.4/backend/funix/build/static/css/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9350 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/static/css/main.521e60ca.css
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.897476 funix-0.4.4/backend/funix/build/static/js/
+-rw-r--r--   0 yazawazi   (501) staff       (20)  6555220 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/static/js/main.ef806516.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4231 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.897830 funix-0.4.4/backend/funix/config/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      928 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/config/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.901346 funix-0.4.4/backend/funix/decorator/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    53592 2023-06-01 23:35:40.000000 funix-0.4.4/backend/funix/decorator/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3113 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/decorator/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10936 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/decorator/magic.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.901474 funix-0.4.4/backend/funix/frontend/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-05-23 09:37:53.000000 funix-0.4.4/backend/funix/frontend/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.901706 funix-0.4.4/backend/funix/hint/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10668 2023-06-01 23:31:16.000000 funix-0.4.4/backend/funix/hint/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3823 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/hint/layout.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.901891 funix-0.4.4/backend/funix/prep/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.4.4/backend/funix/prep/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     7547 2023-05-26 10:41:26.000000 funix-0.4.4/backend/funix/prep/global_to_session.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.902197 funix-0.4.4/backend/funix/session/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2023-05-26 11:04:02.000000 funix-0.4.4/backend/funix/session/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.903884 funix-0.4.4/backend/funix/test/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5327 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/test/test_magic.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.904178 funix-0.4.4/backend/funix/theme/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10204 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/theme/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.905019 funix-0.4.4/backend/funix/util/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      456 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      771 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/module.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4268 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/network.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      467 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/uri.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.905303 funix-0.4.4/backend/funix/widget/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4602 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/widget/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4689 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/widget/builtin.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.890812 funix-0.4.4/backend/funix.egg-info/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     8669 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1323 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/SOURCES.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        1 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/dependency_links.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)       50 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/entry_points.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)      206 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/requires.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        6 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/top_level.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1021 2023-07-04 15:01:30.000000 funix-0.4.4/pyproject.toml
+-rw-r--r--   0 yazawazi   (501) staff       (20)      114 2023-07-04 15:06:11.905937 funix-0.4.4/setup.cfg
```

### Comparing `funix-0.4.3/LICENSE` & `funix-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/PKG-INFO` & `funix-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.4.3
+Version: 0.4.4
 Summary: Building web apps without manually creating widgets
 Author-email: "Textea Inc." <bao@textea.co>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Flask
 Classifier: Framework :: Matplotlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: plot
+Provides-Extra: git
+Provides-Extra: all
 License-File: LICENSE
 
 <h1 align="center">
     <b>
         Funix.IO<br>
     </b>
     ⭐️  The laziest way to build AI/data apps in Python.  ⭐️ <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funix Version: 0.4.3 Summary: Building web apps
+Metadata-Version: 2.1 Name: funix Version: 0.4.4 Summary: Building web apps
 without manually creating widgets Author-email: "Textea Inc."
 textea.co> License: MIT License Copyright (c) 2022-2023 Textea Inc. Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -16,15 +16,16 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: homepage, https://github.com/TexteaInc/
 funix Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Operating System
 :: OS Independent Classifier: Framework :: Flask Classifier: Framework ::
 Matplotlib Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: plot License-File: LICENSE
+Provides-Extra: plot Provides-Extra: git Provides-Extra: all License-File:
+LICENSE
                                 ****** Funix.IO
         â­ï¸ The laziest way to build AI/data apps in Python. â­ï¸
                                      ******
 [![PyPI version](https://badge.fury.io/py/funix.svg)](https://badge.fury.io/py/
                                     funix)
       *** Intro_video | QuickStart_Guide | Reference_Manual | Gallary ***
 https://user-images.githubusercontent.com/438579/236646521-30ed67f4-4708-4cf1-
```

### Comparing `funix-0.4.3/README.md` & `funix-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/__init__.py` & `funix-0.4.4/backend/funix/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from os import listdir
 from os.path import dirname, exists, isdir, join
 from sys import exit, path
 from typing import Generator, Optional
 from urllib.parse import quote
 from flask import Flask
 
-from git import Repo
-
 import funix.decorator as decorator
 import funix.hint as hint
 from funix.app import app
 from funix.frontend import OpenFrontend, run_open_frontend, start
 from funix.prep.global_to_session import get_new_python_file
 from funix.util.file import create_safe_tempdir
 from funix.util.module import import_module_from_file
@@ -37,14 +35,26 @@
 
 # ---- Util ----
 new_funix_type = hint.new_funix_type
 set_app_secret = decorator.set_app_secret
 # ---- Util ----
 # ---- Exports ----
 
+__use_git = False
+"""
+Funix uses git to clone repo, now this feature is optional.
+"""
+
+try:
+    from git import Repo
+
+    __use_git = True
+except:
+    pass
+
 
 def __prep(
     module_or_file: Optional[str],
     lazy: bool,
     need_path: bool,
     is_module: bool,
     need_name: bool,
@@ -108,14 +118,15 @@
                 join(base_dir, file), add_to_sys_path, need_full_path
             )
         if file.endswith(".py") and file != "__init__.py":
             if need_full_path:
                 yield join(base_dir, file)
             yield file[:-3]
 
+
 def import_from_config(
     file_or_module_name: str,
     lazy: Optional[bool] = False,
     dir_mode: Optional[bool] = False,
     package_mode: Optional[bool] = False,
     from_git: Optional[str] = None,
     repo_dir: Optional[str] = None,
@@ -140,31 +151,34 @@
 
     Raises:
         See code for more info.
     """
     if transform and (dir_mode or package_mode):
         raise ValueError("Transform mode is not supported for dir or package mode!")
 
-    if from_git:
-        tempdir = create_safe_tempdir()
-        print("Please wait, cloning git repo...")
-        Repo.clone_from(url=from_git, to_path=tempdir)
-        new_path = tempdir
-        if repo_dir:
-            new_path = join(tempdir, repo_dir)
-        path.append(new_path)
-
-        if file_or_module_name:
-            pass
-        elif dir_mode:
-            file_or_module_name = new_path
-        elif package_mode:
-            raise ValueError(
-                "Package mode is not supported for git mode, try to use dir mode!"
-            )
+    if __use_git:
+        if from_git:
+            tempdir = create_safe_tempdir()
+            print("Please wait, cloning git repo...")
+            Repo.clone_from(url=from_git, to_path=tempdir)
+            new_path = tempdir
+            if repo_dir:
+                new_path = join(tempdir, repo_dir)
+            path.append(new_path)
+
+            if file_or_module_name:
+                pass
+            elif dir_mode:
+                file_or_module_name = new_path
+            elif package_mode:
+                raise ValueError(
+                    "Package mode is not supported for git mode, try to use dir mode!"
+                )
+    else:
+        raise Exception("GitPython is not installed, please install it first!")
 
     if app_secret and isinstance(app_secret, str):
         set_app_secret(app_secret)
 
     if dir_mode:
         if exists(file_or_module_name) and isdir(file_or_module_name):
             for single_file in get_python_files_in_dir(
```

### Comparing `funix-0.4.3/backend/funix/__main__.py` & `funix-0.4.4/backend/funix/__main__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/build/favicon.ico` & `funix-0.4.4/backend/funix/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/build/index.html` & `funix-0.4.4/backend/funix/build/index.html`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/build/logo192.png` & `funix-0.4.4/backend/funix/build/logo192.png`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/build/logo512.png` & `funix-0.4.4/backend/funix/build/logo512.png`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/build/static/css/main.521e60ca.css` & `funix-0.4.4/backend/funix/build/static/css/main.521e60ca.css`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/build/static/js/main.ef806516.js` & `funix-0.4.4/backend/funix/build/static/js/main.ef806516.js`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt` & `funix-0.4.4/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/config/__init__.py` & `funix-0.4.4/backend/funix/config/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/decorator/__init__.py` & `funix-0.4.4/backend/funix/decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/decorator/file.py` & `funix-0.4.4/backend/funix/decorator/file.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/decorator/magic.py` & `funix-0.4.4/backend/funix/decorator/magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/frontend/__init__.py` & `funix-0.4.4/backend/funix/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/hint/__init__.py` & `funix-0.4.4/backend/funix/hint/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/hint/layout.py` & `funix-0.4.4/backend/funix/hint/layout.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/prep/global_to_session.py` & `funix-0.4.4/backend/funix/prep/global_to_session.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/session/__init__.py` & `funix-0.4.4/backend/funix/session/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/test/test_magic.py` & `funix-0.4.4/backend/funix/test/test_magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/theme/__init__.py` & `funix-0.4.4/backend/funix/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/util/module.py` & `funix-0.4.4/backend/funix/util/module.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/util/network.py` & `funix-0.4.4/backend/funix/util/network.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/widget/__init__.py` & `funix-0.4.4/backend/funix/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix/widget/builtin.py` & `funix-0.4.4/backend/funix/widget/builtin.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/backend/funix.egg-info/PKG-INFO` & `funix-0.4.4/backend/funix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.4.3
+Version: 0.4.4
 Summary: Building web apps without manually creating widgets
 Author-email: "Textea Inc." <bao@textea.co>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Flask
 Classifier: Framework :: Matplotlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: plot
+Provides-Extra: git
+Provides-Extra: all
 License-File: LICENSE
 
 <h1 align="center">
     <b>
         Funix.IO<br>
     </b>
     ⭐️  The laziest way to build AI/data apps in Python.  ⭐️ <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funix Version: 0.4.3 Summary: Building web apps
+Metadata-Version: 2.1 Name: funix Version: 0.4.4 Summary: Building web apps
 without manually creating widgets Author-email: "Textea Inc."
 textea.co> License: MIT License Copyright (c) 2022-2023 Textea Inc. Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -16,15 +16,16 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: homepage, https://github.com/TexteaInc/
 funix Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Operating System
 :: OS Independent Classifier: Framework :: Flask Classifier: Framework ::
 Matplotlib Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: plot License-File: LICENSE
+Provides-Extra: plot Provides-Extra: git Provides-Extra: all License-File:
+LICENSE
                                 ****** Funix.IO
         â­ï¸ The laziest way to build AI/data apps in Python. â­ï¸
                                      ******
 [![PyPI version](https://badge.fury.io/py/funix.svg)](https://badge.fury.io/py/
                                     funix)
       *** Intro_video | QuickStart_Guide | Reference_Manual | Gallary ***
 https://user-images.githubusercontent.com/438579/236646521-30ed67f4-4708-4cf1-
```

### Comparing `funix-0.4.3/backend/funix.egg-info/SOURCES.txt` & `funix-0.4.4/backend/funix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funix-0.4.3/pyproject.toml` & `funix-0.4.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "funix"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   {name = "Textea Inc.", email = "bao@textea.co"}
 ]
 license = {file = "LICENSE"}
 description = "Building web apps without manually creating widgets"
 readme = "README.md"
 requires-python = ">=3.10"
@@ -18,23 +18,30 @@
   "Framework :: Matplotlib"
 ]
 dependencies = [
   "flask>=2.2.2",
   "flask_cors>=3.0.10",
   "functions-framework==3.*",
   "requests>=2.28.1",
-  "plac>=1.3.5",
-  "GitPython>=3.1.31",
+  "plac>=1.3.5"
 ]
 
 [project.optional-dependencies]
 plot = [
   "matplotlib>=3.4.3",
   "mpld3>=0.5.8",
 ]
+git = [
+  "GitPython>=3.1.31",
+]
+all = [
+  "matplotlib>=3.4.3",
+  "mpld3>=0.5.8",
+  "GitPython>=3.1.31",
+]
 
 [project.urls]
 homepage = "https://github.com/TexteaInc/funix"
 
 [project.scripts]
 funix = "funix.__main__:cli_main"
```

