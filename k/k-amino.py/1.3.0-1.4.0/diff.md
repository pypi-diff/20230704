# Comparing `tmp/k-amino.py-1.3.0.tar.gz` & `tmp/k-amino.py-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k-amino.py-1.3.0.tar", last modified: Thu May 18 08:00:40 2023, max compression
+gzip compressed data, was "k-amino.py-1.4.0.tar", last modified: Tue Jul  4 09:28:58 2023, max compression
```

## Comparing `k-amino.py-1.3.0.tar` & `k-amino.py-1.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.613183 k-amino.py-1.3.0/
--rw-rw-rw-   0        0        0      586 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     2143 2023-05-18 08:00:40.613183 k-amino.py-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.491336 k-amino.py-1.3.0/k_amino/
--rw-rw-rw-   0        0        0      872 2023-05-18 07:58:35.000000 k-amino.py-1.3.0/k_amino/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.536282 k-amino.py-1.3.0/k_amino/k_async/
--rw-rw-rw-   0        0        0      122 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/__init__.py
--rw-rw-rw-   0        0        0     4438 2023-05-11 06:13:50.000000 k-amino.py-1.3.0/k_amino/k_async/acm.py
--rw-rw-rw-   0        0        0     2392 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/bot.py
--rw-rw-rw-   0        0        0    31693 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/client.py
--rw-rw-rw-   0        0        0    47044 2023-05-12 21:17:23.000000 k-amino.py-1.3.0/k_amino/k_async/local.py
--rw-rw-rw-   0        0        0    27434 2023-05-18 07:57:43.000000 k-amino.py-1.3.0/k_amino/k_async/sockets.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.575287 k-amino.py-1.3.0/k_amino/k_async/websocket_async/
--rw-rw-rw-   0        0        0      801 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/__init__.py
--rw-rw-rw-   0        0        0    13388 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_abnf.py
--rw-rw-rw-   0        0        0    20115 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_app.py
--rw-rw-rw-   0        0        0     2118 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_cookiejar.py
--rw-rw-rw-   0        0        0    20129 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_core.py
--rw-rw-rw-   0        0        0     2105 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_exceptions.py
--rw-rw-rw-   0        0        0     6073 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_handshake.py
--rw-rw-rw-   0        0        0    11803 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_http.py
--rw-rw-rw-   0        0        0     2027 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_logging.py
--rw-rw-rw-   0        0        0     4922 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_socket.py
--rw-rw-rw-   0        0        0     1122 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_ssl_compat.py
--rw-rw-rw-   0        0        0     4797 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_url.py
--rw-rw-rw-   0        0        0     3516 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_utils.py
--rw-rw-rw-   0        0        0     6909 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_wsdump.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.592239 k-amino.py-1.3.0/k_amino/k_sync/
--rw-rw-rw-   0        0        0      102 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_sync/__init__.py
--rw-rw-rw-   0        0        0     4256 2023-05-11 06:14:07.000000 k-amino.py-1.3.0/k_amino/k_sync/acm.py
--rw-rw-rw-   0        0        0     1912 2023-05-11 06:16:04.000000 k-amino.py-1.3.0/k_amino/k_sync/bot.py
--rw-rw-rw-   0        0        0    30339 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_sync/client.py
--rw-rw-rw-   0        0        0    45934 2023-05-18 08:00:07.000000 k-amino.py-1.3.0/k_amino/k_sync/local.py
--rw-rw-rw-   0        0        0    24349 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_sync/sockets.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.610190 k-amino.py-1.3.0/k_amino/lib/
--rw-rw-rw-   0        0        0       95 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/async_sessions.py
--rw-rw-rw-   0        0        0     8314 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/exception.py
--rw-rw-rw-   0        0        0     1986 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/headers.py
--rw-rw-rw-   0        0        0   198102 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/objects.py
--rw-rw-rw-   0        0        0     2422 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/sessions.py
--rw-rw-rw-   0        0        0     1688 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/util.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.516329 k-amino.py-1.3.0/k_amino.py.egg-info/
--rw-rw-rw-   0        0        0     2143 2023-05-18 08:00:39.000000 k-amino.py-1.3.0/k_amino.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1297 2023-05-18 08:00:40.000000 k-amino.py-1.3.0/k_amino.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 08:00:39.000000 k-amino.py-1.3.0/k_amino.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-05-18 08:00:39.000000 k-amino.py-1.3.0/k_amino.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 08:00:39.000000 k-amino.py-1.3.0/k_amino.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 08:00:40.617174 k-amino.py-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:28:58.542780 k-amino.py-1.4.0/
+-rw-rw-rw-   0        0        0      586 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2425 2023-07-04 09:28:58.542780 k-amino.py-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1878 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 09:28:58.495936 k-amino.py-1.4.0/k_amino/
+-rw-rw-rw-   0        0        0      872 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:28:58.508892 k-amino.py-1.4.0/k_amino/k_async/
+-rw-rw-rw-   0        0        0      122 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/__init__.py
+-rw-rw-rw-   0        0        0     4438 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/acm.py
+-rw-rw-rw-   0        0        0     2392 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/bot.py
+-rw-rw-rw-   0        0        0    32678 2023-07-04 09:27:45.000000 k-amino.py-1.4.0/k_amino/k_async/client.py
+-rw-rw-rw-   0        0        0    47044 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/local.py
+-rw-rw-rw-   0        0        0    27434 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:28:58.525836 k-amino.py-1.4.0/k_amino/k_async/websocket_async/
+-rw-rw-rw-   0        0        0      801 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/__init__.py
+-rw-rw-rw-   0        0        0    13388 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_abnf.py
+-rw-rw-rw-   0        0        0    20115 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_app.py
+-rw-rw-rw-   0        0        0     2118 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_cookiejar.py
+-rw-rw-rw-   0        0        0    20129 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_core.py
+-rw-rw-rw-   0        0        0     2105 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_exceptions.py
+-rw-rw-rw-   0        0        0     6073 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_handshake.py
+-rw-rw-rw-   0        0        0    11803 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_http.py
+-rw-rw-rw-   0        0        0     2027 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_logging.py
+-rw-rw-rw-   0        0        0     4922 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_socket.py
+-rw-rw-rw-   0        0        0     1122 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_ssl_compat.py
+-rw-rw-rw-   0        0        0     4797 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_url.py
+-rw-rw-rw-   0        0        0     3516 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_utils.py
+-rw-rw-rw-   0        0        0     6909 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_async/websocket_async/_wsdump.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:28:58.532813 k-amino.py-1.4.0/k_amino/k_sync/
+-rw-rw-rw-   0        0        0      102 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_sync/__init__.py
+-rw-rw-rw-   0        0        0     4256 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_sync/acm.py
+-rw-rw-rw-   0        0        0     1912 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_sync/bot.py
+-rw-rw-rw-   0        0        0    31306 2023-07-04 09:26:10.000000 k-amino.py-1.4.0/k_amino/k_sync/client.py
+-rw-rw-rw-   0        0        0    45934 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_sync/local.py
+-rw-rw-rw-   0        0        0    24349 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/k_sync/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:28:58.541784 k-amino.py-1.4.0/k_amino/lib/
+-rw-rw-rw-   0        0        0       95 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/lib/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/lib/async_sessions.py
+-rw-rw-rw-   0        0        0     8314 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/lib/exception.py
+-rw-rw-rw-   0        0        0     1986 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/lib/headers.py
+-rw-rw-rw-   0        0        0   198102 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/lib/objects.py
+-rw-rw-rw-   0        0        0     2422 2023-07-04 07:24:20.000000 k-amino.py-1.4.0/k_amino/lib/sessions.py
+-rw-rw-rw-   0        0        0     1957 2023-07-04 09:24:26.000000 k-amino.py-1.4.0/k_amino/lib/util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:28:58.501916 k-amino.py-1.4.0/k_amino.py.egg-info/
+-rw-rw-rw-   0        0        0     2425 2023-07-04 09:28:58.000000 k-amino.py-1.4.0/k_amino.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-07-04 09:28:58.000000 k-amino.py-1.4.0/k_amino.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 09:28:58.000000 k-amino.py-1.4.0/k_amino.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-07-04 09:28:58.000000 k-amino.py-1.4.0/k_amino.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 09:28:58.000000 k-amino.py-1.4.0/k_amino.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 09:28:58.543775 k-amino.py-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-07-04 09:28:22.000000 k-amino.py-1.4.0/setup.py
```

### Comparing `k-amino.py-1.3.0/LICENSE` & `k-amino.py-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/PKG-INFO` & `k-amino.py-1.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: k-amino.py
-Version: 1.3.0
-Summary: Amino Bots with python!
-Home-page: https://github.com/kwel999/KAmino
-Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
-Author: KWEL
-Author-email: itskwel999@gmail.com
-License: Apache
-Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## k_amino
 k_amino is unofficial client for [Aminoapps](https://aminoapps.com/) API in Python.
 
 ## Installation
 You can use either `python3 setup.py install` or `pip3 install k-amino.py` to install. This module is tested on Python 3.9+.
 
 ## Contributing
@@ -65,15 +52,29 @@
 client = k_amino.Client()
 client.sid_login("< sid >")
 print(client.sid)
 ```
 #### Send a message in chat
 
 ```py
-import k_amino
+from k_amino import(
+Client,
+SubClient
+)
+import getpass
+
+client = Client()
+email = input("email:  ")
+password = getpass.getpass("password:  ")
+client.login(email=email, password=password)
+
+chat_link = client.get_from_link(input("chat link:  "))
+chat_id = chat_link.objectId
+ndc_client = SubClient(comId=chat_link.comId)
 
-client = k_amino.Client()
-client.login("< email >", "< password >")
-path = client.get_from_link("< chat link >")
-local = k_amino.Local(path.comId)
-local.send_message(path.objectId, "< message >")
+
+
+while True:
+    text = input("Your message: ")
+    ndc_client.send_message(chatId=chat_id,message=text, messageType=0)
+    print(f"message sended:  {text}")
 ```
```

### Comparing `k-amino.py-1.3.0/k_amino/__init__.py` & `k-amino.py-1.4.0/k_amino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .k_async.acm import AsyncAcm
 from .k_async.client import AsyncClient
 from .k_async.local import AsyncSubClient
 # from .k_async.sockets import *
 from .k_async.bot import AsyncBot
 
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 
 __newest__ = loads(get("https://pypi.python.org/pypi/k-amino.py/json").text)["info"]["version"]
 
 if __version__ != __newest__:
     print(f"\033[1;31;38mk_amino New Version!: {__newest__} (You are using {__version__})\033[1;36;33m\nDiscord server: \"https://discord.gg/zd8gyFJquT\"\033[1;0m")
 else:
```

### Comparing `k-amino.py-1.3.0/k_amino/k_async/acm.py` & `k-amino.py-1.4.0/k_amino/k_async/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/bot.py` & `k-amino.py-1.4.0/k_amino/k_async/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/client.py` & `k-amino.py-1.4.0/k_amino/k_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 from time import time as timestamp
 from typing import BinaryIO, Union
 from uuid import UUID
 import asyncio
 
 from ..lib.objects import *
 from ..lib.async_sessions import AsyncSession as Session
+from ..lib.util import updateDevice, generateDevice
 from .sockets import Wss
 
 
 class AsyncClient(Wss, Session):
     def __init__(self, deviceId: str = None, proxies: dict = None, trace: bool = False, bot: bool = False):
         self.trace = trace
         self.proxies = proxies
-        self.deviceId = deviceId
+        self.deviceId = updateDevice(deviceId) if deviceId else generateDevice()
 
         Wss.__init__(self, self, trace=self.trace, is_bot=bot)
         Session.__init__(self, proxies=self.proxies, staticDevice=self.deviceId)
 
     def change_lang(self, lang: str = "en"):
         self.updateHeaders(lang=lang)
 
@@ -882,14 +883,48 @@
             "identity": email,
             "timestamp": int(timestamp() * 1000),
         }
 
         req = await self.postRequest("/g/s/auth/register", data)
         return Json(req)
 
+    async def ads_config(
+        self,
+        chatId: str,
+        title: str = None,
+        content: str = None,
+        icon: str = None,
+        background: str = None,
+        ):
+        res, data = [], {"timestamp": int(timestamp() * 1000)}
+
+        if title:
+            data["title"] = title
+
+        if content:
+            data["content"] = content
+
+        if icon:
+            data["icon"] = icon
+
+        if background:
+            data = {
+                "media": [100, background, None],
+                "timestamp": int(timestamp() * 1000),
+            }
+            req = await self.postRequest(
+                f"/g/s/chat/thread/{chatId}/member/{self.uid}/background",
+                data,
+            )
+            res.append(Json(req))
+
+        req = await self.postRequest(f"/g/s/chat/thread/{chatId}", data)
+        res.append(Json(req))
+        return res
+
     async def remove_host(self, chatId: str, userId: str):
         req = await self.deleteRequest(f"/g/s/chat/thread/{chatId}/co-host/{userId}")
         return Json(req)
 
     async def edit_comment(self, commentId: str, comment: str, userId: str):
         data = {"content": comment, "timestamp": int(timestamp() * 1000)}
         req = await self.postRequest(f"/g/s/user-profile/{userId}/comment/{commentId}", data)
```

### Comparing `k-amino.py-1.3.0/k_amino/k_async/local.py` & `k-amino.py-1.4.0/k_amino/k_async/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/sockets.py` & `k-amino.py-1.4.0/k_amino/k_async/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/__init__.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/__init__.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_abnf.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_abnf.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_app.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_app.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_cookiejar.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_cookiejar.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_core.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_core.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_exceptions.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_exceptions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_handshake.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_handshake.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_http.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_http.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_logging.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_logging.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_socket.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_socket.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_ssl_compat.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_url.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_url.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_utils.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_utils.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_wsdump.py` & `k-amino.py-1.4.0/k_amino/k_async/websocket_async/_wsdump.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_sync/acm.py` & `k-amino.py-1.4.0/k_amino/k_sync/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_sync/bot.py` & `k-amino.py-1.4.0/k_amino/k_sync/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_sync/client.py` & `k-amino.py-1.4.0/k_amino/k_sync/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 from binascii import hexlify
 from time import time as timestamp
 from typing import BinaryIO, Union
 from uuid import UUID
 
 from ..lib.objects import *
 from ..lib.sessions import Session
+from ..lib.util import updateDevice, generateDevice
 from .sockets import Wss
 
 
 class Client(Wss, Session):
     def __init__(self, deviceId: str = None, proxies: dict = None, trace: bool = False, bot: bool = False):
         self.trace = trace
         self.proxies = proxies
-        self.deviceId = deviceId
+        self.deviceId = updateDevice(deviceId) if deviceId else generateDevice()
 
         Wss.__init__(self, self, trace=self.trace, is_bot=bot)
         Session.__init__(self, proxies=self.proxies, staticDevice=self.deviceId)
 
     def change_lang(self, lang: str = "en"):
         self.updateHeaders(lang=lang)
 
@@ -867,14 +868,48 @@
             "identity": email,
             "timestamp": int(timestamp() * 1000),
         }
 
         req = self.postRequest("/g/s/auth/register", data)
         return Json(req)
 
+    def ads_config(
+        self,
+        chatId: str,
+        title: str = None,
+        content: str = None,
+        icon: str = None,
+        background: str = None,
+        ):
+        res, data = [], {"timestamp": int(timestamp() * 1000)}
+
+        if title:
+            data["title"] = title
+
+        if content:
+            data["content"] = content
+
+        if icon:
+            data["icon"] = icon
+
+        if background:
+            data = {
+                "media": [100, background, None],
+                "timestamp": int(timestamp() * 1000),
+            }
+            req = self.postRequest(
+                f"/g/s/chat/thread/{chatId}/member/{self.uid}/background",
+                data,
+            )
+            res.append(Json(req))
+
+        req = self.postRequest(f"/g/s/chat/thread/{chatId}", data)
+        res.append(Json(req))
+        return res
+
     def remove_host(self, chatId: str, userId: str):
         req = self.deleteRequest(f"/g/s/chat/thread/{chatId}/co-host/{userId}")
         return Json(req)
 
     def edit_comment(self, commentId: str, comment: str, userId: str):
         data = {"content": comment, "timestamp": int(timestamp() * 1000)}
         req = self.postRequest(f"/g/s/user-profile/{userId}/comment/{commentId}", data)
```

### Comparing `k-amino.py-1.3.0/k_amino/k_sync/local.py` & `k-amino.py-1.4.0/k_amino/k_sync/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/k_sync/sockets.py` & `k-amino.py-1.4.0/k_amino/k_sync/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/lib/async_sessions.py` & `k-amino.py-1.4.0/k_amino/lib/async_sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/lib/exception.py` & `k-amino.py-1.4.0/k_amino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/lib/headers.py` & `k-amino.py-1.4.0/k_amino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/lib/objects.py` & `k-amino.py-1.4.0/k_amino/lib/objects.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino/lib/sessions.py` & `k-amino.py-1.4.0/k_amino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/k_amino.py.egg-info/SOURCES.txt` & `k-amino.py-1.4.0/k_amino.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.3.0/setup.py` & `k-amino.py-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,12 +47,12 @@
         "httpx",
         "setuptools",
         "aiohttp",
         "websocket-client==1.3.1",
         "websockets",
         "ujson",
         "requests",
-        "easy-events==2.8.2"
+        "easy-events>=2.8.2"
     ],
     setup_requires=["wheel"],
     packages=find_packages(),
 )
```

