# Comparing `tmp/flet_ivid_hks-1.4.tar.gz` & `tmp/flet_ivid_hks-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_ivid_hks-1.4.tar", last modified: Sat Jun 24 08:19:11 2023, max compression
+gzip compressed data, was "flet_ivid_hks-1.5.tar", last modified: Tue Jul  4 12:58:48 2023, max compression
```

## Comparing `flet_ivid_hks-1.4.tar` & `flet_ivid_hks-1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 08:19:11.644427 flet_ivid_hks-1.4/
--rw-rw-rw-   0        0        0     1081 2023-06-05 11:51:13.000000 flet_ivid_hks-1.4/LICENSE
--rw-rw-rw-   0        0        0       18 2023-06-05 11:51:13.000000 flet_ivid_hks-1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1505 2023-06-24 08:19:11.644427 flet_ivid_hks-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1062 2023-06-08 02:55:17.000000 flet_ivid_hks-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 08:19:11.637427 flet_ivid_hks-1.4/example/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:56:27.000000 flet_ivid_hks-1.4/example/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-06-24 07:54:33.000000 flet_ivid_hks-1.4/example/video_ad.py
--rw-rw-rw-   0        0        0     4070 2023-06-24 07:45:46.000000 flet_ivid_hks-1.4/example/video_grid.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:19:11.639427 flet_ivid_hks-1.4/flet_ivid_hks/
--rw-rw-rw-   0        0        0       88 2023-06-24 08:18:50.000000 flet_ivid_hks-1.4/flet_ivid_hks/__init__.py
--rw-rw-rw-   0        0        0    12897 2023-06-24 07:56:16.000000 flet_ivid_hks-1.4/flet_ivid_hks/clip_container.py
--rw-rw-rw-   0        0        0    12108 2023-06-24 03:23:35.000000 flet_ivid_hks-1.4/flet_ivid_hks/video_container.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:19:11.643426 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/
--rw-rw-rw-   0        0        0     1505 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 11:51:13.000000 flet_ivid_hks-1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 08:19:11.644427 flet_ivid_hks-1.4/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-06-24 08:19:09.000000 flet_ivid_hks-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:58:48.626425 flet_ivid_hks-1.5/
+-rw-rw-rw-   0        0        0     1081 2023-06-05 11:51:13.000000 flet_ivid_hks-1.5/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-06-05 11:51:13.000000 flet_ivid_hks-1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1505 2023-07-04 12:58:48.626425 flet_ivid_hks-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1062 2023-06-08 02:55:17.000000 flet_ivid_hks-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 12:58:48.618425 flet_ivid_hks-1.5/example/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:56:27.000000 flet_ivid_hks-1.5/example/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-06-24 07:54:33.000000 flet_ivid_hks-1.5/example/video_ad.py
+-rw-rw-rw-   0        0        0     4070 2023-06-24 07:45:46.000000 flet_ivid_hks-1.5/example/video_grid.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:58:48.620425 flet_ivid_hks-1.5/flet_ivid_hks/
+-rw-rw-rw-   0        0        0       88 2023-06-24 08:18:50.000000 flet_ivid_hks-1.5/flet_ivid_hks/__init__.py
+-rw-rw-rw-   0        0        0    12815 2023-07-04 12:57:14.000000 flet_ivid_hks-1.5/flet_ivid_hks/clip_container.py
+-rw-rw-rw-   0        0        0    12108 2023-06-24 03:23:35.000000 flet_ivid_hks-1.5/flet_ivid_hks/video_container.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:58:48.625425 flet_ivid_hks-1.5/flet_ivid_hks.egg-info/
+-rw-rw-rw-   0        0        0     1505 2023-07-04 12:58:48.000000 flet_ivid_hks-1.5/flet_ivid_hks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-07-04 12:58:48.000000 flet_ivid_hks-1.5/flet_ivid_hks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 12:58:48.000000 flet_ivid_hks-1.5/flet_ivid_hks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-04 12:58:48.000000 flet_ivid_hks-1.5/flet_ivid_hks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-04 12:58:48.000000 flet_ivid_hks-1.5/flet_ivid_hks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 11:51:13.000000 flet_ivid_hks-1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 12:58:48.626425 flet_ivid_hks-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-07-04 12:58:14.000000 flet_ivid_hks-1.5/setup.py
```

### Comparing `flet_ivid_hks-1.4/LICENSE` & `flet_ivid_hks-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.4/PKG-INFO` & `flet_ivid_hks-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_ivid_hks
-Version: 1.4
+Version: 1.5
 Summary: A package tool that provide basic video player and easy clip for flet.
 Home-page: https://github.com/Uni-Gal/fork-flet_ived
 Author: SKbarbon, Hocassian
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_ivid_hks-1.4/README.md` & `flet_ivid_hks-1.5/README.md`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.4/example/video_ad.py` & `flet_ivid_hks-1.5/example/video_ad.py`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.4/example/video_grid.py` & `flet_ivid_hks-1.5/example/video_grid.py`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.4/flet_ivid_hks/clip_container.py` & `flet_ivid_hks-1.5/flet_ivid_hks/clip_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from flet_core import ClipBehavior, Container
 
 from flet_ivid_hks import VideoContainer
 import flet as ft
 import flet.canvas as cv
 
 
@@ -21,23 +23,16 @@
 def float2gtd(
         dur: float
 ) -> float:
     return round(dur, 4)
 
 
 def indices_for_n_parts(lst, n):
-    """给定一个列表和整数N，输出列表每N个元素的索引"""
-
-    # 确保N不会大于列表长度，如果N大于列表长度，则每个元素都是等分点
     n = min(n, len(lst))
-
-    # 计算每一部分的长度
     step = len(lst) / float(n)
-
-    # 创建一个索引列表，使用round函数来保证索引是整数
     indices = [round(step * i) for i in range(n)]
 
     return indices
 
 
 class ClipContainer(Container):
 
@@ -108,17 +103,18 @@
                 cur_timecode
             ) + "s"
             timecode_st.update()
 
             self.start_time = cur_timecode
 
         def move_left_end(e):
-            print('左边拖拽结束，x=', state.selector_x, 'width=', state.selector_width)
-            print('视频起始点占比=', (state.selector_x + state.circle_radius) / 400)
-            print('视频时长跨度占比=', state.selector_width / 400)
+            # print('左边拖拽结束，x=', state.selector_x, 'width=', state.selector_width)
+            # print('视频起始点占比=', (state.selector_x + state.circle_radius) / 400)
+            # print('视频时长跨度占比=', state.selector_width / 400)
+            pass
 
         def move_right_start(e):
             state.init_local_x = e.local_x
             state.last_x = state.selector_x
             state.last_width = state.selector_width
 
         def move_right_update(e):
@@ -161,17 +157,18 @@
                 cur_timecode
             ) + "s"
             timecode_ed.update()
 
             self.end_time = cur_timecode
 
         def move_right_end(e):
-            print('右边拖拽结束，x=', state.selector_x, 'width=', state.selector_width)
-            print('视频起始点占比=', (state.selector_x + state.circle_radius) / 400)
-            print('视频时长跨度占比=', state.selector_width / 400)
+            # print('右边拖拽结束，x=', state.selector_x, 'width=', state.selector_width)
+            # print('视频起始点占比=', (state.selector_x + state.circle_radius) / 400)
+            # print('视频时长跨度占比=', state.selector_width / 400)
+            pass
 
         bg_paint = ft.Paint(
             style=ft.PaintingStyle.FILL,
             color=ft.colors.with_opacity(0.64, ft.colors.BLUE_800)
         )
 
         stroke_paint = ft.Paint(
@@ -218,15 +215,14 @@
             ],
             width=float("inf"),
             expand=True,
         )
 
         range_selector_left_item = ft.Container(
             left=state.selector_x,
-            # bgcolor=ft.colors.RED,
             width=16,
             height=60,
             expand=False,
             content=cv.Canvas(
                 [
                     cv.Line(
                         state.circle_radius,
@@ -249,15 +245,14 @@
                     on_pan_end=move_left_end,
                 )
             )
         )
 
         range_selector_right_item = ft.Container(
             width=16,
-            # bgcolor=ft.colors.YELLOW,
             height=60,
             expand=False,
             left=state.selector_x + state.selector_width,
             content=cv.Canvas(
                 [
                     cv.Line(state.circle_radius, 0, state.circle_radius, 60, paint=stroke_paint),
                     cv.Circle(state.circle_radius, 30, state.circle_radius, fill_paint),
@@ -279,27 +274,34 @@
                     ft.Image(
                         height=float("inf"),
                         src_base64=self.vc.all_frames_of_video[frame],
                         fit=ft.ImageFit.COVER,
                         expand=True,
                     )
                 )
-            timeline_frames.update()
+
+            try:
+                timeline_frames.update()
+            except Exception as e:
+                pattern = r"control with ID '(.*)' not found"
+                match = re.search(pattern, e.args[0])
+                if not match:
+                    print(e)
+                return
 
             timecode_ed.value = "end：" + str(
                 float2gtd(self.vc.vid_duration)
             ) + "s"
 
             self.end_time = float2gtd(self.vc.vid_duration)
 
             self.content.update()
 
         self.vc = VideoContainer(
             self.video_path,
-            # border_radius=10,
             width=400,
             expand=True,
             play_after_loading=False,
             video_play_button=True,
             exec_after_full_loaded=timeline_frames_update
         )
```

### Comparing `flet_ivid_hks-1.4/flet_ivid_hks/video_container.py` & `flet_ivid_hks-1.5/flet_ivid_hks/video_container.py`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.4/flet_ivid_hks.egg-info/PKG-INFO` & `flet_ivid_hks-1.5/flet_ivid_hks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-ivid-hks
-Version: 1.4
+Version: 1.5
 Summary: A package tool that provide basic video player and easy clip for flet.
 Home-page: https://github.com/Uni-Gal/fork-flet_ived
 Author: SKbarbon, Hocassian
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_ivid_hks-1.4/setup.py` & `flet_ivid_hks-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='flet_ivid_hks',
-    version='1.4',
+    version='1.5',
     author='SKbarbon, Hocassian',
     description='A package tool that provide basic video player and easy clip for flet.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/Uni-Gal/fork-flet_ived',
     install_requires=["flet", "opencv-python"],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"
     ],
-)
+)
```

