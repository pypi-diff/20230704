# Comparing `tmp/martin_binance-1.3.2.post3.tar.gz` & `tmp/martin_binance-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-1.3.2.post3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-1.3.2.post3.tar` & `martin_binance-1.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1079 2023-07-02 16:21:19.194030 martin_binance-1.3.2.post3/LICENSE
--rwxr-xr-x   0        0        0     4025 2023-07-02 16:21:19.194030 martin_binance-1.3.2.post3/README.md
--rw-r--r--   0        0        0     2015 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/__init__.py
--rw-r--r--   0        0        0     4642 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2946 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    14575 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6721 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6716 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6722 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4707 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/client.py
--rw-r--r--   0        0        0   186162 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2023-07-02 16:21:19.242031 martin_binance-1.3.2.post3/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2023-07-02 16:21:19.242031 martin_binance-1.3.2.post3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2023-07-02 16:21:19.242031 martin_binance-1.3.2.post3/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-07-02 16:21:19.242031 martin_binance-1.3.2.post3/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    83217 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16282 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1282 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1427 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/pyproject.toml
--rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 martin_binance-1.3.2.post3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-04 17:38:43.607429 martin_binance-1.3.3/LICENSE
+-rwxr-xr-x   0        0        0     4025 2023-07-04 17:38:43.607429 martin_binance-1.3.3/README.md
+-rw-r--r--   0        0        0     2013 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/__init__.py
+-rw-r--r--   0        0        0     4642 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2946 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    14575 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6721 2023-07-04 17:38:43.655432 martin_binance-1.3.3/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6716 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6722 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4707 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/client.py
+-rw-r--r--   0        0        0   186647 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2023-07-04 17:38:43.659433 martin_binance-1.3.3/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    83215 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16282 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1282 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2023-07-04 17:38:43.663433 martin_binance-1.3.3/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1427 2023-07-04 17:38:43.663433 martin_binance-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 martin_binance-1.3.3/PKG-INFO
```

### Comparing `martin_binance-1.3.2.post3/LICENSE` & `martin_binance-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/README.md` & `martin_binance-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/__init__.py` & `martin_binance-1.3.3/martin_binance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.2-3"
+__version__ = "1.3.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 STANDALONE = True
```

### Comparing `martin_binance-1.3.2.post3/martin_binance/backtest/OoTSP.py` & `martin_binance-1.3.3/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/backtest/VCoSEL.py` & `martin_binance-1.3.3/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/backtest/exchange_simulator.py` & `martin_binance-1.3.3/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/cli_0_BTCUSDT.py.template` & `martin_binance-1.3.3/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/cli_1_BTCUSDT.py.template` & `martin_binance-1.3.3/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin_binance-1.3.3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/client.py` & `martin_binance-1.3.3/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/executor.py` & `martin_binance-1.3.3/martin_binance/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.2-3"
+__version__ = "1.3.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -902,15 +902,27 @@
                             and not self.reverse_hold
                             and not GRID_ONLY
                             and not self.grid_update_started
                             and not self.start_after_shift
                             and not self.tp_hold
                             and not self.tp_was_filled
                             and not self.orders_init)
-            if MODE in ('T', 'TC') and stable_state:
+            if (MODE in ('T', 'TC')
+                    and (
+                    stable_state
+                    or (
+                    self.grid_hold.get('timestamp')
+                    and int(self.local_time() - self.grid_hold['timestamp']) > HOLD_TP_ORDER_TIMEOUT
+                    )
+                    or (
+                    self.tp_order_hold.get('timestamp')
+                    and int(self.local_time() - self.tp_order_hold['timestamp']) > HOLD_TP_ORDER_TIMEOUT
+                    )
+                )
+            ):
                 orders = self.get_buffered_open_orders()
                 order_buy = len([i for i in orders if i.buy is True])
                 order_sell = len([i for i in orders if i.buy is False])
                 order_hold = len(self.orders_hold)
                 cycle_status = (self.cycle_buy, order_buy, order_sell, order_hold)
                 if self.cycle_status != cycle_status:
                     self.cycle_status = cycle_status
@@ -991,15 +1003,15 @@
                                          f" {self.s_currency if self.cycle_buy else self.f_currency} depo.\n"
                                          f"Available first: {fund_f} {self.f_currency}\n"
                                          f"Available second: {fund_s} {self.s_currency}\n"
                                          f"Last ticker price: {last_price}\n"
                                          f"WSS status: {ticker_update}s\n"
                                          f"From start {ct}\n"
                                          f"Delay: {time_diff} sec", tlg=True)
-                    elif self.tp_order_hold['timestamp']:
+                    elif self.tp_order_hold.get('timestamp'):
                         time_diff = int(self.local_time() - self.tp_order_hold['timestamp'])
                         if time_diff > HOLD_TP_ORDER_TIMEOUT:
                             self.message_log(f"Exist hold TP order for"
                                              f" {'Sell' if self.cycle_buy else 'Buy'} {self.tp_order_hold['amount']}"
                                              f" {self.f_currency if self.cycle_buy else self.s_currency}\n"
                                              f"Available first:{fund_f} {self.f_currency}\n"
                                              f"Available second:{fund_s} {self.s_currency}\n"
```

### Comparing `martin_binance-1.3.2.post3/martin_binance/funds_rate.db.template` & `martin_binance-1.3.3/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin_binance-1.3.3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/margin_wrapper.py` & `martin_binance-1.3.3/martin_binance/margin_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 margin.de <-> Python strategy <-> <margin_wrapper> <-> exchanges-wrapper <-> Exchanges API/WSS
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.2-3"
+__version__ = "1.3.3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import simplejson as json
 import logging
```

### Comparing `martin_binance-1.3.2.post3/martin_binance/ms_cfg.toml.template` & `martin_binance-1.3.3/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/service/funds_rate_exporter.py` & `martin_binance-1.3.3/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/service/grafana.json` & `martin_binance-1.3.3/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/martin_binance/service/relaunch.py` & `martin_binance-1.3.3/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post3/pyproject.toml` & `martin_binance-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper==1.3.2",
+    "exchanges-wrapper==1.3.3",
     "margin-strategy-sdk==0.0.11",
     "aiohttp==3.8.4",
     "grpcio==1.48.1",
     "grpcio-tools==1.48.1",
     "jsonpickle==3.0.1",
     "psutil==5.9.5",
     "requests==2.31.0",
```

### Comparing `martin_binance-1.3.2.post3/PKG-INFO` & `martin_binance-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.2.post3
+Version: 1.3.3
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==1.3.2
+Requires-Dist: exchanges-wrapper==1.3.3
 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: grpcio==1.48.1
 Requires-Dist: grpcio-tools==1.48.1
 Requires-Dist: jsonpickle==3.0.1
 Requires-Dist: psutil==5.9.5
 Requires-Dist: requests==2.31.0
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.2.post3 Summary: Free
-trading system for Binance SPOT API Author-email: Jerry Fedorenko
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.3 Summary: Free trading
+system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: exchanges-wrapper==1.3.2 Requires-Dist: margin-strategy-sdk==0.0.11
+Dist: exchanges-wrapper==1.3.3 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist:
 grpcio-tools==1.48.1 Requires-Dist: jsonpickle==3.0.1 Requires-Dist:
 psutil==5.9.5 Requires-Dist: requests==2.31.0 Requires-Dist: simplejson==3.19.1
 Requires-Dist: toml==0.10.2 Requires-Dist: libtmux==0.22.1 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.17.0 Requires-Dist:
 optuna==3.2.0 Requires-Dist: plotly==5.15.0 Requires-Dist: pandas==2.0.2
 Requires-Dist: dash==2.10.2 Requires-Dist: future==0.18.3 Requires-Dist:
```

