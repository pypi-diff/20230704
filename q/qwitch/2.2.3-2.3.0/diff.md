# Comparing `tmp/qwitch-2.2.3.tar.gz` & `tmp/qwitch-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwitch-2.2.3.tar", last modified: Mon Jul  3 19:55:06 2023, max compression
+gzip compressed data, was "qwitch-2.3.0.tar", last modified: Mon Jul  3 22:55:00 2023, max compression
```

## Comparing `qwitch-2.2.3.tar` & `qwitch-2.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:55:06.736073 qwitch-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-03 19:55:06.736073 qwitch-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-07-03 19:54:56.000000 qwitch-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 19:54:56.000000 qwitch-2.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:55:06.732073 qwitch-2.2.3/qwitch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:54:56.000000 qwitch-2.2.3/qwitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-03 19:54:56.000000 qwitch-2.2.3/qwitch/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-03 19:54:56.000000 qwitch-2.2.3/qwitch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-03 19:54:56.000000 qwitch-2.2.3/qwitch/qwitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:55:06.732073 qwitch-2.2.3/qwitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-03 19:55:06.000000 qwitch-2.2.3/qwitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 19:55:06.000000 qwitch-2.2.3/qwitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:55:06.000000 qwitch-2.2.3/qwitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 19:55:06.000000 qwitch-2.2.3/qwitch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:55:06.000000 qwitch-2.2.3/qwitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 19:55:06.000000 qwitch-2.2.3/qwitch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 19:55:06.736073 qwitch-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-03 19:54:56.000000 qwitch-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:00.967921 qwitch-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-03 22:55:00.967921 qwitch-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-07-03 22:54:48.000000 qwitch-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 22:54:48.000000 qwitch-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:00.967921 qwitch-2.3.0/qwitch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:54:48.000000 qwitch-2.3.0/qwitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-03 22:54:48.000000 qwitch-2.3.0/qwitch/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-03 22:54:48.000000 qwitch-2.3.0/qwitch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-03 22:54:48.000000 qwitch-2.3.0/qwitch/qwitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:00.967921 qwitch-2.3.0/qwitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-03 22:55:00.000000 qwitch-2.3.0/qwitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 22:55:00.000000 qwitch-2.3.0/qwitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:55:00.000000 qwitch-2.3.0/qwitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 22:55:00.000000 qwitch-2.3.0/qwitch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 22:55:00.000000 qwitch-2.3.0/qwitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:55:00.000000 qwitch-2.3.0/qwitch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 22:55:00.967921 qwitch-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-03 22:54:48.000000 qwitch-2.3.0/setup.py
```

### Comparing `qwitch-2.2.3/PKG-INFO` & `qwitch-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwitch
-Version: 2.2.3
+Version: 2.3.0
 Summary: Stream twitch in Quicktime.
 Home-page: https://github.com/gencys/qwitch
 Author: Jean-Francois Vaduret
 Author-email: Jean-Francois Vaduret <jean.francois.vaduret@gmail.com>
 Project-URL: Source, https://github.com/gencys/qwitch
 Project-URL: Tracker, https://github.com/gencys/qwitch/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qwitch-2.2.3/README.md` & `qwitch-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qwitch-2.2.3/pyproject.toml` & `qwitch-2.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qwitch"
-version = "2.2.3"
+version = "2.3.0"
 description = "Stream twitch in Quicktime."
 readme = "README.md"
 authors = [{ name = "Jean-Francois Vaduret", email = "jean.francois.vaduret@gmail.com" }]
 license = {file = "LICENSE"}
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `qwitch-2.2.3/qwitch/api.py` & `qwitch-2.3.0/qwitch/api.py`

 * *Files identical despite different names*

### Comparing `qwitch-2.2.3/qwitch/config.py` & `qwitch-2.3.0/qwitch/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import json
 import webbrowser
 import time
 import requests
 
 DEBUG = False
+VER = '2.3.0'
 
 home_dir = os.path.expanduser('~')
 home_dir += '/Library/Application Support'
 if not os.path.exists(home_dir + '/qwitch/config.json'):
     os.makedirs(os.path.dirname(home_dir + '/qwitch/config.json'), exist_ok=True)
 
 def debug_log(*args):
@@ -68,15 +69,15 @@
     return res_get
 
 def write_streamlink_config():
     if os.path.exists(home_dir + '/qwitch/config.json'):
         token = ask_for_token(validate = True)
         with open(home_dir + '/qwitch/config.json', 'r', encoding='utf-8') as file:
             cache_json = json.loads(file.read())
-        if len(cache_json) == 2:
+        if len(cache_json) >= 2:
             cache_json[1].update({'twitch-api-header': 'Authorization=OAuth ' + token})
         else:
             config = {
                 'twitch-api-header': 'Authorization=OAuth ' + token
             }
             cache_json.append(config)
         config = cache_json[1]
@@ -86,15 +87,15 @@
     return False
 
 def check_streamlink_config():
     old_token = ''
     with open(home_dir + '/qwitch/config.json', 'r', encoding='utf-8') as file:
         content = json.loads(file.read())
         debug_log('Content of config:', content)
-    if len(content) == 2:
+    if len(content) >= 2:
         if 'twitch-api-header' in content[1]:
             token = re.findall('Authorization=OAuth\s([a-z0-9]{30})', content[1]['twitch-api-header'])
         else:
             config = write_streamlink_config()
             return config
     else:
         config = write_streamlink_config()
@@ -150,8 +151,31 @@
                 return False
             return cache_json[0]['access_token']
     except:
         token = auth_api()
         debug_log('Token returned by auth_api() after error:', token)
         if token:
             return token
-        return False
+        return False
+    
+# Get Qwitch's latest version from pypi.org's API
+
+def get_package_ver_and_compare():
+    with open(home_dir + '/qwitch/config.json', 'r', encoding='utf-8') as cache:
+        cache_json = json.loads(cache.read())
+    now = int(time.time())
+    if len(cache_json) >= 3:
+        if 'last_update_check' in cache_json[2]:
+            time_to_check = cache_json[2]['last_update_check'] + 86400
+            if  now < time_to_check:
+                return False
+        cache_json[2].update({'last_update_check': now})
+    else:
+        cache_json.append({'last_update_check': now})
+    with open(home_dir + '/qwitch/config.json', 'w', encoding='utf-8') as file:
+        json.dump(cache_json, file, ensure_ascii=False, indent=4)
+    res_get = requests.get(url = 'https://pypi.org/pypi/qwitch/json').json()
+    remote_ver = res_get['info']['version']
+    if remote_ver != VER:
+        print('A new version of Qwitch is available!\nPlease update Qwitch by running:\n    \033[91m\033[1mpip install qwitch --upgrade\033[0m')
+        return True
+    return False
```

### Comparing `qwitch-2.2.3/qwitch/qwitch.py` & `qwitch-2.3.0/qwitch/qwitch.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,36 @@
             description = 'Stream twitch in Quicktime'
         )
         group = cli.add_mutually_exclusive_group(required=True)
 
         cli.add_argument('channel', nargs='?', default = False, help= 'channel name given in red with -s/--streams. Needed to launch livestream or videos.')
         cli.add_argument('quality', nargs='?', default = False, help= 'video quality name, e.g. 720p, 1080p, best, worst, etc... (defaults to best). You can defined a default quality in the config file (see the README)')
         cli.add_argument('-d', '--debug', action = 'store_true', help= 'enable debugging.')
-        cli.add_argument('--version', action='version', version='%(prog)s 2.2.3')
+        cli.add_argument('--version', action='version', version = f'%(prog)s {config.VER}')
 
         group.add_argument('-l', '--last', action = 'store_true', help= 'play the most recent video of the channel.')
         group.add_argument('-V', '--Videos', action = 'store_true', help= 'list the last 20 videos of the channel.')
         group.add_argument('-s', '--streams', action = 'store_true', help= 'list the streamers you follow which are currently currently live.')
         group.add_argument('-f', '--follows', action = 'store_true', help= 'list the streamers you follow.')
         group.add_argument('-v', '--vod', action = 'store', type = str, help= 'search for a video by keyword(s) or ID. The keyword needs to be in quotation marks and an exact match (this is not a search engine)')
         args = cli.parse_args()
 
-        auth_token = config.check_auth()
-        streamlink_config = config.check_streamlink_config()
-        if not auth_token:
-            cli.error('Could not authenticate in the Twitch API')
+        try:
+            auth_token = config.check_auth()
+            streamlink_config = config.check_streamlink_config()
+            if not auth_token:
+                cli.error('Could not authenticate in the Twitch API.')
+        except:
+            config.debug_log('An error occured when trying to authenticate in the Twitch API.\nLet us heck for an update which may fix the issue...')
+            if (config.get_package_ver_and_compare()):
+                exit()
+            cli.error('Could not authenticate in the Twitch API.')
+        
+        if (config.get_package_ver_and_compare()):
+            exit()
 
         if args.debug:
             config.DEBUG = True
 
         if args.follows:
             try:
                 api.get_follows(token = auth_token)
```

### Comparing `qwitch-2.2.3/qwitch.egg-info/PKG-INFO` & `qwitch-2.3.0/qwitch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwitch
-Version: 2.2.3
+Version: 2.3.0
 Summary: Stream twitch in Quicktime.
 Home-page: https://github.com/gencys/qwitch
 Author: Jean-Francois Vaduret
 Author-email: Jean-Francois Vaduret <jean.francois.vaduret@gmail.com>
 Project-URL: Source, https://github.com/gencys/qwitch
 Project-URL: Tracker, https://github.com/gencys/qwitch/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qwitch-2.2.3/setup.cfg` & `qwitch-2.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qwitch
-version = 2.2.3
+version = 2.3.0
 author = Jean-Francois Vaduret
 author_email = jean.francois.vaduret@gmail.com
 description = Stream twitch in Quicktime.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gencys/qwitch
 project_urls =
```

