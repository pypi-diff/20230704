# Comparing `tmp/sfctools-1.1.0.1.tar.gz` & `tmp/sfctools-1.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.1.0.1.tar", max compression
+gzip compressed data, was "sfctools-1.1.0.2.tar", max compression
```

## Comparing `sfctools-1.1.0.1.tar` & `sfctools-1.1.0.2.tar`

### file list

```diff
@@ -1,261 +1,110 @@
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.1.0.1/LICENSE
--rw-r--r--   0        0        0     1620 2023-07-04 09:26:32.596314 sfctools-1.1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1865 2023-06-23 11:07:04.102942 sfctools-1.1.0.1/README.md
--rw-r--r--   0        0        0       39 2023-01-26 10:19:31.537790 sfctools-1.1.0.1/sfctools/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-01-26 10:19:31.537845 sfctools-1.1.0.1/sfctools/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-01-26 10:19:31.536780 sfctools-1.1.0.1/sfctools/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-01-26 10:19:31.537845 sfctools-1.1.0.1/sfctools/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-01-26 10:19:31.539052 sfctools-1.1.0.1/sfctools/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.1.0.1/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.1.0.1/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.1.0.1/sfctools/automation/__init__.py
--rw-r--r--   0        0        0      177 2023-01-25 08:23:20.053567 sfctools-1.1.0.1/sfctools/automation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      159 2023-01-19 21:54:26.523852 sfctools-1.1.0.1/sfctools/automation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8273 2023-01-25 08:23:20.054862 sfctools-1.1.0.1/sfctools/automation/__pycache__/runner.cpython-311.pyc
--rw-r--r--   0        0        0     4139 2023-01-19 21:54:26.530954 sfctools-1.1.0.1/sfctools/automation/__pycache__/runner.cpython-38.pyc
--rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.1.0.1/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.1.0.1/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.1.0.1/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.1.0.1/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.1.0.1/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0      175 2023-01-25 08:23:19.248631 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      157 2023-01-19 21:54:25.705346 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    13033 2023-06-23 17:29:26.741582 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/matching.cpython-311.pyc
--rw-r--r--   0        0        0     8647 2023-02-06 10:24:45.316244 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/matching.cpython-38.pyc
--rw-r--r--   0        0        0    20113 2023-06-23 17:29:27.675222 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/productiontree.cpython-311.pyc
--rw-r--r--   0        0        0    11855 2023-05-04 16:23:16.775833 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/productiontree.cpython-38.pyc
--rw-r--r--   0        0        0     8339 2023-01-25 08:23:19.250795 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/stock_manager.cpython-311.pyc
--rw-r--r--   0        0        0     5937 2023-01-19 21:54:25.707915 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/stock_manager.cpython-38.pyc
--rw-r--r--   0        0        0     4085 2023-06-23 17:29:27.677221 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/treestruct.cpython-311.pyc
--rw-r--r--   0        0        0     2863 2023-01-25 08:16:32.090879 sfctools-1.1.0.1/sfctools/bottomup/__pycache__/treestruct.cpython-38.pyc
--rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.1.0.1/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.1.0.1/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.1.0.1/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.1.0.1/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.1.0.1/sfctools/core/__init__.py
--rw-r--r--   0        0        0      171 2023-01-25 08:23:16.612109 sfctools-1.1.0.1/sfctools/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      153 2023-01-19 21:54:24.854116 sfctools-1.1.0.1/sfctools/core/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      153 2022-12-22 08:43:56.478191 sfctools-1.1.0.1/sfctools/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    10127 2023-01-25 08:23:16.614415 sfctools-1.1.0.1/sfctools/core/__pycache__/agent.cpython-311.pyc
--rw-r--r--   0        0        0     7106 2023-01-19 21:54:24.857704 sfctools-1.1.0.1/sfctools/core/__pycache__/agent.cpython-38.pyc
--rw-r--r--   0        0        0     7096 2022-12-22 08:43:56.499523 sfctools-1.1.0.1/sfctools/core/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0     3200 2023-01-25 08:23:17.901786 sfctools-1.1.0.1/sfctools/core/__pycache__/clock.cpython-311.pyc
--rw-r--r--   0        0        0     2503 2023-01-19 21:54:25.148426 sfctools-1.1.0.1/sfctools/core/__pycache__/clock.cpython-38.pyc
--rw-r--r--   0        0        0      855 2023-06-23 17:29:25.224686 sfctools-1.1.0.1/sfctools/core/__pycache__/custom_warnings.cpython-311.pyc
--rw-r--r--   0        0        0      677 2023-04-04 07:45:29.386549 sfctools-1.1.0.1/sfctools/core/__pycache__/custom_warnings.cpython-38.pyc
--rw-r--r--   0        0        0    20139 2023-06-23 17:29:26.550025 sfctools-1.1.0.1/sfctools/core/__pycache__/flow_matrix.cpython-311.pyc
--rw-r--r--   0        0        0    12285 2023-06-23 12:23:26.073508 sfctools-1.1.0.1/sfctools/core/__pycache__/flow_matrix.cpython-38.pyc
--rw-r--r--   0        0        0    13244 2023-06-23 17:29:26.503632 sfctools-1.1.0.1/sfctools/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     8933 2023-04-04 07:45:29.692870 sfctools-1.1.0.1/sfctools/core/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0        0        0     1482 2023-01-25 08:23:17.905919 sfctools-1.1.0.1/sfctools/core/__pycache__/singleton.cpython-311.pyc
--rw-r--r--   0        0        0     1091 2023-01-19 21:54:25.153899 sfctools-1.1.0.1/sfctools/core/__pycache__/singleton.cpython-38.pyc
--rw-r--r--   0        0        0     8850 2023-06-23 17:29:24.074064 sfctools-1.1.0.1/sfctools/core/__pycache__/world.cpython-311.pyc
--rw-r--r--   0        0        0     5654 2023-02-06 10:24:44.695973 sfctools-1.1.0.1/sfctools/core/__pycache__/world.cpython-38.pyc
--rw-r--r--   0        0        0     5547 2022-12-22 08:43:56.518896 sfctools-1.1.0.1/sfctools/core/__pycache__/world.cpython-39.pyc
--rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.1.0.1/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.1.0.1/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.1.0.1/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15252 2023-06-23 11:02:51.691877 sfctools-1.1.0.1/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.1.0.1/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.1.0.1/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.1.0.1/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.1.0.1/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0      178 2023-01-25 08:23:16.618054 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      160 2023-01-19 21:54:24.869946 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      160 2022-12-22 08:43:56.522922 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    36524 2023-06-23 17:29:26.500628 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/balance.cpython-311.pyc
--rw-r--r--   0        0        0    22057 2023-04-04 07:45:29.687338 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/balance.cpython-38.pyc
--rw-r--r--   0        0        0    19917 2023-06-23 17:29:26.738552 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/bank_order_book.cpython-311.pyc
--rw-r--r--   0        0        0    13962 2023-02-06 10:24:45.311852 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/bank_order_book.cpython-38.pyc
--rw-r--r--   0        0        0     8907 2023-06-23 17:29:26.733550 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-311.pyc
--rw-r--r--   0        0        0     6617 2023-04-04 07:45:29.894931 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-38.pyc
--rw-r--r--   0        0        0     6937 2023-01-25 08:23:16.619099 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/collection.cpython-311.pyc
--rw-r--r--   0        0        0     4736 2023-01-19 21:54:24.876121 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/collection.cpython-38.pyc
--rw-r--r--   0        0        0     4718 2022-12-22 08:43:56.543068 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/collection.cpython-39.pyc
--rw-r--r--   0        0        0    18682 2023-06-23 17:29:26.731851 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/income_statement.cpython-311.pyc
--rw-r--r--   0        0        0    13398 2023-06-23 12:23:26.555886 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/income_statement.cpython-38.pyc
--rw-r--r--   0        0        0     8382 2023-01-25 08:23:20.048441 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/inventory.cpython-311.pyc
--rw-r--r--   0        0        0     5672 2023-01-19 21:54:26.507228 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/inventory.cpython-38.pyc
--rw-r--r--   0        0        0     6583 2023-01-25 08:23:20.050844 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/market_registry.cpython-311.pyc
--rw-r--r--   0        0        0     5167 2023-01-19 21:54:26.513706 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/market_registry.cpython-38.pyc
--rw-r--r--   0        0        0     8490 2023-01-25 08:23:19.471344 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/signalslot.cpython-311.pyc
--rw-r--r--   0        0        0     6018 2023-01-19 21:54:25.936504 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/signalslot.cpython-38.pyc
--rw-r--r--   0        0        0     5449 2023-06-23 17:29:27.482654 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/worker_registry.cpython-311.pyc
--rw-r--r--   0        0        0     3836 2023-06-23 12:23:27.182016 sfctools-1.1.0.1/sfctools/datastructs/__pycache__/worker_registry.cpython-38.pyc
--rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.1.0.1/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.1.0.1/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.1.0.1/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.1.0.1/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14094 2023-06-23 11:02:51.692877 sfctools-1.1.0.1/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.1.0.1/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.1.0.1/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.1.0.1/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     3096 2023-06-23 11:02:51.692877 sfctools-1.1.0.1/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      591 2023-06-23 11:02:51.693876 sfctools-1.1.0.1/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     1089 2023-06-23 17:29:32.294856 sfctools-1.1.0.1/sfctools/examples/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      865 2023-06-23 17:20:20.493314 sfctools-1.1.0.1/sfctools/examples/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5634 2023-06-23 17:29:32.297478 sfctools-1.1.0.1/sfctools/examples/__pycache__/balance.cpython-311.pyc
--rw-r--r--   0        0        0     2927 2023-05-04 16:23:19.857662 sfctools-1.1.0.1/sfctools/examples/__pycache__/balance.cpython-38.pyc
--rw-r--r--   0        0        0     2546 2023-06-23 17:29:32.304466 sfctools-1.1.0.1/sfctools/examples/__pycache__/clock.cpython-311.pyc
--rw-r--r--   0        0        0     1438 2023-05-04 16:23:19.865976 sfctools-1.1.0.1/sfctools/examples/__pycache__/clock.cpython-38.pyc
--rw-r--r--   0        0        0     2299 2023-06-23 17:29:32.298470 sfctools-1.1.0.1/sfctools/examples/__pycache__/example_wrapper.cpython-311.pyc
--rw-r--r--   0        0        0     1589 2023-06-23 17:20:20.497529 sfctools-1.1.0.1/sfctools/examples/__pycache__/example_wrapper.cpython-38.pyc
--rw-r--r--   0        0        0     7433 2023-06-23 17:29:32.330267 sfctools-1.1.0.1/sfctools/examples/__pycache__/flowmatrix.cpython-311.pyc
--rw-r--r--   0        0        0     3815 2023-05-04 16:23:19.896381 sfctools-1.1.0.1/sfctools/examples/__pycache__/flowmatrix.cpython-38.pyc
--rw-r--r--   0        0        0     2430 2023-06-23 17:29:32.317580 sfctools-1.1.0.1/sfctools/examples/__pycache__/hello_agent.cpython-311.pyc
--rw-r--r--   0        0        0     1407 2023-05-04 16:23:19.880081 sfctools-1.1.0.1/sfctools/examples/__pycache__/hello_agent.cpython-38.pyc
--rw-r--r--   0        0        0     2904 2023-06-23 17:29:32.327467 sfctools-1.1.0.1/sfctools/examples/__pycache__/inventory.cpython-311.pyc
--rw-r--r--   0        0        0     1631 2023-06-23 17:20:20.539877 sfctools-1.1.0.1/sfctools/examples/__pycache__/inventory.cpython-38.pyc
--rw-r--r--   0        0        0     7815 2023-07-04 09:25:31.243629 sfctools-1.1.0.1/sfctools/examples/__pycache__/order_book.cpython-311.pyc
--rw-r--r--   0        0        0     4083 2023-06-23 17:20:20.505936 sfctools-1.1.0.1/sfctools/examples/__pycache__/order_book.cpython-38.pyc
--rw-r--r--   0        0        0     2370 2023-06-23 17:29:32.331741 sfctools-1.1.0.1/sfctools/examples/__pycache__/readme_example.cpython-311.pyc
--rw-r--r--   0        0        0     1492 2023-06-23 17:20:20.544044 sfctools-1.1.0.1/sfctools/examples/__pycache__/readme_example.cpython-38.pyc
--rw-r--r--   0        0        0     3371 2023-06-23 17:29:32.326597 sfctools-1.1.0.1/sfctools/examples/__pycache__/signal_slot.cpython-311.pyc
--rw-r--r--   0        0        0     1972 2023-06-23 17:20:20.536883 sfctools-1.1.0.1/sfctools/examples/__pycache__/signal_slot.cpython-38.pyc
--rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.1.0.1/sfctools/examples/balance.py
--rw-r--r--   0        0        0     4200 2023-06-23 17:29:32.303465 sfctools-1.1.0.1/sfctools/examples/basic_example/__pycache__/basic_example.cpython-311.pyc
--rw-r--r--   0        0        0     2118 2023-06-23 17:20:20.515615 sfctools-1.1.0.1/sfctools/examples/basic_example/__pycache__/basic_example.cpython-38.pyc
--rw-r--r--   0        0        0     1811 2023-06-23 11:02:51.693876 sfctools-1.1.0.1/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.1.0.1/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.1.0.1/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1397 2023-06-23 11:02:51.694877 sfctools-1.1.0.1/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0     6132 2023-06-23 17:29:32.307784 sfctools-1.1.0.1/sfctools/examples/exampleabm/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     2852 2023-05-04 16:23:19.868021 sfctools-1.1.0.1/sfctools/examples/exampleabm/__pycache__/model.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0      193 2023-06-23 17:29:32.308467 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      175 2023-05-04 16:23:19.869741 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3570 2023-06-23 17:29:32.315468 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/government.cpython-311.pyc
--rw-r--r--   0        0        0     2090 2023-05-04 16:23:19.876662 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/government.cpython-38.pyc
--rw-r--r--   0        0        0     3820 2023-06-23 17:29:32.310826 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/household.cpython-311.pyc
--rw-r--r--   0        0        0     2150 2023-05-04 16:23:19.871660 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/household.cpython-38.pyc
--rw-r--r--   0        0        0     3694 2023-06-23 17:29:32.314595 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/production.cpython-311.pyc
--rw-r--r--   0        0        0     2340 2023-05-04 16:23:19.874661 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/production.cpython-38.pyc
--rw-r--r--   0        0        0     7341 2023-06-23 17:29:32.312947 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/transactions.cpython-311.pyc
--rw-r--r--   0        0        0     2821 2023-05-04 16:23:19.873541 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/__pycache__/transactions.cpython-38.pyc
--rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.1.0.1/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.1.0.1/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.1.0.1/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.1.0.1/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.1.0.1/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.1.0.1/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.1.0.1/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.1.0.1/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.1.0.1/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.1.0.1/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.1.0.1/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1249 2023-06-23 11:02:51.694877 sfctools-1.1.0.1/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     4589 2023-06-23 17:29:32.319829 sfctools-1.1.0.1/sfctools/examples/market_example/__pycache__/market.cpython-311.pyc
--rw-r--r--   0        0        0     2791 2023-06-23 17:20:20.525903 sfctools-1.1.0.1/sfctools/examples/market_example/__pycache__/market.cpython-38.pyc
--rw-r--r--   0        0        0     6554 2023-06-23 17:29:32.322688 sfctools-1.1.0.1/sfctools/examples/market_example/__pycache__/market2.cpython-311.pyc
--rw-r--r--   0        0        0     3805 2023-06-23 17:20:20.530041 sfctools-1.1.0.1/sfctools/examples/market_example/__pycache__/market2.cpython-38.pyc
--rw-r--r--   0        0        0     1839 2023-06-23 11:02:51.695876 sfctools-1.1.0.1/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2791 2023-06-23 11:02:51.695876 sfctools-1.1.0.1/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0     5950 2023-06-23 17:29:32.324921 sfctools-1.1.0.1/sfctools/examples/monte_carlo/__pycache__/monte_carlo.cpython-311.pyc
--rw-r--r--   0        0        0     3075 2023-06-23 17:20:20.533690 sfctools-1.1.0.1/sfctools/examples/monte_carlo/__pycache__/monte_carlo.cpython-38.pyc
--rw-r--r--   0        0        0     2548 2023-06-23 11:02:51.696877 sfctools-1.1.0.1/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0       28 2023-07-04 09:25:31.728773 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/errors.txt
--rw-r--r--   0        0        0      450 2023-07-04 09:25:31.788773 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.0
--rw-r--r--   0        0        0      454 2023-07-04 09:25:31.845774 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.1
--rw-r--r--   0        0        0      443 2023-07-04 09:25:31.903287 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.2
--rw-r--r--   0        0        0      454 2023-07-04 09:25:31.962780 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.3
--rw-r--r--   0        0        0      455 2023-07-04 09:25:32.021780 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.4
--rw-r--r--   0        0        0      445 2023-07-04 09:25:32.078783 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.5
--rw-r--r--   0        0        0      458 2023-07-04 09:25:32.136778 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.6
--rw-r--r--   0        0        0      450 2023-07-04 09:25:32.192796 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.7
--rw-r--r--   0        0        0      451 2023-07-04 09:25:32.249779 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.8
--rw-r--r--   0        0        0      454 2023-07-04 09:25:32.305780 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.9
--rw-r--r--   0        0        0      537 2023-07-04 09:25:32.306779 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/output.txt
--rw-r--r--   0        0        0      258 2023-07-04 09:25:32.307068 sfctools-1.1.0.1/sfctools/examples/monte_carlo/results/progress.txt
--rw-r--r--   0        0        0      188 2023-06-23 11:02:51.697422 sfctools-1.1.0.1/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3907 2023-06-23 17:31:16.217873 sfctools-1.1.0.1/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.1.0.1/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0      798 2023-06-23 11:02:51.697878 sfctools-1.1.0.1/sfctools/examples/readme_example.py
--rw-r--r--   0        0        0     1561 2023-06-23 11:02:51.698876 sfctools-1.1.0.1/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0     1285 2023-06-23 11:02:51.698876 sfctools-1.1.0.1/sfctools/examples/worker_registry.py
--rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.1.0.1/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.1.0.1/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.1.0.1/sfctools/gui/__init__.py
--rw-r--r--   0        0        0      269 2023-01-25 08:23:20.061472 sfctools-1.1.0.1/sfctools/gui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      221 2023-01-25 08:17:49.221422 sfctools-1.1.0.1/sfctools/gui/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1128 2023-06-23 17:29:27.785287 sfctools-1.1.0.1/sfctools/gui/__pycache__/attune_main.cpython-311.pyc
--rw-r--r--   0        0        0      835 2023-04-04 07:45:30.299298 sfctools-1.1.0.1/sfctools/gui/__pycache__/attune_main.cpython-38.pyc
--rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.1.0.1/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.1.0.1/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0      177 2022-12-22 08:51:44.532604 sfctools-1.1.0.1/sfctools/gui/attune/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      159 2022-11-23 08:49:18.431057 sfctools-1.1.0.1/sfctools/gui/attune/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.1.0.1/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0      181 2022-12-22 08:51:44.534815 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      163 2022-11-23 08:49:18.433350 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    51801 2023-06-23 17:29:31.141165 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-311.pyc
--rw-r--r--   0        0        0    20359 2023-06-23 12:23:28.929321 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-38.pyc
--rw-r--r--   0        0        0    86739 2023-07-04 09:25:30.935664 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-311.pyc
--rw-r--r--   0        0        0    35342 2023-06-23 17:20:19.969633 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-38.pyc
--rw-r--r--   0        0        0    23682 2023-06-23 17:29:28.317264 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-311.pyc
--rw-r--r--   0        0        0    10483 2023-06-23 12:23:28.355204 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-38.pyc
--rw-r--r--   0        0        0    10883 2023-06-23 17:29:28.313067 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-311.pyc
--rw-r--r--   0        0        0     4813 2023-02-06 10:17:36.928510 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-38.pyc
--rw-r--r--   0        0        0     2913 2023-07-04 09:12:37.990559 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/my_interpolation.cpython-311.pyc
--rw-r--r--   0        0        0    32778 2023-06-23 17:29:28.323058 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/output_display.cpython-311.pyc
--rw-r--r--   0        0        0    12521 2023-04-04 07:45:30.873144 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/output_display.cpython-38.pyc
--rw-r--r--   0        0        0     2636 2023-06-23 17:29:28.309388 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2023-06-23 12:23:28.326179 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-38.pyc
--rw-r--r--   0        0        0   165773 2023-06-26 08:10:06.168054 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/qtattune.cpython-311.pyc
--rw-r--r--   0        0        0    69669 2023-06-23 17:20:18.298431 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/qtattune.cpython-38.pyc
--rw-r--r--   0        0        0     7007 2023-01-25 08:23:24.383425 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/resources.cpython-311.pyc
--rw-r--r--   0        0        0     6499 2022-11-23 08:49:30.377800 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/resources.cpython-38.pyc
--rw-r--r--   0        0        0    10549 2023-07-04 05:18:43.430986 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-311.pyc
--rw-r--r--   0        0        0     5060 2023-06-23 12:23:28.975064 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-38.pyc
--rw-r--r--   0        0        0    20267 2023-07-04 05:18:43.420374 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-311.pyc
--rw-r--r--   0        0        0     9582 2023-06-23 12:23:28.953960 sfctools-1.1.0.1/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-38.pyc
--rw-r--r--   0        0        0    34562 2023-06-23 11:02:51.699876 sfctools-1.1.0.1/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-06-23 11:02:51.699876 sfctools-1.1.0.1/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    76962 2023-07-04 09:26:32.597870 sfctools-1.1.0.1/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.1.0.1/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13478 2023-06-23 11:02:51.701876 sfctools-1.1.0.1/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.1.0.1/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.1.0.1/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0     1199 2023-07-04 09:26:32.598315 sfctools-1.1.0.1/sfctools/gui/attune/src/my_interpolation.py
--rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.1.0.1/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.1.0.1/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-06-23 11:02:51.701876 sfctools-1.1.0.1/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   137422 2023-06-23 17:31:16.220161 sfctools-1.1.0.1/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.1.0.1/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.1.0.1/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-06-23 11:02:51.703877 sfctools-1.1.0.1/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.1.0.1/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.1.0.1/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-07-04 09:26:12.233558 sfctools-1.1.0.1/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4018 2023-07-04 09:26:32.598315 sfctools-1.1.0.1/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.1.0.1/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.1.0.1/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.1.0.1/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.1.0.1/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6968 2023-07-04 09:26:32.599316 sfctools-1.1.0.1/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85083 2023-07-04 09:26:32.600535 sfctools-1.1.0.1/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11727 2023-07-04 09:26:32.601318 sfctools-1.1.0.1/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.1.0.1/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.1.0.1/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.1.0.1/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.1.0.1/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.1.0.1/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.1.0.1/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.1.0.1/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-06-23 11:02:51.705877 sfctools-1.1.0.1/sfctools/gui/sfctheme
--rw-r--r--   0        0        0     4765 2022-11-23 09:50:36.467143 sfctools-1.1.0.1/sfctools/MAMBA/__pycache__/mamba_interpreter2.cpython-38.pyc
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.1.0.1/sfctools/misc/__init__.py
--rw-r--r--   0        0        0      171 2023-01-25 08:23:20.056190 sfctools-1.1.0.1/sfctools/misc/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      153 2023-01-19 21:54:26.534886 sfctools-1.1.0.1/sfctools/misc/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    27049 2023-06-23 17:29:27.703960 sfctools-1.1.0.1/sfctools/misc/__pycache__/mpl_plotting.cpython-311.pyc
--rw-r--r--   0        0        0    15416 2023-06-23 17:20:18.243867 sfctools-1.1.0.1/sfctools/misc/__pycache__/mpl_plotting.cpython-38.pyc
--rw-r--r--   0        0        0    12386 2023-06-23 17:29:27.488369 sfctools-1.1.0.1/sfctools/misc/__pycache__/reporting_sheet.cpython-311.pyc
--rw-r--r--   0        0        0     7616 2023-04-04 07:45:30.288586 sfctools-1.1.0.1/sfctools/misc/__pycache__/reporting_sheet.cpython-38.pyc
--rw-r--r--   0        0        0    12006 2023-01-25 08:23:21.230666 sfctools-1.1.0.1/sfctools/misc/__pycache__/timeseries.cpython-311.pyc
--rw-r--r--   0        0        0     6420 2023-01-25 08:17:49.793565 sfctools-1.1.0.1/sfctools/misc/__pycache__/timeseries.cpython-38.pyc
--rw-r--r--   0        0        0    21989 2023-06-23 11:02:51.706741 sfctools-1.1.0.1/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.1.0.1/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.1.0.1/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 sfctools-1.1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.1.0.2/LICENSE
+-rw-r--r--   0        0        0     1620 2023-07-04 09:46:03.075401 sfctools-1.1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1865 2023-06-23 11:07:04.102942 sfctools-1.1.0.2/README.md
+-rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.1.0.2/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.1.0.2/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.1.0.2/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.1.0.2/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.1.0.2/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.1.0.2/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.1.0.2/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.1.0.2/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.1.0.2/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.1.0.2/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.1.0.2/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.1.0.2/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.1.0.2/sfctools/core/__init__.py
+-rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.1.0.2/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.1.0.2/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.1.0.2/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15252 2023-06-23 11:02:51.691877 sfctools-1.1.0.2/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.1.0.2/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.1.0.2/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.1.0.2/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.1.0.2/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.1.0.2/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.1.0.2/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.1.0.2/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.1.0.2/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14094 2023-06-23 11:02:51.692877 sfctools-1.1.0.2/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.1.0.2/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.1.0.2/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.1.0.2/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     3096 2023-06-23 11:02:51.692877 sfctools-1.1.0.2/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      591 2023-06-23 11:02:51.693876 sfctools-1.1.0.2/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.1.0.2/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1811 2023-06-23 11:02:51.693876 sfctools-1.1.0.2/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.1.0.2/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.1.0.2/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1397 2023-06-23 11:02:51.694877 sfctools-1.1.0.2/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.1.0.2/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.1.0.2/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.1.0.2/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.1.0.2/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.1.0.2/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.1.0.2/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.1.0.2/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.1.0.2/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1249 2023-06-23 11:02:51.694877 sfctools-1.1.0.2/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1839 2023-06-23 11:02:51.695876 sfctools-1.1.0.2/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2791 2023-06-23 11:02:51.695876 sfctools-1.1.0.2/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0     2548 2023-06-23 11:02:51.696877 sfctools-1.1.0.2/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0      188 2023-06-23 11:02:51.697422 sfctools-1.1.0.2/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3907 2023-06-23 17:31:16.217873 sfctools-1.1.0.2/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.1.0.2/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0      798 2023-06-23 11:02:51.697878 sfctools-1.1.0.2/sfctools/examples/readme_example.py
+-rw-r--r--   0        0        0     1561 2023-06-23 11:02:51.698876 sfctools-1.1.0.2/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0     1285 2023-06-23 11:02:51.698876 sfctools-1.1.0.2/sfctools/examples/worker_registry.py
+-rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.1.0.2/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.1.0.2/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.1.0.2/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.1.0.2/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.1.0.2/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.1.0.2/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0    34562 2023-06-23 11:02:51.699876 sfctools-1.1.0.2/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-06-23 11:02:51.699876 sfctools-1.1.0.2/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    76992 2023-07-04 09:46:03.076666 sfctools-1.1.0.2/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.1.0.2/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13478 2023-06-23 11:02:51.701876 sfctools-1.1.0.2/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.1.0.2/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.1.0.2/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0     1199 2023-07-04 09:26:32.598315 sfctools-1.1.0.2/sfctools/gui/attune/src/my_interpolation.py
+-rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.1.0.2/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.1.0.2/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-06-23 11:02:51.701876 sfctools-1.1.0.2/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   137422 2023-06-23 17:31:16.220161 sfctools-1.1.0.2/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.1.0.2/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.1.0.2/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-06-23 11:02:51.703877 sfctools-1.1.0.2/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.1.0.2/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.1.0.2/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-07-04 09:26:12.233558 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4018 2023-07-04 09:26:32.598315 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6968 2023-07-04 09:26:32.599316 sfctools-1.1.0.2/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85503 2023-07-04 09:46:03.077402 sfctools-1.1.0.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11727 2023-07-04 09:26:32.601318 sfctools-1.1.0.2/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.1.0.2/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.1.0.2/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.1.0.2/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.1.0.2/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.1.0.2/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.1.0.2/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.1.0.2/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-06-23 11:02:51.705877 sfctools-1.1.0.2/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.1.0.2/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0    21989 2023-06-23 11:02:51.706741 sfctools-1.1.0.2/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.1.0.2/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.1.0.2/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 sfctools-1.1.0.2/PKG-INFO
```

### Comparing `sfctools-1.1.0.1/LICENSE` & `sfctools-1.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/pyproject.toml` & `sfctools-1.1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.1.0.1"
+version = "1.1.0.2"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.1.0.1/README.md` & `sfctools-1.1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/__init__.py` & `sfctools-1.1.0.2/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/__main__.py` & `sfctools-1.1.0.2/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/automation/calibration.py` & `sfctools-1.1.0.2/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/automation/cgesolver.py` & `sfctools-1.1.0.2/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/automation/runner.py` & `sfctools-1.1.0.2/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/bottomup/matching.py` & `sfctools-1.1.0.2/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/bottomup/productiontree.py` & `sfctools-1.1.0.2/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/bottomup/stock_manager.py` & `sfctools-1.1.0.2/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/bottomup/treestruct.py` & `sfctools-1.1.0.2/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/core/agent.py` & `sfctools-1.1.0.2/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/core/clock.py` & `sfctools-1.1.0.2/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/core/flow_matrix.py` & `sfctools-1.1.0.2/sfctools/core/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/core/settings.py` & `sfctools-1.1.0.2/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/core/singleton.py` & `sfctools-1.1.0.2/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/core/world.py` & `sfctools-1.1.0.2/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/balance.py` & `sfctools-1.1.0.2/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/bank_order_book.py` & `sfctools-1.1.0.2/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.1.0.2/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/collection.py` & `sfctools-1.1.0.2/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/income_statement.py` & `sfctools-1.1.0.2/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/inventory.py` & `sfctools-1.1.0.2/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/market_registry.py` & `sfctools-1.1.0.2/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/signalslot.py` & `sfctools-1.1.0.2/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/datastructs/worker_registry.py` & `sfctools-1.1.0.2/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/__init__.py` & `sfctools-1.1.0.2/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/balance.py` & `sfctools-1.1.0.2/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.1.0.2/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/clock.py` & `sfctools-1.1.0.2/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/example_wrapper.py` & `sfctools-1.1.0.2/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/info.md` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/model.py` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.1.0.2/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/flowmatrix.py` & `sfctools-1.1.0.2/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/hello_agent.py` & `sfctools-1.1.0.2/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/inventory.py` & `sfctools-1.1.0.2/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/market_example/market.py` & `sfctools-1.1.0.2/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/market_example/market2.py` & `sfctools-1.1.0.2/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.1.0.2/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/order_book.py` & `sfctools-1.1.0.2/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/readme_example.py` & `sfctools-1.1.0.2/sfctools/examples/readme_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/signal_slot.py` & `sfctools-1.1.0.2/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/examples/worker_registry.py` & `sfctools-1.1.0.2/sfctools/examples/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.1.0.2/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/draw_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1444,15 +1444,15 @@
                 qp.drawRect(0,0,self.W-2,self.H-4)
         else:
             if reference == self:
                 qp.drawRect(0,0,self.W-2,self.H-4)
 
 
         # draw grid 
-        if self.show_raster:
+        if self.main_widget.checkBox_raster_2.isChecked():
             for i in np.arange(0, int(self.W-2), self.raster_size):
                 for j in np.arange(0, int(self.H-2),self.raster_size):
                     qp.drawRect(int(i)-1,int(j)-1,2,2)
 
         # pen2 = QtGui.QPen(self.parent().theme_manager.get_color(2),1)
         # qp.setPen(pen2)
         # qp.drawRect(0+self.gox,0+self.goy,self.gox + self.W-2,self.goy + self.H-2)
```

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/my_interpolation.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/my_interpolation.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/output_display.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/qtattune.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/resources.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.1.0.2/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files 0% similar despite different names*

#### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.1.0.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

```diff
@@ -2037,15 +2037,31 @@
                 <x>20</x>
                 <y>220</y>
                 <width>111</width>
                 <height>41</height>
               </rect>
             </property>
             <property name="text">
-              <string>use Raster</string>
+              <string>Use raster</string>
+            </property>
+            <property name="checked">
+              <bool>false</bool>
+            </property>
+          </widget>
+          <widget class="QCheckBox" name="checkBox_raster_2">
+            <property name="geometry">
+              <rect>
+                <x>120</x>
+                <y>220</y>
+                <width>111</width>
+                <height>41</height>
+              </rect>
+            </property>
+            <property name="text">
+              <string>Show raster</string>
             </property>
             <property name="checked">
               <bool>false</bool>
             </property>
           </widget>
         </widget>
         <widget class="QGroupBox" name="groupBox_3">
```

### Comparing `sfctools-1.1.0.1/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.1.0.2/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/CLA.pdf` & `sfctools-1.1.0.2/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.1.0.2/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/LICENSE` & `sfctools-1.1.0.2/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/gui/README.md` & `sfctools-1.1.0.2/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/misc/mpl_plotting.py` & `sfctools-1.1.0.2/sfctools/misc/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/misc/reporting_sheet.py` & `sfctools-1.1.0.2/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/sfctools/misc/timeseries.py` & `sfctools-1.1.0.2/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.1/PKG-INFO` & `sfctools-1.1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.1.0.1
+Version: 1.1.0.2
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
```

