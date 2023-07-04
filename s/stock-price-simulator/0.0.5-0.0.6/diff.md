# Comparing `tmp/stock_price_simulator-0.0.5.tar.gz` & `tmp/stock_price_simulator-0.0.6.tar.gz`

## Comparing `stock_price_simulator-0.0.5.tar` & `stock_price_simulator-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/src/stock_price_simulator/__init__.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/src/stock_price_simulator/candle.py
--rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/src/stock_price_simulator/history.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/src/stock_price_simulator/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/src/stock_price_simulator/candle.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/src/stock_price_simulator/history.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/tests/stock_price_simulator/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/tests/stock_price_simulator/candle.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/README.md
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 stock_price_simulator-0.0.6/PKG-INFO
```

### Comparing `stock_price_simulator-0.0.5/src/stock_price_simulator/candle.py` & `stock_price_simulator-0.0.6/src/stock_price_simulator/candle.py`

 * *Files identical despite different names*

### Comparing `stock_price_simulator-0.0.5/src/stock_price_simulator/history.py` & `stock_price_simulator-0.0.6/src/stock_price_simulator/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import mplfinance as mpf
 import pandas as pd
 import random as rd
 
-from utils.candle import Candle
+from .candle import Candle
 
 class History:
     def __init__ (self, candles: list = []):
         self.candles = candles
         self.length = len(candles)
 
     def addCandle(self, candle: Candle):
```

### Comparing `stock_price_simulator-0.0.5/LICENSE` & `stock_price_simulator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stock_price_simulator-0.0.5/pyproject.toml` & `stock_price_simulator-0.0.6/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stock_price_simulator"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Cereal38", email="guillaume.bruncosmegazot@gmail.com" },
 ]
 description = "A stock price simulator"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
 dependencies = [
   "pandas>=2.0.3",
   "mplfinance>=0.12.9b7"
 ]
+test = [
+  "pytest-cov ~=3.0.0",
+]
 
 [project.urls]
-"Github" = "https://github.com/Cereal38/stock_price_simulator"
+"Github" = "https://github.com/Cereal38/stock_price_simulator"
+
+[tool.pytest.ini_options]
+addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 95"
+
+[tool.coverage.run]
+source = ["src"]
```

### Comparing `stock_price_simulator-0.0.5/PKG-INFO` & `stock_price_simulator-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock_price_simulator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A stock price simulator
 Project-URL: Github, https://github.com/Cereal38/stock_price_simulator
 Author-email: Cereal38 <guillaume.bruncosmegazot@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

