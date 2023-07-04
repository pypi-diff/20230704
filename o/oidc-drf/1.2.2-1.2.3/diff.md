# Comparing `tmp/oidc_drf-1.2.2.tar.gz` & `tmp/oidc_drf-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.2.2.tar", last modified: Tue Jul  4 09:00:47 2023, max compression
+gzip compressed data, was "oidc_drf-1.2.3.tar", last modified: Tue Jul  4 09:11:10 2023, max compression
```

## Comparing `oidc_drf-1.2.2.tar` & `oidc_drf-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 09:00:47.059312 oidc_drf-1.2.2/
--rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 09:00:47.059118 oidc_drf-1.2.2/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     5239 2023-07-04 08:38:47.000000 oidc_drf-1.2.2/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 09:00:47.057762 oidc_drf-1.2.2/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.2/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.2/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    15758 2023-07-03 09:52:34.000000 oidc_drf-1.2.2/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.2/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 09:00:47.058885 oidc_drf-1.2.2/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.2/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.2/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.2/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.2/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     8140 2023-07-04 09:00:30.000000 oidc_drf-1.2.2/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 09:00:47.058677 oidc_drf-1.2.2/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 09:00:47.000000 oidc_drf-1.2.2/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-04 09:00:47.000000 oidc_drf-1.2.2/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-04 09:00:47.000000 oidc_drf-1.2.2/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-04 09:00:47.000000 oidc_drf-1.2.2/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-04 09:00:47.000000 oidc_drf-1.2.2/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-04 09:00:47.059355 oidc_drf-1.2.2/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-04 09:00:41.000000 oidc_drf-1.2.2/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 09:11:10.421074 oidc_drf-1.2.3/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 09:11:10.420961 oidc_drf-1.2.3/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5239 2023-07-04 08:38:47.000000 oidc_drf-1.2.3/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 09:11:10.420001 oidc_drf-1.2.3/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.3/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.3/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    15758 2023-07-03 09:52:34.000000 oidc_drf-1.2.3/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.3/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 09:11:10.420822 oidc_drf-1.2.3/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.3/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.3/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.3/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.3/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     8162 2023-07-04 09:10:59.000000 oidc_drf-1.2.3/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 09:11:10.420694 oidc_drf-1.2.3/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 09:11:10.000000 oidc_drf-1.2.3/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-04 09:11:10.000000 oidc_drf-1.2.3/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-04 09:11:10.000000 oidc_drf-1.2.3/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-04 09:11:10.000000 oidc_drf-1.2.3/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-04 09:11:10.000000 oidc_drf-1.2.3/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-04 09:11:10.421106 oidc_drf-1.2.3/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-04 09:11:07.000000 oidc_drf-1.2.3/setup.py
```

### Comparing `oidc_drf-1.2.2/PKG-INFO` & `oidc_drf-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc_drf
-Version: 1.2.2
+Version: 1.2.3
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.2.2/README.md` & `oidc_drf-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.2/oidc_drf/admin.py` & `oidc_drf-1.2.3/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.2/oidc_drf/backends.py` & `oidc_drf-1.2.3/oidc_drf/backends.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.2/oidc_drf/drf.py` & `oidc_drf-1.2.3/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.2/oidc_drf/utils.py` & `oidc_drf-1.2.3/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.2/oidc_drf/views.py` & `oidc_drf-1.2.3/oidc_drf/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             return self.login_failure("Login failed")
 
 
     def post(self, request):
         """Callback handler for OIDC authorization code flow"""
 
         if "error" in request.GET:
-            return self.login_failure(request.GET.get("error"))
+            return self.login_failure(request.GET.get("error_message"))
 
         elif "code" in request.GET and "state" in request.GET:
 
             data = request.data
             
             kwargs = {
                 "request": request,
@@ -125,15 +125,15 @@
             }
 
             self.user = auth.authenticate(**kwargs)
             
             if self.user and self.user.is_active:
                 return self.login_success()
         
-        return self.login_failure()
+        return self.login_failure("Login failed")
 
 class OIDCLogoutView(APIView):
     permission_classes = [AllowAny]    
 
     def post(self, request):     
         oidc_id_token = request.data.get('oidc_id_token', '')
         if oidc_id_token:
```

### Comparing `oidc_drf-1.2.2/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.2.3/oidc_drf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-drf
-Version: 1.2.2
+Version: 1.2.3
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.2.2/setup.py` & `oidc_drf-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.2.2',
+    version='1.2.3',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

