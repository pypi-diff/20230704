# Comparing `tmp/md2site-0.0.4.tar.gz` & `tmp/md2site-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2site-0.0.4.tar", max compression
+gzip compressed data, was "md2site-0.0.5.tar", max compression
```

## Comparing `md2site-0.0.4.tar` & `md2site-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.4/LICENSE.md
--rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.4/md2site/__init__.py
--rw-r--r--   0        0        0     3321 2023-07-01 10:42:17.319132 md2site-0.0.4/md2site/generator.py
--rw-r--r--   0        0        0     2341 2023-07-01 10:42:29.564710 md2site-0.0.4/md2site/post.py
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.4/md2site/py.typed
--rw-r--r--   0        0        0     2169 2023-07-01 05:43:16.526132 md2site-0.0.4/md2site/renderer.py
--rw-r--r--   0        0        0      419 2023-07-01 10:42:34.126426 md2site-0.0.4/md2site/site.py
--rw-r--r--   0        0        0     1015 2023-07-01 10:43:15.915249 md2site-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.5/md2site/__init__.py
+-rw-r--r--   0        0        0     4048 2023-07-04 11:00:46.653809 md2site-0.0.5/md2site/generator.py
+-rw-r--r--   0        0        0     2464 2023-07-04 10:39:56.386981 md2site-0.0.5/md2site/post.py
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.5/md2site/py.typed
+-rw-r--r--   0        0        0     2169 2023-07-01 05:43:16.526132 md2site-0.0.5/md2site/renderer.py
+-rw-r--r--   0        0        0      419 2023-07-01 10:42:34.126426 md2site-0.0.5/md2site/site.py
+-rw-r--r--   0        0        0     1015 2023-07-04 11:01:05.027423 md2site-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.5/PKG-INFO
```

### Comparing `md2site-0.0.4/LICENSE.md` & `md2site-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `md2site-0.0.4/md2site/generator.py` & `md2site-0.0.5/md2site/generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -71,14 +71,34 @@
         post.backlinks = backlinks
 
 
 def name_to_url(name: str, base_url: str) -> str:
     return f"{base_url}/{name_to_slug(name)}.html"
 
 
+def populate_prev_next_links(posts: list[Post], base_url: str):
+    for index, post in enumerate(posts):
+        if index > 0:
+            prev_post = posts[index - 1]
+            post.prev_post = PostMetaData(
+                prev_post.name,
+                prev_post.title,
+                prev_post.created_at,
+                name_to_url(prev_post.name, base_url),
+            )
+        if index < len(posts) - 1:
+            next_post = posts[index + 1]
+            post.next_post = PostMetaData(
+                next_post.name,
+                next_post.title,
+                next_post.created_at,
+                name_to_url(next_post.name, base_url),
+            )
+
+
 def build_backlink_map(posts: list[Post]) -> dict[str, set[str]]:
     result = {}
     for p in posts:
         links = extract_wikilinks(p.content)
         for link in links:
             if link not in result:
                 result[link] = set()
@@ -111,8 +131,9 @@
     posts = load_post_files()
     site.link_map = build_link_map(posts)
     site.recent_posts = [
         PostMetaData(p.name, p.title, p.created_at, name_to_url(p.name, site.base_url))
         for p in posts[:10]
     ]
     populate_backlinks(posts, site.base_url)
+    populate_prev_next_links(posts, site.base_url)
     build_posts(posts, site)
```

### Comparing `md2site-0.0.4/md2site/post.py` & `md2site-0.0.5/md2site/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import TextIO
 import os
 
 import yaml
 
+from md2site.site import PostMetaData
+
 
 @dataclass
 class MarkdownContent:
     frontmatter: dict[str, str]
     body: str
 
 
@@ -22,14 +24,16 @@
 
     name: str
     title: str
     content: str
     summary: str
     created_at: datetime
     slug: str
+    prev_post: PostMetaData | None = None
+    next_post: PostMetaData | None = None
     backlinks: list[str] = field(default_factory=list)
 
     @classmethod
     def from_file(cls, filepath: Path) -> Post:
         with open(filepath, "r", encoding="utf-8") as f:
             content = separate_frontmatter(f)
             name = filepath.stem
```

### Comparing `md2site-0.0.4/md2site/renderer.py` & `md2site-0.0.5/md2site/renderer.py`

 * *Files identical despite different names*

### Comparing `md2site-0.0.4/pyproject.toml` & `md2site-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md2site"
-version = "0.0.4"
+version = "0.0.5"
 description = "A static site generator with bare-minimum functionality."
 license = "GPL-3.0-or-later"
 authors = ["Yoonseop Kang <e0engoon@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/e0en/md2site"
 repository = "https://github.com/e0en/md2site"
 classifiers = [
```

### Comparing `md2site-0.0.4/PKG-INFO` & `md2site-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2site
-Version: 0.0.4
+Version: 0.0.5
 Summary: A static site generator with bare-minimum functionality.
 Home-page: https://github.com/e0en/md2site
 License: GPL-3.0-or-later
 Author: Yoonseop Kang
 Author-email: e0engoon@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 1 - Planning
```

