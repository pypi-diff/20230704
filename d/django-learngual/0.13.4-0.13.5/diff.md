# Comparing `tmp/django-learngual-0.13.4.tar.gz` & `tmp/django-learngual-0.13.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.13.4.tar", last modified: Mon Jul  3 12:11:02 2023, max compression
+gzip compressed data, was "django-learngual-0.13.5.tar", last modified: Tue Jul  4 13:07:20 2023, max compression
```

## Comparing `django-learngual-0.13.4.tar` & `django-learngual-0.13.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-03 12:09:56.000000 django-learngual-0.13.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 12:09:56.000000 django-learngual-0.13.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-03 12:11:02.212942 django-learngual-0.13.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-03 12:09:56.000000 django-learngual-0.13.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.208942 django-learngual-0.13.4/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-03 12:11:02.000000 django-learngual-0.13.4/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 12:11:02.000000 django-learngual-0.13.4/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:11:02.000000 django-learngual-0.13.4/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 12:11:02.000000 django-learngual-0.13.4/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/learngual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-03 12:11:02.212942 django-learngual-0.13.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:09:56.000000 django-learngual-0.13.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-04 13:06:29.000000 django-learngual-0.13.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 13:06:29.000000 django-learngual-0.13.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-04 13:07:20.167372 django-learngual-0.13.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-04 13:06:29.000000 django-learngual-0.13.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.163372 django-learngual-0.13.5/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-04 13:07:20.000000 django-learngual-0.13.5/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-04 13:07:20.000000 django-learngual-0.13.5/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:07:20.000000 django-learngual-0.13.5/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 13:07:20.000000 django-learngual-0.13.5/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/learngual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-04 13:07:20.171372 django-learngual-0.13.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:06:29.000000 django-learngual-0.13.5/setup.py
```

### Comparing `django-learngual-0.13.4/LICENSE` & `django-learngual-0.13.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/PKG-INFO` & `django-learngual-0.13.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.4
+Version: 0.13.5
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.4/README.rst` & `django-learngual-0.13.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.13.5/django_learngual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.4
+Version: 0.13.5
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.4/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.13.5/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/learngual/apps.py` & `django-learngual-0.13.5/learngual/apps.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/learngual/authentication.py` & `django-learngual-0.13.5/learngual/authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/learngual/permissions.py` & `django-learngual-0.13.5/learngual/permissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,7 +35,20 @@
         """
 
         def has_permission(self, request, view):
             api_key = str(
                 request.META.get("HTTP_API_KEY", "") or request.GET.get("api-key", "")
             )
             return bool(api_key)
+
+    class IsNotApiKey(permissions.BasePermission):
+        """if request is not made with an api key
+
+        Args:
+            permissions (_type_): _description_
+        """
+
+        def has_permission(self, request, view):
+            api_key = str(
+                request.META.get("HTTP_API_KEY", "") or request.GET.get("api-key", "")
+            )
+            return not bool(api_key) and request.user.is_authenticated
```

### Comparing `django-learngual-0.13.4/learngual/tests/request_mock.py` & `django-learngual-0.13.5/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/learngual/tests/test_authentication.py` & `django-learngual-0.13.5/learngual/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/learngual/tests/test_utils.py` & `django-learngual-0.13.5/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/learngual/utils.py` & `django-learngual-0.13.5/learngual/utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.4/setup.cfg` & `django-learngual-0.13.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.13.4
+version = 0.13.5
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

