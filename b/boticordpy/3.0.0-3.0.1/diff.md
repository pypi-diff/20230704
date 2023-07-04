# Comparing `tmp/boticordpy-3.0.0.tar.gz` & `tmp/boticordpy-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boticordpy-3.0.0.tar", last modified: Sat Jul  1 06:31:59 2023, max compression
+gzip compressed data, was "boticordpy-3.0.1.tar", last modified: Tue Jul  4 10:06:04 2023, max compression
```

## Comparing `boticordpy-3.0.0.tar` & `boticordpy-3.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 06:31:59.121819 boticordpy-3.0.0/
--rw-rw-rw-   0        0        0     1074 2023-06-28 06:47:50.000000 boticordpy-3.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3291 2023-07-01 06:31:59.122828 boticordpy-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2583 2023-06-28 06:47:50.000000 boticordpy-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 06:31:59.115682 boticordpy-3.0.0/boticordpy/
--rw-rw-rw-   0        0        0      421 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/__init__.py
--rw-rw-rw-   0        0        0     6189 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/autopost.py
--rw-rw-rw-   0        0        0     6656 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/client.py
--rw-rw-rw-   0        0        0     3865 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/exceptions.py
--rw-rw-rw-   0        0        0     2995 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/http.py
--rw-rw-rw-   0        0        0    26747 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/types.py
--rw-rw-rw-   0        0        0     4942 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/websocket.py
-drwxrwxrwx   0        0        0        0 2023-07-01 06:31:59.121819 boticordpy-3.0.0/boticordpy.egg-info/
--rw-rw-rw-   0        0        0     3291 2023-07-01 06:31:58.000000 boticordpy-3.0.0/boticordpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-07-01 06:31:59.000000 boticordpy-3.0.0/boticordpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 06:31:58.000000 boticordpy-3.0.0/boticordpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-01 06:31:58.000000 boticordpy-3.0.0/boticordpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 06:31:58.000000 boticordpy-3.0.0/boticordpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-01 06:31:59.123365 boticordpy-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1990 2023-06-28 06:47:50.000000 boticordpy-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:06:04.381419 boticordpy-3.0.1/
+-rw-rw-rw-   0        0        0     1074 2023-06-28 06:47:50.000000 boticordpy-3.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3293 2023-07-04 10:06:04.382429 boticordpy-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2585 2023-07-04 10:03:21.000000 boticordpy-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 10:06:04.369820 boticordpy-3.0.1/boticordpy/
+-rw-rw-rw-   0        0        0      421 2023-07-04 10:03:21.000000 boticordpy-3.0.1/boticordpy/__init__.py
+-rw-rw-rw-   0        0        0     6189 2023-06-28 06:47:50.000000 boticordpy-3.0.1/boticordpy/autopost.py
+-rw-rw-rw-   0        0        0     6748 2023-07-04 10:03:21.000000 boticordpy-3.0.1/boticordpy/client.py
+-rw-rw-rw-   0        0        0     3865 2023-06-28 06:47:50.000000 boticordpy-3.0.1/boticordpy/exceptions.py
+-rw-rw-rw-   0        0        0     2996 2023-07-04 10:03:21.000000 boticordpy-3.0.1/boticordpy/http.py
+-rw-rw-rw-   0        0        0    26747 2023-06-28 06:47:50.000000 boticordpy-3.0.1/boticordpy/types.py
+-rw-rw-rw-   0        0        0     4941 2023-07-04 10:03:21.000000 boticordpy-3.0.1/boticordpy/websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:06:04.380912 boticordpy-3.0.1/boticordpy.egg-info/
+-rw-rw-rw-   0        0        0     3293 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-04 10:06:04.383429 boticordpy-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1990 2023-06-28 06:47:50.000000 boticordpy-3.0.1/setup.py
```

### Comparing `boticordpy-3.0.0/LICENSE.txt` & `boticordpy-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boticordpy-3.0.0/PKG-INFO` & `boticordpy-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boticordpy
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Python wrapper for BotiCord API
 Home-page: https://github.com/boticord/boticordpy
 Author: Marakarka
 Author-email: support@kerdoku.top
 License: MIT
 Project-URL: Documentation, https://py.boticord.top/en/stable
 Project-URL: Issue tracker, https://github.com/boticord/boticordpy/issues
@@ -71,15 +71,15 @@
 from boticordpy import BoticordClient
 
 bot = commands.Bot(command_prefix="!")
 
 
 # Function that will return the current bot's stats.
 async def get_stats():
-    return {"servers": len(bot.guilds), "shards": 0, "users": len(bot.users)}
+    return {"servers": len(bot.guilds), "shards": 0, "members": len(bot.users)}
 
 
 # Function that will be called if stats are posted successfully.
 async def on_success_posting():
     print("wow stats posting works")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boticordpy Version: 3.0.0 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: boticordpy Version: 3.0.1 Summary: A Python wrapper
 for BotiCord API Home-page: https://github.com/boticord/boticordpy Author:
 Marakarka Author-email: support@kerdoku.top License: MIT Project-URL:
 Documentation, https://py.boticord.top/en/stable Project-URL: Issue tracker,
 https://github.com/boticord/boticordpy/issues Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 library: ``` pip install boticordpy ``` ``` python3 -m pip install boticordpy
 ``` Or just clone the repo: https://github.com/boticord/boticordpy
 ***** Examples *****
 You can find other examples in an examples folder. **Discord.py Autopost
 example** ```py from discord.ext import commands from boticordpy import
 BoticordClient bot = commands.Bot(command_prefix="!") # Function that will
 return the current bot's stats. async def get_stats(): return {"servers": len
-(bot.guilds), "shards": 0, "users": len(bot.users)} # Function that will be
+(bot.guilds), "shards": 0, "members": len(bot.users)} # Function that will be
 called if stats are posted successfully. async def on_success_posting(): print
 ("wow stats posting works") boticord_client = BoticordClient
 ( "your_boticord_api_token", version=3 ) # <--- BotiCord API token autopost =
 ( boticord_client.autopost() .init_stats(get_stats) .on_success
 (on_success_posting) .start("id_of_your_bot") # <--- ID of your bot ) bot.run
 ("bot token") # <--- Discord bot's token ```
 ***** Links *****
```

### Comparing `boticordpy-3.0.0/README.md` & `boticordpy-3.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 from boticordpy import BoticordClient
 
 bot = commands.Bot(command_prefix="!")
 
 
 # Function that will return the current bot's stats.
 async def get_stats():
-    return {"servers": len(bot.guilds), "shards": 0, "users": len(bot.users)}
+    return {"servers": len(bot.guilds), "shards": 0, "members": len(bot.users)}
 
 
 # Function that will be called if stats are posted successfully.
 async def on_success_posting():
     print("wow stats posting works")
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 library: ``` pip install boticordpy ``` ``` python3 -m pip install boticordpy
 ``` Or just clone the repo: https://github.com/boticord/boticordpy
 ***** Examples *****
 You can find other examples in an examples folder. **Discord.py Autopost
 example** ```py from discord.ext import commands from boticordpy import
 BoticordClient bot = commands.Bot(command_prefix="!") # Function that will
 return the current bot's stats. async def get_stats(): return {"servers": len
-(bot.guilds), "shards": 0, "users": len(bot.users)} # Function that will be
+(bot.guilds), "shards": 0, "members": len(bot.users)} # Function that will be
 called if stats are posted successfully. async def on_success_posting(): print
 ("wow stats posting works") boticord_client = BoticordClient
 ( "your_boticord_api_token", version=3 ) # <--- BotiCord API token autopost =
 ( boticord_client.autopost() .init_stats(get_stats) .on_success
 (on_success_posting) .start("id_of_your_bot") # <--- ID of your bot ) bot.run
 ("bot token") # <--- Discord bot's token ```
 ***** Links *****
```

### Comparing `boticordpy-3.0.0/boticordpy/autopost.py` & `boticordpy-3.0.1/boticordpy/autopost.py`

 * *Files identical despite different names*

### Comparing `boticordpy-3.0.0/boticordpy/client.py` & `boticordpy-3.0.1/boticordpy/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,38 +50,38 @@
         response = await self.http.get_bot_info(bot_id)
         return boticord_types.ResourceBot.from_dict(response)
 
     async def post_bot_stats(
         self,
         bot_id: typing.Union[str, int],
         *,
-        servers: int = 0,
-        shards: int = 0,
-        users: int = 0,
+        servers: typing.Optional[int] = None,
+        shards: typing.Optional[int] = None,
+        users: typing.Optional[int] = None,
     ) -> boticord_types.ResourceBot:
         """Post Bot's stats.
 
         Args:
             bot_id (Union[:obj:`str`, :obj:`int`])
                 Id of the bot to post stats of.
-            servers ( :obj:`int` )
+            servers ( Optional[:obj:`int`] )
                 Bot's servers count
-            shards ( :obj:`int` )
+            shards ( Optional[:obj:`int`] )
                 Bot's shards count
-            users ( :obj:`int` )
+            users ( Optional[:obj:`int`] )
                 Bot's users count
 
         Returns:
             :obj:`~.types.ResourceBot`:
                 ResourceBot object.
         """
         _logger.info("Posting bot stats")
 
         response = await self.http.post_bot_stats(
-            bot_id, {"servers": servers, "shards": shards, "users": users}
+            bot_id, {"servers": servers, "shards": shards, "members": users}
         )
         return boticord_types.ResourceBot.from_dict(response)
 
     async def get_server_info(
         self, server_id: typing.Union[str, int]
     ) -> boticord_types.ResourceServer:
         """Gets information about specified server.
```

### Comparing `boticordpy-3.0.0/boticordpy/exceptions.py` & `boticordpy-3.0.1/boticordpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `boticordpy-3.0.0/boticordpy/http.py` & `boticordpy-3.0.1/boticordpy/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         session: `aiohttp session`_
             The `aiohttp session`_ used for requests to the API.
         loop: `asyncio loop`
     """
 
     def __init__(self, auth_token: str = None, version: int = 3, **kwargs):
         self.token = auth_token
-        self.API_URL = f"https://api.boticord.top/v{version}"
+        self.API_URL = f"https://api.boticord.top/v{version}/"
 
         loop = kwargs.get("loop") or asyncio.get_event_loop()
 
         self.session = kwargs.get("session") or aiohttp.ClientSession(loop=loop)
 
     async def make_request(
         self, method: str, endpoint: str, *, meilisearch_token: str = None, **kwargs
```

### Comparing `boticordpy-3.0.0/boticordpy/types.py` & `boticordpy-3.0.1/boticordpy/types.py`

 * *Files identical despite different names*

### Comparing `boticordpy-3.0.0/boticordpy/websocket.py` & `boticordpy-3.0.1/boticordpy/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     """Represents a client that can be used to interact with the BotiCord by websocket connection."""
 
     def __init__(self, token: str):
         self.__session = None
         self.loop = asyncio.get_event_loop()
         self.ws = None
         self._listeners = {}
-        self.not_closed = True
-
+        self.not_closed = False
         self._token = token
 
     def listener(self):
         """Decorator to set the listener.
 
         .. warning::
```

### Comparing `boticordpy-3.0.0/boticordpy.egg-info/PKG-INFO` & `boticordpy-3.0.1/boticordpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boticordpy
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Python wrapper for BotiCord API
 Home-page: https://github.com/boticord/boticordpy
 Author: Marakarka
 Author-email: support@kerdoku.top
 License: MIT
 Project-URL: Documentation, https://py.boticord.top/en/stable
 Project-URL: Issue tracker, https://github.com/boticord/boticordpy/issues
@@ -71,15 +71,15 @@
 from boticordpy import BoticordClient
 
 bot = commands.Bot(command_prefix="!")
 
 
 # Function that will return the current bot's stats.
 async def get_stats():
-    return {"servers": len(bot.guilds), "shards": 0, "users": len(bot.users)}
+    return {"servers": len(bot.guilds), "shards": 0, "members": len(bot.users)}
 
 
 # Function that will be called if stats are posted successfully.
 async def on_success_posting():
     print("wow stats posting works")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boticordpy Version: 3.0.0 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: boticordpy Version: 3.0.1 Summary: A Python wrapper
 for BotiCord API Home-page: https://github.com/boticord/boticordpy Author:
 Marakarka Author-email: support@kerdoku.top License: MIT Project-URL:
 Documentation, https://py.boticord.top/en/stable Project-URL: Issue tracker,
 https://github.com/boticord/boticordpy/issues Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 library: ``` pip install boticordpy ``` ``` python3 -m pip install boticordpy
 ``` Or just clone the repo: https://github.com/boticord/boticordpy
 ***** Examples *****
 You can find other examples in an examples folder. **Discord.py Autopost
 example** ```py from discord.ext import commands from boticordpy import
 BoticordClient bot = commands.Bot(command_prefix="!") # Function that will
 return the current bot's stats. async def get_stats(): return {"servers": len
-(bot.guilds), "shards": 0, "users": len(bot.users)} # Function that will be
+(bot.guilds), "shards": 0, "members": len(bot.users)} # Function that will be
 called if stats are posted successfully. async def on_success_posting(): print
 ("wow stats posting works") boticord_client = BoticordClient
 ( "your_boticord_api_token", version=3 ) # <--- BotiCord API token autopost =
 ( boticord_client.autopost() .init_stats(get_stats) .on_success
 (on_success_posting) .start("id_of_your_bot") # <--- ID of your bot ) bot.run
 ("bot token") # <--- Discord bot's token ```
 ***** Links *****
```

### Comparing `boticordpy-3.0.0/setup.py` & `boticordpy-3.0.1/setup.py`

 * *Files identical despite different names*

