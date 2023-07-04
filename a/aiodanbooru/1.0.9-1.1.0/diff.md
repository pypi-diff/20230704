# Comparing `tmp/aiodanbooru-1.0.9.tar.gz` & `tmp/aiodanbooru-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodanbooru-1.0.9.tar", last modified: Tue Jul  4 14:49:11 2023, max compression
+gzip compressed data, was "aiodanbooru-1.1.0.tar", last modified: Tue Jul  4 16:01:20 2023, max compression
```

## Comparing `aiodanbooru-1.0.9.tar` & `aiodanbooru-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.545690 aiodanbooru-1.0.9/
--rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     3022 2023-07-04 14:49:11.545186 aiodanbooru-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.535011 aiodanbooru-1.0.9/aiodanbooru/
--rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.9/aiodanbooru/__init__.py
--rw-rw-rw-   0        0        0     1668 2023-07-03 15:18:05.000000 aiodanbooru-1.0.9/aiodanbooru/api.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.542180 aiodanbooru-1.0.9/aiodanbooru/base/
--rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.0.9/aiodanbooru/base/__init__.py
--rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.0.9/aiodanbooru/base/filters.py
--rw-rw-rw-   0        0        0     1011 2023-07-03 15:15:24.000000 aiodanbooru-1.0.9/aiodanbooru/base/handler.py
--rw-rw-rw-   0        0        0     2089 2023-07-03 15:58:16.000000 aiodanbooru-1.0.9/aiodanbooru/dispatcher.py
--rw-rw-rw-   0        0        0     3939 2023-07-04 14:48:13.000000 aiodanbooru-1.0.9/aiodanbooru/models.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.540016 aiodanbooru-1.0.9/aiodanbooru.egg-info/
--rw-rw-rw-   0        0        0     3022 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 14:49:11.545690 aiodanbooru-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-07-04 14:41:58.000000 aiodanbooru-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.544186 aiodanbooru-1.0.9/tests/
--rw-rw-rw-   0        0        0     1666 2023-07-03 15:31:10.000000 aiodanbooru-1.0.9/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:01:20.737407 aiodanbooru-1.1.0/
+-rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3022 2023-07-04 16:01:20.737407 aiodanbooru-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 16:01:20.725896 aiodanbooru-1.1.0/aiodanbooru/
+-rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.1.0/aiodanbooru/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-07-03 15:18:05.000000 aiodanbooru-1.1.0/aiodanbooru/api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:01:20.734408 aiodanbooru-1.1.0/aiodanbooru/base/
+-rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.1.0/aiodanbooru/base/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.1.0/aiodanbooru/base/filters.py
+-rw-rw-rw-   0        0        0     1011 2023-07-03 15:15:24.000000 aiodanbooru-1.1.0/aiodanbooru/base/handler.py
+-rw-rw-rw-   0        0        0     2089 2023-07-03 15:58:16.000000 aiodanbooru-1.1.0/aiodanbooru/dispatcher.py
+-rw-rw-rw-   0        0        0     4061 2023-07-04 16:00:54.000000 aiodanbooru-1.1.0/aiodanbooru/models.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:01:20.730895 aiodanbooru-1.1.0/aiodanbooru.egg-info/
+-rw-rw-rw-   0        0        0     3022 2023-07-04 16:01:20.000000 aiodanbooru-1.1.0/aiodanbooru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-04 16:01:20.000000 aiodanbooru-1.1.0/aiodanbooru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 16:01:20.000000 aiodanbooru-1.1.0/aiodanbooru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-04 16:01:20.000000 aiodanbooru-1.1.0/aiodanbooru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 16:01:20.000000 aiodanbooru-1.1.0/aiodanbooru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 16:01:20.737407 aiodanbooru-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-07-04 16:00:54.000000 aiodanbooru-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:01:20.735407 aiodanbooru-1.1.0/tests/
+-rw-rw-rw-   0        0        0     1666 2023-07-03 15:31:10.000000 aiodanbooru-1.1.0/tests/test_api.py
```

### Comparing `aiodanbooru-1.0.9/LICENSE` & `aiodanbooru-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.9/PKG-INFO` & `aiodanbooru-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.9
+Version: 1.1.0
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.9/README.md` & `aiodanbooru-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.9/aiodanbooru/api.py` & `aiodanbooru-1.1.0/aiodanbooru/api.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.9/aiodanbooru/base/filters.py` & `aiodanbooru-1.1.0/aiodanbooru/base/filters.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.9/aiodanbooru/base/handler.py` & `aiodanbooru-1.1.0/aiodanbooru/base/handler.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.9/aiodanbooru/dispatcher.py` & `aiodanbooru-1.1.0/aiodanbooru/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.9/aiodanbooru/models.py` & `aiodanbooru-1.1.0/aiodanbooru/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,21 +56,25 @@
 
     class Config:
         extra = "allow"
 
     @property
     def extension(self) -> Optional[str]:
         if self.large_file_url:
-            return self.large_file_url.split(".")[-1]
+            return self.large_file_url.split("/")[-1].split(".")[-1]
         elif self.file_url:
-            return self.file_url.split(".")[-1]
+            return self.file_url.split("/")[-1].split(".")[-1]
         elif self.source:
-            return self.source.split(".")[-1] if "." in self.source else self.file_ext
+            return (
+                self.source.split("/")[-1].split(".")[-1]
+                if "." in self.source
+                else self.file_ext
+            )
         else:
-            return None
+            return self.file_ext
 
     async def get_media(self, use_large: bool = True) -> bytes:
         if not self.file_url and not self.large_file_url and self.source:
             return await self._get_media_from_source()
         url = (
             self.large_file_url if use_large and self.large_file_url else self.file_url
         )
```

### Comparing `aiodanbooru-1.0.9/aiodanbooru.egg-info/PKG-INFO` & `aiodanbooru-1.1.0/aiodanbooru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.9
+Version: 1.1.0
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.9/setup.py` & `aiodanbooru-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiodanbooru",
-    version="1.0.9",
+    version="1.1.0",
     description="A Python library for interacting with the Danbooru API",
     author="lrdcxdes",
     author_email="lordgrief176@email.com",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "aiohttp",
         "pydantic<2.0.0",
```

### Comparing `aiodanbooru-1.0.9/tests/test_api.py` & `aiodanbooru-1.1.0/tests/test_api.py`

 * *Files identical despite different names*

