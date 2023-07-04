# Comparing `tmp/wagtail-external-link-richtext-1.1.tar.gz` & `tmp/wagtail-external-link-richtext-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-external-link-richtext-1.1.tar", last modified: Mon Jul  3 14:46:37 2023, max compression
+gzip compressed data, was "wagtail-external-link-richtext-1.1.1.tar", last modified: Tue Jul  4 13:56:50 2023, max compression
```

## Comparing `wagtail-external-link-richtext-1.1.tar` & `wagtail-external-link-richtext-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 14:46:37.210961 wagtail-external-link-richtext-1.1/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       59 2023-07-03 13:55:40.000000 wagtail-external-link-richtext-1.1/MANIFEST.in
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1259 2023-07-03 14:46:37.211449 wagtail-external-link-richtext-1.1/PKG-INFO
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      601 2023-07-03 14:39:39.000000 wagtail-external-link-richtext-1.1/README.rst
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 14:46:37.200779 wagtail-external-link-richtext-1.1/external_link/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1/external_link/__init__.py
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      894 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1/external_link/handlers.py
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 14:46:37.201576 wagtail-external-link-richtext-1.1/external_link/migrations/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1/external_link/migrations/__init__.py
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 14:46:37.196765 wagtail-external-link-richtext-1.1/external_link/static/
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 14:46:37.201988 wagtail-external-link-richtext-1.1/external_link/static/css/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      617 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1/external_link/static/css/newtab_form.css
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 14:46:37.202733 wagtail-external-link-richtext-1.1/external_link/static/js/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     6401 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1/external_link/static/js/newtab.js
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1310 2023-07-03 12:07:09.000000 wagtail-external-link-richtext-1.1/external_link/wagtail_hooks.py
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      714 2023-07-03 14:46:37.214263 wagtail-external-link-richtext-1.1/setup.cfg
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       37 2023-07-03 13:56:32.000000 wagtail-external-link-richtext-1.1/setup.py
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 14:46:37.209818 wagtail-external-link-richtext-1.1/wagtail_external_link_richtext.egg-info/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1259 2023-07-03 14:46:37.000000 wagtail-external-link-richtext-1.1/wagtail_external_link_richtext.egg-info/PKG-INFO
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      452 2023-07-03 14:46:37.000000 wagtail-external-link-richtext-1.1/wagtail_external_link_richtext.egg-info/SOURCES.txt
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        1 2023-07-03 14:46:37.000000 wagtail-external-link-richtext-1.1/wagtail_external_link_richtext.egg-info/dependency_links.txt
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       14 2023-07-03 14:46:37.000000 wagtail-external-link-richtext-1.1/wagtail_external_link_richtext.egg-info/top_level.txt
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.090724 wagtail-external-link-richtext-1.1.1/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     1058 2023-07-04 11:49:42.000000 wagtail-external-link-richtext-1.1.1/LICENSE
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)       59 2023-07-03 13:55:40.000000 wagtail-external-link-richtext-1.1.1/MANIFEST.in
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     2554 2023-07-04 13:56:50.090183 wagtail-external-link-richtext-1.1.1/PKG-INFO
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)      587 2023-07-04 13:56:37.000000 wagtail-external-link-richtext-1.1.1/README.rst
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.082483 wagtail-external-link-richtext-1.1.1/external_link/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1.1/external_link/__init__.py
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)      894 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.1/external_link/handlers.py
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.083050 wagtail-external-link-richtext-1.1.1/external_link/migrations/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1.1/external_link/migrations/__init__.py
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.078301 wagtail-external-link-richtext-1.1.1/external_link/static/
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.083547 wagtail-external-link-richtext-1.1.1/external_link/static/css/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)      617 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.1/external_link/static/css/newtab_form.css
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.084167 wagtail-external-link-richtext-1.1.1/external_link/static/js/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     6401 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.1/external_link/static/js/newtab.js
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     1310 2023-07-03 12:07:09.000000 wagtail-external-link-richtext-1.1.1/external_link/wagtail_hooks.py
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     1017 2023-07-04 13:54:54.000000 wagtail-external-link-richtext-1.1.1/pyproject.toml
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)       38 2023-07-04 13:56:50.090878 wagtail-external-link-richtext-1.1.1/setup.cfg
+drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-04 13:56:50.089424 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)     2554 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/PKG-INFO
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)      509 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/SOURCES.txt
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)        1 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/dependency_links.txt
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)       35 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/requires.txt
+-rw-r--r--   0 rubenhesselink   (501) staff       (20)       14 2023-07-04 13:56:50.000000 wagtail-external-link-richtext-1.1.1/wagtail_external_link_richtext.egg-info/top_level.txt
```

### Comparing `wagtail-external-link-richtext-1.1/README.rst` & `wagtail-external-link-richtext-1.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Quick start
 ------------
 1. Go to your settings and add `external_link` to your `INSTALLED_APPS`
 
     INSTALLED_APPS = [
 
         "...",
+
         "external_link",
-        "...",
 
     ]
 
 
 2. Go to the settings file and add `new_tab_link` to the `RICHTEXT_FEATURES`
 3. When adding or editing a page in the wagtail admin there will be a `New tab` button in the `Richtextfield`
```

### Comparing `wagtail-external-link-richtext-1.1/external_link/handlers.py` & `wagtail-external-link-richtext-1.1.1/external_link/handlers.py`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1/external_link/static/css/newtab_form.css` & `wagtail-external-link-richtext-1.1.1/external_link/static/css/newtab_form.css`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1/external_link/static/js/newtab.js` & `wagtail-external-link-richtext-1.1.1/external_link/static/js/newtab.js`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1/external_link/wagtail_hooks.py` & `wagtail-external-link-richtext-1.1.1/external_link/wagtail_hooks.py`

 * *Files identical despite different names*

