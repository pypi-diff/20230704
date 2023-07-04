# Comparing `tmp/investlib-0.0.3.tar.gz` & `tmp/investlib-0.0.4.tar.gz`

## Comparing `investlib-0.0.3.tar` & `investlib-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,18 @@
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 investlib-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/__init__.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/backtest.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/core.py
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/data.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/download.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/draw.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/filters.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/portfolio.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/rebalance.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/spydiffeqw.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/spystdreb.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0    13283 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/test_data.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/test_filters.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/test_rebalance.py
--rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/test_strategy.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 investlib-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 investlib-0.0.3/LICENSE
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 investlib-0.0.3/README.md
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 investlib-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 investlib-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 investlib-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/__init__.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/data.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/filters.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/rebalance.py
+-rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/strategy.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    13283 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_data.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_filters.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_rebalance.py
+-rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_strategy.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_utils.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 investlib-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 investlib-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 investlib-0.0.4/README.md
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 investlib-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 investlib-0.0.4/PKG-INFO
```

### Comparing `investlib-0.0.3/investlib/data.py` & `investlib-0.0.4/investlib/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
         if end:
             df=df.loc[:end]
         
         buffer.close()
         return df
 
     def load(self, tickers, start=None, end=None):
+        if not os.path.exists(self.backup_path):
+            os.makedirs(self.backup_path)
+
         end = self.fix_end(end)
 
         if(start and start>end):
             raise Exception('Start date must be greater than end date')  
         series = [] 
         
         for ticker in tickers:
```

### Comparing `investlib-0.0.3/investlib/filters.py` & `investlib-0.0.4/investlib/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import calendar
 import pandas as pd
+from investlib.utils import get_interval_by_month
 
 class BaseFilter:
     def __init__(self, days=None, months=None, gt=None, gte=None, lt=None, lte=None, best=None):
         params = [gt, gte, lt, lte, best]
         check = sum(param != None for param in params)
         if check != 1:
             raise Exception('Choose one and only one conditions: gt,gte,lt,lte')
@@ -15,31 +16,19 @@
         self.months=months
         self.gt=gt
         self.gte=gte
         self.lt=lt
         self.lte=lte
         self.best=best
 
-    def get_interval(self, date):
-        start_month = date - pd.DateOffset(months=self.months)
-        first_day = start_month
-        if not first_day.is_month_start:
-            first_day = start_month - pd.offsets.MonthBegin()
-        
-        last_day = date - pd.DateOffset(months=1)
-        if not last_day.is_month_end:
-            last_day += pd.offsets.MonthEnd(0)
-        
-        return (first_day, last_day)
-
 class PctChange(BaseFilter):
     
     def get_filtered(self, equities, date):
         if self.months != None:
-            first_day, last_day = self.get_interval(date)
+            first_day, last_day = get_interval_by_month(date, self.months)
             filtered = (equities.loc[last_day]/equities.loc[first_day]-1).dropna()
         else:
             filtered = equities.pct_change(periods=self.days).loc[date].dropna()
 
         if self.gt is not None:
             filtered = filtered[filtered>self.gt]
         if self.gte is not None:
```

### Comparing `investlib-0.0.3/investlib/strategy.py` & `investlib-0.0.4/investlib/strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,7 +95,9 @@
                 quantity = (capital_to_use/current_close).fillna(0).round(2).apply(math.floor)
                 self.quantity.loc[i, :] += quantity
                 #self.quantity.loc[i, pos_asset] += (capital_to_use/current_close).apply(math.floor)
                 self.invested.loc[i, (slice(None), 'current')] = history.loc[i].xs('close',  level=1).mul(quantity).tolist()
                 self.invested.loc[i, (slice(None), 'value')] = self.quantity.loc[i,:].mul(history.loc[i].xs('close',  level=1)).tolist()
 
             self.cash.loc[i, 'post_close'] = self.cash.loc[i, 'pre_close']-self.invested.loc[i, (slice(None), 'current')].sum()
+        
+        self.equity = self.invested.loc[:, (slice(None), 'value')].droplevel(1, axis=1).sum(axis=1) + self.cash['post_close']
```

### Comparing `investlib-0.0.3/tests/test_data.py` & `investlib-0.0.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.3/tests/test_filters.py` & `investlib-0.0.4/tests/test_filters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,14 @@
 import pandas as pd
 import os
 import unittest
 from investlib.filters import PctChange, SharpRatio, BaseFilter
 
 
 class BaseFilterTest(unittest.TestCase):
-    def test_get_interval_middle_month_day(self):
-        f = BaseFilter(days=30, months=3, gt=0)
-        first, last = f.get_interval(pd.to_datetime('2022-05-03'))
-        self.assertEqual(first.date().__str__(), '2022-02-01')
-        self.assertEqual(last.date().__str__(), '2022-04-30')
-
-    def test_get_interval_last_month_day(self):
-        f = BaseFilter(days=30, months=3, gt=0)
-        first, last = f.get_interval(pd.to_datetime('2022-05-31'))
-        self.assertEqual(first.date().__str__(), '2022-02-01')
-        self.assertEqual(last.date().__str__(), '2022-04-30')
-
-    def test_get_interval_first_month_day(self):
-        f = BaseFilter(days=30, months=3, gt=0)
-        first, last = f.get_interval(pd.to_datetime('2022-05-01'))
-        self.assertEqual(first.date().__str__(), '2022-02-01')
-        self.assertEqual(last.date().__str__(), '2022-04-30')
 
     def test_month_or_day_mandatory(self):
         self.assertRaises(Exception, BaseFilter, **dict(gt=0))
 
 
 class PctChangeTest(unittest.TestCase):
```

### Comparing `investlib-0.0.3/tests/test_strategy.py` & `investlib-0.0.4/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.3/.gitignore` & `investlib-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `investlib-0.0.3/LICENSE` & `investlib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `investlib-0.0.3/README.md` & `investlib-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     - Percentage variation in month/days
     - Sharpe ratio (assuming risk-free rate as zero)
 ### Allocations
 You can allocate percentages between the chosen ETFs using:
 	- Fixed allocation
 		- Statically
 		- Dinamically based on the number of filtered ETFs
+    - PctChangeRank
+        Allow you to make a ranking on filtered ETF and allocate money based on your preference
 
 ## Data
 The current unique data source is Tiingo. InvestLib automatically manages cash to avoid making repeated data calls. To use this feature, you need to create a free account on Tiingo and set the following environment variables:
 
 - **tiingo_api_key**: the API token provided by Tiingo upon subscription
 - **tiingo_backup_path**: the folder where you want to save the end-of-day CSV data for all the ETFs you need (default '/tmp/Tiingo'). 
 
@@ -45,26 +47,30 @@
     
     start = '2007-01-01'
     end = '2021-06-04'
     tickers = ['VTI', 'IEF']
     
     # We create a strategy that rebalances the current money (invested + cash) to 60% VTI and 40% IEF
     # every month on the first Friday.
-    s = Strategy(tickers, start=start, end=end, timer=MonthlyTimer(months=1, day=FirstFriday()),allocation_class=FixedAllocation({'VTI':0.6,'IEF':0.4}))
+    s = Strategy(
+        tickers, 
+        start=start, 
+        end=end, 
+        timer=MonthlyTimer(months=1, day=FirstFriday()),
+        allocation_class=FixedAllocation({'VTI':0.6,'IEF':0.4})
+    )
     s.run()
-    # Build the final equity by summing up the value of investments per asset and the remaining cash
-    eq = s.invested.loc[:, (slice(None), 'value')].droplevel(1, axis=1).sum(axis=1) + s.cash['post_close']
-    
+   
     # Plot the results
     fig = go.Figure()
-    fig.add_trace(go.Scatter(x=s.invested.index, y=eq, name='6040', yaxis='y1'))
-    fig.add_trace(go.Scatter(x=bench.invested.index, y=bench_eq, name='VTI', yaxis='y1'))
-    fig.update_layout(
-        yaxis2=dict(
-            title='Dati 2',
-            overlaying='y',
-            side='right'
-        )
-    )
+    fig.add_trace(go.Scatter(x=s.invested.index, y=s.equity, name='6040'))
+    fig.add_trace(go.Scatter(x=bench.invested.index, y=bench_eq, name='VTI'))
+
     fig.show()
 
     
+### Futures 
+    - Add more stats
+    - Currency
+    - Tax
+    - Portfolio over Strategy
+
```

### Comparing `investlib-0.0.3/pyproject.toml` & `investlib-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "investlib"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Cellarosi Marco", email="cellarosi@gmail.com" },
 ]
 description = "InvestLib is a Python package for backtesting ETF investments"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `investlib-0.0.3/PKG-INFO` & `investlib-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investlib
-Version: 0.0.3
+Version: 0.0.4
 Summary: InvestLib is a Python package for backtesting ETF investments
 Project-URL: Homepage, https://github.com/cellarosi/investlib
 Project-URL: Bug Tracker, https://github.com/cellarosi/investlib/issues
 Author-email: Cellarosi Marco <cellarosi@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -42,14 +42,16 @@
     - Percentage variation in month/days
     - Sharpe ratio (assuming risk-free rate as zero)
 ### Allocations
 You can allocate percentages between the chosen ETFs using:
 	- Fixed allocation
 		- Statically
 		- Dinamically based on the number of filtered ETFs
+    - PctChangeRank
+        Allow you to make a ranking on filtered ETF and allocate money based on your preference
 
 ## Data
 The current unique data source is Tiingo. InvestLib automatically manages cash to avoid making repeated data calls. To use this feature, you need to create a free account on Tiingo and set the following environment variables:
 
 - **tiingo_api_key**: the API token provided by Tiingo upon subscription
 - **tiingo_backup_path**: the folder where you want to save the end-of-day CSV data for all the ETFs you need (default '/tmp/Tiingo'). 
 
@@ -72,26 +74,30 @@
     
     start = '2007-01-01'
     end = '2021-06-04'
     tickers = ['VTI', 'IEF']
     
     # We create a strategy that rebalances the current money (invested + cash) to 60% VTI and 40% IEF
     # every month on the first Friday.
-    s = Strategy(tickers, start=start, end=end, timer=MonthlyTimer(months=1, day=FirstFriday()),allocation_class=FixedAllocation({'VTI':0.6,'IEF':0.4}))
+    s = Strategy(
+        tickers, 
+        start=start, 
+        end=end, 
+        timer=MonthlyTimer(months=1, day=FirstFriday()),
+        allocation_class=FixedAllocation({'VTI':0.6,'IEF':0.4})
+    )
     s.run()
-    # Build the final equity by summing up the value of investments per asset and the remaining cash
-    eq = s.invested.loc[:, (slice(None), 'value')].droplevel(1, axis=1).sum(axis=1) + s.cash['post_close']
-    
+   
     # Plot the results
     fig = go.Figure()
-    fig.add_trace(go.Scatter(x=s.invested.index, y=eq, name='6040', yaxis='y1'))
-    fig.add_trace(go.Scatter(x=bench.invested.index, y=bench_eq, name='VTI', yaxis='y1'))
-    fig.update_layout(
-        yaxis2=dict(
-            title='Dati 2',
-            overlaying='y',
-            side='right'
-        )
-    )
+    fig.add_trace(go.Scatter(x=s.invested.index, y=s.equity, name='6040'))
+    fig.add_trace(go.Scatter(x=bench.invested.index, y=bench_eq, name='VTI'))
+
     fig.show()
 
     
+### Futures 
+    - Add more stats
+    - Currency
+    - Tax
+    - Portfolio over Strategy
+
```

