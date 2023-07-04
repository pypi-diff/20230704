# Comparing `tmp/aiodanbooru-1.0.8.tar.gz` & `tmp/aiodanbooru-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodanbooru-1.0.8.tar", last modified: Mon Jul  3 15:58:44 2023, max compression
+gzip compressed data, was "aiodanbooru-1.0.9.tar", last modified: Tue Jul  4 14:49:11 2023, max compression
```

## Comparing `aiodanbooru-1.0.8.tar` & `aiodanbooru-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:58:44.300972 aiodanbooru-1.0.8/
--rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3022 2023-07-03 15:58:44.299970 aiodanbooru-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 15:58:44.290243 aiodanbooru-1.0.8/aiodanbooru/
--rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.8/aiodanbooru/__init__.py
--rw-rw-rw-   0        0        0     1668 2023-07-03 15:18:05.000000 aiodanbooru-1.0.8/aiodanbooru/api.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:58:44.297970 aiodanbooru-1.0.8/aiodanbooru/base/
--rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.0.8/aiodanbooru/base/__init__.py
--rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.0.8/aiodanbooru/base/filters.py
--rw-rw-rw-   0        0        0     1011 2023-07-03 15:15:24.000000 aiodanbooru-1.0.8/aiodanbooru/base/handler.py
--rw-rw-rw-   0        0        0     2089 2023-07-03 15:58:16.000000 aiodanbooru-1.0.8/aiodanbooru/dispatcher.py
--rw-rw-rw-   0        0        0     3344 2023-07-03 15:57:23.000000 aiodanbooru-1.0.8/aiodanbooru/models.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:58:44.295965 aiodanbooru-1.0.8/aiodanbooru.egg-info/
--rw-rw-rw-   0        0        0     3022 2023-07-03 15:58:44.000000 aiodanbooru-1.0.8/aiodanbooru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-03 15:58:44.000000 aiodanbooru-1.0.8/aiodanbooru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 15:58:44.000000 aiodanbooru-1.0.8/aiodanbooru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-03 15:58:44.000000 aiodanbooru-1.0.8/aiodanbooru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 15:58:44.000000 aiodanbooru-1.0.8/aiodanbooru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 15:58:44.300972 aiodanbooru-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-07-03 15:58:42.000000 aiodanbooru-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:58:44.298972 aiodanbooru-1.0.8/tests/
--rw-rw-rw-   0        0        0     1666 2023-07-03 15:31:10.000000 aiodanbooru-1.0.8/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.545690 aiodanbooru-1.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3022 2023-07-04 14:49:11.545186 aiodanbooru-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.535011 aiodanbooru-1.0.9/aiodanbooru/
+-rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.9/aiodanbooru/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-07-03 15:18:05.000000 aiodanbooru-1.0.9/aiodanbooru/api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.542180 aiodanbooru-1.0.9/aiodanbooru/base/
+-rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.0.9/aiodanbooru/base/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.0.9/aiodanbooru/base/filters.py
+-rw-rw-rw-   0        0        0     1011 2023-07-03 15:15:24.000000 aiodanbooru-1.0.9/aiodanbooru/base/handler.py
+-rw-rw-rw-   0        0        0     2089 2023-07-03 15:58:16.000000 aiodanbooru-1.0.9/aiodanbooru/dispatcher.py
+-rw-rw-rw-   0        0        0     3939 2023-07-04 14:48:13.000000 aiodanbooru-1.0.9/aiodanbooru/models.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.540016 aiodanbooru-1.0.9/aiodanbooru.egg-info/
+-rw-rw-rw-   0        0        0     3022 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 14:49:11.000000 aiodanbooru-1.0.9/aiodanbooru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 14:49:11.545690 aiodanbooru-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-07-04 14:41:58.000000 aiodanbooru-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:49:11.544186 aiodanbooru-1.0.9/tests/
+-rw-rw-rw-   0        0        0     1666 2023-07-03 15:31:10.000000 aiodanbooru-1.0.9/tests/test_api.py
```

### Comparing `aiodanbooru-1.0.8/LICENSE` & `aiodanbooru-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.8/PKG-INFO` & `aiodanbooru-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.8/README.md` & `aiodanbooru-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.8/aiodanbooru/api.py` & `aiodanbooru-1.0.9/aiodanbooru/api.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.8/aiodanbooru/base/filters.py` & `aiodanbooru-1.0.9/aiodanbooru/base/filters.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.8/aiodanbooru/base/handler.py` & `aiodanbooru-1.0.9/aiodanbooru/base/handler.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.8/aiodanbooru/dispatcher.py` & `aiodanbooru-1.0.9/aiodanbooru/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.8/aiodanbooru/models.py` & `aiodanbooru-1.0.9/aiodanbooru/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,22 +41,36 @@
     has_children: bool
     image_height: Optional[int]
     created_at: str
     updated_at: str
 
     @validator("source")
     def validate_source(cls, source):
-        if source is not None and len(source) < 1:
+        if (
+            source is not None
+            and len(source) < 1
+            and not cls.file_url
+            and not cls.large_file_url
+        ):
             raise ValueError("Source must have at least 1 character")
         return source
 
     class Config:
         extra = "allow"
 
-    extension: Optional[str] = Field(None, alias="file_ext")
+    @property
+    def extension(self) -> Optional[str]:
+        if self.large_file_url:
+            return self.large_file_url.split(".")[-1]
+        elif self.file_url:
+            return self.file_url.split(".")[-1]
+        elif self.source:
+            return self.source.split(".")[-1] if "." in self.source else self.file_ext
+        else:
+            return None
 
     async def get_media(self, use_large: bool = True) -> bytes:
         if not self.file_url and not self.large_file_url and self.source:
             return await self._get_media_from_source()
         url = (
             self.large_file_url if use_large and self.large_file_url else self.file_url
         )
@@ -79,15 +93,21 @@
             self.large_file_url if self.large_file_url else self.file_url or self.source
         )
 
     def is_video(self) -> bool:
         return self.extension in ["webm", "mp4"]
 
     def is_image(self) -> bool:
-        return self.extension in ["jpg", "jpeg", "png", "gif"]
+        return self.extension in ["jpg", "jpeg", "png", "webp"]
+
+    def is_animation(self) -> bool:
+        return self.extension in ["gif", "gifv"]
+
+    def is_zip(self) -> bool:
+        return self.extension in ["zip"]
 
     @property
     def filename(self):
         return f"{self.md5}.{self.extension}"
 
     async def _get_media_from_source(self):
         async with aiohttp.ClientSession() as session:
```

### Comparing `aiodanbooru-1.0.8/aiodanbooru.egg-info/PKG-INFO` & `aiodanbooru-1.0.9/aiodanbooru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.8/setup.py` & `aiodanbooru-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiodanbooru",
-    version="1.0.8",
+    version="1.0.9",
     description="A Python library for interacting with the Danbooru API",
     author="lrdcxdes",
     author_email="lordgrief176@email.com",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "aiohttp",
         "pydantic<2.0.0",
```

### Comparing `aiodanbooru-1.0.8/tests/test_api.py` & `aiodanbooru-1.0.9/tests/test_api.py`

 * *Files identical despite different names*

