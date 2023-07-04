# Comparing `tmp/bilibili_up-1.2.0.0.tar.gz` & `tmp/bilibili_up-2.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bilibili_up-1.2.0.0.tar", last modified: Tue Jul  4 07:26:50 2023, max compression
+gzip compressed data, was "dist\bilibili_up-2.0.0.0.tar", last modified: Tue Jul  4 07:41:32 2023, max compression
```

## Comparing `bilibili_up-1.2.0.0.tar` & `bilibili_up-2.0.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/
--rw-rw-rw-   0        0        0     3872 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2851 2023-07-04 07:26:42.000000 bilibili_up-1.2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/bilibili_up/
--rw-rw-rw-   0        0        0     4109 2023-07-04 07:13:40.000000 bilibili_up-1.2.0.0/bilibili_up/BV.py
--rw-rw-rw-   0        0        0       28 2023-07-04 07:13:21.000000 bilibili_up-1.2.0.0/bilibili_up/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/bilibili_up.egg-info/
--rw-rw-rw-   0        0        0     3872 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/bilibili_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/bilibili_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/bilibili_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/bilibili_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/bilibili_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 07:26:50.000000 bilibili_up-1.2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      574 2023-07-04 07:26:42.000000 bilibili_up-1.2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/
+-rw-rw-rw-   0        0        0     4189 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3128 2023-07-04 07:41:18.000000 bilibili_up-2.0.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/bilibili_up/
+-rw-rw-rw-   0        0        0     4090 2023-07-04 07:40:05.000000 bilibili_up-2.0.0.0/bilibili_up/AV.py
+-rw-rw-rw-   0        0        0     4109 2023-07-04 07:13:40.000000 bilibili_up-2.0.0.0/bilibili_up/BV.py
+-rw-rw-rw-   0        0        0       28 2023-07-04 07:13:21.000000 bilibili_up-2.0.0.0/bilibili_up/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/bilibili_up.egg-info/
+-rw-rw-rw-   0        0        0     4189 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/bilibili_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/bilibili_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/bilibili_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/bilibili_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/bilibili_up.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 07:41:32.000000 bilibili_up-2.0.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      574 2023-07-04 07:40:05.000000 bilibili_up-2.0.0.0/setup.py
```

### Comparing `bilibili_up-1.2.0.0/PKG-INFO` & `bilibili_up-2.0.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: bilibili_up
-Version: 1.2.0.0
+Version: 2.0.0.0
 Summary: bilibili_up获取bilibili视频信息的爬虫！
 Home-page: https://pypi.org/user/SuiBo/
 Author: SuiBo
 Author-email: 534047068@qq.com
 License: UNKNOWN
 Description: # Bilibili_up 使用方法
         ****
+        >如果程序错了（特别是av号的操作和ip），请报告给534047068@qq.com。
         ### 关于 BV 号视频的操作<br><br>
-        **导入BV操作**<br>
+        **导入BV操作(av号也一样)**<br>
         获取BV视频评论区（字典）<br>
         ```ruby
-        from bilibili_up import BV
+        from bilibili_up import BV # BV 号
+        from bilibili_up import AV # av 号
         ```
         ```ruby
         #获取BV视频评论区（字典）
         comments = BV_get_comments(BV=123456789, 
                    PageNumber=5, 
                    headers={"User-Agent": "Mozilla/5.0"})
         for username, content in comments.items():
@@ -43,14 +45,15 @@
                         "发布时间": publish_time,
                         "作者": {
                             "名称": author_name,
                             "UID": author_uid
                         },
                         "弹幕数量": danmaku_count,
                         "bvid": video_data['bvid'],  # 视频BV号
+                        # av号是"avid"
                         "援助": video_data['aid'],  # 视频援助号
                         "视频tid": video_data['tid'],  # 视频tid
                         "tname": video_data['tname'],  # 视频分类名
                         "版权": video_data['rights'],  # 版权信息
                         "封面图片": video_data['pic'],  # 封面图片链接
                         "title": video_data['title']  # 视频标题
                     }
@@ -91,11 +94,13 @@
         >支持选择ip<br>
         >增加了BV_get_File函数的多个选项<br>
         ****
         ### 1.1.0.0 正式版本更新
         >支持获取弹幕<br>
         ****
         ### 1.2.0.0 正式版本修复
-        
         >取消了不必要的错误<br>
+        ****
+        ### 2.0.0.0 正式版本更新
+        >增加了av号的操作！和BV号同步更新！<br>
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `bilibili_up-1.2.0.0/README.md` & `bilibili_up-2.0.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Bilibili_up 使用方法
 ****
+>如果程序错了（特别是av号的操作和ip），请报告给534047068@qq.com。
 ### 关于 BV 号视频的操作<br><br>
-**导入BV操作**<br>
+**导入BV操作(av号也一样)**<br>
 获取BV视频评论区（字典）<br>
 ```ruby
-from bilibili_up import BV
+from bilibili_up import BV # BV 号
+from bilibili_up import AV # av 号
 ```
 ```ruby
 #获取BV视频评论区（字典）
 comments = BV_get_comments(BV=123456789, 
            PageNumber=5, 
            headers={"User-Agent": "Mozilla/5.0"})
 for username, content in comments.items():
@@ -35,14 +37,15 @@
                 "发布时间": publish_time,
                 "作者": {
                     "名称": author_name,
                     "UID": author_uid
                 },
                 "弹幕数量": danmaku_count,
                 "bvid": video_data['bvid'],  # 视频BV号
+                # av号是"avid"
                 "援助": video_data['aid'],  # 视频援助号
                 "视频tid": video_data['tid'],  # 视频tid
                 "tname": video_data['tname'],  # 视频分类名
                 "版权": video_data['rights'],  # 版权信息
                 "封面图片": video_data['pic'],  # 封面图片链接
                 "title": video_data['title']  # 视频标题
             }
@@ -83,9 +86,11 @@
 >支持选择ip<br>
 >增加了BV_get_File函数的多个选项<br>
 ****
 ### 1.1.0.0 正式版本更新
 >支持获取弹幕<br>
 ****
 ### 1.2.0.0 正式版本修复
-
->取消了不必要的错误<br>
+>取消了不必要的错误<br>
+****
+### 2.0.0.0 正式版本更新
+>增加了av号的操作！和BV号同步更新！<br>
```

### Comparing `bilibili_up-1.2.0.0/bilibili_up/BV.py` & `bilibili_up-2.0.0.0/bilibili_up/BV.py`

 * *Files identical despite different names*

### Comparing `bilibili_up-1.2.0.0/bilibili_up.egg-info/PKG-INFO` & `bilibili_up-2.0.0.0/bilibili_up.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: bilibili-up
-Version: 1.2.0.0
+Version: 2.0.0.0
 Summary: bilibili_up获取bilibili视频信息的爬虫！
 Home-page: https://pypi.org/user/SuiBo/
 Author: SuiBo
 Author-email: 534047068@qq.com
 License: UNKNOWN
 Description: # Bilibili_up 使用方法
         ****
+        >如果程序错了（特别是av号的操作和ip），请报告给534047068@qq.com。
         ### 关于 BV 号视频的操作<br><br>
-        **导入BV操作**<br>
+        **导入BV操作(av号也一样)**<br>
         获取BV视频评论区（字典）<br>
         ```ruby
-        from bilibili_up import BV
+        from bilibili_up import BV # BV 号
+        from bilibili_up import AV # av 号
         ```
         ```ruby
         #获取BV视频评论区（字典）
         comments = BV_get_comments(BV=123456789, 
                    PageNumber=5, 
                    headers={"User-Agent": "Mozilla/5.0"})
         for username, content in comments.items():
@@ -43,14 +45,15 @@
                         "发布时间": publish_time,
                         "作者": {
                             "名称": author_name,
                             "UID": author_uid
                         },
                         "弹幕数量": danmaku_count,
                         "bvid": video_data['bvid'],  # 视频BV号
+                        # av号是"avid"
                         "援助": video_data['aid'],  # 视频援助号
                         "视频tid": video_data['tid'],  # 视频tid
                         "tname": video_data['tname'],  # 视频分类名
                         "版权": video_data['rights'],  # 版权信息
                         "封面图片": video_data['pic'],  # 封面图片链接
                         "title": video_data['title']  # 视频标题
                     }
@@ -91,11 +94,13 @@
         >支持选择ip<br>
         >增加了BV_get_File函数的多个选项<br>
         ****
         ### 1.1.0.0 正式版本更新
         >支持获取弹幕<br>
         ****
         ### 1.2.0.0 正式版本修复
-        
         >取消了不必要的错误<br>
+        ****
+        ### 2.0.0.0 正式版本更新
+        >增加了av号的操作！和BV号同步更新！<br>
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `bilibili_up-1.2.0.0/setup.py` & `bilibili_up-2.0.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='bilibili_up',
-    version='1.2.0.0',
+    version='2.0.0.0',
     author='SuiBo',
     author_email='534047068@qq.com',
     description='bilibili_up获取bilibili视频信息的爬虫！',
     install_requires=[
         'requests',
     ],
     py_modules=["bilibili_up"],
```

