# Comparing `tmp/crypto-ws-api-1.0.0b5.tar.gz` & `tmp/crypto-ws-api-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-ws-api-1.0.0b5.tar", last modified: Mon Jul  3 19:09:52 2023, max compression
+gzip compressed data, was "crypto-ws-api-1.0.0b6.tar", last modified: Mon Jul  3 19:17:56 2023, max compression
```

## Comparing `crypto-ws-api-1.0.0b5.tar` & `crypto-ws-api-1.0.0b6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 crypto-ws-api-1.0.0b5/.deepsource.toml
--rwxr-xr-x   0        0        0        0 2023-06-30 17:00:48.867088 crypto-ws-api-1.0.0b5/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-30 17:01:10.037954 crypto-ws-api-1.0.0b5/LICENSE.md
--rw-r--r--   0        0        0     5136 2023-07-03 17:43:53.839959 crypto-ws-api-1.0.0b5/README.md
--rw-r--r--   0        0        0     1302 2023-07-03 19:09:42.881579 crypto-ws-api-1.0.0b5/crypto_ws_api/__init__.py
--rw-r--r--   0        0        0     3143 2023-07-03 17:58:56.640301 crypto-ws-api-1.0.0b5/crypto_ws_api/demo.py
--rw-r--r--   0        0        0      551 2023-07-01 18:52:39.110102 crypto-ws-api-1.0.0b5/crypto_ws_api/ws_api.toml.template
--rw-r--r--   0        0        0    10263 2023-07-03 19:09:26.747828 crypto-ws-api-1.0.0b5/crypto_ws_api/ws_session.py
--rw-r--r--   0        0        0     1002 2023-07-02 15:35:03.964461 crypto-ws-api-1.0.0b5/pyproject.toml
--rw-r--r--   0        0        0       90 2023-07-03 18:01:56.150626 crypto-ws-api-1.0.0b5/requirements.txt
--rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 crypto-ws-api-1.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 crypto-ws-api-1.0.0b6/.deepsource.toml
+-rwxr-xr-x   0        0        0        0 2023-06-30 17:00:48.867088 crypto-ws-api-1.0.0b6/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-30 17:01:10.037954 crypto-ws-api-1.0.0b6/LICENSE.md
+-rw-r--r--   0        0        0     5136 2023-07-03 17:43:53.839959 crypto-ws-api-1.0.0b6/README.md
+-rw-r--r--   0        0        0     1302 2023-07-03 19:17:40.027531 crypto-ws-api-1.0.0b6/crypto_ws_api/__init__.py
+-rw-r--r--   0        0        0     3143 2023-07-03 17:58:56.640301 crypto-ws-api-1.0.0b6/crypto_ws_api/demo.py
+-rw-r--r--   0        0        0      551 2023-07-01 18:52:39.110102 crypto-ws-api-1.0.0b6/crypto_ws_api/ws_api.toml.template
+-rw-r--r--   0        0        0    10263 2023-07-03 19:09:26.747828 crypto-ws-api-1.0.0b6/crypto_ws_api/ws_session.py
+-rw-r--r--   0        0        0     1000 2023-07-03 19:17:40.031531 crypto-ws-api-1.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-07-03 18:01:56.150626 crypto-ws-api-1.0.0b6/requirements.txt
+-rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 crypto-ws-api-1.0.0b6/PKG-INFO
```

### Comparing `crypto-ws-api-1.0.0b5/LICENSE.md` & `crypto-ws-api-1.0.0b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.0b5/README.md` & `crypto-ws-api-1.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.0b5/crypto_ws_api/__init__.py` & `crypto-ws-api-1.0.0b6/crypto_ws_api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 __authors__ = ["Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.0.0b5"
+__version__ = "1.0.0b6"
 
 from pathlib import Path
 import shutil
 from platformdirs import user_config_path
 
 TIMEOUT = 10  # sec timeout for WSS receive
```

### Comparing `crypto-ws-api-1.0.0b5/crypto_ws_api/demo.py` & `crypto-ws-api-1.0.0b6/crypto_ws_api/demo.py`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.0b5/crypto_ws_api/ws_api.toml.template` & `crypto-ws-api-1.0.0b6/crypto_ws_api/ws_api.toml.template`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.0b5/crypto_ws_api/ws_session.py` & `crypto-ws-api-1.0.0b6/crypto_ws_api/ws_session.py`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.0b5/pyproject.toml` & `crypto-ws-api-1.0.0b6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper~=1.3.2-2",
+    "exchanges-wrapper~=1.3.2",
     "aiohttp==3.8.4",
     "shortuuid~=1.0.11",
     "platformdirs~=3.8.0",
     "toml~=0.10.2",
 ]
 
 [tool.flit.module]
```

### Comparing `crypto-ws-api-1.0.0b5/PKG-INFO` & `crypto-ws-api-1.0.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: crypto-ws-api
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: Crypto WS API connector for ASYNC requests
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper~=1.3.2-2
+Requires-Dist: exchanges-wrapper~=1.3.2
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: shortuuid~=1.0.11
 Requires-Dist: platformdirs~=3.8.0
 Requires-Dist: toml~=0.10.2
 Project-URL: Source, https://github.com/DogsTailFarmer/crypto-ws-api
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: crypto-ws-api Version: 1.0.0b5 Summary: Crypto WS
+Metadata-Version: 2.1 Name: crypto-ws-api Version: 1.0.0b6 Summary: Crypto WS
 API connector for ASYNC requests Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: exchanges-wrapper~=1.3.2-2 Requires-Dist: aiohttp==3.8.4 Requires-Dist:
+Dist: exchanges-wrapper~=1.3.2 Requires-Dist: aiohttp==3.8.4 Requires-Dist:
 shortuuid~=1.0.11 Requires-Dist: platformdirs~=3.8.0 Requires-Dist:
 toml~=0.10.2 Project-URL: Source, https://github.com/DogsTailFarmer/crypto-ws-
 api
  [https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-
                           4467-a0cd-21627a6a41ed.svg]
 ***
            ****** Crypto WS API connector for ASYNC requests ******
```

