# Comparing `tmp/nonebot_plugin_poke-0.0.5.tar.gz` & `tmp/nonebot_plugin_poke-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_poke-0.0.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_poke-0.0.6.tar", max compression
```

## Comparing `nonebot_plugin_poke-0.0.5.tar` & `nonebot_plugin_poke-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/LICENSE
--rw-r--r--   0        0        0     2923 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/README.md
--rw-r--r--   0        0        0     3441 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/__init__.py
--rw-r--r--   0        0        0      753 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/config.py
--rw-r--r--   0        0        0     3988 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/utils.py
--rw-r--r--   0        0        0      922 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2923 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/README.md
+-rw-r--r--   0        0        0     5088 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/__init__.py
+-rw-r--r--   0        0        0      753 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/config.py
+-rw-r--r--   0        0        0     4623 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/utils.py
+-rw-r--r--   0        0        0      922 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.6/PKG-INFO
```

### Comparing `nonebot_plugin_poke-0.0.5/LICENSE` & `nonebot_plugin_poke-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.5/README.md` & `nonebot_plugin_poke-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/config.py` & `nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/utils.py` & `nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 from nonebot.matcher import Matcher
 from nonebot.adapters.onebot.v11 import PokeNotifyEvent,MessageSegment, Message
 
 import random
+import aiohttp
 from typing import List
+from pathlib import Path
 
 from .config import config
 
-
+async def get_data(url:str):
+    """获取url内容"""
+    headers = {
+    'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
+    }
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url, headers=headers, timeout=600) as response:
+            if response.status == 200:
+                return await response.read()
+            else:
+                return None
+            
+            
 async def acc_send(matcher:Matcher):
     """音乐部分"""
     if not config.poke_send_acc:
         return
     else:
         poke_file_path = config.poke_path
         poke_file_path.joinpath('acc').mkdir(parents=True, exist_ok=True)
@@ -94,7 +108,13 @@
         else:
             if group in config.poke_allow_group:
                 return True
             else:
                 return False
     else:
         return False
+
+
+async def add_pic():
+    pic_file_path = config.poke_path.joinpath('pic')
+    pic_file_path.mkdir(parents=True, exist_ok=True)
+
```

### Comparing `nonebot_plugin_poke-0.0.5/pyproject.toml` & `nonebot_plugin_poke-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_poke"
-version = "0.0.5"
+version = "0.0.6"
 description = "群聊戳戳事件 plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_poke"
 repository = "https://github.com/Agnes4m/nonebot_plugin_poke"
 keywords = ["nonebot2", "plugin","event"]
```

### Comparing `nonebot_plugin_poke-0.0.5/PKG-INFO` & `nonebot_plugin_poke-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-poke
-Version: 0.0.5
+Version: 0.0.6
 Summary: 群聊戳戳事件 plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_poke
 License: MIT
 Keywords: nonebot2,plugin,event
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.6 Summary:
 ç¾¤èæ³æ³äºä»¶ plugin for NoneBot2 Home-page: https://github.com/Agnes4m/
 nonebot_plugin_poke License: MIT Keywords: nonebot2,plugin,event Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

