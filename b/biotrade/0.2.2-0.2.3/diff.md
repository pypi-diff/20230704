# Comparing `tmp/biotrade-0.2.2.tar.gz` & `tmp/biotrade-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotrade-0.2.2.tar", last modified: Mon Jun 26 15:40:41 2023, max compression
+gzip compressed data, was "biotrade-0.2.3.tar", last modified: Tue Jul  4 13:21:25 2023, max compression
```

## Comparing `biotrade-0.2.2.tar` & `biotrade-0.2.3.tar`

### file list

```diff
@@ -1,95 +1,94 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.177583 biotrade-0.2.2/
--rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.2.2/LICENCE.md
--rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.2.2/MANIFEST.in
--rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.2.2/NOTICE.txt
--rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-06-26 15:40:41.177583 biotrade-0.2.2/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     7600 2023-06-26 14:05:44.000000 biotrade-0.2.2/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.157583 biotrade-0.2.2/biotrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     3634 2023-06-26 15:28:17.000000 biotrade-0.2.2/biotrade/__init__.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.161583 biotrade-0.2.2/biotrade/common/
--rw-r--r--   0 paul      (1000) paul      (1000)    13743 2023-06-26 13:47:11.000000 biotrade-0.2.2/biotrade/common/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)    20436 2023-05-10 16:55:49.000000 biotrade-0.2.2/biotrade/common/compare.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/common/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5715 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/common/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/common/logger.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/common/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3921 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/common/reallocate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/common/sanitize.py
--rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/common/time_series.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.2.2/biotrade/common/update.py
--rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.2.2/biotrade/common/url_request_header.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.161583 biotrade-0.2.2/biotrade/comtrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/comtrade/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.2.2/biotrade/comtrade/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.2.2/biotrade/comtrade/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    20253 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/comtrade/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6819 2023-06-26 13:47:11.000000 biotrade-0.2.2/biotrade/comtrade/dump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/comtrade/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    46862 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/comtrade/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/comtrade/quality.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.169583 biotrade-0.2.2/biotrade/config_data/
--rw-r--r--   0 paul      (1000) paul      (1000)     3860 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/config_data/column_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6719 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/config_data/comtrade_faostat_product_mapping.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.2.2/biotrade/config_data/comtrade_hs_2d.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.2.2/biotrade/config_data/comtrade_hs_product_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.2.2/biotrade/config_data/comtrade_reporters.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4713 2023-03-08 17:45:22.000000 biotrade-0.2.2/biotrade/config_data/faostat_commodity_tree.csv
--rw-r--r--   0 paul      (1000) paul      (1000)    43339 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/config_data/faostat_country_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.2.2/biotrade/config_data/faostat_forestry_production_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.2.2/biotrade/config_data/faostat_forestry_production_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.2.2/biotrade/config_data/faostat_forestry_trade_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.2.2/biotrade/config_data/faostat_products_name_code_shortname.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.2.2/biotrade/config_data/regulation_front_end_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)   233668 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/config_data/regulation_products.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.2.2/biotrade/config_data/wood_product_aggregates.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.169583 biotrade-0.2.2/biotrade/eurostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.2.2/biotrade/eurostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4632 2023-06-26 14:05:44.000000 biotrade-0.2.2/biotrade/eurostat/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.173583 biotrade-0.2.2/biotrade/faostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/faostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.2.2/biotrade/faostat/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.2.2/biotrade/faostat/coefficients.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/faostat/convert.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/faostat/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:47:11.000000 biotrade-0.2.2/biotrade/faostat/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    23448 2023-03-21 11:14:58.000000 biotrade-0.2.2/biotrade/faostat/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4179 2023-06-08 08:14:15.000000 biotrade-0.2.2/biotrade/faostat/mirror.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/faostat/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    18105 2023-05-10 13:26:24.000000 biotrade-0.2.2/biotrade/faostat/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/faostat/quality.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/faostat/share_coefficients.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.173583 biotrade-0.2.2/biotrade/hwp/
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.2.2/biotrade/hwp/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/hwp/country.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.173583 biotrade-0.2.2/biotrade/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/tests/test_aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3469 2023-06-26 13:50:21.000000 biotrade-0.2.2/biotrade/tests/test_front_end.py
--rw-r--r--   0 paul      (1000) paul      (1000)      837 2023-05-15 17:30:05.000000 biotrade-0.2.2/biotrade/tests/test_mirror.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3145 2023-06-26 13:47:11.000000 biotrade-0.2.2/biotrade/tests/test_reallocate.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.173583 biotrade-0.2.2/biotrade/world_bank/
--rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/world_bank/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.2.2/biotrade/world_bank/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     9162 2023-05-15 15:21:01.000000 biotrade-0.2.2/biotrade/world_bank/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.157583 biotrade-0.2.2/biotrade.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-06-26 15:40:41.000000 biotrade-0.2.2/biotrade.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     2754 2023-06-26 15:40:41.000000 biotrade-0.2.2/biotrade.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-06-26 15:40:41.000000 biotrade-0.2.2/biotrade.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      130 2023-06-26 15:40:41.000000 biotrade-0.2.2/biotrade.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       43 2023-06-26 15:40:41.000000 biotrade-0.2.2/biotrade.egg-info/top_level.txt
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.153583 biotrade-0.2.2/scripts/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.177583 biotrade-0.2.2/scripts/front_end/
--rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.2.2/scripts/front_end/DEPRECATED_reporter_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2583 2023-06-26 13:50:21.000000 biotrade-0.2.2/scripts/front_end/annual_variation_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6803 2023-03-21 11:14:58.000000 biotrade-0.2.2/scripts/front_end/annual_variation_trade_quantity_value.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3571 2023-06-26 13:50:21.000000 biotrade-0.2.2/scripts/front_end/average_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)    10277 2023-03-21 11:14:58.000000 biotrade-0.2.2/scripts/front_end/average_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.2.2/scripts/front_end/db_scheduler.py
--rw-r--r--   0 paul      (1000) paul      (1000)    27701 2023-06-26 13:50:21.000000 biotrade-0.2.2/scripts/front_end/functions.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.2.2/scripts/front_end/product_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3669 2023-03-21 11:14:58.000000 biotrade-0.2.2/scripts/front_end/trends_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.2.2/scripts/front_end/trends_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)      346 2022-08-08 14:29:00.000000 biotrade-0.2.2/scripts/front_end/update_db.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-26 15:40:41.177583 biotrade-0.2.2/scripts/quality/
--rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.2.2/scripts/quality/faostat_compare_aggregates_to_constituents.py
--rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-06-26 15:40:41.177583 biotrade-0.2.2/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1651 2023-06-26 15:28:17.000000 biotrade-0.2.2/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.517373 biotrade-0.2.3/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.2.3/LICENCE.md
+-rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.2.3/MANIFEST.in
+-rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.2.3/NOTICE.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-07-04 13:21:25.517373 biotrade-0.2.3/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7600 2023-06-26 14:05:44.000000 biotrade-0.2.3/README.md
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.505375 biotrade-0.2.3/biotrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3634 2023-07-04 13:20:44.000000 biotrade-0.2.3/biotrade/__init__.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.509375 biotrade-0.2.3/biotrade/common/
+-rw-r--r--   0 paul      (1000) paul      (1000)    13743 2023-06-26 13:47:11.000000 biotrade-0.2.3/biotrade/common/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    20436 2023-05-10 16:55:49.000000 biotrade-0.2.3/biotrade/common/compare.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/common/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5715 2023-07-04 06:37:21.000000 biotrade-0.2.3/biotrade/common/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/common/logger.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/common/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3929 2023-07-04 13:06:38.000000 biotrade-0.2.3/biotrade/common/reallocate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/common/sanitize.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/common/time_series.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.2.3/biotrade/common/update.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.2.3/biotrade/common/url_request_header.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.509375 biotrade-0.2.3/biotrade/comtrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:50:21.000000 biotrade-0.2.3/biotrade/comtrade/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.2.3/biotrade/comtrade/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.2.3/biotrade/comtrade/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    20233 2023-07-04 08:14:43.000000 biotrade-0.2.3/biotrade/comtrade/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6819 2023-06-26 13:47:11.000000 biotrade-0.2.3/biotrade/comtrade/dump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/comtrade/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    46862 2023-06-26 13:50:21.000000 biotrade-0.2.3/biotrade/comtrade/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/comtrade/quality.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.513374 biotrade-0.2.3/biotrade/config_data/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3860 2023-06-26 13:50:21.000000 biotrade-0.2.3/biotrade/config_data/column_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6719 2023-06-26 13:50:21.000000 biotrade-0.2.3/biotrade/config_data/comtrade_faostat_product_mapping.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.2.3/biotrade/config_data/comtrade_hs_2d.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.2.3/biotrade/config_data/comtrade_hs_product_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.2.3/biotrade/config_data/comtrade_reporters.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     5480 2023-07-04 13:18:13.000000 biotrade-0.2.3/biotrade/config_data/faostat_commodity_tree.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)    43339 2023-06-26 13:50:21.000000 biotrade-0.2.3/biotrade/config_data/faostat_country_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.2.3/biotrade/config_data/faostat_forestry_production_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.2.3/biotrade/config_data/faostat_forestry_production_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.2.3/biotrade/config_data/faostat_forestry_trade_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.2.3/biotrade/config_data/faostat_products_name_code_shortname.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.2.3/biotrade/config_data/regulation_front_end_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)   233668 2023-06-26 13:50:21.000000 biotrade-0.2.3/biotrade/config_data/regulation_products.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.2.3/biotrade/config_data/wood_product_aggregates.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.513374 biotrade-0.2.3/biotrade/eurostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.2.3/biotrade/eurostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4632 2023-06-26 14:05:44.000000 biotrade-0.2.3/biotrade/eurostat/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.513374 biotrade-0.2.3/biotrade/faostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/faostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.2.3/biotrade/faostat/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.2.3/biotrade/faostat/coefficients.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/faostat/convert.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/faostat/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-06-26 13:47:11.000000 biotrade-0.2.3/biotrade/faostat/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    23993 2023-07-04 08:14:43.000000 biotrade-0.2.3/biotrade/faostat/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4179 2023-06-08 08:14:15.000000 biotrade-0.2.3/biotrade/faostat/mirror.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/faostat/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    18105 2023-05-10 13:26:24.000000 biotrade-0.2.3/biotrade/faostat/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/faostat/quality.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/faostat/share_coefficients.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.513374 biotrade-0.2.3/biotrade/hwp/
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.2.3/biotrade/hwp/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/hwp/country.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.513374 biotrade-0.2.3/biotrade/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/tests/test_aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3469 2023-06-26 13:50:21.000000 biotrade-0.2.3/biotrade/tests/test_front_end.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      837 2023-05-15 17:30:05.000000 biotrade-0.2.3/biotrade/tests/test_mirror.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3157 2023-07-04 13:06:38.000000 biotrade-0.2.3/biotrade/tests/test_reallocate.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.517373 biotrade-0.2.3/biotrade/world_bank/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/world_bank/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.2.3/biotrade/world_bank/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9162 2023-05-15 15:21:01.000000 biotrade-0.2.3/biotrade/world_bank/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.509375 biotrade-0.2.3/biotrade.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     8357 2023-07-04 13:21:25.000000 biotrade-0.2.3/biotrade.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     2723 2023-07-04 13:21:25.000000 biotrade-0.2.3/biotrade.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-07-04 13:21:25.000000 biotrade-0.2.3/biotrade.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      130 2023-07-04 13:21:25.000000 biotrade-0.2.3/biotrade.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       43 2023-07-04 13:21:25.000000 biotrade-0.2.3/biotrade.egg-info/top_level.txt
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.505375 biotrade-0.2.3/scripts/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.517373 biotrade-0.2.3/scripts/front_end/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.2.3/scripts/front_end/DEPRECATED_reporter_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2583 2023-06-26 13:50:21.000000 biotrade-0.2.3/scripts/front_end/annual_variation_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6622 2023-07-04 08:14:43.000000 biotrade-0.2.3/scripts/front_end/annual_variation_trade_quantity_value.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3571 2023-06-26 13:50:21.000000 biotrade-0.2.3/scripts/front_end/average_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    10192 2023-07-04 08:14:43.000000 biotrade-0.2.3/scripts/front_end/average_trade_quantity.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.2.3/scripts/front_end/db_scheduler.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    27527 2023-07-04 08:14:43.000000 biotrade-0.2.3/scripts/front_end/functions.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.2.3/scripts/front_end/product_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3819 2023-07-04 08:14:43.000000 biotrade-0.2.3/scripts/front_end/trends_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.2.3/scripts/front_end/trends_trade_quantity.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-04 13:21:25.517373 biotrade-0.2.3/scripts/quality/
+-rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.2.3/scripts/quality/faostat_compare_aggregates_to_constituents.py
+-rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-07-04 13:21:25.517373 biotrade-0.2.3/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1651 2023-07-04 13:20:44.000000 biotrade-0.2.3/setup.py
```

### Comparing `biotrade-0.2.2/LICENCE.md` & `biotrade-0.2.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/NOTICE.txt` & `biotrade-0.2.3/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/PKG-INFO` & `biotrade-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.2.2
+Version: 0.2.3
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `biotrade-0.2.2/README.md` & `biotrade-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/__init__.py` & `biotrade-0.2.3/biotrade/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     >>> print("database_url:", biotrade.database_url)
 
 """
 
 from pathlib import Path
 import os
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 module_dir = Path(__file__).resolve().parent
 
 # Where is the data, default case
 data_dir = Path.home() / "repos/forobs/biotrade_data/"
 
 # But you can override that with an environment variable
```

### Comparing `biotrade-0.2.2/biotrade/common/aggregate.py` & `biotrade-0.2.3/biotrade/common/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/compare.py` & `biotrade-0.2.3/biotrade/common/compare.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/country.py` & `biotrade-0.2.3/biotrade/common/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/database.py` & `biotrade-0.2.3/biotrade/common/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/logger.py` & `biotrade-0.2.3/biotrade/common/logger.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/products.py` & `biotrade-0.2.3/biotrade/common/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/reallocate.py` & `biotrade-0.2.3/biotrade/common/reallocate.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,21 +68,22 @@
 def split_by_partners(
     df_prod: pandas.DataFrame,
     df_trade: pandas.DataFrame,
     allocation_step: int,
 ) -> pandas.DataFrame:
     """Reallocate a quantity, by splitting it between different trade partners"""
     index = ["reporter", "primary_product", "year"]
-    # Add optional code columns only if they are present in df
+    # Add optional code columns if they are present in df
     optional_cols = ["reporter_code", "primary_product_code"]
-    index += [col for col in optional_cols if col in df_trade.columns]
-    df = df_prod.merge(df_trade, on=index, how="left")
+    optional_cols = [col for col in optional_cols if col in df_trade.columns]
+    df = df_prod.merge(df_trade, on=index + optional_cols, how="left")
     # Compute the proportion among all trade partners
-    index = ["primary_product", "year"]
-    df["prop"] = df.groupby(index)["import_quantity"].transform(lambda x: x / x.sum())
+    df["prop"] = df.groupby(index + optional_cols)["import_quantity"].transform(
+        lambda x: x / x.sum()
+    )
     var_this_step = f"primary_eq_imp_{allocation_step}"
     var_previous_step = f"primary_eq_imp_{allocation_step - 1}"
     # Reallocate the import to partners according to the proportion
     df[var_this_step] = df[var_previous_step] * df["prop"]
     return df
```

### Comparing `biotrade-0.2.2/biotrade/common/sanitize.py` & `biotrade-0.2.3/biotrade/common/sanitize.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/time_series.py` & `biotrade-0.2.3/biotrade/common/time_series.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/update.py` & `biotrade-0.2.3/biotrade/common/update.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/common/url_request_header.py` & `biotrade-0.2.3/biotrade/common/url_request_header.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/comtrade/__init__.py` & `biotrade-0.2.3/biotrade/comtrade/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/comtrade/aggregate.py` & `biotrade-0.2.3/biotrade/comtrade/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/comtrade/country_groups.py` & `biotrade-0.2.3/biotrade/comtrade/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/comtrade/database.py` & `biotrade-0.2.3/biotrade/comtrade/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,18 @@
 
         # Create the schema if it doesn't exist.
         # Exclude the SQLite engine because there is only a default schemas for that engine.
         # And the SQLite dialect doesn't have a has_schema() method.
         if hasattr(self.engine.dialect, "has_schema") and callable(
             getattr(self.engine.dialect, "has_schema")
         ):
-            if not self.engine.dialect.has_schema(self.engine, self.schema):
-                self.engine.execute(CreateSchema(self.schema))
+            with self.engine.connect() as conn:
+                if not self.engine.dialect.has_schema(conn, self.schema):
+                    conn.execute(CreateSchema(self.schema))
+                    conn.commit()
 
         # Describe table metadata and create them if they don't exist
         # Product table
         self.product = self.describe_product_table(name="product")
         # Trade tables with data at the HS 6 digit level
         self.monthly = self.describe_trade_table(name="monthly")
         self.yearly = self.describe_trade_table(name="yearly")
@@ -200,15 +202,17 @@
             ),
             schema=self.schema,
         )
         return table
 
     def read_sql_query(self, stmt):
         """A wrapper around pandas.read_sql_query"""
-        return pandas.read_sql_query(stmt, self.engine)
+        with self.engine.connect() as conn:
+            df = pandas.read_sql_query(stmt, conn)
+        return df
 
     def check_data_presence(
         self,
         table,
         start_year,
         end_year,
         frequency,
@@ -385,33 +389,29 @@
         regex_pat = re.compile(r"\W+")
         # flow data
         flow_data = comtradeapicall.getReference("flow")[["id", "text"]].rename(
             columns={"id": "flow_code", "text": "flow"}
         )
         # rename flow column content to snake case using the compiled regex
         flow_data["flow"] = (
-            flow_data["flow"]
-            .str.replace(regex_pat, "_", regex=True)
-            .str.lower()
+            flow_data["flow"].str.replace(regex_pat, "_", regex=True).str.lower()
         )
         # mode of transport data
         mot_data = (
             comtradeapicall.getReference("mot")[["id", "text"]]
             .astype({"id": int})
             .rename(
                 columns={
                     "id": "mode_of_transport_code",
                     "text": "mode_of_transport",
                 }
             )
         )
         # custom procedure data
-        customs_data = comtradeapicall.getReference("customs")[
-            ["id", "text"]
-        ].rename(
+        customs_data = comtradeapicall.getReference("customs")[["id", "text"]].rename(
             columns={
                 "id": "customs_proc_code",
                 "text": "customs",
             }
         )
         if reporter is not None:
             # Obtain codes from reporter data
@@ -437,31 +437,28 @@
             stmt = stmt.where(table.c.reporter_code.in_(reporter_code))
         if partner_code is not None:
             stmt = stmt.where(table.c.partner_code.in_(partner_code))
         if product_code is not None:
             stmt = stmt.where(table.c.product_code.in_(product_code))
         if product_code_start is not None:
             stmt = stmt.where(
-                or_(
-                    table.c.product_code.ilike(f"{c}%")
-                    for c in product_code_start
-                )
+                or_(table.c.product_code.ilike(f"{c}%") for c in product_code_start)
             )
         if flow is not None:
             # Rename flow list to snake case using the compiled regex
             flow = [regex_pat.sub("_", item).lower() for item in flow]
             # Obtain codes from flow data
             flow_code = flow_data[flow_data.flow.isin(flow)].flow_code.tolist()
             stmt = stmt.where(table.c.flow_code.in_(flow_code))
         if period_start is not None:
             stmt = stmt.where(table.c.period >= period_start)
         if period_end is not None:
             stmt = stmt.where(table.c.period <= period_end)
         # Query the database and return a data frame
-        df = pandas.read_sql_query(stmt, self.engine)
+        df = self.read_sql_query(stmt)
         # Merge with complementary data
         df = (
             df.merge(reporter_data, on="reporter_code", how="left")
             .merge(partner_data, on="partner_code", how="left")
             .merge(quantity_data, on="unit_code", how="left")
             .merge(flow_data, on="flow_code", how="left")
             .merge(mot_data, on="mode_of_transport_code", how="left")
@@ -484,17 +481,15 @@
         # Remove empty columns
         not_empty = [col for col in df.columns if not all(df[col].isna())]
         df = df[not_empty]
         # This can be removed once this is dealt with in comtrade/pump.py
         # Rename column content to snake case using a compiled regex
         regex_pat = re.compile(r"\W+")
         if "flow" in df.columns:
-            df["flow"] = (
-                df["flow"].str.replace(regex_pat, "_", regex=True).str.lower()
-            )
+            df["flow"] = df["flow"].str.replace(regex_pat, "_", regex=True).str.lower()
             # Remove the plural "s"
             df["flow"] = df["flow"].str.replace("s", "", regex=True)
         # TODO: Change period to a date time object
         # Reshape to long format
         value_cols = ["net_weight", "trade_value"]
         index = set(df.columns) - set(value_cols)
         df_long = df.melt(
```

### Comparing `biotrade-0.2.2/biotrade/comtrade/dump.py` & `biotrade-0.2.3/biotrade/comtrade/dump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/comtrade/products.py` & `biotrade-0.2.3/biotrade/comtrade/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/comtrade/pump.py` & `biotrade-0.2.3/biotrade/comtrade/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/comtrade/quality.py` & `biotrade-0.2.3/biotrade/comtrade/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/column_names.csv` & `biotrade-0.2.3/biotrade/config_data/column_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/comtrade_faostat_product_mapping.csv` & `biotrade-0.2.3/biotrade/config_data/comtrade_faostat_product_mapping.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/comtrade_hs_2d.csv` & `biotrade-0.2.3/biotrade/config_data/comtrade_hs_2d.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/comtrade_hs_product_short_names.csv` & `biotrade-0.2.3/biotrade/config_data/comtrade_hs_product_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/comtrade_reporters.csv` & `biotrade-0.2.3/biotrade/config_data/comtrade_reporters.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/faostat_commodity_tree.csv` & `biotrade-0.2.3/biotrade/config_data/faostat_commodity_tree.csv`

 * *Files 16% similar despite different names*

```diff
@@ -48,7 +48,19 @@
 wood_fuel,1864,wood_fuel,1864,wood_charcoal,1630,0
 wood_fuel,1864,wood_fuel,1864,wood_pellets_and_other_agglomerates,1696,0
 industrial_roundwood,1865,industrial_roundwood,1865,veneer_sheets,1634,0
 industrial_roundwood,1865,industrial_roundwood,1865,sawnwood,1872,0
 industrial_roundwood,1865,industrial_roundwood,1865,wood_based_panels,1873,0
 industrial_roundwood,1865,industrial_roundwood,1865,wood_pulp,1875,0
 industrial_roundwood,1865,wood_pulp,1875,paper_and_paperboard,1876,0
+maize_corn,56,maize_corn,56,flour_of_maize,58,0
+maize_corn,56,maize_corn,56,bran_of_maize,59,0
+maize_corn,56,maize_corn,56,germ_of_maize,57,0
+maize_corn,56,maize_corn,56,brewing_or_distilling_dregs_and_waste,654,0
+maize_corn,56,maize_corn,56,undenatured_ethyl_alcohol_of_an_alcoholic_strength_by_volume_of_less_than_80_vol_spirits_liqueurs_and_other_spirituous_beverages,634,0
+maize_corn,56,maize_corn,56,breakfast_cereals,41,0
+maize_corn,56,maize_corn,56,cereal_preparations,113,0
+maize_corn,56,bran_of_maize,59,gluten_feed_and_meal,846,0
+maize_corn,56,germ_of_maize,57,cake_of_maize,61,1
+maize_corn,56,germ_of_maize,57,oil_of_maize,60,1
+maize_corn,56,oil_of_maize,60,margarine_and_shortening,1242,0
+maize_corn,56,oil_of_maize,60,liquid_margarine,1241,0
```

### Comparing `biotrade-0.2.2/biotrade/config_data/faostat_country_groups.csv` & `biotrade-0.2.3/biotrade/config_data/faostat_country_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/faostat_forestry_production_groups.csv` & `biotrade-0.2.3/biotrade/config_data/faostat_forestry_production_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/faostat_forestry_production_short_names.csv` & `biotrade-0.2.3/biotrade/config_data/faostat_forestry_production_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/faostat_forestry_trade_groups.csv` & `biotrade-0.2.3/biotrade/config_data/faostat_forestry_trade_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/faostat_products_name_code_shortname.csv` & `biotrade-0.2.3/biotrade/config_data/faostat_products_name_code_shortname.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/regulation_front_end_groups.csv` & `biotrade-0.2.3/biotrade/config_data/regulation_front_end_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/regulation_products.csv` & `biotrade-0.2.3/biotrade/config_data/regulation_products.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/config_data/wood_product_aggregates.csv` & `biotrade-0.2.3/biotrade/config_data/wood_product_aggregates.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/eurostat/__init__.py` & `biotrade-0.2.3/biotrade/eurostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/eurostat/pump.py` & `biotrade-0.2.3/biotrade/eurostat/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/__init__.py` & `biotrade-0.2.3/biotrade/faostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/aggregate.py` & `biotrade-0.2.3/biotrade/faostat/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/convert.py` & `biotrade-0.2.3/biotrade/faostat/convert.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/country.py` & `biotrade-0.2.3/biotrade/faostat/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/country_groups.py` & `biotrade-0.2.3/biotrade/faostat/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/database.py` & `biotrade-0.2.3/biotrade/faostat/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,25 +42,34 @@
 
     More examples are available under the documentation of the `select` method below.
 
     Select data for Italy using an SQL Alchemy select statement. Return results
     using a pandas data frame:
 
         >>> import pandas
+        >>> from biotrade.faostat import faostat
         >>> db = faostat.db
         >>> reporter = db.forestry_production.columns.get("reporter")
         >>> statement = db.forestry_production.select().where(reporter == "Italy")
-        >>> fp_it = pandas.read_sql_query(statement, db.engine)
+        >>> with faostat.db.engine.connect() as conn:
+        >>>     fp_it = pandas.read_sql_query(statement, conn)
 
     Use a SQL select statement directly
 
-        >>> query = "SELECT * FROM forestry_production WHERE reporter = 'Italy'"
-        >>> fp_it = pandas.read_sql_query(query, db.engine)
-        >>> query = "SELECT * FROM forestry_trade WHERE reporter = 'Italy'"
-        >>> ft_it = pandas.read_sql_query(query, db.engine)
+        >>> from sqlalchemy import text
+        >>> # In case you are using an SQLite database
+        >>> schema = "main"
+        >>> # In case you are using a PostGreSQL database
+        >>> schema = "raw_faostat"
+        >>> query = text(f"SELECT * FROM {schema}.forestry_production WHERE reporter = 'Italy'")
+        >>> with faostat.db.engine.connect() as conn:
+        >>>     fp_it = pandas.read_sql_query(query, conn)
+        >>> query = text(f"SELECT * FROM {schema}.forestry_trade  WHERE reporter = 'Italy'")
+        >>> with faostat.db.engine.connect() as conn:
+        >>>     ft_it = pandas.read_sql_query(query, conn)
 
     Database update methods are in the faostat.pump object.
 
     """
 
     # To be overwritten by the children
     database_url = None
@@ -85,16 +94,18 @@
 
         # Create the schema if it doesn't exist.
         # Exclude the SQLite engine because there is only a default schemas for that engine.
         # And the SQLite dialect doesn't have a has_schema() method.
         if hasattr(self.engine.dialect, "has_schema") and callable(
             getattr(self.engine.dialect, "has_schema")
         ):
-            if not self.engine.dialect.has_schema(self.engine, self.schema):
-                self.engine.execute(CreateSchema(self.schema))
+            with self.engine.connect() as conn:
+                if not self.engine.dialect.has_schema(conn, self.schema):
+                    conn.execute(CreateSchema(self.schema))
+                    conn.commit()
 
         # Describe table metadata
         self.forestry_production = self.describe_production_table(
             name="forestry_production"
         )
         self.country = self.describe_country_table(name="country")
         self.crop_production = self.describe_production_table(name="crop_production")
@@ -289,15 +300,17 @@
             ),
             schema=self.schema,
         )
         return table
 
     def read_sql_query(self, stmt):
         """A wrapper around pandas.read_sql_query"""
-        return pandas.read_sql_query(stmt, self.engine)
+        with self.engine.connect() as conn:
+            df = pandas.read_sql_query(stmt, conn)
+        return df
 
     def select(
         self,
         table,
         reporter=None,
         partner=None,
         product=None,
@@ -441,15 +454,15 @@
         if product_code is not None:
             stmt = stmt.where(table.c.product_code.in_(product_code))
         if period_start is not None:
             stmt = stmt.where(table.c.period >= period_start)
         if period_end is not None:
             stmt = stmt.where(table.c.period <= period_end)
         # Query the database and return a data frame
-        df = pandas.read_sql_query(stmt, self.engine)
+        df = self.read_sql_query(stmt)
         return df
 
     def agg_reporter_partner_eu_row(
         self,
         table,
         product_code,
     ):
@@ -533,15 +546,15 @@
         # Select column subset of join selection to return for dataframe
         stmt = select(join_columns)
         # Delete from column list the column not used for the groupby
         del join_columns[-1]
         # Aggregate by columns the join selection
         stmt = stmt.group_by(*join_columns)
         # Return the dataframe from the query to db
-        df = pandas.read_sql_query(stmt, self.engine)
+        df = self.read_sql_query(stmt)
         return df
 
     def extract_product_names_codes(self, table_list):
         """
         Extract product names and product codes from tables of
         Faostat db. Duplicates are dropped out.
 
@@ -566,15 +579,15 @@
                 faostat_table.select()
                 .with_only_columns(
                     [faostat_table.c.product_code, faostat_table.c.product]
                 )
                 .distinct(faostat_table.c.product_code, faostat_table.c.product)
             )
             # Retrieve dataset
-            table_products = pandas.read_sql_query(stmt, self.engine)
+            table_products = self.read_sql_query(stmt)
             faostat_products = pandas.concat(
                 [faostat_products, table_products], ignore_index=True
             )
         # Drop duplicates
         faostat_products.drop_duplicates(
             subset="product_code", ignore_index=True, inplace=True
         )
```

### Comparing `biotrade-0.2.2/biotrade/faostat/mirror.py` & `biotrade-0.2.3/biotrade/faostat/mirror.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/products.py` & `biotrade-0.2.3/biotrade/faostat/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/pump.py` & `biotrade-0.2.3/biotrade/faostat/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/quality.py` & `biotrade-0.2.3/biotrade/faostat/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/faostat/share_coefficients.py` & `biotrade-0.2.3/biotrade/faostat/share_coefficients.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/hwp/country.py` & `biotrade-0.2.3/biotrade/hwp/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/tests/test_aggregate.py` & `biotrade-0.2.3/biotrade/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/tests/test_front_end.py` & `biotrade-0.2.3/biotrade/tests/test_front_end.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/tests/test_mirror.py` & `biotrade-0.2.3/biotrade/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/tests/test_reallocate.py` & `biotrade-0.2.3/biotrade/tests/test_reallocate.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,26 +62,26 @@
 def test_split_by_partners():
     df_prod = pandas.DataFrame(
         {
             "year": 1,
             "reporter": ["a", "b"],
             "reporter_code": [1, 2],
             "primary_product": ["p", "p"],
-            "primary_eq_imp": [6, 14],
+            "primary_eq_imp_0": [6, 14],
         }
     )
     df_trade = pandas.DataFrame(
         {
             "year": 1,
             "reporter": ["a", "a", "b", "b"],
             "reporter_code": [1, 1, 2, 2],
             "partner": ["x", "y", "x", "z"],
             "partner_code": [24, 25, 24, 26],
             "primary_product": ["p", "p", "p", "p"],
-            "value": [1, 2, 3, 4],
+            "import_quantity": [1, 2, 3, 4],
         }
     )
     output = split_by_partners(df_prod, df_trade, 1)
     expected = df_trade.copy()
     # Use float in the expected series
     expected["primary_eq_imp_1"] = [2, 4, 6, 8.0]
     assert_frame_equal(output[expected.columns], expected)
```

### Comparing `biotrade-0.2.2/biotrade/world_bank/__init__.py` & `biotrade-0.2.3/biotrade/world_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/world_bank/database.py` & `biotrade-0.2.3/biotrade/world_bank/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade/world_bank/pump.py` & `biotrade-0.2.3/biotrade/world_bank/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/biotrade.egg-info/PKG-INFO` & `biotrade-0.2.3/biotrade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.2.2
+Version: 0.2.3
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `biotrade-0.2.2/biotrade.egg-info/SOURCES.txt` & `biotrade-0.2.3/biotrade.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,9 +71,8 @@
 scripts/front_end/average_harvested_area_production.py
 scripts/front_end/average_trade_quantity.py
 scripts/front_end/db_scheduler.py
 scripts/front_end/functions.py
 scripts/front_end/product_list.py
 scripts/front_end/trends_harvested_area_production.py
 scripts/front_end/trends_trade_quantity.py
-scripts/front_end/update_db.py
 scripts/quality/faostat_compare_aggregates_to_constituents.py
```

### Comparing `biotrade-0.2.2/scripts/front_end/DEPRECATED_reporter_list.py` & `biotrade-0.2.3/scripts/front_end/DEPRECATED_reporter_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/scripts/front_end/annual_variation_harvested_area_production.py` & `biotrade-0.2.3/scripts/front_end/annual_variation_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/scripts/front_end/annual_variation_trade_quantity_value.py` & `biotrade-0.2.3/scripts/front_end/annual_variation_trade_quantity_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,49 +6,43 @@
 
 Script made to export data related to trade quantities of countries associated to the regulation and commodity tree products, for the web platform
 
 """
 
 
 def main():
-    import pandas as pd
     from scripts.front_end.functions import (
         main_product_list,
         comtrade_products,
         merge_faostat_comtrade_data,
-        consistency_check_china_data,
+        aggregated_data,
         reporter_iso_codes,
         replace_zero_with_nan_values,
         save_file,
     )
+    from biotrade.faostat import faostat
     from biotrade.faostat.aggregate import agg_trade_eu_row
 
     # Obtain faostat product codes
     faostat_list = main_product_list(["crop_trade"])
     # Obtain comtrade regulation codes
     comtrade_regulation = comtrade_products()
     # Trade data related to product code list
     trade_data = merge_faostat_comtrade_data(
         faostat_list, comtrade_regulation, aggregate=False
     )
-    # China Mainland + Taiwan data
-    df_china = consistency_check_china_data(trade_data)
-    # Add China data to trade_data (exclude Taiwan data)
-    trade_data = pd.concat(
-        [
-            trade_data[
-                ~(
-                    (trade_data[["reporter_code", "partner_code"]] == 214).any(
-                        axis=1
-                    )
-                )
-            ],
-            df_china,
-        ],
-        ignore_index=True,
+    # Aggregate french territories values to France and add them to the dataframe
+    code_list = [68, 69, 87, 135, 182, 270, 281]
+    agg_country_code = 68
+    agg_country_name = faostat.country_groups.df
+    agg_country_name = agg_country_name[
+        agg_country_name.faost_code == agg_country_code
+    ].fao_table_name.values[0]
+    trade_data = aggregated_data(
+        trade_data, code_list, agg_country_code, agg_country_name
     )
     # Substitute faostat codes with iso3 codes
     trade_data = reporter_iso_codes(trade_data)
     # Columns to be retained
     column_list = [
         "reporter_code",
         "partner_code",
@@ -107,17 +101,14 @@
     # Aggregate to EU and ROW for reporters
     eu_row_data = agg_trade_eu_row(
         trade_data,
         grouping_side="reporter",
         drop_index_col=[
             "year",
             "flag",
-            "faost_code",
-            "iso3_code",
-            "fao_status_info",
         ],
     )
     # Substitute with name and codes of the aggregations for the web platform
     selector = eu_row_data["reporter"] == "eu"
     eu_row_data.loc[selector, "reporter_code"] = "EU27"
     eu_row_data.loc[~selector, "reporter_code"] = "ROW"
     eu_row_data["reporter"].replace(
@@ -147,17 +138,14 @@
     # Aggregate to EU and ROW for partners
     eu_row_data = agg_trade_eu_row(
         trade_data,
         grouping_side="partner",
         drop_index_col=[
             "year",
             "flag",
-            "faost_code",
-            "iso3_code",
-            "fao_status_info",
         ],
     )
     # Substitute with name and codes of the aggregations for the web platform
     selector = eu_row_data["partner"] == "eu"
     eu_row_data.loc[selector, "partner_code"] = "EU27"
     eu_row_data.loc[~selector, "partner_code"] = "ROW"
     eu_row_data["partner"].replace(
```

### Comparing `biotrade-0.2.2/scripts/front_end/average_harvested_area_production.py` & `biotrade-0.2.3/scripts/front_end/average_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/scripts/front_end/average_trade_quantity.py` & `biotrade-0.2.3/scripts/front_end/average_trade_quantity.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,50 +10,45 @@
 
 
 def main():
     from scripts.front_end.functions import (
         main_product_list,
         comtrade_products,
         merge_faostat_comtrade_data,
-        consistency_check_china_data,
+        aggregated_data,
         reporter_iso_codes,
         average_results,
         replace_zero_with_nan_values,
         save_file,
     )
     from scripts.front_end.functions import (
         COLUMN_PERC_SUFFIX,
         COLUMN_AVG_SUFFIX,
     )
+    from biotrade.faostat import faostat
     from biotrade.faostat.aggregate import agg_trade_eu_row
     import pandas as pd
 
     # Obtain faostat product codes
     faostat_list = main_product_list(["crop_trade"])
     # Obtain comtrade regulation codes
     comtrade_regulation = comtrade_products()
     # Trade data related to product code list
     trade_data = merge_faostat_comtrade_data(
         faostat_list, comtrade_regulation, aggregate=False
     )
-    # China Mainland + Taiwan data
-    df_china = consistency_check_china_data(trade_data)
-    # Add China data to trade_data (exclude Taiwan data)
-    trade_data = pd.concat(
-        [
-            trade_data[
-                ~(
-                    (trade_data[["reporter_code", "partner_code"]] == 214).any(
-                        axis=1
-                    )
-                )
-            ],
-            df_china,
-        ],
-        ignore_index=True,
+    # Aggregate french territories values to France and add them to the dataframe
+    code_list = [68, 69, 87, 135, 182, 270, 281]
+    agg_country_code = 68
+    agg_country_name = faostat.country_groups.df
+    agg_country_name = agg_country_name[
+        agg_country_name.faost_code == agg_country_code
+    ].fao_table_name.values[0]
+    trade_data = aggregated_data(
+        trade_data, code_list, agg_country_code, agg_country_name
     )
     # Substitute faostat codes with iso3 codes
     trade_data = reporter_iso_codes(trade_data)
     # Define the columns and codes for the average calculations
     dict_list = [
         {
             "average_col": "product_code",
@@ -151,21 +146,21 @@
     ][column_list]
     save_file(df_comtrade_partner, "comtrade_average_mf.csv")
     # Consider averages for EU and rest of the world partners
     # Aggregate data with reporters as eu and row
     df_group_reporter = agg_trade_eu_row(
         trade_data,
         grouping_side="reporter",
-        drop_index_col=["flag", "faost_code", "iso3_code", "fao_status_info"],
+        drop_index_col=["flag"],
     )
     # Aggregate data with partners as eu and row
     df_group_partner = agg_trade_eu_row(
         trade_data,
         grouping_side="partner",
-        drop_index_col=["flag", "faost_code", "iso3_code", "fao_status_info"],
+        drop_index_col=["flag"],
     )
     # Concatenate in a unique df
     df_group = pd.concat(
         [df_group_reporter, df_group_partner],
         ignore_index=True,
     )
     # Substitute with name and codes of the aggregations for the web platform
```

### Comparing `biotrade-0.2.2/scripts/front_end/db_scheduler.py` & `biotrade-0.2.3/scripts/front_end/db_scheduler.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/scripts/front_end/functions.py` & `biotrade-0.2.3/scripts/front_end/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,21 +160,17 @@
             how="left",
             left_on=["partner_code"],
             right_on=["faost_code"],
         )
         df["partner_code"] = df["iso3_code"]
     df.drop(columns=["faost_code", "iso3_code"], inplace=True)
     # Consider only data of official country codes by GISCO
-    if os.environ.get("FRONT_END_SCRIPTS"):
-        path = Path(os.environ["FRONT_END_SCRIPTS"])
-    else:
-        path = Path(os.getenv("PYTHONPATH")) / "scripts" / "front_end"
     country_codes = (
         pd.read_csv(
-            path / "GISCO_CNTR_LIST.txt",
+            data_dir / "GISCO_CNTR_LIST.txt",
             sep=";",
         )
         .ISO3_CODE.drop_duplicates()
         .to_list()
     )
     df = df[df.reporter_code.isin(country_codes)].reset_index(drop=True)
     if "partner_code" in df.columns:
```

### Comparing `biotrade-0.2.2/scripts/front_end/product_list.py` & `biotrade-0.2.3/scripts/front_end/product_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/scripts/front_end/trends_harvested_area_production.py` & `biotrade-0.2.3/scripts/front_end/trends_harvested_area_production.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def main():
     import sys
     from biotrade.faostat import faostat
     import pandas as pd
     import numpy as np
     from scripts.front_end.functions import (
-        consistency_check_china_data,
+        aggregated_data,
         main_product_list,
         reporter_iso_codes,
         replace_zero_with_nan_values,
         trend_analysis,
         save_file,
     )
 
@@ -44,20 +44,23 @@
         table="forestry_production",
         product_code=main_product_list,
         element=["production"],
     )
     # Merge data
     crop_data = pd.concat([crop_data, wood_data], ignore_index=True)
     crop_data = crop_data[crop_data["reporter_code"] < 1000]
-    # China Mainland + Taiwan data
-    df_china = consistency_check_china_data(crop_data)
-    # Add China data to crop_data (exclude Taiwan data)
-    crop_data = pd.concat(
-        [crop_data[~(crop_data["reporter_code"] == 214)], df_china],
-        ignore_index=True,
+    # Aggregate french territories values to France and add them to the dataframe
+    code_list = [68, 69, 87, 135, 182, 270, 281]
+    agg_country_code = 68
+    agg_country_name = faostat.country_groups.df
+    agg_country_name = agg_country_name[
+        agg_country_name.faost_code == agg_country_code
+    ].fao_table_name.values[0]
+    crop_data = aggregated_data(
+        crop_data, code_list, agg_country_code, agg_country_name
     )
     # Substitute faostat codes with iso3 codes
     crop_data = reporter_iso_codes(crop_data)
     # Consider data after 1985 to calculate trends of last year
     crop_data = crop_data[crop_data["year"] > 1985]
     # Perform trend analysis
     df = trend_analysis(crop_data, multi_process=multi_process)
```

### Comparing `biotrade-0.2.2/scripts/front_end/trends_trade_quantity.py` & `biotrade-0.2.3/scripts/front_end/trends_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/scripts/quality/faostat_compare_aggregates_to_constituents.py` & `biotrade-0.2.3/scripts/quality/faostat_compare_aggregates_to_constituents.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.2.2/setup.py` & `biotrade-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 readme_path = path.join(this_dir, "README.md")
 with open(readme_path, encoding="utf-8") as handle:
     readme = handle.read()
 
 # Call setup #
 setup(
     name="biotrade",
-    version="0.2.2",
+    version="0.2.3",
     description="Agriculture and forestry statistics.",
     license="MIT",
     url="https://gitlab.com/bioeconomy/forobs/biotrade/",
     author="Paul Rougieux, Selene Patani",
     author_email="paul.rougieux@gmail.com",
     packages=find_namespace_packages(exclude=["notebooks", "scripts"]),
     install_requires=[
```

