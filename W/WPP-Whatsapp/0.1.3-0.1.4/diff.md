# Comparing `tmp/WPP_Whatsapp-0.1.3.tar.gz` & `tmp/WPP_Whatsapp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPP_Whatsapp-0.1.3.tar", last modified: Tue Jul  4 12:23:51 2023, max compression
+gzip compressed data, was "WPP_Whatsapp-0.1.4.tar", last modified: Tue Jul  4 18:33:17 2023, max compression
```

## Comparing `WPP_Whatsapp-0.1.3.tar` & `WPP_Whatsapp-0.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.488743 WPP_Whatsapp-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 12:23:51.488743 WPP_Whatsapp-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.480743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.480743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.480743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/_future_/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/_future_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/_future_/threaded_child_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.480743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/browser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.480743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/Whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.484743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/helpers/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/helpers/jsFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/helpers/scrap-img.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.484743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/BusinessLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/CatalogLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/ControlsLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/GroupLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20986 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/HostLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/LabelsLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/ListenerLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/ProfileLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/RetrieverLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/SenderLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/StatusLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/UILayer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.484743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/model/status_find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.484743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/controllers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/controllers/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/controllers/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.484743 WPP_Whatsapp-0.1.3/WPP_Whatsapp/js_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    88869 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp/js_lib/wapi.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:23:51.488743 WPP_Whatsapp-0.1.3/WPP_Whatsapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 12:23:51.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-04 12:23:51.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:23:51.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 12:23:51.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 12:23:51.000000 WPP_Whatsapp-0.1.3/WPP_Whatsapp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 12:23:51.488743 WPP_Whatsapp-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-04 12:23:39.000000 WPP_Whatsapp-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.431052 WPP_Whatsapp-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 18:33:17.427052 WPP_Whatsapp-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.423052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.423052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.423052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.423052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/future_/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/future_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/future_/threaded_child_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.423052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/Whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.427052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/helpers/jsFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/helpers/scrap-img.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.427052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/BusinessLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/CatalogLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/ControlsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/GroupLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20986 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/HostLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/LabelsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/ListenerLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/ProfileLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/RetrieverLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/SenderLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/StatusLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/UILayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.427052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/model/status_find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.427052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/controllers/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/controllers/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.427052 WPP_Whatsapp-0.1.4/WPP_Whatsapp/js_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    88869 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp/js_lib/wapi.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:33:17.427052 WPP_Whatsapp-0.1.4/WPP_Whatsapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 18:33:17.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-04 18:33:17.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:33:17.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 18:33:17.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 18:33:17.000000 WPP_Whatsapp-0.1.4/WPP_Whatsapp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:33:17.431052 WPP_Whatsapp-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-04 18:33:07.000000 WPP_Whatsapp-0.1.4/setup.py
```

### Comparing `WPP_Whatsapp-0.1.3/LICENSE` & `WPP_Whatsapp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/PKG-INFO` & `WPP_Whatsapp-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.1.3
+Version: 0.1.4
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `WPP_Whatsapp-0.1.3/README.md` & `WPP_Whatsapp-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # from: https://github.com/medialab/minet/blob/master/minet/browser/threadsafe_browser.py
 
 import inspect
 import os
 import typing
-from typing import Callable, Optional, TypeVar, Awaitable, Literal, ParamSpec, Concatenate
+from typing import Literal
 import asyncio
 import platform
 from threading import Thread, Event
 import psutil
 from playwright._impl import _api_types
-from playwright.async_api import async_playwright, Page, Browser, BrowserType
+from playwright.async_api import async_playwright, Browser, BrowserType
 from playwright_stealth import stealth_async
 from WPP_Whatsapp.PlaywrightSafeThread.browser.plawright_shim import run_playwright
 
 UNIX = "windows" not in platform.system().lower()
 LTE_PY37 = platform.python_version_tuple()[:2] <= ("3", "7")
 
 SUPPORTED_BROWSERS = ("chromium", "firefox", "webkit")
-BrowserName = Literal[*SUPPORTED_BROWSERS]
-T = TypeVar("T")
-P = ParamSpec("P")
-PageCallable = Callable[Concatenate[Page, P], Awaitable[T]]
-BrowserCallable = Callable[Concatenate[Browser, P], Awaitable[T]]
+BrowserName = Literal["chromium", "firefox", "webkit"]
 
 
 class ThreadsafeBrowser:
     def __init__(
             self,
             browser: BrowserName = "chromium",
             stealthy: bool = False,
@@ -204,15 +200,15 @@
         """
         if browser not in SUPPORTED_BROWSERS:
             raise TypeError("unsupported browser")
 
         # NOTE: on unix python 3.7, child watching does not
         # work properly when asyncio is not running from the main thread
         if UNIX and LTE_PY37:
-            from WPP_Whatsapp.PlaywrightSafeThread._future_.threaded_child_watcher import ThreadedChildWatcher
+            from WPP_Whatsapp.PlaywrightSafeThread.future_.threaded_child_watcher import ThreadedChildWatcher
             asyncio.set_child_watcher(ThreadedChildWatcher())
 
         self._stealthy = stealthy
         self._browser_name = browser
 
         self._browser_option = {}
         self._browser_persistent_option = {}
```

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/Whatsapp.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/Whatsapp.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/const.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/const.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/helpers/decorators.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/helpers/jsFunction.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/helpers/jsFunction.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/ControlsLayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/ControlsLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/GroupLayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/GroupLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/HostLayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/HostLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/LabelsLayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/LabelsLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/ListenerLayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/ListenerLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/ProfileLayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/ProfileLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/RetrieverLayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/RetrieverLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/SenderLayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/SenderLayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/layers/UILayer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/layers/UILayer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/api/model/status_find.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/api/model/status_find.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/controllers/browser.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/controllers/browser.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/controllers/initializer.py` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/controllers/initializer.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp/js_lib/wapi.js` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp/js_lib/wapi.js`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp.egg-info/PKG-INFO` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPP-Whatsapp
-Version: 0.1.3
+Version: 0.1.4
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `WPP_Whatsapp-0.1.3/WPP_Whatsapp.egg-info/SOURCES.txt` & `WPP_Whatsapp-0.1.4/WPP_Whatsapp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE
 README.md
 setup.py
 ./WPP_Whatsapp/README.md
 ./WPP_Whatsapp/__init__.py
 ./WPP_Whatsapp/PlaywrightSafeThread/__init__.py
-./WPP_Whatsapp/PlaywrightSafeThread/_future_/__init__.py
-./WPP_Whatsapp/PlaywrightSafeThread/_future_/threaded_child_watcher.py
 ./WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
 ./WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
 ./WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
+./WPP_Whatsapp/PlaywrightSafeThread/future_/__init__.py
+./WPP_Whatsapp/PlaywrightSafeThread/future_/threaded_child_watcher.py
 ./WPP_Whatsapp/api/Whatsapp.py
 ./WPP_Whatsapp/api/__init__.py
 ./WPP_Whatsapp/api/const.py
 ./WPP_Whatsapp/api/helpers/__init__.py
 ./WPP_Whatsapp/api/helpers/decorators.py
 ./WPP_Whatsapp/api/helpers/function.py
 ./WPP_Whatsapp/api/helpers/jsFunction.py
```

### Comparing `WPP_Whatsapp-0.1.3/setup.py` & `WPP_Whatsapp-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import os
-from distutils.sysconfig import get_python_inc
 from setuptools import find_packages
 from setuptools import setup
-from setuptools.extension import Extension
+
 
 long_description = open("README.md", encoding="utf-8").read()
 description = "WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination"
 
-incdir = os.path.join('Numerical')
-version = "0.1.3"
+version = "0.1.4"
 
 
 setup(
     name="WPP_Whatsapp",
     version=version,
     license="MIT License",
     author="Ammar Alkotb",
@@ -30,15 +27,14 @@
         "pyee",
         'segno',
         'typing_extensions',
         "playwright-stealth"
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    # py_modules=["WPP_Whatsapp"],
     package_dir={"": "."},
     package_data={"WPP_Whatsapp": ["*/*.js", "*.md"]},
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

