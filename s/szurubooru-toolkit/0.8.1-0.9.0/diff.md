# Comparing `tmp/szurubooru_toolkit-0.8.1.tar.gz` & `tmp/szurubooru_toolkit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szurubooru_toolkit-0.8.1.tar", max compression
+gzip compressed data, was "szurubooru_toolkit-0.9.0.tar", max compression
```

## Comparing `szurubooru_toolkit-0.8.1.tar` & `szurubooru_toolkit-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-05-08 20:16:35.829065 szurubooru_toolkit-0.8.1/LICENSE
--rw-r--r--   0        0        0    23244 2023-05-08 20:16:35.829065 szurubooru_toolkit-0.8.1/README.md
--rw-r--r--   0        0        0     2466 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1430 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/__init__.py
--rw-r--r--   0        0        0     8809 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/config.py
--rw-r--r--   0        0        0     5146 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/danbooru.py
--rw-r--r--   0        0        0     3716 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/deepbooru.py
--rw-r--r--   0        0        0     1604 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/gelbooru.py
--rw-r--r--   0        0        0    10520 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/saucenao.py
--rw-r--r--   0        0        0      405 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/__init__.py
--rw-r--r--   0        0        0    12349 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/auto_tagger.py
--rw-r--r--   0        0        0     3544 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/create_tags.py
--rw-r--r--   0        0        0     2841 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/delete_posts.py
--rw-r--r--   0        0        0     6461 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_booru.py
--rw-r--r--   0        0        0     4044 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_twitter.py
--rw-r--r--   0        0        0     6013 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_url.py
--rw-r--r--   0        0        0     3314 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/reset_posts.py
--rw-r--r--   0        0        0     4713 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/tag_posts.py
--rw-r--r--   0        0        0    10615 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/upload_media.py
--rw-r--r--   0        0        0    10195 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/szurubooru.py
--rw-r--r--   0        0        0     7036 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/twitter.py
--rw-r--r--   0        0        0    13441 2023-05-08 20:16:35.833065 szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/utils.py
--rw-r--r--   0        0        0    24828 1970-01-01 00:00:00.000000 szurubooru_toolkit-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/LICENSE
+-rw-r--r--   0        0        0    23353 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/README.md
+-rw-r--r--   0        0        0     2625 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1924 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/__init__.py
+-rw-r--r--   0        0        0     8965 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/config.py
+-rw-r--r--   0        0        0     5290 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/danbooru.py
+-rw-r--r--   0        0        0     3716 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/deepbooru.py
+-rw-r--r--   0        0        0     1604 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/gelbooru.py
+-rw-r--r--   0        0        0     5773 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/saucenao.py
+-rw-r--r--   0        0        0      453 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/__init__.py
+-rw-r--r--   0        0        0    12824 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/auto_tagger.py
+-rw-r--r--   0        0        0     7203 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/create_relations.py
+-rw-r--r--   0        0        0     3544 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/create_tags.py
+-rw-r--r--   0        0        0     2841 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/delete_posts.py
+-rw-r--r--   0        0        0     6519 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_booru.py
+-rw-r--r--   0        0        0     4044 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_twitter.py
+-rw-r--r--   0        0        0     7058 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_url.py
+-rw-r--r--   0        0        0     3314 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/reset_posts.py
+-rw-r--r--   0        0        0     4713 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/tag_posts.py
+-rw-r--r--   0        0        0    11103 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/upload_media.py
+-rw-r--r--   0        0        0    12255 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/szurubooru.py
+-rw-r--r--   0        0        0     7036 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/twitter.py
+-rw-r--r--   0        0        0    19173 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/utils.py
+-rw-r--r--   0        0        0    24881 1970-01-01 00:00:00.000000 szurubooru_toolkit-0.9.0/PKG-INFO
```

### Comparing `szurubooru_toolkit-0.8.1/LICENSE` & `szurubooru_toolkit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/README.md` & `szurubooru_toolkit-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 | `twitter` | `access_token` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
 | `twitter` | `access_token_secret` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
 | `upload_media` | `src_path` | Every valid media file under this dir (recursively) will get uploaded | `"/local/path/to/upload/dir"` |
 | `upload_media` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `upload_media` | `cleanup` | Set this to true if images in the `src_path` should be deleted after upload | `false` |
 | `upload_media` | `tags` | These tags will get set for all uploaded posts. Separate them by a comma. | `["tagme", "tag1", "tag2", "tagN"]` |
 | `upload_media` | `auto_tag` | Set this to true if you want your post to be automatically tagged after upload | `false` |
-| `upload_media` | `max_similarity` | Adjust this value to ignore posts if a similar post higher than the threshold has already been uploaded | `"0.99"` |
+| `upload_media` | `max_similarity` | Adjust this value to ignore posts if a similar post higher than the threshold has already been uploaded. 1.00 being basically the same image, but not necessarily. Set to 1.00 if you know there are not duplicates. | `"0.99"` |
 | `upload_media` | `convert_to_jpg` | Convert images to JPG to save disk space. This won't overwrite the source files and only affects the uploaded image. Images might slip through identical post check. | `false` |
 | `upload_media` | `convert_quality` | Only images above this threshold will be converted to jpg if `convert_to_jpg` is True. | `"3MB\|500KB"` |
 | `upload_media` | `shrink` | Set to true to shrink images to shrink_dimensions based on shrink_threshold below. Images might slip through identical post check. | `false` |
 | `upload_media` | `shrink_threshold` | Images which total pixel size exceeds this treshold will be resized to `shrink_size`. E.g. 2000x3000 results in 6000000. | `"6000000"` |
 | `upload_media` | `shrink_dimensions` | Set the max value for width/height. Keeps aspect ratio. E.g. 2000x4000 results in 700x1400, 4000x2000 in 1400x700 (with `"1400x1400"`). | `"2500x2500"` |
 | `upload_media` | `default_safety` | # Set the default safety in case neither SauceNAO, nor Deepbooru could determine it | `safe` |
 | `import_from_booru` | `deepbooru_enabled` | Apply Deepbooru tagging additionally besides fetched tags from Booru | `false` |
```

### Comparing `szurubooru_toolkit-0.8.1/pyproject.toml` & `szurubooru_toolkit-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -34,55 +34,58 @@
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 
 
 [tool.poetry]
 name = "szurubooru-toolkit"
-version = "0.8.1"
+version = "0.9.0"
 description = "Python package and script collection to manage szurubooru."
 authors = ["reluce <reluce@fkosquad.moe>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/reluce/szurubooru-toolkit"
 documentation = "https://github.com/reluce/szurubooru-toolkit"
 keywords = ["szurubooru", "szuru", "booru", "saucenao", "deepbooru"]
 
 [tool.poetry.scripts]
 auto-tagger = 'szurubooru_toolkit.scripts.auto_tagger:main'
 upload-media = 'szurubooru_toolkit.scripts.upload_media:main'
 create-tags = 'szurubooru_toolkit.scripts.create_tags:main'
+create-relations = 'szurubooru_toolkit.scripts.create_relations:main'
 import-from-url = 'szurubooru_toolkit.scripts.import_from_url:main'
 import-from-booru = 'szurubooru_toolkit.scripts.import_from_booru:main'
 import-from-twitter = 'szurubooru_toolkit.scripts.import_from_twitter:main'
 tag-posts = 'szurubooru_toolkit.scripts.tag_posts:main'
 delete-posts = 'szurubooru_toolkit.scripts.delete_posts:main'
 reset-posts = 'szurubooru_toolkit.scripts.reset_posts:main'
+# szuru-toolkit = 'szurubooru_toolkit.scripts.szuru_toolkit:cli'
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.11,<3.12"
 beautifulsoup4="^4.10.0"
-Pillow = "^9.1.1"
+Pillow = "^9.5.0"
 Pybooru="^4.2.2"
-pygelbooru="^0.3.2"
+pygelbooru="^0.5.0"
 pysaucenao="^1.6.1"
 requests="^2.25.1"
-tqdm="^4.59.0"
-tensorflow="^2.8.0"
-keras="^2.8.0"
-numpy="^1.22.1"
-pyszuru="^0.2.4"
-tomlkit = "^0.10.0"
-syncer = "^1.3.0"
-loguru = "^0.6.0"
-pathvalidate = "^2.5.0"
-validators = "^0.18.2"
-lxml = "^4.8.0"
-tweepy = "^4.10.0"
-gallery-dl = "^1.25.1"
+tqdm="^4.65.0"
+tensorflow="^2.12.0"
+keras="^2.12.0"
+numpy="^1.23.5"
+pyszuru="^0.3.1"
+syncer = "^2.0.3"
+loguru = "^0.7.0"
+pathvalidate = "^2.5.2"
+validators = "^0.20.0"
+lxml = "^4.9.2"
+tweepy = "^4.14.0"
+gallery-dl = "^1.25.4"
+cunnypy = "^2.0.0"
+tldextract = "^3.4.4"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 flake8 = "^4.0.1"
 interrogate = "^1.5.0"
 isort = "^5.10.1"
 mkdocs = "^1.2.3"
```

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/config.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import re
+import tomllib
 import urllib
 from pathlib import Path
 
 import validators
 from loguru import logger
-from tomlkit import parse
 from validators import ValidationFailure
 
 
 class Config:
     """Holds the options set in config.toml as attributes."""
 
-    def __init__(self) -> None:
+    def __init__(self, config_file: str = 'config.toml') -> None:
         """Parse the user config (config.toml) and set this objects attributes accordingly."""
 
         try:
-            with open('config.toml') as f:
-                content = f.read()
-
+            with open(config_file, 'rb') as f:
                 try:
-                    self.config = parse(content)
+                    self.config = tomllib.load(f)
                 except Exception as e:
                     logger.critical(e)
                     exit(1)
         except FileNotFoundError as e:
             logger.critical(e)
             exit(1)
 
@@ -50,21 +48,23 @@
         """Check if necessary options in config.toml are set."""
 
         req_opts = {
             'szurubooru': ['url', 'username', 'api_token', 'public'],
             'auto_tagger': [
                 'saucenao_api_token',
                 'saucenao_enabled',
+                'md5_search_enabled',
                 'deepbooru_enabled',
                 'deepbooru_model',
                 'deepbooru_threshold',
                 'deepbooru_forced',
                 'deepbooru_set_tag',
                 'hide_progress',
                 'use_pixiv_artist',
+                'update_relations',
             ],
             'upload_media': [
                 'src_path',
                 'hide_progress',
                 'cleanup',
                 'tags',
                 'max_similarity',
@@ -75,19 +75,20 @@
                 'shrink',
                 'shrink_threshold',
                 'shrink_dimensions',
                 'default_safety',
             ],
             'import_from_booru': ['deepbooru_enabled', 'hide_progress'],
             'import_from_twitter': ['saucenao_enabled', 'deepbooru_enabled', 'hide_progress'],
-            'import_from_url': ['hide_progress', 'tmp_path'],
+            'import_from_url': ['deepbooru_enabled', 'hide_progress', 'tmp_path', 'use_twitter_artist'],
             'tag_posts': ['hide_progress'],
             'delete_posts': ['hide_progress'],
             'reset_posts': ['hide_progress'],
             'create_tags': ['hide_progress'],
+            'create_relations': ['threshold'],
             'logging': ['log_enabled', 'log_file', 'log_level', 'log_colorized'],
             'danbooru': ['user', 'api_key'],
             'gelbooru': ['user', 'api_key'],
             'konachan': ['user', 'password'],
             'yandere': ['user', 'password'],
             'sankaku': ['user', 'password'],
             'pixiv': ['user', 'password', 'token'],
```

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/danbooru.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/danbooru.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         for _ in range(1, 12):
             try:
                 logger.debug(f'Trying to fetch result by md5sum {md5sum}')
                 result = self.client.post_list(md5=md5sum)
                 logger.debug(f'Returning result: {result}')
 
                 break
+            except PybooruHTTPError as e:
+                if 'Not Found' in e._msg:
+                    result = None
+                    break
             except (TimeoutError, PybooruError, PybooruHTTPError, PybooruAPIError):
                 logger.debug('Got no result')
                 sleep(5)
         else:
             logger.debug('Could not establish connection to Danbooru, returning None...')
             result = None
```

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/deepbooru.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/deepbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/gelbooru.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/gelbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/auto_tagger.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/auto_tagger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 from __future__ import annotations
 
 import argparse
+import asyncio
 from sys import argv
 from time import sleep
 
 from loguru import logger
 from PIL import UnidentifiedImageError
 from tqdm import tqdm
 
 from szurubooru_toolkit import Post
 from szurubooru_toolkit import SauceNao
 from szurubooru_toolkit import config
 from szurubooru_toolkit import szuru
 from szurubooru_toolkit.utils import collect_sources
 from szurubooru_toolkit.utils import download_media
-from szurubooru_toolkit.utils import sanitize_tags
-from szurubooru_toolkit.utils import scrape_sankaku
+from szurubooru_toolkit.utils import prepare_post
+from szurubooru_toolkit.utils import search_boorus
 from szurubooru_toolkit.utils import shrink_img
 from szurubooru_toolkit.utils import statistics
 
 
 def parse_args() -> tuple:
     """Parse the input args to the script auto_tagger.py and set the variables accordingly."""
 
     parser = argparse.ArgumentParser(
         description='This script will automagically tag your szurubooru posts based on your input query.',
     )
 
     parser.add_argument(
-        '--sankaku-url',
-        default=None,
-        help='Fetch tags from specified Sankaku URL instead of searching SauceNAO.',
-    )
-
-    parser.add_argument(
         '--add-tags',
         default=None,
         help='Specify tags, separated by a comma, which will be added to all posts matching your query.',
     )
 
     parser.add_argument(
         '--remove-tags',
@@ -56,22 +51,19 @@
     # As -h won't get interpreted with this approach, we have to implement it manually
     if any(help_str in ['-h', '-help', '--help'] for help_str in argv):
         parser.print_help()
         exit()
     args = parser.parse_args(argv[:-1])
     query = argv[-1]
 
-    sankaku_url = args.sankaku_url
-    logger.debug(f'sankaku_url = {sankaku_url}')
-
     logger.debug(f'query = {query}')
 
-    if 'type:' in query:
-        logger.critical('Search token "type" is not allowed in queries!')
-        exit()
+    # if 'type:' in query:
+    #     logger.critical('Search token "type" is not allowed in queries!')
+    #     exit()
 
     if '\'' in query:
         logger.warning(
             'Your query contains single quotes (\'). '
             'Consider using double quotes (") if the script doesn\'t behave as intended.',
         )
 
@@ -81,54 +73,56 @@
     if add_tags:
         logger.debug(f'add_tags = {add_tags}')
         add_tags = add_tags.replace(' ', '').split(',')
     if remove_tags:
         remove_tags = remove_tags.replace(' ', '').split(',')
         logger.debug(f'remove_tags = {remove_tags}')
 
-    return sankaku_url, query, add_tags, remove_tags
+    return query, add_tags, remove_tags
 
 
-def parse_saucenao_results(sauce: SauceNao, post: Post, image: bytes) -> tuple[list, str, str, bool]:
-    """Retrieve and parse result from SauceNAO with the `image` to be uploaded.
+def get_saucenao_results(sauce: SauceNao, post: Post, image: bytes) -> tuple[list, str, str, bool]:
+    """Retrieve results from SauceNAO with the `image` to be uploaded.
 
     Args:
         sauce (SauceNao): SauceNao object.
         post (Post): szurubooru Post object.
         image (bytes): The image to uploade to upload to SauceNAO.
 
     Returns:
         tuple[list, str, str, bool]: List of tags, the source, rating and if the SauceNAO limit has been reached.
     """
 
+    results = {}
     limit_reached = False
-    tags, source, rating, limit_short, limit_long = sauce.get_metadata(post.content_url, image)
+    matches, limit_short, limit_long = asyncio.run(sauce.get_metadata(post.content_url, image))
+
+    for index, data in matches.items():
+        if data and index != 'pixiv':
+            results.update(asyncio.run(search_boorus(data['site'], f'id:{str(data["post_id"])}', 1, 0)))
 
-    # Get previously set sources and add new sources
-    source = collect_sources(*source.splitlines(), *post.source.splitlines())
+        if data and index == 'pixiv':
+            results[index] = data
 
     if not limit_long == 0:
         # Sleep 35 seconds after short limit has been reached
         if limit_short == 0:
             print('')
             logger.debug('Short limit reached for SauceNAO, trying again in 35s...')
             sleep(35)
     else:
         limit_reached = True
         print('')
         logger.info('Your daily SauceNAO limit has been reached. Consider upgrading your account.')
 
-    if tags:
-        statistics(tagged=1)
-
     if limit_reached and config.auto_tagger['deepbooru_enabled']:
         config.auto_tagger['saucenao_enabled'] = False
         logger.info('Continuing tagging with Deepbooru only...')
 
-    return sanitize_tags(tags), source, rating, limit_reached
+    return results, limit_reached
 
 
 def set_tags_from_relations(post: Post) -> None:
     """Copy artist, character and series from relations.
 
     Useful for FANBOX/Fantia sets where only the main post is uploaded to a Booru.
 
@@ -140,14 +134,26 @@
         result = szuru.api.getPost(relation['id'])
 
         for relation_tag in result.tags:
             if not relation_tag.category == 'default' or not relation_tag.category == 'meta':
                 post.tags.append(relation_tag.primary_name)
 
 
+def print_statistics(from_upload_media, total_posts):
+    if not from_upload_media:
+        total_tagged, total_deepbooru, total_untagged, total_skipped = statistics()
+
+        logger.success('Script has finished tagging.')
+        logger.success(f'Total:     {total_posts}')
+        logger.success(f'Tagged:    {str(total_tagged)}')
+        logger.success(f'Deepbooru: {str(total_deepbooru)}')
+        logger.success(f'Untagged:  {str(total_untagged)}')
+        logger.success(f'Skipped:   {str(total_skipped)}')
+
+
 @logger.catch
 def main(post_id: str = None, file_to_upload: bytes = None) -> None:  # noqa C901
     """Automatically tag posts with SauceNAO and/or Deepbooru.
 
     To auto tag a specific post, supply the `post_id` of the szurubooru post.
     You can also provide `file_to_upload` in case the file is already locally available so
     it doesn't have to get downloaded.
@@ -171,17 +177,16 @@
 
         if not config.auto_tagger['saucenao_enabled'] and not config.auto_tagger['deepbooru_enabled']:
             logger.info('Nothing to do. Enable either SauceNAO or Deepbooru in your config.')
             exit()
 
         # If posts are being tagged directly from upload-media script
         if not from_upload_media:
-            sankaku_url, query, add_tags, remove_tags = parse_args()
+            query, add_tags, remove_tags = parse_args()
         else:
-            sankaku_url = None
             query = post_id
             add_tags = None
             remove_tags = None
 
         if config.auto_tagger['saucenao_enabled']:
             sauce = SauceNao(config)
 
@@ -189,141 +194,146 @@
             from szurubooru_toolkit import Deepbooru
 
             deepbooru = Deepbooru(config.auto_tagger['deepbooru_model'])
 
         if not from_upload_media:
             logger.info(f'Retrieving posts from {config.szurubooru["url"]} with query "{query}"...')
 
-        posts = szuru.get_posts(query)
+        posts = szuru.get_posts(query, videos=True)
 
         try:
             total_posts = next(posts)
         except StopIteration:
             logger.info(f'Found no posts for your query: {query}')
             exit()
 
         if not from_upload_media:
             logger.info(f'Found {total_posts} posts. Start tagging...')
 
-        if sankaku_url:
-            if query.isnumeric():
-                post = next(posts)
-                post.tags, post.safety = scrape_sankaku(sankaku_url)
-                post.source = sankaku_url
-
-                try:
-                    szuru.update_post(post)
-                    statistics(tagged=1)
-                except Exception as e:
-                    statistics(untagged=1)
-                    logger.error(f'Could not tag post with Sankaku: {e}')
-            else:
-                logger.critical('Can only tag a single post if you specify --sankaku_url.')
-        else:
-            for index, post in enumerate(
-                tqdm(
-                    posts,
-                    ncols=80,
-                    position=0,
-                    leave=False,
-                    disable=config.auto_tagger['hide_progress'],
-                    total=int(total_posts),
-                ),
-            ):
-                tags = []
-
-                # Download the file from szurubooru if its not already locally present.
-                # This might be the case if this function was called from upload_media.
-                if not file_to_upload:
-                    if not config.szurubooru['public'] or config.auto_tagger['deepbooru_enabled']:
-                        image = download_media(post.content_url, post.md5)
-                        # Shrink files >2MB
-                        try:
-                            if len(image) > 2000000:
-                                image = shrink_img(image, resize=True, convert=True)
-                        except UnidentifiedImageError:
-                            logger.warning('Could not shrink image')
-                    else:
-                        image = None  # Let SauceNAO download the image from public szurubooru URL
+        for index, post in enumerate(
+            tqdm(
+                posts,
+                ncols=80,
+                position=0,
+                leave=False,
+                disable=config.auto_tagger['hide_progress'],
+                total=int(total_posts),
+            ),
+        ):
+            # Search boorus by md5 hash of the file
+            if config.auto_tagger['md5_search_enabled']:
+                md5_results = asyncio.run(search_boorus('all', 'md5:' + post.md5, 1, 0))
+
+                if md5_results:
+                    tags_by_md5, sources, post.rating = prepare_post(md5_results)
+                    post.source = collect_sources(*sources, *post.source.splitlines())
                 else:
-                    image = file_to_upload
+                    tags_by_md5 = []
+            else:
+                tags_by_md5 = []
 
-                if config.auto_tagger['saucenao_enabled']:
-                    tags, post.source, post.safety, limit_reached = parse_saucenao_results(
-                        sauce,
-                        post,
-                        image,
-                    )
-
-                    if add_tags:
-                        post.tags = list(set().union(post.tags, tags, add_tags))  # Keep previous tags, add user tags
-                    else:
-                        post.tags = list(set().union(post.tags, tags))  # Keep previous tags, add user tags
+            # Download the file from szurubooru if its not already locally present.
+            # This might be the case if this function was called from upload_media.
+            if not file_to_upload:
+                if (
+                    (not config.szurubooru['public'] or config.auto_tagger['deepbooru_enabled'])
+                    or config.auto_tagger['deepbooru_forced']
+                ) and post.type != 'video':
+                    image = download_media(post.content_url, post.md5)
+                    # Shrink files >2MB
+                    try:
+                        if len(image) > 2000000:
+                            image = shrink_img(image, resize=True, convert=True)
+                    except UnidentifiedImageError:
+                        logger.debug('Could not shrink image')
                 else:
-                    limit_reached = False
+                    image = None  # Let SauceNAO download the image from public szurubooru URL
+            else:
+                image = file_to_upload
 
-                if (not tags and config.auto_tagger['deepbooru_enabled']) or config.auto_tagger['deepbooru_forced']:
-                    result = deepbooru.tag_image(
-                        image,
-                        config.auto_tagger['deepbooru_threshold'],
-                        config.auto_tagger['deepbooru_set_tag'],
-                    )
-
-                    if result is None:
-                        continue
-
-                    tags, post.safety = result
-
-                    if post.relations:
-                        set_tags_from_relations(post)
-
-                    if add_tags:
-                        post.tags = list(set().union(post.tags, tags, add_tags))  # Keep previous tags and add user tags
-                    else:
-                        post.tags = list(set().union(post.tags, tags))  # Keep previous tags
-
-                    if 'DeepBooru' in post.source:
-                        post.source = post.source.replace('DeepBooru\n', '')
-                        post.source = post.source.replace('\nDeepBooru', '')
-
-                    if 'Deepbooru' not in post.source:
-                        post.source = collect_sources(post.source, 'Deepbooru')
-
-                    if tags:
-                        statistics(deepbooru=1)
-                    else:
-                        statistics(untagged=1)
-                elif not tags:
-                    statistics(untagged=1)
-
-                if remove_tags:
-                    [post.tags.remove(tag) for tag in remove_tags if tag in post.tags]
-
-                # If any tags were collected with SauceNAO or Deepbooru, remove tagme and deepbooru tag
-                if tags:
-                    [post.tags.remove(tag) for tag in post.tags if tag == 'tagme']
+            # Search SauceNAO with file
+            if config.auto_tagger['saucenao_enabled'] and post.type != 'video':
+                sauce_results, limit_reached = get_saucenao_results(sauce, post, image)
+
+                if sauce_results:
+                    tags_by_sauce, sources, post.rating = prepare_post(sauce_results)
+                    post.source = collect_sources(*sources, *post.source.splitlines())
                 else:
-                    post.tags.append('tagme')
+                    tags_by_sauce = []
+            else:
+                limit_reached = False
+                tags_by_sauce = []
 
-                szuru.update_post(post)
+            # Tag with Deepbooru.
+            pixiv_result_only = True if len(tags_by_sauce) < 2 else False
+            if (
+                (not tags_by_md5 and pixiv_result_only and config.auto_tagger['deepbooru_enabled'])
+                or config.auto_tagger['deepbooru_forced']
+            ) and post.type != 'video':
+                result = deepbooru.tag_image(
+                    image,
+                    config.auto_tagger['deepbooru_threshold'],
+                    config.auto_tagger['deepbooru_set_tag'],
+                )
+
+                if result is None:
+                    continue
+
+                tags_by_deepbooru, post.safety = result
+
+                # Deepbooru detects characters, but not the parody.
+                # Set the parody based on the character if configured.
+                if (not config.auto_tagger['saucenao_enabled'] or limit_reached) and config.auto_tagger[
+                    'update_relations'
+                ]:
+                    for tag in tags_by_deepbooru:
+                        szuru_tag = szuru.api.getTag(tag)
+                        for implication in szuru_tag.implications:
+                            szuru_implication = szuru.api.getTag(implication)
+                            if szuru_implication not in post.tags:
+                                post.tags.append(szuru_implication.primary_name)
 
-                if limit_reached and not config.auto_tagger['deepbooru_enabled']:
-                    statistics(untagged=int(total_posts) - index - 1)  # Index starts at 0
-                    break
+                if post.relations:
+                    set_tags_from_relations(post)
+            else:
+                tags_by_deepbooru = []
 
-        if not from_upload_media:
-            total_tagged, total_deepbooru, total_untagged, total_skipped = statistics()
+            # Keep previous tags and add user tags if configured
+            if add_tags:
+                post.tags = list(set().union(post.tags, tags_by_md5, tags_by_sauce, tags_by_deepbooru, add_tags))
+            else:
+                post.tags = list(set().union(post.tags, tags_by_md5, tags_by_sauce, tags_by_deepbooru))
+
+            if remove_tags:
+                [post.tags.remove(tag) for tag in remove_tags if tag in post.tags]
+
+            # If any tags were collected, remove tagme and deepbooru tag
+            if tags_by_md5 or tags_by_sauce or tags_by_deepbooru:
+                [post.tags.remove(tag) for tag in post.tags if tag == 'tagme']
+            else:
+                post.tags.append('tagme')
+
+            szuru.update_post(post)
+
+            if tags_by_md5 or tags_by_sauce:
+                statistics(tagged=1)
+
+            if tags_by_deepbooru:
+                statistics(deepbooru=1)
+
+            if not tags_by_md5 and not tags_by_sauce and not tags_by_deepbooru:
+                statistics(untagged=1)
+
+            if limit_reached and not config.auto_tagger['deepbooru_enabled']:
+                statistics(untagged=int(total_posts) - index - 1)  # Index starts at 0
+                break
 
-            logger.success('Script has finished tagging.')
-            logger.success(f'Total:     {total_posts}')
-            logger.success(f'Tagged:    {str(total_tagged)}')
-            logger.success(f'Deepbooru: {str(total_deepbooru)}')
-            logger.success(f'Untagged:  {str(total_untagged)}')
-            logger.success(f'Skipped:   {str(total_skipped)}')
+        print_statistics(from_upload_media, total_posts)
     except KeyboardInterrupt:
         print('')
         logger.info('Received keyboard interrupt from user.')
+        print_statistics(from_upload_media, total_posts)
         exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/create_tags.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/create_tags.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/delete_posts.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/delete_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_booru.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_booru.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,27 +86,28 @@
     try:
         file = download_media(file_url, md5)
     except Exception as e:
         print('')
         logger.warning(f'Could not download post from {file_url}: {e}')
         return
 
-    if booru == 'gelbooru':
-        tags = post.tags
-        safety = convert_rating(post.rating)
-        source = 'https://gelbooru.com/index.php?page=post&s=view&id=' + str(post.id)
-    elif booru == 'danbooru':
-        tags = post['tag_string'].split()
-        source = 'https://danbooru.donmai.us/posts/' + str(post['id'])
-    elif booru == 'yandere':
-        tags = post['tags'].split()
-        source = 'https://yande.re/post/show/' + str(post['id'])
-    elif booru == 'konachan':
-        tags = post['tags'].split()
-        source = 'https://konachan.com/post/show/' + str(post['id'])
+    match booru:
+        case 'gelbooru':
+            tags = post.tags
+            safety = convert_rating(post.rating)
+            source = 'https://gelbooru.com/index.php?page=post&s=view&id=' + str(post.id)
+        case 'danbooru':
+            tags = post['tag_string'].split()
+            source = 'https://danbooru.donmai.us/posts/' + str(post['id'])
+        case 'yandere':
+            tags = post['tags'].split()
+            source = 'https://yande.re/post/show/' + str(post['id'])
+        case 'konachan':
+            tags = post['tags'].split()
+            source = 'https://konachan.com/post/show/' + str(post['id'])
 
     if not booru == 'gelbooru':
         safety = convert_rating(post['rating'])
 
     metadata = {'tags': tags, 'safety': safety, 'source': source}
 
     upload_media.main(file, file_ext, metadata)
@@ -130,22 +131,23 @@
             boorus = ['danbooru', 'gelbooru', 'yandere', 'konachan']
         else:
             boorus = [booru]
 
         for booru in boorus:
             logger.info(f'Retrieving posts from {booru} with query "{query}"...')
 
-            if booru == 'danbooru':
-                booru_client = Danbooru('danbooru', config.danbooru['user'], config.danbooru['api_key'])
-            elif booru == 'gelbooru':
-                booru_client = Gelbooru(config.gelbooru['user'], config.gelbooru['api_key'])
-            elif booru == 'konachan':
-                booru_client = Moebooru('konachan', config.konachan['user'], config.konachan['password'])
-            elif booru == 'yandere':
-                booru_client = Moebooru('yandere', config.yandere['user'], config.yandere['password'])
+            match booru:
+                case 'danbooru':
+                    booru_client = Danbooru('danbooru', config.danbooru['user'], config.danbooru['api_key'])
+                case 'gelbooru':
+                    booru_client = Gelbooru(config.gelbooru['user'], config.gelbooru['api_key'])
+                case 'konachan':
+                    booru_client = Moebooru('konachan', config.konachan['user'], config.konachan['password'])
+                case 'yandere':
+                    booru_client = Moebooru('yandere', config.yandere['user'], config.yandere['password'])
 
             posts = get_posts_from_booru(booru_client, query, limit)
 
             total_posts = next(posts)
             logger.info(f'Found {total_posts} posts. Start importing...')
 
             for post in tqdm(
```

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/import_from_twitter.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_twitter.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/reset_posts.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/reset_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/tag_posts.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/tag_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/scripts/upload_media.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/upload_media.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,31 +91,37 @@
         response = requests.post(post_url, headers=szuru.headers, data=metadata)
 
         if 'description' in response.json():
             raise Exception(response.json()['description'])
         else:
             exact_post = response.json()['exactPost']
             similar_posts = response.json()['similarPosts']
-            return exact_post, similar_posts
+            errors = False
+            return exact_post, similar_posts, errors
     except Exception as e:
-        logger.critical(f'An error occured during the similarity check: {e}')
+        print('')
+        logger.warning(f'An error occured during the similarity check: {e}. Skipping post...')
+        errors = True
+        return False, [], errors
 
 
 def upload_file(szuru: Szurubooru, post: Post) -> None:
     """Uploads/Moves our temporary image to 'production' with similar posts if any were found.
 
     Deletes file after upload has been completed.
 
     Args:
         szuru (Szurubooru): Szurubooru object to interact with the API.
         post (Post): Post object with attr `similar_posts` and `image_token`.
-        file_to_upload (str): Local file path of the file to upload.
 
     Raises:
         Exception
+
+    Returns:
+        None
     """
 
     safety = post.safety if post.safety else config.upload_media['default_safety']
     source = post.source if post.source else ''
 
     post_url = szuru.szuru_api_url + '/posts'
     metadata = json.dumps(
@@ -133,26 +139,29 @@
 
         if 'description' in response.json():
             raise Exception(response.json()['description'])
         else:
             return response.json()['id']
     except Exception as e:
         print('')
-        logger.warning(f'An error occured during the upload for file "{post.file_to_upload}": {e}')
+        logger.warning(f'An error occured during the upload for file "{post.file_path}": {e}')
         return None
 
 
 def cleanup_dirs(dir: str) -> None:
     """Remove empty directories recursively from bottom to top.
 
     Args:
         dir (str): The directory under which to cleanup - dir is the root level and won't get deleted.
 
     Raises:
         OSError
+
+    Returns:
+        None
     """
 
     for root, dirs, files in os.walk(dir, topdown=False):
         for name in files:
             # Remove Thumbs.db file created by Windows
             if name == 'Thumbs.db':
                 os.remove(os.path.join(root, name))
@@ -221,60 +230,77 @@
     except OSError:
         print('')
         logger.warning(f'Could not shrink image {file_to_upload}. Keeping dimensions...')
 
     return image
 
 
-def upload_post(file: bytes, file_ext: str, metadata: dict = None, file_to_upload: str = None) -> None:
+def upload_post(file: bytes, file_ext: str, metadata: dict = None, file_path: str = None) -> bool:
+    """Uploads given file to temporary file space in szurubooru.
+
+    Args:
+        file (bytes): The file as bytes
+        file_ext (str): The file extension
+        metadata (dict, optional): Attach metadata to the post. Defaults to None.
+        file_path (str, optional): The path to the file (used for debugging). Defaults to None.
+
+    Returns:
+        bool: If the upload was successful or not
+    """
+
     post = Post()
 
     if file_ext not in ['mp4', 'webm', 'gif']:
-        post.media = eval_convert_image(file, file_ext, file_to_upload)
+        post.media = eval_convert_image(file, file_ext, file_path)
     else:
         post.media = file
 
     post.token = get_media_token(szuru, post.media)
-    post.exact_post, similar_posts = check_similarity(szuru, post.token)
+    post.exact_post, similar_posts, errors = check_similarity(szuru, post.token)
+
+    if errors:
+        return False
+
     threshold = 1 - float(config.upload_media['max_similarity'])
 
     for entry in similar_posts:
         if entry['distance'] < threshold and not post.exact_post:
             print()
             logger.debug(
-                f'File "{file_to_upload} is too similar to post {entry["post"]["id"]} ({100 - entry["distance"]}%)',
+                f'File "{file_path} is too similar to post {entry["post"]["id"]} ({100 - entry["distance"]}%)',
             )
             post.exact_post = True
             break
 
     if not post.exact_post:
         if not metadata:
             post.tags = config.upload_media['tags']
             post.safety = None
             post.source = None
         else:
             post.tags = metadata['tags']
             post.safety = metadata['safety']
             post.source = metadata['source']
 
-        post.file_to_upload = file_to_upload
+        post.file_path = file_path
 
         post.similar_posts = []
         for entry in similar_posts:
             post.similar_posts.append(entry['post']['id'])
 
         post_id = upload_file(szuru, post)
 
         if not post_id:
             return
 
         # Tag post if enabled
         if config.upload_media['auto_tag']:
-            if file_ext not in ['mp4', 'webm']:
-                auto_tagger(str(post_id), post.media)
+            auto_tagger(str(post_id), post.media)
+
+    return True
 
 
 def main(file_to_upload: bytes = None, file_ext: str = None, metadata: dict = None) -> int:
     """Main logic of the script."""
 
     try:
         if not file_to_upload:
@@ -285,28 +311,28 @@
             from_import_from = True
             config.upload_media['hide_progress'] = True
 
         if files_to_upload:
             if not from_import_from:
                 logger.info('Found ' + str(len(files_to_upload)) + ' file(s). Starting upload...')
 
-                for file_to_upload in tqdm(
+                for file_path in tqdm(
                     files_to_upload,
                     ncols=80,
                     position=0,
                     leave=False,
                     disable=config.upload_media['hide_progress'],
                 ):
-                    with open(file_to_upload, 'rb') as f:
+                    with open(file_path, 'rb') as f:
                         file = f.read()
-                    upload_post(file, file_ext=Path(file_to_upload).suffix[1:], file_to_upload=file_to_upload)
+                    success = upload_post(file, file_ext=Path(file_path).suffix[1:], file_path=file_path)
 
-                    if config.upload_media['cleanup']:
-                        if os.path.exists(file_to_upload):
-                            os.remove(file_to_upload)
+                    if config.upload_media['cleanup'] and success:
+                        if os.path.exists(file_path):
+                            os.remove(file_path)
 
                 if config.upload_media['cleanup']:
                     cleanup_dirs(config.upload_media['src_path'])  # Remove dirs after files have been deleted
 
                 if not from_import_from:
                     logger.success('Script has finished uploading!')
             else:
```

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/szurubooru.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/szurubooru.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,73 @@
 
         token = self.encode_auth_headers(szuru_user, szuru_token)
         self.headers = {'Accept': 'application/json', 'Authorization': 'Token ' + token}
 
         # Use the api object to interact with pyszuru module
         self.api = pyszuru.API(base_url=szuru_url, username=szuru_user, token=szuru_token)
 
+        self.allowed_tokens = [
+            'ar',
+            'area',
+            'aspect-ratio',
+            'comment',
+            'comment-count',
+            'comment-date',
+            'comment-time',
+            'content-checksum',
+            'creation-date',
+            'creation-time',
+            'date',
+            'disliked',
+            'edit-date',
+            'edit-time',
+            'fav',
+            'fav-count',
+            'fav-date',
+            'fav-time',
+            'feature-count',
+            'feature-date',
+            'feature-time',
+            'file-size',
+            'flag',
+            'height',
+            'id',
+            'image-ar',
+            'image-area',
+            'image-aspect-ratio',
+            'image-height',
+            'image-width',
+            'last-edit-date',
+            'last-edit-time',
+            'liked',
+            'md5',
+            'note-count',
+            'note-text',
+            'pool',
+            'rating',
+            'relation-count',
+            'safety',
+            'score',
+            'sha1',
+            'source',
+            'submit',
+            'tag',
+            'tag-count',
+            'time',
+            'type',
+            'upload',
+            'uploader',
+            'width',
+            'sort',
+            'liked',
+            'disliked',
+            'fav',
+            'tumbleweed',
+        ]
+
     def get_posts(
         self,
         query: str,
         pagination: bool = True,
         videos: bool = False,
     ) -> Generator[str | Post, None, None]:
         """Return the found post ids of the supplied query.
@@ -60,14 +119,23 @@
             Generator[str | Post, None, None]: Will yield the total amount of search results first, then Post objects.
         """
 
         if query.isnumeric():
             query = 'id:' + query
             logger.debug(f'Modified input query to "{query}"')
 
+        if ':' in query:
+            query_list = query.split()
+            for tag in query_list:
+                if ':' in tag:
+                    token = tag.split(':')[0]
+                    if token not in self.allowed_tokens and token not in ['-' + t for t in self.allowed_tokens]:
+                        sanitized_tag = tag.replace(':', '\\:')  # noqa W605
+                        query = query.replace(tag, sanitized_tag)
+
         try:
             if videos:
                 query_params = {'query': query}
             else:
                 query_params = {'query': f'type:image,animation {query}'}
             query_url = self.szuru_api_url + '/posts/?' + urllib.parse.urlencode(query_params)
             logger.debug(f'Getting post from query_url: {query_url}')
@@ -75,15 +143,15 @@
             response_json = requests.get(query_url, headers=self.headers)
             response = response_json.json()
             # logger.debug(f'Got following response: {response}')
 
             if 'name' in response and response['name'] == 'SearchError':
                 print('')
                 logger.critical(f'{response["name"]}: {response["description"]}')
-                exit()
+                raise UnknownTokenError(response['description'])
 
             total = str(response['total'])
             logger.debug(f'Got a total of {total} results')
 
             results = response['results']
             # logger.debug(f'Got following results: {results}')
             pages = ceil(int(total) / 100)  # Max posts per pages is 100
@@ -127,14 +195,15 @@
         post.id = str(response['id'])
         post.source = response['source'] if response['source'] else ''
         content_url = response['contentUrl']
         post.content_url = self.szuru_url + '/' + content_url
         post.version = response['version']
         post.relations = response['relations']
         post.md5 = response['checksumMD5']
+        post.type = response['type']
         post.safety = response['safety']
 
         tags = response['tags']
         post.tags = []
 
         for tag in tags:
             post.tags.append(tag['names'][0])
@@ -247,14 +316,16 @@
         self.id: str = None
         self.source: str = None
         self.content_url: str = None
         self.version = None
         self.relations: list = []
         self.tags: list = []
         self.safety = 'safe'
+        self.md5 = None
+        self.type = None
 
     def __repr__(self) -> str:
         """Returns the current attributes of this object.
 
         Returns:
             str: A formatted string with currently set attributes.
         """
@@ -279,7 +350,13 @@
     pass
 
 
 class TagExistsError(SzurubooruError):
     """Raise if the tag already exists."""
 
     pass
+
+
+class UnknownTokenError(SzurubooruError):
+    """Raise if the search token does not valid."""
+
+    pass
```

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/twitter.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/twitter.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.8.1/src/szurubooru_toolkit/utils.py` & `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from __future__ import annotations
 
 import hashlib
 import sys
 import warnings
+from asyncio import sleep
+from asyncio.exceptions import CancelledError
 from io import BytesIO
 from math import ceil
+from typing import Any
 from typing import Iterator
 from urllib.error import ContentTooShortError
 
 import bs4
+import cunnypy
 import requests
+from httpx import HTTPStatusError
+from httpx import ReadTimeout
 from loguru import logger
 from lxml import etree
 from PIL import Image
 from pybooru import Moebooru
 from pybooru.exceptions import PybooruHTTPError
 from pygelbooru.gelbooru import GelbooruImage
 from syncer import sync
@@ -25,15 +31,26 @@
 
 # Keep track of total tagged posts
 total_tagged = 0
 total_deepbooru = 0
 total_untagged = 0
 total_skipped = 0
 
-warnings.simplefilter('error', Image.DecompressionBombWarning)
+
+# Define a filter function to ignore the DecompressionBombWarning
+def ignore_decompression_bomb_warning(message, category, filename, lineno, file=None, line=None):
+    if isinstance(message, Image.DecompressionBombWarning):
+        return
+    else:
+        return warnings.defaultaction(message, category, filename, lineno, file, line)
+
+
+# Set the filter to ignore the warning
+warnings.filterwarnings('ignore', category=Image.DecompressionBombWarning)
+warnings.showwarning = ignore_decompression_bomb_warning
 warnings.filterwarnings('ignore', '.*Palette images with Transparency.*', module='PIL')
 
 
 def shrink_img(
     tmp_file: bytes,
     resize: bool = False,
     shrink_threshold: int = None,
@@ -99,14 +116,15 @@
     Example:
         convert_rating('rating:safe') -> 'safe'
     """
     switch = {
         'Safe': 'safe',
         'safe': 'safe',
         's': 'safe',
+        'g': 'safe',
         'Questionable': 'sketchy',
         'questionable': 'sketchy',
         'q': 'sketchy',
         'Explicit': 'unsafe',
         'explicit': 'unsafe',
         'e': 'unsafe',
         'rating:safe': 'safe',
@@ -258,19 +276,15 @@
 
     delimiter = '\n'
     source_collected = delimiter.join(source_valid)
     return source_collected
 
 
 def setup_logger(config: Config) -> None:
-    """Setup loguru logging handlers.
-
-    Args:
-        config (Config): Config object with user configuration from `config.toml`.
-    """
+    """Setup loguru logging handlers."""
 
     logger.configure(
         handlers=[
             dict(
                 sink=config.logging['log_file'],
                 colorize=config.logging['log_colorized'],
                 level=config.logging['log_level'],
@@ -431,7 +445,150 @@
                 results = booru.post_list(limit=limit, tags=query)
             except PybooruHTTPError:
                 logger.critical('Importing from Danbooru accepts only a maximum of two tags for you search query!')
                 exit()
 
     yield len(results)
     yield from results
+
+
+def generate_src(metadata: dict) -> str:
+    """Generate and return post source URL.
+
+    Args:
+        metadata (dict): Contains the site and id of the post
+
+    Returns:
+        str: The source URL of the post.
+    """
+
+    if 'id' in metadata:
+        id = str(metadata['id'])
+
+    try:
+        match metadata['site']:
+            case 'danbooru':
+                src = 'https://danbooru.donmai.us/posts/' + id
+            case 'e-hentai':
+                id = str(metadata['gid'])
+                token = metadata['token']
+                src = f'https://e-hentai.org/g/{id}/{token}'
+            case 'gelbooru':
+                src = 'https://gelbooru.com/index.php?page=post&s=view&id=' + id
+            case 'konachan':
+                src = 'https://konachan.com/post/show/' + id
+            case 'sankaku':
+                src = 'https://chan.sankakucomplex.com/post/show/' + id
+            case 'yandere':
+                src = 'https://yande.re/post/show/' + id
+            case 'twitter':
+                user = metadata['author']['name']
+                id = str(metadata['tweet_id'])
+                src = f'https://twitter.com/{user}/status/{id}'
+            case 'kemono':
+                user = metadata['user']
+                id = metadata['id']
+                service = metadata['service']
+                src = f'https://kemono.party/{service}/user/{user}/post/{id}'
+            case _:
+                src = None
+    except KeyError:
+        src = None
+
+    return src
+
+
+async def search_boorus(booru: str, query: str, limit: int, page: int = 1) -> dict:
+    results = {}
+
+    boorus_to_search = ['sankaku', 'danbooru', 'gelbooru', 'konachan', 'yandere'] if booru == 'all' else [booru]
+    for booru in boorus_to_search:
+        for attempt in range(1, 12):
+            try:
+                result = await cunnypy.search(booru, query, limit, page)
+                if result:
+                    results[booru] = result
+                break
+            except (KeyError, ExceptionGroup, CancelledError):
+                logger.debug(f'No result found in {booru} with "{query}"')
+                break
+            except (HTTPStatusError, ReadTimeout):
+                logger.debug(f'Could not establish connection to {booru}. Trying again in 5s...')
+                if attempt < 11:  # no need to sleep on the last attempt
+                    await sleep(5)
+            except Exception as e:
+                logger.debug(f'Could not get result from {booru} with "{query}": {e}. Trying again. in 5s...')
+                if attempt < 11:  # no need to sleep on the last attempt
+                    await sleep(5)
+        else:
+            logger.debug(f'Could not establish connection to {booru}, trying with next post...')
+            statistics(skipped=1)
+
+    return results
+
+
+def prepare_post(results: dict):
+    tags = []
+    sources = []
+    rating = []
+
+    for booru, result in results.items():
+        if booru != 'pixiv':
+            tags.append(result[0].tags.split())
+            sources.append(generate_src({'site': booru, 'id': result[0].id}))
+            rating = convert_rating(result[0].rating)
+        else:
+            pixiv_sources, pixiv_artist = extract_pixiv_artist(results['pixiv'])
+            sources.append(pixiv_sources)
+
+    final_tags = [item for sublist in tags for item in sublist]
+
+    if not final_tags and 'pixiv' in results and pixiv_artist:
+        final_tags = pixiv_artist
+
+    return final_tags, sources, rating
+
+
+def extract_pixiv_artist(result: Any) -> tuple[str, list]:
+    pixiv_artist = result.author_name
+    source = result.url
+    from szurubooru_toolkit import config
+    from szurubooru_toolkit import danbooru_client
+    from szurubooru_toolkit import szuru
+
+    if pixiv_artist:
+        artist = danbooru_client.search_artist(pixiv_artist)
+        if not artist and config.auto_tagger['use_pixiv_artist']:
+            artist = pixiv_artist.lower().replace(' ', '_')
+            try:
+                szuru.create_tag(artist, category='artist', overwrite=True)
+            except Exception as e:
+                logger.debug(f'Could not create pixiv artist {pixiv_artist}: {e}')
+    else:
+        artist = None
+
+    return source, [artist]
+
+
+def extract_twitter_artist(metadata: dict) -> str:
+    from szurubooru_toolkit import config
+    from szurubooru_toolkit import danbooru_client
+    from szurubooru_toolkit import szuru
+
+    twitter_name = metadata['author']['name']
+    twitter_nick = metadata['author']['nick']
+    artist_aliases = None
+
+    artist = danbooru_client.search_artist(twitter_name)
+    if not artist:
+        artist = danbooru_client.search_artist(twitter_nick)
+
+    if not artist and config.import_from_url['use_twitter_artist']:
+        artist_aliases = [twitter_name.lower().replace(' ', '_')]
+        artist_aliases.append(twitter_nick.lower().replace(' ', '_'))
+        for artist_alias in artist_aliases:
+            try:
+                szuru.create_tag(artist_alias, category='artist', overwrite=True)
+            except Exception as e:
+                logger.debug(f'Could not create Twitter artist {artist_alias}: {e}')
+
+    return [artist] if not artist_aliases else artist_aliases
```

### Comparing `szurubooru_toolkit-0.8.1/PKG-INFO` & `szurubooru_toolkit-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: szurubooru-toolkit
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python package and script collection to manage szurubooru.
 Home-page: https://github.com/reluce/szurubooru-toolkit
 License: GPL-3.0-only
 Keywords: szurubooru,szuru,booru,saucenao,deepbooru
 Author: reluce
 Author-email: reluce@fkosquad.moe
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Pillow (>=9.1.1,<10.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.5.0,<10.0.0)
 Requires-Dist: Pybooru (>=4.2.2,<5.0.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
-Requires-Dist: gallery-dl (>=1.25.1,<2.0.0)
-Requires-Dist: keras (>=2.8.0,<3.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: lxml (>=4.8.0,<5.0.0)
-Requires-Dist: numpy (>=1.22.1,<2.0.0)
-Requires-Dist: pathvalidate (>=2.5.0,<3.0.0)
-Requires-Dist: pygelbooru (>=0.3.2,<0.4.0)
+Requires-Dist: cunnypy (>=2.0.0,<3.0.0)
+Requires-Dist: gallery-dl (>=1.25.4,<2.0.0)
+Requires-Dist: keras (>=2.12.0,<3.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
+Requires-Dist: pygelbooru (>=0.5.0,<0.6.0)
 Requires-Dist: pysaucenao (>=1.6.1,<2.0.0)
-Requires-Dist: pyszuru (>=0.2.4,<0.3.0)
+Requires-Dist: pyszuru (>=0.3.1,<0.4.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: syncer (>=1.3.0,<2.0.0)
-Requires-Dist: tensorflow (>=2.8.0,<3.0.0)
-Requires-Dist: tomlkit (>=0.10.0,<0.11.0)
-Requires-Dist: tqdm (>=4.59.0,<5.0.0)
-Requires-Dist: tweepy (>=4.10.0,<5.0.0)
-Requires-Dist: validators (>=0.18.2,<0.19.0)
+Requires-Dist: syncer (>=2.0.3,<3.0.0)
+Requires-Dist: tensorflow (>=2.12.0,<3.0.0)
+Requires-Dist: tldextract (>=3.4.4,<4.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: tweepy (>=4.14.0,<5.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
 Project-URL: Documentation, https://github.com/reluce/szurubooru-toolkit
 Project-URL: Repository, https://github.com/reluce/szurubooru-toolkit
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://cdn-icons-png.flaticon.com/512/2581/2581053.png"
   alt="szurubooru-toolkit icon"
@@ -138,15 +137,15 @@
 | `twitter` | `access_token` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
 | `twitter` | `access_token_secret` | See https://developer.twitter.com/en/docs/authentication/oauth-1-0a | `"None"` |
 | `upload_media` | `src_path` | Every valid media file under this dir (recursively) will get uploaded | `"/local/path/to/upload/dir"` |
 | `upload_media` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `upload_media` | `cleanup` | Set this to true if images in the `src_path` should be deleted after upload | `false` |
 | `upload_media` | `tags` | These tags will get set for all uploaded posts. Separate them by a comma. | `["tagme", "tag1", "tag2", "tagN"]` |
 | `upload_media` | `auto_tag` | Set this to true if you want your post to be automatically tagged after upload | `false` |
-| `upload_media` | `max_similarity` | Adjust this value to ignore posts if a similar post higher than the threshold has already been uploaded | `"0.99"` |
+| `upload_media` | `max_similarity` | Adjust this value to ignore posts if a similar post higher than the threshold has already been uploaded. 1.00 being basically the same image, but not necessarily. Set to 1.00 if you know there are not duplicates. | `"0.99"` |
 | `upload_media` | `convert_to_jpg` | Convert images to JPG to save disk space. This won't overwrite the source files and only affects the uploaded image. Images might slip through identical post check. | `false` |
 | `upload_media` | `convert_quality` | Only images above this threshold will be converted to jpg if `convert_to_jpg` is True. | `"3MB\|500KB"` |
 | `upload_media` | `shrink` | Set to true to shrink images to shrink_dimensions based on shrink_threshold below. Images might slip through identical post check. | `false` |
 | `upload_media` | `shrink_threshold` | Images which total pixel size exceeds this treshold will be resized to `shrink_size`. E.g. 2000x3000 results in 6000000. | `"6000000"` |
 | `upload_media` | `shrink_dimensions` | Set the max value for width/height. Keeps aspect ratio. E.g. 2000x4000 results in 700x1400, 4000x2000 in 1400x700 (with `"1400x1400"`). | `"2500x2500"` |
 | `upload_media` | `default_safety` | # Set the default safety in case neither SauceNAO, nor Deepbooru could determine it | `safe` |
 | `import_from_booru` | `deepbooru_enabled` | Apply Deepbooru tagging additionally besides fetched tags from Booru | `false` |
```

