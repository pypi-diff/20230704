# Comparing `tmp/tradingeconomics-4.2.6.tar.gz` & `tmp/tradingeconomics-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingeconomics-4.2.6.tar", last modified: Tue Jul  4 08:58:42 2023, max compression
+gzip compressed data, was "tradingeconomics-4.2.7.tar", last modified: Tue Jul  4 10:33:03 2023, max compression
```

## Comparing `tradingeconomics-4.2.6.tar` & `tradingeconomics-4.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:58:42.126787 tradingeconomics-4.2.6/
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       18 2021-08-04 09:35:15.000000 tradingeconomics-4.2.6/MANIFEST.in
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2719 2023-07-04 08:58:42.127793 tradingeconomics-4.2.6/PKG-INFO
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1708 2023-07-04 08:56:55.000000 tradingeconomics-4.2.6/README.rst
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       79 2023-07-04 08:58:42.128794 tradingeconomics-4.2.6/setup.cfg
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1157 2023-07-04 08:57:28.000000 tradingeconomics-4.2.6/setup.py
-drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:58:42.116748 tradingeconomics-4.2.6/tradingeconomics/
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     3627 2023-03-30 12:04:47.000000 tradingeconomics-4.2.6/tradingeconomics/__init__.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    10861 2023-03-02 09:48:16.000000 tradingeconomics-4.2.6/tradingeconomics/calendar.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    16631 2023-03-30 12:04:47.000000 tradingeconomics-4.2.6/tradingeconomics/comtrade.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4113 2023-05-22 15:34:38.000000 tradingeconomics-4.2.6/tradingeconomics/earnings.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     7002 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/eurostat.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    12372 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/federalReserve.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     5532 2023-03-30 12:04:47.000000 tradingeconomics-4.2.6/tradingeconomics/financials.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     5244 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/forecasts.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     8630 2023-05-22 15:34:38.000000 tradingeconomics-4.2.6/tradingeconomics/functions.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1234 2023-03-02 09:48:16.000000 tradingeconomics-4.2.6/tradingeconomics/glob.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    13237 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/historical.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4509 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/historicalDB.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     3073 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/historicalEurostat.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2702 2023-03-02 09:48:16.000000 tradingeconomics-4.2.6/tradingeconomics/historicalFinancials.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4185 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/historicalMarkets.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    16263 2023-03-23 08:22:30.000000 tradingeconomics-4.2.6/tradingeconomics/indicators.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    22232 2023-03-30 12:04:47.000000 tradingeconomics-4.2.6/tradingeconomics/markets.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    13802 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/news.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2149 2021-09-21 08:26:38.000000 tradingeconomics-4.2.6/tradingeconomics/search.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1969 2022-08-29 11:34:45.000000 tradingeconomics-4.2.6/tradingeconomics/stream.py
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     9449 2022-09-27 08:00:02.000000 tradingeconomics-4.2.6/tradingeconomics/worldBank.py
-drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 08:58:42.125282 tradingeconomics-4.2.6/tradingeconomics.egg-info/
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2719 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/PKG-INFO
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)      886 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/SOURCES.txt
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        1 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/dependency_links.txt
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       24 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/requires.txt
--rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       17 2023-07-04 08:58:42.000000 tradingeconomics-4.2.6/tradingeconomics.egg-info/top_level.txt
+drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 10:33:03.300051 tradingeconomics-4.2.7/
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       18 2021-08-04 09:35:15.000000 tradingeconomics-4.2.7/MANIFEST.in
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2719 2023-07-04 10:33:03.300051 tradingeconomics-4.2.7/PKG-INFO
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1708 2023-07-04 08:56:55.000000 tradingeconomics-4.2.7/README.rst
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       79 2023-07-04 10:33:03.301057 tradingeconomics-4.2.7/setup.cfg
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1157 2023-07-04 10:32:31.000000 tradingeconomics-4.2.7/setup.py
+drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 10:33:03.289980 tradingeconomics-4.2.7/tradingeconomics/
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     3639 2023-07-04 10:29:47.000000 tradingeconomics-4.2.7/tradingeconomics/__init__.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    10861 2023-03-02 09:48:16.000000 tradingeconomics-4.2.7/tradingeconomics/calendar.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    16631 2023-03-30 12:04:47.000000 tradingeconomics-4.2.7/tradingeconomics/comtrade.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4395 2023-07-04 10:29:47.000000 tradingeconomics-4.2.7/tradingeconomics/earnings.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     7002 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/eurostat.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    12372 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/federalReserve.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     6398 2023-07-04 10:29:47.000000 tradingeconomics-4.2.7/tradingeconomics/financials.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     5244 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/forecasts.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     8933 2023-07-04 10:29:47.000000 tradingeconomics-4.2.7/tradingeconomics/functions.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1234 2023-03-02 09:48:16.000000 tradingeconomics-4.2.7/tradingeconomics/glob.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    13237 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/historical.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4509 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/historicalDB.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     3073 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/historicalEurostat.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2702 2023-03-02 09:48:16.000000 tradingeconomics-4.2.7/tradingeconomics/historicalFinancials.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     4185 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/historicalMarkets.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    16263 2023-03-23 08:22:30.000000 tradingeconomics-4.2.7/tradingeconomics/indicators.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    22232 2023-03-30 12:04:47.000000 tradingeconomics-4.2.7/tradingeconomics/markets.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)    13802 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/news.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2149 2021-09-21 08:26:38.000000 tradingeconomics-4.2.7/tradingeconomics/search.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     1969 2022-08-29 11:34:45.000000 tradingeconomics-4.2.7/tradingeconomics/stream.py
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     9449 2022-09-27 08:00:02.000000 tradingeconomics-4.2.7/tradingeconomics/worldBank.py
+drwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        0 2023-07-04 10:33:03.298543 tradingeconomics-4.2.7/tradingeconomics.egg-info/
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)     2719 2023-07-04 10:33:03.000000 tradingeconomics-4.2.7/tradingeconomics.egg-info/PKG-INFO
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)      886 2023-07-04 10:33:03.000000 tradingeconomics-4.2.7/tradingeconomics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)        1 2023-07-04 10:33:03.000000 tradingeconomics-4.2.7/tradingeconomics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       24 2023-07-04 10:33:03.000000 tradingeconomics-4.2.7/tradingeconomics.egg-info/requires.txt
+-rwxrwxrwx   0 fguerreiro  (1000) fguerreiro  (1000)       17 2023-07-04 10:33:03.000000 tradingeconomics-4.2.7/tradingeconomics.egg-info/top_level.txt
```

### Comparing `tradingeconomics-4.2.6/PKG-INFO` & `tradingeconomics-4.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingeconomics
-Version: 4.2.6
+Version: 4.2.7
 Summary: Trading Economics API
 Home-page: https://github.com/tradingeconomics/tradingeconomics-python
 Author: Trading Economics
 Author-email: support@tradingeconomics.com
 License: MIT
 Download-URL: https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist
 Description: =====================
```

### Comparing `tradingeconomics-4.2.6/README.rst` & `tradingeconomics-4.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/setup.py` & `tradingeconomics-4.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     this_directory = path.abspath(path.dirname(__file__))
     with io.open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
       return f.read()
 
 setup(
   name = 'tradingeconomics',
   packages = find_packages(exclude=['tests*']),  
-  version = '4.2.6',
+  version = '4.2.7',
   description = 'Trading Economics API',
   long_description =readme(),
   long_description_content_type='text/x-rst',
   author = 'Trading Economics',
   author_email = 'support@tradingeconomics.com',
   license = 'MIT',
   url = 'https://github.com/tradingeconomics/tradingeconomics-python',
```

### Comparing `tradingeconomics-4.2.6/tradingeconomics/__init__.py` & `tradingeconomics-4.2.7/tradingeconomics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from .earnings import getEarnings, getEarningsType
     from .news import getNews, getArticles, getArticleId 
     from .worldBank import getWBCategories, getWBIndicator, getWBCountry, getWBHistorical
     from .comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType, getCmtSnapshotByType
     from .federalReserve import getFedRStates, getFedRSnaps, getFedRHistorical, getFedRCounty
     from .eurostat import getEurostatData,getEurostatCountries,getEurostatCategoryGroups
     from .historicalEurostat import getHistoricalEurostat
-    from .financials import getFinancialsData, getFinancialsCategoryList, getFinancialsDataByCategory
+    from .financials import getFinancialsData, getFinancialsCategoryList, getFinancialsDataByCategory, getSectors
     from .historicalFinancials import getFinancialsHistorical
     from .search import getSearch
 
 
 else: # Python 2.X
     from historicalDB import getHistorical
     from historical import getHistoricalData, getHistoricalRatings,getHistoricalByTicker
```

### Comparing `tradingeconomics-4.2.6/tradingeconomics/calendar.py` & `tradingeconomics-4.2.7/tradingeconomics/calendar.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/comtrade.py` & `tradingeconomics-4.2.7/tradingeconomics/comtrade.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/earnings.py` & `tradingeconomics-4.2.7/tradingeconomics/historicalDB.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,137 @@
-import json 
+import json
+import itertools
 import urllib 
 import pandas as pd
 import sys
 from datetime import *
+from dateutil.relativedelta import relativedelta
+from . import functions as fn
 from . import glob
 import ssl
-from . import functions as fn
-from dateutil.relativedelta import relativedelta
-import time
 
 PY3 = sys.version_info[0] == 3
 
 if PY3: # Python 3+
     from urllib.request import urlopen
     from urllib.parse import quote
 else: # Python 2.X
     from urllib import urlopen
     from urllib import quote
 
-
 class ParametersError(ValueError):
     pass
 
-class CredentialsError(ValueError):
+class DateError(ValueError):
     pass
 
-class LoginError(AttributeError):
+class CredentialsError(ValueError):
     pass
 
-class DateError(ValueError):
+class LoginError(AttributeError):
     pass
 
 class WebRequestError(ValueError):
     pass
 
-def getEarnings(symbols=None, country=None, initDate=None, endDate=None, output_type=None):
-    """
-    Returns earnings calendar data.
-    ==========================================================
 
+
+def getHistorical(symbol = None, initDate = None, endDate = None, output_type = None, *args): 
+    """
+    Return historical information for specific symbol.
+    =================================================================
     Parameters:
     -----------
-    symbols: string or list.
-             String to get data for symbol. List of strings to get data for
-             several symbols.
-    
-    country: string or list.
-             String to get data for a specific country. List of strings to get data for
-             several countries.
-
-    initDate: string with format: YYYY-MM-DD.
-             For example: '2011-01-01' 
-
-    endDate: string with format: YYYY-MM-DD.
-
+    symbol: string or list.
+             String to get data for one symbol. List of strings to get data for
+             several symbols. 
+            
     output_type: string.
-             ''dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.  
-
+             'dict'(default) for dictionary format output,
+             'raw' for list of dictionaries without any parsing.
+    Notes
+    ----- 
+    Must put symbol and type of data.
     Example
     -------
-    getEarnings(symbols = 'msft:us', initDate='2016-01-01', endDate='2017-12-31')
-    getEarnings(country = 'united states')
+    te.getHistorical("indu:ind", '2015-01-01')
+    te.getHistorical("indu:ind", '2015-01-01', '2017-01-01' )
+    te.getHistorical("USURTOT", '2015-01-01')
+    te.getHistorical(['aapl:us', 'indu:ind'])
+    te.getHistorical("USURTOT")
+    te.getHistorical("aapl:us")
+    te.getHistorical("are.fr.inr.rinr:worldbank")
+    te.getHistorical("RACEDISPARITY005007:fred")
+    te.getHistorical("PRTESP24031:comtrade")
     """
+    linkAPI = 'https://api.tradingeconomics.com/'
+ 
     try:
         _create_unverified_https_context = ssl._create_unverified_context
     except AttributeError:
         pass
     else:
         ssl._create_default_https_context = _create_unverified_https_context
+
+    if (symbol[-10:] == ':worldbank'):  
+        linkAPI += 'worldBank/historical?' + 's=' + quote(symbol[:-10], safe=':') 
         
+    elif (symbol[-9:] == ':comtrade'):    
+        linkAPI += 'comtrade/historical/' +  quote(symbol[:-9], safe=':')  
     
-    # linkAPI = 'https://api.tradingeconomics.com/earnings/' 
-    linkAPI = 'https://api.tradingeconomics.com/earnings-revenues'
-    if symbols:
-        linkAPI += '/symbol/'
-        if type(symbols) is not str:
-            linkAPI += quote(",".join(symbols), safe='')
-        else:
-            linkAPI += quote(symbols)
-    elif country:
-        linkAPI += '/country/'
-        if type(country) is not str:
-            linkAPI += quote(",".join(country), safe='')
+    elif (symbol[-5:] == ':fred'):
+        linkAPI += 'fred/historical/' + quote(symbol[:-5], safe=':')          
+    
+    elif(':' not in symbol and type(symbol) is str):
+        linkAPI += 'historical/ticker/' + quote(symbol, safe='')
+                
+    elif (':' in symbol): 
+        linkAPI += 'markets/historical/' + quote(symbol, safe='') 
+    else:
+        linkAPI += 'markets/historical/' + quote(','.join(symbol), safe='')     
+    
+    if (initDate is not None) and (endDate is not None):
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try: 
+            fn.validate(endDate)
+        except ValueError:
+            raise DateError ('Incorrect endDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+        try:        
+            fn.validatePeriod(initDate, endDate)
+        except ValueError:
+            raise DateError ('Invalid time period.')
+        linkAPI += '?d1=' + initDate + '&d2=' + endDate
+    
+    if (initDate is not None) and endDate == None :        
+        try: 
+            fn.validate(initDate)
+        except ValueError:
+            raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
+            if initDate > str(date.today()):
+                raise DateError ('Initial date out of range.')
+        if('markets' in linkAPI):
+            linkAPI += '?d1=' + initDate
         else:
-            linkAPI += quote(country)
-    try:
-        linkAPI += '?c=' + glob.apikey
-    except AttributeError:
-        raise LoginError('You need to do login before making any request')
+            linkAPI += '/' + initDate
         
-    linkAPI = fn.checkDates(linkAPI, initDate, endDate)
-    #print(linkAPI)
-    try:
-        #print(linkAPI)
-        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
-    except Exception as e:
-        print(e)
-
+    if initDate == None and (endDate is not None):
+        initDate = (datetime.strptime(endDate, '%Y-%m-%d') - relativedelta(months=1)).strftime('%Y-%m-%d')
+        linkAPI += '?d1=' + initDate + '&d2=' + endDate
 
-def getEarningsType(type=None, output_type=None):
-    """
-    Returns earnings by type.
-    ==========================================================
-
-    Parameters:
-    -----------
-    type: string or list.
-             String to get data by type.
-             Type can be: earnings, ipo and dividends.
-
-    output_type: string.
-             'dict'(default) for dictionary format output, 'df' for data frame,
-             'raw' for list of dictionaries directly from the web.  
-
-    Example
-    -------
-    getEarningsType(type = 'ipo')
-    """
     try:
-        _create_unverified_https_context = ssl._create_unverified_context
-    except AttributeError:
-        pass
-    else:
-        ssl._create_default_https_context = _create_unverified_https_context
+        if ('?' in linkAPI):
+            linkAPI += '&c='+glob.apikey 
+        else:   
+            linkAPI += '?c='+glob.apikey
         
-    
-    linkAPI = 'https://api.tradingeconomics.com/earnings?type=' 
-    if type:
-        linkAPI += quote((type), safe='')  
-    try:
-        linkAPI += '&c=' + glob.apikey
-      
     except AttributeError:
         raise LoginError('You need to do login before making any request')
-    #print(linkAPI) 
     try:
         #print(linkAPI)
         return fn.dataRequest(api_request=linkAPI, output_type=output_type)
     except Exception as e:
-        print(e)
+        print(e) 
+            
+
```

### Comparing `tradingeconomics-4.2.6/tradingeconomics/eurostat.py` & `tradingeconomics-4.2.7/tradingeconomics/eurostat.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/federalReserve.py` & `tradingeconomics-4.2.7/tradingeconomics/federalReserve.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/financials.py` & `tradingeconomics-4.2.7/tradingeconomics/financials.py`

 * *Files 10% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     api_url_request = "%s%s" % (d['url_base'], d['key'])
 
     return fn.dataRequest(api_request=api_url_request, output_type=output_type)
 
 
 
 def getFinancialsDataByCategory(category=None, output_type=None):
+
     """
     Returns financial data by categories.
     ==========================================================
 
     Parameters:
     -----------
     category: string or list.
@@ -171,8 +172,42 @@
         d['category'] = f'/{category}'
     else:
         return 'No category supplied'
 
 
     api_url_request = "%s%s%s" % (d['url_base'], d['category'], d['key'])
 
-    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+    return fn.dataRequest(api_request=api_url_request, output_type=output_type)
+
+
+def getSectors(output_type=None):
+    """
+    Returns all sectors.
+    ==========================================================
+
+    Parameters:
+    -----------
+
+    output_type: string.
+             'dict'(default) for dictionary format output, 'df' for data frame,
+             'raw' for list of dictionaries directly from the web. 
+    
+    Example
+    -------
+    Get data by financial categories:
+            getSectors()
+
+    """
+
+    linkAPI = 'https://api.tradingeconomics.com/sectors/'
+
+    try:
+        linkAPI += '?c=' + glob.apikey
+    except AttributeError:
+        raise LoginError('You need to do login before making any request')
+        
+    linkAPI = fn.checkDates(linkAPI)
+    
+    try:
+        return fn.dataRequest(api_request=linkAPI, output_type=output_type)
+    except Exception as e:
+        print(e)
```

### Comparing `tradingeconomics-4.2.6/tradingeconomics/forecasts.py` & `tradingeconomics-4.2.7/tradingeconomics/forecasts.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/functions.py` & `tradingeconomics-4.2.7/tradingeconomics/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -227,8 +227,17 @@
             validatePeriod(initDate, endDate)
         except ValueError:
             raise DateError ('Invalid time period.')
         baseLink += '&d1=' + quote(initDate) + '&d2=' + quote(endDate)
 
     if initDate == None and (endDate is not None):
         raise DateError('initDate value is missing')
-    return baseLink
+    return baseLink
+
+
+def isStringOrList(string_or_list):
+    if type(string_or_list) is str:
+        return quote(string_or_list)
+    elif type(string_or_list) is list:
+        return quote(",".join(string_or_list))
+    else:
+        raise ValueError('Invalid input type. Should be string or list of strings.')
```

### Comparing `tradingeconomics-4.2.6/tradingeconomics/glob.py` & `tradingeconomics-4.2.7/tradingeconomics/glob.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/historical.py` & `tradingeconomics-4.2.7/tradingeconomics/historical.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/historicalEurostat.py` & `tradingeconomics-4.2.7/tradingeconomics/historicalEurostat.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/historicalFinancials.py` & `tradingeconomics-4.2.7/tradingeconomics/historicalFinancials.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/historicalMarkets.py` & `tradingeconomics-4.2.7/tradingeconomics/historicalMarkets.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/indicators.py` & `tradingeconomics-4.2.7/tradingeconomics/indicators.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/markets.py` & `tradingeconomics-4.2.7/tradingeconomics/markets.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/news.py` & `tradingeconomics-4.2.7/tradingeconomics/news.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/search.py` & `tradingeconomics-4.2.7/tradingeconomics/search.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/stream.py` & `tradingeconomics-4.2.7/tradingeconomics/stream.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics/worldBank.py` & `tradingeconomics-4.2.7/tradingeconomics/worldBank.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.6/tradingeconomics.egg-info/PKG-INFO` & `tradingeconomics-4.2.7/tradingeconomics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingeconomics
-Version: 4.2.6
+Version: 4.2.7
 Summary: Trading Economics API
 Home-page: https://github.com/tradingeconomics/tradingeconomics-python
 Author: Trading Economics
 Author-email: support@tradingeconomics.com
 License: MIT
 Download-URL: https://github.com/tradingeconomics/tradingeconomics-python/tree/main/dist
 Description: =====================
```

### Comparing `tradingeconomics-4.2.6/tradingeconomics.egg-info/SOURCES.txt` & `tradingeconomics-4.2.7/tradingeconomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

