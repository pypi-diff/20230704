# Comparing `tmp/gantry-0.6.8.tar.gz` & `tmp/gantry-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.6.8.tar", last modified: Sat Jul  1 00:55:04 2023, max compression
+gzip compressed data, was "gantry-0.6.9.tar", last modified: Tue Jul  4 00:41:55 2023, max compression
```

## Comparing `gantry-0.6.8.tar` & `gantry-0.6.9.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.363473 gantry-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-01 00:54:52.000000 gantry-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-01 00:54:52.000000 gantry-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-01 00:55:04.363473 gantry-0.6.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.323473 gantry-0.6.8/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.327473 gantry-0.6.8/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.327473 gantry-0.6.8/gantry/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30565 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.327473 gantry-0.6.8/gantry/automations/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.331473 gantry-0.6.8/gantry/automations/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.331473 gantry-0.6.8/gantry/automations/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/stock_curators.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.331473 gantry-0.6.8/gantry/automations/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/triggers/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.335473 gantry-0.6.8/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.335473 gantry-0.6.8/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.335473 gantry-0.6.8/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.339473 gantry-0.6.8/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.339473 gantry-0.6.8/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    94223 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.343473 gantry-0.6.8/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.343473 gantry-0.6.8/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    39714 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.343473 gantry-0.6.8/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.343473 gantry-0.6.8/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.323473 gantry-0.6.8/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 00:55:04.363473 gantry-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-01 00:54:52.000000 gantry-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.347473 gantry-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.347473 gantry-0.6.8/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.351473 gantry-0.6.8/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/test_llm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.351473 gantry-0.6.8/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.355473 gantry-0.6.8/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.355473 gantry-0.6.8/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.355473 gantry-0.6.8/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.359473 gantry-0.6.8/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   110166 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.359473 gantry-0.6.8/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.363473 gantry-0.6.8/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.363473 gantry-0.6.8/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.363473 gantry-0.6.8/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.558759 gantry-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-04 00:41:44.000000 gantry-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-04 00:41:44.000000 gantry-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-04 00:41:55.558759 gantry-0.6.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.530759 gantry-0.6.9/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.534759 gantry-0.6.9/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.538759 gantry-0.6.9/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30565 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17982 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/applications/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/applications/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.538759 gantry-0.6.9/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.538759 gantry-0.6.9/gantry/automations/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.542759 gantry-0.6.9/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.542759 gantry-0.6.9/gantry/automations/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/automations/triggers/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.546759 gantry-0.6.9/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.546759 gantry-0.6.9/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.546759 gantry-0.6.9/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.546759 gantry-0.6.9/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.550759 gantry-0.6.9/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94223 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.550759 gantry-0.6.9/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.550759 gantry-0.6.9/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39714 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.550759 gantry-0.6.9/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.550759 gantry-0.6.9/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 00:41:44.000000 gantry-0.6.9/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.534759 gantry-0.6.9/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-04 00:41:55.000000 gantry-0.6.9/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-04 00:41:55.000000 gantry-0.6.9/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:41:55.000000 gantry-0.6.9/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 00:41:55.000000 gantry-0.6.9/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-04 00:41:55.000000 gantry-0.6.9/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 00:41:55.000000 gantry-0.6.9/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:41:55.558759 gantry-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-04 00:41:44.000000 gantry-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.550759 gantry-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.554759 gantry-0.6.9/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.554759 gantry-0.6.9/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/applications/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/applications/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/applications/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/applications/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/applications/test_llm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.554759 gantry-0.6.9/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.554759 gantry-0.6.9/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.554759 gantry-0.6.9/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.554759 gantry-0.6.9/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.554759 gantry-0.6.9/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110166 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.558759 gantry-0.6.9/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.558759 gantry-0.6.9/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.558759 gantry-0.6.9/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:55.558759 gantry-0.6.9/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-04 00:41:44.000000 gantry-0.6.9/tests/test_validator.py
```

### Comparing `gantry-0.6.8/LICENSE` & `gantry-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/PKG-INFO` & `gantry-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.8
+Version: 0.6.9
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.8/gantry/__init__.py` & `gantry-0.6.9/gantry/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/alerts/client.py` & `gantry-0.6.9/gantry/alerts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
                 application_data_nodes = (
                     application_schema["prediction_datanodes"]
                     + application_schema["feedback_datanodes"]
                 )
                 application_data_nodes_map = {}
                 for data_node in application_data_nodes:
                     application_data_nodes_map[data_node["name"]] = data_node["user_dtype"]
-
+                application_data_nodes_map["__time"] = "Unix_Time"
                 for i in range(len(check_as_dict["subqueries"])):
                     subquery = check_as_dict["subqueries"][i]
                     if subquery["field_names"][0] not in application_data_nodes_map:
                         raise ValueError(
                             f'Could not find "{subquery["field_names"]}"'
                             f'in application "{application_name}".'
                         )
```

### Comparing `gantry-0.6.8/gantry/alerts/globals.py` & `gantry-0.6.9/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/alerts/main.py` & `gantry-0.6.9/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/api_client.py` & `gantry-0.6.9/gantry/api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/applications/client.py` & `gantry-0.6.9/gantry/applications/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/applications/core.py` & `gantry-0.6.9/gantry/applications/core.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/applications/llm.py` & `gantry-0.6.9/gantry/applications/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,15 @@
             ),
             raise_for_status=True,
         )
         config_data = res["data"][0]
 
         return VersionDetails(
             config=config_data,
-            description=version_data["notes"],
+            description=version_data["description"],
             app_name=self._name,
             version_id=uuid.UUID(version_data["id"]),
             version_number=version_data["version"],
         )
 
     def log_completion(
         self,
```

### Comparing `gantry-0.6.8/gantry/applications/llm_utils.py` & `gantry-0.6.9/gantry/applications/llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/applications/main.py` & `gantry-0.6.9/gantry/applications/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/actions/actions.py` & `gantry-0.6.9/gantry/automations/actions/actions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/automations.py` & `gantry-0.6.9/gantry/automations/automations.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/curators/__init__.py` & `gantry-0.6.9/gantry/automations/curators/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/curators/curators.py` & `gantry-0.6.9/gantry/automations/curators/curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/curators/main.py` & `gantry-0.6.9/gantry/automations/curators/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/curators/models.py` & `gantry-0.6.9/gantry/automations/curators/models.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/curators/selectors.py` & `gantry-0.6.9/gantry/automations/curators/selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/curators/stock_curators.py` & `gantry-0.6.9/gantry/automations/curators/stock_curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/main.py` & `gantry-0.6.9/gantry/automations/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/automations/triggers/triggers.py` & `gantry-0.6.9/gantry/automations/triggers/triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,22 +188,24 @@
 
     def compile_subqueries(self):
         subqueries = []
         for query, aggregation in zip(self.queries, self.query_aggregation):
             self.api_client = query.api_client
             if not query.relative_time_window:
                 raise ValueError("Relative time window must be specified for all queries")
-            tags_as_filters = [
-                {
-                    "feature_name": tag_key,
-                    "category_query": [tag_value],
-                    "dtype": "tag",
-                }
-                for tag_key, tag_value in query.tags.items()
-            ]
+            tags_as_filters = []
+            if query.tags:
+                tags_as_filters = [
+                    {
+                        "feature_name": tag_key,
+                        "category_query": [tag_value],
+                        "dtype": "tag",
+                    }
+                    for tag_key, tag_value in query.tags.items()
+                ]
             subquery = {
                 "app_name": query.application,
                 "field_names": self.fields,
                 "aggregation": aggregation.value,
                 "filters": query.filters + tags_as_filters,
                 "relative_time_window": to_isoformat_duration(query.relative_time_window),
                 "relative_time_delay": to_isoformat_duration(query.relative_time_delay)
```

### Comparing `gantry-0.6.8/gantry/cli/application.py` & `gantry-0.6.9/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/cli/bucket.py` & `gantry-0.6.9/gantry/cli/bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/cli/data_connector.py` & `gantry-0.6.9/gantry/cli/data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/cli/labeling.py` & `gantry-0.6.9/gantry/cli/labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/cli/main.py` & `gantry-0.6.9/gantry/cli/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/cli/projection.py` & `gantry-0.6.9/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/cli/secret.py` & `gantry-0.6.9/gantry/cli/secret.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/data_generator/data_generator.py` & `gantry-0.6.9/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/dataset/client.py` & `gantry-0.6.9/gantry/dataset/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/dataset/constants.py` & `gantry-0.6.9/gantry/dataset/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/dataset/gantry_dataset.py` & `gantry-0.6.9/gantry/dataset/gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/dataset/main.py` & `gantry-0.6.9/gantry/dataset/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.9/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/exceptions.py` & `gantry-0.6.9/gantry/exceptions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/logger/client.py` & `gantry-0.6.9/gantry/logger/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/logger/constants.py` & `gantry-0.6.9/gantry/logger/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/logger/consumer.py` & `gantry-0.6.9/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/logger/event_builder.py` & `gantry-0.6.9/gantry/logger/event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/logger/main.py` & `gantry-0.6.9/gantry/logger/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/logger/stores.py` & `gantry-0.6.9/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/logger/types.py` & `gantry-0.6.9/gantry/logger/types.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/logger/utils.py` & `gantry-0.6.9/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/__init__.py` & `gantry-0.6.9/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/client.py` & `gantry-0.6.9/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/core/dataframe.py` & `gantry-0.6.9/gantry/query/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/core/distance.py` & `gantry-0.6.9/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/core/metric.py` & `gantry-0.6.9/gantry/query/core/metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/core/queryframe.py` & `gantry-0.6.9/gantry/query/core/queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/core/utils.py` & `gantry-0.6.9/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/distance/main.py` & `gantry-0.6.9/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/globals.py` & `gantry-0.6.9/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/main.py` & `gantry-0.6.9/gantry/query/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/metric/__init__.py` & `gantry-0.6.9/gantry/query/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/metric/main.py` & `gantry-0.6.9/gantry/query/metric/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/query/time_window.py` & `gantry-0.6.9/gantry/query/time_window.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/serializers.py` & `gantry-0.6.9/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/utils.py` & `gantry-0.6.9/gantry/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry/validators.py` & `gantry-0.6.9/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/gantry.egg-info/PKG-INFO` & `gantry-0.6.9/gantry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.8
+Version: 0.6.9
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.8/gantry.egg-info/SOURCES.txt` & `gantry-0.6.9/gantry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/setup.py` & `gantry-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/alerts/test_client.py` & `gantry-0.6.9/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/alerts/test_main.py` & `gantry-0.6.9/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/applications/test_client.py` & `gantry-0.6.9/tests/applications/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/applications/test_core.py` & `gantry-0.6.9/tests/applications/test_core.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/applications/test_llm.py` & `gantry-0.6.9/tests/applications/test_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
                 "data": {
                     "id": str(version_id),
                     "configuration_id": str(uuid.uuid4()),
                     "version": 1,
                     "checksum": "1234",
                     "s3_paths": ["s3://test_bucket/test_path"],
                     "notes": description,
+                    "description": description,
                     "created_at": "2020-01-01T00:00:00.000000Z",
                 },
             },
             headers={"Content-Type": "application/json"},
             match=[
                 matchers.json_params_matcher(
                     {
@@ -196,14 +197,15 @@
     version_data = {
         "id": str(version_id),
         "configuration_id": str(configuration_id),
         "version": 1,
         "checksum": "1234",
         "s3_paths": ["s3://test_bucket/test_path"],
         "notes": description,
+        "description": description,
         "created_at": "2020-01-01T00:00:00.000000Z",
     }
 
     with responses.RequestsMock() as resp:
         resp.add(
             resp.GET,
             (
```

### Comparing `gantry-0.6.8/tests/applications/test_llm_utils.py` & `gantry-0.6.9/tests/applications/test_llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/cli/test_bucket.py` & `gantry-0.6.9/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/cli/test_data_connector.py` & `gantry-0.6.9/tests/cli/test_data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/cli/test_labeling.py` & `gantry-0.6.9/tests/cli/test_labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/cli/test_projection.py` & `gantry-0.6.9/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/cli/test_secrets.py` & `gantry-0.6.9/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/conftest.py` & `gantry-0.6.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/curator/conftest.py` & `gantry-0.6.9/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/curator/test_curator.py` & `gantry-0.6.9/tests/curator/test_curator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/curator/test_main.py` & `gantry-0.6.9/tests/curator/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/curator/test_selectors.py` & `gantry-0.6.9/tests/curator/test_selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/data_generator/test_data_generator.py` & `gantry-0.6.9/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/dataset/conftest.py` & `gantry-0.6.9/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/dataset/test_client.py` & `gantry-0.6.9/tests/dataset/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.9/tests/dataset/test_gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/dataset/test_main.py` & `gantry-0.6.9/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/logger/test_client.py` & `gantry-0.6.9/tests/logger/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/logger/test_consumer.py` & `gantry-0.6.9/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/logger/test_event_builder.py` & `gantry-0.6.9/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/logger/test_main.py` & `gantry-0.6.9/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/logger/test_stores.py` & `gantry-0.6.9/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/logger/test_utils.py` & `gantry-0.6.9/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/conftest.py` & `gantry-0.6.9/tests/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/core/test_dataframe.py` & `gantry-0.6.9/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/core/test_distance.py` & `gantry-0.6.9/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/core/test_filters.py` & `gantry-0.6.9/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/core/test_metric.py` & `gantry-0.6.9/tests/query/core/test_metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/core/test_queryframe.py` & `gantry-0.6.9/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/core/test_series.py` & `gantry-0.6.9/tests/query/core/test_series.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/core/test_utils.py` & `gantry-0.6.9/tests/query/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/distance/test_main.py` & `gantry-0.6.9/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/metric/test_main.py` & `gantry-0.6.9/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/test_client.py` & `gantry-0.6.9/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/query/test_main.py` & `gantry-0.6.9/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/test_api_client.py` & `gantry-0.6.9/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/test_init.py` & `gantry-0.6.9/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/test_utils.py` & `gantry-0.6.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.8/tests/test_validator.py` & `gantry-0.6.9/tests/test_validator.py`

 * *Files identical despite different names*

