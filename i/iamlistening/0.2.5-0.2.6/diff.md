# Comparing `tmp/iamlistening-0.2.5.tar.gz` & `tmp/iamlistening-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.2.5.tar", max compression
+gzip compressed data, was "iamlistening-0.2.6.tar", max compression
```

## Comparing `iamlistening-0.2.5.tar` & `iamlistening-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-03 17:08:54.605363 iamlistening-0.2.5/LICENSE
--rw-r--r--   0        0        0     1857 2023-07-03 17:08:54.605363 iamlistening-0.2.5/README.md
--rw-r--r--   0        0        0       99 2023-07-03 17:08:55.309372 iamlistening-0.2.5/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-03 17:08:54.605363 iamlistening-0.2.5/iamlistening/config.py
--rw-r--r--   0        0        0      805 2023-07-03 17:08:54.605363 iamlistening-0.2.5/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     3839 2023-07-03 17:08:54.605363 iamlistening-0.2.5/iamlistening/main.py
--rw-r--r--   0        0        0     2163 2023-07-03 17:08:55.305372 iamlistening-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 iamlistening-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-04 07:03:56.563760 iamlistening-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1857 2023-07-04 07:03:56.563760 iamlistening-0.2.6/README.md
+-rw-r--r--   0        0        0       99 2023-07-04 07:03:57.299777 iamlistening-0.2.6/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-04 07:03:56.563760 iamlistening-0.2.6/iamlistening/config.py
+-rw-r--r--   0        0        0      805 2023-07-04 07:03:56.563760 iamlistening-0.2.6/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3961 2023-07-04 07:03:56.563760 iamlistening-0.2.6/iamlistening/main.py
+-rw-r--r--   0        0        0     2163 2023-07-04 07:03:57.299777 iamlistening-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 iamlistening-0.2.6/PKG-INFO
```

### Comparing `iamlistening-0.2.5/LICENSE` & `iamlistening-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.5/README.md` & `iamlistening-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.5/iamlistening/config.py` & `iamlistening-0.2.6/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.5/iamlistening/default_settings.toml` & `iamlistening-0.2.6/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.5/iamlistening/main.py` & `iamlistening-0.2.6/iamlistening/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import threading
 
 import discord
 from telethon import TelegramClient, events
 import simplematrixbotlib as botlib
 
 from .config import settings
-
+from iamlistening import __version__
 
 class Listener:
     """ 👂 Listener class """
 
     def __init__(self):
         self.logger = logging.getLogger("Listener")
         self.latest_message = None
@@ -115,7 +115,10 @@
 
     async def post_init(self):
         return "bot is online"
 
     def stop(self):
         """Stop the listener."""
         self.stopped = True
+
+    async def get_info(self):
+        return f"{__class__.__name__} {__version__}\n"
```

### Comparing `iamlistening-0.2.5/pyproject.toml` & `iamlistening-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.2.5"
+version = "0.2.6"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.2.5/PKG-INFO` & `iamlistening-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.2.5
+Version: 0.2.6
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

