# Comparing `tmp/bilibili_up-1.0.0.0.tar.gz` & `tmp/bilibili_up-1.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bilibili_up-1.0.0.0.tar", last modified: Tue Jul  4 06:11:29 2023, max compression
+gzip compressed data, was "dist\bilibili_up-1.1.0.0.tar", last modified: Tue Jul  4 07:18:49 2023, max compression
```

## Comparing `bilibili_up-1.0.0.0.tar` & `bilibili_up-1.1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/
--rw-rw-rw-   0        0        0     3014 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2217 2023-07-04 06:11:00.000000 bilibili_up-1.0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/bilibili_up/
--rw-rw-rw-   0        0        0     2791 2023-07-04 06:02:48.000000 bilibili_up-1.0.0.0/bilibili_up/BV.py
--rw-rw-rw-   0        0        0        0 2023-07-03 11:25:14.000000 bilibili_up-1.0.0.0/bilibili_up/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/
--rw-rw-rw-   0        0        0     3014 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-04 06:11:28.000000 bilibili_up-1.0.0.0/bilibili_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 06:11:29.000000 bilibili_up-1.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      574 2023-07-04 06:11:00.000000 bilibili_up-1.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/
+-rw-rw-rw-   0        0        0     3675 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2710 2023-07-04 07:18:29.000000 bilibili_up-1.1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up/
+-rw-rw-rw-   0        0        0     4109 2023-07-04 07:13:40.000000 bilibili_up-1.1.0.0/bilibili_up/BV.py
+-rw-rw-rw-   0        0        0       28 2023-07-04 07:13:21.000000 bilibili_up-1.1.0.0/bilibili_up/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/
+-rw-rw-rw-   0        0        0     3675 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/bilibili_up.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 07:18:49.000000 bilibili_up-1.1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-04 07:18:29.000000 bilibili_up-1.1.0.0/setup.py
```

### Comparing `bilibili_up-1.0.0.0/PKG-INFO` & `bilibili_up-1.1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,84 @@
-Metadata-Version: 2.1
-Name: bilibili_up
-Version: 1.0.0.0
-Summary: bilibili_up获取bilibili视频信息的爬虫！
-Home-page: https://pypi.org/user/SuiBo/
-Author: SuiBo
-Author-email: 534047068@qq.com
-License: UNKNOWN
-Description: # Bilibili_up 使用方法
-        ****
-        ### 关于 BV 号视频的操作<br><br>
-        **导入BV操作**<br>
-        获取BV视频评论区（字典）<br>
-        ```ruby
-        from bilibili_up import BV
-        ```
-        ```ruby
-        #获取BV视频评论区（字典）
-        comments = BV_get_comments(BV=123456789, 
-                   PageNumber=5, 
-                   headers={"User-Agent": "Mozilla/5.0"})
-        for username, content in comments.items():
-            print(f"{username}: {content}")
-        ```
-        其中，BV、PageNumber是必选参数，其他为可选参数。<br>
-        PageNumber：页数（1~PageNumber）<br>
-        BV：视频BV号<br>
-        headers（可选）：自定义请求头<br>
-        ip（可选）:自定义ip<br>
-        返回值是一个字典｛username:content｝<br>
-        >自定义ip选项加上了<br>
-        
-        获取视频信息<br>
-        ```ruby
-        video_info = BV_get_File("BVxxxxxxxx", headers={"User-Agent": "Mozilla/5.0"})
-        print(video_info)
-        ```
-        该函数会返回一个字典，包含视频的播放量、发布时间、作者信息和弹幕数量。<br>
-        源代码的一部分：
-        ```ruby
-        return {
-                        "播放量": play_count,
-                        "发布时间": publish_time,
-                        "作者": {
-                            "名称": author_name,
-                            "UID": author_uid
-                        },
-                        "弹幕数量": danmaku_count,
-                        "bvid": video_data['bvid'],  # 视频BV号
-                        "援助": video_data['aid'],  # 视频援助号
-                        "视频tid": video_data['tid'],  # 视频tid
-                        "tname": video_data['tname'],  # 视频分类名
-                        "版权": video_data['rights'],  # 版权信息
-                        "封面图片": video_data['pic'],  # 封面图片链接
-                        "title": video_data['title']  # 视频标题
-                    }
-        ```
-        想获得作者的uid就需要：
-        ```
-        a = BV_get_File("BVxxxxxxxx")["作者"]["UID"]
-        ```
-        其中，BV是必选参数，其他为可选参数。<br>
-        BV：视频BV号<br>
-        ip（可选）:自定义ip<br>
-        headers（可选）：自定义请求头<br>
-        >在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（以过时）
-        ****
-        ### 1.0.0.0 正式版本更新
-        
-        >支持选择ip<br>
-        >增加了BV_get_File函数的多个选项
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Bilibili_up 使用方法
+****
+### 关于 BV 号视频的操作<br><br>
+**导入BV操作**<br>
+获取BV视频评论区（字典）<br>
+```ruby
+from bilibili_up import BV
+```
+```ruby
+#获取BV视频评论区（字典）
+comments = BV_get_comments(BV=123456789, 
+           PageNumber=5, 
+           headers={"User-Agent": "Mozilla/5.0"})
+for username, content in comments.items():
+    print(f"{username}: {content}")
+```
+其中，BV、PageNumber是必选参数，其他为可选参数。<br>
+PageNumber：页数（1~PageNumber）<br>
+BV：视频BV号<br>
+headers（可选）：自定义请求头<br>
+ip（可选）:自定义ip<br>
+返回值是一个字典｛username:content｝<br>
+>自定义ip选项加上了<br>
+
+获取视频信息<br>
+```ruby
+video_info = BV_get_File("BVxxxxxxxx", headers={"User-Agent": "Mozilla/5.0"})
+print(video_info)
+```
+该函数会返回一个字典，包含视频的播放量、发布时间、作者信息和弹幕数量。<br>
+源代码的一部分：
+```ruby
+return {
+                "播放量": play_count,
+                "发布时间": publish_time,
+                "作者": {
+                    "名称": author_name,
+                    "UID": author_uid
+                },
+                "弹幕数量": danmaku_count,
+                "bvid": video_data['bvid'],  # 视频BV号
+                "援助": video_data['aid'],  # 视频援助号
+                "视频tid": video_data['tid'],  # 视频tid
+                "tname": video_data['tname'],  # 视频分类名
+                "版权": video_data['rights'],  # 版权信息
+                "封面图片": video_data['pic'],  # 封面图片链接
+                "title": video_data['title']  # 视频标题
+            }
+```
+想获得作者的uid就需要：
+```
+a = BV_get_File("BVxxxxxxxx")["作者"]["UID"]
+```
+其中，BV是必选参数，其他为可选参数。<br>
+BV：视频BV号<br>
+ip（可选）:自定义ip<br>
+headers（可选）：自定义请求头<br>
+
+获取BV视频弹幕（字典）<br>
+```ruby
+# 调用函数
+BV_get_danmaku(bvid)
+# 传入指定的 BV 号
+bvid = 'BV**********'
+
+# 调用函数获取弹幕数据
+danmaku_data = BV_get_danmaku(bvid)
+```
+弹幕数据格式说明： `danmaku_data` 是一个字典，以弹幕的时间为键，弹幕内容为值：
+```ruby
+{
+    time_1: content_1,
+    time_2: content_2,
+    ...
+}
+```
+>请确保提供的 BV 号是有效的，对应的视频存在并且具有弹幕。
+****
+>在0.2.1.1版本中，获取BV视频评论区中的BV参数是video_bv（已过时）
+****
+### 1.0.0.0 正式版本更新
+
+>支持选择ip<br>
+>增加了BV_get_File函数的多个选项
```

### Comparing `bilibili_up-1.0.0.0/bilibili_up/BV.py` & `bilibili_up-1.1.0.0/bilibili_up/BV.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-
+import json
 # 报错信息
 class 查询失败(Exception):
     pass
 
 # 获取BV视频信息
 def BV_get_File(bv, headers=None, ip=None):
     # 构建API链接
@@ -61,7 +61,41 @@
             for comment_info in data['data']['replies']:
                 username = comment_info['member']['uname']
                 content = comment_info['content']['message']
                 comments_dict[username] = content
         return comments_dict
     except Exception as e:
         raise 查询失败("出现错误，请检查连接网络、请求头或BV号。")
+
+# 获取BV视频弹幕（字典）
+def BV_get_danmaku(bvid):
+    def get_danmaku_by_bvid(bvid):
+        try:
+            url = f'https://api.bilibili.com/x/v1/dm/list.so?oid={get_oid_by_bvid(bvid)}'
+            response = requests.get(url)
+            response.encoding = response.apparent_encoding
+            danmaku_data = parse_danmaku(response.text)
+            return danmaku_data
+        except Exception as e:
+            print(f"Failed to get danmaku for BV{bvid}: {e}")
+
+    def get_oid_by_bvid(bvid):
+        try:
+            url = f'https://api.bilibili.com/x/player/pagelist?bvid={bvid}'
+            response = requests.get(url)
+            response_json = json.loads(response.text)
+            return response_json['data'][0]['cid']
+        except Exception as e:
+            print(f"Failed to get oid for BV{bvid}: {e}")
+
+    def parse_danmaku(xml_text):
+        danmaku_dict = {}
+        from xml.dom.minidom import parseString
+        dom = parseString(xml_text)
+        chats = dom.getElementsByTagName('d')
+        for chat in chats:
+            time = float(chat.getAttribute('p').split(',')[0])
+            content = chat.childNodes[0].nodeValue
+            danmaku_dict[time] = content
+        return danmaku_dict
+
+    return get_danmaku_by_bvid(bvid)
```

### Comparing `bilibili_up-1.0.0.0/setup.py` & `bilibili_up-1.1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='bilibili_up',
-    version='1.0.0.0',
+    version='1.1.0.0',
     author='SuiBo',
     author_email='534047068@qq.com',
     description='bilibili_up获取bilibili视频信息的爬虫！',
     install_requires=[
         'requests',
+        'json',
     ],
     py_modules=["bilibili_up"],
     packages=find_packages(),
     url = "https://pypi.org/user/SuiBo/",
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

