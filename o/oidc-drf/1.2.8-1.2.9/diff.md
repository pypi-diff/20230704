# Comparing `tmp/oidc_drf-1.2.8.tar.gz` & `tmp/oidc_drf-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.2.8.tar", last modified: Tue Jul  4 11:05:30 2023, max compression
+gzip compressed data, was "oidc_drf-1.2.9.tar", last modified: Tue Jul  4 11:09:44 2023, max compression
```

## Comparing `oidc_drf-1.2.8.tar` & `oidc_drf-1.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:05:30.642728 oidc_drf-1.2.8/
--rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 11:05:30.642597 oidc_drf-1.2.8/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     5239 2023-07-04 08:38:47.000000 oidc_drf-1.2.8/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:05:30.641536 oidc_drf-1.2.8/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.8/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.8/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    16020 2023-07-04 11:05:08.000000 oidc_drf-1.2.8/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.8/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:05:30.642456 oidc_drf-1.2.8/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.8/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.8/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.8/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.8/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     8684 2023-07-04 11:01:44.000000 oidc_drf-1.2.8/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:05:30.642310 oidc_drf-1.2.8/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-04 11:05:30.642763 oidc_drf-1.2.8/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-04 11:05:27.000000 oidc_drf-1.2.8/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:09:44.923215 oidc_drf-1.2.9/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 11:09:44.923090 oidc_drf-1.2.9/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5239 2023-07-04 08:38:47.000000 oidc_drf-1.2.9/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:09:44.922111 oidc_drf-1.2.9/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.9/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.9/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    16020 2023-07-04 11:05:08.000000 oidc_drf-1.2.9/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.9/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:09:44.922935 oidc_drf-1.2.9/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.9/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.9/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.9/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.9/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     8944 2023-07-04 11:09:32.000000 oidc_drf-1.2.9/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:09:44.922797 oidc_drf-1.2.9/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-04 11:09:44.000000 oidc_drf-1.2.9/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-04 11:09:44.923249 oidc_drf-1.2.9/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-04 11:09:41.000000 oidc_drf-1.2.9/setup.py
```

### Comparing `oidc_drf-1.2.8/PKG-INFO` & `oidc_drf-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc_drf
-Version: 1.2.8
+Version: 1.2.9
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.2.8/README.md` & `oidc_drf-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.8/oidc_drf/admin.py` & `oidc_drf-1.2.9/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.8/oidc_drf/backends.py` & `oidc_drf-1.2.9/oidc_drf/backends.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.8/oidc_drf/drf.py` & `oidc_drf-1.2.9/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.8/oidc_drf/utils.py` & `oidc_drf-1.2.9/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.8/oidc_drf/views.py` & `oidc_drf-1.2.9/oidc_drf/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from rest_framework.views import APIView
 from rest_framework.response import Response
 from rest_framework import status
 from urllib.parse import urlencode
 from django.utils.crypto import get_random_string
 from oidc_drf.utils import import_from_settings
 import requests
+LOGGER = logging.getLogger(__name__)
 
 
 from  oidc_drf.utils import generate_code_challenge
 
 class OIDCGenerateAuthenticationUrlView(APIView):
     permission_classes = [AllowAny]    
     def get(self, request):
@@ -106,14 +107,18 @@
             return JsonResponse(data)
     
         except:
             return self.login_failure("Login failed")
 
 
     def post(self, request):
+        LOGGER.debug("=================== LOGGER.debug===================")
+        print("=======================================")
+        print("=======================================")
+        print("in post request")
         """Callback handler for OIDC authorization code flow"""
         data = request.data
         
         if "error" in request.GET:
             return self.login_failure(request.GET.get("error_description"))
         
         elif import_from_settings("OIDC_USE_PKCE", True):
```

### Comparing `oidc_drf-1.2.8/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.2.9/oidc_drf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-drf
-Version: 1.2.8
+Version: 1.2.9
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.2.8/setup.py` & `oidc_drf-1.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.2.8',
+    version='1.2.9',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

