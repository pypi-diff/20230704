# Comparing `tmp/streamlitopencvplayer-1.2.9.tar.gz` & `tmp/streamlitopencvplayer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.2.9.tar", last modified: Tue Jul  4 19:41:58 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.3.0.tar", last modified: Tue Jul  4 19:46:25 2023, max compression
```

## Comparing `streamlitopencvplayer-1.2.9.tar` & `streamlitopencvplayer-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 19:41:58.151104 streamlitopencvplayer-1.2.9/
--rw-rw-rw-   0        0        0      419 2023-07-04 19:41:58.149104 streamlitopencvplayer-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 19:41:58.151104 streamlitopencvplayer-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-04 19:41:53.000000 streamlitopencvplayer-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:41:58.119466 streamlitopencvplayer-1.2.9/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6636 2023-07-04 19:41:40.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:41:58.137646 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-04 19:41:57.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-04 19:41:57.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 19:41:57.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-04 19:41:57.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 19:41:58.144102 streamlitopencvplayer-1.2.9/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.9/test/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-07-04 19:05:23.000000 streamlitopencvplayer-1.2.9/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:46:25.791895 streamlitopencvplayer-1.3.0/
+-rw-rw-rw-   0        0        0      419 2023-07-04 19:46:25.789895 streamlitopencvplayer-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 19:46:25.792898 streamlitopencvplayer-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-04 19:46:21.000000 streamlitopencvplayer-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:46:25.761120 streamlitopencvplayer-1.3.0/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.0/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6514 2023-07-04 19:45:11.000000 streamlitopencvplayer-1.3.0/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:46:25.779783 streamlitopencvplayer-1.3.0/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-04 19:46:25.000000 streamlitopencvplayer-1.3.0/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-04 19:46:25.000000 streamlitopencvplayer-1.3.0/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 19:46:25.000000 streamlitopencvplayer-1.3.0/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-04 19:46:25.000000 streamlitopencvplayer-1.3.0/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 19:46:25.786343 streamlitopencvplayer-1.3.0/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1690 2023-07-04 19:05:23.000000 streamlitopencvplayer-1.3.0/test/test.py
```

### Comparing `streamlitopencvplayer-1.2.9/README.md` & `streamlitopencvplayer-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.2.9/setup.py` & `streamlitopencvplayer-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.9' 
+VERSION = '1.3.0' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.2.9/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.3.0/streamlitopencvplayer/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     st.session_state['frames'] = []
 if 'alerts' not in st.session_state:
     st.session_state['alerts'] = []
 if 'data' not in st.session_state:
     st.session_state['data'] = []
 if 'alerts_list' not in st.session_state:
     st.session_state['alerts_list'] = []
-if 'name_vid_sel' not in st.session_state:
-    st.session_state['name_vid_sel'] = "1687441603.4032989_1687441609.4032989"
+
 
 
 # Function to display video in the Streamlit app
 
 def display_video(video_path, json_file):
     # Open the video file
```

### Comparing `streamlitopencvplayer-1.2.9/test/test.py` & `streamlitopencvplayer-1.3.0/test/test.py`

 * *Files identical despite different names*

