# Comparing `tmp/WPP_Whatsapp-0.1.0.tar.gz` & `tmp/WPP_Whatsapp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPP_Whatsapp-0.1.0.tar", last modified: Sun Jul  2 14:52:47 2023, max compression
+gzip compressed data, was "WPP_Whatsapp-0.1.1.tar", last modified: Tue Jul  4 10:18:42 2023, max compression
```

## Comparing `WPP_Whatsapp-0.1.0.tar` & `WPP_Whatsapp-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.632437 WPP_Whatsapp-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-02 14:52:47.632437 WPP_Whatsapp-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.620437 WPP_Whatsapp-0.1.0/WPP_Whatsapp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.620437 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.620437 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)    21892 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.624436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.624436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/Whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.624436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/jsFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/scrap-img.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.628436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/BusinessLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/CatalogLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ControlsLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/GroupLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/HostLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/LabelsLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ListenerLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ProfileLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/RetrieverLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/SenderLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/StatusLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/UILayer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.628436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/model/status_find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.628436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 14:52:47.632437 WPP_Whatsapp-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/Whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/jsFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/scrap-img.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/BusinessLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/CatalogLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ControlsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/GroupLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20711 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/HostLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/LabelsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ListenerLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ProfileLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/RetrieverLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/SenderLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/StatusLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/UILayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/model/status_find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/setup.py
```

### Comparing `WPP_Whatsapp-0.1.0/PKG-INFO` & `WPP_Whatsapp-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.1.0
+Version: 0.1.1
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
+License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # WPP_Whatsapp
 <p align="center">
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/WPP-Whatsapp.svg?maxAge=86400" /></a>
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/WPP-Whatsapp.svg?maxAge=86400" /></a>
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://static.pepy.tech/personalized-badge/WPP-Whatsapp?period=total&units=international_system&left_color=gray&left_text=Downloads" /></a>
+  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/WPP_Whatsapp.svg?maxAge=86400" /></a>
+  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://static.pepy.tech/personalized-badge/WPP_Whatsapp?period=total&units=international_system&left_color=gray&left_text=Downloads" /></a>
 </p>
 
 WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of
 any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many
 other things, use your imagination         
 WPP_Whatsapp > [WPPConnect](https://github.com/wppconnect-team/wppconnect) Converted to python, so Documentation is same
```

### Comparing `WPP_Whatsapp-0.1.0/README.md` & `WPP_Whatsapp-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # WPP_Whatsapp
 <p align="center">
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/WPP-Whatsapp.svg?maxAge=86400" /></a>
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/WPP-Whatsapp.svg?maxAge=86400" /></a>
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://static.pepy.tech/personalized-badge/WPP-Whatsapp?period=total&units=international_system&left_color=gray&left_text=Downloads" /></a>
+  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/WPP_Whatsapp.svg?maxAge=86400" /></a>
+  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://static.pepy.tech/personalized-badge/WPP_Whatsapp?period=total&units=international_system&left_color=gray&left_text=Downloads" /></a>
 </p>
 
 WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of
 any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many
 other things, use your imagination         
 WPP_Whatsapp > [WPPConnect](https://github.com/wppconnect-team/wppconnect) Converted to python, so Documentation is same
```

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,16 +309,19 @@
             await self.browser.close()
 
         # NOTE: this hangs without the proper child watcher
         if hasattr(self, "playwright"):
             await self.playwright.stop()
 
     def stop(self) -> None:
-        self.loop.call_soon_threadsafe(self.loop.stop)
-        self.thread.join()
+        try:
+            self.loop.call_soon_threadsafe(self.loop.stop)
+            self.thread.join()
+        except Exception as error:
+            print(error)
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.stop()
```

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/PKG-INFO` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: WPP-Whatsapp
-Version: 0.1.0
+Version: 0.1.1
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
+License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # WPP_Whatsapp
 <p align="center">
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/WPP-Whatsapp.svg?maxAge=86400" /></a>
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/WPP-Whatsapp.svg?maxAge=86400" /></a>
-  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://static.pepy.tech/personalized-badge/WPP-Whatsapp?period=total&units=international_system&left_color=gray&left_text=Downloads" /></a>
+  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/WPP_Whatsapp.svg?maxAge=86400" /></a>
+  <a href="https://pypi.org/project/WPP-Whatsapp"><img alt="Python Versions" src="https://static.pepy.tech/personalized-badge/WPP_Whatsapp?period=total&units=international_system&left_color=gray&left_text=Downloads" /></a>
 </p>
 
 WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of
 any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many
 other things, use your imagination         
 WPP_Whatsapp > [WPPConnect](https://github.com/wppconnect-team/wppconnect) Converted to python, so Documentation is same
```

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/SOURCES.txt` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+LICENSE
 README.md
 setup.py
+WPP_Whatsapp/__init__.py
+WPP_Whatsapp.egg-info/PKG-INFO
+WPP_Whatsapp.egg-info/SOURCES.txt
+WPP_Whatsapp.egg-info/dependency_links.txt
+WPP_Whatsapp.egg-info/requires.txt
+WPP_Whatsapp.egg-info/top_level.txt
 WPP_Whatsapp/PlaywrightSafeThread/__init__.py
 WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
 WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
 WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
-WPP_Whatsapp/WPP_Whatsapp.egg-info/PKG-INFO
-WPP_Whatsapp/WPP_Whatsapp.egg-info/SOURCES.txt
-WPP_Whatsapp/WPP_Whatsapp.egg-info/dependency_links.txt
-WPP_Whatsapp/WPP_Whatsapp.egg-info/requires.txt
-WPP_Whatsapp/WPP_Whatsapp.egg-info/top_level.txt
 WPP_Whatsapp/api/Whatsapp.py
 WPP_Whatsapp/api/__init__.py
 WPP_Whatsapp/api/const.py
 WPP_Whatsapp/api/helpers/__init__.py
 WPP_Whatsapp/api/helpers/decorators.py
 WPP_Whatsapp/api/helpers/function.py
 WPP_Whatsapp/api/helpers/jsFunction.py
```

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/Whatsapp.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/Whatsapp.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/const.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/const.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/decorators.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/jsFunction.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/jsFunction.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ControlsLayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ControlsLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/GroupLayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/GroupLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/HostLayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/HostLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,9 +518,8 @@
     def valid_chatId(chatId):
         chatId = chatId.replace("+", "")
         if chatId and (not chatId.endswith('@c.us') and not chatId.endswith('@g.us')):
             chatId += '@g.us' if len(chatId) > 15 else '@c.us'
         return chatId
 
     def close(self):
-        if not self.page.is_closed():
-            self.ThreadsafeBrowser.sync_close()
+        self.ThreadsafeBrowser.sync_close()
```

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/LabelsLayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/LabelsLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ListenerLayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ListenerLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ProfileLayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ProfileLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/RetrieverLayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/RetrieverLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/SenderLayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/SenderLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/UILayer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/UILayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/model/status_find.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/model/status_find.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/browser.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/browser.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/initializer.py` & `WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/initializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,23 @@
 
     def __init__(
             self, session: str, user_data_dir='', folderNameToken="",
             catchQR: types.FunctionType = None,
             statusFind: types.FunctionType = None, onLoadingScreen: types.FunctionType = None,
             onStateChange: types.FunctionType = None, waitForLogin: bool = True, logQR: bool = False,
             autoClose: int = 0, *args, **kwargs) -> None:
-
+        """
+        class Create:
+            custom class to open browser and start whatsapp
+            you can custom your class, you need only:
+                ThreadsafeBrowser = ThreadsafeBrowser(browser="chromium")
+                client = Whatsapp(session="test", ThreadsafeBrowser)
+                client.start()
+                client.waitForLogin()
+        """
         self.browserSessionToken = None
         self.waitLoginPromise = None
         self.client = None
         self.state = "CLOSED"
         self.statusFind_dict = {}
         self.catchQR_dict = {}
         self.session = session
@@ -48,18 +56,24 @@
         self.onStateChange = onStateChange if type(onStateChange) == types.FunctionType else None
         self.logger = Logger
         self.waitForLogin = waitForLogin
         self.logQR = logQR
         self.autoClose = autoClose
         self.__kwargs = kwargs
 
-    def close(self):
-        if self.client:
-            self.client.close()
-            self.state = "CLOSED"
+    def __exit__(self, *args):
+        self.sync_close()
+
+    async def close(self):
+        await self.ThreadsafeBrowser.close()
+        self.state = "CLOSED"
+
+    def sync_close(self):
+        self.ThreadsafeBrowser.sync_close()
+        self.state = "CLOSED"
 
     def _onStateChange(self, state):
         if type(self.onStateChange) == types.FunctionType:
             self.onStateChange(state)
         self.state = state
         connected = self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.isRegistered()")
         if not connected:
@@ -111,22 +125,24 @@
         default = {"channel": "chrome", "no_viewport": True, "bypass_csp": True, "headless": False}
         for key in default:
             if key not in self.__kwargs:
                 self.__kwargs[key] = default[key]
 
         self.ThreadsafeBrowser = ThreadsafeBrowser(
             browser="chromium", install=False, user_data_dir=self.user_data_dir, **self.__kwargs)
+
+        self.ThreadsafeBrowser.page.on("close", self.close)
+        self.ThreadsafeBrowser.page.on("crash", self.close)
         self.ThreadsafeBrowser.browser.on("disconnected", lambda: self.statusFind('browserClose', self.session))
 
         self.client = Whatsapp(self.session, self.ThreadsafeBrowser, logQR=self.logQR,
                                autoClose=self.autoClose)
         self.client.catchQR = self.catchQR
         self.client.statusFind = self.statusFind
         self.client.onLoadingScreen = self.onLoadingScreen
-
         self.client.start()
 
         if self.waitForLogin:
             is_logged = self.client.waitForLogin()
             if not is_logged:
                 raise Exception('Not Logged')
             self.state = "CONNECTED"
```

### Comparing `WPP_Whatsapp-0.1.0/setup.py` & `WPP_Whatsapp-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = "WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination"
 
-version = "0.1.0"
+version = "0.1.1"
 
 setup(
     name="WPP_Whatsapp",
     version=version,
-    # license="MIT License",
+    license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
     description=description,
-    packages=find_packages("WPP_Whatsapp"),
-    package_dir={"": "WPP_Whatsapp"},
+    packages=find_packages("."),
     url="https://github.com/3mora2/WPP_Whatsapp",
     project_urls={"Bug Report": "https://github.com/3mora2/WPP_Whatsapp/issues/new"},
     install_requires=[
         "event-emitter-js",
         "greenlet",
         "playwright",
         "Pillow",
@@ -28,14 +27,14 @@
         'typing_extensions',
         "playwright-stealth"
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["WPP_Whatsapp"],
     classifiers=[
-        # "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
 
     ],
 )
```

