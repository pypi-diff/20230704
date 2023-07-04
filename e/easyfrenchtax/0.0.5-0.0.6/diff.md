# Comparing `tmp/easyfrenchtax-0.0.5.tar.gz` & `tmp/easyfrenchtax-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfrenchtax-0.0.5.tar", last modified: Thu Jun 29 16:04:20 2023, max compression
+gzip compressed data, was "easyfrenchtax-0.0.6.tar", last modified: Tue Jul  4 20:10:10 2023, max compression
```

## Comparing `easyfrenchtax-0.0.5.tar` & `easyfrenchtax-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.818938 easyfrenchtax-0.0.5/
--rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.5/LICENSE
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-06-29 16:04:20.819012 easyfrenchtax-0.0.5/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.5/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.5/pyproject.toml
--rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-06-29 16:04:20.819304 easyfrenchtax-0.0.5/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.815135 easyfrenchtax-0.0.5/src/
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.816553 easyfrenchtax-0.0.5/src/easyfrenchtax/
--rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.5/src/easyfrenchtax/__init__.py
--rw-r--r--   0 hadrien    (501) staff       (20)    19882 2023-06-29 16:02:58.000000 easyfrenchtax-0.0.5/src/easyfrenchtax/stock_helper.py
--rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.5/src/easyfrenchtax/tax_simulator.py
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.817365 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-06-29 16:04:20.000000 easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/top_level.txt
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-06-29 16:04:20.818693 easyfrenchtax-0.0.5/tests/
--rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.5/tests/test_capital_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.5/tests/test_fiscal_advantages.py
--rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.5/tests/test_income_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.5/tests/test_rental_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    12933 2023-06-29 16:00:34.000000 easyfrenchtax-0.0.5/tests/test_stock_helper.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.513974 easyfrenchtax-0.0.6/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.6/LICENSE
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-04 20:10:10.514038 easyfrenchtax-0.0.6/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.6/README.md
+-rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.6/pyproject.toml
+-rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-07-04 20:10:10.514293 easyfrenchtax-0.0.6/setup.cfg
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.510055 easyfrenchtax-0.0.6/src/
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.511287 easyfrenchtax-0.0.6/src/easyfrenchtax/
+-rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.6/src/easyfrenchtax/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    19593 2023-07-04 20:10:04.000000 easyfrenchtax-0.0.6/src/easyfrenchtax/stock_helper.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.6/src/easyfrenchtax/tax_simulator.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.512241 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/top_level.txt
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.513731 easyfrenchtax-0.0.6/tests/
+-rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.6/tests/test_capital_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.6/tests/test_fiscal_advantages.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.6/tests/test_income_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.6/tests/test_rental_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    12885 2023-07-04 20:09:13.000000 easyfrenchtax-0.0.6/tests/test_stock_helper.py
```

### Comparing `easyfrenchtax-0.0.5/LICENSE` & `easyfrenchtax-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.5/PKG-INFO` & `easyfrenchtax-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.5/README.md` & `easyfrenchtax-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.5/setup.cfg` & `easyfrenchtax-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyfrenchtax
-version = 0.0.5
+version = 0.0.6
 author = Hadrien Hamel
 author_email = hadrien.hamel@gmail.com
 license = MIT
 description = A simulator of French taxes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/had/easyfrenchtax
```

### Comparing `easyfrenchtax-0.0.5/src/easyfrenchtax/stock_helper.py` & `easyfrenchtax-0.0.6/src/easyfrenchtax/stock_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from collections import defaultdict
 import csv
 import glob
 
 
 @dataclass
 class StockGroup:
-    owner: int  # taxpayer 1 or 2, typically, for tax statements
     count: int
     available: int
     acq_price: float
     acq_price_eur: float
     acq_date: date
     plan_name: str
 
@@ -117,45 +116,42 @@
                 name=name,
                 approval_date=approval_date,
                 taxation_scheme=StockHelper._determine_rsu_plans_type(approval_date),
                 stock_symbol=symbol,
                 currency=currency
             )
 
-    def rsu_vesting(self, owner: int, symbol: str, plan_name: str, count: int, acq_date: date, acq_price: float,
+    def rsu_vesting(self, symbol: str, plan_name: str, count: int, acq_date: date, acq_price: float,
                     currency: str = None) -> None:
         if not currency:
             currency = self.rsu_plans[plan_name].currency
         self.rsus[symbol].append(StockGroup(
-            owner=owner,
             count=count,
             available=count,  # new acquisition, so everything available
             acq_price=acq_price,
             acq_price_eur=cc.convert(acq_price, currency, "EUR", date=acq_date),
             acq_date=acq_date,
             plan_name=plan_name
         ))
         self.rsus[symbol].sort(key=lambda a: a.acq_date)
 
-    def add_espp(self, owner: int, symbol: str, count: int, acq_date: date, acq_price: float, currency: str) -> None:
+    def add_espp(self, symbol: str, count: int, acq_date: date, acq_price: float, currency: str) -> None:
         self.espp_stocks[symbol].append(StockGroup(
-            owner=owner,
             count=count,
             available=count,  # new acquisition, so everything available
             acq_price=acq_price,
             acq_price_eur=cc.convert(acq_price, currency, "EUR", date=acq_date),
             acq_date=acq_date,
             plan_name="espp"
         ))
         self.espp_stocks[symbol].sort(key=lambda a: a.acq_date)
 
-    def add_stockoptions(self, owner: int, symbol: str, plan_name: str, count: int, vesting_date: date,
+    def add_stockoptions(self, symbol: str, plan_name: str, count: int, vesting_date: date,
                          strike_price: float, currency: str) -> None:
         self.stock_options[symbol].append(StockGroup(
-            owner=owner,
             count=count,
             available=count,  # new acquisition, so everything available
             acq_price=strike_price if currency != "EUR" else None,  # only set one of the two acquisition prices...
             acq_price_eur=strike_price if currency == "EUR" else None,
             # ...if conversion is needed, it will happen at sale time
             acq_date=vesting_date,
             plan_name=plan_name
@@ -173,36 +169,34 @@
         # read all files found in tsv_files (glob format)
         rsu_data = []
         for tsv_name in glob.glob(tsv_files):
             print("Opening ", tsv_name)
             with open(tsv_name) as tsv_file:
                 tsv_data = csv.DictReader(tsv_file, delimiter="\t")
                 for row in tsv_data:
-                    owner = int(row["Owner"])
-                    assert (owner == 1 or owner == 2)
                     plan_name = row["Plan name"]
                     stock_type = row["Stock type"]
                     currency = row["Currency"]
                     symbol = row["Symbol"]
                     acq_count = int(float(row["Count"].replace('\u202f', '')))
                     acq_price = float(row["Acquisition price"])
                     acq_date = parse_date(row["Acquisition date"])
                     if stock_type == "RSU":
                         if plan_name not in self.rsu_plans:
                             plan_date = parse_date(row["Plan date"])
                             self.rsu_plan(plan_name, plan_date, symbol, currency)
-                        self.rsu_vesting(owner, symbol, plan_name, acq_count, acq_date, acq_price, currency)
+                        self.rsu_vesting(symbol, plan_name, acq_count, acq_date, acq_price, currency)
                     elif stock_type == "ESPP":
-                        self.add_espp(owner, symbol, acq_count, acq_date, acq_price, currency)
+                        self.add_espp(symbol, acq_count, acq_date, acq_price, currency)
                     elif stock_type == "StockOption":
-                        self.add_stockoptions(owner, symbol, plan_name, acq_count, acq_date, acq_price, currency)
+                        self.add_stockoptions(symbol, plan_name, acq_count, acq_date, acq_price, currency)
 
     ####### stock selling related load functions #######
 
-    def sell_stockoptions(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
+    def sell_stockoptions(self, owner: int, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
                           currency: str = "EUR"):
         if nb_stocks == 0:
             return
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
         stocks_before_sell_date = [r for r in self.stock_options[symbol] if r.acq_date < sell_date]
         for i, acq in enumerate(stocks_before_sell_date):
@@ -215,15 +209,15 @@
                 symbol=symbol,
                 stock_type="stockoption",
                 nb_stocks_sold=sell_from_acq,
                 unit_acquisition_price=strike_price_eur,  # re-using this field to store the strike price
                 sell_date=sell_date,
                 sell_price_eur=sell_price_eur,
                 selling_fees=round(cc.convert(fees, currency, "EUR", date=sell_date), 2),
-                owner=acq.owner
+                owner=owner
             ))
             # update the stock options data with new availability
             self.stock_options[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
             if to_sell == 0:
                 break
         if to_sell > 0:
```

### Comparing `easyfrenchtax-0.0.5/src/easyfrenchtax/tax_simulator.py` & `easyfrenchtax-0.0.6/src/easyfrenchtax/tax_simulator.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.5/src/easyfrenchtax.egg-info/PKG-INFO` & `easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.5/tests/test_capital_tax.py` & `easyfrenchtax-0.0.6/tests/test_capital_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.5/tests/test_fiscal_advantages.py` & `easyfrenchtax-0.0.6/tests/test_fiscal_advantages.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.5/tests/test_income_tax.py` & `easyfrenchtax-0.0.6/tests/test_income_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.5/tests/test_rental_tax.py` & `easyfrenchtax-0.0.6/tests/test_rental_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.5/tests/test_stock_helper.py` & `easyfrenchtax-0.0.6/tests/test_stock_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 from currency_converter import CurrencyConverter
 
 
 @pytest.fixture
 def stock_helper_with_plan():
     stock_helper = StockHelper()
     stock_helper.rsu_plan("Cake1", date(2016, 6, 28), "CAKE", "USD")
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 240, date(2018, 6, 29), 20)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 7, 30), 18)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 8, 28), 19)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 9, 28), 14)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 10, 29), 15)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 11, 28), 14)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2018, 12, 28), 19)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2019, 1, 28), 23)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 10, date(2019, 2, 28), 24)
-    stock_helper.rsu_vesting(1, "CAKE", "Cake1", 100, date(2020, 2, 28), 24)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 240, date(2018, 6, 29), 20)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2018, 7, 30), 18)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2018, 8, 28), 19)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2018, 9, 28), 14)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2018, 10, 29), 15)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2018, 11, 28), 14)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2018, 12, 28), 19)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2019, 1, 28), 23)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2019, 2, 28), 24)
+    stock_helper.rsu_vesting("CAKE", "Cake1", 100, date(2020, 2, 28), 24)
     stock_helper.rsu_plan("Pineapple", date(2016, 6, 29), "PZZA", "USD")
-    stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 313, date(2020, 12, 28), 20.84)
-    stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 312, date(2021, 3, 28), 27.44)
-    stock_helper.rsu_vesting(1, "PZZA", "Pineapple", 313, date(2021, 6, 28), 37.25)
+    stock_helper.rsu_vesting("PZZA", "Pineapple", 313, date(2020, 12, 28), 20.84)
+    stock_helper.rsu_vesting("PZZA", "Pineapple", 312, date(2021, 3, 28), 27.44)
+    stock_helper.rsu_vesting("PZZA", "Pineapple", 313, date(2021, 6, 28), 37.25)
     stock_helper.rsu_plan("Pepperoni", date(2017, 7, 28), "PZZA", "USD")
-    stock_helper.rsu_vesting(1, "PZZA", "Pepperoni", 398, date(2020, 12, 16), 18.75)
-    stock_helper.rsu_vesting(1, "PZZA", "Pepperoni", 133, date(2021, 1, 26), 19.13)
-    stock_helper.add_espp(1, "BUD", 200, date(2019, 1, 15), 22, "USD")
-    stock_helper.add_espp(1, "BUD", 300, date(2019, 7, 15), 19, "USD")
-    stock_helper.add_stockoptions(1, "PZZA", "SO", 150, date(2018, 1, 15), 5, "USD")
+    stock_helper.rsu_vesting("PZZA", "Pepperoni", 398, date(2020, 12, 16), 18.75)
+    stock_helper.rsu_vesting("PZZA", "Pepperoni", 133, date(2021, 1, 26), 19.13)
+    stock_helper.add_espp("BUD", 200, date(2019, 1, 15), 22, "USD")
+    stock_helper.add_espp("BUD", 300, date(2019, 7, 15), 19, "USD")
+    stock_helper.add_stockoptions("PZZA", "SO", 150, date(2018, 1, 15), 5, "USD")
     return stock_helper
 
 
 @pytest.fixture
 def convert_fn() -> Callable[[float, str, str, date], float]:
     cc = CurrencyConverter(fallback_on_wrong_date=True)
     return cc.convert
@@ -137,16 +137,16 @@
     assert report_2074[2]['global_acquisition_cost_521'] == 2095
     assert report_2074[2]['global_selling_proceeds_516'] == 3462
     stock_helper_with_plan.helper_capital_gain_tax(report_cg)
 
 
 def test_espp_sale(convert_fn):
     stock_helper = StockHelper()
-    stock_helper.add_espp(1, "BUD", 200, date(2019, 1, 15), 22, "USD")
-    stock_helper.add_espp(1, "BUD", 300, date(2019, 7, 15), 19, "USD")
+    stock_helper.add_espp("BUD", 200, date(2019, 1, 15), 22, "USD")
+    stock_helper.add_espp("BUD", 300, date(2019, 7, 15), 19, "USD")
     sell_price = 28
     final_count = stock_helper.sell_espp("BUD", 300, date(2021, 8, 2), sell_price=sell_price, fees=0, currency="USD")
     assert final_count == 300
 
     report_ag = stock_helper.compute_acquisition_gain_tax(2021)
     assert not any(report_ag.values()), "ESPP should not yield acquisition gain (thus no acquisition gain tax)"
 
@@ -167,15 +167,15 @@
     )
     assert report_2042C["capital_gain_3VG"] == expected_capital_gain, \
         "Capital gain tax should be compliant"
 
 
 def test_stockoptions_sale(stock_helper_with_plan, convert_fn):
     sell_price = 40
-    final_count = stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=sell_price,
+    final_count = stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=sell_price,
                                                                     fees=0, currency="USD")
     agt = stock_helper_with_plan.compute_acquisition_gain_tax(2021)
     cgt = stock_helper_with_plan.compute_capital_gain_tax(2021)
 
     strike_price = stock_helper_with_plan.stock_options["PZZA"][0].acq_price
     assert final_count == 50
     ex_gain_usd = 50 * (sell_price - strike_price)
@@ -188,27 +188,27 @@
         "Stock options 'exercise and sell' should not yield capital gain (thus no capital gain tax)"
 
 
 def test_reset_all(stock_helper_with_plan):
     # CAKE=240 ; BUD=200 ; PZZA=150
     stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
+    stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.reset()
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
     assert len(stock_helper_with_plan.stock_sales[2021]) == 0
 
 
 def test_reset_by_stocktype(stock_helper_with_plan):
     # CAKE=240 ; BUD=200 ; PZZA=150
     stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
+    stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
     stock_helper_with_plan.reset(stock_types=["espp"])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
@@ -222,15 +222,15 @@
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
 
 
 def test_reset_by_symbol(stock_helper_with_plan):
     # CAKE=240 ; BUD=200 ; PZZA=150
     stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_stockoptions("PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
+    stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
     stock_helper_with_plan.reset(symbols=["CAKE", "PZZA"])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
```

