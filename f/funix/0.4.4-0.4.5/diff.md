# Comparing `tmp/funix-0.4.4.tar.gz` & `tmp/funix-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funix-0.4.4.tar", last modified: Tue Jul  4 15:06:11 2023, max compression
+gzip compressed data, was "funix-0.4.5.tar", last modified: Tue Jul  4 15:31:55 2023, max compression
```

## Comparing `funix-0.4.4.tar` & `funix-0.4.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.905564 funix-0.4.4/
--rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.4.4/LICENSE
--rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.4.4/MANIFEST.in
--rw-r--r--   0 yazawazi   (501) staff       (20)     8669 2023-07-04 15:06:11.905652 funix-0.4.4/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)     6748 2023-05-08 21:04:14.000000 funix-0.4.4/README.md
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.886555 funix-0.4.4/backend/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.888396 funix-0.4.4/backend/funix/
--rw-r--r--   0 yazawazi   (501) staff       (20)    12895 2023-07-04 15:03:42.000000 funix-0.4.4/backend/funix/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4171 2023-05-23 06:01:29.000000 funix-0.4.4/backend/funix/__main__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.890925 funix-0.4.4/backend/funix/app/
--rw-r--r--   0 yazawazi   (501) staff       (20)      178 2023-05-26 11:05:26.000000 funix-0.4.4/backend/funix/app/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.892492 funix-0.4.4/backend/funix/build/
--rw-r--r--   0 yazawazi   (501) staff       (20)      240 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/asset-manifest.json
--rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2023-05-27 08:54:36.000000 funix-0.4.4/backend/funix/build/favicon.ico
--rw-r--r--   0 yazawazi   (501) staff       (20)      806 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/index.html
--rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2023-05-27 08:54:36.000000 funix-0.4.4/backend/funix/build/logo192.png
--rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2023-05-27 08:54:36.000000 funix-0.4.4/backend/funix/build/logo512.png
--rw-r--r--   0 yazawazi   (501) staff       (20)      492 2023-05-27 08:54:36.000000 funix-0.4.4/backend/funix/build/manifest.json
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.886823 funix-0.4.4/backend/funix/build/static/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.892919 funix-0.4.4/backend/funix/build/static/css/
--rw-r--r--   0 yazawazi   (501) staff       (20)     9350 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/static/css/main.521e60ca.css
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.897476 funix-0.4.4/backend/funix/build/static/js/
--rw-r--r--   0 yazawazi   (501) staff       (20)  6555220 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/static/js/main.ef806516.js
--rw-r--r--   0 yazawazi   (501) staff       (20)     4231 2023-05-27 08:54:58.000000 funix-0.4.4/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.897830 funix-0.4.4/backend/funix/config/
--rw-r--r--   0 yazawazi   (501) staff       (20)      928 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/config/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.901346 funix-0.4.4/backend/funix/decorator/
--rw-r--r--   0 yazawazi   (501) staff       (20)    53592 2023-06-01 23:35:40.000000 funix-0.4.4/backend/funix/decorator/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3113 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/decorator/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    10936 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/decorator/magic.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.901474 funix-0.4.4/backend/funix/frontend/
--rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-05-23 09:37:53.000000 funix-0.4.4/backend/funix/frontend/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.901706 funix-0.4.4/backend/funix/hint/
--rw-r--r--   0 yazawazi   (501) staff       (20)    10668 2023-06-01 23:31:16.000000 funix-0.4.4/backend/funix/hint/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3823 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/hint/layout.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.901891 funix-0.4.4/backend/funix/prep/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.4.4/backend/funix/prep/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     7547 2023-05-26 10:41:26.000000 funix-0.4.4/backend/funix/prep/global_to_session.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.902197 funix-0.4.4/backend/funix/session/
--rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2023-05-26 11:04:02.000000 funix-0.4.4/backend/funix/session/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.903884 funix-0.4.4/backend/funix/test/
--rw-r--r--   0 yazawazi   (501) staff       (20)     5327 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/test/test_magic.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.904178 funix-0.4.4/backend/funix/theme/
--rw-r--r--   0 yazawazi   (501) staff       (20)    10204 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/theme/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.905019 funix-0.4.4/backend/funix/util/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      456 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      771 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/module.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4268 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/network.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      467 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/util/uri.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.905303 funix-0.4.4/backend/funix/widget/
--rw-r--r--   0 yazawazi   (501) staff       (20)     4602 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/widget/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4689 2023-05-23 03:43:55.000000 funix-0.4.4/backend/funix/widget/builtin.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:06:11.890812 funix-0.4.4/backend/funix.egg-info/
--rw-r--r--   0 yazawazi   (501) staff       (20)     8669 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)     1323 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/SOURCES.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        1 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/dependency_links.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)       50 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/entry_points.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)      206 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/requires.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        6 2023-07-04 15:06:11.000000 funix-0.4.4/backend/funix.egg-info/top_level.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)     1021 2023-07-04 15:01:30.000000 funix-0.4.4/pyproject.toml
--rw-r--r--   0 yazawazi   (501) staff       (20)      114 2023-07-04 15:06:11.905937 funix-0.4.4/setup.cfg
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.103181 funix-0.4.5/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.4.5/LICENSE
+-rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.4.5/MANIFEST.in
+-rw-r--r--   0 yazawazi   (501) staff       (20)     8669 2023-07-04 15:31:55.103269 funix-0.4.5/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)     6748 2023-05-08 21:04:14.000000 funix-0.4.5/README.md
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.083332 funix-0.4.5/backend/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.084955 funix-0.4.5/backend/funix/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    12921 2023-07-04 15:28:39.000000 funix-0.4.5/backend/funix/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4171 2023-05-23 06:01:29.000000 funix-0.4.5/backend/funix/__main__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.085842 funix-0.4.5/backend/funix/app/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      178 2023-05-26 11:05:26.000000 funix-0.4.5/backend/funix/app/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.087663 funix-0.4.5/backend/funix/build/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      240 2023-05-27 08:54:58.000000 funix-0.4.5/backend/funix/build/asset-manifest.json
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2023-05-27 08:54:36.000000 funix-0.4.5/backend/funix/build/favicon.ico
+-rw-r--r--   0 yazawazi   (501) staff       (20)      806 2023-05-27 08:54:58.000000 funix-0.4.5/backend/funix/build/index.html
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2023-05-27 08:54:36.000000 funix-0.4.5/backend/funix/build/logo192.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2023-05-27 08:54:36.000000 funix-0.4.5/backend/funix/build/logo512.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)      492 2023-05-27 08:54:36.000000 funix-0.4.5/backend/funix/build/manifest.json
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.083609 funix-0.4.5/backend/funix/build/static/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.087907 funix-0.4.5/backend/funix/build/static/css/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9350 2023-05-27 08:54:58.000000 funix-0.4.5/backend/funix/build/static/css/main.521e60ca.css
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.091269 funix-0.4.5/backend/funix/build/static/js/
+-rw-r--r--   0 yazawazi   (501) staff       (20)  6555220 2023-05-27 08:54:58.000000 funix-0.4.5/backend/funix/build/static/js/main.ef806516.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4231 2023-05-27 08:54:58.000000 funix-0.4.5/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.091922 funix-0.4.5/backend/funix/config/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      928 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/config/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.096693 funix-0.4.5/backend/funix/decorator/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    54713 2023-07-04 15:28:39.000000 funix-0.4.5/backend/funix/decorator/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3113 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/decorator/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10936 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/decorator/magic.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.096812 funix-0.4.5/backend/funix/frontend/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-05-23 09:37:53.000000 funix-0.4.5/backend/funix/frontend/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.097029 funix-0.4.5/backend/funix/hint/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10668 2023-07-04 15:28:39.000000 funix-0.4.5/backend/funix/hint/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3823 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/hint/layout.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.097215 funix-0.4.5/backend/funix/prep/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.4.5/backend/funix/prep/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     7547 2023-07-04 15:28:39.000000 funix-0.4.5/backend/funix/prep/global_to_session.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.097328 funix-0.4.5/backend/funix/session/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2023-07-04 15:28:37.000000 funix-0.4.5/backend/funix/session/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.097437 funix-0.4.5/backend/funix/test/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5327 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/test/test_magic.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.097568 funix-0.4.5/backend/funix/theme/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10204 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/theme/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.102768 funix-0.4.5/backend/funix/util/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/util/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      456 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/util/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      771 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/util/module.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4268 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/util/network.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      467 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/util/uri.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.103065 funix-0.4.5/backend/funix/widget/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4602 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/widget/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4689 2023-05-23 03:43:55.000000 funix-0.4.5/backend/funix/widget/builtin.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-04 15:31:55.085715 funix-0.4.5/backend/funix.egg-info/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     8669 2023-07-04 15:31:55.000000 funix-0.4.5/backend/funix.egg-info/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1323 2023-07-04 15:31:55.000000 funix-0.4.5/backend/funix.egg-info/SOURCES.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        1 2023-07-04 15:31:55.000000 funix-0.4.5/backend/funix.egg-info/dependency_links.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)       50 2023-07-04 15:31:55.000000 funix-0.4.5/backend/funix.egg-info/entry_points.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)      206 2023-07-04 15:31:55.000000 funix-0.4.5/backend/funix.egg-info/requires.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        6 2023-07-04 15:31:55.000000 funix-0.4.5/backend/funix.egg-info/top_level.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1021 2023-07-04 15:29:57.000000 funix-0.4.5/pyproject.toml
+-rw-r--r--   0 yazawazi   (501) staff       (20)      114 2023-07-04 15:31:55.103546 funix-0.4.5/setup.cfg
```

### Comparing `funix-0.4.4/LICENSE` & `funix-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/PKG-INFO` & `funix-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.4.4
+Version: 0.4.5
 Summary: Building web apps without manually creating widgets
 Author-email: "Textea Inc." <bao@textea.co>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funix Version: 0.4.4 Summary: Building web apps
+Metadata-Version: 2.1 Name: funix Version: 0.4.5 Summary: Building web apps
 without manually creating widgets Author-email: "Textea Inc."
 textea.co> License: MIT License Copyright (c) 2022-2023 Textea Inc. Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `funix-0.4.4/README.md` & `funix-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/__init__.py` & `funix-0.4.5/backend/funix/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from inspect import isfunction
 from ipaddress import ip_address
 from os import listdir
 from os.path import dirname, exists, isdir, join
 from sys import exit, path
 from typing import Generator, Optional
 from urllib.parse import quote
+
 from flask import Flask
 
 import funix.decorator as decorator
 import funix.hint as hint
 from funix.app import app
 from funix.frontend import OpenFrontend, run_open_frontend, start
 from funix.prep.global_to_session import get_new_python_file
@@ -170,15 +171,16 @@
             elif dir_mode:
                 file_or_module_name = new_path
             elif package_mode:
                 raise ValueError(
                     "Package mode is not supported for git mode, try to use dir mode!"
                 )
     else:
-        raise Exception("GitPython is not installed, please install it first!")
+        if from_git:
+            raise Exception("GitPython is not installed, please install it first!")
 
     if app_secret and isinstance(app_secret, str):
         set_app_secret(app_secret)
 
     if dir_mode:
         if exists(file_or_module_name) and isdir(file_or_module_name):
             for single_file in get_python_files_in_dir(
```

### Comparing `funix-0.4.4/backend/funix/__main__.py` & `funix-0.4.5/backend/funix/__main__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/build/favicon.ico` & `funix-0.4.5/backend/funix/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/build/index.html` & `funix-0.4.5/backend/funix/build/index.html`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/build/logo192.png` & `funix-0.4.5/backend/funix/build/logo192.png`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/build/logo512.png` & `funix-0.4.5/backend/funix/build/logo512.png`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/build/static/css/main.521e60ca.css` & `funix-0.4.5/backend/funix/build/static/css/main.521e60ca.css`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/build/static/js/main.ef806516.js` & `funix-0.4.5/backend/funix/build/static/js/main.ef806516.js`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt` & `funix-0.4.5/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/config/__init__.py` & `funix-0.4.5/backend/funix/config/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/decorator/__init__.py` & `funix-0.4.5/backend/funix/decorator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,23 +36,24 @@
     DecoratedFunctionListItem,
     DestinationType,
     DirectionType,
     ExamplesType,
     InputLayout,
     LabelsType,
     OutputLayout,
+    PreFillEmpty,
+    PreFillType,
     SessionVariablesType,
     TreatAsType,
     WhitelistType,
-    WidgetsType, PreFillType, PreFillEmpty,
+    WidgetsType,
 )
+from funix.session import get_global_variable, set_global_variable
 from funix.theme import get_dict_theme, parse_theme
 from funix.widget import generate_frontend_widget_config
-from funix.session import set_global_variable, get_global_variable
-
 
 __matplotlib_use = False
 """
 Whether Funix can handle matplotlib-related logic
 """
 
 try:
@@ -547,24 +548,34 @@
                         return_output_indexes.append(row_item_done["index"])
                     row_layout.append(row_item_done)
                 return_output_layout.append(row_layout)
 
             if pre_fill:
                 for _, from_arg_function_info in pre_fill.items():
                     if isinstance(from_arg_function_info, tuple):
-                        from_arg_function_name = getattr(from_arg_function_info[0], "__name__")
+                        from_arg_function_name = getattr(
+                            from_arg_function_info[0], "__name__"
+                        )
                         from_arg_function_index_or_key = from_arg_function_info[1]
                         if from_arg_function_name in pre_fill_metadata:
-                            pre_fill_metadata[from_arg_function_name].append(from_arg_function_index_or_key)
+                            pre_fill_metadata[from_arg_function_name].append(
+                                from_arg_function_index_or_key
+                            )
                         else:
-                            pre_fill_metadata[from_arg_function_name] = [from_arg_function_index_or_key]
+                            pre_fill_metadata[from_arg_function_name] = [
+                                from_arg_function_index_or_key
+                            ]
                     else:
-                        from_arg_function_name = getattr(from_arg_function_info, "__name__")
+                        from_arg_function_name = getattr(
+                            from_arg_function_info, "__name__"
+                        )
                         if from_arg_function_name in pre_fill_metadata:
-                            pre_fill_metadata[from_arg_function_name].append(PreFillEmpty)
+                            pre_fill_metadata[from_arg_function_name].append(
+                                PreFillEmpty
+                            )
                         else:
                             pre_fill_metadata[from_arg_function_name] = [PreFillEmpty]
 
             def create_decorated_params(arg_name: str) -> None:
                 """
                 Creates a decorated_params entry for the given arg_name if it doesn't exist
 
@@ -900,24 +911,31 @@
                     flask.Response: The function's parameters
                 """
                 if pre_fill is not None:
                     new_decorated_function = deepcopy(decorated_function)
                     for argument_key, from_function_info in pre_fill.items():
                         if isinstance(from_function_info, tuple):
                             last_result = get_global_variable(
-                                getattr(from_function_info[0], "__name__") + f"_{from_function_info[1]}"
+                                getattr(from_function_info[0], "__name__")
+                                + f"_{from_function_info[1]}"
                             )
                         else:
                             last_result = get_global_variable(
                                 getattr(from_function_info, "__name__") + "_result"
                             )
                         if last_result is not None:
-                            new_decorated_function["params"][argument_key]["default"] = last_result
-                            new_decorated_function["schema"]["properties"][argument_key]["default"] = last_result
-                    return Response(dumps(new_decorated_function), mimetype="application/json")
+                            new_decorated_function["params"][argument_key][
+                                "default"
+                            ] = last_result
+                            new_decorated_function["schema"]["properties"][
+                                argument_key
+                            ]["default"] = last_result
+                    return Response(
+                        dumps(new_decorated_function), mimetype="application/json"
+                    )
                 return Response(dumps(decorated_function), mimetype="application/json")
 
             decorated_function_param_getter.__setattr__(
                 "__name__", f"{function_name}_param_getter"
             )
             get_wrapper_endpoint(decorated_function_param_getter)
             get_wrapper_id(decorated_function_param_getter)
@@ -1027,49 +1045,58 @@
                         The function's wrapper
                         """
                         # TODO: Best result handling, refactor it if possible
                         try:
                             function_call_result = function(**wrapped_function_kwargs)
                             function_call_name = getattr(function, "__name__")
                             if function_call_name in pre_fill_metadata:
-                                for index_or_key in pre_fill_metadata[function_call_name]:
+                                for index_or_key in pre_fill_metadata[
+                                    function_call_name
+                                ]:
                                     if index_or_key is PreFillEmpty:
-                                        set_global_variable(function_call_name + "_result", function_call_result)
+                                        set_global_variable(
+                                            function_call_name + "_result",
+                                            function_call_result,
+                                        )
                                     else:
                                         set_global_variable(
                                             function_call_name + f"_{index_or_key}",
-                                            function_call_result[index_or_key]
+                                            function_call_result[index_or_key],
                                         )
                             if return_type_parsed == "Figure":
                                 return [get_figure(function_call_result)]
                             if return_type_parsed in supported_basic_file_types:
-                                return [
-                                    get_static_uri(function_call_result)
-                                ]
+                                return [get_static_uri(function_call_result)]
                             else:
                                 if isinstance(function_call_result, list):
                                     return [function_call_result]
-                                if not isinstance(function_call_result, (str, dict, tuple)):
+                                if not isinstance(
+                                    function_call_result, (str, dict, tuple)
+                                ):
                                     function_call_result = dumps(function_call_result)
                                 if cast_to_list_flag:
                                     function_call_result = list(function_call_result)
                                 else:
                                     if isinstance(function_call_result, (str, dict)):
                                         function_call_result = [function_call_result]
                                     if isinstance(function_call_result, tuple):
-                                        function_call_result = list(function_call_result)
+                                        function_call_result = list(
+                                            function_call_result
+                                        )
                                 if function_call_result and isinstance(
                                     function_call_result, list
                                 ):
                                     if isinstance(return_type_parsed, list):
                                         for position, single_return_type in enumerate(
                                             return_type_parsed
                                         ):
                                             if single_return_type == "Figure":
-                                                function_call_result[position] = get_figure(
+                                                function_call_result[
+                                                    position
+                                                ] = get_figure(
                                                     function_call_result[position]
                                                 )
                                             if (
                                                 single_return_type
                                                 in supported_basic_file_types
                                             ):
                                                 if (
@@ -1098,20 +1125,24 @@
                                             return_type_parsed
                                             in supported_basic_file_types
                                         ):
                                             if type(function_call_result[0]) == "list":
                                                 function_call_result = [
                                                     [
                                                         get_static_uri(single)
-                                                        for single in function_call_result[0]
+                                                        for single in function_call_result[
+                                                            0
+                                                        ]
                                                     ]
                                                 ]
                                             else:
                                                 function_call_result = [
-                                                    get_static_uri(function_call_result[0])
+                                                    get_static_uri(
+                                                        function_call_result[0]
+                                                    )
                                                 ]
                                         return function_call_result
                                 return function_call_result
                         except:
                             return {
                                 "error_type": "function",
                                 "error_body": format_exc(),
```

### Comparing `funix-0.4.4/backend/funix/decorator/file.py` & `funix-0.4.5/backend/funix/decorator/file.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/decorator/magic.py` & `funix-0.4.5/backend/funix/decorator/magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/frontend/__init__.py` & `funix-0.4.5/backend/funix/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/hint/__init__.py` & `funix-0.4.5/backend/funix/hint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This file is used to define the type hint of the Funix backend.
 """
 
-from typing import Literal, NewType, Optional, TypeAlias, TypedDict, TypeVar, Callable
+from typing import Callable, Literal, NewType, Optional, TypeAlias, TypedDict, TypeVar
 
 from funix.hint.layout import InputRow, OutputRow
 from funix.widget import builtin
 
 DestinationType = Optional[Literal["column", "row", "sheet"]]
 """
 For yodas only, the destination of the page.
```

### Comparing `funix-0.4.4/backend/funix/hint/layout.py` & `funix-0.4.5/backend/funix/hint/layout.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/prep/global_to_session.py` & `funix-0.4.5/backend/funix/prep/global_to_session.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/session/__init__.py` & `funix-0.4.5/backend/funix/session/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Control the global variables.
 """
 
-from typing import Any
 from copy import deepcopy
+from typing import Any
 
 from flask import session
 
 UserID = str
 """
 User ID, `__funix_id` in session.
 """
@@ -85,11 +85,11 @@
     global __funix_global_variables, __funix_default_global_variables
     user_id = session.get("__funix_id")
     if not user_id:
         raise RuntimeError("User ID not found in session.")
     if user_id not in __funix_global_variables:
         __funix_global_variables[user_id] = {}
     if name not in __funix_global_variables[user_id]:
-        __funix_global_variables[user_id][name] = deepcopy(__funix_default_global_variables.get(
-            name, None
-        ))
+        __funix_global_variables[user_id][name] = deepcopy(
+            __funix_default_global_variables.get(name, None)
+        )
     return __funix_global_variables[user_id].get(name, None)
```

### Comparing `funix-0.4.4/backend/funix/test/test_magic.py` & `funix-0.4.5/backend/funix/test/test_magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/theme/__init__.py` & `funix-0.4.5/backend/funix/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/util/module.py` & `funix-0.4.5/backend/funix/util/module.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/util/network.py` & `funix-0.4.5/backend/funix/util/network.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/widget/__init__.py` & `funix-0.4.5/backend/funix/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix/widget/builtin.py` & `funix-0.4.5/backend/funix/widget/builtin.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/backend/funix.egg-info/PKG-INFO` & `funix-0.4.5/backend/funix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.4.4
+Version: 0.4.5
 Summary: Building web apps without manually creating widgets
 Author-email: "Textea Inc." <bao@textea.co>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funix Version: 0.4.4 Summary: Building web apps
+Metadata-Version: 2.1 Name: funix Version: 0.4.5 Summary: Building web apps
 without manually creating widgets Author-email: "Textea Inc."
 textea.co> License: MIT License Copyright (c) 2022-2023 Textea Inc. Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `funix-0.4.4/backend/funix.egg-info/SOURCES.txt` & `funix-0.4.5/backend/funix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funix-0.4.4/pyproject.toml` & `funix-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "funix"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
   {name = "Textea Inc.", email = "bao@textea.co"}
 ]
 license = {file = "LICENSE"}
 description = "Building web apps without manually creating widgets"
 readme = "README.md"
 requires-python = ">=3.10"
```

