# Comparing `tmp/bilibili_up-1.1.0.0.tar.gz` & `tmp/bilibili_up-1.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bilibili_up-1.1.0.0.tar", last modified: Tue Jul  4 07:18:49 2023, max compression
+gzip compressed data, was "dist\bilibili_up-1.1.0.1.tar", last modified: Tue Jul  4 07:23:06 2023, max compression
```

## Comparing `bilibili_up-1.1.0.0.tar` & `bilibili_up-1.1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/
--rw-rw-rw-   0        0        0     3675 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2710 2023-07-04 07:18:29.000000 bilibili_up-1.1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up/
--rw-rw-rw-   0        0        0     4109 2023-07-04 07:13:40.000000 bilibili_up-1.1.0.0/bilibili_up/BV.py
--rw-rw-rw-   0        0        0       28 2023-07-04 07:13:21.000000 bilibili_up-1.1.0.0/bilibili_up/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/
--rw-rw-rw-   0        0        0     3675 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-07-04 07:18:29.000000 bilibili_up-1.1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/
+-rw-rw-rw-   0        0        0     3776 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2779 2023-07-04 07:23:01.000000 bilibili_up-1.1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/bilibili_up/
+-rw-rw-rw-   0        0        0     4109 2023-07-04 07:13:40.000000 bilibili_up-1.1.0.1/bilibili_up/BV.py
+-rw-rw-rw-   0        0        0       28 2023-07-04 07:13:21.000000 bilibili_up-1.1.0.1/bilibili_up/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/bilibili_up.egg-info/
+-rw-rw-rw-   0        0        0     3776 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/bilibili_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/bilibili_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/bilibili_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/bilibili_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/bilibili_up.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 07:23:06.000000 bilibili_up-1.1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-04 07:23:01.000000 bilibili_up-1.1.0.1/setup.py
```

### Comparing `bilibili_up-1.1.0.0/PKG-INFO` & `bilibili_up-1.1.0.1/bilibili_up.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bilibili_up
-Version: 1.1.0.0
+Name: bilibili-up
+Version: 1.1.0.1
 Summary: bilibili_up获取bilibili视频信息的爬虫！
 Home-page: https://pypi.org/user/SuiBo/
 Author: SuiBo
 Author-email: 534047068@qq.com
 License: UNKNOWN
 Description: # Bilibili_up 使用方法
         ****
@@ -85,10 +85,14 @@
         >请确保提供的 BV 号是有效的，对应的视频存在并且具有弹幕。
         ****
         >在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（已过时）
         ****
         ### 1.0.0.0 正式版本更新
         
         >支持选择ip<br>
-        >增加了BV_get_File函数的多个选项
+        >增加了BV_get_File函数的多个选项<br>
+        ****
+        ### 1.1.0.0 正式版本更新
+        
+        >支持获取弹幕<br>
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `bilibili_up-1.1.0.0/README.md` & `bilibili_up-1.1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -77,8 +77,12 @@
 >请确保提供的 BV 号是有效的，对应的视频存在并且具有弹幕。
 ****
 >在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（已过时）
 ****
 ### 1.0.0.0 正式版本更新
 
 >支持选择ip<br>
->增加了BV_get_File函数的多个选项
+>增加了BV_get_File函数的多个选项<br>
+****
+### 1.1.0.0 正式版本更新
+
+>支持获取弹幕<br>
```

### Comparing `bilibili_up-1.1.0.0/bilibili_up/BV.py` & `bilibili_up-1.1.0.1/bilibili_up/BV.py`

 * *Files identical despite different names*

### Comparing `bilibili_up-1.1.0.0/bilibili_up.egg-info/PKG-INFO` & `bilibili_up-1.1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bilibili-up
-Version: 1.1.0.0
+Name: bilibili_up
+Version: 1.1.0.1
 Summary: bilibili_up获取bilibili视频信息的爬虫！
 Home-page: https://pypi.org/user/SuiBo/
 Author: SuiBo
 Author-email: 534047068@qq.com
 License: UNKNOWN
 Description: # Bilibili_up 使用方法
         ****
@@ -85,10 +85,14 @@
         >请确保提供的 BV 号是有效的，对应的视频存在并且具有弹幕。
         ****
         >在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（已过时）
         ****
         ### 1.0.0.0 正式版本更新
         
         >支持选择ip<br>
-        >增加了BV_get_File函数的多个选项
+        >增加了BV_get_File函数的多个选项<br>
+        ****
+        ### 1.1.0.0 正式版本更新
+        
+        >支持获取弹幕<br>
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `bilibili_up-1.1.0.0/setup.py` & `bilibili_up-1.1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='bilibili_up',
-    version='1.1.0.0',
+    version='1.1.0.1',
     author='SuiBo',
     author_email='534047068@qq.com',
     description='bilibili_up获取bilibili视频信息的爬虫！',
     install_requires=[
         'requests',
         'json',
     ],
```

