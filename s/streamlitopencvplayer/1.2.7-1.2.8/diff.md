# Comparing `tmp/streamlitopencvplayer-1.2.7.tar.gz` & `tmp/streamlitopencvplayer-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.2.7.tar", last modified: Tue Jun 20 08:47:01 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.2.8.tar", last modified: Tue Jul  4 19:03:10 2023, max compression
```

## Comparing `streamlitopencvplayer-1.2.7.tar` & `streamlitopencvplayer-1.2.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:47:01.872329 streamlitopencvplayer-1.2.7/
--rw-rw-rw-   0        0        0      419 2023-06-20 08:47:01.870329 streamlitopencvplayer-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 08:47:01.873326 streamlitopencvplayer-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-06-20 08:46:58.000000 streamlitopencvplayer-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:47:01.841327 streamlitopencvplayer-1.2.7/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6565 2023-06-20 00:38:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:47:01.857329 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-20 08:47:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-06-20 08:47:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:47:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-20 08:47:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 08:47:01.866325 streamlitopencvplayer-1.2.7/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.7/test/__init__.py
--rw-rw-rw-   0        0        0     2200 2023-06-20 00:01:41.000000 streamlitopencvplayer-1.2.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:03:10.941803 streamlitopencvplayer-1.2.8/
+-rw-rw-rw-   0        0        0      419 2023-07-04 19:03:10.940226 streamlitopencvplayer-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 19:03:10.941803 streamlitopencvplayer-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-04 19:03:03.000000 streamlitopencvplayer-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:03:10.903248 streamlitopencvplayer-1.2.8/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6776 2023-07-04 19:02:47.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:03:10.926505 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-04 19:03:10.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-04 19:03:10.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 19:03:10.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-04 19:03:10.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 19:03:10.934228 streamlitopencvplayer-1.2.8/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.8/test/__init__.py
+-rw-rw-rw-   0        0        0     1690 2023-06-23 09:45:03.000000 streamlitopencvplayer-1.2.8/test/test.py
```

### Comparing `streamlitopencvplayer-1.2.7/README.md` & `streamlitopencvplayer-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.2.7/setup.py` & `streamlitopencvplayer-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.7' 
+VERSION = '1.2.8' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.2.7/test/test.py` & `streamlitopencvplayer-1.2.8/test/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,28 +25,20 @@
     """Class streamlit opencv player."""
 
     def __init__(self, video_path, json_file):
         self.video_path = video_path
         self.json_file = json_file
 
 
-    #@st.cache_data()
     def main(self):
         """Test function.
 
         Args:
             video_path (required): video file path or video url.
-            alerts_dict (Optional) : Dictionary of alerts passed to the alerts table.
-            alerts (Required when data is used) : List of alerts time
-            data (Optional) : bounding box coordinates, score and class
-            This is an example for test :
-                self.alerts_dict = {"Alerts": [43, 64]}
-                self.alerts = [43, 64]
-                self.data = [[[10, 100, 290, 200], 0.82, 0, "Class 0"],
-                        [[55, 22, 100, 120], 0.9, 1, "Class 1"]]
+            json_file
 
         Returns:
             The video Player.
         """
         if self.video_path is not None:
             return display_video(self.video_path, self.json_file)
```

