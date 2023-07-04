# Comparing `tmp/showroom-recorder-0.6.6.tar.gz` & `tmp/showroom-recorder-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.6.6.tar", last modified: Thu Jun 29 16:46:44 2023, max compression
+gzip compressed data, was "showroom-recorder-0.6.7.tar", last modified: Tue Jul  4 11:22:52 2023, max compression
```

## Comparing `showroom-recorder-0.6.6.tar` & `showroom-recorder-0.6.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)    35149 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/LICENSE
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       53 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/MANIFEST.in
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     1307 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/PKG-INFO
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     1394 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/README.md
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      964 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/description.md
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       38 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/setup.cfg
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     1175 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/setup.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      562 2023-06-27 14:38:51.000000 showroom-recorder-0.6.6/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.512138 showroom-recorder-0.6.6/src/
-drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.512138 showroom-recorder-0.6.6/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       48 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      185 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     3497 2023-06-27 14:38:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)        0 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)    31904 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     2973 2023-06-29 16:38:34.000000 showroom-recorder-0.6.6/src/showroom_recorder/processor/uploader.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     9677 2023-06-29 16:35:11.000000 showroom-recorder-0.6.6/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)        0 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     5538 2023-06-29 16:35:28.000000 showroom-recorder-0.6.6/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)    16581 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       46 2023-06-29 16:40:29.000000 showroom-recorder-0.6.6/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.512138 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     1307 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      835 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)        1 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       71 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       66 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       18 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)        1 2023-06-26 14:12:42.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/zip-safe
-drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/test/
--rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      424 2023-06-27 14:38:51.000000 showroom-recorder-0.6.6/test/test_config.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-07-04 11:22:52.849945 showroom-recorder-0.6.7/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/LICENSE
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-07-04 11:22:52.849945 showroom-recorder-0.6.7/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/description.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-07-04 11:22:52.849945 showroom-recorder-0.6.7/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      562 2023-06-27 12:42:56.000000 showroom-recorder-0.6.7/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-07-04 11:22:52.833945 showroom-recorder-0.6.7/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-07-04 11:22:52.849945 showroom-recorder-0.6.7/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-27 14:29:02.000000 showroom-recorder-0.6.7/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3497 2023-06-27 14:25:32.000000 showroom-recorder-0.6.7/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-07-04 11:22:52.849945 showroom-recorder-0.6.7/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31981 2023-07-04 11:19:40.000000 showroom-recorder-0.6.7/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     2973 2023-06-29 16:52:47.000000 showroom-recorder-0.6.7/src/showroom_recorder/processor/uploader.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     9677 2023-06-29 16:52:47.000000 showroom-recorder-0.6.7/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-07-04 11:22:52.849945 showroom-recorder-0.6.7/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     5538 2023-06-29 16:52:47.000000 showroom-recorder-0.6.7/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.7/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-07-04 11:20:39.000000 showroom-recorder-0.6.7/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-07-04 11:22:52.849945 showroom-recorder-0.6.7/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-07-04 11:22:52.000000 showroom-recorder-0.6.7/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      835 2023-07-04 11:22:52.000000 showroom-recorder-0.6.7/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-07-04 11:22:52.000000 showroom-recorder-0.6.7/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-07-04 11:22:52.000000 showroom-recorder-0.6.7/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       66 2023-07-04 11:22:52.000000 showroom-recorder-0.6.7/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-07-04 11:22:52.000000 showroom-recorder-0.6.7/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.7/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-07-04 11:22:52.849945 showroom-recorder-0.6.7/test/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      424 2023-06-27 14:26:00.000000 showroom-recorder-0.6.7/test/test_config.py
```

### Comparing `showroom-recorder-0.6.6/LICENSE` & `showroom-recorder-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/PKG-INFO` & `showroom-recorder-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.6
+Version: 0.6.7
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.6/README.md` & `showroom-recorder-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/description.md` & `showroom-recorder-0.6.7/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/setup.py` & `showroom-recorder-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/showroom-recorder.json` & `showroom-recorder-0.6.7/showroom-recorder.json`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/src/showroom_recorder/common.py` & `showroom-recorder-0.6.7/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.6.7/src/showroom_recorder/processor/danmaku.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import datetime
 import threading
 import json
 import math
 import random
 import logging
 import logging.handlers
+import csv
 
 from json import JSONDecodeError
 from argparse import ArgumentParser
 from ..utils import delete_emoji
 # requirements.txt
 import pytz
 import requests
@@ -427,14 +428,17 @@
                     # print(s2.isdecimal())  # False
                     # int(s1)  # ValueError
                     # int(s2)  # ValueError
                     pass
                 else:
                     # replace line break to a space
                     comment = comment.replace('\n', ' ')
+
+                    comment = '[' + data['ac'] + '] ' + comment
+
                     if self.settings['program_settings']['show_comments'] > 0:
                         logging.info('{}: {}'.format(
                             self.room_url_key, comment))
 
                     if self.comment_output_func is not None:
                         self.comment_output_func(comment)
```

### Comparing `showroom-recorder-0.6.6/src/showroom_recorder/processor/uploader.py` & `showroom-recorder-0.6.7/src/showroom_recorder/processor/uploader.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.6.7/src/showroom_recorder/processor/video.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.6.7/src/showroom_recorder/utils/config.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.6.7/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.6/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.6.7/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.6
+Version: 0.6.7
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.6/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.6.7/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

