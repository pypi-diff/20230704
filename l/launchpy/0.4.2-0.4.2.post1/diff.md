# Comparing `tmp/launchpy-0.4.2.tar.gz` & `tmp/launchpy-0.4.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchpy-0.4.2.tar", last modified: Thu Jun 22 12:30:36 2023, max compression
+gzip compressed data, was "launchpy-0.4.2.post1.tar", last modified: Tue Jul  4 19:29:40 2023, max compression
```

## Comparing `launchpy-0.4.2.tar` & `launchpy-0.4.2.post1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:36.945758 launchpy-0.4.2/
--rw-rw-rw-   0        0        0    35823 2021-10-20 19:49:46.000000 launchpy-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     2294 2023-06-22 12:30:36.944760 launchpy-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1208 2023-06-22 12:01:59.000000 launchpy-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:36.855149 launchpy-0.4.2/docs/
--rw-rw-rw-   0        0        0     3258 2022-07-13 12:52:02.000000 launchpy-0.4.2/docs/admin.md
--rw-rw-rw-   0        0        0     3892 2021-10-20 19:49:46.000000 launchpy-0.4.2/docs/getstarted.md
--rw-rw-rw-   0        0        0     3727 2021-10-20 19:49:46.000000 launchpy-0.4.2/docs/library.md
--rw-rw-rw-   0        0        0     7521 2021-10-20 19:49:47.000000 launchpy-0.4.2/docs/main.md
--rw-rw-rw-   0        0        0    16546 2023-05-10 18:11:54.000000 launchpy-0.4.2/docs/property.md
--rw-rw-rw-   0        0        0     4657 2023-06-21 19:15:59.000000 launchpy-0.4.2/docs/releases.md
--rw-rw-rw-   0        0        0     8286 2023-05-11 13:25:38.000000 launchpy-0.4.2/docs/synchronizer.md
--rw-rw-rw-   0        0        0     4234 2023-05-10 18:06:32.000000 launchpy-0.4.2/docs/translator.md
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:36.908869 launchpy-0.4.2/launchpy/
--rw-rw-rw-   0        0        0      268 2022-11-08 13:23:21.000000 launchpy-0.4.2/launchpy/__init__.py
--rw-rw-rw-   0        0        0       21 2023-06-21 19:15:00.000000 launchpy-0.4.2/launchpy/__version__.py
--rw-rw-rw-   0        0        0    14165 2023-05-10 17:31:08.000000 launchpy-0.4.2/launchpy/admin.py
--rw-rw-rw-   0        0        0      810 2023-06-21 19:22:23.000000 launchpy-0.4.2/launchpy/config.py
--rw-rw-rw-   0        0        0     8018 2023-06-22 10:59:40.000000 launchpy-0.4.2/launchpy/configs.py
--rw-rw-rw-   0        0        0    13613 2023-06-22 11:00:34.000000 launchpy-0.4.2/launchpy/connector.py
--rw-rw-rw-   0        0        0    29268 2023-05-10 17:31:00.000000 launchpy-0.4.2/launchpy/launchpy.py
--rw-rw-rw-   0        0        0    16796 2023-05-10 17:30:51.000000 launchpy-0.4.2/launchpy/library.py
--rw-rw-rw-   0        0        0    74941 2023-05-10 17:30:38.000000 launchpy-0.4.2/launchpy/property.py
--rw-rw-rw-   0        0        0    25209 2023-05-11 12:16:25.000000 launchpy-0.4.2/launchpy/synchronizer.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:30:36.940774 launchpy-0.4.2/launchpy.egg-info/
--rw-rw-rw-   0        0        0     2294 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      564 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 12:30:36.000000 launchpy-0.4.2/launchpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1361 2023-06-22 12:02:18.000000 launchpy-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0      101 2021-10-20 19:49:47.000000 launchpy-0.4.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 12:30:36.946756 launchpy-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1754 2021-10-20 19:49:47.000000 launchpy-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:29:40.389595 launchpy-0.4.2.post1/
+-rw-rw-rw-   0        0        0    35823 2021-10-20 19:49:46.000000 launchpy-0.4.2.post1/LICENSE
+-rw-rw-rw-   0        0        0     2300 2023-07-04 19:29:40.382961 launchpy-0.4.2.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     1208 2023-06-22 12:01:59.000000 launchpy-0.4.2.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 19:29:40.182381 launchpy-0.4.2.post1/docs/
+-rw-rw-rw-   0        0        0     3258 2022-07-13 12:52:02.000000 launchpy-0.4.2.post1/docs/admin.md
+-rw-rw-rw-   0        0        0     3892 2021-10-20 19:49:46.000000 launchpy-0.4.2.post1/docs/getstarted.md
+-rw-rw-rw-   0        0        0     3727 2021-10-20 19:49:46.000000 launchpy-0.4.2.post1/docs/library.md
+-rw-rw-rw-   0        0        0     7521 2021-10-20 19:49:47.000000 launchpy-0.4.2.post1/docs/main.md
+-rw-rw-rw-   0        0        0    16546 2023-05-10 18:11:54.000000 launchpy-0.4.2.post1/docs/property.md
+-rw-rw-rw-   0        0        0     4657 2023-06-21 19:15:59.000000 launchpy-0.4.2.post1/docs/releases.md
+-rw-rw-rw-   0        0        0     8286 2023-05-11 13:25:38.000000 launchpy-0.4.2.post1/docs/synchronizer.md
+-rw-rw-rw-   0        0        0     4234 2023-05-10 18:06:32.000000 launchpy-0.4.2.post1/docs/translator.md
+drwxrwxrwx   0        0        0        0 2023-07-04 19:29:40.284768 launchpy-0.4.2.post1/launchpy/
+-rw-rw-rw-   0        0        0      268 2022-11-08 13:23:21.000000 launchpy-0.4.2.post1/launchpy/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-04 19:28:41.000000 launchpy-0.4.2.post1/launchpy/__version__.py
+-rw-rw-rw-   0        0        0    14165 2023-05-10 17:31:08.000000 launchpy-0.4.2.post1/launchpy/admin.py
+-rw-rw-rw-   0        0        0      810 2023-06-21 19:22:23.000000 launchpy-0.4.2.post1/launchpy/config.py
+-rw-rw-rw-   0        0        0     8022 2023-07-04 14:32:35.000000 launchpy-0.4.2.post1/launchpy/configs.py
+-rw-rw-rw-   0        0        0    13613 2023-06-22 11:00:34.000000 launchpy-0.4.2.post1/launchpy/connector.py
+-rw-rw-rw-   0        0        0    29268 2023-05-10 17:31:00.000000 launchpy-0.4.2.post1/launchpy/launchpy.py
+-rw-rw-rw-   0        0        0    16796 2023-05-10 17:30:51.000000 launchpy-0.4.2.post1/launchpy/library.py
+-rw-rw-rw-   0        0        0    74941 2023-05-10 17:30:38.000000 launchpy-0.4.2.post1/launchpy/property.py
+-rw-rw-rw-   0        0        0    25209 2023-05-11 12:16:25.000000 launchpy-0.4.2.post1/launchpy/synchronizer.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:29:40.368764 launchpy-0.4.2.post1/launchpy.egg-info/
+-rw-rw-rw-   0        0        0     2300 2023-07-04 19:29:39.000000 launchpy-0.4.2.post1/launchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      564 2023-07-04 19:29:40.000000 launchpy-0.4.2.post1/launchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 19:29:39.000000 launchpy-0.4.2.post1/launchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-04 19:29:39.000000 launchpy-0.4.2.post1/launchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 19:29:39.000000 launchpy-0.4.2.post1/launchpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1361 2023-06-22 12:02:18.000000 launchpy-0.4.2.post1/pyproject.toml
+-rw-rw-rw-   0        0        0      101 2021-10-20 19:49:47.000000 launchpy-0.4.2.post1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 19:29:40.390114 launchpy-0.4.2.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1754 2021-10-20 19:49:47.000000 launchpy-0.4.2.post1/setup.py
```

### Comparing `launchpy-0.4.2/LICENSE` & `launchpy-0.4.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/PKG-INFO` & `launchpy-0.4.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchpy
-Version: 0.4.2
+Version: 0.4.2.post1
 Summary: Adobe Launch API wrapper
 Home-page: https://github.com/pitchmuc/launchpy
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/launchpy
 Project-URL: changelog, https://github.com/pitchmuc/launchpy/blob/master/docs/releases.md
```

### Comparing `launchpy-0.4.2/README.md` & `launchpy-0.4.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/docs/admin.md` & `launchpy-0.4.2.post1/docs/admin.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/docs/getstarted.md` & `launchpy-0.4.2.post1/docs/getstarted.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/docs/library.md` & `launchpy-0.4.2.post1/docs/library.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/docs/main.md` & `launchpy-0.4.2.post1/docs/main.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/docs/property.md` & `launchpy-0.4.2.post1/docs/property.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/docs/releases.md` & `launchpy-0.4.2.post1/docs/releases.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/docs/synchronizer.md` & `launchpy-0.4.2.post1/docs/synchronizer.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/docs/translator.md` & `launchpy-0.4.2.post1/docs/translator.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/launchpy/admin.py` & `launchpy-0.4.2.post1/launchpy/admin.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/launchpy/config.py` & `launchpy-0.4.2.post1/launchpy/config.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/launchpy/configs.py` & `launchpy-0.4.2.post1/launchpy/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 auth_type = 'oauthV2'
             elif 'tech_id' in provided_keys and "pathToKey" in provided_keys:
                 auth_type = 'jwt'
         args = {
             "org_id" : provided_config['org_id'],
             "secret" : provided_config['secret'],
             "client_id" : client_id,
-            "scope" : provided_config['scope']
+            "scope" : provided_config.get('scope')
         }
         if auth_type == 'oauthV2':
             args["scopes"] = provided_config["scopes"].replace(' ','')
         if auth_type == 'jwt':
             args["tech_id"] = provided_config["tech_id"]
             args["path_to_key"] = provided_config["pathToKey"]
         configure(**args)
```

### Comparing `launchpy-0.4.2/launchpy/connector.py` & `launchpy-0.4.2.post1/launchpy/connector.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/launchpy/launchpy.py` & `launchpy-0.4.2.post1/launchpy/launchpy.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/launchpy/library.py` & `launchpy-0.4.2.post1/launchpy/library.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/launchpy/property.py` & `launchpy-0.4.2.post1/launchpy/property.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/launchpy/synchronizer.py` & `launchpy-0.4.2.post1/launchpy/synchronizer.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/launchpy.egg-info/PKG-INFO` & `launchpy-0.4.2.post1/launchpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchpy
-Version: 0.4.2
+Version: 0.4.2.post1
 Summary: Adobe Launch API wrapper
 Home-page: https://github.com/pitchmuc/launchpy
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/launchpy
 Project-URL: changelog, https://github.com/pitchmuc/launchpy/blob/master/docs/releases.md
```

### Comparing `launchpy-0.4.2/launchpy.egg-info/SOURCES.txt` & `launchpy-0.4.2.post1/launchpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/pyproject.toml` & `launchpy-0.4.2.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2/setup.py` & `launchpy-0.4.2.post1/setup.py`

 * *Files identical despite different names*

