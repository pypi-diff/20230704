# Comparing `tmp/quantplay-1.2.99.tar.gz` & `tmp/quantplay-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.2.99.tar", last modified: Tue Jul  4 04:16:34 2023, max compression
+gzip compressed data, was "quantplay-1.3.1.tar", last modified: Tue Jul  4 04:23:20 2023, max compression
```

## Comparing `quantplay-1.2.99.tar` & `quantplay-1.3.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      938 2023-07-04 04:16:34.047299 quantplay-1.2.99/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      494 2022-04-21 03:10:36.000000 quantplay-1.2.99/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/backtest/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/backtest/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17605 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/backtest/backtest_trades.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/broker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10902 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/angelone.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/broker_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       87 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/broker/finvasia_utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/finvasia_utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2576 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/finvasia_utils/shoonya.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/broker/generics/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/generics/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28802 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/generics/broker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3897 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/iifl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      588 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/iifl_xts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/kite_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31836 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/motilal.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19618 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/shoonya.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/symphony.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19145 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/broker/xts_utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33446 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/Connect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3046 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/Exception.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6456 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9106 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17192 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/zerodha.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/brokerage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/brokerage/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/brokerage/angelone/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/brokerage/angelone/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10989 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/brokerage/angelone/angel_broker.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/brokerage/generics/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/brokerage/generics/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28259 2023-07-04 04:12:52.000000 quantplay-1.2.99/quantplay/brokerage/generics/broker.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/brokerage/zerodha/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17690 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/brokerage/zerodha/ZBroker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/brokerage/zerodha/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/config/qplay_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1127 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/create_sample_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1725 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/data_modify_script.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3481 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/date_fix.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/exception/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/exception/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2162 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/exception/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6064 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/executor/strategy_executor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/indicators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1747 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/indicators/Indicator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/indicators/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/indicators/atr.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/model/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/model/exchange/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/model/exchange/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1472 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/model/exchange/instrument.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8794 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/model/exchange/order.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3238 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/model/exchange/tick.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/model/strategy/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/model/strategy/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/model/strategy/strategy_response.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/oms/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/oms/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/order_execution/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/order_execution/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2048 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/order_execution/execution_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1281 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/order_execution/mean_price.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/reporting/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/reporting/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10801 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/reporting/strategy_report.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/reporting/visuals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      231 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/services/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/services/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18366 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/services/market.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11648 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/services/tradelens.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/strategy/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/strategy/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12759 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/strategy/base.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/quantplay/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      723 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/utils/config_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24181 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/constant.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5433 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/data_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      711 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/utils/exchange.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/number_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/pickle_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/selenium_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4094 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/utils/transaction_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      938 2023-07-04 04:16:33.000000 quantplay-1.2.99/quantplay.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2854 2023-07-04 04:16:34.000000 quantplay-1.2.99/quantplay.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-04 04:16:33.000000 quantplay-1.2.99/quantplay.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-07-04 04:16:33.000000 quantplay-1.2.99/quantplay.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-07-04 04:16:33.000000 quantplay-1.2.99/quantplay.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-07-04 04:16:34.047299 quantplay-1.2.99/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2023-07-04 04:13:39.000000 quantplay-1.2.99/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/test/broker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/test/broker/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      220 2023-07-04 04:08:13.000000 quantplay-1.2.99/test/broker/finvasia.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/test/executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/executor/strategy_executor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/test/strategy/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/strategy/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/strategy/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2194 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/strategy/sample_strategy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3302 2023-07-04 04:08:13.000000 quantplay-1.2.99/test/test_motilal.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.035290 quantplay-1.3.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      937 2023-07-04 04:23:20.035290 quantplay-1.3.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      494 2022-04-21 03:10:36.000000 quantplay-1.3.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.027290 quantplay-1.3.1/quantplay/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.027290 quantplay-1.3.1/quantplay/backtest/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/backtest/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17605 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/backtest/backtest_trades.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/broker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10902 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/angelone.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/broker_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       87 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/broker/finvasia_utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/finvasia_utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2576 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/finvasia_utils/shoonya.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/broker/generics/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/generics/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28802 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/generics/broker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3897 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/iifl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      588 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/iifl_xts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/kite_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31836 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/motilal.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19618 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/shoonya.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/symphony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19145 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/xts.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/broker/xts_utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33446 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/xts_utils/Connect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3046 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/xts_utils/Exception.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6456 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9106 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/xts_utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17192 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/broker/zerodha.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/brokerage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/brokerage/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/brokerage/angelone/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/brokerage/angelone/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10989 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/brokerage/angelone/angel_broker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/brokerage/generics/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/brokerage/generics/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28260 2023-07-04 04:23:00.000000 quantplay-1.3.1/quantplay/brokerage/generics/broker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/brokerage/zerodha/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17690 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/brokerage/zerodha/ZBroker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/brokerage/zerodha/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2022-04-21 03:10:36.000000 quantplay-1.3.1/quantplay/config/qplay_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1127 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/create_sample_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1725 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/data_modify_script.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3481 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/date_fix.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/exception/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/exception/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2162 2022-04-21 03:10:36.000000 quantplay-1.3.1/quantplay/exception/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6064 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/executor/strategy_executor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/indicators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1747 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/indicators/Indicator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/indicators/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/indicators/atr.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/model/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/model/exchange/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/model/exchange/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1472 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/model/exchange/instrument.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8794 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/model/exchange/order.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3238 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/model/exchange/tick.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/model/strategy/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/model/strategy/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-04-21 03:10:36.000000 quantplay-1.3.1/quantplay/model/strategy/strategy_response.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/oms/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/oms/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/order_execution/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/order_execution/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2048 2022-04-21 03:10:36.000000 quantplay-1.3.1/quantplay/order_execution/execution_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1281 2022-04-21 03:10:36.000000 quantplay-1.3.1/quantplay/order_execution/mean_price.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/reporting/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/reporting/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10801 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/reporting/strategy_report.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/reporting/visuals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      231 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/services/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/services/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18366 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/services/market.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11648 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/services/tradelens.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.031290 quantplay-1.3.1/quantplay/strategy/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/strategy/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12759 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/strategy/base.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.035290 quantplay-1.3.1/quantplay/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.3.1/quantplay/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      723 2022-04-21 03:10:36.000000 quantplay-1.3.1/quantplay/utils/config_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24181 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/utils/constant.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5433 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/utils/data_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      711 2022-04-21 03:10:36.000000 quantplay-1.3.1/quantplay/utils/exchange.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/utils/number_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/utils/pickle_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2023-07-04 04:08:13.000000 quantplay-1.3.1/quantplay/utils/selenium_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4094 2022-04-21 03:10:36.000000 quantplay-1.3.1/quantplay/utils/transaction_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.027290 quantplay-1.3.1/quantplay.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      937 2023-07-04 04:23:19.000000 quantplay-1.3.1/quantplay.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2854 2023-07-04 04:23:20.000000 quantplay-1.3.1/quantplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-04 04:23:19.000000 quantplay-1.3.1/quantplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-07-04 04:23:19.000000 quantplay-1.3.1/quantplay.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-07-04 04:23:19.000000 quantplay-1.3.1/quantplay.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-07-04 04:23:20.035290 quantplay-1.3.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-07-04 04:23:08.000000 quantplay-1.3.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.035290 quantplay-1.3.1/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.3.1/test/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.035290 quantplay-1.3.1/test/broker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.3.1/test/broker/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      220 2023-07-04 04:08:13.000000 quantplay-1.3.1/test/broker/finvasia.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.035290 quantplay-1.3.1/test/executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.3.1/test/executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2022-04-21 03:10:36.000000 quantplay-1.3.1/test/executor/strategy_executor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:23:20.035290 quantplay-1.3.1/test/strategy/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.3.1/test/strategy/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-04-21 03:10:36.000000 quantplay-1.3.1/test/strategy/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2194 2022-04-21 03:10:36.000000 quantplay-1.3.1/test/strategy/sample_strategy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3302 2023-07-04 04:08:13.000000 quantplay-1.3.1/test/test_motilal.py
```

### Comparing `quantplay-1.2.99/PKG-INFO` & `quantplay-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: quantplay
-Version: 1.2.99
+Version: 1.3.1
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.99/quantplay/backtest/backtest_trades.py` & `quantplay-1.3.1/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/angelone.py` & `quantplay-1.3.1/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/broker_client.py` & `quantplay-1.3.1/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.3.1/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/generics/broker.py` & `quantplay-1.3.1/quantplay/broker/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/iifl.py` & `quantplay-1.3.1/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/iifl_xts.py` & `quantplay-1.3.1/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/kite_utils.py` & `quantplay-1.3.1/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/motilal.py` & `quantplay-1.3.1/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/shoonya.py` & `quantplay-1.3.1/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/symphony.py` & `quantplay-1.3.1/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/xts.py` & `quantplay-1.3.1/quantplay/broker/xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.3.1/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.3.1/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.3.1/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.3.1/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/broker/zerodha.py` & `quantplay-1.3.1/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.3.1/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/brokerage/generics/broker.py` & `quantplay-1.3.1/quantplay/brokerage/generics/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             start_date = start_date.replace(minute=0, hour=0)
 
             try:
                 response = self.get_historical_data(
                     instrument_id, start_date=start_date, end_date=end_date, interval_max_days=interval_max_days
                 )
             except Exception as e:
-                Constant.logger.error(f"[HISTORICLA_DATA_FETCH_FAILED] {instrument_id}")
+                Constants.logger.error(f"[HISTORICAL_DATA_FETCH_FAILED] {instrument_id}")
                 continue
             for interval, data in response.items():
                 if len(data) > 0:
                     data = self.add_today_candles(data, symbol)
                     data.loc[:, "security_type"] = security_type
                     instrument_data_by_interval[interval].append(data)
                 else:
```

### Comparing `quantplay-1.2.99/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.3.1/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/config/qplay_config.py` & `quantplay-1.3.1/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/create_sample_data.py` & `quantplay-1.3.1/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/data_modify_script.py` & `quantplay-1.3.1/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/date_fix.py` & `quantplay-1.3.1/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/exception/exceptions.py` & `quantplay-1.3.1/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/executor/strategy_executor.py` & `quantplay-1.3.1/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/indicators/Indicator.py` & `quantplay-1.3.1/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/model/exchange/instrument.py` & `quantplay-1.3.1/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/model/exchange/order.py` & `quantplay-1.3.1/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/model/exchange/tick.py` & `quantplay-1.3.1/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.3.1/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/order_execution/mean_price.py` & `quantplay-1.3.1/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/reporting/strategy_report.py` & `quantplay-1.3.1/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/reporting/visuals.py` & `quantplay-1.3.1/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/services/market.py` & `quantplay-1.3.1/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/services/tradelens.py` & `quantplay-1.3.1/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/strategy/base.py` & `quantplay-1.3.1/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/utils/config_util.py` & `quantplay-1.3.1/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/utils/constant.py` & `quantplay-1.3.1/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/utils/data_utils.py` & `quantplay-1.3.1/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/utils/exchange.py` & `quantplay-1.3.1/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/utils/number_utils.py` & `quantplay-1.3.1/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/utils/selenium_utils.py` & `quantplay-1.3.1/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay/utils/transaction_utils.py` & `quantplay-1.3.1/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/quantplay.egg-info/PKG-INFO` & `quantplay-1.3.1/quantplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: quantplay
-Version: 1.2.99
+Version: 1.3.1
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.99/quantplay.egg-info/SOURCES.txt` & `quantplay-1.3.1/quantplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/setup.py` & `quantplay-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.2.99",
+    version="1.3.1",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.2.99/test/strategy/sample_strategy.py` & `quantplay-1.3.1/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.99/test/test_motilal.py` & `quantplay-1.3.1/test/test_motilal.py`

 * *Files identical despite different names*

