# Comparing `tmp/stock_price_simulator-0.0.3.tar.gz` & `tmp/stock_price_simulator-0.0.4.tar.gz`

## Comparing `stock_price_simulator-0.0.3.tar` & `stock_price_simulator-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/requirements.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/src/stock-price-simulator/__init__.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/src/stock-price-simulator/candle.py
--rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/src/stock-price-simulator/history.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/src/stock_price_simulator/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/src/stock_price_simulator/candle.py
+-rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/src/stock_price_simulator/history.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.4/PKG-INFO
```

### Comparing `stock_price_simulator-0.0.3/src/stock-price-simulator/candle.py` & `stock_price_simulator-0.0.4/src/stock_price_simulator/candle.py`

 * *Files identical despite different names*

### Comparing `stock_price_simulator-0.0.3/src/stock-price-simulator/history.py` & `stock_price_simulator-0.0.4/src/stock_price_simulator/history.py`

 * *Files identical despite different names*

### Comparing `stock_price_simulator-0.0.3/LICENSE` & `stock_price_simulator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stock_price_simulator-0.0.3/pyproject.toml` & `stock_price_simulator-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stock_price_simulator"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Cereal38", email="guillaume.bruncosmegazot@gmail.com" },
 ]
 description = "A stock price simulator"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

