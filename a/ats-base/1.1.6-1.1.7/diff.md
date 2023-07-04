# Comparing `tmp/ats_base-1.1.6.tar.gz` & `tmp/ats_base-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_base-1.1.6.tar", last modified: Sat Jul  1 07:44:31 2023, max compression
+gzip compressed data, was "ats_base-1.1.7.tar", last modified: Tue Jul  4 00:58:43 2023, max compression
```

## Comparing `ats_base-1.1.6.tar` & `ats_base-1.1.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 07:44:31.859262 ats_base-1.1.6/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_base-1.1.6/LICENSE
--rw-rw-rw-   0        0        0      305 2023-04-08 10:09:46.000000 ats_base-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-07-01 07:44:31.858098 ats_base-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_base-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 07:44:31.326115 ats_base-1.1.6/ats_base/
--rw-rw-rw-   0        0        0        0 2022-09-15 08:20:17.000000 ats_base-1.1.6/ats_base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:44:31.480158 ats_base-1.1.6/ats_base/base/
--rw-rw-rw-   0        0        0        0 2022-09-15 08:27:28.000000 ats_base-1.1.6/ats_base/base/__init__.py
--rw-rw-rw-   0        0        0      868 2022-10-08 05:21:17.000000 ats_base-1.1.6/ats_base/base/entrance.py
--rw-rw-rw-   0        0        0     1739 2023-04-07 00:56:47.000000 ats_base-1.1.6/ats_base/base/req.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:44:31.541046 ats_base-1.1.6/ats_base/common/
--rw-rw-rw-   0        0        0        0 2022-05-30 03:34:10.000000 ats_base-1.1.6/ats_base/common/__init__.py
--rw-rw-rw-   0        0        0     3778 2023-04-12 02:34:23.000000 ats_base-1.1.6/ats_base/common/func.py
--rw-rw-rw-   0        0        0      656 2022-10-11 06:12:32.000000 ats_base-1.1.6/ats_base/common/resp.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:44:31.602085 ats_base-1.1.6/ats_base/config/
--rw-rw-rw-   0        0        0        0 2022-05-26 08:20:18.000000 ats_base-1.1.6/ats_base/config/__init__.py
--rw-rw-rw-   0        0        0      422 2023-04-22 07:34:22.000000 ats_base-1.1.6/ats_base/config/config.ini
--rw-rw-rw-   0        0        0      251 2022-05-30 01:53:51.000000 ats_base-1.1.6/ats_base/config/configure.py
--rw-rw-rw-   0        0        0     1108 2022-12-22 02:31:24.000000 ats_base-1.1.6/ats_base/config/rewrite_config.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:44:31.634001 ats_base-1.1.6/ats_base/log/
--rw-rw-rw-   0        0        0        0 2022-09-20 00:58:33.000000 ats_base-1.1.6/ats_base/log/__init__.py
--rw-rw-rw-   0        0        0     3449 2023-04-12 01:14:31.000000 ats_base-1.1.6/ats_base/log/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:44:31.833005 ats_base-1.1.6/ats_base/service/
--rw-rw-rw-   0        0        0        0 2022-05-26 08:20:27.000000 ats_base-1.1.6/ats_base/service/__init__.py
--rw-rw-rw-   0        0        0      225 2022-09-16 06:07:59.000000 ats_base-1.1.6/ats_base/service/app.py
--rw-rw-rw-   0        0        0      724 2023-07-01 07:43:43.000000 ats_base-1.1.6/ats_base/service/build_in.py
--rw-rw-rw-   0        0        0     1691 2022-10-08 06:47:45.000000 ats_base-1.1.6/ats_base/service/db.py
--rw-rw-rw-   0        0        0      432 2023-04-11 01:28:00.000000 ats_base-1.1.6/ats_base/service/em.py
--rw-rw-rw-   0        0        0     8729 2022-10-26 00:59:06.000000 ats_base-1.1.6/ats_base/service/mm.py
--rw-rw-rw-   0        0        0      957 2022-10-09 01:12:00.000000 ats_base-1.1.6/ats_base/service/pro.py
--rw-rw-rw-   0        0        0      778 2023-04-22 07:53:11.000000 ats_base-1.1.6/ats_base/service/udm.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:44:31.419149 ats_base-1.1.6/ats_base.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-07-01 07:44:30.000000 ats_base-1.1.6/ats_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      732 2023-07-01 07:44:31.000000 ats_base-1.1.6/ats_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 07:44:30.000000 ats_base-1.1.6/ats_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-01 07:44:30.000000 ats_base-1.1.6/ats_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 07:44:30.000000 ats_base-1.1.6/ats_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 07:44:31.860237 ats_base-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      947 2023-07-01 07:43:53.000000 ats_base-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:58:43.273970 ats_base-1.1.7/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_base-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0      305 2023-04-08 10:09:46.000000 ats_base-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-07-04 00:58:43.270975 ats_base-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_base-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 00:58:42.764505 ats_base-1.1.7/ats_base/
+-rw-rw-rw-   0        0        0        0 2022-09-15 08:20:17.000000 ats_base-1.1.7/ats_base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:58:42.920090 ats_base-1.1.7/ats_base/base/
+-rw-rw-rw-   0        0        0        0 2022-09-15 08:27:28.000000 ats_base-1.1.7/ats_base/base/__init__.py
+-rw-rw-rw-   0        0        0      868 2022-10-08 05:21:17.000000 ats_base-1.1.7/ats_base/base/entrance.py
+-rw-rw-rw-   0        0        0     1739 2023-04-07 00:56:47.000000 ats_base-1.1.7/ats_base/base/req.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:58:42.982921 ats_base-1.1.7/ats_base/common/
+-rw-rw-rw-   0        0        0        0 2022-05-30 03:34:10.000000 ats_base-1.1.7/ats_base/common/__init__.py
+-rw-rw-rw-   0        0        0     3778 2023-04-12 02:34:23.000000 ats_base-1.1.7/ats_base/common/func.py
+-rw-rw-rw-   0        0        0      656 2022-10-11 06:12:32.000000 ats_base-1.1.7/ats_base/common/resp.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:58:43.039770 ats_base-1.1.7/ats_base/config/
+-rw-rw-rw-   0        0        0        0 2022-05-26 08:20:18.000000 ats_base-1.1.7/ats_base/config/__init__.py
+-rw-rw-rw-   0        0        0      422 2023-04-22 07:34:22.000000 ats_base-1.1.7/ats_base/config/config.ini
+-rw-rw-rw-   0        0        0      251 2022-05-30 01:53:51.000000 ats_base-1.1.7/ats_base/config/configure.py
+-rw-rw-rw-   0        0        0     1108 2022-12-22 02:31:24.000000 ats_base-1.1.7/ats_base/config/rewrite_config.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:58:43.071685 ats_base-1.1.7/ats_base/log/
+-rw-rw-rw-   0        0        0        0 2022-09-20 00:58:33.000000 ats_base-1.1.7/ats_base/log/__init__.py
+-rw-rw-rw-   0        0        0     3449 2023-04-12 01:14:31.000000 ats_base-1.1.7/ats_base/log/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:58:43.241397 ats_base-1.1.7/ats_base/service/
+-rw-rw-rw-   0        0        0        0 2022-05-26 08:20:27.000000 ats_base-1.1.7/ats_base/service/__init__.py
+-rw-rw-rw-   0        0        0      225 2022-09-16 06:07:59.000000 ats_base-1.1.7/ats_base/service/app.py
+-rw-rw-rw-   0        0        0      724 2023-07-01 07:43:43.000000 ats_base-1.1.7/ats_base/service/build_in.py
+-rw-rw-rw-   0        0        0     1691 2022-10-08 06:47:45.000000 ats_base-1.1.7/ats_base/service/db.py
+-rw-rw-rw-   0        0        0      432 2023-04-11 01:28:00.000000 ats_base-1.1.7/ats_base/service/em.py
+-rw-rw-rw-   0        0        0     8729 2022-10-26 00:59:06.000000 ats_base-1.1.7/ats_base/service/mm.py
+-rw-rw-rw-   0        0        0      957 2022-10-09 01:12:00.000000 ats_base-1.1.7/ats_base/service/pro.py
+-rw-rw-rw-   0        0        0      778 2023-04-22 07:53:11.000000 ats_base-1.1.7/ats_base/service/udm.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:58:42.861247 ats_base-1.1.7/ats_base.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-07-04 00:58:42.000000 ats_base-1.1.7/ats_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      732 2023-07-04 00:58:42.000000 ats_base-1.1.7/ats_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 00:58:42.000000 ats_base-1.1.7/ats_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-04 00:58:42.000000 ats_base-1.1.7/ats_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 00:58:42.000000 ats_base-1.1.7/ats_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 00:58:43.273970 ats_base-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      947 2023-07-04 00:58:28.000000 ats_base-1.1.7/setup.py
```

### Comparing `ats_base-1.1.6/PKG-INFO` & `ats_base-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_base
-Version: 1.1.6
+Version: 1.1.7
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_base
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_base-1.1.6/README.md` & `ats_base-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/base/entrance.py` & `ats_base-1.1.7/ats_base/base/entrance.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/base/req.py` & `ats_base-1.1.7/ats_base/base/req.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/common/func.py` & `ats_base-1.1.7/ats_base/common/func.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/common/resp.py` & `ats_base-1.1.7/ats_base/common/resp.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/config/rewrite_config.py` & `ats_base-1.1.7/ats_base/config/rewrite_config.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/log/logger.py` & `ats_base-1.1.7/ats_base/log/logger.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/service/build_in.py` & `ats_base-1.1.7/ats_base/service/build_in.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/service/db.py` & `ats_base-1.1.7/ats_base/service/db.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/service/mm.py` & `ats_base-1.1.7/ats_base/service/mm.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/service/pro.py` & `ats_base-1.1.7/ats_base/service/pro.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base/service/udm.py` & `ats_base-1.1.7/ats_base/service/udm.py`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/ats_base.egg-info/PKG-INFO` & `ats_base-1.1.7/ats_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-base
-Version: 1.1.6
+Version: 1.1.7
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_base
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_base-1.1.6/ats_base.egg-info/SOURCES.txt` & `ats_base-1.1.7/ats_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_base-1.1.6/setup.py` & `ats_base-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_base",
-    version="1.1.6",
+    version="1.1.7",
     py_modules=['ats_base'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_base",
```

