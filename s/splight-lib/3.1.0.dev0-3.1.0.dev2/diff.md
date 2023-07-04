# Comparing `tmp/splight-lib-3.1.0.dev0.tar.gz` & `tmp/splight-lib-3.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.1.0.dev0.tar", last modified: Wed Jun 21 13:10:10 2023, max compression
+gzip compressed data, was "splight-lib-3.1.0.dev2.tar", last modified: Tue Jul  4 20:19:06 2023, max compression
```

## Comparing `splight-lib-3.1.0.dev0.tar` & `splight-lib-3.1.0.dev2.tar`

### file list

```diff
@@ -1,98 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.054694 splight-lib-3.1.0.dev2/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.054694 splight-lib-3.1.0.dev2/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.054694 splight-lib-3.1.0.dev2/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.058694 splight-lib-3.1.0.dev2/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.058694 splight-lib-3.1.0.dev2/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.058694 splight-lib-3.1.0.dev2/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.058694 splight-lib-3.1.0.dev2/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/grpc/reflector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/log_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.054694 splight-lib-3.1.0.dev2/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.1.0.dev0/PKG-INFO` & `splight-lib-3.1.0.dev2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.1.0.dev0
+Version: 3.1.0.dev2
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.1.0.dev0/setup.py` & `splight-lib-3.1.0.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.1.0.dev0",
+    version="3.1.0.dev2",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/abstract/client.py` & `splight-lib-3.1.0.dev2/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/auth/mac_auth.py` & `splight-lib-3.1.0.dev2/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/communication/abstract.py` & `splight-lib-3.1.0.dev2/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/communication/remote_client.py` & `splight-lib-3.1.0.dev2/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/database/abstract.py` & `splight-lib-3.1.0.dev2/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/database/builder.py` & `splight-lib-3.1.0.dev2/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/database/classmap.py` & `splight-lib-3.1.0.dev2/splight_lib/client/database/classmap.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from splight_lib.constants import ENGINE_PREFIX
 
 MODEL_NAME_MAP = {
+    "advancedfilter": f"{ENGINE_PREFIX}/alert/advancedfilters/",
     "alert": f"{ENGINE_PREFIX}/alert/alerts/",
     "asset": f"{ENGINE_PREFIX}/assets/",
     "attribute": f"{ENGINE_PREFIX}/attributes/",
+    "chart": f"{ENGINE_PREFIX}/dashboard/charts/",
+    "chartitem": f"{ENGINE_PREFIX}/dashboard/chartitems/",
     "component": f"{ENGINE_PREFIX}/component/components/",
     "componentobject": f"{ENGINE_PREFIX}/component/objects/",
+    "dashboard": f"{ENGINE_PREFIX}/dashboard/dashboards/",
     "file": f"{ENGINE_PREFIX}/files/",
+    "filter": f"{ENGINE_PREFIX}/dashboard/filters/",
     "query": f"{ENGINE_PREFIX}/queries/",
     "secret": f"{ENGINE_PREFIX}/secrets/",
     "setpoint": f"{ENGINE_PREFIX}/setpoints/",
+    "tab": f"{ENGINE_PREFIX}/dashboard/tabs/",
 }
 
 CUSTOM_PATHS_MAP = {
     "set-asset-attribute": "{prefix}/assets/{asset}/set-attribute/",
     "get-asset-attribute": "{prefix}/assets/{asset}/get-attribute/",
 }
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/database/local_client.py` & `splight-lib-3.1.0.dev2/splight_lib/client/database/local_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 from splight_lib.client.database.abstract import AbstractDatabaseClient
 from splight_lib.client.exceptions import InstanceNotFound
 from splight_lib.client.filter import value_filter_on_tuple
 from splight_lib.logging._internal import LogTags, get_splight_logger
 
 logger = get_splight_logger()
 
+LOCAL_DB_FILE = "splight-db.json"
+
 
 class LocalDatabaseClient(AbstractDatabaseClient):
     """Database Client implementation for a local database that uses a
     JSON file.
     """
 
     def __init__(self, path: str, *args, **kwargs):
         super().__init__()
-        self._db_file = os.path.join(path, "splight-db.json")
+        self._db_file = os.path.join(path, LOCAL_DB_FILE)
 
         if not os.path.exists(self._db_file):
             self._save_db(self._db_file, {})
         logger.debug(
             "Local database client initialized.", tags=LogTags.DATABASE
         )
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/database/remote_client.py` & `splight-lib-3.1.0.dev2/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/datalake/abstract.py` & `splight-lib-3.1.0.dev2/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/datalake/builder.py` & `splight-lib-3.1.0.dev2/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/datalake/local_client.py` & `splight-lib-3.1.0.dev2/splight_lib/client/datalake/local_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 class LocalDatalakeClient(AbstractDatalakeClient):
     """Datalake client implementation for a storing locally documents
     in different files.
     """
 
     _DEFAULT = "default"
     _PREFIX = "splight-dl_"
+    _SUFFIX = ".json"
     _TOTAL_DOCS = 10000
 
     def __init__(self, path: str, *args, **kwargs):
         super().__init__()
         self._base_path = path
         logger.info(
             "Local datalake client initialized.", tags=LogTags.DATALAKE
@@ -155,8 +156,8 @@
         for key, value in filters.items():
             if value is None:
                 continue
             new_filters[key] = value
         return new_filters
 
     def _get_file_name(self, collection: str) -> str:
-        return f"{self._PREFIX}{collection}"
+        return f"{self._PREFIX}{collection}{self._SUFFIX}"
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.1.0.dev2/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/exceptions.py` & `splight-lib-3.1.0.dev2/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/file_handler.py` & `splight-lib-3.1.0.dev2/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/filter.py` & `splight-lib-3.1.0.dev2/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/hub/abstract.py` & `splight-lib-3.1.0.dev2/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/client/hub/client.py` & `splight-lib-3.1.0.dev2/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/communication/event_handler.py` & `splight-lib-3.1.0.dev2/splight_lib/communication/event_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/component/abstract.py` & `splight-lib-3.1.0.dev2/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/component/exceptions.py` & `splight-lib-3.1.0.dev2/splight_lib/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/component/spec.py` & `splight-lib-3.1.0.dev2/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/encryption.py` & `splight-lib-3.1.0.dev2/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/execution.py` & `splight-lib-3.1.0.dev2/splight_lib/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,17 @@
         return
 
     def _start_task(self, job: Task) -> None:
         logger.debug("Starting Task", tags=LogTags.RUNTIME)
         if not getattr(self, "_scheduler", None):
             # Instantiate and start Scheduler thread
             self._scheduler = Scheduler()
-            self._start_thread(Thread(target=self._scheduler.start))
+            self._start_thread(
+                Thread(target=self._scheduler.start, daemon=False)
+            )
 
         return self._scheduler.schedule(job)
 
     def _stop_task(self, job: Task) -> None:
         logger.debug("Stopping Task", tags=LogTags.RUNTIME)
         return self._scheduler.unschedule(job)
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/logging/_internal.py` & `splight-lib-3.1.0.dev2/splight_lib/logging/_internal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from enum import auto
 from logging import INFO, Formatter, Handler
 from typing import Optional
 
 from concurrent_log_handler import ConcurrentRotatingFileHandler
-from splight_lib.logging.constants import LOGGING_DEV
+# from splight_lib.logging.constants import LOGGING_DEV
 from splight_lib.logging.logging import (
-    ElasticDocumentFormatter,
+    # ElasticDocumentFormatter,
     SplightFormatter,
     SplightLogger,
-    elastic_document_handler,
+    # elastic_document_handler,
     standard_output_handler,
 )
 from strenum import UppercaseStrEnum
 
 
 # TODO: add more tags
 class LogTags(UppercaseStrEnum):
@@ -53,15 +53,15 @@
     """Stdout logger."""
     if name is None:
         name = "splight-dev"
     logger = SplightLogger(name=name)
     logger.propagate = False
     stdout_handler = standard_output_handler(log_level=logger.level)
     logger.addHandler(stdout_handler)
-    es_handler = elastic_document_handler(
-        formatter=ElasticDocumentFormatter(type=LOGGING_DEV),
-        log_level=logger.level,
-    )
-    logger.addHandler(es_handler)
+    # es_handler = elastic_document_handler(
+    #     formatter=ElasticDocumentFormatter(type=LOGGING_DEV),
+    #     log_level=logger.level,
+    # )
+    # logger.addHandler(es_handler)
     # Add logger.level to root logger
     logger.setLevel(logger.level)
     return logger
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/logging/component.py` & `splight-lib-3.1.0.dev2/splight_lib/logging/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
-from logging import INFO, Formatter, Handler, basicConfig
+from logging import INFO, Formatter, Handler  # , basicConfig
 from typing import Optional
 
 from concurrent_log_handler import ConcurrentRotatingFileHandler
-from splight_lib.logging.constants import LOGGING_COMPONENTS
+# from splight_lib.logging.constants import LOGGING_COMPONENTS
 from splight_lib.logging.logging import (
-    ElasticDocumentFormatter,
+    # ElasticDocumentFormatter,
     SplightFormatter,
     SplightLogger,
-    elastic_document_handler,
+    # elastic_document_handler,
     standard_output_handler,
 )
 
 
 def component_file_handler(
     formatter: Optional[Formatter] = SplightFormatter(),
     log_level: Optional[str] = INFO,
@@ -35,19 +35,19 @@
         name = "component"
     logger = SplightLogger(name=name)
     logger.propagate = False
     stdout_handler = standard_output_handler(log_level=logger.level)
     logger.addHandler(stdout_handler)
     file_handler = component_file_handler(log_level=logger.level)
     logger.addHandler(file_handler)
-    es_handler = elastic_document_handler(
-        formatter=ElasticDocumentFormatter(type=LOGGING_COMPONENTS),
-        log_level=logger.level,
-    )
-    logger.addHandler(es_handler)
+    # es_handler = elastic_document_handler(
+    #     formatter=ElasticDocumentFormatter(type=LOGGING_COMPONENTS),
+    #     log_level=logger.level,
+    # )
+    # logger.addHandler(es_handler)
 
     # Add logger.level to root logger
     logger.setLevel(logger.level)
     return logger
 
 
 def getLogger(name: Optional[str] = None):
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/logging/logging.py` & `splight-lib-3.1.0.dev2/splight_lib/logging/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import json
+# import json
 import os
 import sys
-import time
+# import time
 from logging import (
     CRITICAL,
     DEBUG,
     ERROR,
     INFO,
     NOTSET,
     WARNING,
     Formatter,
     Handler,
     Logger,
     StreamHandler,
 )
 from logging import root as rootLogger
-from typing import Dict, Literal, Optional
+from typing import Dict, Optional
 
-from concurrent_log_handler import ConcurrentRotatingFileHandler
-from pydantic import BaseSettings
-from splight_lib.logging.constants import LOGGING_DEV, LogType
+# from concurrent_log_handler import ConcurrentRotatingFileHandler
+# from pydantic import BaseSettings
+# from splight_lib.logging.constants import LOGGING_DEV, LogType
 
 TAGS_KEY = "tags"
 
 
 class SplightFormatter(Formatter):
     DEFAULT_FMT: str = (
         "%(levelname)s | %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
@@ -32,32 +32,41 @@
     def format(self, record):
         fmt = self.DEFAULT_FMT
         try:
             if record.tags is not None:
                 fmt = " | ".join([fmt, "%(tags)s"])
         except AttributeError:
             pass  # tags aren't present
-        formatter = Formatter(fmt=fmt)
-        formatter.converter = time.gmtime
+        formatter = Formatter(fmt=fmt, datefmt="%Y-%m-%dT%H:%M:%S%z")
+        # formatter.converter = time.gmtime
         return formatter.format(record)
 
 
-class ElasticDocumentFormatter(Formatter):
-    def __init__(self, fmt: str = None, type: LogType = LOGGING_DEV) -> None:
-        super().__init__(fmt=fmt)
-        self.type = type
-
-    @property
-    def _extra_fields(self) -> Dict:
-        return {
-            "type": self.type,
-        }
-
-    def format(self, record):
-        return json.dumps({**record.__dict__, **self._extra_fields})
+# class SplightExceptionFormatter(SplightFormatter):
+#     def format(self, record):
+#         fmt = self.DEFAULT_FMT
+#
+#         __import__('ipdb').set_trace()
+#         formatter = Formatter(fmt=fmt, datefmt="%Y-%m-%dT%H:%M:%S%z")
+#         return formatter.format(record)
+
+
+# class ElasticDocumentFormatter(Formatter):
+#     def __init__(self, fmt: str = None, type: LogType = LOGGING_DEV) -> None:
+#         super().__init__(fmt=fmt)
+#         self.type = type
+#
+#     @property
+#     def _extra_fields(self) -> Dict:
+#         return {
+#             "type": self.type,
+#         }
+#
+#     def format(self, record):
+#         return json.dumps({**record.__dict__, **self._extra_fields})
 
 
 class SplightLogger(Logger):
     def __init__(self, name: str = None) -> None:
         # this is to avoid adding handlers to root logger
         # and interfering with third party app logs
         self.name = name if name is not None else "splight"
@@ -163,32 +172,32 @@
 ) -> Handler:
     handler = StreamHandler(sys.stdout)
     handler.setFormatter(formatter)
     handler.setLevel(log_level)
     return handler
 
 
-class ElasticDocumentHandlerSettings(BaseSettings):
-    splight_elastic_logs_filename: str = "/tmp/splight_elastic_logs.log"
-    splight_elastic_logs_max_bytes: int = 5e6
-    splight_elastic_logs_backup_count: int = 5
-
-    @property
-    def file_handler_settings(self) -> Dict:
-        return {
-            "filename": self.splight_elastic_logs_filename,
-            "maxBytes": self.splight_elastic_logs_max_bytes,
-            "backupCount": self.splight_elastic_logs_backup_count,
-            "encoding": "utf-8",
-        }
-
-
-def elastic_document_handler(
-    formatter: Optional[Formatter] = SplightFormatter(),
-    log_level: Optional[str] = INFO,
-) -> Handler:
-    settings = ElasticDocumentHandlerSettings()
-    handler = ConcurrentRotatingFileHandler(**settings.file_handler_settings)
-
-    handler.setFormatter(formatter)
-    handler.setLevel(log_level)
-    return handler
+# class ElasticDocumentHandlerSettings(BaseSettings):
+#     splight_elastic_logs_filename: str = "/tmp/splight_elastic_logs.log"
+#     splight_elastic_logs_max_bytes: int = 5e6
+#     splight_elastic_logs_backup_count: int = 5
+#
+#     @property
+#     def file_handler_settings(self) -> Dict:
+#         return {
+#             "filename": self.splight_elastic_logs_filename,
+#             "maxBytes": self.splight_elastic_logs_max_bytes,
+#             "backupCount": self.splight_elastic_logs_backup_count,
+#             "encoding": "utf-8",
+#         }
+#
+#
+# def elastic_document_handler(
+#     formatter: Optional[Formatter] = SplightFormatter(),
+#     log_level: Optional[str] = INFO,
+# ) -> Handler:
+#     settings = ElasticDocumentHandlerSettings()
+#     handler = ConcurrentRotatingFileHandler(**settings.file_handler_settings)
+#
+#     handler.setFormatter(formatter)
+#     handler.setLevel(log_level)
+#     return handler
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/__init__.py` & `splight-lib-3.1.0.dev2/splight_lib/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,39 @@
 from splight_lib.models.asset import Asset
 from splight_lib.models.attribute import Attribute
 from splight_lib.models.component import (
     Component,
     ComponentObject,
     ComponentObjectInstance,
 )
+from splight_lib.models.dashboard import Dashboard, Tab, Chart, ChartItem, Filter, AdvancedFilter
 from splight_lib.models.file import File
 from splight_lib.models.hub import HubComponent, HubComponentVersion
 from splight_lib.models.native import Boolean, Number, String
 from splight_lib.models.query import Query
 from splight_lib.models.secret import Secret
 from splight_lib.models.setpoint import SetPoint
 
 __all__ = [
+    AdvancedFilter,
     Alert,
     AlertCondition,
     Asset,
     Attribute,
     Boolean,
+    Chart,
+    ChartItem,
     Component,
     ComponentObject,
     ComponentObjectInstance,
+    Dashboard,
     File,
+    Filter,
     HubComponent,
     HubComponentVersion,
     Number,
     Query,
     String,
     Secret,
     SetPoint,
+    Tab,
 ]
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/alert.py` & `splight-lib-3.1.0.dev2/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/asset.py` & `splight-lib-3.1.0.dev2/splight_lib/models/asset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Tuple
 
-from geojson_pydantic import GeometryCollection, Point
+from geojson_pydantic import GeometryCollection
 from splight_lib.models.attribute import Attribute
 from splight_lib.models.base import SplightDatabaseBaseModel
 
 
-class Tag:
-    name: str
-    description: Optional[str] = None
-
-
 class Asset(SplightDatabaseBaseModel):
     id: Optional[str]
     name: str
     description: Optional[str] = None
-    tags: List[Tag] = []
+    tags: List[str] = []
     attributes: List[Attribute] = []
     verified: bool = False
     geometry: Optional[GeometryCollection]
-    centroid: Optional[Point]
+    centroid_coordinates: Optional[Tuple[float, float]]
     external_id: Optional[str] = None
     is_public: bool = False
 
     def set_attribute(self, attribute: Attribute, value: Any, value_type: str):
         new_value = self._db_client.operate(
             resource_name="set-asset-attribute",
             instance={
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/base.py` & `splight-lib-3.1.0.dev2/splight_lib/models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/communication.py` & `splight-lib-3.1.0.dev2/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/component.py` & `splight-lib-3.1.0.dev2/splight_lib/models/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,14 +156,17 @@
     return value
 
 
 def get_field_value(field: InputParameter):
     multiple = field.multiple
 
     value = field.value
+    if not value:
+        return [] if multiple else None
+
     if field.type in NATIVE_TYPES:
         value = (
             field.value
             if not isinstance(field.value, str)
             else parse_variable_string(field.value)
         )
     elif field.type in DATABASE_TYPES:
@@ -275,14 +278,17 @@
         custom_type: CustomType,
         component_id: Optional[str] = None,
     ) -> Type["ComponentObjectInstance"]:
         fields = {}
         for field in custom_type.fields:
             field_type = DB_MODEL_TYPE_MAPPING.get(field.type, cls)
             field_type = List[field_type] if field.multiple else field_type
+            field_type = (
+                Optional[field_type] if not field.required else field_type
+            )
             fields.update({field.name: (field_type, ...)})
         fields.update(
             {
                 "_schema": (
                     ClassVar[Optional[CustomType]],
                     custom_type,
                 ),
@@ -314,7 +320,17 @@
             {
                 "id": instance.id,
                 "name": instance.name,
                 "description": instance.description,
             }
         )
         return cls.parse_obj(params_dict)
+
+    @classmethod
+    def from_component(
+        cls,
+        component: Component,
+    ) -> Dict[str, "ComponentObjectInstance"]:
+        return {
+            ct.name: cls.from_custom_type(ct, component.id)
+            for ct in component.custom_types
+        }
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/event.py` & `splight-lib-3.1.0.dev2/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/file.py` & `splight-lib-3.1.0.dev2/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/hub.py` & `splight-lib-3.1.0.dev2/splight_lib/models/hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,26 +153,28 @@
     def upload(cls, path: str):
         hub_client = get_hub_client()
         spec = get_spec(path)
         name = spec["name"]
         version = spec["version"]
         file_name = f"{name}-{version}.{COMPRESSION_TYPE}"
         ignore_pathspec = get_ignore_pathspec(path)
-        versioned_name = f"{name}-{version}"
+        versioned_path = f"{name}-{version}"
         readme_path = os.path.join(path, README_FILE_1)
         if not os.path.exists(readme_path):
             readme_path = os.path.join(path, README_FILE_2)
         with py7zr.SevenZipFile(file_name, "w") as archive:
-
             all_files = glob(f"{path}/**", recursive=True)
-            for filename in all_files:
-                filepath = os.path.join(path, filename)
+            for filepath in all_files:
                 if ignore_pathspec and ignore_pathspec.match_file(filepath):
                     continue
-                archive.write(filepath, os.path.join(versioned_name, filename))
+                if os.path.isdir(filepath):
+                    continue
+                filename = os.path.basename(filepath)
+                new_filepath = os.path.join(versioned_path, filename)
+                archive.write(filepath, new_filepath)
 
         data = {
             "name": name,
             "version": version,
             "splight_cli_version": spec["splight_cli_version"],
             "privacy_policy": spec.get("privacy_policy", "private"),
             "tags": spec.get("tags", []),
@@ -186,15 +188,19 @@
             "bindings": json.dumps(spec.get("bindings", [])),
             "endpoints": json.dumps(spec.get("endpoints", [])),
         }
         files = {
             "file": open(file_name, "rb"),
             "readme": open(readme_path, "rb"),
         }
-        component = hub_client.upload(data=data, files=files)
-        if os.path.exists(file_name):
-            os.remove(file_name)
+        try:
+            component = hub_client.upload(data=data, files=files)
+        except Exception as exc:
+            raise Exception("unable to push component") from exc
+        finally:
+            if os.path.exists(file_name):
+                os.remove(file_name)
         return cls.parse_obj(component)
 
 
 class HubComponentVersion(HubComponent):
     pass
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/native.py` & `splight-lib-3.1.0.dev2/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/query.py` & `splight-lib-3.1.0.dev2/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/models/setpoint.py` & `splight-lib-3.1.0.dev2/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/restclient/client.py` & `splight-lib-3.1.0.dev2/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/restclient/exceptions.py` & `splight-lib-3.1.0.dev2/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/restclient/types.py` & `splight-lib-3.1.0.dev2/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/settings.py` & `splight-lib-3.1.0.dev2/splight_lib/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     return config
 
 
 class SplightSettings(BaseSettings, Singleton):
     SPLIGHT_ACCESS_ID: str = ""
     SPLIGHT_SECRET_KEY: str = ""
     SPLIGHT_PLATFORM_API_HOST: str = "https://api.splight-ai.com"
+    SPLIGHT_GRPC_HOST: str = "integrationgrpc.splight-ai.com:443"
+    # SPLIGHT_GRPC_HOST: str = "grpc.splight-ai.com:443"
 
     # Parameters for local environment
     LOCAL_ENVIRONMENT: bool = False
     CURRENT_DIR: Optional[str]
 
     @root_validator(allow_reuse=True)
     def validate_local_environment(cls, values: Dict):
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib/testing/__init__.py` & `splight-lib-3.1.0.dev2/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/utils/custom_model.py` & `splight-lib-3.1.0.dev2/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/utils/hub.py` & `splight-lib-3.1.0.dev2/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib/webhook.py` & `splight-lib-3.1.0.dev2/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev0/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.1.0.dev2/splight_lib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.1.0.dev0
+Version: 3.1.0.dev2
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.1.0.dev0/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.1.0.dev2/splight_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,35 +36,40 @@
 splight_lib/client/database/local_client.py
 splight_lib/client/database/remote_client.py
 splight_lib/client/datalake/__init__.py
 splight_lib/client/datalake/abstract.py
 splight_lib/client/datalake/builder.py
 splight_lib/client/datalake/local_client.py
 splight_lib/client/datalake/remote_client.py
+splight_lib/client/grpc/__init__.py
+splight_lib/client/grpc/client.py
+splight_lib/client/grpc/reflector.py
 splight_lib/client/hub/__init__.py
 splight_lib/client/hub/abstract.py
 splight_lib/client/hub/client.py
 splight_lib/communication/__init__.py
 splight_lib/communication/event_handler.py
 splight_lib/component/__init__.py
 splight_lib/component/abstract.py
 splight_lib/component/exceptions.py
+splight_lib/component/log_streamer.py
 splight_lib/component/spec.py
 splight_lib/logging/__init__.py
 splight_lib/logging/_internal.py
 splight_lib/logging/component.py
 splight_lib/logging/constants.py
 splight_lib/logging/logging.py
 splight_lib/models/__init__.py
 splight_lib/models/alert.py
 splight_lib/models/asset.py
 splight_lib/models/attribute.py
 splight_lib/models/base.py
 splight_lib/models/communication.py
 splight_lib/models/component.py
+splight_lib/models/dashboard.py
 splight_lib/models/event.py
 splight_lib/models/exceptions.py
 splight_lib/models/file.py
 splight_lib/models/hub.py
 splight_lib/models/native.py
 splight_lib/models/query.py
 splight_lib/models/secret.py
```

