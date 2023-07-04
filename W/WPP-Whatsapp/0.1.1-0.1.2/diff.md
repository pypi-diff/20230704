# Comparing `tmp/WPP_Whatsapp-0.1.1.tar.gz` & `tmp/WPP_Whatsapp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPP_Whatsapp-0.1.1.tar", last modified: Tue Jul  4 10:18:42 2023, max compression
+gzip compressed data, was "WPP_Whatsapp-0.1.2.tar", last modified: Tue Jul  4 10:25:15 2023, max compression
```

## Comparing `WPP_Whatsapp-0.1.1.tar` & `WPP_Whatsapp-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/Whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/jsFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/scrap-img.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/BusinessLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/CatalogLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ControlsLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/GroupLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20711 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/HostLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/LabelsLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ListenerLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ProfileLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/RetrieverLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/SenderLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/StatusLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/UILayer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/model/status_find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:42.553883 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 10:18:42.000000 WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:18:42.557883 WPP_Whatsapp-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 10:18:30.000000 WPP_Whatsapp-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.371503 WPP_Whatsapp-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 10:25:15.371503 WPP_Whatsapp-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.363503 WPP_Whatsapp-0.1.2/WPP_Whatsapp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.363503 WPP_Whatsapp-0.1.2/WPP_Whatsapp/PlaywrightSafeThread/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/PlaywrightSafeThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.367503 WPP_Whatsapp-0.1.2/WPP_Whatsapp/PlaywrightSafeThread/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.367503 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/Whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.367503 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/helpers/jsFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/helpers/scrap-img.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.371503 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/BusinessLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/CatalogLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/ControlsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/GroupLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20711 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/HostLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/LabelsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/ListenerLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/ProfileLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/RetrieverLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/SenderLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/StatusLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/UILayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.371503 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/model/status_find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.371503 WPP_Whatsapp-0.1.2/WPP_Whatsapp/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/controllers/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp/controllers/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:25:15.363503 WPP_Whatsapp-0.1.2/WPP_Whatsapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 10:25:15.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-04 10:25:15.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:25:15.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 10:25:15.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 10:25:15.000000 WPP_Whatsapp-0.1.2/WPP_Whatsapp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:25:15.371503 WPP_Whatsapp-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 10:25:03.000000 WPP_Whatsapp-0.1.2/setup.py
```

### Comparing `WPP_Whatsapp-0.1.1/LICENSE` & `WPP_Whatsapp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/PKG-INFO` & `WPP_Whatsapp-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.1.1
+Version: 0.1.2
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `WPP_Whatsapp-0.1.1/README.md` & `WPP_Whatsapp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/Whatsapp.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/Whatsapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import inspect
 
-from api.layers.HostLayer import HostLayer
+from WPP_Whatsapp.api.layers.HostLayer import HostLayer
 from WPP_Whatsapp.api.const import defaultOptions, Logger
 from WPP_Whatsapp.api.layers.BusinessLayer import BusinessLayer
-from api.layers.ListenerLayer import ListenerLayer
+from WPP_Whatsapp.api.layers.ListenerLayer import ListenerLayer
 
 
 class Whatsapp(BusinessLayer):
     connected = None
 
     def __init__(self, session, threadsafe_browser, *args, **kwargs):
         self.session = session
```

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/const.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/const.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/decorators.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/helpers/jsFunction.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/helpers/jsFunction.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ControlsLayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/ControlsLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/GroupLayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/GroupLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/HostLayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/HostLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/LabelsLayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/LabelsLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ListenerLayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/ListenerLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/ProfileLayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/ProfileLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/RetrieverLayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/RetrieverLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/SenderLayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/SenderLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/layers/UILayer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/layers/UILayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/api/model/status_find.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/api/model/status_find.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/browser.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/controllers/browser.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp/controllers/initializer.py` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp/controllers/initializer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/PKG-INFO` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPP-Whatsapp
-Version: 0.1.1
+Version: 0.1.2
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `WPP_Whatsapp-0.1.1/WPP_Whatsapp.egg-info/SOURCES.txt` & `WPP_Whatsapp-0.1.2/WPP_Whatsapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.1/setup.py` & `WPP_Whatsapp-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = "WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination"
 
-version = "0.1.1"
+version = "0.1.2"
 
 setup(
     name="WPP_Whatsapp",
     version=version,
     license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
```

