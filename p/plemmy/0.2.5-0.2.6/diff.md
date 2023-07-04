# Comparing `tmp/plemmy-0.2.5.tar.gz` & `tmp/plemmy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.2.5.tar", last modified: Fri Jun 30 20:44:48 2023, max compression
+gzip compressed data, was "plemmy-0.2.6.tar", last modified: Tue Jul  4 01:27:26 2023, max compression
```

## Comparing `plemmy-0.2.5.tar` & `plemmy-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-30 20:44:48.100899 plemmy-0.2.5/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.5/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-30 20:44:48.100728 plemmy-0.2.5/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.5/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-30 20:44:48.099532 plemmy-0.2.5/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.5/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    70949 2023-06-24 16:56:44.000000 plemmy-0.2.5/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-06-30 20:43:38.000000 plemmy-0.2.5/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-30 20:43:24.000000 plemmy-0.2.5/plemmy/version.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-30 20:44:48.100495 plemmy-0.2.5/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-30 20:44:48.100948 plemmy-0.2.5/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.5/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-04 01:27:26.043209 plemmy-0.2.6/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.6/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-07-04 01:27:26.043018 plemmy-0.2.6/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.6/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-04 01:27:26.041907 plemmy-0.2.6/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.6/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-04 01:27:01.000000 plemmy-0.2.6/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-06-30 20:43:38.000000 plemmy-0.2.6/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-04 01:27:01.000000 plemmy-0.2.6/plemmy/version.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-04 01:27:26.042808 plemmy-0.2.6/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-04 01:27:26.043258 plemmy-0.2.6/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.6/setup.py
```

### Comparing `plemmy-0.2.5/LICENSE` & `plemmy-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.5/PKG-INFO` & `plemmy-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.2.5/README.md` & `plemmy-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.5/plemmy/lemmyhttp.py` & `plemmy-0.2.6/plemmy/lemmyhttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,41 +815,43 @@
             None
 
         Returns:
             requests.Response: result of API call
         """
 
         form = {"auth": self.key}
-        return get_handler(f"{self._api_url}/user/banned", self._headers, form)
+        return get_handler(f"{self._api_url}/user/banned", self._headers,
+                           None, params=form)
 
     def get_captcha(self) -> requests.Response:
         """ get_captcha: get captcha for current user
 
         Args:
             None
 
         Returns:
             requests.Response: result of API call
         """
 
         return get_handler(f"{self._api_url}/user/get_captcha",
-                           self._headers, {})
+                           self._headers, None, None)
 
     def get_comment(self, id: int) -> requests.Response:
         """ get_comment: obtain a comment by ID
 
         Args:
             id (int): comment ID
 
         Returns:
             requests.Response: result of API call
         """
 
         form = {"id": id, "auth": self.key}
-        return get_handler(f"{self._api_url}/comment", self._headers, form)
+        return get_handler(f"{self._api_url}/comment", self._headers,
+                           None, params=form)
 
     def get_comments(self, community_id: int = None,
                      community_name: str = None, limit: int = None,
                      max_depth: int = None, page: int = None,
                      parent_id: int = None, post_id: int = None,
                      saved_only: bool = None, sort: str = None,
                      type_: str = None) -> requests.Response:
@@ -874,15 +876,15 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/comment/list",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def get_community(self, id: int = None,
                       name: str = None) -> requests.Response:
         """ get_community: get a community
 
         Args:
             id (int): ID of community (optional)
@@ -905,15 +907,15 @@
 
         Returns:
             requests.Response: result of API call
         """
 
         form = {"auth": self.key}
         return get_handler(f"{self._api_url}/federated_instances",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def get_modlog(self, type_: str, community_id: int = None,
                    limit: int = None, mod_person_id: int = None,
                    other_person_id: int = None,
                    page: int = None) -> requests.Response:
         """ get_modlog: obtain the moderation log
 
@@ -933,15 +935,16 @@
 
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
-        return get_handler(f"{self._api_url}/modlog", self._headers, form)
+        return get_handler(f"{self._api_url}/modlog", self._headers,
+                           None, params=form)
 
     def get_person_details(self, community_id: int = None, limit: int = None,
                            page: int = None, person_id: int = None,
                            saved_only: bool = None, sort: str = None,
                            username: str = None) -> requests.Response:
         """ get_person_details: get information for a user
 
@@ -959,15 +962,16 @@
 
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
-        return get_handler(f"{self._api_url}/user", self._headers, form)
+        return get_handler(f"{self._api_url}/user", self._headers,
+                           None, params=form)
 
     def get_person_mentions(self, limit: int = None, page: int = None,
                             sort: str = None,
                             unread_only: bool = None) -> requests.Response:
         """ get_person_mentions: obtain comments where current user is
         mentioned
 
@@ -981,15 +985,15 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/user/mention",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def get_post(self, comment_id: int = None,
                  id: int = None) -> requests.Response:
         """ get_post: get post from post ID or comment ID
 
         Args:
             comment_id (int): ID of comment in post (optional)
@@ -997,15 +1001,16 @@
 
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
-        return get_handler(f"{self._api_url}/post", self._headers, form)
+        return get_handler(f"{self._api_url}/post", self._headers,
+                           None, params=form)
 
     def get_posts(self, community_id: int = None, community_name: str = None,
                   limit: int = None, page: int = None, saved_only: bool = None,
                   sort: str = None,
                   type_: str = None) -> requests.Response:
         """ get_posts: obtain posts from a community
 
@@ -1023,15 +1028,16 @@
 
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
-        return get_handler(f"{self._api_url}/post/list", self._headers, form)
+        return get_handler(f"{self._api_url}/post/list", self._headers,
+                           None, params=form)
 
     def get_private_messages(self, limit: int = None, page: int = None,
                              unread_only: bool = None) -> requests.Response:
         """ get_private_messages: get private messages
 
         Args:
             limit (int): max. num. messages to obtain (optional)
@@ -1042,15 +1048,15 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/private_message/list",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def get_replies(self, limit: int = None, page: int = None,
                     sort: str = None,
                     unread_only: bool = None) -> requests.Response:
         """ get_replies: get replies for current user
 
         Args:
@@ -1063,71 +1069,72 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/user/replies",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def get_report_count(self, community_id: int = None) -> requests.Response:
         """ get_report_count: number of reports
 
         Args:
             community_id (int): ID of community to query (optional)
 
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/user/report_count",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def get_site(self) -> requests.Response:
         """ get_site: return site info
 
         Args:
             None
 
         Returns:
             requests.Response: result of API call
         """
 
         form = {"auth": self.key}
-        return get_handler(f"{self._api_url}/site", self._headers, form)
+        return get_handler(f"{self._api_url}/site", self._headers,
+                           None, params=form)
 
     def get_site_metadata(self, url: str) -> requests.Response:
         """ get_site_metadata: return an instance's metadata
 
         Args:
             url (str): Lemmy instance
 
         Returns:
             requests.Response: result of API call
         """
 
         form = {"url": url}
         return get_handler(f"{self._api_url}/post/site_metadata",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def get_unread_count(self) -> requests.Response:
         """ get_unread_count: get number of unread notifications
 
         Args:
             None
 
         Returns:
             requests.Response: result of API call
         """
 
         form = {"auth": self.key}
         return get_handler(f"{self._api_url}/user/unread_count",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def get_unread_registration_application_count(self) -> requests.Response:
         """ get_unread_registration_application_count: number of unread
         instance applications
 
         Args:
             None
@@ -1135,15 +1142,15 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = {"auth": self.key}
         return get_handler(
             f"{self._api_url}/admin/registration_application/count",
-            self._headers, form
+            self._headers, None, params=form
         )
 
     def leave_admin(self) -> requests.Response:
         """ leave_admin: current user leaves admin group
 
         Args:
             None
@@ -1202,15 +1209,15 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/comment/report/list",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def list_communities(self, limit: int = None, page: int = None,
                          sort: str = None,
                          type_: str = None) -> requests.Response:
         """ list_communities: return list of communities
 
         Args:
@@ -1224,15 +1231,15 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/community/list",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def list_post_reports(self, community_id: int = None, limit: int = None,
                           page: int = None, unresolved_only: bool = None
                           ) -> requests.Response:
         """ list_post_reports: return a list of post reports
 
         Args:
@@ -1245,15 +1252,15 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/post/report/list",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def list_private_message_reports(self, limit: int = None, page: int = None,
                                      unresolved_only: bool = None
                                      ) -> requests.Response:
         """ list_private_message_reports: return a list of private message
         reports
 
@@ -1266,15 +1273,15 @@
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(f"{self._api_url}/private_message/report/list",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def list_registration_applications(self, limit: int = None,
                                        page: int = None,
                                        unread_only: bool = None
                                        ) -> requests.Response:
         """ list_registration_applications: return a list of registration
         applications
@@ -1289,15 +1296,15 @@
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
         return get_handler(
             f"{self._api_url}/admin/registration_application/list",
-            self._headers, form
+            self._headers, None, params=form
         )
 
     def lock_post(self, locked: bool, post_id: int) -> requests.Response:
         """ lock_post: lock a post
 
         Args:
             locked (bool): True if post is locked, False otherwise
@@ -1614,15 +1621,15 @@
 
         Returns:
             requests.Response: result of API call
         """
 
         form = {"q": q, "auth": self.key}
         return get_handler(f"{self._api_url}/resolve_object",
-                           self._headers, form)
+                           self._headers, None, params=form)
 
     def resolve_post_report(self, report_id: int,
                             resolved: bool) -> requests.Response:
         """ resolve_post_report: resolve a post report
 
         Args:
             report_id (int): ID of post report
@@ -1763,15 +1770,16 @@
 
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
-        return get_handler(f"{self._api_url}/search", self._headers, form)
+        return get_handler(f"{self._api_url}/search", self._headers,
+                           None, params=form)
 
     def transfer_community(self, community_id: int,
                            person_id: int) -> requests.Response:
         """ transfer_community: transfer ownership of a community
 
         Args:
             community_id (int): ID of community
```

### Comparing `plemmy-0.2.5/plemmy/utils.py` & `plemmy-0.2.6/plemmy/utils.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.5/plemmy.egg-info/PKG-INFO` & `plemmy-0.2.6/plemmy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.2.5/setup.py` & `plemmy-0.2.6/setup.py`

 * *Files identical despite different names*

