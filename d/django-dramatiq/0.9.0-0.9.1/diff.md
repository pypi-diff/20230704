# Comparing `tmp/django_dramatiq-0.9.0.tar.gz` & `tmp/django_dramatiq-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django_dramatiq-0.9.0.tar", last modified: Sat Feb  1 11:33:14 2020, max compression
+gzip compressed data, was "dist/django_dramatiq-0.9.1.tar", last modified: Tue Feb  4 08:44:23 2020, max compression
```

## Comparing `django_dramatiq-0.9.0.tar` & `django_dramatiq-0.9.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/
--rw-r--r--   0 bogdan     (501) staff       (20)       73 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/MANIFEST.in
--rw-r--r--   0 bogdan     (501) staff       (20)      748 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/PKG-INFO
--rw-r--r--   0 bogdan     (501) staff       (20)     7427 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/README.md
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq/
--rw-r--r--   0 bogdan     (501) staff       (20)       88 2020-02-01 11:32:57.000000 django_dramatiq-0.9.0/django_dramatiq/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1657 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/admin.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3801 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/apps.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq/management/
--rw-r--r--   0 bogdan     (501) staff       (20)        0 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/management/__init__.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq/management/commands/
--rw-r--r--   0 bogdan     (501) staff       (20)        0 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/management/commands/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     5550 2020-01-23 11:01:00.000000 django_dramatiq-0.9.0/django_dramatiq/management/commands/rundramatiq.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2346 2020-01-23 11:16:31.000000 django_dramatiq-0.9.0/django_dramatiq/middleware.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq/migrations/
--rw-r--r--   0 bogdan     (501) staff       (20)     1084 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/migrations/0001_initial.py
--rw-r--r--   0 bogdan     (501) staff       (20)      863 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/migrations/0002_auto_20191104_1354.py
--rw-r--r--   0 bogdan     (501) staff       (20)        0 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/migrations/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1984 2020-01-23 11:16:31.000000 django_dramatiq-0.9.0/django_dramatiq/models.py
--rw-r--r--   0 bogdan     (501) staff       (20)       30 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/setup.py
--rw-r--r--   0 bogdan     (501) staff       (20)      243 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/tasks.py
--rw-r--r--   0 bogdan     (501) staff       (20)      438 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/test.py
--rw-r--r--   0 bogdan     (501) staff       (20)      494 2020-01-23 10:56:18.000000 django_dramatiq-0.9.0/django_dramatiq/utils.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq.egg-info/
--rw-r--r--   0 bogdan     (501) staff       (20)      748 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq.egg-info/PKG-INFO
--rw-r--r--   0 bogdan     (501) staff       (20)      740 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq.egg-info/SOURCES.txt
--rw-r--r--   0 bogdan     (501) staff       (20)        1 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq.egg-info/dependency_links.txt
--rw-r--r--   0 bogdan     (501) staff       (20)      118 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq.egg-info/requires.txt
--rw-r--r--   0 bogdan     (501) staff       (20)       16 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/django_dramatiq.egg-info/top_level.txt
--rw-r--r--   0 bogdan     (501) staff       (20)      512 2020-02-01 11:33:14.000000 django_dramatiq-0.9.0/setup.cfg
--rw-r--r--   0 bogdan     (501) staff       (20)     1749 2020-01-23 11:01:00.000000 django_dramatiq-0.9.0/setup.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/
+-rw-r--r--   0 bogdan     (501) staff       (20)       73 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/MANIFEST.in
+-rw-r--r--   0 bogdan     (501) staff       (20)      748 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/PKG-INFO
+-rw-r--r--   0 bogdan     (501) staff       (20)     7427 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/README.md
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq/
+-rw-r--r--   0 bogdan     (501) staff       (20)       88 2020-02-04 08:44:16.000000 django_dramatiq-0.9.1/django_dramatiq/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1657 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/admin.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     3801 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/apps.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq/management/
+-rw-r--r--   0 bogdan     (501) staff       (20)        0 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/management/__init__.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq/management/commands/
+-rw-r--r--   0 bogdan     (501) staff       (20)        0 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/management/commands/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     5550 2020-01-23 11:01:00.000000 django_dramatiq-0.9.1/django_dramatiq/management/commands/rundramatiq.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2346 2020-01-23 11:16:31.000000 django_dramatiq-0.9.1/django_dramatiq/middleware.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq/migrations/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1084 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/migrations/0001_initial.py
+-rw-r--r--   0 bogdan     (501) staff       (20)      863 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/migrations/0002_auto_20191104_1354.py
+-rw-r--r--   0 bogdan     (501) staff       (20)      765 2020-02-04 08:42:44.000000 django_dramatiq-0.9.1/django_dramatiq/migrations/0003_auto_20200204_0842.py
+-rw-r--r--   0 bogdan     (501) staff       (20)        0 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/migrations/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1984 2020-01-23 11:16:31.000000 django_dramatiq-0.9.1/django_dramatiq/models.py
+-rw-r--r--   0 bogdan     (501) staff       (20)       30 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/setup.py
+-rw-r--r--   0 bogdan     (501) staff       (20)      243 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/tasks.py
+-rw-r--r--   0 bogdan     (501) staff       (20)      438 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/test.py
+-rw-r--r--   0 bogdan     (501) staff       (20)      494 2020-01-23 10:56:18.000000 django_dramatiq-0.9.1/django_dramatiq/utils.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq.egg-info/
+-rw-r--r--   0 bogdan     (501) staff       (20)      748 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq.egg-info/PKG-INFO
+-rw-r--r--   0 bogdan     (501) staff       (20)      794 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq.egg-info/SOURCES.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)        1 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq.egg-info/dependency_links.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)      118 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq.egg-info/requires.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)       16 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/django_dramatiq.egg-info/top_level.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)      512 2020-02-04 08:44:23.000000 django_dramatiq-0.9.1/setup.cfg
+-rw-r--r--   0 bogdan     (501) staff       (20)     1749 2020-01-23 11:01:00.000000 django_dramatiq-0.9.1/setup.py
```

### Comparing `django_dramatiq-0.9.0/PKG-INFO` & `django_dramatiq-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_dramatiq
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Django app for Dramatiq.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: Visit https://github.com/Bogdanp/django_dramatiq for more information.
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
```

### Comparing `django_dramatiq-0.9.0/README.md` & `django_dramatiq-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/django_dramatiq/admin.py` & `django_dramatiq-0.9.1/django_dramatiq/admin.py`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/django_dramatiq/apps.py` & `django_dramatiq-0.9.1/django_dramatiq/apps.py`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/django_dramatiq/management/commands/rundramatiq.py` & `django_dramatiq-0.9.1/django_dramatiq/management/commands/rundramatiq.py`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/django_dramatiq/middleware.py` & `django_dramatiq-0.9.1/django_dramatiq/middleware.py`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/django_dramatiq/migrations/0001_initial.py` & `django_dramatiq-0.9.1/django_dramatiq/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/django_dramatiq/migrations/0002_auto_20191104_1354.py` & `django_dramatiq-0.9.1/django_dramatiq/migrations/0002_auto_20191104_1354.py`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/django_dramatiq/models.py` & `django_dramatiq-0.9.1/django_dramatiq/models.py`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/django_dramatiq.egg-info/PKG-INFO` & `django_dramatiq-0.9.1/django_dramatiq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dramatiq
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Django app for Dramatiq.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: Visit https://github.com/Bogdanp/django_dramatiq for more information.
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
```

### Comparing `django_dramatiq-0.9.0/django_dramatiq.egg-info/SOURCES.txt` & `django_dramatiq-0.9.1/django_dramatiq.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 django_dramatiq.egg-info/requires.txt
 django_dramatiq.egg-info/top_level.txt
 django_dramatiq/management/__init__.py
 django_dramatiq/management/commands/__init__.py
 django_dramatiq/management/commands/rundramatiq.py
 django_dramatiq/migrations/0001_initial.py
 django_dramatiq/migrations/0002_auto_20191104_1354.py
+django_dramatiq/migrations/0003_auto_20200204_0842.py
 django_dramatiq/migrations/__init__.py
```

### Comparing `django_dramatiq-0.9.0/setup.cfg` & `django_dramatiq-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_dramatiq-0.9.0/setup.py` & `django_dramatiq-0.9.1/setup.py`

 * *Files identical despite different names*

