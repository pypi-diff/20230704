# Comparing `tmp/kucoin-futures-python-1.0.6.tar.gz` & `tmp/kucoin-futures-python-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aaron/Workspace/test/1129/kucoin-futures-python-sdk/dist/tmpun2d2212/kucoin-futures-python-1.0.6.tar", last modified: Fri Dec  3 06:26:41 2021, max compression
+gzip compressed data, was "kucoin-futures-python-1.0.7.tar", last modified: Tue Jul  4 02:25:17 2023, max compression
```

## Comparing `kucoin-futures-python-1.0.6.tar` & `kucoin-futures-python-1.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.236861 kucoin-futures-python-1.0.6/
--rw-r--r--   0 aaron      (501) staff       (20)     1063 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/LICENSE
--rw-r--r--   0 aaron      (501) staff       (20)      420 2021-12-03 06:26:41.236562 kucoin-futures-python-1.0.6/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)     3732 2021-12-01 13:55:36.000000 kucoin-futures-python-1.0.6/README.rst
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.228529 kucoin-futures-python-1.0.6/kucoin_futures/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/__init__.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.229372 kucoin-futures-python-1.0.6/kucoin_futures/base_request/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/base_request/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)     4299 2021-12-01 14:01:50.000000 kucoin-futures-python-1.0.6/kucoin_futures/base_request/base_request.py
--rw-r--r--   0 aaron      (501) staff       (20)      350 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/client.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.230443 kucoin-futures-python-1.0.6/kucoin_futures/marke_data/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/marke_data/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)    22513 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/marke_data/market_data.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.231522 kucoin-futures-python-1.0.6/kucoin_futures/trade/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/trade/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)    28743 2021-12-01 13:49:30.000000 kucoin-futures-python-1.0.6/kucoin_futures/trade/trade.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.232890 kucoin-futures-python-1.0.6/kucoin_futures/user/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/user/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)     9818 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/user/user.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.233586 kucoin-futures-python-1.0.6/kucoin_futures/websocket/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/websocket/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)     5633 2021-12-02 12:37:01.000000 kucoin-futures-python-1.0.6/kucoin_futures/websocket/websocket.py
--rw-r--r--   0 aaron      (501) staff       (20)     1620 2021-12-02 12:40:53.000000 kucoin-futures-python-1.0.6/kucoin_futures/ws_client.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.234554 kucoin-futures-python-1.0.6/kucoin_futures/ws_token/
--rw-r--r--   0 aaron      (501) staff       (20)        0 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/ws_token/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)      480 2021-12-01 13:19:22.000000 kucoin-futures-python-1.0.6/kucoin_futures/ws_token/token.py
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-12-03 06:26:41.236239 kucoin-futures-python-1.0.6/kucoin_futures_python.egg-info/
--rw-r--r--   0 aaron      (501) staff       (20)      420 2021-12-03 06:26:41.000000 kucoin-futures-python-1.0.6/kucoin_futures_python.egg-info/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)      761 2021-12-03 06:26:41.000000 kucoin-futures-python-1.0.6/kucoin_futures_python.egg-info/SOURCES.txt
--rw-r--r--   0 aaron      (501) staff       (20)        1 2021-12-03 06:26:41.000000 kucoin-futures-python-1.0.6/kucoin_futures_python.egg-info/dependency_links.txt
--rw-r--r--   0 aaron      (501) staff       (20)       20 2021-12-03 06:26:41.000000 kucoin-futures-python-1.0.6/kucoin_futures_python.egg-info/requires.txt
--rw-r--r--   0 aaron      (501) staff       (20)      159 2021-12-03 06:26:41.000000 kucoin-futures-python-1.0.6/kucoin_futures_python.egg-info/top_level.txt
--rw-r--r--   0 aaron      (501) staff       (20)       38 2021-12-03 06:26:41.236950 kucoin-futures-python-1.0.6/setup.cfg
--rw-r--r--   0 aaron      (501) staff       (20)      751 2021-12-01 13:56:49.000000 kucoin-futures-python-1.0.6/setup.py
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.948233 kucoin-futures-python-1.0.7/
+-rw-rw-r--   0 bernardong   (501) staff       (20)     1063 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/LICENSE
+-rw-r--r--   0 bernardong   (501) staff       (20)      392 2023-07-04 02:25:17.947957 kucoin-futures-python-1.0.7/PKG-INFO
+-rw-rw-r--   0 bernardong   (501) staff       (20)     3732 2023-07-04 02:24:30.000000 kucoin-futures-python-1.0.7/README.rst
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.931737 kucoin-futures-python-1.0.7/kucoin_futures/
+-rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/__init__.py
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.932503 kucoin-futures-python-1.0.7/kucoin_futures/base_request/
+-rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/base_request/__init__.py
+-rw-rw-r--   0 bernardong   (501) staff       (20)     4299 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/base_request/base_request.py
+-rw-rw-r--   0 bernardong   (501) staff       (20)      350 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/client.py
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.933275 kucoin-futures-python-1.0.7/kucoin_futures/marke_data/
+-rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/marke_data/__init__.py
+-rw-rw-r--   0 bernardong   (501) staff       (20)    22513 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/marke_data/market_data.py
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.934050 kucoin-futures-python-1.0.7/kucoin_futures/trade/
+-rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/trade/__init__.py
+-rw-rw-r--   0 bernardong   (501) staff       (20)    28743 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/trade/trade.py
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.934894 kucoin-futures-python-1.0.7/kucoin_futures/user/
+-rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/user/__init__.py
+-rw-rw-r--   0 bernardong   (501) staff       (20)    15637 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/user/user.py
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.935616 kucoin-futures-python-1.0.7/kucoin_futures/websocket/
+-rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/websocket/__init__.py
+-rw-rw-r--   0 bernardong   (501) staff       (20)     5633 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/websocket/websocket.py
+-rw-rw-r--   0 bernardong   (501) staff       (20)     1620 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/ws_client.py
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.936392 kucoin-futures-python-1.0.7/kucoin_futures/ws_token/
+-rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/ws_token/__init__.py
+-rw-rw-r--   0 bernardong   (501) staff       (20)      480 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/ws_token/token.py
+drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.947456 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/
+-rw-r--r--   0 bernardong   (501) staff       (20)      392 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/PKG-INFO
+-rw-r--r--   0 bernardong   (501) staff       (20)      761 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/SOURCES.txt
+-rw-r--r--   0 bernardong   (501) staff       (20)        1 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/dependency_links.txt
+-rw-r--r--   0 bernardong   (501) staff       (20)       20 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/requires.txt
+-rw-r--r--   0 bernardong   (501) staff       (20)      159 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/top_level.txt
+-rw-r--r--   0 bernardong   (501) staff       (20)       38 2023-07-04 02:25:17.948288 kucoin-futures-python-1.0.7/setup.cfg
+-rw-rw-r--   0 bernardong   (501) staff       (20)      751 2023-07-04 02:24:03.000000 kucoin-futures-python-1.0.7/setup.py
```

### Comparing `kucoin-futures-python-1.0.6/LICENSE` & `kucoin-futures-python-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.6/README.rst` & `kucoin-futures-python-1.0.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - Implementation of REST endpoints
 - Simple handling of authentication
 - Response exception handling
 - Implement websockets (note only python3.6+)
 
 update
 ----------
-- 2021 12/01
+- 2023 07/04
 
 Quick Start
 -----------
 
 Register an account with `KuCoin_Futures <https://futures.kucoin.com/signup?utm=api_github>`_.
 
 To test on the Sandbox  with `KuCoin_Futures Sandbox <https://sandbox-futures.kucoin.com>`_.
```

### Comparing `kucoin-futures-python-1.0.6/kucoin_futures/base_request/base_request.py` & `kucoin-futures-python-1.0.7/kucoin_futures/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.6/kucoin_futures/marke_data/market_data.py` & `kucoin-futures-python-1.0.7/kucoin_futures/marke_data/market_data.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.6/kucoin_futures/trade/trade.py` & `kucoin-futures-python-1.0.7/kucoin_futures/trade/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.6/kucoin_futures/websocket/websocket.py` & `kucoin-futures-python-1.0.7/kucoin_futures/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.6/kucoin_futures/ws_client.py` & `kucoin-futures-python-1.0.7/kucoin_futures/ws_client.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.6/kucoin_futures_python.egg-info/SOURCES.txt` & `kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.6/setup.py` & `kucoin-futures-python-1.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 from setuptools import setup
 
 
 setup(
     name='kucoin-futures-python',
-    version='v1.0.6',
+    version='v1.0.7',
     packages=['kucoin_futures', 'kucoin_futures/base_request', 'kucoin_futures/marke_data', 'kucoin_futures/trade', 'kucoin_futures/user',
               'kucoin_futures/websocket', 'kucoin_futures/ws_token'],
     license="MIT",
     author='Grape',
     author_email="grape.zhang@kucoin.com",
     url='https://github.com/Kucoin/kucoin-futures-python-sdk',
     description="kucoin-futures-api-sdk",
```

