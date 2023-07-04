# Comparing `tmp/opr-210.tar.gz` & `tmp/opr-220.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opr-210.tar", last modified: Tue Jul  4 00:54:05 2023, max compression
+gzip compressed data, was "opr-220.tar", last modified: Tue Jul  4 14:57:11 2023, max compression
```

## Comparing `opr-210.tar` & `opr-220.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.379548 opr-210/
--rw-r--r--   0 bart      (1000) bart      (1000)     2325 2023-07-04 00:54:05.379548 opr-210/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1775 2023-07-01 05:55:02.000000 opr-210/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.375548 opr-210/opr/
--rw-r--r--   0 bart      (1000) bart      (1000)      134 2023-07-03 12:59:17.000000 opr-210/opr/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     8946 2023-07-03 12:53:54.000000 opr-210/opr/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)      535 2023-07-03 12:35:01.000000 opr-210/opr/loggers.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.375548 opr-210/opr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      460 2023-07-03 19:18:45.000000 opr-210/opr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      221 2023-07-03 00:11:35.000000 opr-210/opr/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      704 2023-07-03 00:11:44.000000 opr-210/opr/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      390 2023-07-03 11:40:39.000000 opr-210/opr/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      937 2023-07-03 11:41:20.000000 opr-210/opr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    20759 2023-07-03 12:52:48.000000 opr-210/opr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      826 2023-07-03 00:19:09.000000 opr-210/opr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)      330 2023-07-03 11:17:11.000000 opr-210/opr/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     8130 2023-07-03 11:42:24.000000 opr-210/opr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1039 2023-07-03 00:19:36.000000 opr-210/opr/modules/shp.py
--rw-r--r--   0 bart      (1000) bart      (1000)      342 2023-07-03 11:42:39.000000 opr-210/opr/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1065 2023-07-03 00:20:30.000000 opr-210/opr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)      995 2023-07-03 00:15:32.000000 opr-210/opr/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)      218 2023-07-03 00:15:40.000000 opr-210/opr/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6951 2023-07-03 12:35:39.000000 opr-210/opr/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5121 2023-07-03 14:25:17.000000 opr-210/opr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1429 2023-07-03 12:41:32.000000 opr-210/opr/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4395 2023-07-04 00:48:57.000000 opr-210/opr/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2372 2023-07-03 12:33:25.000000 opr-210/opr/threads.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1978 2023-07-03 12:42:29.000000 opr-210/opr/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.375548 opr-210/opr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2325 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      778 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       41 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      886 2023-07-04 00:53:22.000000 opr-210/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-04 00:54:05.379548 opr-210/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-01 10:59:30.000000 opr-210/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.379548 opr-210/test/
--rw-r--r--   0 bart      (1000) bart      (1000)      675 2023-07-01 05:55:02.000000 opr-210/test/test_composite.py
--rw-r--r--   0 bart      (1000) bart      (1000)      442 2023-07-03 12:00:09.000000 opr-210/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      370 2023-07-03 12:00:20.000000 opr-210/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      935 2023-07-01 05:55:02.000000 opr-210/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4376 2023-07-03 11:59:37.000000 opr-210/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)      642 2023-07-03 13:43:53.000000 opr-210/test/test_recursive.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1232 2023-07-03 01:04:57.000000 opr-210/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-07-04 14:57:11.079510 opr-220/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1923 2023-07-04 14:13:27.000000 opr-220/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/opr/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1914 2023-07-04 11:49:32.000000 opr-220/opr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      134 2023-07-03 12:59:17.000000 opr-220/opr/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     8946 2023-07-03 12:53:54.000000 opr-220/opr/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      535 2023-07-03 12:35:01.000000 opr-220/opr/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/opr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      361 2023-07-04 13:24:11.000000 opr-220/opr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      937 2023-07-03 11:41:20.000000 opr-220/opr/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    20759 2023-07-03 12:52:48.000000 opr-220/opr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      826 2023-07-03 00:19:09.000000 opr-220/opr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4225 2023-07-03 11:59:03.000000 opr-220/opr/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17810 2023-07-03 12:57:45.000000 opr-220/opr/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2354 2023-07-01 05:55:02.000000 opr-220/opr/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     8130 2023-07-03 11:42:24.000000 opr-220/opr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1039 2023-07-03 00:19:36.000000 opr-220/opr/modules/shp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1065 2023-07-03 00:20:30.000000 opr-220/opr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2934 2023-07-03 11:58:30.000000 opr-220/opr/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5691 2023-07-01 05:55:02.000000 opr-220/opr/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7012 2023-07-04 11:52:44.000000 opr-220/opr/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5121 2023-07-03 14:25:17.000000 opr-220/opr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1429 2023-07-03 12:41:32.000000 opr-220/opr/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7803 2023-07-04 14:10:29.000000 opr-220/opr/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2372 2023-07-03 12:33:25.000000 opr-220/opr/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1978 2023-07-03 12:42:29.000000 opr-220/opr/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/opr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      756 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       41 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      900 2023-07-04 14:56:37.000000 opr-220/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-04 14:57:11.079510 opr-220/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-01 10:59:30.000000 opr-220/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/test/
+-rw-r--r--   0 bart      (1000) bart      (1000)      675 2023-07-01 05:55:02.000000 opr-220/test/test_composite.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      442 2023-07-03 12:00:09.000000 opr-220/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      370 2023-07-03 12:00:20.000000 opr-220/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      935 2023-07-01 05:55:02.000000 opr-220/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4382 2023-07-04 02:35:41.000000 opr-220/test/test_objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      642 2023-07-03 13:43:53.000000 opr-220/test/test_recursive.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1232 2023-07-03 01:04:57.000000 opr-220/test/test_storage.py
```

### Comparing `opr-210/PKG-INFO` & `opr-220/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 210
+Version: 220
 Summary: Object Programming Runtime
-Author-email: Bart Thate <bthate@dds.nl>
+Author-email: Bart Thate <programmingobject@gmail.com>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/opr
 Project-URL: bugs, https://github.com/bthate/opr/issues
 Project-URL: source, https://github.com/bthate/opr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
@@ -15,34 +15,39 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
 NAME
 
 ::
 
-    OPR - Object Programming Runtime
+   OPR - Object Programming Runtime
 
 
-SYNOPSIS
+DESCRIPTION
+
 
 ::
 
-    opr <cmd> [key=val] 
-    opr <cmd> [key==val]
-    opr [-c] [-d] [-v]
+    OPR is a python3 runtime is intended to be programmable  in a
+    static, only code, no popen, no user imports and no reading
+    modules from a directory, way. 
 
+    OPR provides some functionality, it can connect to IRC, fetch
+    and display RSS feeds, take todo notes, keep a shopping list and
+    log text.
 
-DESCRIPTION
 
-::
+SYNOPSIS
 
 
-    OPR is a python3 runtime is intended to be programmable  in a
-    static, only code, no popen, no user imports and no reading
-    modules from a directory, way. 
+::
+
+    opr <cmd> [key=val] 
+    opr <cmd> [key==val]
+    opr [-c] [-d] [-v]
 
 
 INSTALL
 
 
 ::
 
@@ -55,15 +60,14 @@
 ::
 
     list of commands
 
     $ opr cmd
     cmd,err,flt,sts,thr,upt
 
-
     start a console
 
     $ opr -c
     >
 
     start additional modules
 
@@ -145,15 +149,14 @@
 
     ~/.local/bin/opr
     ~/.local/pipx/venvs/opr/
 
 
 AUTHOR
 
-
 ::
 
     Bart Thate <bthate@dds.nl>
 
 
 COPYRIGHT
```

### Comparing `opr-210/README.rst` & `opr-220/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 NAME
 
 ::
 
-    OPR - Object Programming Runtime
+   OPR - Object Programming Runtime
 
 
-SYNOPSIS
+DESCRIPTION
+
 
 ::
 
-    opr <cmd> [key=val] 
-    opr <cmd> [key==val]
-    opr [-c] [-d] [-v]
+    OPR is a python3 runtime is intended to be programmable  in a
+    static, only code, no popen, no user imports and no reading
+    modules from a directory, way. 
 
+    OPR provides some functionality, it can connect to IRC, fetch
+    and display RSS feeds, take todo notes, keep a shopping list and
+    log text.
 
-DESCRIPTION
 
-::
+SYNOPSIS
 
 
-    OPR is a python3 runtime is intended to be programmable  in a
-    static, only code, no popen, no user imports and no reading
-    modules from a directory, way. 
+::
+
+    opr <cmd> [key=val] 
+    opr <cmd> [key==val]
+    opr [-c] [-d] [-v]
 
 
 INSTALL
 
 
 ::
 
@@ -38,15 +43,14 @@
 ::
 
     list of commands
 
     $ opr cmd
     cmd,err,flt,sts,thr,upt
 
-
     start a console
 
     $ opr -c
     >
 
     start additional modules
 
@@ -128,15 +132,14 @@
 
     ~/.local/bin/opr
     ~/.local/pipx/venvs/opr/
 
 
 AUTHOR
 
-
 ::
 
     Bart Thate <bthate@dds.nl>
 
 
 COPYRIGHT
```

### Comparing `opr-210/opr/handler.py` & `opr-220/opr/handler.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/loggers.py` & `opr-220/opr/loggers.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/modules/fnd.py` & `opr-220/opr/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/modules/irc.py` & `opr-220/opr/modules/irc.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/modules/log.py` & `opr-220/opr/modules/log.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/modules/rss.py` & `opr-220/opr/modules/rss.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/modules/shp.py` & `opr-220/opr/modules/shp.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/modules/tdo.py` & `opr-220/opr/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/objects.py` & `opr-220/opr/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,42 @@
 import datetime
 import json
 import os
 import uuid
 import _thread
 
 
-# DEFINEs
+# DEFINES
 
 
 def __dir__():
     return (
             'Object',
             'ObjectDecoder',
             'ObjectEncoder',
             'copy',
             'dump',
             'dumprec',
             'dumps',
+            'edit',
             'ident',
             'items',
             'keys',
             'kind',
             'load',
             'loads',
+            'prt',
             'update',
             'values'
            )
 
 
+__all__ = __dir__()
+
+
 disklock = _thread.allocate_lock()
 
 
 # CLASSES
 
 
 class Object:
```

### Comparing `opr-210/opr/persist.py` & `opr-220/opr/persist.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/repeats.py` & `opr-220/opr/repeats.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/threads.py` & `opr-220/opr/threads.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr/utility.py` & `opr-220/opr/utility.py`

 * *Files identical despite different names*

### Comparing `opr-210/opr.egg-info/PKG-INFO` & `opr-220/opr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 210
+Version: 220
 Summary: Object Programming Runtime
-Author-email: Bart Thate <bthate@dds.nl>
+Author-email: Bart Thate <programmingobject@gmail.com>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/opr
 Project-URL: bugs, https://github.com/bthate/opr/issues
 Project-URL: source, https://github.com/bthate/opr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
@@ -15,34 +15,39 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
 NAME
 
 ::
 
-    OPR - Object Programming Runtime
+   OPR - Object Programming Runtime
 
 
-SYNOPSIS
+DESCRIPTION
+
 
 ::
 
-    opr <cmd> [key=val] 
-    opr <cmd> [key==val]
-    opr [-c] [-d] [-v]
+    OPR is a python3 runtime is intended to be programmable  in a
+    static, only code, no popen, no user imports and no reading
+    modules from a directory, way. 
 
+    OPR provides some functionality, it can connect to IRC, fetch
+    and display RSS feeds, take todo notes, keep a shopping list and
+    log text.
 
-DESCRIPTION
 
-::
+SYNOPSIS
 
 
-    OPR is a python3 runtime is intended to be programmable  in a
-    static, only code, no popen, no user imports and no reading
-    modules from a directory, way. 
+::
+
+    opr <cmd> [key=val] 
+    opr <cmd> [key==val]
+    opr [-c] [-d] [-v]
 
 
 INSTALL
 
 
 ::
 
@@ -55,15 +60,14 @@
 ::
 
     list of commands
 
     $ opr cmd
     cmd,err,flt,sts,thr,upt
 
-
     start a console
 
     $ opr -c
     >
 
     start additional modules
 
@@ -145,15 +149,14 @@
 
     ~/.local/bin/opr
     ~/.local/pipx/venvs/opr/
 
 
 AUTHOR
 
-
 ::
 
     Bart Thate <bthate@dds.nl>
 
 
 COPYRIGHT
```

### Comparing `opr-210/opr.egg-info/SOURCES.txt` & `opr-220/opr.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.rst
 pyproject.toml
 setup.py
+opr/__init__.py
 opr/__main__.py
 opr/handler.py
 opr/loggers.py
 opr/objects.py
 opr/persist.py
 opr/repeats.py
 opr/runtime.py
@@ -14,27 +15,25 @@
 opr.egg-info/SOURCES.txt
 opr.egg-info/dependency_links.txt
 opr.egg-info/entry_points.txt
 opr.egg-info/requires.txt
 opr.egg-info/top_level.txt
 opr.egg-info/zip-safe
 opr/modules/__init__.py
-opr/modules/cmd.py
-opr/modules/err.py
-opr/modules/flt.py
 opr/modules/fnd.py
 opr/modules/irc.py
 opr/modules/log.py
-opr/modules/mod.py
+opr/modules/mbx.py
+opr/modules/mdl.py
+opr/modules/req.py
 opr/modules/rss.py
 opr/modules/shp.py
-opr/modules/sts.py
 opr/modules/tdo.py
-opr/modules/thr.py
-opr/modules/upt.py
+opr/modules/udp.py
+opr/modules/wsd.py
 test/test_composite.py
 test/test_decoder.py
 test/test_encoder.py
 test/test_inherit.py
 test/test_objects.py
 test/test_recursive.py
 test/test_storage.py
```

### Comparing `opr-210/pyproject.toml` & `opr-220/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "opr"
 description = "Object Programming Runtime"
-version = "210"
+version = "220"
 authors = [
-    {name = "Bart Thate", email = "bthate@dds.nl" },
+    {name = "Bart Thate", email = "programmingobject@gmail.com" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers=[
              'Development Status :: 3 - Alpha',
              'License :: Public Domain',
              'Operating System :: Unix',
```

### Comparing `opr-210/test/test_composite.py` & `opr-220/test/test_composite.py`

 * *Files identical despite different names*

### Comparing `opr-210/test/test_inherit.py` & `opr-220/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `opr-210/test/test_objects.py` & `opr-220/test/test_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 class TestObject(unittest.TestCase):
 
     def test_constructor(self):
         obj = Object()
         self.assertTrue(type(obj), Object)
 
-    def test__class(self):
+    def test_class(self):
         obj = Object()
         clz = obj.__class__()
         self.assertTrue("Object" in str(type(clz)))
 
     def test_contains(self):
         obj = Object()
         obj.key = "value"
@@ -98,15 +98,15 @@
         self.assertEqual(obj.__format__(""), "{}")
 
     def test_getattribute(self):
         obj = Object()
         obj.key = "value"
         self.assertEqual(obj.__getattribute__("key"), "value")
 
-    def test_hash__(self):
+    def test_hash(self):
         obj = Object()
         hsj = hash(obj)
         self.assertTrue(isinstance(hsj, int))
 
     def test_init(self):
         obj = Object()
         self.assertTrue(type(Object.__init__(obj)), Object)
@@ -122,15 +122,15 @@
         )
 
     def test_len(self):
         obj = Object()
         self.assertEqual(len(obj), 0)
 
     def test_module(self):
-        self.assertTrue(Object().__module__, "nop")
+        self.assertEqual(Object().__module__, "opr.objects")
 
     def test_kind(self):
         self.assertEqual(kind(Object()), "opr.objects.Object")
 
     def test_repr(self):
         self.assertTrue(update(Object(),
                                {"key": "value"}).__repr__(), {"key": "value"})
```

### Comparing `opr-210/test/test_recursive.py` & `opr-220/test/test_recursive.py`

 * *Files identical despite different names*

### Comparing `opr-210/test/test_storage.py` & `opr-220/test/test_storage.py`

 * *Files identical despite different names*

