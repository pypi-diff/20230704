# Comparing `tmp/ofscraper-2.6.3.tar.gz` & `tmp/ofscraper-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.6.3.tar", max compression
+gzip compressed data, was "ofscraper-2.6.4.tar", max compression
```

## Comparing `ofscraper-2.6.3.tar` & `ofscraper-2.6.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1067 2023-07-01 17:49:04.668305 ofscraper-2.6.3/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-01 17:49:04.668305 ofscraper-2.6.3/README.md
--rw-r--r--   0        0        0      607 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     8526 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/archive.py
--rw-r--r--   0        0        0     5019 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/init.py
--rw-r--r--   0        0        0     2859 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/me.py
--rw-r--r--   0        0        0     9222 2023-07-01 17:49:04.672305 ofscraper-2.6.3/ofscraper/api/messages.py
--rw-r--r--   0        0        0    10084 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5672 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11976 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3909 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3408 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     8918 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    14531 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/commands/check.py
--rw-r--r--   0        0        0     4942 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    13717 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6339 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     5037 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      696 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7683 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    27832 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1209 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    11211 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8986 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10803 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    20240 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3376 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     6486 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     9615 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/of.py
--rw-r--r--   0        0        0    11732 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0    29248 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/table.py
--rw-r--r--   0        0        0     5811 2023-07-01 17:49:04.676305 ofscraper-2.6.3/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1759 2023-07-01 17:49:35.624240 ofscraper-2.6.3/pyproject.toml
--rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 ofscraper-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-01 20:38:09.278774 ofscraper-2.6.4/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-01 20:38:09.278774 ofscraper-2.6.4/README.md
+-rw-r--r--   0        0        0      607 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     8526 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     5019 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2859 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9222 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    10084 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5672 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11976 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3909 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3408 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     8918 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    14531 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     4942 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    13967 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6339 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     5037 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      696 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7683 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    27832 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1209 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-07-01 20:38:09.286774 ofscraper-2.6.4/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    11211 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8986 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10803 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    20240 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3376 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     6486 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     9615 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/of.py
+-rw-r--r--   0        0        0    11732 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0    29248 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/table.py
+-rw-r--r--   0        0        0     5818 2023-07-01 20:38:09.290774 ofscraper-2.6.4/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1759 2023-07-01 20:38:42.271109 ofscraper-2.6.4/pyproject.toml
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 ofscraper-2.6.4/PKG-INFO
```

### Comparing `ofscraper-2.6.3/LICENSE` & `ofscraper-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/README.md` & `ofscraper-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/__init__.py` & `ofscraper-2.6.4/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/__version__.py` & `ofscraper-2.6.4/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/archive.py` & `ofscraper-2.6.4/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/highlights.py` & `ofscraper-2.6.4/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/init.py` & `ofscraper-2.6.4/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/me.py` & `ofscraper-2.6.4/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/messages.py` & `ofscraper-2.6.4/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/paid.py` & `ofscraper-2.6.4/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/pinned.py` & `ofscraper-2.6.4/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/posts.py` & `ofscraper-2.6.4/ofscraper/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/profile.py` & `ofscraper-2.6.4/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/subscriptions.py` & `ofscraper-2.6.4/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/api/timeline.py` & `ofscraper-2.6.4/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/commands/check.py` & `ofscraper-2.6.4/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/commands/manual.py` & `ofscraper-2.6.4/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/commands/scraper.py` & `ofscraper-2.6.4/ofscraper/commands/scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         if args.users_first:
             output=[]
             userdata=userselector.getselected_usernames(rescan=False)
             length=len(userdata)
             for count,ele in enumerate(userdata):
-                log.debug(f"getting content for {count+1}/{length} model")
+                log.info(f"Progress {count+1}/{length} model")
                 if args.posts:
                     log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
                     model_id = profile.get_id( ele["name"])
                     operations.create_tables(model_id,ele['name'])
                     operations.write_profile_table(model_id,ele['name'])
                     output.extend(OF.process_areas( ele, model_id)) 
@@ -162,16 +162,16 @@
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         userdata=userselector.getselected_usernames(rescan=False)
         length=len(userdata)
         for count,ele in enumerate(userdata):
+            log.info(f"Progress {count+1}/{length} model")
             if args.posts:
-                log.info(f"Progress {count+1}/{length} model")
                 log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
             try:
                 model_id = profile.get_id( ele["name"])
                 operations.create_tables(model_id,ele['name'])
                 operations.write_profile_table(model_id,ele['name'])
                 combined_urls=OF.process_areas( ele, model_id)
                 asyncio.run(download.process_dicts(
@@ -204,16 +204,19 @@
 
 def process_like():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         userdata=userselector.getselected_usernames(rescan=False)
+        active=list(filter(lambda x: x["active"],userdata))
+        length=len(active)
         with stdout.lowstdout():
-            for ele in list(filter(lambda x: x["active"],userdata)):
+            for count,ele in enumerate(active):
+                    log.info(f"Progress {count+1}/{length} model")
                     model_id = profile.get_id( ele["name"])
                     posts = like.get_posts(model_id)
                     unfavorited_posts = like.filter_for_unfavorited(posts)  
                     unfavorited_posts=filters.timeline_array_filter(unfavorited_posts)   
                     log.debug(f"[bold]Number of unliked posts left after date filters[/bold] {len(unfavorited_posts)}")
                     post_ids = like.get_post_ids(unfavorited_posts)
                     log.debug(f"[bold]Final Number of open and likable post[/bold] {len(post_ids)}")
@@ -221,16 +224,19 @@
 
 def process_unlike():
     with scrape_context_manager(): 
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         userdata=userselector.getselected_usernames(rescan=False)
+        active=list(filter(lambda x: x["active"],userdata))
+        length=len(active)
         with stdout.lowstdout():
-            for ele in list(filter(lambda x: x["active"],userdata)):
+            for count,ele in enumerate(active):
+                    log.info(f"Progress {count+1}/{length} model")
                     model_id = profile.get_id( ele["name"])
                     posts = like.get_posts( model_id)
                     favorited_posts = like.filter_for_favorited(posts)
                     favorited_posts=filters.timeline_array_filter(favorited_posts) 
                     log.debug(f"[bold]Number of liked posts left after date filters[/bold] {len(favorited_posts)}")
                     post_ids = like.get_post_ids(favorited_posts)
                     log.debug(f"[bold]Final Number of open and unlikable post[/bold] {len(post_ids)}")
```

### Comparing `ofscraper-2.6.3/ofscraper/constants.py` & `ofscraper-2.6.4/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/db/operations.py` & `ofscraper-2.6.4/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/db/queries.py` & `ofscraper-2.6.4/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/interaction/like.py` & `ofscraper-2.6.4/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.6.4/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.6.4/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/prompts/prompts.py` & `ofscraper-2.6.4/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/start.py` & `ofscraper-2.6.4/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/args.py` & `ofscraper-2.6.4/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/auth.py` & `ofscraper-2.6.4/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/binaries.py` & `ofscraper-2.6.4/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/config.py` & `ofscraper-2.6.4/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/dates.py` & `ofscraper-2.6.4/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/download.py` & `ofscraper-2.6.4/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/encoding.py` & `ofscraper-2.6.4/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/exit.py` & `ofscraper-2.6.4/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/filters.py` & `ofscraper-2.6.4/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/logger.py` & `ofscraper-2.6.4/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/of.py` & `ofscraper-2.6.4/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/paths.py` & `ofscraper-2.6.4/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/profiles.py` & `ofscraper-2.6.4/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/separate.py` & `ofscraper-2.6.4/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/stdout.py` & `ofscraper-2.6.4/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/table.py` & `ofscraper-2.6.4/ofscraper/utils/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6.3/ofscraper/utils/userselector.py` & `ofscraper-2.6.4/ofscraper/utils/userselector.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
            args_.changeargs(args)
     if rescan==True:
         parsed_subscriptions=None
     if not parsed_subscriptions or not args.username:
         selectuserhelper()
 
     usernameset=set(args.username)
-    return list(filter(lambda x:x["name"] in usernameset,parsed_subscriptions)) if args.username!="ALL" else parsed_subscriptions
+    return list(filter(lambda x:x["name"] in usernameset,parsed_subscriptions)) if "ALL" not in args.username else parsed_subscriptions
     
-def selectuserhelper():
+def selectuserhelper(): 
     headers = auth.make_headers(auth.read_auth())
     subscribe_count = process_me(headers)
     global parsed_subscriptions
     all_subs = get_models(headers, subscribe_count)
     if not args.username: 
         selected=None
         while True:
```

### Comparing `ofscraper-2.6.3/pyproject.toml` & `ofscraper-2.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.6.3"
+version = "2.6.4"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-2.6.3/PKG-INFO` & `ofscraper-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.6.3
+Version: 2.6.4
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

