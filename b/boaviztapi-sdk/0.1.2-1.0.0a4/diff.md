# Comparing `tmp/boaviztapi-sdk-0.1.2.tar.gz` & `tmp/boaviztapi-sdk-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boaviztapi-sdk-0.1.2.tar", last modified: Sat Jun 18 10:22:42 2022, max compression
+gzip compressed data, was "boaviztapi-sdk-1.0.0a4.tar", last modified: Tue Jul  4 10:31:31 2023, max compression
```

## Comparing `boaviztapi-sdk-0.1.2.tar` & `boaviztapi-sdk-1.0.0a4.tar`

### file list

```diff
@@ -1,61 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 10:22:42.309848 boaviztapi-sdk-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-06-18 10:22:42.309848 boaviztapi-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7532 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 10:22:42.305848 boaviztapi-sdk-0.1.2/boaviztapi_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 10:22:42.309848 boaviztapi-sdk-0.1.2/boaviztapi_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13434 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/api/cloud_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    42634 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/api/component_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    19524 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    40067 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 10:22:42.309848 boaviztapi-sdk-0.1.2/boaviztapi_sdk/apis/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17088 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     5970 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 10:22:42.309848 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12480 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/case.py
--rw-r--r--   0 runner    (1001) docker     (121)    13309 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/configuration_server.py
--rw-r--r--   0 runner    (1001) docker     (121)    13961 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/cpu.py
--rw-r--r--   0 runner    (1001) docker     (121)    13491 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/disk.py
--rw-r--r--   0 runner    (1001) docker     (121)    12554 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    12121 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/location_inner.py
--rw-r--r--   0 runner    (1001) docker     (121)    13070 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/model_server.py
--rw-r--r--   0 runner    (1001) docker     (121)    12298 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/mother_board.py
--rw-r--r--   0 runner    (1001) docker     (121)    12517 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/power_supply.py
--rw-r--r--   0 runner    (1001) docker     (121)    13717 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/ram.py
--rw-r--r--   0 runner    (1001) docker     (121)    13611 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/server_dto.py
--rw-r--r--   0 runner    (1001) docker     (121)    15186 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/usage_cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)    14930 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/usage_server.py
--rw-r--r--   0 runner    (1001) docker     (121)    12918 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    83480 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 10:22:42.309848 boaviztapi-sdk-0.1.2/boaviztapi_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15174 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 10:22:42.305848 boaviztapi-sdk-0.1.2/boaviztapi_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-06-18 10:22:42.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-06-18 10:22:42.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-18 10:22:42.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-18 10:22:42.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-18 10:22:42.000000 boaviztapi-sdk-0.1.2/boaviztapi_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-18 10:22:42.309848 boaviztapi-sdk-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-06-18 10:22:42.000000 boaviztapi-sdk-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 10:22:42.309848 boaviztapi-sdk-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_cloud_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_component_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_configuration_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_location_inner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_model_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_mother_board.py
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_power_supply.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_ram.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_server_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_server_dto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_usage_cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_usage_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-06-18 10:22:41.000000 boaviztapi-sdk-0.1.2/test/test_validation_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:31:31.967642 boaviztapi-sdk-1.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-04 10:31:31.967642 boaviztapi-sdk-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26140 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:31:31.943642 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:31:31.947642 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40464 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/cloud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   215790 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/component_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/consumption_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123340 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/peripheral_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31938 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178243 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/terminal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56707 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api/utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32675 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:31:31.955642 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-04 10:31:28.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/configuration_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/consumption_profile_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-04 10:31:28.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/desktop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/elec_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/external_hdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/external_ssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/laptop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/location_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/motherboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/power_supply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/smartphone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/tablet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/television.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/time_workload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/usage1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/usage_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/usage_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/usb_stick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/workload_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/models/workload_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:31:31.943642 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-04 10:31:31.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-04 10:31:31.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:31:31.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-04 10:31:31.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 10:31:31.000000 boaviztapi-sdk-1.0.0a4/boaviztapi_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 10:31:31.967642 boaviztapi-sdk-1.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-04 10:31:30.000000 boaviztapi-sdk-1.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:31:31.967642 boaviztapi-sdk-1.0.0a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-04 10:31:28.000000 boaviztapi-sdk-1.0.0a4/test/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_cloud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_component_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_configuration_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_consumption_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_consumption_profile_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-04 10:31:28.000000 boaviztapi-sdk-1.0.0a4/test/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_desktop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_elec_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_external_hdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_external_ssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_laptop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_location_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_motherboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_peripheral_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_power_supply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_smartphone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_tablet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_television.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_terminal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_time_workload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_usage1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_usage_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_usage_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_usb_stick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_workload_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-04 10:31:29.000000 boaviztapi-sdk-1.0.0a4/test/test_workload_time.py
```

### Comparing `boaviztapi-sdk-0.1.2/boaviztapi_sdk/api_client.py` & `boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/api_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,87 @@
+# coding: utf-8
+
 """
     BOAVIZTAPI - DEMO
 
-    # 🎯 Retrieving the impacts of digital elements This is a quick demo, to see full documentation [click here](https://doc.api.boavizta.org)  ## ➡️Server router  ### Server routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |     X    | |   ADP  |        X       |     X    | |   PE   |        X       |     X    | ## ➡️Cloud router  ### Cloud routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |     X    | |   ADP  |        X       |     X    | |   PE   |        X       |     X    | ## ➡️Component router  ### Component routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |          | |   ADP  |        X       |          | |   PE   |        X       |          |   # noqa: E501
+    <p>🎯 Retrieving the impacts of digital elements.</p> <p>This is a quick demo, to see full documentation <a href=\"https://doc.api.boavizta.org\">click here</a></p> <h2>Features</h2> <p>Bellow a list of all available features.</p> <h3>👄 Verbose</h3> <p>Verbose is an HTTP parameter. If set at true :</p> <ul> <li>Shows the impacts of each component</li> <li>Shows the value used for each attribute</li> </ul> <p><em>\"attribute\": {\"value\": \"value\", \"unit\": \"unit\", \"status\": \"Status\", \"source\": \"Source\", \"min\":\"min\", \"max\":\"max\", \"significant_figures\":\"significant_figures\"}</em></p> <h3>🔨 Embedded</h3> <ul> <li>Embedded impacts are the impacts occurring during raw material extraction, manufacture, distribution and end of life</li> <li>When end of life is not taken into account, we specified it in the <code>warnings</code></li> </ul> <h3>🔌  Usage</h3> <p>Usage impacts are assessed by multiplying :</p> <ul> <li> <p>a <strong>duration</strong></p> </li> <li> <p>an <strong>impact factor</strong> </p> </li> <li> <p>an <strong>electrical consumption</strong> </p> </li> </ul> <h4>⏲ Duration</h4> <p>Usage impacts can be given as a router parameter, in hours.</p> <p>If no duration is given, <strong>the impact is assess for the all life duration of the asset</strong>.</p> <h4>✖️ Impact factors</h4> <ul> <li>Impact factors can be given : <em>\"usage\":{\"elec_factors\":{[criterion]_factors: 0.38}}</em></li> <li> <p>Impact factors can be retrieved from : <em>\"usage\":{\"usage_location\": \"FRA\"}</em>. </p> </li> <li> <p>See the list of locations : <a href=\"/v1/utils/country_code\">/v1/utils/country_code</a>*</p> </li> </ul> <h4>⚡ Electrical consumption</h4> <h5>⏺️ Given</h5> <ul> <li>Electrical consumption can be given for one hour (average) <em>\"usage\":{\"avg_power\": 1}</em>.</li> </ul> <h5>📈 Modeled</h5> <ul> <li>Electrical consumption can be retrieved from consumption profile using <em>usage:{time_workload: 50}</em>.</li> </ul> <h5>📋 Archetype</h5> <ul> <li>In some cases, default electrical consumption can be taken from the archetype</li> </ul> <h3>🔃 Auto-complete &amp; 📋 Archetype</h3> <p>The API will complete the missing attributes in a request with a completion function or with values taken from the <code>archetype</code> specified in the route parameter.</p> <h3>⏬ Allocation</h3> <ul> <li>Usage impacts are assessed on the duration given in route parameter</li> <li>Embedded impacts are allocated linearly on the duration given in parameter <code>embedded_impact = impact * (duration/life_duration)</code></li> </ul> <p>If no duration is given, the life_duration (<code>`hours_life_time</code>) of the asset is used.</p>  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0a4
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-    The version of the OpenAPI document: 0.1.2
-    Generated by: https://openapi-generator.tech
+    Do not edit the class manually.
 """
 
 
-import json
 import atexit
+import datetime
+from dateutil.parser import parse
+import json
 import mimetypes
 from multiprocessing.pool import ThreadPool
-import io
 import os
 import re
-import typing
-from urllib.parse import quote
-from urllib3.fields import RequestField
+import tempfile
 
+from urllib.parse import quote
 
-from boaviztapi_sdk import rest
 from boaviztapi_sdk.configuration import Configuration
-from boaviztapi_sdk.exceptions import ApiTypeError, ApiValueError, ApiException
-from boaviztapi_sdk.model_utils import (
-    ModelNormal,
-    ModelSimple,
-    ModelComposed,
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    deserialize_file,
-    file_type,
-    model_to_dict,
-    none_type,
-    validate_and_convert_types
-)
+from boaviztapi_sdk.api_response import ApiResponse
+import boaviztapi_sdk.models
+from boaviztapi_sdk import rest
+from boaviztapi_sdk.exceptions import ApiValueError, ApiException
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
     the methods and models for each application are generated from the OpenAPI
     templates.
 
-    NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
-
     :param configuration: .Configuration object for this client
     :param header_name: a header to pass when making calls to the API.
     :param header_value: a header value to pass when making calls to
         the API.
     :param cookie: a cookie to include in the header when making calls
         to the API
     :param pool_threads: The number of threads to use for async requests
         to the API. More threads means more concurrent API requests.
     """
 
+    PRIMITIVE_TYPES = (float, bool, bytes, str, int)
+    NATIVE_TYPES_MAPPING = {
+        'int': int,
+        'long': int, # TODO remove as only py3 is supported?
+        'float': float,
+        'str': str,
+        'bool': bool,
+        'date': datetime.date,
+        'datetime': datetime.datetime,
+        'object': object,
+    }
     _pool = None
 
     def __init__(self, configuration=None, header_name=None, header_value=None,
                  cookie=None, pool_threads=1):
+        # use default configuration if none is provided
         if configuration is None:
-            configuration = Configuration.get_default_copy()
+            configuration = Configuration.get_default()
         self.configuration = configuration
         self.pool_threads = pool_threads
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -110,35 +111,48 @@
     @user_agent.setter
     def user_agent(self, value):
         self.default_headers['User-Agent'] = value
 
     def set_default_header(self, header_name, header_value):
         self.default_headers[header_name] = header_value
 
+
+    _default = None
+
+    @classmethod
+    def get_default(cls):
+        """Return new instance of ApiClient.
+
+        This method returns newly created, based on default constructor,
+        object of ApiClient class or returns a copy of default
+        ApiClient.
+
+        :return: The ApiClient object.
+        """
+        if cls._default is None:
+            cls._default = ApiClient()
+        return cls._default
+
+    @classmethod
+    def set_default(cls, default):
+        """Set default instance of ApiClient.
+
+        It stores default ApiClient.
+
+        :param default: object of ApiClient.
+        """
+        cls._default = default
+
     def __call_api(
-        self,
-        resource_path: str,
-        method: str,
-        path_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        query_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
-        header_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        body: typing.Optional[typing.Any] = None,
-        post_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
-        files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None,
-        response_type: typing.Optional[typing.Tuple[typing.Any]] = None,
-        auth_settings: typing.Optional[typing.List[str]] = None,
-        _return_http_data_only: typing.Optional[bool] = None,
-        collection_formats: typing.Optional[typing.Dict[str, str]] = None,
-        _preload_content: bool = True,
-        _request_timeout: typing.Optional[typing.Union[int, float, typing.Tuple]] = None,
-        _host: typing.Optional[str] = None,
-        _check_type: typing.Optional[bool] = None,
-        _content_type: typing.Optional[str] = None,
-        _request_auths: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
-    ):
+            self, resource_path, method, path_params=None,
+            query_params=None, header_params=None, body=None, post_params=None,
+            files=None, response_types_map=None, auth_settings=None,
+            _return_http_data_only=None, collection_formats=None,
+            _preload_content=True, _request_timeout=None, _host=None,
+            _request_auth=None):
 
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
@@ -156,343 +170,312 @@
             for k, v in path_params:
                 # specified safe chars, encode everything
                 resource_path = resource_path.replace(
                     '{%s}' % k,
                     quote(str(v), safe=config.safe_chars_for_path_param)
                 )
 
-        # query parameters
-        if query_params:
-            query_params = self.sanitize_for_serialization(query_params)
-            query_params = self.parameters_to_tuples(query_params,
-                                                     collection_formats)
-
         # post parameters
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(post_params,
                                                     collection_formats)
             post_params.extend(self.files_parameters(files))
-            if header_params['Content-Type'].startswith("multipart"):
-                post_params = self.parameters_to_multipart(post_params,
-                                                           (dict))
+
+        # auth setting
+        self.update_params_for_auth(
+            header_params, query_params, auth_settings,
+            resource_path, method, body,
+            request_auth=_request_auth)
 
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
-        # auth setting
-        self.update_params_for_auth(header_params, query_params,
-                                    auth_settings, resource_path, method, body,
-                                    request_auths=_request_auths)
-
         # request url
         if _host is None:
             url = self.configuration.host + resource_path
         else:
             # use server/host defined in path or operation instead
             url = _host + resource_path
 
+        # query parameters
+        if query_params:
+            query_params = self.sanitize_for_serialization(query_params)
+            url_query = self.parameters_to_url_query(query_params,
+                                                     collection_formats)
+            url += "?" + url_query
+
         try:
             # perform request and return response
             response_data = self.request(
-                method, url, query_params=query_params, headers=header_params,
+                method, url,
+                query_params=query_params,
+                headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout)
         except ApiException as e:
-            e.body = e.body.decode('utf-8')
+            if e.body:
+                e.body = e.body.decode('utf-8')
             raise e
 
         self.last_response = response_data
 
-        return_data = response_data
-
-        if not _preload_content:
-            return (return_data)
-            return return_data
-
-        # deserialize response data
-        if response_type:
-            if response_type != (file_type,):
-                encoding = "utf-8"
-                content_type = response_data.getheader('content-type')
-                if content_type is not None:
-                    match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
-                    if match:
-                        encoding = match.group(1)
-                response_data.data = response_data.data.decode(encoding)
-
-            return_data = self.deserialize(
-                response_data,
-                response_type,
-                _check_type
-            )
-        else:
-            return_data = None
+        return_data = None # assuming derialization is not needed
+        # data needs deserialization or returns HTTP data (deserialized) only
+        if _preload_content or _return_http_data_only:
+          response_type = response_types_map.get(str(response_data.status), None)
+
+          if response_type == "bytearray":
+              response_data.data = response_data.data
+          else:
+              match = None
+              content_type = response_data.getheader('content-type')
+              if content_type is not None:
+                  match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
+              encoding = match.group(1) if match else "utf-8"
+              response_data.data = response_data.data.decode(encoding)
+
+          # deserialize response data
+          if response_type == "bytearray":
+              return_data = response_data.data
+          elif response_type:
+              return_data = self.deserialize(response_data, response_type)
+          else:
+              return_data = None
 
         if _return_http_data_only:
-            return (return_data)
+            return return_data
         else:
-            return (return_data, response_data.status,
-                    response_data.getheaders())
+            return ApiResponse(status_code = response_data.status,
+                           data = return_data,
+                           headers = response_data.getheaders(),
+                           raw_data = response_data.data)
 
-    def parameters_to_multipart(self, params, collection_types):
-        """Get parameters as list of tuples, formatting as json if value is collection_types
+    def sanitize_for_serialization(self, obj):
+        """Builds a JSON POST object.
 
-        :param params: Parameters as list of two-tuples
-        :param dict collection_types: Parameter collection types
-        :return: Parameters as list of tuple or urllib3.fields.RequestField
-        """
-        new_params = []
-        if collection_types is None:
-            collection_types = (dict)
-        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
-            if isinstance(
-                     v, collection_types): # v is instance of collection_type, formatting as application/json
-                v = json.dumps(v, ensure_ascii=False).encode("utf-8")
-                field = RequestField(k, v)
-                field.make_multipart(content_type="application/json; charset=utf-8")
-                new_params.append(field)
-            else:
-                new_params.append((k, v))
-        return new_params
-
-    @classmethod
-    def sanitize_for_serialization(cls, obj):
-        """Prepares data for transmission before it is sent with the rest client
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
-        If obj is io.IOBase, return the bytes
+
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
-        if isinstance(obj, (ModelNormal, ModelComposed)):
-            return {
-                key: cls.sanitize_for_serialization(val) for key,
-                val in model_to_dict(
-                    obj,
-                    serialize=True).items()}
-        elif isinstance(obj, io.IOBase):
-            return cls.get_file_data_and_close_file(obj)
-        elif isinstance(obj, (str, int, float, none_type, bool)):
+        if obj is None:
+            return None
+        elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
-        elif isinstance(obj, (datetime, date)):
+        elif isinstance(obj, list):
+            return [self.sanitize_for_serialization(sub_obj)
+                    for sub_obj in obj]
+        elif isinstance(obj, tuple):
+            return tuple(self.sanitize_for_serialization(sub_obj)
+                         for sub_obj in obj)
+        elif isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
-        elif isinstance(obj, ModelSimple):
-            return cls.sanitize_for_serialization(obj.value)
-        elif isinstance(obj, (list, tuple)):
-            return [cls.sanitize_for_serialization(item) for item in obj]
+
         if isinstance(obj, dict):
-            return {key: cls.sanitize_for_serialization(val) for key, val in obj.items()}
-        raise ApiValueError(
-            'Unable to prepare type {} for serialization'.format(
-                obj.__class__.__name__))
+            obj_dict = obj
+        else:
+            # Convert model obj to dict except
+            # attributes `openapi_types`, `attribute_map`
+            # and attributes which value is not None.
+            # Convert attribute name to json key in
+            # model definition for request.
+            obj_dict = obj.to_dict()
 
-    def deserialize(self, response, response_type, _check_type):
+        return {key: self.sanitize_for_serialization(val)
+                for key, val in obj_dict.items()}
+
+    def deserialize(self, response, response_type):
         """Deserializes response into an object.
 
         :param response: RESTResponse object to be deserialized.
-        :param response_type: For the response, a tuple containing:
-            valid classes
-            a list containing valid classes (for list schemas)
-            a dict containing a tuple of valid classes as the value
-            Example values:
-            (str,)
-            (Pet,)
-            (float, none_type)
-            ([int, none_type],)
-            ({str: (bool, str, int, float, date, datetime, str, none_type)},)
-        :param _check_type: boolean, whether to check the types of the data
-            received from the server
-        :type _check_type: bool
+        :param response_type: class literal for
+            deserialized object, or string of class name.
 
         :return: deserialized object.
         """
         # handle file downloading
         # save response body into a tmp file and return the instance
-        if response_type == (file_type,):
-            content_disposition = response.getheader("Content-Disposition")
-            return deserialize_file(response.data, self.configuration,
-                                    content_disposition=content_disposition)
+        if response_type == "file":
+            return self.__deserialize_file(response)
 
         # fetch data from response object
         try:
-            received_data = json.loads(response.data)
+            data = json.loads(response.data)
         except ValueError:
-            received_data = response.data
+            data = response.data
+
+        return self.__deserialize(data, response_type)
+
+    def __deserialize(self, data, klass):
+        """Deserializes dict, list, str into an object.
+
+        :param data: dict, list or str.
+        :param klass: class literal, or string of class name.
+
+        :return: object.
+        """
+        if data is None:
+            return None
+
+        if type(klass) == str:
+            if klass.startswith('List['):
+                sub_kls = re.match(r'List\[(.*)]', klass).group(1)
+                return [self.__deserialize(sub_data, sub_kls)
+                        for sub_data in data]
+
+            if klass.startswith('Dict['):
+                sub_kls = re.match(r'Dict\[([^,]*), (.*)]', klass).group(2)
+                return {k: self.__deserialize(v, sub_kls)
+                        for k, v in data.items()}
+
+            # convert str to class
+            if klass in self.NATIVE_TYPES_MAPPING:
+                klass = self.NATIVE_TYPES_MAPPING[klass]
+            else:
+                klass = getattr(boaviztapi_sdk.models, klass)
 
-        # store our data under the key of 'received_data' so users have some
-        # context if they are deserializing a string and the data type is wrong
-        deserialized_data = validate_and_convert_types(
-            received_data,
-            response_type,
-            ['received_data'],
-            True,
-            _check_type,
-            configuration=self.configuration
-        )
-        return deserialized_data
-
-    def call_api(
-        self,
-        resource_path: str,
-        method: str,
-        path_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        query_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
-        header_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        body: typing.Optional[typing.Any] = None,
-        post_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
-        files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None,
-        response_type: typing.Optional[typing.Tuple[typing.Any]] = None,
-        auth_settings: typing.Optional[typing.List[str]] = None,
-        async_req: typing.Optional[bool] = None,
-        _return_http_data_only: typing.Optional[bool] = None,
-        collection_formats: typing.Optional[typing.Dict[str, str]] = None,
-        _preload_content: bool = True,
-        _request_timeout: typing.Optional[typing.Union[int, float, typing.Tuple]] = None,
-        _host: typing.Optional[str] = None,
-        _check_type: typing.Optional[bool] = None,
-        _request_auths: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
-    ):
+        if klass in self.PRIMITIVE_TYPES:
+            return self.__deserialize_primitive(data, klass)
+        elif klass == object:
+            return self.__deserialize_object(data)
+        elif klass == datetime.date:
+            return self.__deserialize_date(data)
+        elif klass == datetime.datetime:
+            return self.__deserialize_datetime(data)
+        else:
+            return self.__deserialize_model(data, klass)
+
+    def call_api(self, resource_path, method,
+                 path_params=None, query_params=None, header_params=None,
+                 body=None, post_params=None, files=None,
+                 response_types_map=None, auth_settings=None,
+                 async_req=None, _return_http_data_only=None,
+                 collection_formats=None, _preload_content=True,
+                 _request_timeout=None, _host=None, _request_auth=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
         :param query_params: Query parameters in the url.
         :param header_params: Header parameters to be
             placed in the request header.
         :param body: Request body.
         :param post_params dict: Request post form parameters,
             for `application/x-www-form-urlencoded`, `multipart/form-data`.
         :param auth_settings list: Auth Settings names for the request.
-        :param response_type: For the response, a tuple containing:
-            valid classes
-            a list containing valid classes (for list schemas)
-            a dict containing a tuple of valid classes as the value
-            Example values:
-            (str,)
-            (Pet,)
-            (float, none_type)
-            ([int, none_type],)
-            ({str: (bool, str, int, float, date, datetime, str, none_type)},)
-        :param files: key -> field name, value -> a list of open file
-            objects for `multipart/form-data`.
-        :type files: dict
+        :param response: Response data type.
+        :param files dict: key -> filename, value -> filepath,
+            for `multipart/form-data`.
         :param async_req bool: execute request asynchronously
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :param collection_formats: dict of collection formats for path, query,
             header, and post parameters.
-        :type collection_formats: dict, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _check_type: boolean describing if the data back from the server
-            should have its type checked.
-        :type _check_type: bool, optional
-        :param _request_auths: set to override the auth_settings for an a single
+        :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
-        :type _request_auths: list, optional
+        :type _request_token: dict, optional
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
         """
         if not async_req:
             return self.__call_api(resource_path, method,
                                    path_params, query_params, header_params,
                                    body, post_params, files,
-                                   response_type, auth_settings,
+                                   response_types_map, auth_settings,
                                    _return_http_data_only, collection_formats,
                                    _preload_content, _request_timeout, _host,
-                                   _check_type, _request_auths=_request_auths)
+                                   _request_auth)
 
         return self.pool.apply_async(self.__call_api, (resource_path,
                                                        method, path_params,
                                                        query_params,
                                                        header_params, body,
                                                        post_params, files,
-                                                       response_type,
+                                                       response_types_map,
                                                        auth_settings,
                                                        _return_http_data_only,
                                                        collection_formats,
                                                        _preload_content,
                                                        _request_timeout,
-                                                       _host, _check_type, None, _request_auths))
+                                                       _host, _request_auth))
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
                 _request_timeout=None):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
-            return self.rest_client.GET(url,
+            return self.rest_client.get_request(url,
                                         query_params=query_params,
                                         _preload_content=_preload_content,
                                         _request_timeout=_request_timeout,
                                         headers=headers)
         elif method == "HEAD":
-            return self.rest_client.HEAD(url,
+            return self.rest_client.head_request(url,
                                          query_params=query_params,
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
                                          headers=headers)
         elif method == "OPTIONS":
-            return self.rest_client.OPTIONS(url,
+            return self.rest_client.options_request(url,
                                             query_params=query_params,
                                             headers=headers,
-                                            post_params=post_params,
                                             _preload_content=_preload_content,
-                                            _request_timeout=_request_timeout,
-                                            body=body)
+                                            _request_timeout=_request_timeout)
         elif method == "POST":
-            return self.rest_client.POST(url,
+            return self.rest_client.post_request(url,
                                          query_params=query_params,
                                          headers=headers,
                                          post_params=post_params,
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
                                          body=body)
         elif method == "PUT":
-            return self.rest_client.PUT(url,
+            return self.rest_client.put_request(url,
                                         query_params=query_params,
                                         headers=headers,
                                         post_params=post_params,
                                         _preload_content=_preload_content,
                                         _request_timeout=_request_timeout,
                                         body=body)
         elif method == "PATCH":
-            return self.rest_client.PATCH(url,
+            return self.rest_client.patch_request(url,
                                           query_params=query_params,
                                           headers=headers,
                                           post_params=post_params,
                                           _preload_content=_preload_content,
                                           _request_timeout=_request_timeout,
                                           body=body)
         elif method == "DELETE":
-            return self.rest_client.DELETE(url,
+            return self.rest_client.delete_request(url,
                                            query_params=query_params,
                                            headers=headers,
                                            _preload_content=_preload_content,
                                            _request_timeout=_request_timeout,
                                            body=body)
         else:
             raise ApiValueError(
@@ -526,371 +509,247 @@
                         delimiter = ','
                     new_params.append(
                         (k, delimiter.join(str(value) for value in v)))
             else:
                 new_params.append((k, v))
         return new_params
 
-    @staticmethod
-    def get_file_data_and_close_file(file_instance: io.IOBase) -> bytes:
-        file_data = file_instance.read()
-        file_instance.close()
-        return file_data
-
-    def files_parameters(self,
-                         files: typing.Optional[typing.Dict[str,
-                                                            typing.List[io.IOBase]]] = None):
-        """Builds form parameters.
+    def parameters_to_url_query(self, params, collection_formats):
+        """Get parameters as list of tuples, formatting collections.
 
-        :param files: None or a dict with key=param_name and
-            value is a list of open file objects
-        :return: List of tuples of form parameters with file data
+        :param params: Parameters as dict or list of two-tuples
+        :param dict collection_formats: Parameter collection formats
+        :return: URL query string (e.g. a=Hello%20World&b=123)
         """
-        if files is None:
-            return []
+        new_params = []
+        if collection_formats is None:
+            collection_formats = {}
+        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
+            if isinstance(v, (int, float)):
+                v = str(v)
+            if isinstance(v, bool):
+                v = str(v).lower()
+            if isinstance(v, dict):
+                v = json.dumps(v)
 
+            if k in collection_formats:
+                collection_format = collection_formats[k]
+                if collection_format == 'multi':
+                    new_params.extend((k, value) for value in v)
+                else:
+                    if collection_format == 'ssv':
+                        delimiter = ' '
+                    elif collection_format == 'tsv':
+                        delimiter = '\t'
+                    elif collection_format == 'pipes':
+                        delimiter = '|'
+                    else:  # csv is the default
+                        delimiter = ','
+                    new_params.append(
+                        (k, delimiter.join(quote(str(value)) for value in v)))
+            else:
+                new_params.append((k, quote(str(v))))
+
+        return "&".join(["=".join(item) for item in new_params])
+
+    def files_parameters(self, files=None):
+        """Builds form parameters.
+
+        :param files: File parameters.
+        :return: Form parameters with files.
+        """
         params = []
-        for param_name, file_instances in files.items():
-            if file_instances is None:
-                # if the file field is nullable, skip None values
-                continue
-            for file_instance in file_instances:
-                if file_instance is None:
-                    # if the file field is nullable, skip None values
+
+        if files:
+            for k, v in files.items():
+                if not v:
                     continue
-                if file_instance.closed is True:
-                    raise ApiValueError(
-                        "Cannot read a closed file. The passed in file_type "
-                        "for %s must be open." % param_name
-                    )
-                filename = os.path.basename(file_instance.name)
-                filedata = self.get_file_data_and_close_file(file_instance)
-                mimetype = (mimetypes.guess_type(filename)[0] or
-                            'application/octet-stream')
-                params.append(
-                    tuple([param_name, tuple([filename, filedata, mimetype])]))
+                file_names = v if type(v) is list else [v]
+                for n in file_names:
+                    with open(n, 'rb') as f:
+                        filename = os.path.basename(f.name)
+                        filedata = f.read()
+                        mimetype = (mimetypes.guess_type(filename)[0] or
+                                    'application/octet-stream')
+                        params.append(
+                            tuple([k, tuple([filename, filedata, mimetype])]))
 
         return params
 
     def select_header_accept(self, accepts):
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
         """
         if not accepts:
             return
 
-        accepts = [x.lower() for x in accepts]
+        for accept in accepts:
+            if re.search('json', accept, re.IGNORECASE):
+                return accept
 
-        if 'application/json' in accepts:
-            return 'application/json'
-        else:
-            return ', '.join(accepts)
+        return accepts[0]
 
-    def select_header_content_type(self, content_types, method=None, body=None):
+    def select_header_content_type(self, content_types):
         """Returns `Content-Type` based on an array of content_types provided.
 
         :param content_types: List of content-types.
-        :param method: http method (e.g. POST, PATCH).
-        :param body: http body to send.
         :return: Content-Type (e.g. application/json).
         """
         if not content_types:
             return None
 
-        content_types = [x.lower() for x in content_types]
-
-        if (method == 'PATCH' and
-                'application/json-patch+json' in content_types and
-                isinstance(body, list)):
-            return 'application/json-patch+json'
+        for content_type in content_types:
+            if re.search('json', content_type, re.IGNORECASE):
+                return content_type
 
-        if 'application/json' in content_types or '*/*' in content_types:
-            return 'application/json'
-        else:
-            return content_types[0]
+        return content_types[0]
 
     def update_params_for_auth(self, headers, queries, auth_settings,
-                               resource_path, method, body, request_auths=None):
+                               resource_path, method, body,
+                               request_auth=None):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
         :param queries: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
-        :param resource_path: A string representation of the HTTP request resource path.
-        :param method: A string representation of the HTTP request method.
-        :param body: A object representing the body of the HTTP request.
-            The object type is the return value of _encoder.default().
-        :param request_auths: if set, the provided settings will
-            override the token in the configuration.
+        :resource_path: A string representation of the HTTP request resource path.
+        :method: A string representation of the HTTP request method.
+        :body: A object representing the body of the HTTP request.
+        The object type is the return value of sanitize_for_serialization().
+        :param request_auth: if set, the provided settings will
+                             override the token in the configuration.
         """
         if not auth_settings:
             return
 
-        if request_auths:
-            for auth_setting in request_auths:
-                self._apply_auth_params(
-                    headers, queries, resource_path, method, body, auth_setting)
+        if request_auth:
+            self._apply_auth_params(headers, queries,
+                                    resource_path, method, body,
+                                    request_auth)
             return
 
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if auth_setting:
-                self._apply_auth_params(
-                    headers, queries, resource_path, method, body, auth_setting)
+                self._apply_auth_params(headers, queries,
+                                        resource_path, method, body,
+                                        auth_setting)
+
+    def _apply_auth_params(self, headers, queries,
+                           resource_path, method, body,
+                           auth_setting):
+        """Updates the request parameters based on a single auth_setting
 
-    def _apply_auth_params(self, headers, queries, resource_path, method, body, auth_setting):
+        :param headers: Header parameters dict to be updated.
+        :param queries: Query parameters tuple list to be updated.
+        :resource_path: A string representation of the HTTP request resource path.
+        :method: A string representation of the HTTP request method.
+        :body: A object representing the body of the HTTP request.
+        The object type is the return value of sanitize_for_serialization().
+        :param auth_setting: auth settings for the endpoint
+        """
         if auth_setting['in'] == 'cookie':
-            headers['Cookie'] = auth_setting['key'] + "=" + auth_setting['value']
+            headers['Cookie'] = auth_setting['value']
         elif auth_setting['in'] == 'header':
             if auth_setting['type'] != 'http-signature':
                 headers[auth_setting['key']] = auth_setting['value']
         elif auth_setting['in'] == 'query':
             queries.append((auth_setting['key'], auth_setting['value']))
         else:
             raise ApiValueError(
                 'Authentication token must be in `query` or `header`'
             )
 
+    def __deserialize_file(self, response):
+        """Deserializes body to file
 
-class Endpoint(object):
-    def __init__(self, settings=None, params_map=None, root_map=None,
-                 headers_map=None, api_client=None, callable=None):
-        """Creates an endpoint
-
-        Args:
-            settings (dict): see below key value pairs
-                'response_type' (tuple/None): response type
-                'auth' (list): a list of auth type keys
-                'endpoint_path' (str): the endpoint path
-                'operation_id' (str): endpoint string identifier
-                'http_method' (str): POST/PUT/PATCH/GET etc
-                'servers' (list): list of str servers that this endpoint is at
-            params_map (dict): see below key value pairs
-                'all' (list): list of str endpoint parameter names
-                'required' (list): list of required parameter names
-                'nullable' (list): list of nullable parameter names
-                'enum' (list): list of parameters with enum values
-                'validation' (list): list of parameters with validations
-            root_map
-                'validations' (dict): the dict mapping endpoint parameter tuple
-                    paths to their validation dictionaries
-                'allowed_values' (dict): the dict mapping endpoint parameter
-                    tuple paths to their allowed_values (enum) dictionaries
-                'openapi_types' (dict): param_name to openapi type
-                'attribute_map' (dict): param_name to camelCase name
-                'location_map' (dict): param_name to  'body', 'file', 'form',
-                    'header', 'path', 'query'
-                collection_format_map (dict): param_name to `csv` etc.
-            headers_map (dict): see below key value pairs
-                'accept' (list): list of Accept header strings
-                'content_type' (list): list of Content-Type header strings
-            api_client (ApiClient) api client instance
-            callable (function): the function which is invoked when the
-                Endpoint is called
-        """
-        self.settings = settings
-        self.params_map = params_map
-        self.params_map['all'].extend([
-            'async_req',
-            '_host_index',
-            '_preload_content',
-            '_request_timeout',
-            '_return_http_data_only',
-            '_check_input_type',
-            '_check_return_type',
-            '_content_type',
-            '_spec_property_naming',
-            '_request_auths'
-        ])
-        self.params_map['nullable'].extend(['_request_timeout'])
-        self.validations = root_map['validations']
-        self.allowed_values = root_map['allowed_values']
-        self.openapi_types = root_map['openapi_types']
-        extra_types = {
-            'async_req': (bool,),
-            '_host_index': (none_type, int),
-            '_preload_content': (bool,),
-            '_request_timeout': (none_type, float, (float,), [float], int, (int,), [int]),
-            '_return_http_data_only': (bool,),
-            '_check_input_type': (bool,),
-            '_check_return_type': (bool,),
-            '_spec_property_naming': (bool,),
-            '_content_type': (none_type, str),
-            '_request_auths': (none_type, list)
-        }
-        self.openapi_types.update(extra_types)
-        self.attribute_map = root_map['attribute_map']
-        self.location_map = root_map['location_map']
-        self.collection_format_map = root_map['collection_format_map']
-        self.headers_map = headers_map
-        self.api_client = api_client
-        self.callable = callable
-
-    def __validate_inputs(self, kwargs):
-        for param in self.params_map['enum']:
-            if param in kwargs:
-                check_allowed_values(
-                    self.allowed_values,
-                    (param,),
-                    kwargs[param]
-                )
+        Saves response body into a file in a temporary folder,
+        using the filename from the `Content-Disposition` header if provided.
 
-        for param in self.params_map['validation']:
-            if param in kwargs:
-                check_validations(
-                    self.validations,
-                    (param,),
-                    kwargs[param],
-                    configuration=self.api_client.configuration
-                )
+        :param response:  RESTResponse.
+        :return: file path.
+        """
+        fd, path = tempfile.mkstemp(dir=self.configuration.temp_folder_path)
+        os.close(fd)
+        os.remove(path)
 
-        if kwargs['_check_input_type'] is False:
-            return
+        content_disposition = response.getheader("Content-Disposition")
+        if content_disposition:
+            filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
+                                 content_disposition).group(1)
+            path = os.path.join(os.path.dirname(path), filename)
 
-        for key, value in kwargs.items():
-            fixed_val = validate_and_convert_types(
-                value,
-                self.openapi_types[key],
-                [key],
-                kwargs['_spec_property_naming'],
-                kwargs['_check_input_type'],
-                configuration=self.api_client.configuration
-            )
-            kwargs[key] = fixed_val
+        with open(path, "wb") as f:
+            f.write(response.data)
 
-    def __gather_params(self, kwargs):
-        params = {
-            'body': None,
-            'collection_format': {},
-            'file': {},
-            'form': [],
-            'header': {},
-            'path': {},
-            'query': []
-        }
-
-        for param_name, param_value in kwargs.items():
-            param_location = self.location_map.get(param_name)
-            if param_location is None:
-                continue
-            if param_location:
-                if param_location == 'body':
-                    params['body'] = param_value
-                    continue
-                base_name = self.attribute_map[param_name]
-                if (param_location == 'form' and
-                        self.openapi_types[param_name] == (file_type,)):
-                    params['file'][base_name] = [param_value]
-                elif (param_location == 'form' and
-                        self.openapi_types[param_name] == ([file_type],)):
-                    # param_value is already a list
-                    params['file'][base_name] = param_value
-                elif param_location in {'form', 'query'}:
-                    param_value_full = (base_name, param_value)
-                    params[param_location].append(param_value_full)
-                if param_location not in {'form', 'query'}:
-                    params[param_location][base_name] = param_value
-                collection_format = self.collection_format_map.get(param_name)
-                if collection_format:
-                    params['collection_format'][base_name] = collection_format
+        return path
 
-        return params
+    def __deserialize_primitive(self, data, klass):
+        """Deserializes string to primitive type.
+
+        :param data: str.
+        :param klass: class literal.
 
-    def __call__(self, *args, **kwargs):
-        """ This method is invoked when endpoints are called
-        Example:
+        :return: int, long, float, str, bool.
+        """
+        try:
+            return klass(data)
+        except UnicodeEncodeError:
+            return str(data)
+        except TypeError:
+            return data
 
-        api_instance = CloudApi()
-        api_instance.instance_cloud_impact_v1_cloud_aws_post  # this is an instance of the class Endpoint
-        api_instance.instance_cloud_impact_v1_cloud_aws_post()  # this invokes api_instance.instance_cloud_impact_v1_cloud_aws_post.__call__()
-        which then invokes the callable functions stored in that endpoint at
-        api_instance.instance_cloud_impact_v1_cloud_aws_post.callable or self.callable in this class
+    def __deserialize_object(self, value):
+        """Return an original value.
 
+        :return: object.
         """
-        return self.callable(self, *args, **kwargs)
+        return value
 
-    def call_with_http_info(self, **kwargs):
+    def __deserialize_date(self, string):
+        """Deserializes string to date.
 
+        :param string: str.
+        :return: date.
+        """
         try:
-            index = self.api_client.configuration.server_operation_index.get(
-                self.settings['operation_id'], self.api_client.configuration.server_index
-            ) if kwargs['_host_index'] is None else kwargs['_host_index']
-            server_variables = self.api_client.configuration.server_operation_variables.get(
-                self.settings['operation_id'], self.api_client.configuration.server_variables
-            )
-            _host = self.api_client.configuration.get_host_from_settings(
-                index, variables=server_variables, servers=self.settings['servers']
+            return parse(string).date()
+        except ImportError:
+            return string
+        except ValueError:
+            raise rest.ApiException(
+                status=0,
+                reason="Failed to parse `{0}` as date object".format(string)
             )
-        except IndexError:
-            if self.settings['servers']:
-                raise ApiValueError(
-                    "Invalid host index. Must be 0 <= index < %s" %
-                    len(self.settings['servers'])
-                )
-            _host = None
 
-        for key, value in kwargs.items():
-            if key not in self.params_map['all']:
-                raise ApiTypeError(
-                    "Got an unexpected parameter '%s'"
-                    " to method `%s`" %
-                    (key, self.settings['operation_id'])
-                )
-            # only throw this nullable ApiValueError if _check_input_type
-            # is False, if _check_input_type==True we catch this case
-            # in self.__validate_inputs
-            if (key not in self.params_map['nullable'] and value is None
-                    and kwargs['_check_input_type'] is False):
-                raise ApiValueError(
-                    "Value may not be None for non-nullable parameter `%s`"
-                    " when calling `%s`" %
-                    (key, self.settings['operation_id'])
-                )
+    def __deserialize_datetime(self, string):
+        """Deserializes string to datetime.
 
-        for key in self.params_map['required']:
-            if key not in kwargs.keys():
-                raise ApiValueError(
-                    "Missing the required parameter `%s` when calling "
-                    "`%s`" % (key, self.settings['operation_id'])
-                )
+        The string should be in iso8601 datetime format.
 
-        self.__validate_inputs(kwargs)
+        :param string: str.
+        :return: datetime.
+        """
+        try:
+            return parse(string)
+        except ImportError:
+            return string
+        except ValueError:
+            raise rest.ApiException(
+                status=0,
+                reason=(
+                    "Failed to parse `{0}` as datetime object"
+                    .format(string)
+                )
+            )
 
-        params = self.__gather_params(kwargs)
+    def __deserialize_model(self, data, klass):
+        """Deserializes list or dict to model.
 
-        accept_headers_list = self.headers_map['accept']
-        if accept_headers_list:
-            params['header']['Accept'] = self.api_client.select_header_accept(
-                accept_headers_list)
+        :param data: dict, list.
+        :param klass: class literal.
+        :return: model object.
+        """
 
-        if kwargs.get('_content_type'):
-            params['header']['Content-Type'] = kwargs['_content_type']
-        else:
-            content_type_headers_list = self.headers_map['content_type']
-            if content_type_headers_list:
-                if params['body'] != "":
-                    content_types_list = self.api_client.select_header_content_type(
-                        content_type_headers_list, self.settings['http_method'],
-                        params['body'])
-                    if content_types_list:
-                        params['header']['Content-Type'] = content_types_list
-
-        return self.api_client.call_api(
-            self.settings['endpoint_path'], self.settings['http_method'],
-            params['path'],
-            params['query'],
-            params['header'],
-            body=params['body'],
-            post_params=params['form'],
-            files=params['file'],
-            response_type=self.settings['response_type'],
-            auth_settings=self.settings['auth'],
-            async_req=kwargs['async_req'],
-            _check_type=kwargs['_check_return_type'],
-            _return_http_data_only=kwargs['_return_http_data_only'],
-            _preload_content=kwargs['_preload_content'],
-            _request_timeout=kwargs['_request_timeout'],
-            _host=_host,
-            _request_auths=kwargs['_request_auths'],
-            collection_formats=params['collection_format'])
+        return klass.from_dict(data)
```

### Comparing `boaviztapi-sdk-0.1.2/boaviztapi_sdk/configuration.py` & `boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,70 @@
+# coding: utf-8
+
 """
     BOAVIZTAPI - DEMO
 
-    # 🎯 Retrieving the impacts of digital elements This is a quick demo, to see full documentation [click here](https://doc.api.boavizta.org)  ## ➡️Server router  ### Server routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |     X    | |   ADP  |        X       |     X    | |   PE   |        X       |     X    | ## ➡️Cloud router  ### Cloud routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |     X    | |   ADP  |        X       |     X    | |   PE   |        X       |     X    | ## ➡️Component router  ### Component routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |          | |   ADP  |        X       |          | |   PE   |        X       |          |   # noqa: E501
+    <p>🎯 Retrieving the impacts of digital elements.</p> <p>This is a quick demo, to see full documentation <a href=\"https://doc.api.boavizta.org\">click here</a></p> <h2>Features</h2> <p>Bellow a list of all available features.</p> <h3>👄 Verbose</h3> <p>Verbose is an HTTP parameter. If set at true :</p> <ul> <li>Shows the impacts of each component</li> <li>Shows the value used for each attribute</li> </ul> <p><em>\"attribute\": {\"value\": \"value\", \"unit\": \"unit\", \"status\": \"Status\", \"source\": \"Source\", \"min\":\"min\", \"max\":\"max\", \"significant_figures\":\"significant_figures\"}</em></p> <h3>🔨 Embedded</h3> <ul> <li>Embedded impacts are the impacts occurring during raw material extraction, manufacture, distribution and end of life</li> <li>When end of life is not taken into account, we specified it in the <code>warnings</code></li> </ul> <h3>🔌  Usage</h3> <p>Usage impacts are assessed by multiplying :</p> <ul> <li> <p>a <strong>duration</strong></p> </li> <li> <p>an <strong>impact factor</strong> </p> </li> <li> <p>an <strong>electrical consumption</strong> </p> </li> </ul> <h4>⏲ Duration</h4> <p>Usage impacts can be given as a router parameter, in hours.</p> <p>If no duration is given, <strong>the impact is assess for the all life duration of the asset</strong>.</p> <h4>✖️ Impact factors</h4> <ul> <li>Impact factors can be given : <em>\"usage\":{\"elec_factors\":{[criterion]_factors: 0.38}}</em></li> <li> <p>Impact factors can be retrieved from : <em>\"usage\":{\"usage_location\": \"FRA\"}</em>. </p> </li> <li> <p>See the list of locations : <a href=\"/v1/utils/country_code\">/v1/utils/country_code</a>*</p> </li> </ul> <h4>⚡ Electrical consumption</h4> <h5>⏺️ Given</h5> <ul> <li>Electrical consumption can be given for one hour (average) <em>\"usage\":{\"avg_power\": 1}</em>.</li> </ul> <h5>📈 Modeled</h5> <ul> <li>Electrical consumption can be retrieved from consumption profile using <em>usage:{time_workload: 50}</em>.</li> </ul> <h5>📋 Archetype</h5> <ul> <li>In some cases, default electrical consumption can be taken from the archetype</li> </ul> <h3>🔃 Auto-complete &amp; 📋 Archetype</h3> <p>The API will complete the missing attributes in a request with a completion function or with values taken from the <code>archetype</code> specified in the route parameter.</p> <h3>⏬ Allocation</h3> <ul> <li>Usage impacts are assessed on the duration given in route parameter</li> <li>Embedded impacts are allocated linearly on the duration given in parameter <code>embedded_impact = impact * (duration/life_duration)</code></li> </ul> <p>If no duration is given, the life_duration (<code>`hours_life_time</code>) of the asset is used.</p>  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0a4
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-    The version of the OpenAPI document: 0.1.2
-    Generated by: https://openapi-generator.tech
+    Do not edit the class manually.
 """
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
+import http.client as httplib
 from boaviztapi_sdk.exceptions import ApiValueError
 
-
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
+    """This class contains various settings of the API client.
 
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format
+      in PEM format.
 
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
-                 access_token=None,
                  username=None, password=None,
-                 discard_unknown_keys=False,
-                 disabled_client_side_validations="",
+                 access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ):
         """Constructor
         """
         self._base_path = "http://localhost" if host is None else host
@@ -103,15 +78,14 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.access_token = access_token
         self.api_key = {}
         if api_key:
             self.api_key = api_key
         """dict to store API key(s)
         """
         self.api_key_prefix = {}
         if api_key_prefix:
@@ -123,16 +97,17 @@
         """
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
-        self.discard_unknown_keys = discard_unknown_keys
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("boaviztapi_sdk")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -163,43 +138,53 @@
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
         self.proxy = None
         """Proxy URL
         """
-        self.no_proxy = None
-        """bypass proxy for host in the no_proxy list.
-        """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -209,46 +194,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -294,23 +282,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -375,15 +363,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.2\n"\
+               "Version of the API: 1.0.0a4\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `boaviztapi-sdk-0.1.2/boaviztapi_sdk/rest.py` & `boaviztapi-sdk-1.0.0a4/boaviztapi_sdk/rest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+# coding: utf-8
+
 """
     BOAVIZTAPI - DEMO
 
-    # 🎯 Retrieving the impacts of digital elements This is a quick demo, to see full documentation [click here](https://doc.api.boavizta.org)  ## ➡️Server router  ### Server routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |     X    | |   ADP  |        X       |     X    | |   PE   |        X       |     X    | ## ➡️Cloud router  ### Cloud routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |     X    | |   ADP  |        X       |     X    | |   PE   |        X       |     X    | ## ➡️Component router  ### Component routers support the following impacts:  | Impact | 🔨 Manufacture | 🔌 Usage | |--------|----------------|----------| |   GWP  |        X       |          | |   ADP  |        X       |          | |   PE   |        X       |          |   # noqa: E501
+    <p>🎯 Retrieving the impacts of digital elements.</p> <p>This is a quick demo, to see full documentation <a href=\"https://doc.api.boavizta.org\">click here</a></p> <h2>Features</h2> <p>Bellow a list of all available features.</p> <h3>👄 Verbose</h3> <p>Verbose is an HTTP parameter. If set at true :</p> <ul> <li>Shows the impacts of each component</li> <li>Shows the value used for each attribute</li> </ul> <p><em>\"attribute\": {\"value\": \"value\", \"unit\": \"unit\", \"status\": \"Status\", \"source\": \"Source\", \"min\":\"min\", \"max\":\"max\", \"significant_figures\":\"significant_figures\"}</em></p> <h3>🔨 Embedded</h3> <ul> <li>Embedded impacts are the impacts occurring during raw material extraction, manufacture, distribution and end of life</li> <li>When end of life is not taken into account, we specified it in the <code>warnings</code></li> </ul> <h3>🔌  Usage</h3> <p>Usage impacts are assessed by multiplying :</p> <ul> <li> <p>a <strong>duration</strong></p> </li> <li> <p>an <strong>impact factor</strong> </p> </li> <li> <p>an <strong>electrical consumption</strong> </p> </li> </ul> <h4>⏲ Duration</h4> <p>Usage impacts can be given as a router parameter, in hours.</p> <p>If no duration is given, <strong>the impact is assess for the all life duration of the asset</strong>.</p> <h4>✖️ Impact factors</h4> <ul> <li>Impact factors can be given : <em>\"usage\":{\"elec_factors\":{[criterion]_factors: 0.38}}</em></li> <li> <p>Impact factors can be retrieved from : <em>\"usage\":{\"usage_location\": \"FRA\"}</em>. </p> </li> <li> <p>See the list of locations : <a href=\"/v1/utils/country_code\">/v1/utils/country_code</a>*</p> </li> </ul> <h4>⚡ Electrical consumption</h4> <h5>⏺️ Given</h5> <ul> <li>Electrical consumption can be given for one hour (average) <em>\"usage\":{\"avg_power\": 1}</em>.</li> </ul> <h5>📈 Modeled</h5> <ul> <li>Electrical consumption can be retrieved from consumption profile using <em>usage:{time_workload: 50}</em>.</li> </ul> <h5>📋 Archetype</h5> <ul> <li>In some cases, default electrical consumption can be taken from the archetype</li> </ul> <h3>🔃 Auto-complete &amp; 📋 Archetype</h3> <p>The API will complete the missing attributes in a request with a completion function or with values taken from the <code>archetype</code> specified in the route parameter.</p> <h3>⏬ Allocation</h3> <ul> <li>Usage impacts are assessed on the duration given in route parameter</li> <li>Embedded impacts are allocated linearly on the duration given in parameter <code>embedded_impact = impact * (duration/life_duration)</code></li> </ul> <p>If no duration is given, the life_duration (<code>`hours_life_time</code>) of the asset is used.</p>  # noqa: E501
+
+    The version of the OpenAPI document: 1.0.0a4
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-    The version of the OpenAPI document: 0.1.2
-    Generated by: https://openapi-generator.tech
+    Do not edit the class manually.
 """
 
 
 import io
 import json
 import logging
 import re
 import ssl
-from urllib.parse import urlencode
-from urllib.parse import urlparse
-from urllib.request import proxy_bypass_environment
+
+from urllib.parse import urlencode, quote_plus
 import urllib3
-import ipaddress
 
-from boaviztapi_sdk.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from boaviztapi_sdk.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError, BadRequestException
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
 
@@ -31,19 +33,19 @@
         self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
         """Returns a dictionary of the response headers."""
-        return self.urllib3_response.getheaders()
+        return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
-        return self.urllib3_response.getheader(name, default)
+        return self.urllib3_response.headers.get(name, default)
 
 
 class RESTClientObject(object):
 
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
@@ -60,26 +62,29 @@
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.tls_server_name:
+            addition_pool_args['server_hostname'] = configuration.tls_server_name
+
+
         if configuration.socket_options is not None:
             addition_pool_args['socket_options'] = configuration.socket_options
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
         # https pool manager
-        if configuration.proxy and not should_bypass_proxies(
-                configuration.host, no_proxy=configuration.no_proxy or ''):
+        if configuration.proxy:
             self.pool_manager = urllib3.ProxyManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
@@ -126,34 +131,33 @@
         if post_params and body:
             raise ApiValueError(
                 "body parameter cannot be used with post_params parameter."
             )
 
         post_params = post_params or {}
         headers = headers or {}
+        # url already contains the URL query string
+        # so reset query_params to empty dict
+        query_params = {}
 
         timeout = None
         if _request_timeout:
-            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
+            if isinstance(_request_timeout, (int,float)):  # noqa: E501,F821
                 timeout = urllib3.Timeout(total=_request_timeout)
             elif (isinstance(_request_timeout, tuple) and
                   len(_request_timeout) == 2):
                 timeout = urllib3.Timeout(
                     connect=_request_timeout[0], read=_request_timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
-                if (method != 'DELETE') and ('Content-Type' not in headers):
-                    headers['Content-Type'] = 'application/json'
-                if query_params:
-                    url += '?' + urlencode(query_params)
-                if ('Content-Type' not in headers) or (re.search('json',
-                                                                 headers['Content-Type'], re.IGNORECASE)):
+
+                # no content type provided or payload is json
+                if not headers.get('Content-Type') or re.search('json', headers['Content-Type'], re.IGNORECASE):
                     request_body = None
                     if body is not None:
                         request_body = json.dumps(body)
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
                         preload_content=_preload_content,
@@ -195,29 +199,32 @@
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
                 r = self.pool_manager.request(method, url,
-                                              fields=query_params,
+                                              fields={},
                                               preload_content=_preload_content,
                                               timeout=timeout,
                                               headers=headers)
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
         if _preload_content:
             r = RESTResponse(r)
 
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
+            if r.status == 400:
+                raise BadRequestException(http_resp=r)
+
             if r.status == 401:
                 raise UnauthorizedException(http_resp=r)
 
             if r.status == 403:
                 raise ForbiddenException(http_resp=r)
 
             if r.status == 404:
@@ -226,127 +233,71 @@
             if 500 <= r.status <= 599:
                 raise ServiceException(http_resp=r)
 
             raise ApiException(http_resp=r)
 
         return r
 
-    def GET(self, url, headers=None, query_params=None, _preload_content=True,
+    def get_request(self, url, headers=None, query_params=None, _preload_content=True,
             _request_timeout=None):
         return self.request("GET", url,
                             headers=headers,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             query_params=query_params)
 
-    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
+    def head_request(self, url, headers=None, query_params=None, _preload_content=True,
              _request_timeout=None):
         return self.request("HEAD", url,
                             headers=headers,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             query_params=query_params)
 
-    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
+    def options_request(self, url, headers=None, query_params=None, post_params=None,
                 body=None, _preload_content=True, _request_timeout=None):
         return self.request("OPTIONS", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def DELETE(self, url, headers=None, query_params=None, body=None,
+    def delete_request(self, url, headers=None, query_params=None, body=None,
                _preload_content=True, _request_timeout=None):
         return self.request("DELETE", url,
                             headers=headers,
                             query_params=query_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def POST(self, url, headers=None, query_params=None, post_params=None,
+    def post_request(self, url, headers=None, query_params=None, post_params=None,
              body=None, _preload_content=True, _request_timeout=None):
         return self.request("POST", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def PUT(self, url, headers=None, query_params=None, post_params=None,
+    def put_request(self, url, headers=None, query_params=None, post_params=None,
             body=None, _preload_content=True, _request_timeout=None):
         return self.request("PUT", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def PATCH(self, url, headers=None, query_params=None, post_params=None,
+    def patch_request(self, url, headers=None, query_params=None, post_params=None,
               body=None, _preload_content=True, _request_timeout=None):
         return self.request("PATCH", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
-
-# end of class RESTClientObject
-
-
-def is_ipv4(target):
-    """ Test if IPv4 address or not
-    """
-    try:
-        chk = ipaddress.IPv4Address(target)
-        return True
-    except ipaddress.AddressValueError:
-        return False
-
-
-def in_ipv4net(target, net):
-    """ Test if target belongs to given IPv4 network
-    """
-    try:
-        nw = ipaddress.IPv4Network(net)
-        ip = ipaddress.IPv4Address(target)
-        if ip in nw:
-            return True
-        return False
-    except ipaddress.AddressValueError:
-        return False
-    except ipaddress.NetmaskValueError:
-        return False
-
-
-def should_bypass_proxies(url, no_proxy=None):
-    """ Yet another requests.should_bypass_proxies
-    Test if proxies should not be used for a particular url.
-    """
-
-    parsed = urlparse(url)
-
-    # special cases
-    if parsed.hostname in [None, '']:
-        return True
-
-    # special cases
-    if no_proxy in [None, '']:
-        return False
-    if no_proxy == '*':
-        return True
-
-    no_proxy = no_proxy.lower().replace(' ', '');
-    entries = (
-        host for host in no_proxy.split(',') if host
-    )
-
-    if is_ipv4(parsed.hostname):
-        for item in entries:
-            if in_ipv4net(parsed.hostname, item):
-                return True
-    return proxy_bypass_environment(parsed.hostname, {'no': no_proxy})
```

