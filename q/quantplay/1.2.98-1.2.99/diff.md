# Comparing `tmp/quantplay-1.2.98.tar.gz` & `tmp/quantplay-1.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.2.98.tar", last modified: Fri Jun 23 06:50:58 2023, max compression
+gzip compressed data, was "quantplay-1.2.99.tar", last modified: Tue Jul  4 04:16:34 2023, max compression
```

## Comparing `quantplay-1.2.98.tar` & `quantplay-1.2.99.tar`

### file list

```diff
@@ -1,140 +1,119 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.755872 quantplay-1.2.98/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-23 06:50:58.755923 quantplay-1.2.98/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.98/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.740078 quantplay-1.2.98/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.740951 quantplay-1.2.98/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.98/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.743541 quantplay-1.2.98/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.743968 quantplay-1.2.98/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.98/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.744307 quantplay-1.2.98/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.98/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.98/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.2.98/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.98/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.98/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.2.98/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.745756 quantplay-1.2.98/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.98/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.2.98/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.98/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.745848 quantplay-1.2.98/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.746026 quantplay-1.2.98/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.746425 quantplay-1.2.98/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.98/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.747161 quantplay-1.2.98/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.98/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.747380 quantplay-1.2.98/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.98/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.2.98/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.747614 quantplay-1.2.98/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.747934 quantplay-1.2.98/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.748654 quantplay-1.2.98/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.748800 quantplay-1.2.98/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.749405 quantplay-1.2.98/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.98/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.749650 quantplay-1.2.98/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.749789 quantplay-1.2.98/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.750149 quantplay-1.2.98/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.750496 quantplay-1.2.98/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.2.98/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.98/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.98/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751332 quantplay-1.2.98/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-06-23 06:49:50.000000 quantplay-1.2.98/quantplay/services/alphawiz.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.98/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.2.98/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751456 quantplay-1.2.98/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.98/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751558 quantplay-1.2.98/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.98/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751666 quantplay-1.2.98/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.98/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751775 quantplay-1.2.98/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.98/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751879 quantplay-1.2.98/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.98/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751977 quantplay-1.2.98/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.98/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.752078 quantplay-1.2.98/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.98/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.752819 quantplay-1.2.98/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.98/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.98/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.98/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.98/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.753078 quantplay-1.2.98/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.98/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.98/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.754647 quantplay-1.2.98/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.98/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.98/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.740740 quantplay-1.2.98/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3422 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-06-23 06:50:58.756115 quantplay-1.2.98/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      876 2023-06-23 06:50:55.000000 quantplay-1.2.98/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.754904 quantplay-1.2.98/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.98/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.755138 quantplay-1.2.98/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.755374 quantplay-1.2.98/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.755751 quantplay-1.2.98/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/test_motilal.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      938 2023-07-04 04:16:34.047299 quantplay-1.2.99/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      494 2022-04-21 03:10:36.000000 quantplay-1.2.99/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/backtest/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/backtest/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17605 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/backtest/backtest_trades.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/broker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10902 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/angelone.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/broker_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       87 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/broker/finvasia_utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/finvasia_utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2576 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/finvasia_utils/shoonya.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay/broker/generics/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/generics/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28802 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/generics/broker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3897 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/iifl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      588 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/iifl_xts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/kite_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31836 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/motilal.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19618 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/shoonya.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/symphony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19145 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/broker/xts_utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33446 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/Connect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3046 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/Exception.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6456 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9106 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/xts_utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17192 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/broker/zerodha.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/brokerage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/brokerage/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/brokerage/angelone/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/brokerage/angelone/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10989 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/brokerage/angelone/angel_broker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/brokerage/generics/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/brokerage/generics/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28259 2023-07-04 04:12:52.000000 quantplay-1.2.99/quantplay/brokerage/generics/broker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/brokerage/zerodha/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17690 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/brokerage/zerodha/ZBroker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/brokerage/zerodha/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/config/qplay_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1127 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/create_sample_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1725 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/data_modify_script.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3481 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/date_fix.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/exception/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/exception/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2162 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/exception/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6064 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/executor/strategy_executor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/indicators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1747 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/indicators/Indicator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/indicators/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/indicators/atr.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/model/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/model/exchange/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/model/exchange/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1472 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/model/exchange/instrument.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8794 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/model/exchange/order.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3238 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/model/exchange/tick.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/model/strategy/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/model/strategy/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/model/strategy/strategy_response.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/oms/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/oms/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/order_execution/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/order_execution/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2048 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/order_execution/execution_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1281 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/order_execution/mean_price.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/reporting/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/reporting/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10801 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/reporting/strategy_report.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/reporting/visuals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      231 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/services/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/services/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18366 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/services/market.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11648 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/services/tradelens.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.043299 quantplay-1.2.99/quantplay/strategy/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/strategy/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12759 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/strategy/base.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/quantplay/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-08 04:42:36.000000 quantplay-1.2.99/quantplay/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      723 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/utils/config_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24181 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/constant.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5433 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/data_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      711 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/utils/exchange.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/number_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/pickle_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2023-07-04 04:08:13.000000 quantplay-1.2.99/quantplay/utils/selenium_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4094 2022-04-21 03:10:36.000000 quantplay-1.2.99/quantplay/utils/transaction_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.039299 quantplay-1.2.99/quantplay.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      938 2023-07-04 04:16:33.000000 quantplay-1.2.99/quantplay.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2854 2023-07-04 04:16:34.000000 quantplay-1.2.99/quantplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-04 04:16:33.000000 quantplay-1.2.99/quantplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-07-04 04:16:33.000000 quantplay-1.2.99/quantplay.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-07-04 04:16:33.000000 quantplay-1.2.99/quantplay.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-07-04 04:16:34.047299 quantplay-1.2.99/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2023-07-04 04:13:39.000000 quantplay-1.2.99/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/test/broker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:08:13.000000 quantplay-1.2.99/test/broker/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      220 2023-07-04 04:08:13.000000 quantplay-1.2.99/test/broker/finvasia.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/test/executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/executor/strategy_executor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 04:16:34.047299 quantplay-1.2.99/test/strategy/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/strategy/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/strategy/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2194 2022-04-21 03:10:36.000000 quantplay-1.2.99/test/strategy/sample_strategy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3302 2023-07-04 04:08:13.000000 quantplay-1.2.99/test/test_motilal.py
```

### Comparing `quantplay-1.2.98/quantplay/backtest/backtest_trades.py` & `quantplay-1.2.99/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/angelone.py` & `quantplay-1.2.99/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/broker_client.py` & `quantplay-1.2.99/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.2.99/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/generics/broker.py` & `quantplay-1.2.99/quantplay/broker/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/iifl.py` & `quantplay-1.2.99/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/iifl_xts.py` & `quantplay-1.2.99/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/kite_utils.py` & `quantplay-1.2.99/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/motilal.py` & `quantplay-1.2.99/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/shoonya.py` & `quantplay-1.2.99/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/symphony.py` & `quantplay-1.2.99/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/xts.py` & `quantplay-1.2.99/quantplay/broker/xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.2.99/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.2.99/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.2.99/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.2.99/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/broker/zerodha.py` & `quantplay-1.2.99/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.2.99/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/brokerage/generics/broker.py` & `quantplay-1.2.99/quantplay/brokerage/generics/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,21 @@
 
             end_date = datetime.now()
             end_date = end_date.replace(second=0, microsecond=0)
 
             start_date = end_date - timedelta(days=20)
             start_date = start_date.replace(minute=0, hour=0)
 
-            response = self.get_historical_data(
-                instrument_id, start_date=start_date, end_date=end_date, interval_max_days=interval_max_days
-            )
+            try:
+                response = self.get_historical_data(
+                    instrument_id, start_date=start_date, end_date=end_date, interval_max_days=interval_max_days
+                )
+            except Exception as e:
+                Constant.logger.error(f"[HISTORICLA_DATA_FETCH_FAILED] {instrument_id}")
+                continue
             for interval, data in response.items():
                 if len(data) > 0:
                     data = self.add_today_candles(data, symbol)
                     data.loc[:, "security_type"] = security_type
                     instrument_data_by_interval[interval].append(data)
                 else:
                     Constants.logger.info(
```

### Comparing `quantplay-1.2.98/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.2.99/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/config/qplay_config.py` & `quantplay-1.2.99/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/create_sample_data.py` & `quantplay-1.2.99/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/data_modify_script.py` & `quantplay-1.2.99/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/date_fix.py` & `quantplay-1.2.99/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/exception/exceptions.py` & `quantplay-1.2.99/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/executor/strategy_executor.py` & `quantplay-1.2.99/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/indicators/Indicator.py` & `quantplay-1.2.99/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/model/exchange/instrument.py` & `quantplay-1.2.99/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/model/exchange/order.py` & `quantplay-1.2.99/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/model/exchange/tick.py` & `quantplay-1.2.99/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.2.99/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/order_execution/mean_price.py` & `quantplay-1.2.99/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/reporting/strategy_report.py` & `quantplay-1.2.99/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/reporting/visuals.py` & `quantplay-1.2.99/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/services/market.py` & `quantplay-1.2.99/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/services/tradelens.py` & `quantplay-1.2.99/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/strategy/base.py` & `quantplay-1.2.99/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/utils/config_util.py` & `quantplay-1.2.99/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/utils/constant.py` & `quantplay-1.2.99/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/utils/data_utils.py` & `quantplay-1.2.99/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/utils/exchange.py` & `quantplay-1.2.99/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/utils/number_utils.py` & `quantplay-1.2.99/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/utils/selenium_utils.py` & `quantplay-1.2.99/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay/utils/transaction_utils.py` & `quantplay-1.2.99/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/quantplay.egg-info/SOURCES.txt` & `quantplay-1.2.99/quantplay.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 setup.cfg
 setup.py
 quantplay/__init__.py
 quantplay/create_sample_data.py
 quantplay/data_modify_script.py
 quantplay/date_fix.py
 quantplay/service.py
-quantplay/strategy_run.py
 quantplay.egg-info/PKG-INFO
 quantplay.egg-info/SOURCES.txt
 quantplay.egg-info/dependency_links.txt
 quantplay.egg-info/requires.txt
 quantplay.egg-info/top_level.txt
 quantplay/backtest/__init__.py
 quantplay/backtest/backtest_trades.py
@@ -62,28 +61,16 @@
 quantplay/order_execution/__init__.py
 quantplay/order_execution/execution_algorithm.py
 quantplay/order_execution/mean_price.py
 quantplay/reporting/__init__.py
 quantplay/reporting/strategy_report.py
 quantplay/reporting/visuals.py
 quantplay/services/__init__.py
-quantplay/services/alphawiz.py
 quantplay/services/market.py
 quantplay/services/tradelens.py
-quantplay/strategies/__init__.py
-quantplay/strategies/equities/__init__.py
-quantplay/strategies/equities/intraday/__init__.py
-quantplay/strategies/equities/overnight/__init__.py
-quantplay/strategies/futures/__init__.py
-quantplay/strategies/futures/overnight/__init__.py
-quantplay/strategies/options/__init__.py
-quantplay/strategies/options/intraday/__init__.py
-quantplay/strategies/options/intraday/ladder.py
-quantplay/strategies/options/intraday/musk.py
-quantplay/strategies/options/intraday/short_straddle.py
 quantplay/strategy/__init__.py
 quantplay/strategy/base.py
 quantplay/utils/__init__.py
 quantplay/utils/config_util.py
 quantplay/utils/constant.py
 quantplay/utils/data_utils.py
 quantplay/utils/exchange.py
```

### Comparing `quantplay-1.2.98/setup.py` & `quantplay-1.2.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.2.98",
+    version="1.2.99",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.2.98/test/strategy/sample_strategy.py` & `quantplay-1.2.99/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.98/test/test_motilal.py` & `quantplay-1.2.99/test/test_motilal.py`

 * *Files identical despite different names*

