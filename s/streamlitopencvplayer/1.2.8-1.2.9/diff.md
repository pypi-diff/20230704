# Comparing `tmp/streamlitopencvplayer-1.2.8.tar.gz` & `tmp/streamlitopencvplayer-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.2.8.tar", last modified: Tue Jul  4 19:03:10 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.2.9.tar", last modified: Tue Jul  4 19:41:58 2023, max compression
```

## Comparing `streamlitopencvplayer-1.2.8.tar` & `streamlitopencvplayer-1.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 19:03:10.941803 streamlitopencvplayer-1.2.8/
--rw-rw-rw-   0        0        0      419 2023-07-04 19:03:10.940226 streamlitopencvplayer-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 19:03:10.941803 streamlitopencvplayer-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-04 19:03:03.000000 streamlitopencvplayer-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:03:10.903248 streamlitopencvplayer-1.2.8/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6776 2023-07-04 19:02:47.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:03:10.926505 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-04 19:03:10.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-04 19:03:10.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 19:03:10.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-04 19:03:10.000000 streamlitopencvplayer-1.2.8/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 19:03:10.934228 streamlitopencvplayer-1.2.8/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.8/test/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-06-23 09:45:03.000000 streamlitopencvplayer-1.2.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:41:58.151104 streamlitopencvplayer-1.2.9/
+-rw-rw-rw-   0        0        0      419 2023-07-04 19:41:58.149104 streamlitopencvplayer-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 19:41:58.151104 streamlitopencvplayer-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-04 19:41:53.000000 streamlitopencvplayer-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:41:58.119466 streamlitopencvplayer-1.2.9/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6636 2023-07-04 19:41:40.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:41:58.137646 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-04 19:41:57.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-04 19:41:57.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 19:41:57.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-04 19:41:57.000000 streamlitopencvplayer-1.2.9/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 19:41:58.144102 streamlitopencvplayer-1.2.9/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.9/test/__init__.py
+-rw-rw-rw-   0        0        0     1690 2023-07-04 19:05:23.000000 streamlitopencvplayer-1.2.9/test/test.py
```

### Comparing `streamlitopencvplayer-1.2.8/README.md` & `streamlitopencvplayer-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.2.8/setup.py` & `streamlitopencvplayer-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.8' 
+VERSION = '1.2.9' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.2.8/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.2.9/streamlitopencvplayer/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 
 # Function to display video in the Streamlit app
 
 def display_video(video_path, json_file):
     # Open the video file
     
-    st.session_state['cap'] = cv2.VideoCapture(video_path)
-    fps = st.session_state['cap'].get(cv2.CAP_PROP_FPS)
+    cap = cv2.VideoCapture(video_path)
+    fps = cap.get(cv2.CAP_PROP_FPS)
     # Opening JSON file and returns JSON object as a dictionnary
     if json_file is not None:
         response = urllib.request.urlopen(json_file)
         fileReader = json.loads(response.read())
         list_ts = []
         list_data = []
 
@@ -103,21 +103,21 @@
         st.session_state['frames'] = []
         resume = False
 
 
         # get all the frames from video when the list is empty
     if not st.session_state['frames']:
         while True:
-            successs, frames = st.session_state['cap'].read()
+            successs, frames = cap.read()
             if successs:
                 frames = cv2.cvtColor(frames, cv2.COLOR_BGR2RGB)
                 st.session_state['frames'].append(frames)
             else:
                 break
-        st.session_state['cap'].release()
+        cap.release()
     # back to the first frame if the video is finished
     if st.session_state['counter'] == len(st.session_state['frames']):
         st.session_state['counter'] = 0
 
     stframe.image(st.session_state['frames']
                   [st.session_state['counter']], caption='', width=450)
     if not resume:
@@ -165,15 +165,15 @@
         pause = container_2.button('▶')
         resume = False
 
 def main():
 
 
     video_path = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989.webm?sp=r&st=2023-07-04T15:19:38Z&se=2023-07-06T23:19:38Z&spr=https&sv=2022-11-02&sr=b&sig=beK2pXlTRKEEPSEQ31sZjkpc%2FPtQU1vpDLUN4gvX2xQ%3D"
-    down_json = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989_global.json?sv=2021-10-04&st=2023-06-22T15%3A00%3A52Z&se=2023-07-23T15%3A00%3A00Z&sr=b&sp=r&sig=mg%2F2tUw06jobBy%2B%2BhBb916akn7BM%2FMVCdYQjsKJidWg%3D"
+    down_json = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441611.4008365.json?se=2023-07-05T19%3A17%3A04Z&sp=r&sv=2021-08-06&sr=b&sig=1IkIpRp%2BVh3DkTKIVjFbvwk0nAApzGi9LiwZTrsq6AA%3D"
     
     if video_path is not None:
         display_video(video_path, down_json)
 
 
 
 if __name__ == "__main__":
```

### Comparing `streamlitopencvplayer-1.2.8/test/test.py` & `streamlitopencvplayer-1.2.9/test/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 if 'alerts' not in st.session_state:
     st.session_state['alerts'] = []
 if 'data' not in st.session_state:
     st.session_state['data'] = []
 if 'alerts_list' not in st.session_state:
     st.session_state['alerts_list'] = []
 if 'name_vid_sel' not in st.session_state:
-    st.session_state['name_vid_sel'] = "1678352121.8713963_1678352127.8713963"
+    st.session_state['name_vid_sel'] = "1687441603.4032989_1687441609.4032989"
 
 class opencvplayer:
     """Class streamlit opencv player."""
 
     def __init__(self, video_path, json_file):
         self.video_path = video_path
         self.json_file = json_file
```

