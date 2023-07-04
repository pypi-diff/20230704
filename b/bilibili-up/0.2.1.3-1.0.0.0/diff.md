# Comparing `tmp/bilibili_up-0.2.1.3.tar.gz` & `tmp/bilibili_up-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bilibili_up-0.2.1.3.tar", last modified: Tue Jul  4 05:08:40 2023, max compression
+gzip compressed data, was "dist\bilibili_up-1.0.0.0.tar", last modified: Tue Jul  4 06:11:29 2023, max compression
```

## Comparing `bilibili_up-0.2.1.3.tar` & `bilibili_up-1.0.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/
--rw-rw-rw-   0        0        0     2258 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2023-07-04 04:56:54.000000 bilibili_up-0.2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/bilibili_up/
--rw-rw-rw-   0        0        0     2147 2023-07-04 04:40:44.000000 bilibili_up-0.2.1.3/bilibili_up/BV.py
--rw-rw-rw-   0        0        0        0 2023-07-03 11:25:14.000000 bilibili_up-0.2.1.3/bilibili_up/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/bilibili_up.egg-info/
--rw-rw-rw-   0        0        0     2258 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/bilibili_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/bilibili_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/bilibili_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/bilibili_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/bilibili_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 05:08:40.000000 bilibili_up-0.2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      574 2023-07-04 05:08:18.000000 bilibili_up-0.2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/
+-rw-rw-rw-   0        0        0     3014 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2217 2023-07-04 06:11:00.000000 bilibili_up-1.0.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/bilibili_up/
+-rw-rw-rw-   0        0        0     2791 2023-07-04 06:02:48.000000 bilibili_up-1.0.0.0/bilibili_up/BV.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 11:25:14.000000 bilibili_up-1.0.0.0/bilibili_up/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/
+-rw-rw-rw-   0        0        0     3014 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      574 2023-07-04 06:11:00.000000 bilibili_up-1.0.0.0/setup.py
```

### Comparing `bilibili_up-0.2.1.3/PKG-INFO` & `bilibili_up-1.0.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 Metadata-Version: 2.1
 Name: bilibili_up
-Version: 0.2.1.3
+Version: 1.0.0.0
 Summary: bilibili_up获取bilibili视频信息的爬虫！
 Home-page: https://pypi.org/user/SuiBo/
 Author: SuiBo
 Author-email: 534047068@qq.com
 License: UNKNOWN
 Description: # Bilibili_up 使用方法
         ****
         ### 关于 BV 号视频的操作<br><br>
         **导入BV操作**<br>
         获取BV视频评论区（字典）<br>
-        `from bilibili_up import BV`
+        ```ruby
+        from bilibili_up import BV
+        ```
         ```ruby
         #获取BV视频评论区（字典）
         comments = BV_get_comments(BV=123456789, 
                    PageNumber=5, 
                    headers={"User-Agent": "Mozilla/5.0"})
         for username, content in comments.items():
             print(f"{username}: {content}")
         ```
         其中，BV、PageNumber是必选参数，其他为可选参数。<br>
         PageNumber：页数（1~PageNumber）<br>
         BV：视频BV号<br>
         headers（可选）：自定义请求头<br>
+        ip（可选）:自定义ip<br>
         返回值是一个字典｛username:content｝<br>
-        >自定义ip选项下一个版本加上<br>
+        >自定义ip选项加上了<br>
         
         获取视频信息<br>
         ```ruby
         video_info = BV_get_File("BVxxxxxxxx", headers={"User-Agent": "Mozilla/5.0"})
         print(video_info)
         ```
         该函数会返回一个字典，包含视频的播放量、发布时间、作者信息和弹幕数量。<br>
         源代码的一部分：
-        ```
+        ```ruby
         return {
                         "播放量": play_count,
                         "发布时间": publish_time,
                         "作者": {
                             "名称": author_name,
                             "UID": author_uid
                         },
-                        "弹幕数量": danmaku_count
+                        "弹幕数量": danmaku_count,
+                        "bvid": video_data['bvid'],  # 视频BV号
+                        "援助": video_data['aid'],  # 视频援助号
+                        "视频tid": video_data['tid'],  # 视频tid
+                        "tname": video_data['tname'],  # 视频分类名
+                        "版权": video_data['rights'],  # 版权信息
+                        "封面图片": video_data['pic'],  # 封面图片链接
+                        "title": video_data['title']  # 视频标题
                     }
         ```
         想获得作者的uid就需要：
         ```
         a = BV_get_File("BVxxxxxxxx")["作者"]["UID"]
         ```
         其中，BV是必选参数，其他为可选参数。<br>
         BV：视频BV号<br>
+        ip（可选）:自定义ip<br>
         headers（可选）：自定义请求头<br>
         >在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（以过时）
+        ****
+        ### 1.0.0.0 正式版本更新
+        
+        >支持选择ip<br>
+        >增加了BV_get_File函数的多个选项
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `bilibili_up-0.2.1.3/README.md` & `bilibili_up-1.0.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 # Bilibili_up 使用方法
 ****
 ### 关于 BV 号视频的操作<br><br>
 **导入BV操作**<br>
 获取BV视频评论区（字典）<br>
-`from bilibili_up import BV`
+```ruby
+from bilibili_up import BV
+```
 ```ruby
 #获取BV视频评论区（字典）
 comments = BV_get_comments(BV=123456789, 
            PageNumber=5, 
            headers={"User-Agent": "Mozilla/5.0"})
 for username, content in comments.items():
     print(f"{username}: {content}")
 ```
 其中，BV、PageNumber是必选参数，其他为可选参数。<br>
 PageNumber：页数（1~PageNumber）<br>
 BV：视频BV号<br>
 headers（可选）：自定义请求头<br>
+ip（可选）:自定义ip<br>
 返回值是一个字典｛username:content｝<br>
->自定义ip选项下一个版本加上<br>
+>自定义ip选项加上了<br>
 
 获取视频信息<br>
 ```ruby
 video_info = BV_get_File("BVxxxxxxxx", headers={"User-Agent": "Mozilla/5.0"})
 print(video_info)
 ```
 该函数会返回一个字典，包含视频的播放量、发布时间、作者信息和弹幕数量。<br>
 源代码的一部分：
-```
+```ruby
 return {
                 "播放量": play_count,
                 "发布时间": publish_time,
                 "作者": {
                     "名称": author_name,
                     "UID": author_uid
                 },
-                "弹幕数量": danmaku_count
+                "弹幕数量": danmaku_count,
+                "bvid": video_data['bvid'],  # 视频BV号
+                "援助": video_data['aid'],  # 视频援助号
+                "视频tid": video_data['tid'],  # 视频tid
+                "tname": video_data['tname'],  # 视频分类名
+                "版权": video_data['rights'],  # 版权信息
+                "封面图片": video_data['pic'],  # 封面图片链接
+                "title": video_data['title']  # 视频标题
             }
 ```
 想获得作者的uid就需要：
 ```
 a = BV_get_File("BVxxxxxxxx")["作者"]["UID"]
 ```
 其中，BV是必选参数，其他为可选参数。<br>
 BV：视频BV号<br>
+ip（可选）:自定义ip<br>
 headers（可选）：自定义请求头<br>
->在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（以过时）
+>在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（以过时）
+****
+### 1.0.0.0 正式版本更新
+
+>支持选择ip<br>
+>增加了BV_get_File函数的多个选项
```

### Comparing `bilibili_up-0.2.1.3/bilibili_up/BV.py` & `bilibili_up-1.0.0.0/bilibili_up/BV.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import requests
+
 # 报错信息
 class 查询失败(Exception):
     pass
 
 # 获取BV视频信息
-def BV_get_File(bv,headers=None):
+def BV_get_File(bv, headers=None, ip=None):
     # 构建API链接
     api_url = f"https://api.bilibili.com/x/web-interface/view?bvid={bv}"
 
     try:
-        response = requests.get(api_url,headers=headers)
+        response = requests.get(api_url, headers=headers, proxies={'http': ip, 'https': ip} if ip else None)
         data = response.json()
 
         if data['code'] == 0:
             video_data = data['data']
 
             play_count = video_data['stat']['view']  # 播放量
             publish_time = video_data['pubdate']  # 发布时间
@@ -24,36 +25,43 @@
             return {
                 "播放量": play_count,
                 "发布时间": publish_time,
                 "作者": {
                     "名称": author_name,
                     "UID": author_uid
                 },
-                "弹幕数量": danmaku_count
+                "弹幕数量": danmaku_count,
+                "bvid": video_data['bvid'],  # 视频BV号
+                "援助": video_data['aid'],  # 视频援助号
+                "视频tid": video_data['tid'],  # 视频tid
+                "tname": video_data['tname'],  # 视频分类名
+                "版权": video_data['rights'],  # 版权信息
+                "封面图片": video_data['pic'],  # 封面图片链接
+                "title": video_data['title']  # 视频标题
             }
         else:
             raise 查询失败("出现错误，请检查连接网络或请求头。")
+            pass
     except Exception as e:
         raise 查询失败("出现错误，请检查连接网络或请求头。")
+        pass
 
 # 获取BV视频评论区（字典）
-def BV_get_comments(BV,PageNumber,headers=None):
+def BV_get_comments(BV, PageNumber, headers=None, ip=None):
     try:
         url = f'https://api.bilibili.com/x/v2/reply/main?pn=1&type=1&oid={BV}&sort=0'
         comments_dict = {}
         PageNumber = int(PageNumber)
         PageNumber += 1
         for page in range(1, PageNumber):  # 获取前五页评论
             params = {'pn': page}
-            response = requests.get(url, headers=headers, params=params)
+            response = requests.get(url, headers=headers, proxies={'http': ip, 'https': ip} if ip else None,
+                                    params=params)
             data = response.json()
 
             for comment_info in data['data']['replies']:
                 username = comment_info['member']['uname']
                 content = comment_info['content']['message']
                 comments_dict[username] = content
         return comments_dict
     except Exception as e:
         raise 查询失败("出现错误，请检查连接网络、请求头或BV号。")
-
-
-
```

### Comparing `bilibili_up-0.2.1.3/bilibili_up.egg-info/PKG-INFO` & `bilibili_up-1.0.0.0/bilibili_up.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 Metadata-Version: 2.1
 Name: bilibili-up
-Version: 0.2.1.3
+Version: 1.0.0.0
 Summary: bilibili_up获取bilibili视频信息的爬虫！
 Home-page: https://pypi.org/user/SuiBo/
 Author: SuiBo
 Author-email: 534047068@qq.com
 License: UNKNOWN
 Description: # Bilibili_up 使用方法
         ****
         ### 关于 BV 号视频的操作<br><br>
         **导入BV操作**<br>
         获取BV视频评论区（字典）<br>
-        `from bilibili_up import BV`
+        ```ruby
+        from bilibili_up import BV
+        ```
         ```ruby
         #获取BV视频评论区（字典）
         comments = BV_get_comments(BV=123456789, 
                    PageNumber=5, 
                    headers={"User-Agent": "Mozilla/5.0"})
         for username, content in comments.items():
             print(f"{username}: {content}")
         ```
         其中，BV、PageNumber是必选参数，其他为可选参数。<br>
         PageNumber：页数（1~PageNumber）<br>
         BV：视频BV号<br>
         headers（可选）：自定义请求头<br>
+        ip（可选）:自定义ip<br>
         返回值是一个字典｛username:content｝<br>
-        >自定义ip选项下一个版本加上<br>
+        >自定义ip选项加上了<br>
         
         获取视频信息<br>
         ```ruby
         video_info = BV_get_File("BVxxxxxxxx", headers={"User-Agent": "Mozilla/5.0"})
         print(video_info)
         ```
         该函数会返回一个字典，包含视频的播放量、发布时间、作者信息和弹幕数量。<br>
         源代码的一部分：
-        ```
+        ```ruby
         return {
                         "播放量": play_count,
                         "发布时间": publish_time,
                         "作者": {
                             "名称": author_name,
                             "UID": author_uid
                         },
-                        "弹幕数量": danmaku_count
+                        "弹幕数量": danmaku_count,
+                        "bvid": video_data['bvid'],  # 视频BV号
+                        "援助": video_data['aid'],  # 视频援助号
+                        "视频tid": video_data['tid'],  # 视频tid
+                        "tname": video_data['tname'],  # 视频分类名
+                        "版权": video_data['rights'],  # 版权信息
+                        "封面图片": video_data['pic'],  # 封面图片链接
+                        "title": video_data['title']  # 视频标题
                     }
         ```
         想获得作者的uid就需要：
         ```
         a = BV_get_File("BVxxxxxxxx")["作者"]["UID"]
         ```
         其中，BV是必选参数，其他为可选参数。<br>
         BV：视频BV号<br>
+        ip（可选）:自定义ip<br>
         headers（可选）：自定义请求头<br>
         >在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（以过时）
+        ****
+        ### 1.0.0.0 正式版本更新
+        
+        >支持选择ip<br>
+        >增加了BV_get_File函数的多个选项
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `bilibili_up-0.2.1.3/setup.py` & `bilibili_up-1.0.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='bilibili_up',
-    version='0.2.1.3',
+    version='1.0.0.0',
     author='SuiBo',
     author_email='534047068@qq.com',
     description='bilibili_up获取bilibili视频信息的爬虫！',
     install_requires=[
         'requests',
     ],
     py_modules=["bilibili_up"],
```

