# Comparing `tmp/bilibili_up-0.2.1.1.tar.gz` & `tmp/bilibili_up-0.2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bilibili_up-0.2.1.1.tar", last modified: Mon Jul  3 13:45:14 2023, max compression
+gzip compressed data, was "dist\bilibili_up-0.2.1.2.tar", last modified: Tue Jul  4 05:04:52 2023, max compression
```

## Comparing `bilibili_up-0.2.1.1.tar` & `bilibili_up-0.2.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/
--rw-rw-rw-   0        0        0      208 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/bilibili_up/
--rw-rw-rw-   0        0        0     2159 2023-07-03 13:40:16.000000 bilibili_up-0.2.1.1/bilibili_up/BV.py
--rw-rw-rw-   0        0        0        0 2023-07-03 11:25:14.000000 bilibili_up-0.2.1.1/bilibili_up/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/bilibili_up.egg-info/
--rw-rw-rw-   0        0        0      208 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/bilibili_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/bilibili_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/bilibili_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/bilibili_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/bilibili_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 13:45:14.000000 bilibili_up-0.2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      315 2023-07-03 13:44:59.000000 bilibili_up-0.2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/
+-rw-rw-rw-   0        0        0      267 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2023-07-04 04:56:54.000000 bilibili_up-0.2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/bilibili_up/
+-rw-rw-rw-   0        0        0     2147 2023-07-04 04:40:44.000000 bilibili_up-0.2.1.2/bilibili_up/BV.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 11:25:14.000000 bilibili_up-0.2.1.2/bilibili_up/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/bilibili_up.egg-info/
+-rw-rw-rw-   0        0        0      267 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/bilibili_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/bilibili_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/bilibili_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/bilibili_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/bilibili_up.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 05:04:52.000000 bilibili_up-0.2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      395 2023-07-04 05:02:38.000000 bilibili_up-0.2.1.2/setup.py
```

### Comparing `bilibili_up-0.2.1.1/bilibili_up/BV.py` & `bilibili_up-0.2.1.2/bilibili_up/BV.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
             }
         else:
             raise 查询失败("出现错误，请检查连接网络或请求头。")
     except Exception as e:
         raise 查询失败("出现错误，请检查连接网络或请求头。")
 
 # 获取BV视频评论区（字典）
-def BV_get_comments(video_id,PageNumber,headers=None):
+def BV_get_comments(BV,PageNumber,headers=None):
     try:
-        url = f'https://api.bilibili.com/x/v2/reply/main?pn=1&type=1&oid={video_id}&sort=0'
+        url = f'https://api.bilibili.com/x/v2/reply/main?pn=1&type=1&oid={BV}&sort=0'
         comments_dict = {}
         PageNumber = int(PageNumber)
         PageNumber += 1
         for page in range(1, PageNumber):  # 获取前五页评论
             params = {'pn': page}
             response = requests.get(url, headers=headers, params=params)
             data = response.json()
```

