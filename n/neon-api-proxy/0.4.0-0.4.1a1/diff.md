# Comparing `tmp/neon-api-proxy-0.4.0.tar.gz` & `tmp/neon-api-proxy-0.4.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-api-proxy-0.4.0.tar", last modified: Wed Jun 28 22:52:11 2023, max compression
+gzip compressed data, was "neon-api-proxy-0.4.1a1.tar", last modified: Tue Jul  4 21:02:37 2023, max compression
```

## Comparing `neon-api-proxy-0.4.0.tar` & `neon-api-proxy-0.4.1a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:52:11.808069 neon-api-proxy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-28 22:52:11.804068 neon-api-proxy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:52:11.800068 neon-api-proxy-0.4.0/neon_api_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/alpha_vantage_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/cached_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:52:11.804068 neon-api-proxy-0.4.0/neon_api_proxy/client/
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/client/alpha_vantage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/client/financial_modeling_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/client/open_weather_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/client/wolfram_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/owm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:52:11.804068 neon-api-proxy-0.4.0/neon_api_proxy/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/services/alpha_vantage_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/services/owm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/services/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/services/wolfram_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/socket_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/neon_api_proxy/wolfram_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:52:11.804068 neon-api-proxy-0.4.0/neon_api_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-28 22:52:11.000000 neon-api-proxy-0.4.0/neon_api_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-28 22:52:11.000000 neon-api-proxy-0.4.0/neon_api_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:52:11.000000 neon-api-proxy-0.4.0/neon_api_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-28 22:52:11.000000 neon-api-proxy-0.4.0/neon_api_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-28 22:52:11.000000 neon-api-proxy-0.4.0/neon_api_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-28 22:52:11.000000 neon-api-proxy-0.4.0/neon_api_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:52:11.000000 neon-api-proxy-0.4.0/neon_api_proxy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 22:52:11.808069 neon-api-proxy-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-28 22:52:03.000000 neon-api-proxy-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:02:37.668978 neon-api-proxy-0.4.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-04 21:02:37.668978 neon-api-proxy-0.4.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:02:37.660978 neon-api-proxy-0.4.1a1/neon_api_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/alpha_vantage_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/cached_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:02:37.664978 neon-api-proxy-0.4.1a1/neon_api_proxy/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/client/alpha_vantage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/client/financial_modeling_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/client/open_weather_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/client/wolfram_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/owm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:02:37.668978 neon-api-proxy-0.4.1a1/neon_api_proxy/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/services/alpha_vantage_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/services/owm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/services/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/services/wolfram_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/socket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/neon_api_proxy/wolfram_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:02:37.664978 neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-04 21:02:37.000000 neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-04 21:02:37.000000 neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:02:37.000000 neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 21:02:37.000000 neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-04 21:02:37.000000 neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 21:02:37.000000 neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:02:37.000000 neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:02:37.668978 neon-api-proxy-0.4.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-04 21:02:33.000000 neon-api-proxy-0.4.1a1/setup.py
```

### Comparing `neon-api-proxy-0.4.0/LICENSE.md` & `neon-api-proxy-0.4.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/PKG-INFO` & `neon-api-proxy-0.4.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-api-proxy
-Version: 0.4.0
+Version: 0.4.1a1
 Summary: Neon Proxy for external API Calls
 Home-page: https://github.com/NeonGeckoCom/neon_api_proxy
 Author: Neongecko
 Author-email: developers@neon.ai
 License: NeonAI License v1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-api-proxy-0.4.0/README.md` & `neon-api-proxy-0.4.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/__init__.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/__main__.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/alpha_vantage_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/alpha_vantage_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/api_connector.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/api_connector.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/cached_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/cached_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/client/__init__.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/client/alpha_vantage.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/client/alpha_vantage.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/client/financial_modeling_prep.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/client/financial_modeling_prep.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/client/open_weather_map.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/client/open_weather_map.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/client/wolfram_alpha.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/client/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/config.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/config.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/controller.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/controller.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/owm_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/owm_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/services/__init__.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/services/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/services/alpha_vantage_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/services/alpha_vantage_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/services/owm_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/services/owm_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/services/test_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/services/test_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/services/wolfram_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/services/wolfram_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/socket_handler.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/socket_handler.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/test_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/test_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy/wolfram_api.py` & `neon-api-proxy-0.4.1a1/neon_api_proxy/wolfram_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy.egg-info/PKG-INFO` & `neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-api-proxy
-Version: 0.4.0
+Version: 0.4.1a1
 Summary: Neon Proxy for external API Calls
 Home-page: https://github.com/NeonGeckoCom/neon_api_proxy
 Author: Neongecko
 Author-email: developers@neon.ai
 License: NeonAI License v1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-api-proxy-0.4.0/neon_api_proxy.egg-info/SOURCES.txt` & `neon-api-proxy-0.4.1a1/neon_api_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.4.0/setup.py` & `neon-api-proxy-0.4.1a1/setup.py`

 * *Files identical despite different names*

