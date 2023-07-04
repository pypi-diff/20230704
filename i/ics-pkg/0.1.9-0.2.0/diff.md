# Comparing `tmp/ics-pkg-0.1.9.tar.gz` & `tmp/ics-pkg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ics-pkg-0.1.9.tar", last modified: Fri Feb 17 12:31:55 2023, max compression
+gzip compressed data, was "ics-pkg-0.2.0.tar", last modified: Tue Jul  4 07:01:03 2023, max compression
```

## Comparing `ics-pkg-0.1.9.tar` & `ics-pkg-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10811 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9761 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.987065 ics-pkg-0.1.9/ics/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.987065 ics-pkg-0.1.9/ics/apps/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.987065 ics-pkg-0.1.9/ics/apps/media/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.987065 ics-pkg-0.1.9/ics/apps/media/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.987065 ics-pkg-0.1.9/ics/apps/media/js/
--rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/js/utility.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.987065 ics-pkg-0.1.9/ics/apps/media/template/
--rw-r--r--   0 runner    (1001) docker     (122)     3384 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/about.html
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/admin_basewithmenu.html
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/basewithmenu.html
--rw-r--r--   0 runner    (1001) docker     (122)    38561 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/browseandcode.html
--rw-r--r--   0 runner    (1001) docker     (122)    20936 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/classification_view.html
--rw-r--r--   0 runner    (1001) docker     (122)    51881 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/classifiers.html
--rw-r--r--   0 runner    (1001) docker     (122)    16064 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/classify.html
--rw-r--r--   0 runner    (1001) docker     (122)    21955 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/datasets.html
--rw-r--r--   0 runner    (1001) docker     (122)    21047 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/ips.html
--rw-r--r--   0 runner    (1001) docker     (122)    15971 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/jobs.html
--rw-r--r--   0 runner    (1001) docker     (122)    22362 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/keys.html
--rw-r--r--   0 runner    (1001) docker     (122)     8339 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/locks.html
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/login.html
--rw-r--r--   0 runner    (1001) docker     (122)     7466 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/public_api.html
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/public_basewithmenu.html
--rw-r--r--   0 runner    (1001) docker     (122)    16582 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/public_typeandcode.html
--rw-r--r--   0 runner    (1001) docker     (122)    17504 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/training_data_view.html
--rw-r--r--   0 runner    (1001) docker     (122)    20563 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/typeandcode.html
--rw-r--r--   0 runner    (1001) docker     (122)    24150 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/media/template/users.html
--rw-r--r--   0 runner    (1001) docker     (122)     3625 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/web_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5794 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/web_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/apps/web_public.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/ics/classifier/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/classifier/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/classifier/classifier.py
--rw-r--r--   0 runner    (1001) docker     (122)    12116 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/classifier/lri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5010 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/classifier/lri_online_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/ics/client/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    31044 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/client/client_session.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/ics/db/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    70778 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/db/sqlalchemydb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/ics/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36116 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/scripts/list_exposed_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/scripts/twitter_uploader.py
--rw-r--r--   0 runner    (1001) docker     (122)    11736 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/scripts/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/ics/services/
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/auth_controller_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     6390 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/background_processor_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    39465 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/classifier_collection_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    25701 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/dataset_collection_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     4737 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/ip_controller_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/jobs_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     4419 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/key_controller_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/services/user_controller_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/ics/util/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/ics/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/ics_pkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10811 2023-02-17 12:31:55.000000 ics-pkg-0.1.9/ics_pkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-02-17 12:31:55.000000 ics-pkg-0.1.9/ics_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-17 12:31:55.000000 ics-pkg-0.1.9/ics_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-02-17 12:31:55.000000 ics-pkg-0.1.9/ics_pkg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-17 12:31:55.000000 ics-pkg-0.1.9/ics_pkg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-02-17 12:31:55.000000 ics-pkg-0.1.9/ics_pkg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-17 12:31:55.991065 ics-pkg-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-02-17 12:31:45.000000 ics-pkg-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.671054 ics-pkg-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11838 2023-07-04 07:01:03.671054 ics-pkg-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10788 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.663054 ics-pkg-0.2.0/ics/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.663054 ics-pkg-0.2.0/ics/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.663054 ics-pkg-0.2.0/ics/apps/media/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.663054 ics-pkg-0.2.0/ics/apps/media/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.663054 ics-pkg-0.2.0/ics/apps/media/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/js/utility.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.667054 ics-pkg-0.2.0/ics/apps/media/template/
+-rw-r--r--   0 runner    (1001) docker     (122)     3384 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/about.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/admin_basewithmenu.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/basewithmenu.html
+-rw-r--r--   0 runner    (1001) docker     (122)    38561 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/browseandcode.html
+-rw-r--r--   0 runner    (1001) docker     (122)    20936 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/classification_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)    51881 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/classifiers.html
+-rw-r--r--   0 runner    (1001) docker     (122)    16064 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/classify.html
+-rw-r--r--   0 runner    (1001) docker     (122)    21955 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/datasets.html
+-rw-r--r--   0 runner    (1001) docker     (122)    21047 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/ips.html
+-rw-r--r--   0 runner    (1001) docker     (122)    15572 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/jobs.html
+-rw-r--r--   0 runner    (1001) docker     (122)    22362 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/keys.html
+-rw-r--r--   0 runner    (1001) docker     (122)     8339 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/locks.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/login.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7466 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/public_api.html
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/public_basewithmenu.html
+-rw-r--r--   0 runner    (1001) docker     (122)    16582 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/public_typeandcode.html
+-rw-r--r--   0 runner    (1001) docker     (122)    17504 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/training_data_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)    20563 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/typeandcode.html
+-rw-r--r--   0 runner    (1001) docker     (122)    24150 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/media/template/users.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3625 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/web_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5794 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/web_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/apps/web_public.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.667054 ics-pkg-0.2.0/ics/classifier/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/classifier/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/classifier/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12116 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/classifier/lri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5010 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/classifier/lri_online_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.667054 ics-pkg-0.2.0/ics/client/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31044 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/client/client_session.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.667054 ics-pkg-0.2.0/ics/db/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71035 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/db/sqlalchemydb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.667054 ics-pkg-0.2.0/ics/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36116 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/scripts/list_exposed_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/scripts/twitter_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13341 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/scripts/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.671054 ics-pkg-0.2.0/ics/services/
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/auth_controller_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6512 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/background_processor_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39465 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/classifier_collection_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25701 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/dataset_collection_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4737 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/ip_controller_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/jobs_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4419 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/key_controller_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/services/user_controller_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.671054 ics-pkg-0.2.0/ics/util/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/ics/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 07:01:03.671054 ics-pkg-0.2.0/ics_pkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11838 2023-07-04 07:01:03.000000 ics-pkg-0.2.0/ics_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-07-04 07:01:03.000000 ics-pkg-0.2.0/ics_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 07:01:03.000000 ics-pkg-0.2.0/ics_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-04 07:01:03.000000 ics-pkg-0.2.0/ics_pkg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-04 07:01:03.000000 ics-pkg-0.2.0/ics_pkg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-07-04 07:01:03.000000 ics-pkg-0.2.0/ics_pkg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 07:01:03.671054 ics-pkg-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-04 07:00:52.000000 ics-pkg-0.2.0/setup.py
```

### Comparing `ics-pkg-0.1.9/COPYING` & `ics-pkg-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/PKG-INFO` & `ics-pkg-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ics-pkg
-Version: 0.1.9
+Version: 0.2.0
 Summary: Interactive Classification System (ICS): a tool for machine learning-supported labeling of text
 Home-page: https://github.com/aesuli/ics
 Author: Andrea Esuli
 Author-email: andrea@esuli.it
 License: BSD
 Project-URL: Bug Reports, https://github.com/aesuli/ics/issues
 Project-URL: Source, https://github.com/aesuli/ics/
@@ -52,38 +52,55 @@
 
 [A. Esuli, "ICS: Total Freedom in Manual Text Classification Supported by Unobtrusive Machine Learning," in IEEE Access, vol. 10, pp. 64741-64760, 2022, doi: 10.1109/ACCESS.2022.3184009](https://doi.org/10.1109/ACCESS.2022.3184009)
 
 ## <a name="installation"></a> Installation
 
 You can have a working installation of ICS in many ways:
 
+- [Single file executable](#single-file-executable) (to start using ICS)
 - [Docker](#docker) (for a single user)
-- [Docker compose](#docker-compose) (recommended for most cases)
+- [Docker compose](#docker-compose) (for larger installation)
 - [Pip install](#pip)
 - [From source](#from-source)
 
+### Single file executable
+
+Executable files of ICS are downloadable from the [releases page](https://github.com/aesuli/ics/releases).
+Once downloaded it can be run and have a working instance of ICS, provided a [database is configured](#db-configuration).
+
+```shell
+ics-webapp
+```
+
+
+The executable are from source using [pyinstaller](https://pyinstaller.org/):
+
+```shell
+pyinstaller -F ics\scripts\webapp.py --add-data="ics\apps\media;ics\apps\media" --collect-all sklearn --name ics-webapp
+```
+
 ### Docker
 
 A quick way have a running instance of ICS is to use [Docker](https://docker.com).
 
 ```shell
-docker run -p 8080:8080 andreaesuli/ics
+docker run -p 8080:8080 ghcr.io/aesuli/ics
 ```
 
 This command pulls the ICS image from Docker hub and runs it, publishing the application on port 8080 of the host machine, accessible from any interface.
 Once started ICS is accessible from the host machine using a browser at the address [http://127.0.0.1:8080](http://127.0.0.1:8080)
 
 To have ICS accessible only from the local host machine add local ip address:
 
 ```shell
-docker run -p 127.0.0.1:8080:8080 andreaesuli/ics
+docker run -p 127.0.0.1:8080:8080 ghcr.io/aesuli/ics
 ```
 
-__NOTE:__ by default the ICS image uses the SQLite database engine, which can results in performance drops caused by the access to DB, specially when multiple users access the system.
-A configuration using PostgreSQL is recommended. It can be easily set up using docker compose.
+__NOTE:__ by default the ICS image uses the SQLite database engine, which may result in reduced efficiency and functionalities.
+A configuration using PostgreSQL is strongly recommended. It can be easily set up using docker compose.
 
 #### Data persistence
 
 ICS image use volumes to keep information persistent:
 - ics-db stores the sqlite file, this is the only volume that should be saved to keep the state of the application.
 - ics-data stores the files that are uploaded or downloaded from the system. It is defined for inspection in case of failures, it is not necessary to save it.
 - ics-log stores the log files. It is defined for inspection in case of failures, it is not necessary to save it.
@@ -123,15 +140,15 @@
 On Linux/Mac:
 ```shell
 DB_DATA=/var/lib/ics/data docker compose up
 ```
 
 ### Pip
 
-The suggested way to quickly set up the python enviroment is to use
+The suggested way to quickly set up the python environment is to use
 the [Anaconda/Miniconda distribution](https://www.anaconda.com/products/distribution) and the `conda` package manager to
 create the virtual enviroment.
 
 ```shell
 conda create -n ics python
 conda activate ics
 ````
@@ -156,46 +173,55 @@
 pip install -r requirements.txt
 ```
 
 The last required step is to [configure a database](#db-configuration).
 
 ### DB configuration
 
-Docker installation already includes the setup of the DB, so you can skip this section.
-If you installed ICS using pip or the source code you must set up a DB.
+The Docker compose installation already includes the setup of the PostgreSQL database, so you can skip this section.
+Any another requires to have a database available to connect to.
+The use of [PostgreSQL](https://www.postgresql.org/) is strongly recommended.
 
-The use of [PostgreSQL](https://www.postgresql.org/) is recommended to avoid performance drops caused by the access to 
-DB, specially when multiple users access the system.
-Howerever, ICS can also work using other DB engines, such as [SQLite](https://www.sqlite.org/).
+#### PostgreSQL
 
-#### SQLite
+To connect to PostgreSQL, a dedicated DB must be created.
+These are the SQL commands to create the required user and database on PostgreSQL.
+
+```
+CREATE USER ics WITH PASSWORD 'ics';
+CREATE DATABASE ics;
+GRANT ALL PRIVILEGES ON DATABASE ics to ics;
+```
+
+These commands can be issued using the `psql` SQL shell (or using pgAdmin, or similar db frontends).
+The tables required by ICS are created automatically at the first run.
 
-Running ICS using SQLite as the DB only require to pass a ``--db_connection_string`` argument to the launch script:
+Then ICS can be launched passing the DB connection string:
 
 ```shell
-ics-webapp --db_connection_string sqlite:///ics.sqlite
+ics-webapp --db_connection_string postgresql://ics:ics@localhost:5432/ics
 ```
 
-SQLite is
+The above connection string is the correct one for a locally running database, change it according to your configuration.
 
-#### PostgreSQL
+#### SQLite
 
-By default ICS assumes to connect to PostgreSQL, using a database named 'ics' and a user named 'ics' (with password 'ics').
+By default ICS uses SQLite as the DB, yet please note that **the use of SQLite is intended only for a first exploration of ICS and that using PostgreSQL is strongly recommended**.
+Using SQLite can result in reduced efficiency and some functionalities may be missing or not properly working.
 
-These are the SQL commands to create the required user and database on PostgreSQL.
+To use SQLite use the following ``--db_connection_string`` argument to the launch script:
 
-```
-CREATE USER ics WITH PASSWORD 'ics';
-CREATE DATABASE ics;
-GRANT ALL PRIVILEGES ON DATABASE ics to ics;
+```shell
+ics-webapp --db_connection_string sqlite:///ics.sqlite
 ```
 
-These command can be issued using the `psql` SQL shell (or using pgAdmin, or similar db frontends).
+This is the default connection string, it creates the DB file in the current working directory.
+Change it to point to the path where you want to store your file.
 
-The tables required by ICS are created automatically at the first run.
+Again, PostgreSQL is the recommended database.
 
 ## <a name="startmain"></a> The main app
 
 Running the docker image automatically starts the main application, which can be accessed with a browser at the ip and 
 port defined with the docker launch command or docker compose file.
 Installations that do not use docker can run ics by using the ics-webapp script.
```

### Comparing `ics-pkg-0.1.9/README.md` & `ics-pkg-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,38 +26,55 @@
 
 [A. Esuli, "ICS: Total Freedom in Manual Text Classification Supported by Unobtrusive Machine Learning," in IEEE Access, vol. 10, pp. 64741-64760, 2022, doi: 10.1109/ACCESS.2022.3184009](https://doi.org/10.1109/ACCESS.2022.3184009)
 
 ## <a name="installation"></a> Installation
 
 You can have a working installation of ICS in many ways:
 
+- [Single file executable](#single-file-executable) (to start using ICS)
 - [Docker](#docker) (for a single user)
-- [Docker compose](#docker-compose) (recommended for most cases)
+- [Docker compose](#docker-compose) (for larger installation)
 - [Pip install](#pip)
 - [From source](#from-source)
 
+### Single file executable
+
+Executable files of ICS are downloadable from the [releases page](https://github.com/aesuli/ics/releases).
+Once downloaded it can be run and have a working instance of ICS, provided a [database is configured](#db-configuration).
+
+```shell
+ics-webapp
+```
+
+
+The executable are from source using [pyinstaller](https://pyinstaller.org/):
+
+```shell
+pyinstaller -F ics\scripts\webapp.py --add-data="ics\apps\media;ics\apps\media" --collect-all sklearn --name ics-webapp
+```
+
 ### Docker
 
 A quick way have a running instance of ICS is to use [Docker](https://docker.com).
 
 ```shell
-docker run -p 8080:8080 andreaesuli/ics
+docker run -p 8080:8080 ghcr.io/aesuli/ics
 ```
 
 This command pulls the ICS image from Docker hub and runs it, publishing the application on port 8080 of the host machine, accessible from any interface.
 Once started ICS is accessible from the host machine using a browser at the address [http://127.0.0.1:8080](http://127.0.0.1:8080)
 
 To have ICS accessible only from the local host machine add local ip address:
 
 ```shell
-docker run -p 127.0.0.1:8080:8080 andreaesuli/ics
+docker run -p 127.0.0.1:8080:8080 ghcr.io/aesuli/ics
 ```
 
-__NOTE:__ by default the ICS image uses the SQLite database engine, which can results in performance drops caused by the access to DB, specially when multiple users access the system.
-A configuration using PostgreSQL is recommended. It can be easily set up using docker compose.
+__NOTE:__ by default the ICS image uses the SQLite database engine, which may result in reduced efficiency and functionalities.
+A configuration using PostgreSQL is strongly recommended. It can be easily set up using docker compose.
 
 #### Data persistence
 
 ICS image use volumes to keep information persistent:
 - ics-db stores the sqlite file, this is the only volume that should be saved to keep the state of the application.
 - ics-data stores the files that are uploaded or downloaded from the system. It is defined for inspection in case of failures, it is not necessary to save it.
 - ics-log stores the log files. It is defined for inspection in case of failures, it is not necessary to save it.
@@ -97,15 +114,15 @@
 On Linux/Mac:
 ```shell
 DB_DATA=/var/lib/ics/data docker compose up
 ```
 
 ### Pip
 
-The suggested way to quickly set up the python enviroment is to use
+The suggested way to quickly set up the python environment is to use
 the [Anaconda/Miniconda distribution](https://www.anaconda.com/products/distribution) and the `conda` package manager to
 create the virtual enviroment.
 
 ```shell
 conda create -n ics python
 conda activate ics
 ````
@@ -130,46 +147,55 @@
 pip install -r requirements.txt
 ```
 
 The last required step is to [configure a database](#db-configuration).
 
 ### DB configuration
 
-Docker installation already includes the setup of the DB, so you can skip this section.
-If you installed ICS using pip or the source code you must set up a DB.
+The Docker compose installation already includes the setup of the PostgreSQL database, so you can skip this section.
+Any another requires to have a database available to connect to.
+The use of [PostgreSQL](https://www.postgresql.org/) is strongly recommended.
 
-The use of [PostgreSQL](https://www.postgresql.org/) is recommended to avoid performance drops caused by the access to 
-DB, specially when multiple users access the system.
-Howerever, ICS can also work using other DB engines, such as [SQLite](https://www.sqlite.org/).
+#### PostgreSQL
 
-#### SQLite
+To connect to PostgreSQL, a dedicated DB must be created.
+These are the SQL commands to create the required user and database on PostgreSQL.
+
+```
+CREATE USER ics WITH PASSWORD 'ics';
+CREATE DATABASE ics;
+GRANT ALL PRIVILEGES ON DATABASE ics to ics;
+```
+
+These commands can be issued using the `psql` SQL shell (or using pgAdmin, or similar db frontends).
+The tables required by ICS are created automatically at the first run.
 
-Running ICS using SQLite as the DB only require to pass a ``--db_connection_string`` argument to the launch script:
+Then ICS can be launched passing the DB connection string:
 
 ```shell
-ics-webapp --db_connection_string sqlite:///ics.sqlite
+ics-webapp --db_connection_string postgresql://ics:ics@localhost:5432/ics
 ```
 
-SQLite is
+The above connection string is the correct one for a locally running database, change it according to your configuration.
 
-#### PostgreSQL
+#### SQLite
 
-By default ICS assumes to connect to PostgreSQL, using a database named 'ics' and a user named 'ics' (with password 'ics').
+By default ICS uses SQLite as the DB, yet please note that **the use of SQLite is intended only for a first exploration of ICS and that using PostgreSQL is strongly recommended**.
+Using SQLite can result in reduced efficiency and some functionalities may be missing or not properly working.
 
-These are the SQL commands to create the required user and database on PostgreSQL.
+To use SQLite use the following ``--db_connection_string`` argument to the launch script:
 
-```
-CREATE USER ics WITH PASSWORD 'ics';
-CREATE DATABASE ics;
-GRANT ALL PRIVILEGES ON DATABASE ics to ics;
+```shell
+ics-webapp --db_connection_string sqlite:///ics.sqlite
 ```
 
-These command can be issued using the `psql` SQL shell (or using pgAdmin, or similar db frontends).
+This is the default connection string, it creates the DB file in the current working directory.
+Change it to point to the path where you want to store your file.
 
-The tables required by ICS are created automatically at the first run.
+Again, PostgreSQL is the recommended database.
 
 ## <a name="startmain"></a> The main app
 
 Running the docker image automatically starts the main application, which can be accessed with a browser at the ip and 
 port defined with the docker launch command or docker compose file.
 Installations that do not use docker can run ics by using the ics-webapp script.
```

### Comparing `ics-pkg-0.1.9/ics/apps/media/css/style.css` & `ics-pkg-0.2.0/ics/apps/media/css/style.css`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/js/utility.js` & `ics-pkg-0.2.0/ics/apps/media/js/utility.js`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/about.html` & `ics-pkg-0.2.0/ics/apps/media/template/about.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/admin_basewithmenu.html` & `ics-pkg-0.2.0/ics/apps/media/template/admin_basewithmenu.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/base.html` & `ics-pkg-0.2.0/ics/apps/media/template/base.html`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     ${self.body()}
 </section>
 
 <footer class="w3-container w3-text-theme w3-padding w3-tiny">
     <p><span>Version ${version} - &copy; 2022-2023 <a href="http://esuli.it">Andrea Esuli</a></span> <span
         class="w3-right">Cookie info: this website uses only one session cookie to manage login.</span>
     </p>
-    % if engine_name == 'sqlite':
-    <p class="w3-yellow pointer w3-right" onclick="popup(this,'sqlitepopup')">Warning</p>
-    <div id="sqlitepopup" class="w3-pale-yellow popuptext">This instance of ${name} uses an SQLite database engine. This could result in a
-        slow response when load is high. The use of a PostgreSQL database is recommended.</div>
+    % if engine_name != 'postgresql':
+    <p class="w3-red w3-padding pointer w3-right" onclick="popup(this,'sqlitepopup')"><b>Warning</b></p>
+    <div id="sqlitepopup" class="w3-pale-yellow popuptext">WARNING: this instance of ${name} is not using the recommented PostgreSQL database configuration.<br/>
+    This can result in reduced efficiency and some functionalities may be missing or not properly working.<br />
+    The use of PostgreSQL is strongly recommended. More info on how to setup it at <a href="https://github.com/aesuli/ics#db-configuration">https://github.com/aesuli/ics</a></div>
     % endif
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -2,13 +2,16 @@
 
 
  <%block name="head" />
 *** ${name} ***
 <%block name="menu" /> <%block name="menu2" />   ${self.body()}
 Version ${version} - © 2022-2023 Andrea_Esuli Cookie info: this website uses
 only one session cookie to manage login.
-% if engine_name == 'sqlite':
+% if engine_name != 'postgresql':
 Warning
-This instance of ${name} uses an SQLite database engine. This could result in a
-slow response when load is high. The use of a PostgreSQL database is
-recommended.
+WARNING: this instance of ${name} is not using the recommented PostgreSQL
+database configuration.
+This can result in reduced efficiency and some functionalities may be missing
+or not properly working.
+The use of PostgreSQL is strongly recommended. More info on how to setup it at
+https://github.com/aesuli/ics
 % endif
```

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/basewithmenu.html` & `ics-pkg-0.2.0/ics/apps/media/template/basewithmenu.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/browseandcode.html` & `ics-pkg-0.2.0/ics/apps/media/template/browseandcode.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/classification_view.html` & `ics-pkg-0.2.0/ics/apps/media/template/classification_view.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/classifiers.html` & `ics-pkg-0.2.0/ics/apps/media/template/classifiers.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/classify.html` & `ics-pkg-0.2.0/ics/apps/media/template/classify.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/datasets.html` & `ics-pkg-0.2.0/ics/apps/media/template/datasets.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/ips.html` & `ics-pkg-0.2.0/ics/apps/media/template/ips.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/jobs.html` & `ics-pkg-0.2.0/ics/apps/media/template/jobs.html`

 * *Files 2% similar despite different names*

```diff
@@ -158,20 +158,14 @@
         })
         .fail(function(errMsg) {
             document.getElementById('delete_all_job_done_button').style.display='block';
             document.getElementById('delete_all_job_done_button_wait').style.display='none';
             custom_error(errMsg.responseText);
         });
         return false;
-        if(!confirm('Please confirm the DELETE request, proceed?'))
-            return;
-        $.ajax({
-            type:'POST',
-            url:'${jobs_path}/delete_all_done'})
-        .done(update);
     };
 
     function delete_all_jobs() {
         document.getElementById('delete_all_job_button').style.display='none';
         document.getElementById('delete_all_job_button_wait').style.display='block';
         $.ajax({
             type:'POST',
@@ -184,20 +178,14 @@
         })
         .fail(function(errMsg) {
             document.getElementById('delete_all_job_button').style.display='block';
             document.getElementById('delete_all_job_button_wait').style.display='none';
             custom_error(errMsg.responseText);
         });
         return false;
-        if(!confirm('Please confirm the DELETE request, proceed?'))
-            return;
-        $.ajax({
-            type:'POST',
-            url:'${jobs_path}/delete_all'})
-        .done(update);
     };
 
     function delete_job() {
         document.getElementById('delete_job_button').style.display='none';
         document.getElementById('delete_job_button_wait').style.display='block';
         var job = $("#del\\_from").val();
         $.ajax({
```

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/keys.html` & `ics-pkg-0.2.0/ics/apps/media/template/keys.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/locks.html` & `ics-pkg-0.2.0/ics/apps/media/template/locks.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/login.html` & `ics-pkg-0.2.0/ics/apps/media/template/login.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/public_api.html` & `ics-pkg-0.2.0/ics/apps/media/template/public_api.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/public_typeandcode.html` & `ics-pkg-0.2.0/ics/apps/media/template/public_typeandcode.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/training_data_view.html` & `ics-pkg-0.2.0/ics/apps/media/template/training_data_view.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/typeandcode.html` & `ics-pkg-0.2.0/ics/apps/media/template/typeandcode.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/media/template/users.html` & `ics-pkg-0.2.0/ics/apps/media/template/users.html`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/web_admin.py` & `ics-pkg-0.2.0/ics/apps/web_admin.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/web_app.py` & `ics-pkg-0.2.0/ics/apps/web_app.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/apps/web_public.py` & `ics-pkg-0.2.0/ics/apps/web_public.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/classifier/analyzer.py` & `ics-pkg-0.2.0/ics/classifier/analyzer.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/classifier/classifier.py` & `ics-pkg-0.2.0/ics/classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/classifier/lri.py` & `ics-pkg-0.2.0/ics/classifier/lri.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/classifier/lri_online_classifier.py` & `ics-pkg-0.2.0/ics/classifier/lri_online_classifier.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/client/client_session.py` & `ics-pkg-0.2.0/ics/client/client_session.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/db/sqlalchemydb.py` & `ics-pkg-0.2.0/ics/db/sqlalchemydb.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,14 +342,23 @@
     def __init__(self, db_connection_string: str, poolclass=None):
         self._engine = create_engine(db_connection_string, poolclass=poolclass)
         Base.metadata.create_all(self._engine)
         self._sessionmaker = scoped_session(sessionmaker(bind=self._engine))
         configure_mappers()
         self._preload_data()
 
+    @classmethod
+    def test_connection(cls, db_connection_string):
+        engine = create_engine(db_connection_string)
+        try:
+            with engine.connect():
+                return True
+        except OperationalError:
+            return False
+
     def engine_name(self):
         return self._engine.name
 
     def _preload_data(self):
         with self.session_scope() as session:
             if not session.query(
                     exists().where(User.name == _ADMIN_NAME)).scalar():
```

### Comparing `ics-pkg-0.1.9/ics/scripts/cli.py` & `ics-pkg-0.2.0/ics/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/scripts/list_exposed_methods.py` & `ics-pkg-0.2.0/ics/scripts/list_exposed_methods.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/scripts/twitter_uploader.py` & `ics-pkg-0.2.0/ics/scripts/twitter_uploader.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,26 +40,26 @@
     args = parser.parse_args(sys.argv[1:])
 
     try:
         with open(args.bearer_filename, mode='rt', encoding='utf-8') as input_file:
             bearer = input_file.readline().strip()
     except:
         print(f'Cannot load the bearer token from {args.bearer_filename}')
-        exit(-1)
+        sys.exit(-1)
 
     client = ClientSession(args.protocol, args.host, args.port, dataset_path=args.dataset_path,
                            user_auth_path=args.user_auth_path)
 
     print(f'Logging into {args.protocol}://{args.host}:{args.port}{args.user_auth_path}')
     username = input('Username: ').strip()
     try:
         client.login(username, getpass.getpass('Password: '))
     except Exception as e:
         print(f'Login failed: {e.args[0]}')
-        exit(-1)
+        sys.exit(-1)
 
     twigetcli = TwiGetCLIBase(bearer)
 
     twigetcli._twiget.add_callback('uploader', create_uploader(client))
 
     twigetcli.cmdloop()
```

### Comparing `ics-pkg-0.1.9/ics/scripts/webapp.py` & `ics-pkg-0.2.0/ics/scripts/webapp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
+import multiprocessing
 import os
 import sys
 from logging import handlers
 from tempfile import TemporaryDirectory
 
 import cherrypy
 from cherrypy.process.plugins import SignalHandler
 from configargparse import ArgParser
-from sqlalchemy.exc import OperationalError
+from sqlalchemy.exc import OperationalError, ArgumentError, NoSuchModuleError
 
+import ics
 from ics.apps import WebAdmin
 from ics.apps import WebApp
 from ics.apps import WebPublic
 from ics.db.sqlalchemydb import SQLAlchemyDB
 from ics.services import BackgroundProcessor
 from ics.services import ClassifierCollectionService
 from ics.services import DatasetCollectionService
@@ -25,38 +27,44 @@
 from ics.services.background_processor_service import setup_background_processor_log
 from ics.services.user_controller_service import logged_in, name_is
 from ics.util.util import str_to_bool
 
 __author__ = 'Andrea Esuli'
 
 
-def setup_log(access_filename, app_filename):
+def setup_log(access_filename, app_filename, environment):
     path = os.path.dirname(access_filename)
     os.makedirs(path, exist_ok=True)
     path = os.path.dirname(app_filename)
     os.makedirs(path, exist_ok=True)
 
-    cherrypy.config.update({  # 'environment': 'production',
+    cherrypy.config.update({
+        'environment': environment,
         'log.error_file': '',
         'log.access_file': ''})
 
     error_handler = handlers.TimedRotatingFileHandler(app_filename + '.log', when='midnight')
     error_handler.setLevel(logging.DEBUG)
     cherrypy.log.error_log.addHandler(error_handler)
 
     access_handler = handlers.TimedRotatingFileHandler(access_filename + '.log', when='midnight')
     access_handler.setLevel(logging.DEBUG)
     cherrypy.log.access_log.addHandler(access_handler)
 
 
+CONNECT_SQLITE_DB = 'sqlite:///ics.sqlite'
+CONNECT_PGSQL_DB = 'postgresql://ics:ics@localhost:5432/ics'
+
+
 def main():
+    multiprocessing.freeze_support()
     parser = ArgParser()
     parser.add_argument('-c', '--config', help='read configuration from a file', is_config_file=True)
     parser.add_argument('-s', '--save', help='saves configuration to a file', is_write_out_config_file_arg=True)
-    parser.add_argument('--db_connection_string', type=str, default='postgresql://ics:ics@localhost:5432/ics')
+    parser.add_argument('--db_connection_string', type=str, default=CONNECT_SQLITE_DB)
     parser.add_argument('--log_dir', help='local directory for log files', type=str, default=None)
     parser.add_argument('--data_dir', help='local directory where uploaded/downloaded file are placed', type=str,
                         default=None)
     parser.add_argument('--name', help='name to show in the client app', type=str,
                         default='ICS - Interactive Classification System')
     parser.add_argument('--host', help='host server address', type=str, default='127.0.0.1')
     parser.add_argument('--port', help='host server port', type=int, default=8080)
@@ -76,24 +84,50 @@
     parser.add_argument('--classifier_path', help='server path of the classifier web service', type=str,
                         default='/service/classifiers/')
     parser.add_argument('--dataset_path', help='server path of the dataset web service', type=str,
                         default='/service/datasets/')
     parser.add_argument('--jobs_path', help='server path of the jobs web service', type=str,
                         default='/service/jobs/')
     parser.add_argument('--min_password_length', help='minimum password length', type=int, default=8)
+    parser.add_argument('--devel', help='use it to get more log info', action='store_true')
+    parser.add_argument('--version', help='prints the version and exits', action='store_true')
     args = parser.parse_args(sys.argv[1:])
 
+    if args.version:
+        print(f'{ics.__version__}')
+        return 0
+
+    print(f'Starting {args.name} {ics.__version__} with the following configuration:')
+    print(' '.join([f'--{key} {value}' for key, value in args.__dict__.items()]))
+
+    if args.db_connection_string != CONNECT_PGSQL_DB:
+        print()
+        print(f'WARNING: this instance of {args.name} is not using the recommended PostgreSQL database configuration.')
+        print(f'This can result in reduced efficiency and some functionalities may be missing or not properly working.')
+        print(
+            f'The use of PostgreSQL is recommended, e.g., --db_connection_string postgresql://ics:ics@localhost:5432/ics.')
+        print(f'More info on how to setup it at https://github.com/aesuli/ics#db-configuration')
+
+    print()
+    print(f'Serving on http://{args.host}:{args.port}', flush=True)
+
+    if args.devel:
+        environment = None
+    else:
+        environment = 'production'
+
     try:
         with TemporaryDirectory(dir=args.data_dir, prefix='ics-data_') as data_dir, \
                 TemporaryDirectory(dir=args.log_dir, prefix='ics-log_') as log_dir, \
-                SQLAlchemyDB(args.db_connection_string) as db,  \
+                SQLAlchemyDB(args.db_connection_string) as db, \
                 BackgroundProcessor(args.db_connection_string, os.cpu_count() - 2,
                                     initializer=setup_background_processor_log,
                                     initargs=(os.path.join(log_dir, 'bpaccess'),
-                                              os.path.join(log_dir, 'bpapp'))) as background_processor, \
+                                              os.path.join(log_dir, 'bpapp'),
+                                              environment)) as background_processor, \
                 WebApp(db, args.user_auth_path, args.admin_app_path,
                        args.classifier_path, args.dataset_path, args.jobs_path, args.name,
                        args.public_app_path) as main_app, \
                 WebPublic(db, args.ip_auth_path, args.key_auth_path,
                           args.classifier_path, args.name, args.main_app_path) as public_app, \
                 WebAdmin(db, args.main_app_path, args.user_auth_path,
                          args.ip_auth_path, args.key_auth_path, args.classifier_path, args.dataset_path, args.jobs_path,
@@ -101,15 +135,15 @@
                 ClassifierCollectionService(db, data_dir) as classifier_service, \
                 DatasetCollectionService(db, data_dir) as dataset_service, \
                 JobsService(db) as jobs_service, \
                 UserControllerService(db, args.min_password_length) as user_auth_controller, \
                 IPControllerService(db, args.ip_hourly_limit, args.ip_request_limit,
                                     args.allow_unknown_ips) as ip_auth_controller, \
                 KeyControllerService(db) as key_auth_controller:
-            setup_log(os.path.join(log_dir, 'access'), os.path.join(log_dir, 'app'))
+            setup_log(os.path.join(log_dir, 'access'), os.path.join(log_dir, 'app'), environment)
 
             background_processor.start()
 
             cherrypy.server.socket_host = args.host
             cherrypy.server.socket_port = args.port
 
             enable_controller_service()
@@ -225,17 +259,19 @@
                 for handler in handler_list.handlers[:]:
                     if hasattr(handler, "close"):
                         handler.close()
                     elif hasattr(handler, "flush"):
                         handler.flush()
                     handler_list.removeHandler(handler)
 
-    except OperationalError as oe:
+    except (OperationalError, ArgumentError, NoSuchModuleError) as e:
         print('Database error')
-        print(oe)
+        print(e)
+        print()
+        print('Have you set up a database following the instructions? See https://github.com/aesuli/ics#db-configuration')
         return -1
 
     return 0
 
 
 if __name__ == "__main__":
-    exit(main())
+    sys.exit(main())
```

### Comparing `ics-pkg-0.1.9/ics/services/auth_controller_service.py` & `ics-pkg-0.2.0/ics/services/auth_controller_service.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/services/background_processor_service.py` & `ics-pkg-0.2.0/ics/services/background_processor_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,32 +17,33 @@
 from ics.db.sqlalchemydb import SQLAlchemyDB, Job
 
 __author__ = 'Andrea Esuli'
 
 LOOP_WAIT = 0.1
 
 
-def setup_background_processor_log(access_filename, app_filename):
+def setup_background_processor_log(access_filename, app_filename, environment):
     path = os.path.dirname(access_filename)
     os.makedirs(path, exist_ok=True)
     path = os.path.dirname(app_filename)
     os.makedirs(path, exist_ok=True)
 
-    cherrypy.config.update({  # 'environment': 'production',
+    cherrypy.config.update({
+        'environment': environment,
         'log.error_file': '',
         'log.access_file': ''})
 
     process = multiprocessing.current_process()
 
-    error_handler = handlers.TimedRotatingFileHandler(app_filename + '-' + str(process.name) + '.log',
+    error_handler = handlers.TimedRotatingFileHandler(f'{app_filename}-{process.name.replace(":","_")}.log',
                                                       when='midnight')
     error_handler.setLevel(logging.DEBUG)
     cherrypy.log.error_log.addHandler(error_handler)
 
-    access_handler = handlers.TimedRotatingFileHandler(access_filename + '-' + str(process.name) + '.log',
+    access_handler = handlers.TimedRotatingFileHandler(f'{access_filename}-{process.name.replace(":","_")}.log',
                                                        when='midnight')
     access_handler.setLevel(logging.DEBUG)
     cherrypy.log.access_log.addHandler(access_handler)
 
 
 class JobError:
     def __init__(self, exception, msg, tb):
@@ -77,38 +78,40 @@
                 return JobError(e, "FAILED", tb)
         except Exception as e:
             tb = traceback.format_exc()
             return JobError(e, "UNMANAGED", tb)
 
 
 def bp_pool_initializer(db_connection_string, initializer, *initargs):
+    if initializer is not None:
+        initializer(*initargs)
     cherrypy.log(f'BackgroundProcessor: adding {multiprocessing.current_process().name} to pool', severity=logging.INFO)
     global process_db
     process_db = SQLAlchemyDB(db_connection_string, NullPool)
     signal.signal(signal.SIGINT, signal.SIG_IGN)
-    if initializer is not None:
-        initializer(*initargs)
 
 
 class BackgroundProcessor(Process):
     def __init__(self, db_connection_string, pool_size, initializer=None, initargs=None):
         Process.__init__(self)
         self._stop_event = multiprocessing.Event()
         self._pool_size = pool_size
         self._db_connection_string = db_connection_string
-        self._initializer = partial(bp_pool_initializer, db_connection_string, initializer)
+        self._initializer = initializer
+        self._pool_initializer = partial(bp_pool_initializer, db_connection_string, initializer)
         if initargs is None:
             initargs = []
         self._initargs = initargs
         self._running = False
         self._semaphore = BoundedSemaphore(self._pool_size)
 
     def run(self):
+        self._initializer(*self._initargs)
         with SQLAlchemyDB(self._db_connection_string) as db, \
-                Pool(processes=self._pool_size, initializer=self._initializer, initargs=self._initargs) as pool:
+                Pool(processes=self._pool_size, initializer=self._pool_initializer, initargs=self._initargs) as pool:
             cherrypy.log('BackgroundProcessor: started', severity=logging.INFO)
             while not self._stop_event.is_set():
                 try:
                     job = db.get_next_pending_job()
                 except InvalidRequestError as ire:
                     cherrypy.log(
                         f'Error fetching next job \nException: {ire}',
```

### Comparing `ics-pkg-0.1.9/ics/services/classifier_collection_service.py` & `ics-pkg-0.2.0/ics/services/classifier_collection_service.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/services/dataset_collection_service.py` & `ics-pkg-0.2.0/ics/services/dataset_collection_service.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/services/ip_controller_service.py` & `ics-pkg-0.2.0/ics/services/ip_controller_service.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/services/jobs_service.py` & `ics-pkg-0.2.0/ics/services/jobs_service.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/services/key_controller_service.py` & `ics-pkg-0.2.0/ics/services/key_controller_service.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/services/user_controller_service.py` & `ics-pkg-0.2.0/ics/services/user_controller_service.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics/util/util.py` & `ics-pkg-0.2.0/ics/util/util.py`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/ics_pkg.egg-info/PKG-INFO` & `ics-pkg-0.2.0/ics_pkg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ics-pkg
-Version: 0.1.9
+Version: 0.2.0
 Summary: Interactive Classification System (ICS): a tool for machine learning-supported labeling of text
 Home-page: https://github.com/aesuli/ics
 Author: Andrea Esuli
 Author-email: andrea@esuli.it
 License: BSD
 Project-URL: Bug Reports, https://github.com/aesuli/ics/issues
 Project-URL: Source, https://github.com/aesuli/ics/
@@ -52,38 +52,55 @@
 
 [A. Esuli, "ICS: Total Freedom in Manual Text Classification Supported by Unobtrusive Machine Learning," in IEEE Access, vol. 10, pp. 64741-64760, 2022, doi: 10.1109/ACCESS.2022.3184009](https://doi.org/10.1109/ACCESS.2022.3184009)
 
 ## <a name="installation"></a> Installation
 
 You can have a working installation of ICS in many ways:
 
+- [Single file executable](#single-file-executable) (to start using ICS)
 - [Docker](#docker) (for a single user)
-- [Docker compose](#docker-compose) (recommended for most cases)
+- [Docker compose](#docker-compose) (for larger installation)
 - [Pip install](#pip)
 - [From source](#from-source)
 
+### Single file executable
+
+Executable files of ICS are downloadable from the [releases page](https://github.com/aesuli/ics/releases).
+Once downloaded it can be run and have a working instance of ICS, provided a [database is configured](#db-configuration).
+
+```shell
+ics-webapp
+```
+
+
+The executable are from source using [pyinstaller](https://pyinstaller.org/):
+
+```shell
+pyinstaller -F ics\scripts\webapp.py --add-data="ics\apps\media;ics\apps\media" --collect-all sklearn --name ics-webapp
+```
+
 ### Docker
 
 A quick way have a running instance of ICS is to use [Docker](https://docker.com).
 
 ```shell
-docker run -p 8080:8080 andreaesuli/ics
+docker run -p 8080:8080 ghcr.io/aesuli/ics
 ```
 
 This command pulls the ICS image from Docker hub and runs it, publishing the application on port 8080 of the host machine, accessible from any interface.
 Once started ICS is accessible from the host machine using a browser at the address [http://127.0.0.1:8080](http://127.0.0.1:8080)
 
 To have ICS accessible only from the local host machine add local ip address:
 
 ```shell
-docker run -p 127.0.0.1:8080:8080 andreaesuli/ics
+docker run -p 127.0.0.1:8080:8080 ghcr.io/aesuli/ics
 ```
 
-__NOTE:__ by default the ICS image uses the SQLite database engine, which can results in performance drops caused by the access to DB, specially when multiple users access the system.
-A configuration using PostgreSQL is recommended. It can be easily set up using docker compose.
+__NOTE:__ by default the ICS image uses the SQLite database engine, which may result in reduced efficiency and functionalities.
+A configuration using PostgreSQL is strongly recommended. It can be easily set up using docker compose.
 
 #### Data persistence
 
 ICS image use volumes to keep information persistent:
 - ics-db stores the sqlite file, this is the only volume that should be saved to keep the state of the application.
 - ics-data stores the files that are uploaded or downloaded from the system. It is defined for inspection in case of failures, it is not necessary to save it.
 - ics-log stores the log files. It is defined for inspection in case of failures, it is not necessary to save it.
@@ -123,15 +140,15 @@
 On Linux/Mac:
 ```shell
 DB_DATA=/var/lib/ics/data docker compose up
 ```
 
 ### Pip
 
-The suggested way to quickly set up the python enviroment is to use
+The suggested way to quickly set up the python environment is to use
 the [Anaconda/Miniconda distribution](https://www.anaconda.com/products/distribution) and the `conda` package manager to
 create the virtual enviroment.
 
 ```shell
 conda create -n ics python
 conda activate ics
 ````
@@ -156,46 +173,55 @@
 pip install -r requirements.txt
 ```
 
 The last required step is to [configure a database](#db-configuration).
 
 ### DB configuration
 
-Docker installation already includes the setup of the DB, so you can skip this section.
-If you installed ICS using pip or the source code you must set up a DB.
+The Docker compose installation already includes the setup of the PostgreSQL database, so you can skip this section.
+Any another requires to have a database available to connect to.
+The use of [PostgreSQL](https://www.postgresql.org/) is strongly recommended.
 
-The use of [PostgreSQL](https://www.postgresql.org/) is recommended to avoid performance drops caused by the access to 
-DB, specially when multiple users access the system.
-Howerever, ICS can also work using other DB engines, such as [SQLite](https://www.sqlite.org/).
+#### PostgreSQL
 
-#### SQLite
+To connect to PostgreSQL, a dedicated DB must be created.
+These are the SQL commands to create the required user and database on PostgreSQL.
+
+```
+CREATE USER ics WITH PASSWORD 'ics';
+CREATE DATABASE ics;
+GRANT ALL PRIVILEGES ON DATABASE ics to ics;
+```
+
+These commands can be issued using the `psql` SQL shell (or using pgAdmin, or similar db frontends).
+The tables required by ICS are created automatically at the first run.
 
-Running ICS using SQLite as the DB only require to pass a ``--db_connection_string`` argument to the launch script:
+Then ICS can be launched passing the DB connection string:
 
 ```shell
-ics-webapp --db_connection_string sqlite:///ics.sqlite
+ics-webapp --db_connection_string postgresql://ics:ics@localhost:5432/ics
 ```
 
-SQLite is
+The above connection string is the correct one for a locally running database, change it according to your configuration.
 
-#### PostgreSQL
+#### SQLite
 
-By default ICS assumes to connect to PostgreSQL, using a database named 'ics' and a user named 'ics' (with password 'ics').
+By default ICS uses SQLite as the DB, yet please note that **the use of SQLite is intended only for a first exploration of ICS and that using PostgreSQL is strongly recommended**.
+Using SQLite can result in reduced efficiency and some functionalities may be missing or not properly working.
 
-These are the SQL commands to create the required user and database on PostgreSQL.
+To use SQLite use the following ``--db_connection_string`` argument to the launch script:
 
-```
-CREATE USER ics WITH PASSWORD 'ics';
-CREATE DATABASE ics;
-GRANT ALL PRIVILEGES ON DATABASE ics to ics;
+```shell
+ics-webapp --db_connection_string sqlite:///ics.sqlite
 ```
 
-These command can be issued using the `psql` SQL shell (or using pgAdmin, or similar db frontends).
+This is the default connection string, it creates the DB file in the current working directory.
+Change it to point to the path where you want to store your file.
 
-The tables required by ICS are created automatically at the first run.
+Again, PostgreSQL is the recommended database.
 
 ## <a name="startmain"></a> The main app
 
 Running the docker image automatically starts the main application, which can be accessed with a browser at the ip and 
 port defined with the docker launch command or docker compose file.
 Installations that do not use docker can run ics by using the ics-webapp script.
```

### Comparing `ics-pkg-0.1.9/ics_pkg.egg-info/SOURCES.txt` & `ics-pkg-0.2.0/ics_pkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ics-pkg-0.1.9/setup.py` & `ics-pkg-0.2.0/setup.py`

 * *Files identical despite different names*

