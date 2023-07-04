# Comparing `tmp/trustedtwin-0.4.8.tar.gz` & `tmp/trustedtwin-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustedtwin-0.4.8.tar", last modified: Thu Sep 29 11:08:37 2022, max compression
+gzip compressed data, was "trustedtwin-0.4.9.tar", last modified: Fri Sep 30 10:44:50 2022, max compression
```

## Comparing `trustedtwin-0.4.8.tar` & `trustedtwin-0.4.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-29 11:08:37.184132 trustedtwin-0.4.8/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1106 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/LICENSE
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      941 2022-09-29 11:08:37.184132 trustedtwin-0.4.8/PKG-INFO
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      625 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/README.md
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-29 11:08:37.180132 trustedtwin-0.4.8/api_generator/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/api_generator/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)    12134 2022-05-19 08:31:57.000000 trustedtwin-0.4.8/api_generator/generate.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2545 2022-06-07 10:10:43.000000 trustedtwin-0.4.8/api_generator/templates.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-29 11:08:37.180132 trustedtwin-0.4.8/examples/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/examples/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3461 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/examples/ledgers.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1495 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/examples/twins.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      103 2022-09-29 11:08:37.184132 trustedtwin-0.4.8/setup.cfg
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      518 2022-09-29 10:14:24.000000 trustedtwin-0.4.8/setup.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-29 11:08:37.180132 trustedtwin-0.4.8/trustedtwin/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      129 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/trustedtwin/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2990 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/exceptions.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3323 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/http_client.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      319 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/trustedtwin/misc.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-29 11:08:37.184132 trustedtwin-0.4.8/trustedtwin/models/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/trustedtwin/models/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      839 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/trustedtwin/models/responses.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-29 11:08:37.184132 trustedtwin-0.4.8/trustedtwin/operations/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.8/trustedtwin/operations/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4998 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/docs.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1551 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/history.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4773 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/identities.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4320 2022-09-29 10:14:24.000000 trustedtwin-0.4.8/trustedtwin/operations/indexes.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3635 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/ledgers.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1110 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/log.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3144 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/notifications.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3288 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/roles.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3215 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/secrets.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3932 2022-09-29 10:14:24.000000 trustedtwin-0.4.8/trustedtwin/operations/stickers.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4842 2022-09-29 10:14:24.000000 trustedtwin-0.4.8/trustedtwin/operations/timeseries.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1833 2022-09-27 13:35:12.000000 trustedtwin-0.4.8/trustedtwin/operations/token.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      571 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/trace.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2767 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/twins.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1375 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/usage.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2843 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/users.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      583 2022-09-16 13:45:24.000000 trustedtwin-0.4.8/trustedtwin/operations/who_am_i.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4398 2022-09-29 10:14:24.000000 trustedtwin-0.4.8/trustedtwin/service.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-29 11:08:37.184132 trustedtwin-0.4.8/trustedtwin.egg-info/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      941 2022-09-29 11:08:37.000000 trustedtwin-0.4.8/trustedtwin.egg-info/PKG-INFO
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1173 2022-09-29 11:08:37.000000 trustedtwin-0.4.8/trustedtwin.egg-info/SOURCES.txt
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        1 2022-09-29 11:08:37.000000 trustedtwin-0.4.8/trustedtwin.egg-info/dependency_links.txt
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        1 2022-05-20 04:10:03.000000 trustedtwin-0.4.8/trustedtwin.egg-info/not-zip-safe
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        9 2022-09-29 11:08:37.000000 trustedtwin-0.4.8/trustedtwin.egg-info/requires.txt
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)       35 2022-09-29 11:08:37.000000 trustedtwin-0.4.8/trustedtwin.egg-info/top_level.txt
+drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1106 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/LICENSE
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      941 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/PKG-INFO
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      625 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/README.md
+drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.524953 trustedtwin-0.4.9/api_generator/
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/api_generator/__init__.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)    12134 2022-05-19 08:31:57.000000 trustedtwin-0.4.9/api_generator/generate.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2545 2022-06-07 10:10:43.000000 trustedtwin-0.4.9/api_generator/templates.py
+drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/examples/
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/examples/__init__.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3461 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/examples/ledgers.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1495 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/examples/twins.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      103 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/setup.cfg
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      518 2022-09-30 10:40:10.000000 trustedtwin-0.4.9/setup.py
+drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/trustedtwin/
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      129 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/__init__.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2990 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/exceptions.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3323 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/http_client.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      319 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/misc.py
+drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/trustedtwin/models/
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/models/__init__.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      839 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/models/responses.py
+drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/trustedtwin/operations/
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/operations/__init__.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4998 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/docs.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1551 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/history.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4773 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/identities.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4320 2022-09-29 10:14:24.000000 trustedtwin-0.4.9/trustedtwin/operations/indexes.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3635 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/ledgers.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1110 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/log.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3144 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/notifications.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3288 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/roles.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3215 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/secrets.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3933 2022-09-30 10:25:16.000000 trustedtwin-0.4.9/trustedtwin/operations/stickers.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4842 2022-09-29 10:14:24.000000 trustedtwin-0.4.9/trustedtwin/operations/timeseries.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1833 2022-09-27 13:35:12.000000 trustedtwin-0.4.9/trustedtwin/operations/token.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      571 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/trace.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2767 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/twins.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1375 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/usage.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2843 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/users.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      583 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/who_am_i.py
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4398 2022-09-29 10:14:24.000000 trustedtwin-0.4.9/trustedtwin/service.py
+drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/trustedtwin.egg-info/
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      941 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/PKG-INFO
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1173 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/SOURCES.txt
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        1 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/dependency_links.txt
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        1 2022-05-20 04:10:03.000000 trustedtwin-0.4.9/trustedtwin.egg-info/not-zip-safe
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        9 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/requires.txt
+-rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)       35 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/top_level.txt
```

### Comparing `trustedtwin-0.4.8/LICENSE` & `trustedtwin-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/PKG-INFO` & `trustedtwin-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedtwin
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python client for Trusted Twin API
 Home-page: https://gitlab.com/trustedtwinpublic/trustedtwin-python
 Author: TrustedTwin
 Author-email: api@trustedtwin.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `trustedtwin-0.4.8/README.md` & `trustedtwin-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/api_generator/generate.py` & `trustedtwin-0.4.9/api_generator/generate.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/api_generator/templates.py` & `trustedtwin-0.4.9/api_generator/templates.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/examples/ledgers.py` & `trustedtwin-0.4.9/examples/ledgers.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/examples/twins.py` & `trustedtwin-0.4.9/examples/twins.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/setup.py` & `trustedtwin-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='trustedtwin',
-    version='0.4.8',
+    version='0.4.9',
     url='https://gitlab.com/trustedtwinpublic/trustedtwin-python',
     long_description_content_type="text/markdown",
     license='MIT',
     author='TrustedTwin',
     author_email='api@trustedtwin.com',
     description='Python client for Trusted Twin API',
     packages=find_packages(exclude=['tests']),
```

### Comparing `trustedtwin-0.4.8/trustedtwin/exceptions.py` & `trustedtwin-0.4.9/trustedtwin/exceptions.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/http_client.py` & `trustedtwin-0.4.9/trustedtwin/http_client.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/models/responses.py` & `trustedtwin-0.4.9/trustedtwin/models/responses.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/docs.py` & `trustedtwin-0.4.9/trustedtwin/operations/docs.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/history.py` & `trustedtwin-0.4.9/trustedtwin/operations/history.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/identities.py` & `trustedtwin-0.4.9/trustedtwin/operations/identities.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/indexes.py` & `trustedtwin-0.4.9/trustedtwin/operations/indexes.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/ledgers.py` & `trustedtwin-0.4.9/trustedtwin/operations/ledgers.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/log.py` & `trustedtwin-0.4.9/trustedtwin/operations/log.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/notifications.py` & `trustedtwin-0.4.9/trustedtwin/operations/notifications.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/roles.py` & `trustedtwin-0.4.9/trustedtwin/operations/roles.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/secrets.py` & `trustedtwin-0.4.9/trustedtwin/operations/secrets.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/stickers.py` & `trustedtwin-0.4.9/trustedtwin/operations/stickers.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def list_stickers(
         self,
         color: Optional[str] = None,
         context: Optional[str] = None,
         ge: Optional[float] = None,
         le: Optional[float] = None,
         limit: Optional[int] = None,
-        start: Optional[list] = None
+        start: Optional[tuple] = None
     ) -> Dict:
         """Execute list_stickers API operation"""
 
         endpoint = "stickers"
         endpoint = urllib.parse.quote(endpoint)
         params = {
             "color": color,
```

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/timeseries.py` & `trustedtwin-0.4.9/trustedtwin/operations/timeseries.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/token.py` & `trustedtwin-0.4.9/trustedtwin/operations/token.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/trace.py` & `trustedtwin-0.4.9/trustedtwin/operations/trace.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/twins.py` & `trustedtwin-0.4.9/trustedtwin/operations/twins.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/usage.py` & `trustedtwin-0.4.9/trustedtwin/operations/usage.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/users.py` & `trustedtwin-0.4.9/trustedtwin/operations/users.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/operations/who_am_i.py` & `trustedtwin-0.4.9/trustedtwin/operations/who_am_i.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin/service.py` & `trustedtwin-0.4.9/trustedtwin/service.py`

 * *Files identical despite different names*

### Comparing `trustedtwin-0.4.8/trustedtwin.egg-info/PKG-INFO` & `trustedtwin-0.4.9/trustedtwin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedtwin
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python client for Trusted Twin API
 Home-page: https://gitlab.com/trustedtwinpublic/trustedtwin-python
 Author: TrustedTwin
 Author-email: api@trustedtwin.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `trustedtwin-0.4.8/trustedtwin.egg-info/SOURCES.txt` & `trustedtwin-0.4.9/trustedtwin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

