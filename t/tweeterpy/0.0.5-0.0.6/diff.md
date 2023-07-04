# Comparing `tmp/tweeterpy-0.0.5.tar.gz` & `tmp/tweeterpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-0.0.5.tar", last modified: Wed Jun 28 07:57:47 2023, max compression
+gzip compressed data, was "tweeterpy-0.0.6.tar", last modified: Tue Jul  4 18:54:35 2023, max compression
```

## Comparing `tweeterpy-0.0.5.tar` & `tweeterpy-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 07:57:47.935358 tweeterpy-0.0.5/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3389 2023-06-28 07:57:47.935358 tweeterpy-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-28 07:57:47.935358 tweeterpy-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-06-28 07:55:23.000000 tweeterpy-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 07:57:47.908196 tweeterpy-0.0.5/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.5/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     2581 2023-06-20 09:49:11.000000 tweeterpy-0.0.5/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0      671 2023-06-25 06:51:11.000000 tweeterpy-0.0.5/tweeterpy/config.py
--rw-rw-rw-   0        0        0     1980 2023-06-20 14:19:17.000000 tweeterpy-0.0.5/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     6654 2023-06-24 14:06:58.000000 tweeterpy-0.0.5/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.5/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0     2278 2023-06-25 06:51:11.000000 tweeterpy-0.0.5/tweeterpy/session_util.py
--rw-rw-rw-   0        0        0    22817 2023-06-25 07:23:32.000000 tweeterpy-0.0.5/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0     3593 2023-06-28 07:54:04.000000 tweeterpy-0.0.5/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2023-06-28 07:57:47.923821 tweeterpy-0.0.5/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3389 2023-06-28 07:57:47.000000 tweeterpy-0.0.5/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-06-28 07:57:47.000000 tweeterpy-0.0.5/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 07:57:47.000000 tweeterpy-0.0.5/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      221 2023-06-28 07:57:47.000000 tweeterpy-0.0.5/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-28 07:57:47.000000 tweeterpy-0.0.5/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 18:54:35.091717 tweeterpy-0.0.6/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3389 2023-07-04 18:54:35.076105 tweeterpy-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 18:54:35.091717 tweeterpy-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-07-04 18:54:07.000000 tweeterpy-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:54:35.076105 tweeterpy-0.0.6/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.6/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     4037 2023-06-28 13:39:17.000000 tweeterpy-0.0.6/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0      671 2023-06-25 06:51:11.000000 tweeterpy-0.0.6/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     2635 2023-06-28 13:44:31.000000 tweeterpy-0.0.6/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     6654 2023-06-24 14:06:58.000000 tweeterpy-0.0.6/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.6/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2278 2023-06-25 06:51:11.000000 tweeterpy-0.0.6/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    23036 2023-06-28 13:57:16.000000 tweeterpy-0.0.6/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0     3593 2023-06-28 07:54:04.000000 tweeterpy-0.0.6/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:54:35.076105 tweeterpy-0.0.6/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      221 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-04 18:54:34.000000 tweeterpy-0.0.6/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-0.0.5/LICENSE` & `tweeterpy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.5/PKG-INFO` & `tweeterpy-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.5 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.6 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tweeterpy-0.0.5/README.md` & `tweeterpy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.5/setup.py` & `tweeterpy-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-0.0.5/tweeterpy/api_util.py` & `tweeterpy-0.0.6/tweeterpy/api_util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 import re
+import json
 import js2py
-from .constants import Path
+from .constants import Path, FeatureSwitch
 from .request_util import make_request
 
 
 dataset_regex = re.compile(r'''exports\s*=\s*{(.*?)},''', re.VERBOSE)
+api_file_regex = re.compile(r'''api:(.*?),''', re.VERBOSE)
+feature_switch_regex = re.compile(r'''.featureSwitch.:(.*?)}},''', re.VERBOSE)
 
 
 class ApiUpdater:
+    """ 
+        Twitter updates its API quite frequently. Therefore, ApiUpdater checks for the latest updates and modifies the api_endpoints, feature_switches, path etc in constants.py
+    """
+
     def __init__(self):
         try:
             # fmt: off - Turns off formatting for this block of code.
-            api_endpoints_data = self._js_to_py_dict(self._get_api_file_content())
+            page_source = self._get_home_page_source()
+            api_file_url = self._get_api_file_url(page_source)
+            feature_switches = self._get_feature_switches(page_source)
+            api_endpoints_data = self._js_to_py_dict(self._get_api_file_content(api_file_url))
             current_api_endpoints = self._get_current_api_endpoints()
             new_api_endpoints = self._map_data(current_api_endpoints, api_endpoints_data)
             self._update_api_endpoints(new_api_endpoints)
+            self._update_feature_switches(feature_switches)
             print("API Updated Successfully.")
         except Exception as error:
             raise Exception(f"{error}\nCouldn't Update API.")
 
-    def _get_api_file_url(self):
-        page_source = str(make_request(Path.BASE_URL))
-        api_file_name = re.search(r"api:(.*?),", page_source).group(1)
+    def _get_home_page_source(self):
+        return str(make_request(Path.BASE_URL))
+
+    def _get_api_file_url(self,page_source=None):
+        if page_source is None:
+            page_source = self._get_home_page_source
+        api_file_name = re.search(api_file_regex, page_source).group(1)
         api_file_url = f"{Path.TWITTER_CDN}/api.{eval(api_file_name)}a.js"
         return api_file_url
 
     def _get_api_file_content(self, file_url=None):
         if file_url is None:
             file_url = self._get_api_file_url()
         return make_request(file_url)
@@ -35,19 +50,20 @@
             page_source = "\n".join([item for item in page_source])
         else:
             page_source = str(page_source)
         matches = []
         for match in dataset_regex.finditer(page_source):
             matches.append(match.group(0))
 
-        api_dict = [js2py.eval_js(each_match.replace('},', ''))
+        dict_data = [js2py.eval_js(each_match.replace('},', ''))
                     for each_match in matches]
-        return api_dict
+        return dict_data
 
     def _map_data(self, old_endpoints, new_endpoints):
+        FeatureSwitch.api_endpoints = {f"{endpoint['queryId']}/{endpoint['operationName']}" : endpoint for endpoint in new_endpoints}
         new_endpoints = {
             endpoint['operationName']: f"{endpoint['queryId']}/{endpoint['operationName']}" for endpoint in new_endpoints}
         mapped_data = {}
         for key, value in old_endpoints.items():
             mapped_data.update({key: new_value for new_key, new_value in new_endpoints.items()
                                 if value.split("/")[-1] == new_key})
         return mapped_data
@@ -59,10 +75,20 @@
                 api_endpoints[key] = value
         return api_endpoints
 
     def _update_api_endpoints(self, new_endpoints):
         for key, value in new_endpoints.items():
             setattr(Path, key, value)
 
+    def _get_feature_switches(self,page_source=None):
+        if page_source is None:
+            self._get_home_page_source()
+        feature_switch_data = re.search(feature_switch_regex,str(page_source)).group(0)
+        return json.loads("{"+feature_switch_data.rstrip(',')+"}}")
+
+    def _update_feature_switches(self,feature_switches=None):
+        if feature_switches is None:
+            feature_switches = self._get_feature_switches()
+        FeatureSwitch.all_feature_switches = feature_switches['featureSwitch']['defaultConfig']
 
 if __name__ == "__main__":
     pass
```

### Comparing `tweeterpy-0.0.5/tweeterpy/config.py` & `tweeterpy-0.0.6/tweeterpy/config.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.5/tweeterpy/login_util.py` & `tweeterpy-0.0.6/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.5/tweeterpy/request_util.py` & `tweeterpy-0.0.6/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.5/tweeterpy/session_util.py` & `tweeterpy-0.0.6/tweeterpy/session_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.5/tweeterpy/tweeterpy.py` & `tweeterpy-0.0.6/tweeterpy/tweeterpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import json
 import random
 import getpass
 from functools import reduce
 
 from .api_util import ApiUpdater
-from .constants import Path
+from .constants import Path, FeatureSwitch
 from .login_util import TaskHandler
 from .request_util import make_request
 from .session_util import load_session, save_session
 from . import util
 from . import config
 
 
@@ -17,19 +17,21 @@
 
     def __init__(self):
         self.generate_session()
         # update api endpoints
         ApiUpdater()
 
     def _generate_request_data(self, endpoint, variables=None, **kwargs):
+        # fmt: off - Turns off formatting for this block of code. Just for the readability purpose.
         url = util.generate_url(domain=Path.API_URL, url_path=endpoint)
         query_params = {"variables": json.dumps({**variables})}
         if kwargs:
-            features = json.dumps(util.generate_features(**kwargs))
-            query_params["features"] = features
+            features = FeatureSwitch().get_query_features(endpoint) or util.generate_features(**kwargs)
+            query_params["features"] = json.dumps(features)
+        # fmt: on   
         return url, query_params
 
     def _handle_pagination(self, url, query_params, end_cursor=None, data_path=None, total=None):
         # fmt: off  - Turns off formatting for this block of code. Just for the readability purpose.
         def filter_data(response):
             filtered_data = []
             for each_entry in response:
@@ -289,15 +291,15 @@
         """
         if end_cursor is not None and not with_tweet_replies:
             raise Exception(
                 "Either set with_tweet_replies to True or end_cursor to None.")
         referer = 'tweet' if with_tweet_replies else random.choice(
             ['profile', 'home'])
         variables = {"focalTweetId": tweet_id, "referrer": referer, "with_rux_injections": False, "includePromotedContent": True,
-                     "withCommunity": True, "withQuickPromoteEligibilityTweetFields": True, "withBirdwatchNotes": False,
+                     "withCommunity": True, "withQuickPromoteEligibilityTweetFields": True, "withArticleRichContent": False, "withBirdwatchNotes": False,
                      "withVoice": True, "withV2Timeline": True}
         url, query_params = self._generate_request_data(
             Path.TWEET_DETAILS_ENDPOINT, variables, additional_features=True)
         data_path = (
             'data', 'threaded_conversation_with_injections_v2', 'instructions')
         if with_tweet_replies:
             return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
```

### Comparing `tweeterpy-0.0.5/tweeterpy/util.py` & `tweeterpy-0.0.6/tweeterpy/util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.5/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-0.0.6/tweeterpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.5 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.6 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

