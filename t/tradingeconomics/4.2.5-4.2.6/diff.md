# Comparing `tmp/tradingeconomics-4.2.5.tar.gz` & `tmp/tradingeconomics-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingeconomics-4.2.5.tar", last modified: Tue Jul  4 08:53:30 2023, max compression
+gzip compressed data, was "tradingeconomics-4.2.6.tar", last modified: Tue Jul  4 08:58:42 2023, max compression
```

## Comparing `tradingeconomics-4.2.5.tar` & `tradingeconomics-4.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:53:30.811207 tradingeconomics-4.2.5/
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       18 2021-08-04 09:35:15.000000 tradingeconomics-4.2.5/MANIFEST.in
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2712 2023-07-04 08:53:30.811207 tradingeconomics-4.2.5/PKG-INFO
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1701 2023-07-04 08:21:41.000000 tradingeconomics-4.2.5/README.rst
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       79 2023-07-04 08:53:30.812205 tradingeconomics-4.2.5/setup.cfg
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1157 2023-07-04 08:50:08.000000 tradingeconomics-4.2.5/setup.py
-drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:53:30.800531 tradingeconomics-4.2.5/tradingeconomics/
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     3627 2023-03-30 12:04:47.000000 tradingeconomics-4.2.5/tradingeconomics/__init__.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    10861 2023-03-02 09:48:16.000000 tradingeconomics-4.2.5/tradingeconomics/calendar.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    16631 2023-03-30 12:04:47.000000 tradingeconomics-4.2.5/tradingeconomics/comtrade.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4113 2023-05-22 15:34:38.000000 tradingeconomics-4.2.5/tradingeconomics/earnings.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     7002 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/eurostat.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    12372 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/federalReserve.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     5532 2023-03-30 12:04:47.000000 tradingeconomics-4.2.5/tradingeconomics/financials.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     5244 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/forecasts.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     8630 2023-05-22 15:34:38.000000 tradingeconomics-4.2.5/tradingeconomics/functions.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1234 2023-03-02 09:48:16.000000 tradingeconomics-4.2.5/tradingeconomics/glob.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    13237 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/historical.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4509 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/historicalDB.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     3073 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/historicalEurostat.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2702 2023-03-02 09:48:16.000000 tradingeconomics-4.2.5/tradingeconomics/historicalFinancials.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4185 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/historicalMarkets.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    16263 2023-03-23 08:22:30.000000 tradingeconomics-4.2.5/tradingeconomics/indicators.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    22232 2023-03-30 12:04:47.000000 tradingeconomics-4.2.5/tradingeconomics/markets.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    13802 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/news.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2149 2021-09-21 08:26:38.000000 tradingeconomics-4.2.5/tradingeconomics/search.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1969 2022-08-29 11:34:45.000000 tradingeconomics-4.2.5/tradingeconomics/stream.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     9449 2022-09-27 08:00:02.000000 tradingeconomics-4.2.5/tradingeconomics/worldBank.py
-drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:53:30.809045 tradingeconomics-4.2.5/tradingeconomics.egg-info/
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2712 2023-07-04 08:53:30.000000 tradingeconomics-4.2.5/tradingeconomics.egg-info/PKG-INFO
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)      886 2023-07-04 08:53:30.000000 tradingeconomics-4.2.5/tradingeconomics.egg-info/SOURCES.txt
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        1 2023-07-04 08:53:30.000000 tradingeconomics-4.2.5/tradingeconomics.egg-info/dependency_links.txt
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       24 2023-07-04 08:53:30.000000 tradingeconomics-4.2.5/tradingeconomics.egg-info/requires.txt
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       17 2023-07-04 08:53:30.000000 tradingeconomics-4.2.5/tradingeconomics.egg-info/top_level.txt
+drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:58:42.126787 tradingeconomics-4.2.6/
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       18 2021-08-04 09:35:15.000000 tradingeconomics-4.2.6/MANIFEST.in
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2719 2023-07-04 08:58:42.127793 tradingeconomics-4.2.6/PKG-INFO
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1708 2023-07-04 08:56:55.000000 tradingeconomics-4.2.6/README.rst
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       79 2023-07-04 08:58:42.128794 tradingeconomics-4.2.6/setup.cfg
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1157 2023-07-04 08:57:28.000000 tradingeconomics-4.2.6/setup.py
+drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:58:42.116748 tradingeconomics-4.2.6/tradingeconomics/
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     3627 2023-03-30 12:04:47.000000 tradingeconomics-4.2.6/tradingeconomics/__init__.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    10861 2023-03-02 09:48:16.000000 tradingeconomics-4.2.6/tradingeconomics/calendar.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    16631 2023-03-30 12:04:47.000000 tradingeconomics-4.2.6/tradingeconomics/comtrade.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4113 2023-05-22 15:34:38.000000 tradingeconomics-4.2.6/tradingeconomics/earnings.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     7002 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/eurostat.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    12372 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/federalReserve.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     5532 2023-03-30 12:04:47.000000 tradingeconomics-4.2.6/tradingeconomics/financials.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     5244 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/forecasts.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     8630 2023-05-22 15:34:38.000000 tradingeconomics-4.2.6/tradingeconomics/functions.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1234 2023-03-02 09:48:16.000000 tradingeconomics-4.2.6/tradingeconomics/glob.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    13237 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/historical.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4509 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/historicalDB.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     3073 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/historicalEurostat.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2702 2023-03-02 09:48:16.000000 tradingeconomics-4.2.6/tradingeconomics/historicalFinancials.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4185 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/historicalMarkets.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    16263 2023-03-23 08:22:30.000000 tradingeconomics-4.2.6/tradingeconomics/indicators.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    22232 2023-03-30 12:04:47.000000 tradingeconomics-4.2.6/tradingeconomics/markets.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    13802 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/news.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2149 2021-09-21 08:26:38.000000 tradingeconomics-4.2.6/tradingeconomics/search.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1969 2022-08-29 11:34:45.000000 tradingeconomics-4.2.6/tradingeconomics/stream.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     9449 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/worldBank.py
+drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:58:42.125282 tradingeconomics-4.2.6/tradingeconomics.egg-info/
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2719 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/PKG-INFO
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)      886 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        1 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       24 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/requires.txt
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       17 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/top_level.txt
```

### Comparing `tradingeconomics-4.2.5/PKG-INFO` & `tradingeconomics-4.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingeconomics
-Version: 4.2.5
+Version: 4.2.6
 Summary: Trading Economics API
 Home-page: https://github.com/tradingeconomics/tradingeconomics-python
 Author: Trading Economics
 Author-email: support@tradingeconomics.com
 License: MIT
 Download-URL: https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist
 Description: =====================
@@ -43,15 +43,15 @@
             - te.getFinancialsData(symbol='aapl:us', output_type='df')
         
         
         GitHub Examples
         ----------------------------------------
         
         You can find additional examples and usage instructions in the GitHub repository:
-         - https://github.com/tradingeconomics/tradingeconomics/tree/master/python
+         - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
         
         
         Documentation
         ----------------------------------------
         
         For detailed documentation and API reference, please visit the Trading Economics API documentation:
          - https://docs.tradingeconomics.com
```

### Comparing `tradingeconomics-4.2.5/README.rst` & `tradingeconomics-4.2.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     - te.getFinancialsData(symbol='aapl:us', output_type='df')
 
 
 GitHub Examples
 ----------------------------------------
 
 You can find additional examples and usage instructions in the GitHub repository:
- - https://github.com/tradingeconomics/tradingeconomics/tree/master/python
+ - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
 
 
 Documentation
 ----------------------------------------
 
 For detailed documentation and API reference, please visit the Trading Economics API documentation:
  - https://docs.tradingeconomics.com
```

### Comparing `tradingeconomics-4.2.5/setup.py` & `tradingeconomics-4.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     this_directory = path.abspath(path.dirname(__file__))
     with io.open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
       return f.read()
 
 setup(
   name = 'tradingeconomics',
   packages = find_packages(exclude=['tests*']),  
-  version = '4.2.5',
+  version = '4.2.6',
   description = 'Trading Economics API',
   long_description =readme(),
   long_description_content_type='text/x-rst',
   author = 'Trading Economics',
   author_email = 'support@tradingeconomics.com',
   license = 'MIT',
   url = 'https://github.com/tradingeconomics/tradingeconomics-python',
```

### Comparing `tradingeconomics-4.2.5/tradingeconomics/__init__.py` & `tradingeconomics-4.2.6/tradingeconomics/__init__.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/calendar.py` & `tradingeconomics-4.2.6/tradingeconomics/calendar.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/comtrade.py` & `tradingeconomics-4.2.6/tradingeconomics/comtrade.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/earnings.py` & `tradingeconomics-4.2.6/tradingeconomics/earnings.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/eurostat.py` & `tradingeconomics-4.2.6/tradingeconomics/eurostat.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/federalReserve.py` & `tradingeconomics-4.2.6/tradingeconomics/federalReserve.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/financials.py` & `tradingeconomics-4.2.6/tradingeconomics/financials.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/forecasts.py` & `tradingeconomics-4.2.6/tradingeconomics/forecasts.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/functions.py` & `tradingeconomics-4.2.6/tradingeconomics/functions.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/glob.py` & `tradingeconomics-4.2.6/tradingeconomics/glob.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/historical.py` & `tradingeconomics-4.2.6/tradingeconomics/historical.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/historicalDB.py` & `tradingeconomics-4.2.6/tradingeconomics/historicalDB.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/historicalEurostat.py` & `tradingeconomics-4.2.6/tradingeconomics/historicalEurostat.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/historicalFinancials.py` & `tradingeconomics-4.2.6/tradingeconomics/historicalFinancials.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/historicalMarkets.py` & `tradingeconomics-4.2.6/tradingeconomics/historicalMarkets.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/indicators.py` & `tradingeconomics-4.2.6/tradingeconomics/indicators.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/markets.py` & `tradingeconomics-4.2.6/tradingeconomics/markets.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/news.py` & `tradingeconomics-4.2.6/tradingeconomics/news.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/search.py` & `tradingeconomics-4.2.6/tradingeconomics/search.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/stream.py` & `tradingeconomics-4.2.6/tradingeconomics/stream.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics/worldBank.py` & `tradingeconomics-4.2.6/tradingeconomics/worldBank.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.5/tradingeconomics.egg-info/PKG-INFO` & `tradingeconomics-4.2.6/tradingeconomics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingeconomics
-Version: 4.2.5
+Version: 4.2.6
 Summary: Trading Economics API
 Home-page: https://github.com/tradingeconomics/tradingeconomics-python
 Author: Trading Economics
 Author-email: support@tradingeconomics.com
 License: MIT
 Download-URL: https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist
 Description: =====================
@@ -43,15 +43,15 @@
             - te.getFinancialsData(symbol='aapl:us', output_type='df')
         
         
         GitHub Examples
         ----------------------------------------
         
         You can find additional examples and usage instructions in the GitHub repository:
-         - https://github.com/tradingeconomics/tradingeconomics/tree/master/python
+         - https://github.com/tradingeconomics/tradingeconomics-python/tree/main/examples
         
         
         Documentation
         ----------------------------------------
         
         For detailed documentation and API reference, please visit the Trading Economics API documentation:
          - https://docs.tradingeconomics.com
```

### Comparing `tradingeconomics-4.2.5/tradingeconomics.egg-info/SOURCES.txt` & `tradingeconomics-4.2.6/tradingeconomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

