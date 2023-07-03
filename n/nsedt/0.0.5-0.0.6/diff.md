# Comparing `tmp/nsedt-0.0.5.tar.gz` & `tmp/nsedt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsedt-0.0.5.tar", last modified: Tue Jun 27 18:52:42 2023, max compression
+gzip compressed data, was "nsedt-0.0.6.tar", last modified: Mon Jul  3 22:19:28 2023, max compression
```

## Comparing `nsedt-0.0.5.tar` & `nsedt-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.620384 nsedt-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 18:52:28.000000 nsedt-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-27 18:52:42.620384 nsedt-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-27 18:52:28.000000 nsedt-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.616384 nsedt-0.0.5/nsedt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/equity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.620384 nsedt-0.0.5/nsedt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/resources/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.620384 nsedt-0.0.5/nsedt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/utils/data_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.620384 nsedt-0.0.5/nsedt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-27 18:52:42.620384 nsedt-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-27 18:52:28.000000 nsedt-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:19:18.000000 nsedt-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-03 22:19:28.428807 nsedt-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-03 22:19:18.000000 nsedt-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/nsedt/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/equity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/indices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/nsedt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/resources/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/nsedt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/utils/data_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/nsedt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 22:19:28.428807 nsedt-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 22:19:18.000000 nsedt-0.0.6/setup.py
```

### Comparing `nsedt-0.0.5/LICENSE` & `nsedt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.5/PKG-INFO` & `nsedt-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nsedt-0.0.5/README.md` & `nsedt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.5/nsedt/equity.py` & `nsedt-0.0.6/nsedt/equity.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 
 import pandas as pd
 
 from nsedt import utils
 from nsedt.resources import constants as cns
 from nsedt.utils import data_format
 
-logging.basicConfig(
-    level=logging.INFO,
-    format=cns.LOG_FORMAT,
-    datefmt="%m/%d/%Y %I:%M:%S %p",
-)
+logger = logging.getLogger(__name__)
 
 
 def get_companyinfo(
     symbol,
     response_type="panda_df",
 ):
     """
@@ -91,15 +87,15 @@
         input_type (str): Either 'stock' or 'index'
         symbol (str, optional): stock symbol. Defaults to None. TODO: implement for index`
     Returns:
         Pandas DataFrame: df containing data for symbol of provided date range
     """
     cookies = utils.get_cookies()
     base_url = cns.BASE_URL
-    price_api = cns.EQUITY_PRICE_HISTROY
+    price_api = cns.EQUITY_PRICE_HISTORY
     url_list = []
 
     # set the window size to one year
     window_size = datetime.timedelta(days=cns.WINDOW_SIZE)
 
     current_window_start = start_date
     while current_window_start < end_date:
```

### Comparing `nsedt-0.0.5/nsedt/resources/constants.py` & `nsedt-0.0.6/nsedt/resources/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,13 +12,21 @@
     "process": "%(process)s",
     "filename": "%(filename)s",
     "funcName": "%(funcName)s",
     "logmessage": "%(message)s",
 }"""
 
 BASE_URL = "https://www.nseindia.com/"
-EQUITY_PRICE_HISTROY = "api/historical/securityArchives?"
+
+### EQUITY
+EQUITY_PRICE_HISTORY = "api/historical/securityArchives?"
 EQUITY_CORPINFO = "api/corporates-corporateActions?"
 MARKETSTATUS = "api/marketStatus"
 EQUITY_EVENT = "api/event-calendar?"
 EQUITY_CHART = "api/chart-databyindex?"
 EQUITY_INFO = "api/quote-equity?"
+
+### Index
+INDEX_PRICE_HISTORY = "api/historical/indicesHistory?"
+
+### DERIVATIVES
+DERIVATIVES_PRICE = "api/option-chain-equities?"
```

### Comparing `nsedt-0.0.5/nsedt/utils/__init__.py` & `nsedt-0.0.6/nsedt/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 utils for nsedt
 """
 
 import json
 
 import pandas as pd
 import requests
-
 from nsedt.resources import constants as cns
 
 
 def get_headers():
     """
     Args:
        ---
@@ -40,27 +39,36 @@
 
     response = requests.get(cns.BASE_URL, timeout=30, headers=get_headers())
     if response.status_code != 200:
         raise ValueError("Retry again in a minute.")
     return response.cookies.get_dict()
 
 
-def fetch_url(url, cookies, key=None):
+def fetch_url(url, cookies, key=None, response_type="panda_df"):
     """
     Args:
        url (str): URL to fetch
        cookies (str): NSE cokies
        key (str, Optional):
     Returns:
         Pandas DataFrame: df containing url data
 
     """
 
-    response = requests.get(url, timeout=30, headers=get_headers(), cookies=cookies)
+    response = requests.get(
+        url=url,
+        timeout=30,
+        headers=get_headers(),
+        cookies=cookies,
+    )
+
     if response.status_code == 200:
         json_response = json.loads(response.content)
+
+        if response_type != "panda_df":
+            return json_response
         if key is None:
             return pd.DataFrame.from_dict(json_response)
 
         return pd.DataFrame.from_dict(json_response[key])
 
     raise ValueError("Please try again in a minute.")
```

### Comparing `nsedt-0.0.5/nsedt.egg-info/PKG-INFO` & `nsedt-0.0.6/nsedt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nsedt-0.0.5/setup.py` & `nsedt-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Install script
 """
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
+
 setup(
     name="nsedt",
-    version="0.0.5",
+    version="0.0.6",
     author="Pratik Anand",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Library to collect NSE data in pandas dataframe",
     packages=find_packages(),
     url="https://github.com/pratik141/nsedt",
     install_requires=[
```

