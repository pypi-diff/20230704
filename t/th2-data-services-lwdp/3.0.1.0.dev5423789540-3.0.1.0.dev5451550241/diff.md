# Comparing `tmp/th2_data_services_lwdp-3.0.1.0.dev5423789540.tar.gz` & `tmp/th2_data_services_lwdp-3.0.1.0.dev5451550241.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-3.0.1.0.dev5423789540.tar", last modified: Fri Jun 30 14:09:44 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-3.0.1.0.dev5451550241.tar", last modified: Tue Jul  4 06:33:38 2023, max compression
```

## Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540.tar` & `th2_data_services_lwdp-3.0.1.0.dev5451550241.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7683 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-30 14:09:28.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      651 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    60895 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14524 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4354 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7683 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-04 06:33:25.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61689 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14524 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4354 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-04 06:32:11.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-07-04 06:33:37.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-07-04 06:33:38.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 06:33:37.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-04 06:33:37.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-04 06:33:37.000000 th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/PKG-INFO` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 3.0.1.0.dev5423789540
+Version: 3.0.1.0.dev5451550241
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/README.md` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/setup.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,17 +98,15 @@
 
         Returns:
             Data
         """
         self._current_handle_function = self._data_object
         return self
 
-    def _sse_bytes_stream(
-        self, data_source: DataSource
-    ) -> Generator[bytes, None, None]:  # noqa
+    def _sse_bytes_stream(self, data_source: DataSource) -> Generator[bytes, None, None]:  # noqa
         api: API = data_source.source_api
         urls: List[str] = self._get_urls(data_source)
         for url in urls:
             # LOG             logger.info(url)
             yield from api.execute_sse_request(url)
 
     def _sse_events_stream(self, data_source: DataSource) -> Generator[Event, Any, None]:
@@ -1071,14 +1069,19 @@
     """A Class-Command for request to lw-data-provider.
 
     It searches messages stream by page and downloads them.
     Beware that if you request this command with long list of groups,
       you will get multiple files: ‘{filename}.1.gz’, ‘{filename}.2.gz’,
       etc., since the request might exceed url limit.
 
+    File will contain the list of messages for specified groups.
+    Each group will be requested one after another (there is no order guaranties between groups).
+    Messages for a group are not sorted by default.
+    Use sort in order to sort messages for each group
+
     Returns:
         Nothing.
     """
 
     def __init__(
         self,
         filename: str,
@@ -1145,14 +1148,18 @@
     """A Class-Command for request to lw-data-provider.
 
     It searches messages stream by page & groups and downloads them.
     Beware that if you request this command with long list of groups,
       you will get multiple files: ‘{filename}.1.gz’, ‘{filename}.2.gz’,
       etc., since the request might exceed url limit.
 
+    File will contain the list of messages for specified groups.
+    Each group will be requested one after another (there is no order guaranties between groups).
+    Messages for a group are not sorted by default.
+    Use sort in order to sort messages for each group
 
     Returns:
         Nothing.
     """
 
     def __init__(
         self,
@@ -1227,14 +1234,18 @@
     """A Class-Command for request to lw-data-provider.
 
     It searches messages stream by page & groups and downloads them.
     Beware that if you request this command with long list of groups,
       you will get multiple files: ‘{filename}.1.gz’, ‘{filename}.2.gz’,
       etc., since the request might exceed url limit.
 
+    File will contain the list of messages for specified groups.
+    Each group will be requested one after another (there is no order guaranties between groups).
+    Messages for a group are not sorted by default.
+    Use sort in order to sort messages for each group
 
     Returns:
         Nothing.
     """
 
     def __init__(
         self,
```

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/_misc.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 3.0.1.0.dev5423789540
+Version: 3.0.1.0.dev5451550241
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-3.0.1.0.dev5451550241/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

