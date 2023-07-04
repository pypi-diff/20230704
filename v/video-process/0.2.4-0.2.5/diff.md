# Comparing `tmp/video_process-0.2.4.tar.gz` & `tmp/video_process-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_process-0.2.4.tar", max compression
+gzip compressed data, was "video_process-0.2.5.tar", max compression
```

## Comparing `video_process-0.2.4.tar` & `video_process-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      453 2023-07-03 08:39:18.432091 video_process-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      167 2023-07-03 08:37:18.348712 video_process-0.2.4/video_process/__init__.py
--rw-r--r--   0        0        0     5517 2023-06-29 03:51:51.970247 video_process-0.2.4/video_process/graph_builder.py
--rwxr-xr-x   0        0        0     1464 2023-06-29 06:24:47.835149 video_process-0.2.4/video_process/index.py
--rw-r--r--   0        0        0     1741 2023-07-03 08:37:13.109063 video_process-0.2.4/video_process/lib.py
--rw-r--r--   0        0        0     1134 2023-06-28 08:59:43.686218 video_process-0.2.4/video_process/subtitle.py
--rw-r--r--   0        0        0     4074 2023-07-03 07:20:37.997715 video_process-0.2.4/video_process/utils.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      453 2023-07-04 02:56:23.242439 video_process-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-07-03 08:37:18.348712 video_process-0.2.5/video_process/__init__.py
+-rw-r--r--   0        0        0     5517 2023-06-29 03:51:51.970247 video_process-0.2.5/video_process/graph_builder.py
+-rwxr-xr-x   0        0        0     1464 2023-06-29 06:24:47.835149 video_process-0.2.5/video_process/index.py
+-rw-r--r--   0        0        0     1741 2023-07-03 08:37:13.109063 video_process-0.2.5/video_process/lib.py
+-rw-r--r--   0        0        0     1134 2023-06-28 08:59:43.686218 video_process-0.2.5/video_process/subtitle.py
+-rw-r--r--   0        0        0     4076 2023-07-04 02:48:38.881180 video_process-0.2.5/video_process/utils.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.2.5/PKG-INFO
```

### Comparing `video_process-0.2.4/video_process/graph_builder.py` & `video_process-0.2.5/video_process/graph_builder.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.4/video_process/index.py` & `video_process-0.2.5/video_process/index.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.4/video_process/lib.py` & `video_process-0.2.5/video_process/lib.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.4/video_process/subtitle.py` & `video_process-0.2.5/video_process/subtitle.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.4/video_process/utils.py` & `video_process-0.2.5/video_process/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     data["video_path"] = video_path
 
     if data.get("enable_bg"):
         bg = data["bg"]
         if bg["bg_type"] == "video" and bg.get("bg_video_url"):
             video_url = bg["bg_video_url"]
             extension = get_file_extension(video_url)
-            video_path = os.path.join(base_dir, "bg_video{extension}")
+            video_path = os.path.join(base_dir, f"bg_video{extension}")
             download_file(video_url, video_path)
             bg["bg_video_path"] = video_path
         elif bg["bg_type"] == "image" and bg.get("bg_image_url"):
             image_url = bg["bg_image_url"]
             extension = get_file_extension(image_url)
-            image_path = os.path.join(base_dir, "bg_image{extension}")
+            image_path = os.path.join(base_dir, f"bg_image{extension}")
             download_file(image_url, image_path)
             bg["bg_image_path"] = image_path
 
     # 处理背景音乐字段
     if data.get("enable_bgm"):
         bg_music = data["bgm"]
         if bg_music.get("bgm_url"):
```

