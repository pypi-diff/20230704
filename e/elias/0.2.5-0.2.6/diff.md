# Comparing `tmp/elias-0.2.5.tar.gz` & `tmp/elias-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-cof3s9_m/elias-0.2.5.tar", last modified: Tue Jul  4 15:41:22 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-xc4cf2ub/elias-0.2.6.tar", last modified: Tue Jul  4 15:59:47 2023, max compression
```

## Comparing `elias-0.2.5.tar` & `elias-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:41:22.476741 elias-0.2.5/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.5/LICENSE
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-04 15:41:22.476741 elias-0.2.5/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.5/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.5/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-07-04 15:41:22.484990 elias-0.2.5/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.5/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:41:20.769741 elias-0.2.5/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:41:20.953326 elias-0.2.5/src/elias/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    24464 2023-07-04 15:40:44.000000 elias-0.2.5/src/elias/config.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:41:21.336610 elias-0.2.5/src/elias/data/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/data/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/data/combined.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/data/loader.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/data/sampling.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/data/stop_criterion.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:41:21.635111 elias-0.2.5/src/elias/folder/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/folder/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/folder/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.5/src/elias/folder/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.5/src/elias/folder/folder.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.5/src/elias/folder/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.5/src/elias/folder/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:41:21.967096 elias-0.2.5/src/elias/manager/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/manager/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/manager/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/manager/artifact.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.5/src/elias/manager/buffered.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.5/src/elias/manager/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.5/src/elias/manager/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.5/src/elias/manager/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:41:22.422345 elias-0.2.5/src/elias/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.5/src/elias/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.5/src/elias/util/fs.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.5/src/elias/util/io.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.5/src/elias/util/random.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.5/src/elias/util/range.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.5/src/elias/util/timing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1218 2023-07-04 15:24:59.000000 elias-0.2.5/src/elias/util/typing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.5/src/elias/util/version.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:41:21.113326 elias-0.2.5/src/elias.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-04 15:41:20.000000 elias-0.2.5/src/elias.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      948 2023-07-04 15:41:20.000000 elias-0.2.5/src/elias.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-07-04 15:41:20.000000 elias-0.2.5/src/elias.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-07-04 15:41:20.000000 elias-0.2.5/src/elias.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-07-04 15:41:20.000000 elias-0.2.5/src/elias.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:59:47.101853 elias-0.2.6/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.6/LICENSE
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-04 15:59:47.101853 elias-0.2.6/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.6/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.6/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-07-04 15:59:47.109130 elias-0.2.6/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.6/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:59:45.615703 elias-0.2.6/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:59:45.802600 elias-0.2.6/src/elias/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    24490 2023-07-04 15:54:36.000000 elias-0.2.6/src/elias/config.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:59:46.169517 elias-0.2.6/src/elias/data/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/data/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/data/combined.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/data/loader.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/data/sampling.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/data/stop_criterion.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:59:46.427054 elias-0.2.6/src/elias/folder/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/folder/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/folder/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.6/src/elias/folder/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.6/src/elias/folder/folder.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.6/src/elias/folder/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.6/src/elias/folder/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:59:46.721546 elias-0.2.6/src/elias/manager/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/manager/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/manager/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/manager/artifact.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.6/src/elias/manager/buffered.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.6/src/elias/manager/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.6/src/elias/manager/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.6/src/elias/manager/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:59:47.060221 elias-0.2.6/src/elias/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.6/src/elias/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.6/src/elias/util/fs.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.6/src/elias/util/io.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.6/src/elias/util/random.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.6/src/elias/util/range.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.6/src/elias/util/timing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1218 2023-07-04 15:24:59.000000 elias-0.2.6/src/elias/util/typing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.6/src/elias/util/version.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-04 15:59:45.963138 elias-0.2.6/src/elias.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-04 15:59:45.000000 elias-0.2.6/src/elias.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      948 2023-07-04 15:59:45.000000 elias-0.2.6/src/elias.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-07-04 15:59:45.000000 elias-0.2.6/src/elias.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-07-04 15:59:45.000000 elias-0.2.6/src/elias.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-07-04 15:59:45.000000 elias-0.2.6/src/elias.egg-info/top_level.txt
```

### Comparing `elias-0.2.5/PKG-INFO` & `elias-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.5
+Version: 0.2.6
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.5/README.md` & `elias-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/setup.cfg` & `elias-0.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elias
-version = 0.2.5
+version = 0.2.6
 author = Tobias Kirschstein
 author_email = tobias.kirschstein@gmail.com
 description = ELIAS experiment library for facilitating machine learning projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tobias-kirschstein/elias
 project_urls =
```

### Comparing `elias-0.2.5/src/elias/config.py` & `elias-0.2.6/src/elias/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,16 @@
             # Add use-defined type hooks
             all_type_hooks.update(type_hooks)
 
         # Register type hooks to replace every single AbstractDataClass with the respective subclass hinted by the
         # 'type' attribute
         dacite_config = dacite.Config(
             cast=cls._define_casts(),
-            type_hooks=all_type_hooks)
+            type_hooks=all_type_hooks,
+            strict=True)
 
         # backward_cls = type(cls.__name__, cls.__bases__, dict(cls.__dict__))
         #
         # def backward_compatibility_new(cls_new, *args, **kwargs):
         #     obj = super(Config, cls).__new__(cls)
         #     obj._enable_backward_compatibility = True
         #     # For some reason, __init__ isn't called anymore if __new__ is overridden. So manually call it here
```

### Comparing `elias-0.2.5/src/elias/data/combined.py` & `elias-0.2.6/src/elias/data/combined.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/data/loader.py` & `elias-0.2.6/src/elias/data/loader.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/data/sampling.py` & `elias-0.2.6/src/elias/data/sampling.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/data/stop_criterion.py` & `elias-0.2.6/src/elias/data/stop_criterion.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/folder/analysis.py` & `elias-0.2.6/src/elias/folder/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/folder/data.py` & `elias-0.2.6/src/elias/folder/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/folder/folder.py` & `elias-0.2.6/src/elias/folder/folder.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/folder/model.py` & `elias-0.2.6/src/elias/folder/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/folder/run.py` & `elias-0.2.6/src/elias/folder/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/manager/analysis.py` & `elias-0.2.6/src/elias/manager/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/manager/artifact.py` & `elias-0.2.6/src/elias/manager/artifact.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/manager/buffered.py` & `elias-0.2.6/src/elias/manager/buffered.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/manager/data.py` & `elias-0.2.6/src/elias/manager/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/manager/model.py` & `elias-0.2.6/src/elias/manager/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/manager/run.py` & `elias-0.2.6/src/elias/manager/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/util/fs.py` & `elias-0.2.6/src/elias/util/fs.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/util/io.py` & `elias-0.2.6/src/elias/util/io.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/util/range.py` & `elias-0.2.6/src/elias/util/range.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/util/timing.py` & `elias-0.2.6/src/elias/util/timing.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/util/typing.py` & `elias-0.2.6/src/elias/util/typing.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias/util/version.py` & `elias-0.2.6/src/elias/util/version.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.5/src/elias.egg-info/PKG-INFO` & `elias-0.2.6/src/elias.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.5
+Version: 0.2.6
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.5/src/elias.egg-info/SOURCES.txt` & `elias-0.2.6/src/elias.egg-info/SOURCES.txt`

 * *Files identical despite different names*

