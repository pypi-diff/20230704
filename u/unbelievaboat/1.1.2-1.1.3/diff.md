# Comparing `tmp/unbelievaboat-1.1.2.tar.gz` & `tmp/unbelievaboat-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.1.2.tar", last modified: Sun Jul  2 15:29:17 2023, max compression
+gzip compressed data, was "unbelievaboat-1.1.3.tar", last modified: Tue Jul  4 11:43:45 2023, max compression
```

## Comparing `unbelievaboat-1.1.2.tar` & `unbelievaboat-1.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.367874 unbelievaboat-1.1.2/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     3749 2023-07-02 15:29:17.366873 unbelievaboat-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 15:29:17.367874 unbelievaboat-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-02 15:29:02.000000 unbelievaboat-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.302178 unbelievaboat-1.1.2/unbelievaboat/
--rw-rw-rw-   0        0        0     7927 2023-07-01 23:56:31.000000 unbelievaboat-1.1.2/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3390 2023-07-02 15:10:49.000000 unbelievaboat-1.1.2/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.2/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.337385 unbelievaboat-1.1.2/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.2/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.2/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.2/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.351556 unbelievaboat-1.1.2/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.2/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      750 2023-07-01 20:59:31.000000 unbelievaboat-1.1.2/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.2/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.2/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0     1306 2023-07-01 20:56:24.000000 unbelievaboat-1.1.2/unbelievaboat/structures/UserBalance.py
--rw-rw-rw-   0        0        0     2103 2023-07-01 23:12:16.000000 unbelievaboat-1.1.2/unbelievaboat/structures/UserInventory.py
--rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.2/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.360815 unbelievaboat-1.1.2/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1322 2023-07-02 15:20:48.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0     1169 2023-07-02 15:20:05.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0     1623 2023-07-02 15:21:56.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1320 2023-07-02 15:27:56.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1487 2023-07-02 15:27:17.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.365866 unbelievaboat-1.1.2/unbelievaboat/util/
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.2/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.2/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.1.2/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.332422 unbelievaboat-1.1.2/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3749 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.144811 unbelievaboat-1.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3749 2023-07-04 11:43:45.143782 unbelievaboat-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 11:43:45.145835 unbelievaboat-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-04 11:43:08.000000 unbelievaboat-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:43:44.983973 unbelievaboat-1.1.3/unbelievaboat/
+-rw-rw-rw-   0        0        0     7923 2023-07-04 11:42:36.000000 unbelievaboat-1.1.3/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3390 2023-07-02 15:10:49.000000 unbelievaboat-1.1.3/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.3/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.046474 unbelievaboat-1.1.3/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.3/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.3/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.3/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.057619 unbelievaboat-1.1.3/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.3/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      750 2023-07-04 11:42:22.000000 unbelievaboat-1.1.3/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.3/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.3/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1306 2023-07-04 11:42:22.000000 unbelievaboat-1.1.3/unbelievaboat/structures/UserBalance.py
+-rw-rw-rw-   0        0        0     2103 2023-07-04 11:42:22.000000 unbelievaboat-1.1.3/unbelievaboat/structures/UserInventory.py
+-rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.3/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.110528 unbelievaboat-1.1.3/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1322 2023-07-02 15:20:48.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0     1169 2023-07-02 15:20:05.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1623 2023-07-02 15:21:56.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1320 2023-07-02 15:27:56.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1487 2023-07-02 15:27:17.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.141247 unbelievaboat-1.1.3/unbelievaboat/util/
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.3/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.3/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.1.3/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.017591 unbelievaboat-1.1.3/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3749 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.1.2/LICENSE` & `unbelievaboat-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/PKG-INFO` & `unbelievaboat-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.1.2
+Version: 1.1.3
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.1.2/README.md` & `unbelievaboat-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/setup.py` & `unbelievaboat-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.1.2",
+    version="1.1.3",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.1.2/unbelievaboat/Client.py` & `unbelievaboat-1.1.3/unbelievaboat/Client.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             "users": response.get("users", []) if "users" in response else response,
             "page": response.get("page", 1) if "page" in response else 1,
             "total_pages": response.get("total_pages", 1)
             if "total_pages" in response
             else 1,
         }
 
-        return Leaderboard(response)
+        return Leaderboard(data)
 
     async def get_guild(self, guild_id: int) -> Guild:
         endpoint: str = f"guilds/{guild_id}"
         response: Dict[str, Any] = await self._request_handler.request("GET", endpoint)
         return Guild(response)
 
     async def get_application_permission(self, guild_id: int) -> Permission:
```

### Comparing `unbelievaboat-1.1.2/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.1.3/unbelievaboat/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.1.3/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/Leaderboard.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/Store.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/UserBalance.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/UserBalance.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/UserInventory.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/UserInventory.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/items/InventoryItem.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/items/InventoryItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.1.3/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.2/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.1.3/unbelievaboat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.1.2
+Version: 1.1.3
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.1.2/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.1.3/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

