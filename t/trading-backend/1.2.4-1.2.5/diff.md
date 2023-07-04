# Comparing `tmp/trading-backend-1.2.4.tar.gz` & `tmp/trading-backend-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trading-backend-1.2.4.tar", last modified: Mon Jun 26 19:10:42 2023, max compression
+gzip compressed data, was "trading-backend-1.2.5.tar", last modified: Tue Jul  4 18:45:18 2023, max compression
```

## Comparing `trading-backend-1.2.4.tar` & `trading-backend-1.2.5.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-26 19:10:12.000000 trading-backend-1.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-26 19:10:12.000000 trading-backend-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 19:10:12.000000 trading-backend-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 19:10:42.350382 trading-backend-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-26 19:10:12.000000 trading-backend-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 19:10:12.000000 trading-backend-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 19:10:42.354382 trading-backend-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-26 19:10:12.000000 trading-backend-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.346382 trading-backend-1.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_kucoin_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/util/create_order_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/trading_backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchange_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/trading_backend/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/kucoinfutures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/trading_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.885764 trading-backend-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-04 18:44:49.000000 trading-backend-1.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-04 18:44:49.000000 trading-backend-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-04 18:44:49.000000 trading-backend-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-04 18:45:18.885764 trading-backend-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-04 18:44:49.000000 trading-backend-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 18:44:49.000000 trading-backend-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-04 18:45:18.885764 trading-backend-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-04 18:44:49.000000 trading-backend-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.881764 trading-backend-1.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.881764 trading-backend-1.2.5/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_kucoin_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.881764 trading-backend-1.2.5/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/util/create_order_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.881764 trading-backend-1.2.5/trading_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchange_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.885764 trading-backend-1.2.5/trading_backend/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/kucoinfutures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.885764 trading-backend-1.2.5/trading_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/top_level.txt
```

### Comparing `trading-backend-1.2.4/CHANGELOG.md` & `trading-backend-1.2.5/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.2.5] - 2023-06-29
+### Added
+- Crypto.com
+- MEXC
+
 ## [1.2.4] - 2023-06-24
 ### Added
 - Kucoin and Kucoin futures
 
 ## [1.2.3] - 2023-05-02
 ### Updated
 - setup.py
```

### Comparing `trading-backend-1.2.4/LICENSE` & `trading-backend-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/PKG-INFO` & `trading-backend-1.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.4
+Version: 1.2.5
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.4](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.5](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.4/README.md` & `trading-backend-1.2.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# trading-backend [1.2.4](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.5](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.4/setup.py` & `trading-backend-1.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 # from distutils.extension import Extension
 from setuptools import find_packages
 from setuptools import setup
 
-VERSION = "1.2.4"
+VERSION = "1.2.5"
 PROJECT_NAME = "trading-backend"
 
 PACKAGES = find_packages(exclude=["tests"])
 
 
 # long description from README file
 with open('README.md', encoding='utf-8') as f:
```

### Comparing `trading-backend-1.2.4/tests/exchanges/test_ascendex.py` & `trading-backend-1.2.5/tests/exchanges/test_ascendex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/exchanges/test_binance.py` & `trading-backend-1.2.5/tests/exchanges/test_binance.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 import copy
 
 import pytest
 import mock
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import trading_backend
+import tests.util.create_order_tests as create_order_tests
 from tests import binance_exchange
 
 
 def test_get_name(binance_exchange):
     assert exchanges.Binance(binance_exchange).get_name() == ccxt.async_support.binance().id.lower()
 
 
-def test_get_orders_parameters(binance_exchange):
+@pytest.mark.asyncio
+async def test_get_orders_parameters(binance_exchange):
     exchange = exchanges.Binance(binance_exchange)
-    with mock.patch.object(exchange._exchange.connector.client, "uuid22",
-                           mock.Mock(return_value="123456789")) as uuid22_mock:
-        assert exchange.get_orders_parameters({"a": 1}) == {
-            "a": 1,
-            'newClientOrderId': exchange._get_order_custom_id()
-        }
-        # once by get_orders_parameters and once by _get_order_custom_id
-        assert uuid22_mock.call_count == 2
+    await create_order_tests.create_order_mocked_test_args(
+        exchange,
+        exchange_private_post_order_method_name="privatePostOrder",
+        exchange_request_referral_key="newClientOrderId",
+        should_contains=True
+    )
 
 
 @pytest.mark.asyncio
 async def test_is_valid_account(binance_exchange):
     exchange = exchanges.Binance(binance_exchange)
     params = {"apiAgentCode": exchange._get_id()}
     with pytest.raises(trading_backend.ExchangeAuthError):
```

### Comparing `trading-backend-1.2.4/tests/exchanges/test_bitget.py` & `trading-backend-1.2.5/tests/exchanges/test_bitget.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import mock
 import pytest
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
 from tests import bitget_exchange
```

### Comparing `trading-backend-1.2.4/tests/exchanges/test_bybit.py` & `trading-backend-1.2.5/tests/exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/exchanges/test_exchange.py` & `trading-backend-1.2.5/tests/exchanges/test_exchange.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/exchanges/test_gateio.py` & `trading-backend-1.2.5/tests/exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/exchanges/test_huobi.py` & `trading-backend-1.2.5/tests/exchanges/test_huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/exchanges/test_huobipro.py` & `trading-backend-1.2.5/tests/exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/exchanges/test_kucoin.py` & `trading-backend-1.2.5/tests/exchanges/test_kucoin.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 @pytest.mark.asyncio
 async def test_broker_id(kucoin_exchange):
     exchange = exchanges.Kucoin(kucoin_exchange)
     await create_order_tests.sign_test(
         exchange,
         "private",
         "KC-API-PARTNER",
-        "KC-API-PARTNER-SIGN",
+        broker_sign_header_key="KC-API-PARTNER-SIGN",
     )
```

### Comparing `trading-backend-1.2.4/tests/exchanges/test_kucoin_futures.py` & `trading-backend-1.2.5/tests/exchanges/test_kucoin_futures.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 async def test_broker_id(kucoinfutures_exchange):
     exchange = exchanges.KucoinFutures(kucoinfutures_exchange)
     exchange._exchange.exchange_manager.is_future = True
     await create_order_tests.sign_test(
         exchange,
         "futuresPrivate",
         "KC-API-PARTNER",
-        "KC-API-PARTNER-SIGN",
+        broker_sign_header_key="KC-API-PARTNER-SIGN",
     )
```

### Comparing `trading-backend-1.2.4/tests/exchanges/test_okx.py` & `trading-backend-1.2.5/tests/exchanges/test_okx.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/exchanges/test_phemex.py` & `trading-backend-1.2.5/tests/exchanges/test_phemex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/util/__init__.py` & `trading-backend-1.2.5/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/tests/util/create_order_tests.py` & `trading-backend-1.2.5/tests/util/create_order_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
             assert exchange._get_id() in result
         else:
             assert exchange._get_id() == result
 
 
 async def sign_test(
     exchange: exchanges.Exchange,
-    api: str,
+    api,
     broker_id_header_key: str,
-    broker_sign_header_key: str,
+    broker_sign_header_key: str = None,
 ):
     url_path = "url/path"
     method = "POST"
     params = {}
     headers = None
     body = None
     api_key = "123"
@@ -77,25 +77,27 @@
     # without referral patch
     signed_result = ccxt_client.sign(
         url_path, api=api, method=method, params=params, headers=headers, body=body
     )
     assert signed_result
     headers = signed_result["headers"]
     assert headers[broker_id_header_key] != exchange._get_id()
-    assert headers[broker_sign_header_key]
+    if broker_sign_header_key:
+        assert headers[broker_sign_header_key]
 
     # with referral patch
     exchange.get_orders_parameters()
     signed_result = ccxt_client.sign(
         url_path, api=api, method=method, params=params, headers=headers, body=body
     )
     assert signed_result
     headers = signed_result["headers"]
     assert headers[broker_id_header_key] == exchange._get_id()
-    assert headers[broker_sign_header_key]
+    if broker_sign_header_key:
+        assert headers[broker_sign_header_key]
 
 
 async def exchange_requests_contains_headers_test(exchange: exchanges.Exchange,
                                                   exchange_header_referral_key: str,
                                                   exchange_header_referral_value: str):
     request_headers = exchange._exchange.connector.client.prepare_request_headers()
     assert request_headers[exchange_header_referral_key] == exchange_header_referral_value
```

### Comparing `trading-backend-1.2.4/trading_backend/__init__.py` & `trading-backend-1.2.5/trading_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/errors.py` & `trading-backend-1.2.5/trading_backend/errors.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchange_factory.py` & `trading-backend-1.2.5/trading_backend/exchange_factory.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/__init__.py` & `trading-backend-1.2.5/trading_backend/exchanges/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 )
 
 from trading_backend.exchanges import bybit
 from trading_backend.exchanges.bybit import (
     Bybit
 )
 
+from trading_backend.exchanges import cryptocom
+from trading_backend.exchanges.cryptocom import (
+    CryptoCom
+)
+
 from trading_backend.exchanges import ascendex
 from trading_backend.exchanges.ascendex import (
     Ascendex
 )
 
 from trading_backend.exchanges import gateio
 from trading_backend.exchanges.gateio import (
@@ -69,21 +74,28 @@
 )
 
 from trading_backend.exchanges import kucoinfutures
 from trading_backend.exchanges.kucoinfutures import (
     KucoinFutures
 )
 
+from trading_backend.exchanges import mexc
+from trading_backend.exchanges.mexc import (
+    MEXC
+)
+
 __all__ = [
     "Exchange",
     "Binance",
     "Bybit",
+    "CryptoCom",
     "OKX",
     "Ascendex",
     "GateIO",
     "Huobi",
     "HuobiPro",
     "Bitget",
     "Phemex",
     "Kucoin",
     "KucoinFutures",
+    "MEXC",
 ]
```

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/ascendex.py` & `trading-backend-1.2.5/trading_backend/exchanges/ascendex.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,10 +27,11 @@
         return 'ascendex'
 
     def _generate_order_id(self):
         new_id = "".join(self._exchange.connector.client.uuid().split("-"))
         return f"{self._get_id()}{new_id[len(self._get_id()):]}"
 
     def get_orders_parameters(self, params=None) -> dict:
+        # no ccxt broker id automation
         params = super().get_orders_parameters(params)
         params.update({'id': self._generate_order_id()})
         return params
```

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/binance.py` & `trading-backend-1.2.5/trading_backend/exchanges/binance.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,18 +36,27 @@
         return f"x-{self._get_id()}{self._exchange.connector.client.uuid22()}"
 
     @classmethod
     def use_legacy_ids(cls):
         cls.SPOT_ID = cls.LEGACY_SPOT_ID
         cls.FUTURE_ID = cls.LEGACY_FUTURE_ID
 
+    def _get_broker_dict(self, current_broker_params):
+        current_broker_params.update({
+            'spot': f"x-{self.__class__.SPOT_ID}",
+            'swap': f"x-{self.__class__.FUTURE_ID}",  # used in stop orders
+            'future': f"x-{self.__class__.FUTURE_ID}",
+        })
+        return current_broker_params
+
     def get_orders_parameters(self, params=None) -> dict:
-        params = super().get_orders_parameters(params)
-        params.update({'newClientOrderId': self._get_order_custom_id()})
-        return params
+        current_broker_params = self._exchange.connector.client.options.get("broker", {})
+        if current_broker_params != self._get_broker_dict(current_broker_params):
+            self._exchange.connector.client.options["broker"] = self._get_broker_dict(current_broker_params)
+        return super().get_orders_parameters(params)
 
     async def _ensure_broker_status(self):
         try:
             details = await self._get_account_referral_details()
             if not details.get("rebateWorking", False):
                 if (ref_id := details.get("referrerId", None)) and ref_id == self.LEGACY_REF_ID:
                     self.use_legacy_ids()
```

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/bitget.py` & `trading-backend-1.2.5/trading_backend/exchanges/bitget.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     def get_name(cls):
         return 'bitget'
 
     def _generate_order_id(self):
         return f"{self._get_id()}#{self._exchange.connector.client.uuid22()}"
 
     def get_orders_parameters(self, params=None) -> dict:
-        self._exchange.connector.client.options["broker"] = self._get_id()
+        if self._exchange.connector.client.options.get("broker", None) != self._get_id():
+            self._exchange.connector.client.options["broker"] = self._get_id()
         params = super().get_orders_parameters(params)
         params["clientOrderId"] = self._generate_order_id()
         return super().get_orders_parameters(params)
 
     async def _inner_is_valid_account(self) -> (bool, str):
         # Nothing to do
         return await super()._inner_is_valid_account()
```

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/bybit.py` & `trading-backend-1.2.5/trading_backend/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/exchange.py` & `trading-backend-1.2.5/trading_backend/exchanges/exchange.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/gateio.py` & `trading-backend-1.2.5/trading_backend/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/huobi.py` & `trading-backend-1.2.5/trading_backend/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/huobipro.py` & `trading-backend-1.2.5/trading_backend/exchanges/huobipro.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/kucoin.py` & `trading-backend-1.2.5/trading_backend/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/kucoinfutures.py` & `trading-backend-1.2.5/trading_backend/exchanges/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/okx.py` & `trading-backend-1.2.5/trading_backend/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend/exchanges/phemex.py` & `trading-backend-1.2.5/trading_backend/exchanges/phemex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.4/trading_backend.egg-info/PKG-INFO` & `trading-backend-1.2.5/trading_backend.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.4
+Version: 1.2.5
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.4](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.5](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.4/trading_backend.egg-info/SOURCES.txt` & `trading-backend-1.2.5/trading_backend.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 setup.cfg
 setup.py
 tests/exchanges/__init__.py
 tests/exchanges/test_ascendex.py
 tests/exchanges/test_binance.py
 tests/exchanges/test_bitget.py
 tests/exchanges/test_bybit.py
+tests/exchanges/test_cryptocom.py
 tests/exchanges/test_exchange.py
 tests/exchanges/test_gateio.py
 tests/exchanges/test_huobi.py
 tests/exchanges/test_huobipro.py
 tests/exchanges/test_kucoin.py
 tests/exchanges/test_kucoin_futures.py
+tests/exchanges/test_mexc.py
 tests/exchanges/test_okx.py
 tests/exchanges/test_phemex.py
 tests/util/__init__.py
 tests/util/create_order_tests.py
 trading_backend/__init__.py
 trading_backend/errors.py
 trading_backend/exchange_factory.py
@@ -30,15 +32,17 @@
 trading_backend.egg-info/requires.txt
 trading_backend.egg-info/top_level.txt
 trading_backend/exchanges/__init__.py
 trading_backend/exchanges/ascendex.py
 trading_backend/exchanges/binance.py
 trading_backend/exchanges/bitget.py
 trading_backend/exchanges/bybit.py
+trading_backend/exchanges/cryptocom.py
 trading_backend/exchanges/exchange.py
 trading_backend/exchanges/gateio.py
 trading_backend/exchanges/huobi.py
 trading_backend/exchanges/huobipro.py
 trading_backend/exchanges/kucoin.py
 trading_backend/exchanges/kucoinfutures.py
+trading_backend/exchanges/mexc.py
 trading_backend/exchanges/okx.py
 trading_backend/exchanges/phemex.py
```

