# Comparing `tmp/cs-binance-c2c-sapi-0.0.8.tar.gz` & `tmp/cs-binance-c2c-sapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-binance-c2c-sapi-0.0.8.tar", last modified: Fri Jun  2 16:10:49 2023, max compression
+gzip compressed data, was "cs-binance-c2c-sapi-0.0.9.tar", last modified: Thu Jun  8 10:38:31 2023, max compression
```

## Comparing `cs-binance-c2c-sapi-0.0.8.tar` & `cs-binance-c2c-sapi-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-02 16:10:36.000000 cs-binance-c2c-sapi-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/binance_c2c/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 16:10:36.000000 cs-binance-c2c-sapi-0.0.8/binance_c2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-06-02 16:10:36.000000 cs-binance-c2c-sapi-0.0.8/binance_c2c/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 16:10:49.000000 cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:10:49.618006 cs-binance-c2c-sapi-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-02 16:10:36.000000 cs-binance-c2c-sapi-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:38:31.796886 cs-binance-c2c-sapi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-08 10:38:31.796886 cs-binance-c2c-sapi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-08 10:38:04.000000 cs-binance-c2c-sapi-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:38:31.796886 cs-binance-c2c-sapi-0.0.9/binance_c2c/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 10:38:04.000000 cs-binance-c2c-sapi-0.0.9/binance_c2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-08 10:38:04.000000 cs-binance-c2c-sapi-0.0.9/binance_c2c/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:38:31.796886 cs-binance-c2c-sapi-0.0.9/cs_binance_c2c_sapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-08 10:38:31.000000 cs-binance-c2c-sapi-0.0.9/cs_binance_c2c_sapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 10:38:31.000000 cs-binance-c2c-sapi-0.0.9/cs_binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:38:31.000000 cs-binance-c2c-sapi-0.0.9/cs_binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 10:38:31.000000 cs-binance-c2c-sapi-0.0.9/cs_binance_c2c_sapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 10:38:31.000000 cs-binance-c2c-sapi-0.0.9/cs_binance_c2c_sapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:38:31.796886 cs-binance-c2c-sapi-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-08 10:38:04.000000 cs-binance-c2c-sapi-0.0.9/setup.py
```

### Comparing `cs-binance-c2c-sapi-0.0.8/PKG-INFO` & `cs-binance-c2c-sapi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.8/README.md` & `cs-binance-c2c-sapi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cs-binance-c2c-sapi-0.0.8/binance_c2c/api.py` & `cs-binance-c2c-sapi-0.0.9/binance_c2c/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         Returns:
             dict: Response data in JSON format.
         """
         url = f'{self.BASE_URL}{endpoint}'
         server_time = self.get_server_time()
 
-        params = {
+        params = { **params, 
             'timestamp': server_time
         }
 
         signature = self.create_signature(params)
         params['signature'] = signature
 
         headers = {
```

### Comparing `cs-binance-c2c-sapi-0.0.8/cs_binance_c2c_sapi.egg-info/PKG-INFO` & `cs-binance-c2c-sapi-0.0.9/cs_binance_c2c_sapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.8/setup.py` & `cs-binance-c2c-sapi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="cs-binance-c2c-sapi",
     version=VERSION,
```

