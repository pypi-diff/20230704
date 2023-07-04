# Comparing `tmp/SC-Track-0.0.2.tar.gz` & `tmp/SC-Track-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SC-Track-0.0.2.tar", last modified: Tue Jul  4 08:42:52 2023, max compression
+gzip compressed data, was "SC-Track-0.0.3.tar", last modified: Tue Jul  4 08:52:53 2023, max compression
```

## Comparing `SC-Track-0.0.2.tar` & `SC-Track-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:52.416952 SC-Track-0.0.2/
--rw-rw-rw-   0        0        0    35821 2023-07-03 22:48:32.000000 SC-Track-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4326 2023-07-04 08:42:52.416952 SC-Track-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:52.405942 SC-Track-0.0.2/SCTrack/
--rw-rw-rw-   0        0        0      179 2023-07-04 08:35:35.000000 SC-Track-0.0.2/SCTrack/__init__.py
--rw-rw-rw-   0        0        0    27194 2023-07-04 04:54:52.000000 SC-Track-0.0.2/SCTrack/base.py
--rw-rw-rw-   0        0        0      261 2023-07-03 20:41:40.000000 SC-Track-0.0.2/SCTrack/config.py
--rw-rw-rw-   0        0        0    15056 2023-07-04 04:56:48.000000 SC-Track-0.0.2/SCTrack/feature.py
--rw-rw-rw-   0        0        0     9503 2023-07-04 04:29:49.000000 SC-Track-0.0.2/SCTrack/generate_tracking_stack.py
--rw-rw-rw-   0        0        0     3711 2023-07-04 04:47:49.000000 SC-Track-0.0.2/SCTrack/prepare.py
--rw-rw-rw-   0        0        0    24000 2023-07-04 08:24:51.000000 SC-Track-0.0.2/SCTrack/reclassification.py
--rw-rw-rw-   0        0        0     3542 2023-07-04 08:34:28.000000 SC-Track-0.0.2/SCTrack/sctrack.py
--rw-rw-rw-   0        0        0     1666 2023-05-13 09:06:34.000000 SC-Track-0.0.2/SCTrack/t_error.py
--rw-rw-rw-   0        0        0      559 2023-06-30 14:38:42.000000 SC-Track-0.0.2/SCTrack/template.py
--rw-rw-rw-   0        0        0     1905 2023-07-04 04:29:49.000000 SC-Track-0.0.2/SCTrack/track.py
--rw-rw-rw-   0        0        0    54458 2023-07-04 04:39:08.000000 SC-Track-0.0.2/SCTrack/tracker.py
--rw-rw-rw-   0        0        0     7472 2023-07-04 05:21:39.000000 SC-Track-0.0.2/SCTrack/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:52.415950 SC-Track-0.0.2/SC_Track.egg-info/
--rw-rw-rw-   0        0        0     4326 2023-07-04 08:42:52.000000 SC-Track-0.0.2/SC_Track.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-07-04 08:42:52.000000 SC-Track-0.0.2/SC_Track.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:42:52.000000 SC-Track-0.0.2/SC_Track.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-04 08:42:52.000000 SC-Track-0.0.2/SC_Track.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-04 05:53:23.000000 SC-Track-0.0.2/SC_Track.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      314 2023-07-04 08:42:52.000000 SC-Track-0.0.2/SC_Track.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 08:42:52.000000 SC-Track-0.0.2/SC_Track.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 08:42:52.416952 SC-Track-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      990 2023-07-04 08:42:13.000000 SC-Track-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:52:53.042950 SC-Track-0.0.3/
+-rw-rw-rw-   0        0        0    35821 2023-07-03 22:48:32.000000 SC-Track-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4326 2023-07-04 08:52:53.042950 SC-Track-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 08:52:53.025936 SC-Track-0.0.3/SCTrack/
+-rw-rw-rw-   0        0        0      179 2023-07-04 08:35:35.000000 SC-Track-0.0.3/SCTrack/__init__.py
+-rw-rw-rw-   0        0        0    27194 2023-07-04 04:54:52.000000 SC-Track-0.0.3/SCTrack/base.py
+-rw-rw-rw-   0        0        0      261 2023-07-03 20:41:40.000000 SC-Track-0.0.3/SCTrack/config.py
+-rw-rw-rw-   0        0        0    15056 2023-07-04 04:56:48.000000 SC-Track-0.0.3/SCTrack/feature.py
+-rw-rw-rw-   0        0        0     9503 2023-07-04 04:29:49.000000 SC-Track-0.0.3/SCTrack/generate_tracking_stack.py
+-rw-rw-rw-   0        0        0     3711 2023-07-04 04:47:49.000000 SC-Track-0.0.3/SCTrack/prepare.py
+-rw-rw-rw-   0        0        0    24004 2023-07-04 08:48:54.000000 SC-Track-0.0.3/SCTrack/reclassification.py
+-rw-rw-rw-   0        0        0     3542 2023-07-04 08:51:09.000000 SC-Track-0.0.3/SCTrack/sctrack.py
+-rw-rw-rw-   0        0        0     1666 2023-05-13 09:06:34.000000 SC-Track-0.0.3/SCTrack/t_error.py
+-rw-rw-rw-   0        0        0      559 2023-06-30 14:38:42.000000 SC-Track-0.0.3/SCTrack/template.py
+-rw-rw-rw-   0        0        0     1905 2023-07-04 04:29:49.000000 SC-Track-0.0.3/SCTrack/track.py
+-rw-rw-rw-   0        0        0    54458 2023-07-04 04:39:08.000000 SC-Track-0.0.3/SCTrack/tracker.py
+-rw-rw-rw-   0        0        0     7472 2023-07-04 05:21:39.000000 SC-Track-0.0.3/SCTrack/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:52:53.041951 SC-Track-0.0.3/SC_Track.egg-info/
+-rw-rw-rw-   0        0        0     4326 2023-07-04 08:52:52.000000 SC-Track-0.0.3/SC_Track.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-07-04 08:52:52.000000 SC-Track-0.0.3/SC_Track.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:52:52.000000 SC-Track-0.0.3/SC_Track.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-04 08:52:52.000000 SC-Track-0.0.3/SC_Track.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-04 05:53:23.000000 SC-Track-0.0.3/SC_Track.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      314 2023-07-04 08:52:52.000000 SC-Track-0.0.3/SC_Track.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 08:52:52.000000 SC-Track-0.0.3/SC_Track.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 08:52:53.042950 SC-Track-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-07-04 08:52:16.000000 SC-Track-0.0.3/setup.py
```

### Comparing `SC-Track-0.0.2/LICENSE` & `SC-Track-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/PKG-INFO` & `SC-Track-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC-Track
-Version: 0.0.2
+Version: 0.0.3
 Summary: single cell tracking package
 Home-page: https://github.com/frozenleaves/SC-Track
 Author: Li Chengxin
 Author-email: 914814442@qq.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `SC-Track-0.0.2/SCTrack/base.py` & `SC-Track-0.0.3/SCTrack/base.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SCTrack/feature.py` & `SC-Track-0.0.3/SCTrack/feature.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SCTrack/generate_tracking_stack.py` & `SC-Track-0.0.3/SCTrack/generate_tracking_stack.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SCTrack/prepare.py` & `SC-Track-0.0.3/SCTrack/prepare.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SCTrack/reclassification.py` & `SC-Track-0.0.3/SCTrack/reclassification.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List
 import json
 import random
 import pickle
 import pandas as pd
 from SCTrack.base import Cell
 from SCTrack.tracker import Tracker, CellNode, TrackingTree
+from SCTrack.config import RAW_INPUT_IMAGE_SIZE
 
 
 class TreeParser(object):
     """parse TrackingTree"""
 
     def __init__(self, track_tree: TrackingTree):
         self.tree = track_tree
@@ -444,15 +445,14 @@
                 track_detail_dataframe = track_detail_dataframe._append(series, ignore_index=True)
     fname = filepath
     track_detail_dataframe.to_csv(fname, index=False)
 
 
 def track_trees_to_json(tracker: Tracker, output_fname, xrange, basename=None):
     """Export track result to json file"""
-    from config import RAW_INPUT_IMAGE_SIZE
     if basename is None:
         prefix = 'mcy'
     else:
         prefix = basename
 
     def update_region(node):
         # print(type(node))
```

### Comparing `SC-Track-0.0.2/SCTrack/sctrack.py` & `SC-Track-0.0.3/SCTrack/sctrack.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import sys
 import time
 import imagesize
 from SCTrack import track
 
 
 def main():
-    logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", datefmt="%Y-%M-%d %H:%M:%S",
+    logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", datefmt="%Y-%m-%d %H:%M:%S",
                         level=logging.INFO)
 
     parser = argparse.ArgumentParser(description="", add_help=False)
     help_content = """
         Welcome to use SC-Track!
         using this script to auto tracking the single cell images and identify each cell's type.\n
         usage:
```

### Comparing `SC-Track-0.0.2/SCTrack/t_error.py` & `SC-Track-0.0.3/SCTrack/t_error.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SCTrack/template.py` & `SC-Track-0.0.3/SCTrack/template.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SCTrack/track.py` & `SC-Track-0.0.3/SCTrack/track.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SCTrack/tracker.py` & `SC-Track-0.0.3/SCTrack/tracker.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SCTrack/utils.py` & `SC-Track-0.0.3/SCTrack/utils.py`

 * *Files identical despite different names*

### Comparing `SC-Track-0.0.2/SC_Track.egg-info/PKG-INFO` & `SC-Track-0.0.3/SC_Track.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC-Track
-Version: 0.0.2
+Version: 0.0.3
 Summary: single cell tracking package
 Home-page: https://github.com/frozenleaves/SC-Track
 Author: Li Chengxin
 Author-email: 914814442@qq.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `SC-Track-0.0.2/setup.py` & `SC-Track-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open('readme.md', 'r') as f:
     long_description = f.read()
 
 with open('requirements.txt', 'r') as fr:
     pkg_requirements = fr.read().split('\n')
     pkg_requirements.remove('')
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 setuptools.setup(
     name='SC-Track',  # package name
     author="Li Chengxin",
     author_email="914814442@qq.com",
     url="https://github.com/frozenleaves/SC-Track",
     version=VERSION,  # package version
```

