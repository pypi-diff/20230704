# Comparing `tmp/configurun-0.1.0.tar.gz` & `tmp/configurun-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configurun-0.1.0.tar", last modified: Thu Jun 29 02:29:19 2023, max compression
+gzip compressed data, was "configurun-0.2.0.tar", last modified: Tue Jul  4 19:16:20 2023, max compression
```

## Comparing `configurun-0.1.0.tar` & `configurun-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.057271 configurun-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-06-29 02:29:05.000000 configurun-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 02:29:05.000000 configurun-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-06-29 02:29:19.057271 configurun-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22576 2023-06-29 02:29:05.000000 configurun-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.049271 configurun-0.1.0/configurun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.053271 configurun-0.1.0/configurun/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/classes/method_call_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    51436 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/classes/run_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/classes/run_queue_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/classes/run_queue_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    26575 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/classes/run_queue_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.053271 configurun-0.1.0/configurun/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/configuration/argparse_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/configuration/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    30754 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/configuration/configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.053271 configurun-0.1.0/configurun/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/examples/example_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/examples/example_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/examples/example_configuration_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.057271 configurun-0.1.0/configurun/examples/example_options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/examples/example_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/examples/example_options/example_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/examples/example_options/example_sklearn_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-29 02:29:05.000000 configurun-0.1.0/configurun/examples/example_target_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.057271 configurun-0.1.0/configurun/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1155777 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/res/app_resources_rc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.057271 configurun-0.1.0/configurun/windows/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46152 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.057271 configurun-0.1.0/configurun/windows/models/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/models/run_queue_console_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/models/run_queue_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/network_main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.057271 configurun-0.1.0/configurun/windows/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23373 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/ui/main_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/ui/network_login_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/ui/run_queue_widget_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.057271 configurun-0.1.0/configurun/windows/views/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/views/run_queue_tree_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.057271 configurun-0.1.0/configurun/windows/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/widgets/network_login_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-29 02:29:06.000000 configurun-0.1.0/configurun/windows/widgets/run_queue_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 02:29:19.049271 configurun-0.1.0/configurun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-06-29 02:29:19.000000 configurun-0.1.0/configurun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-29 02:29:19.000000 configurun-0.1.0/configurun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 02:29:19.000000 configurun-0.1.0/configurun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 02:29:19.000000 configurun-0.1.0/configurun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 02:29:19.000000 configurun-0.1.0/configurun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 02:29:19.057271 configurun-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 02:29:06.000000 configurun-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.144353 configurun-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-07-04 19:16:08.000000 configurun-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 19:16:08.000000 configurun-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-07-04 19:16:20.144353 configurun-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26717 2023-07-04 19:16:08.000000 configurun-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.132352 configurun-0.2.0/configurun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.136352 configurun-0.2.0/configurun/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/create_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45877 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.136352 configurun-0.2.0/configurun/app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/models/run_queue_console_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/models/run_queue_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/network_main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.136352 configurun-0.2.0/configurun/app/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/ui/main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/ui/network_login_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/ui/run_queue_widget_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.136352 configurun-0.2.0/configurun/app/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/views/run_queue_tree_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.136352 configurun-0.2.0/configurun/app/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/widgets/network_login_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/app/widgets/run_queue_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.140352 configurun-0.2.0/configurun/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/classes/method_call_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54072 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/classes/run_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/classes/run_queue_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/classes/run_queue_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/classes/run_queue_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.140352 configurun-0.2.0/configurun/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/configuration/argparse_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/configuration/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/configuration/configuration_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.140352 configurun-0.2.0/configurun/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/examples/example_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/examples/example_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/examples/example_configuration_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.140352 configurun-0.2.0/configurun/examples/example_options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/examples/example_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/examples/example_options/example_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/examples/example_options/example_sklearn_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/examples/example_target_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.140352 configurun-0.2.0/configurun/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1155777 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/res/app_resources_rc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.144353 configurun-0.2.0/configurun/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-04 19:16:08.000000 configurun-0.2.0/configurun/server/create_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:16:20.136352 configurun-0.2.0/configurun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-07-04 19:16:20.000000 configurun-0.2.0/configurun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-04 19:16:20.000000 configurun-0.2.0/configurun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:16:20.000000 configurun-0.2.0/configurun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-04 19:16:20.000000 configurun-0.2.0/configurun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 19:16:20.000000 configurun-0.2.0/configurun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:16:20.144353 configurun-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-04 19:16:08.000000 configurun-0.2.0/setup.py
```

### Comparing `configurun-0.1.0/LICENSE` & `configurun-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configurun-0.1.0/PKG-INFO` & `configurun-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,406 +1,486 @@
-Metadata-Version: 2.1
-Name: configurun
-Version: 0.1.0
-Summary: PySide6 based user-interface tools to create and manage machine learning training/testing-configurations and run them automatically and/or remotely..
-Home-page: https://github.com/Woutah/configurun
-Author: Wouter Stokman
-License: LGPLv2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Configurun
-Configurun is a cross-platform PySide6-based package that implements an application for managing, creating and (remotely) running python configurations. 
-It was designed mainly with machine-learning tasks in mind, but can be used for any python script that takes arguments as an input. The editor-UI is created automatically using either an `argparse.Argumentparser` or python-`@dataclass`(es).
-
-
-The Configurun-app is especially useful for scripts/experiments that require a lot of arguments to be tweaked across many experiment-runs. It also makes the process of running experiments remotely much easier by enabling the user to edit, add and schedule tasks on any running Configurun server-instance reachable via a network connection.
-
-This package was created in tandem with [pyside6-utils](https://github.com/Woutah/pyside6-utils/).
-
-
-<p align="center">
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/main_window_example.png" width="1200" />
-</p>
-
-# Table of contents
-- [Configurun](#configurun)
-- [Table of contents](#table-of-contents)
-- [Features](#features)
-	- [Configuration Editor](#configuration-editor)
-	- [Run Queue](#run-queue)
-	- [Remote-processing](#remote-processing)
-- [Installation](#installation)
-- [How to run?](#how-to-run)
-	- [Local App](#local-app)
-	- [Client App](#client-app)
-	- [Server-instance](#server-instance)
-- [Option-source](#option-source)
-	- [Custom Options (`@dataclass`)](#custom-options-dataclass)
-	- [Custom Options (`ArgumentParser`)](#custom-options-argumentparser)
-	- [Custom Options (`Callable`)](#custom-options-callable)
-- [Target Function](#target-function)
-- [Configuration](#configuration)
-- [Option metadata](#option-metadata)
-
-
-# Features
-## Configuration Editor
-The configuration editor allows the user to specify a configuration-template using either (groups of) [`@dataclass`-class](#custom-options-dataclass) or an [`ArgumentParser`-instance](#custom-options-dataclass). The editor will then automatically create a UI based on the provided template. Editors are specifically created for each option-property based on provided template-types (and [extra constraints](#option-metadata)). Help-messages are displayed on hover, required arguments are highlighted when not filled in, etc.
-<p align="center">
-	<!-- <img src="./configurun/examples/images/configuration_editor_example.png" width="600" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/configuration_editor_example.png" width="600" />
-</p>
-
-We can also define our own [option-source-method](#custom-options-callable) to dynamically create new option-groups based on the current configuration. This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. E.g: only show `ExtendedExampleModel`-options if property `model_type` in `MainOptions` is set to `"ExtendedExampleModel"`. <br>
-
-Configurations can be saved and loaded, a file-explorer view for the current workspace is made available.:
-<p align="center">
-	<!-- <img src="./configurun/examples/images/file_explorer_example.png" width="400" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/file_explorer_example.png" width="400" />
-</p>
-
-## Run Queue
-The run-queue window manages the currently running items. This could either be locally when using a [local-app](#local-app), or remotely, when using a [client-app](#client-side) and a [server-instance](#server-side) on which the actual Run-Queue is running. The Run-Queue allows us to add/remove items, pause/resume items, change the queue-order of items, and start autoprocessing, which will automatically start the next item in the queue when the current item is finished. We can set the number of processors as well, to run multiple items in parallel.
-<p align="center">
-	<!-- <img src="./configurun/examples/images/run_queue_example.png" width="1100" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/run_queue_example.png" width="1100" />
-</p>
-
-Configurations are passed to the user-provided [run-function](#run-function) in separate processes. The stdout/stderr of each of the items is captured and displayed as a selectable console-output-view in the command-line-output window:
-<p align="center">
-	<!-- <img src="./configurun/examples/images/command_line_output_example.png" width="1100" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/command_line_output_example.png" width="1100" />
-</p>
-
-## Remote-processing
-Instead of using the [local-app](#local-app) to manage and run the configurations on your own machine, we can use the [client-app](#client-side) to connect to a [server-instance](#server-side) on a remote machine. The client-app works analogous to the local-app and allows us to create and manage new configuration, but the Run-Queue runs on the connected remote Configurun-server:
-<p align="center">
-	<!-- <img src="./configurun/examples/images/network_login_example.png" width="300" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/network_login_example.png" width="300" />
-</p>
-
-
-# Installation
-This package can downloaded from [this repository](https://github.com/Woutah/configurun), or can be installed directly from PyPi by using pip:
-```bash
-pip install configurun
-```
-
-# How to run?
-Creating the app is done via the `configurun.create`-module. We can create 3 different types of apps:
-- [**Local app**](#local-app) - For running everything locally on your machine
-- [**Client app**](#client-side) - For running the configurations on a remote machine, connects to a `server`-instance
-- [**Server instance**](#server-side) - Command-line instance that listens to connections from `client`-apps. If login is succesful, accepts control of the `RunQueue` from the `client`-app.
-
-On the client-side, the `options_source` should be set - the template of the settings used to create the [configuration-editor](#configuration-editor).<br>
-On the server/running-machine, the `target_function` should be set - the function that actually runs the task/experiment ([example](#run-function)).<br>
-
-## Local App
-A local app is an all-in-one app that can be used to create and run configurations locally on your machine.
-To run the example app, we can either call `run_example_app()` from `configurun.examples` or run the following code to construct the app ourselves:
-```python
-### This example will run the app with an example configuration
-# Also see `configurun/examples/example_target_function.py`
-# Also see `configurun/examples/example_deduce_new_option_class_types.py`
-import os
-from configurun.create import local_app
-from configurun.examples import example_target_function, example_deduce_new_option_classes
-
-if __name__ == "__main__": #Makes sure bootstrapping process is done when running app
-	local_app( #Create and runs a local configurun app-instance
-		target_function=example_target_function, #The function that will be called with the configuration
-		options_source=example_deduce_new_option_classes, #Template for UI-optiosn: Callable/@datclass/ArgumentParser
-		workspace_path = os.path.join( #Settings, configs and the Run-Queue will be saved/loaded from/to here
-			os.getcwd(), 
-			"LocalExampleWorkspace"
-		) 
-	)
-```
-In this example, [`example_target_function`]([./configurun/examples/example_target_function.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_target_function.py)) runs a dummy task that logs to a file for 20 seconds. We can [specify our own run-function](#run-function) to run our own scripts.
-
-We can [specify our own options source](#option-source) to create our own options-class for the configuration-editor, for example by [using an existing `ArgumentParser`-object.](#custom-options-argumentparser)
-## Client App
-We can create a client-app and use it to login to running [server](#server-instance)-instances. We can then use the client-app analogous to the [local-app](#local-app) to create new confiugrations and add/run/manage configurations on the remote machine.<br>
-
-```python
-# Opens a client-side app that we can use to connect to and control
-# the server-instance
-import os
-from configurun.create import client
-from configurun.examples import example_deduce_new_option_classes
-
-if __name__ == "__main__":
-	client(
-		options_source=example_deduce_new_option_classes,
-		workspace_path=os.path.join(os.getcwd(), "ClientExampleWorkspace"),
-	)
-```
-
-
-## Server-instance
-The server-instance is a command-line app that listens to connections from [`client`](#client-app)-instance(s) to receive new configurations and commands to manage its RunQueue. The actual run-functions are ran on this machine. <br>
-
-**NOTE:** *after* authentication, `pickle`/`dill` is used to transmit data, which indirectly enables arbitrary code execution on the server-side if the password is known. Please run the server on trusted network environments only. Run at your own risk!
-```python 
-# Opens a server-instance which tries to connect with clients and allows
-# them to add configurations to the queue to be run on this machine
-import os
-from configurun.create import server
-from configurun.examples.example_target_function import example_target_function
-
-if __name__ == "__main__":
-	# WARNING:
-	# THIS ALLOWS OTHER MACHINES THAT RESIDE ON THE SAME NETWORK
-	# TO EXECUTE ARBITRARY CODE ON THIS MACHINE IF THEY KNOW THE 
-	# PASSWORD. PLEASE RUN IN A TRUSTED NETWORK ENVIRONMENT ONLY
-	# RUN AT YOUR OWN RISK!
-	server(
-		target_function=example_target_function,
-		workspace_path=os.path.join(os.getcwd(), "ServerExampleWorkspace"),
-		password="password", #Password to connect to the server, make sure to change this!
-		port=5454 #Port to connect to the server, defaults to 5454
-	)
-```
-
-
-# Option-source
-When creating an app using the `create`-module, we can define a custom source, using the `options_source=...`, so we can construct the UI using our own options. 
-We can use the following types as an options-source:
-- [`@dataclass`-object](#custom-options-dataclass)
-- [`ArgumentParser`-object](#custom-options-argumentparser)
-- [`Callable`](#custom-options-callable)
-
-## Custom Options (`@dataclass`)
-**NOTE:** Using fields results in more control over the final UI, for a more thorough example, please see [this section](#option-metadata) and/or the example implementations in [configurun/examples/example_options/example_options.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
-
-**NOTE:**  When implementing custom option-classes, don't forget to add the `@dataclass`-decorator, and always inherit from `BaseOptions`
-```python
-import os
-from dataclasses import dataclass
-from configurun.configuration.base_options import BaseOptions
-from configurun.create import local_app
-from configurun.examples import example_target_function
-
-
-@dataclass #Don't forget to add this(!) - otherwise the app will not recognize the fields
-class MyCustomOptions(BaseOptions): #Always inherit from BaseOptions (required to run config)
-	simple_int : int = 1
-	# etc...
-
-if __name__ == "__main__":
-	local_app(
-		target_function=example_target_function,
-		options_source=MyCustomOptions, #Simple: each configuration consists of a single options-class
-		workspace_path = os.path.join(os.getcwd(), "ExampleDataclassOptions")
-	)
-
-```
-
-## Custom Options (`ArgumentParser`)
-We can use a `ArgumentParser`-object as an options source, this will internally convert the argument parser into a `@dataclass`-object, which is then used as an options-class. Certain arguments are also parsed to control the UI (e.g. `required=True`, `help="Will be displayed on hover"`).
-```python
-import argparse
-import os
-from configurun.create import local_app
-from configurun.examples import example_target_function
-
-parser = argparse.ArgumentParser()
-parser.add_argument("--required_arg", type=str, required=True, help="Required argument help")
-#... add more arguments here
-
-if __name__ == "__main__":
-	local_app(
-		target_function=example_target_function,
-		options_source=parser, #Parser is converted internally to a dataclass-class which is used as the options-class
-		workspace_path = os.path.join(os.getcwd(), "ExampleArgparseOptions")
-	)
-```
-## Custom Options (`Callable`)
-A configuration is a collection of option-instances, which are grouped toghether in a `Configuration`-wrapper, which enables us to access the attributes of all enclosed options-instances using the `configuration[attribute]`/`configuration.<attribute>`/`option_class.get(attribute, default)`. For more information, see [this section](#configuration).
-
-We define an `option`-class as a class that has the `@decorator` and inherits from the `BaseOptions`-class.
-
-As an options-source, we can create a callable which takes the current Configuration-instance as an argument and returns 1 or more new options-classes (***not** instances*) which is called every time a setting is changed. If the types-change, the UI will be updated to reflect the new templates. 
-This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. For example:
-```python
-#In this example, we will create a callable which returns new options-classes based on the 
-# current configuration
-import os
-import typing
-from dataclasses import dataclass
-from configurun.create import local_app
-from configurun.examples import example_target_function
-from configurun.configuration import BaseOptions, Configuration
-
-@dataclass #NOTE: Always use @dataclass for options
-class AlwaysTheSame(BaseOptions): #NOTE: Always use BaseOptions as base class for options
-	base_int : int = 1
-	#...
-
-@dataclass
-class CustomOptionsDefault(BaseOptions):
-	simple_int : int = 1
-	#...
-
-@dataclass
-class CustomOptionsUnderConditions(BaseOptions):
-	simple_int : int = 2
-	some_more_options : str = 'Some string'
-	#...
-
-def deduce_new_option_classes(configuration: Configuration)\
-		-> typing.Dict[str, typing.Type[BaseOptions | None]]: #Always return a dict of option 
-	 		# classes the key of the dict is the name/group of the option-class
-			# the value is the option-class (@dataclass & BaseOptions) itself 
-	if configuration.options is None or len(configuration.options) == 0:
-		pass #If initial configuration is being retrieved -> return default dict
-	elif configuration.base_int == 2 and configuration.simple_int != 1:
-		#Only return the CustomOptionsUnderConditions-class when base_int == 2 & simple_int != 1
-		#NOTE: if we're not sure if attributes exist, we can use the `.get(key, default)` method
-		return { #UI will be built using the following option-classes, each key gets a tab/window:
-			'always_the_same' : AlwaysTheSame,
-			'custom_options' : CustomOptionsUnderConditions
-		}
-	
-	return { #UI will be built using the following option-classes, each key gets a tab/window:
-		'always_the_same' : AlwaysTheSame,
-		'custom_options' : CustomOptionsDefault
-	} #NOTE: we must ALWAYS return a dictionary with at least 1 option class
-
-if __name__ == '__main__':
-	local_app(
-		target_function=example_target_function,
-		options_source=deduce_new_option_classes,
-		workspace_path = os.path.join(os.getcwd(), "ExampleCallableOptions")
-	)
-
-```
-
-
-
-# Target Function
-The target function is the function that does all the work. This is the function that is being called when an item starts "running" in the Run-Queue.
-It takes a single argument: a [`Configuration`-instance](#configuration) - instance.
-The configuration-object contains all settings as set by the user when "add to queue" was pressed.
-
-This example uses the example-configuration from [the Configurtion section](#configuration), we simply print the values of the configuration to the console:
-```python
-def target_function(configuration: Configuration):
-	#Do something with the configuration
-	print(configuration.simple_int)
-	print(configuration.some_other_int)
-	#etc.
-```
-
-If you have replaced an `argparse.Argumentparser` in the previous example, this is the place where you insert the user-provided settings to the script that uses the `ArgumentParser`-object. For example:
-```python
-# parsed_args = parser.parse_args() #will be done by user in UI
-# your_framework_that_used_parsed_args(parsed_args) #Will be called in target_function
-
-def target_function(configurtion : Configuration):
-	# Since we can use the Configuration-instance as a dict 
-	# and as configuration.<attribute> we can just
-	# pass it to the framework compatible with the ArgumentParser:
-	your_framework_that_used_parsed_args(configuration)
-
-```
-
-# Configuration
-Configurun works with `configuration`-objects. A configuration is a collection of option-instances (=`@dataclass`-instances that inherit from `BaseOptions`), which are grouped toghether in a `Configuration`-wrapper.
-We can think of the option-instances as the different groups of options we want to edit and use in our run (e.g. `GeneralOptions()`, `LogOptions()`, `ModelOptions()`, etc.).
-In the simplest case, we have 1 single option-instance which contains all the options, `AllOptions()`. 
-
-The `Configuration`-wrapper enables us to access the attributes of all enclosed options-instances using `configuration[attribute]`/`configuration.<attribute>`/`option_class.get(attribute, default)`.
-
-An example of how to use a `Configuration`-instance:
-
-``` python
-from dataclasses import dataclass
-from configurun.configuration import Configuration
-from configurun.configuration import BaseOptions
-
-@dataclass
-class GeneralOptionsClass(BaseOptions):
-	simple_int : int = 1
-	#etc.
-
-@dataclass
-class OtherOptionClass(BaseOptions):
-	some_other_int : int = 2
-	#etc.
-
-
-config = Configuration()
-config.options['general_options'] = GeneralOptionsClass()
-config.options['other_options'] = OtherOptionClass()
-
-#Accessing the options, all of the following are equivalent:
-print(config['simple_int'])
-print(config.simple_int)
-print(config.get('simple_int', -1)))
-
-#These are also equivalent:
-print(config['some_other_int'])
-print(config.some_other_int)
-print(config.get('some_other_int', -1)))
-
-# Note that we can use the config.<attr>-notation to our advantage
-# when we want to use autocomplete in our editor. For example:
-# def target_function(configuration: GeneralOptionsClass)
-# Would result in our editor of choice recognizing/autocompleting
-# the `configuration.simple_hint` way of accessing `simple_hint`
-```
-
-
-
-# Option metadata
-The UI is mainly built around the [`field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.field) functionality of python-`dataclass`, which allows the display-model to make use of the default values, type hints and other information. 
-For each attribute in our `option`-definition, we can provide additional information in the `metadata` attribute of `field()`. This provides additional information to the UI, which is used to determine the editor-type, constraints etc. <br>
-
-For example:
-```python
-from configurun.configuration import base_options
-from dataclasses import field, dataclass
-#Used to constrain the editors: (can also be imported from sklearn)
-from pyside6_utils.utility.constraints import Interval 
-
-@dataclass
-class TestOptions(BaseOptions):
-	test_int_property : int | None = field(
-		default=None, #The default value used in the UI
-		metadata=dict( #Contains additional information for the UI
-			display_name="Test property", #The display-name
-			help="This is a test property that can also be none", #On-hover help-messagem
-			required=True, #If required, the field is red if not filled in
-			constraints = [ #Limit editors (min/max, options, etc.)
-				#The following constrains the editor to have value > 1
-				Interval(type=int, left=1, right=None, closed="both"), 
-				None #Or value can be None
-			] 
-			# etc...
-		)
-)
-```
-For more examples, please see the [example-options](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py). 
-
-The following metadata-keys are supported:
-
-| Metadata Key | Type | Description |
-| --- | --- | --- |
-| `"display_name"` | `str` | Name to display for this attribute in the view - defaults to the variable name itself |
-| `"display_path"` | `str` | Path to display this attribute - we can group/structure items. If parent does not exist, creates folders. Format as "|
-| `"help"` | `str` | Help-message which will be shown when the user hovers over this item - empty by default|
-| `"constraints"` | `List[constraint]` | Additional constraints on which the editor will be determined to apply to the field**, if none provided, use typehint of the field|
-| `"required"` | `bool` | Whether this field is required to be filled in - if true - a red background will appear if the value is not set|
-| `"editable"` | `bool` | Whether this field is editable - if false - the editor will be disabled|
-
-**: Constraints are sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into the [pyside6-utils](https://github.com/Woutah/pyside6-utils) package under [`utility.constraints`](https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/utility/constraints.py). The following constraints are supported:
-| Constraint | Description | Editor Type
-| --- | --- | --- |
-| `type` | The type of the value should match the type of the constraint | based on type |
-| `Options` / `Container` | The value should be one of the options provided in the constraint | `QComboBox` |
-| `StrOptions` | The value should be one of the str-options provided in the constraint | `QComboBox` |
-| `Interval` | The value should be within the interval provided in the constraint | `QSpinBox` or `QDoubleSpinBox` (limited) |
-| `None` | `None` is a valid value for this field (same as `typing.Optional`) | Adds reset-button to editor |
-| `Range` | The value should be within the range provided in the constraint | `QSpinBox` (limited) |
-
+# Configurun
+
+Configurun is a cross-platform PySide6-based package that implements an application for managing, creating and (remotely) running python configurations.
+It was designed mainly with machine-learning tasks in mind, but can be used for any python script that takes arguments as an input. The editor-UI is created automatically using either an `argparse.Argumentparser` or python-`@dataclass`(es).
+
+The Configurun-app is especially useful for scripts/experiments that require a lot of arguments to be tweaked across many experiment-runs. It also makes the process of running experiments remotely much easier by enabling the user to edit, add and schedule tasks on any running Configurun server-instance reachable via a network connection.
+
+This package was created in tandem with [pyside6-utils](https://github.com/Woutah/pyside6-utils/).
+
+<p align="center">
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/main_window_example.png" width="1200" />
+</p>
+
+# Table of contents
+
+- [Configurun](#configurun)
+- [Table of contents](#table-of-contents)
+- [Features](#features)
+	- [Configuration Editor](#configuration-editor)
+	- [Run Queue](#run-queue)
+	- [Remote-processing](#remote-processing)
+- [Installation](#installation)
+- [How to run?](#how-to-run)
+	- [Local App](#local-app)
+	- [Client App](#client-app)
+	- [Server-instance](#server-instance)
+- [Option-source](#option-source)
+	- [Custom Options (`@dataclass`)](#custom-options-dataclass)
+	- [Custom Options (`ArgumentParser`)](#custom-options-argumentparser)
+	- [Custom Options (`Callable`)](#custom-options-callable)
+- [Target Function](#target-function)
+- [Configuration](#configuration)
+- [Option metadata](#option-metadata)
+- [SSH-tunneling](#ssh-tunneling)
+	- [No-hop](#no-hop)
+	- [Hopping](#hopping)
+
+# Features
+
+## Configuration Editor
+
+The configuration editor allows the user to specify a configuration-template using either (groups of) [`@dataclass`-class](#custom-options-dataclass) or an [`ArgumentParser`-instance](#custom-options-dataclass). The editor will then automatically create a UI based on the provided template. Editors are specifically created for each option-property based on provided template-types (and [extra constraints](#option-metadata)). 
+Help-messages are displayed on hover, required arguments are highlighted when not filled in, etc.
+<p align="center">
+	<!-- <img src="./configurun/examples/images/configuration_editor_example.png" width="600" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/configuration_editor_example.png" width="600" />
+</p>
+
+More complex typehints using `List` / `Union` / `Literal` are supported and are automatically built into widgets that allow the user to add/remove items and switch input-types:
+
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./configurun/examples/images/string_float_list_example.png" width=300/> -->
+</p>
+
+We can also define our own [option-source-method](#custom-options-callable) to dynamically create new option-groups based on the current configuration. This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. E.g: only show `ExtendedExampleModel`-options if property `model_type` in `MainOptions` is set to `"ExtendedExampleModel"`. <br>
+
+Configurations can be saved and loaded, a file-explorer view for the current workspace is made available.:
+<p align="center">
+	<!-- <img src="./configurun/examples/images/file_explorer_example.png" width="400" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/file_explorer_example.png" width="400" />
+</p>
+
+## Run Queue
+
+The run-queue window manages the currently running items. This could either be locally when using a [local-app](#local-app), or remotely, when using a [client-app](#client-app) and a [server-instance](#server-instance) on which the actual Run-Queue is running. The Run-Queue allows us to add/remove items, pause/resume items, change the queue-order of items, and start autoprocessing, which will automatically start the next item in the queue when the current item is finished. We can set the number of processors as well, to run multiple items in parallel.
+<p align="center">
+	<!-- <img src="./configurun/examples/images/run_queue_example.png" width="1100" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/run_queue_example.png" width="1100" />
+</p>
+
+Configurations are passed to the user-provided [target-function](#target-function) in separate processes. The stdout/stderr of each of the items is captured and displayed as a selectable console-output-view in the command-line-output window:
+<p align="center">
+	<!-- <img src="./configurun/examples/images/command_line_output_example.png" width="1100" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/command_line_output_example.png" width="1100" />
+</p>
+
+## Remote-processing
+
+Instead of using the [local-app](#local-app) to manage and run the configurations on your own machine, we can use the [client-app](#client-app) to connect to a [server-instance](#server-instance) on a remote machine. The client-app works analogous to the local-app and allows us to create and manage new configuration, but the Run-Queue runs on the connected remote Configurun-server:
+<p align="center">
+	<!-- <img src="./configurun/examples/images/network_login_example.png" width="300" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/network_login_example.png" width="300" />
+</p>
+
+# Installation
+
+This package can downloaded from [this repository](https://github.com/Woutah/configurun), or can be installed directly from PyPi by using pip:
+
+``` bash
+pip install configurun
+```
+
+# How to run?
+
+Creating the app is done via the `configurun.create`-module. We can create 3 different types of apps:
+
+- [**Local app**](#local-app) - For running everything locally on your machine
+- [**Client app**](#client-app) - For running the configurations on a remote machine, connects to a `server`-instance
+- [**Server instance**](#server-instance) - Command-line instance that listens to connections from `client`-apps. If login is succesful, accepts control of the `RunQueue` from the `client`-app.
+
+On the client-side, the `options_source` should be set - the template of the settings used to create the [configuration-editor](#configuration-editor).<br>
+On the server/running-machine, the `target_function` should be set - the function that actually runs the task/experiment ([example](#target-function)).<br>
+
+## Local App
+
+A local app is an all-in-one app that can be used to create and run configurations locally on your machine.
+To run the example app, we can either call `run_example_app()` from `configurun.examples` or run the following code to construct the app ourselves:
+
+```python
+### This example will run the app with an example configuration
+# Also see `configurun/examples/example_target_function.py`
+# Also see `configurun/examples/example_deduce_new_option_class_types.py`
+import os
+from configurun.app import run_local
+from configurun.examples import example_target_function, example_deduce_new_option_classes
+
+if __name__ == "__main__": #Makes sure bootstrapping process is done when running app
+	run_local( #Create and runs a local configurun app-instance
+		target_function=example_target_function, #The function that will be called with the configuration
+		options_source=example_deduce_new_option_classes, #Template for UI-optiosn: Callable/@datclass/ArgumentParser
+		workspace_path = os.path.join( #Settings, configs and the Run-Queue will be saved/loaded from/to here
+			os.getcwd(),
+			"LocalExampleWorkspace"
+		)
+	)
+```
+
+In this example, [`example_target_function`](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_target_function.py) runs a dummy task that logs to a file for 20 seconds. We can [specify our own target-function](#target-function) to run our own scripts.
+
+We can [specify our own options source](#option-source) to create our own options-class for the configuration-editor, for example by [using an existing `ArgumentParser`-object.](#custom-options-argumentparser)
+
+## Client App
+
+We can create a client-app and use it to login to running [server](#server-instance)-instances. We can then use the client-app analogous to the [local-app](#local-app) to create new confiugrations and add/run/manage configurations on the remote machine.<br>
+
+```python
+# Opens a client-side app that we can use to connect to and control
+# the server-instance
+import os
+from configurun.app import run_client
+from configurun.examples import example_deduce_new_option_classes
+
+if __name__ == "__main__":
+	run_client(
+		options_source=example_deduce_new_option_classes,
+		workspace_path=os.path.join(os.getcwd(), "ClientExampleWorkspace"),
+	)
+```
+
+## Server-instance
+
+The server-instance is a command-line app that listens to connections from [`client`](#client-app)-instance(s) to receive new configurations and commands to manage its RunQueue. The actual target-functions are ran on this machine. <br>
+
+**NOTE:** *after* authentication, `pickle`/`dill` is used to transmit data, which indirectly enables arbitrary code execution on the server-side if the password is known. Please run the server on trusted network environments only. Run at your own risk!
+
+```python
+# Opens a server-instance which tries to connect with clients and allows
+# them to add configurations to the queue to be run on this machine
+import os
+from configurun.server import run_server
+from configurun.examples.example_target_function import example_target_function
+
+if __name__ == "__main__":
+	# WARNING:
+	# THIS ALLOWS OTHER MACHINES THAT RESIDE ON THE SAME NETWORK
+	# TO EXECUTE ARBITRARY CODE ON THIS MACHINE IF THEY KNOW THE
+	# PASSWORD. PLEASE RUN IN A TRUSTED NETWORK ENVIRONMENT ONLY
+	# RUN AT YOUR OWN RISK!
+	run_server(
+		target_function=example_target_function,
+		workspace_path=os.path.join(os.getcwd(), "ServerExampleWorkspace"),
+		password="password", #Password to connect to the server, make sure to change this!
+		port=5454 #Port to connect to the server, defaults to 5454
+	)
+```
+
+# Option-source
+
+When creating an app using the `create`-module, we can define a custom source, using the `options_source=...`, so we can construct the UI using our own options.
+We can use the following types as an options-source:
+
+- [`@dataclass`-object](#custom-options-dataclass)
+- [`ArgumentParser`-object](#custom-options-argumentparser)
+- [`Callable`](#custom-options-callable)
+
+## Custom Options (`@dataclass`)
+
+**NOTE:** Using `@dataclass`-fields results in more control over the final UI, for a more thorough example, please see [this section](#option-metadata) and/or the example implementations in [configurun/examples/example_options/example_options.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
+
+**NOTE:**  When implementing custom option-classes, don't forget to add the `@dataclass`-decorator, and always inherit from `BaseOptions`
+
+UI-supported type-hints include `str`, `int`, `float`, `datatime`, `typing.Literal`  (and more) and combinations using `typing.List`, `typing.Union` / `|`. For example:
+
+```python
+import os
+import typing
+from dataclasses import dataclass
+from configurun.configuration.base_options import BaseOptions
+from configurun.app import run_local
+from configurun.examples import example_target_function
+
+
+@dataclass #Don't forget to add this(!) - otherwise the app will not recognize the fields
+class MyCustomOptions(BaseOptions): #Always inherit from BaseOptions (required to run config)
+	simple_int : int = 1
+	complex_property : typing.List[typing.Union[int, str]] | None = None # Union = |-notation
+	# etc...
+
+if __name__ == "__main__":
+	run_local(
+		target_function=example_target_function,
+		options_source=MyCustomOptions, #Simple: each configuration consists of a single options-class
+		workspace_path = os.path.join(os.getcwd(), "ExampleDataclassOptions")
+	)
+
+
+```
+
+## Custom Options (`ArgumentParser`)
+
+We can use a `ArgumentParser`-object as an options source, this will internally convert the argument parser into a `@dataclass`-object, which is then used as an options-class. Whenever possible, arguments are also parsed to the UI (e.g. `required=True`, `help="Will be displayed on hover"` etc.).
+
+```python
+import argparse
+import os
+from configurun.app import run_local
+from configurun.examples import example_target_function
+
+parser = argparse.ArgumentParser()
+parser.add_argument("--required_arg", type=str, required=True, help="Required argument help")
+#... add more arguments here
+
+if __name__ == "__main__":
+	run_local(
+		target_function=example_target_function,
+		options_source=parser, #Parser is converted internally to a dataclass-class which is used as the options-class
+		workspace_path = os.path.join(os.getcwd(), "ExampleArgparseOptions")
+	)
+```
+
+## Custom Options (`Callable`)
+We define an `option`-class as a class that has the `@decorator` and inherits from the `BaseOptions`-class.
+
+A configuration is a collection of option-instances, which are grouped toghether in a [`Configuration()`](#configuration)-wrapper, which enables us to access the attributes of all enclosed options-instances using the `configuration[attribute]` / `configuration.<attribute>` / `option_class.get(attribute, default)`. For more information, see [this section](#configuration).
+
+As an options-source, we can create a callable which takes the current Configuration-instance as an argument and returns 1 or more new options-classes (***not** instances*) which is called every time a setting is changed. If the types-change, the UI will be updated to reflect the new templates.
+This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. For example:
+
+```python
+#In this example, we will create a callable which returns new options-classes based on the
+# current configuration
+import os
+import typing
+from dataclasses import dataclass
+from configurun.app import run_local
+from configurun.examples import example_target_function
+from configurun.configuration import BaseOptions, Configuration
+
+@dataclass #NOTE: Always use @dataclass for options
+class AlwaysTheSame(BaseOptions): #NOTE: Always use BaseOptions as base class for options
+	base_int : int = 1
+	#...
+
+@dataclass
+class CustomOptionsDefault(BaseOptions):
+	simple_int : int = 1
+	#...
+
+@dataclass
+class CustomOptionsUnderConditions(BaseOptions):
+	simple_int : int = 2
+	some_more_options : str = 'Some string'
+	#...
+
+def deduce_new_option_classes(configuration: Configuration)\
+		-> typing.Dict[str, typing.Type[BaseOptions | None]]: #Always return a dict of option
+	 		# classes the key of the dict is the name/group of the option-class
+			# the value is the option-class (@dataclass & BaseOptions) itself
+	if configuration.options is None or len(configuration.options) == 0:
+		pass #If initial configuration is being retrieved -> return default dict
+	elif configuration.base_int == 2 and configuration.simple_int != 1:
+		#Only return the CustomOptionsUnderConditions-class when base_int == 2 & simple_int != 1
+		#NOTE: if we're not sure if attributes exist, we can use the `.get(key, default)` method
+		return { #UI will be built using the following option-classes, each key gets a tab/window:
+			'always_the_same' : AlwaysTheSame,
+			'custom_options' : CustomOptionsUnderConditions
+		}
+
+	return { #UI will be built using the following option-classes, each key gets a tab/window:
+		'always_the_same' : AlwaysTheSame,
+		'custom_options' : CustomOptionsDefault
+	} #NOTE: we must ALWAYS return a dictionary with at least 1 option class
+
+if __name__ == '__main__':
+	run_local(
+		target_function=example_target_function,
+		options_source=deduce_new_option_classes,
+		workspace_path = os.path.join(os.getcwd(), "ExampleCallableOptions")
+	)
+
+```
+
+# Target Function
+
+The target function is the function that does all the work. This is the function that is being called when an item starts "running" in the Run-Queue.
+It takes a single argument: a [`Configuration`-instance](#configuration).
+The configuration-object contains all settings as set by the user when "add to queue" was pressed. 
+
+This example uses the example-configuration from [the Configuration section](#configuration), we simply print the values of the configuration to the console:
+
+```python
+def target_function(configuration: Configuration):
+	#Do something with the configuration
+	print(configuration.simple_int)
+	print(configuration.some_other_int)
+	#etc.
+```
+
+If you have replaced an `argparse.Argumentparser`, this is the place where you insert the user-provided settings to the script that uses the `ArgumentParser`-object. For example:
+
+```python
+# parsed_args = parser.parse_args() #will be done by user in UI
+# your_framework_that_used_parsed_args(parsed_args) #Will be called in target_function
+
+def target_function(configurtion : Configuration):
+	# Since we can use the Configuration-instance as a dict
+	# and as configuration.<attribute> we can just
+	# pass it to the framework compatible with the ArgumentParser:
+	your_framework_that_used_parsed_args(configuration)
+```
+
+Of course you can also directly pass the `your_framework_that_used_parsed_args(...)`-function as the target function when creating the app:
+
+```python
+if __name__ == '__main__':
+	local_app(
+		target_function=your_framework_that_used_parsed_args,
+		options_source=deduce_new_option_classes,
+		workspace_path = os.path.join(os.getcwd(), "ExampleCallableOptions")
+	)
+```
+
+This example uses the `deduce_new_option_classes`-function from [callable option source example](#custom-options-callable) .
+
+# Configuration
+
+Configurun works with `configuration`-objects. A configuration is a collection of option-instances (=`@dataclass`-instances that inherit from `BaseOptions`), which are grouped toghether in a `Configuration`-wrapper.
+We can think of the option-instances as the different groups of options we want to edit and use in our run (e.g. `GeneralOptions()`, `LogOptions()`, `ModelOptions()`, etc.).
+In the simplest case, we have 1 single option-instance which contains all the options, for example: `AllOptions()`.
+
+The `Configuration`-wrapper enables us to access the attributes of all enclosed options-instances using `configuration[attribute]`/`configuration.<attribute>`/`option_class.get(attribute, default)`.
+
+An example of how to use a `Configuration`-instance:
+
+``` python
+from dataclasses import dataclass
+from configurun.configuration import Configuration
+from configurun.configuration import BaseOptions
+
+@dataclass
+class GeneralOptionsClass(BaseOptions):
+	simple_int : int = 1
+	#etc.
+
+@dataclass
+class OtherOptionClass(BaseOptions):
+	some_other_int : int = 2
+	#etc.
+
+
+# Normally, the following would be done by the app using the UI
+# input and/or the user-provided option-source
+config = Configuration()
+config.options['general_options'] = GeneralOptionsClass()
+config.options['other_options'] = OtherOptionClass()
+
+#Accessing the options, all of the following are equivalent:
+print(config['simple_int'])
+print(config.simple_int)
+print(config.get('simple_int', -1))) #Would return -1 if key-error occurs
+
+#These are also equivalent:
+print(config['some_other_int'])
+print(config.some_other_int)
+print(config.get('some_other_int', -1)))
+
+# Note that we can use the config.<attr>-notation to our advantage
+# when we want to use autocomplete in our editor. For example:
+# def target_function(configuration: GeneralOptionsClass)
+# Would result in our editor of choice recognizing/autocompleting
+# the `configuration.simple_hint` way of accessing `simple_hint`
+```
+
+# Option metadata
+
+The UI is mainly built around the [`field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.field) functionality of python-`dataclass`, which allows the display-model to make use of the default values, type hints and other information.
+While typehints (e.g. `int`, `str`, `typing.List[int]`, etc.) are enough to create the editors, we can also provide additional information in the `metadata`-attribute of `field()` to further constrain the editors and provide additional information to the user. <br>
+
+For example:
+
+```python
+from configurun.configuration import base_options
+from dataclasses import field, dataclass
+#Used to constrain the editors: (can also be imported from sklearn)
+from pyside6_utils.classes.constraints import Interval, ConstrainedList
+
+@dataclass
+class TestOptions(BaseOptions):
+	test_int_list_property : typing.List[int] | None = field(
+		default=None, #The default value used in the UI
+		metadata=dict( #Contains additional information for the UI
+			display_name="Test property", #The display-name
+			help="This is a test property that can also be none", #On-hover help-messagem
+			required=True, #If required, the field is red if not filled in
+			constraints = [ #Limit editors (min/max, options, etc.)
+				#The following constrains the editor to have value > 1
+				ConstrainedList([Interval(type=int, left=1, right=None, closed="both")]),
+				None #Or value can be None
+			]
+			# etc...
+		)
+)
+```
+
+For more examples, please see the [example-options](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
+
+The following metadata-keys are supported:
+
+| Metadata Key | Type | Description |
+| --- | --- | --- |
+| `"display_name"` | `str` | Name to display for this attribute in the view - defaults to the variable name itself |
+| `"display_path"` | `str` | Path to display this attribute - we can group/structure items when using a treeview - defaults to no parents|
+| `"help"` | `str` | Help-message which will be shown when the user hovers over this item - empty by default|
+| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [*](#constraintnote) , if none provided, use typehint of the field|
+| `"required"` | `bool` | Whether this field is required to be filled in - if true - a red background will appear if the value is not set|
+| `"editable"` | `bool` | Whether this field is editable - if false - the editor will be disabled|
+
+<a name="constraintnote">*=</a>Constraints are (almost entirely) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `classes.constraints`. The following constraints are supported:
+| Constraint | Description | Editor Type
+| --- | --- | --- |
+| `type` | The type of the value should match the type of the constraint | based on type |
+| `Options` / `Container` | The value should be one of the options provided in the constraint | `QComboBox` |
+| `StrOptions` | The value should be one of the str-options provided in the constraint | `QComboBox` |
+| `Interval` | The value should be within the interval provided in the constraint | `QSpinBox` or `QDoubleSpinBox` (limited) |
+| `None` | `None` is a valid value for this field, same as `typing.Optional` | Adds reset-button to editor |
+| `Range` | The value should be within the range provided in the constraint | `QSpinBox` (limited) |
+| `ConstrainedList` | [*(Custom - not part of Sklearn)](#constrainedlist) Indicates a list of of values of a constrained type | Based on type of list |
+
+<a name="constrainedlist">*=</a>For example, `ConstrainedList([Interval(float, 0.0, 1.0), StrOptions(["string1", "string2"])])` indicates a list of values that should either be a float between 0.0 and 1.0, or the string "string1" or "string2". The editor for this field would be constructed as a `WidgetList` to which the user can add `WidgetSwitcher`. The `WidgetSwitcher` would then have two widgets, one with a `QSpinBox` and one with a `QComboBox` as the editor. **NOTE:** the same editor would be parsed from a `Typing.List[typing.Union[float, Typing.Literal["string1", "string2"]]]` typehint, minus the bounded-interval constraint on the float:
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/string_float_list_example.png" width=300/> -->
+</p>
+
+# SSH-tunneling
+
+This section contains a quick tutorial on how to use SSH-tunnels to connect to a remote server-instance in case we're not running client and server on the same machine/network.
+
+## No-hop
+
+A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without opening up any ports on the server-side.
+If we can directly SSH into the target machine, we can connect the ports as follows (assuming we're using the default `5454`-port in both the server and client configuration):
+
+```bash
+ssh -L 5454:localhost:5454 user@remote_host
+```
+
+On the client-side, we can then connect to the server-instance by using `localhost:5454` as the host and the password we set in the server-instance.
+
+## Hopping
+
+If we cannot directly access the remote-machine, we can use a 2-step SSH-tunnel to connect to the server-instance.
+This example assumes we have:
+
+- `remote1`: directly accessible from our machine
+- `remote2`: only accessible from `remote1`
+- Using default Configurun-port `5454` on both the client and server-side
+
+We can then connect to `remote2` from our machine using the following command:
+
+```bash
+ssh -L 5454:localhost:61521 <username>@<remote1-ip> ssh -L 61521:localhost:5454 -N <remote2-ip>
+```
+
+This example forwards `localhost:5454`->`remote1:61521`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
```

### Comparing `configurun-0.1.0/README.md` & `configurun-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,396 +1,496 @@
-# Configurun
-Configurun is a cross-platform PySide6-based package that implements an application for managing, creating and (remotely) running python configurations. 
-It was designed mainly with machine-learning tasks in mind, but can be used for any python script that takes arguments as an input. The editor-UI is created automatically using either an `argparse.Argumentparser` or python-`@dataclass`(es).
-
-
-The Configurun-app is especially useful for scripts/experiments that require a lot of arguments to be tweaked across many experiment-runs. It also makes the process of running experiments remotely much easier by enabling the user to edit, add and schedule tasks on any running Configurun server-instance reachable via a network connection.
-
-This package was created in tandem with [pyside6-utils](https://github.com/Woutah/pyside6-utils/).
-
-
-<p align="center">
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/main_window_example.png" width="1200" />
-</p>
-
-# Table of contents
-- [Configurun](#configurun)
-- [Table of contents](#table-of-contents)
-- [Features](#features)
-	- [Configuration Editor](#configuration-editor)
-	- [Run Queue](#run-queue)
-	- [Remote-processing](#remote-processing)
-- [Installation](#installation)
-- [How to run?](#how-to-run)
-	- [Local App](#local-app)
-	- [Client App](#client-app)
-	- [Server-instance](#server-instance)
-- [Option-source](#option-source)
-	- [Custom Options (`@dataclass`)](#custom-options-dataclass)
-	- [Custom Options (`ArgumentParser`)](#custom-options-argumentparser)
-	- [Custom Options (`Callable`)](#custom-options-callable)
-- [Target Function](#target-function)
-- [Configuration](#configuration)
-- [Option metadata](#option-metadata)
-
-
-# Features
-## Configuration Editor
-The configuration editor allows the user to specify a configuration-template using either (groups of) [`@dataclass`-class](#custom-options-dataclass) or an [`ArgumentParser`-instance](#custom-options-dataclass). The editor will then automatically create a UI based on the provided template. Editors are specifically created for each option-property based on provided template-types (and [extra constraints](#option-metadata)). Help-messages are displayed on hover, required arguments are highlighted when not filled in, etc.
-<p align="center">
-	<!-- <img src="./configurun/examples/images/configuration_editor_example.png" width="600" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/configuration_editor_example.png" width="600" />
-</p>
-
-We can also define our own [option-source-method](#custom-options-callable) to dynamically create new option-groups based on the current configuration. This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. E.g: only show `ExtendedExampleModel`-options if property `model_type` in `MainOptions` is set to `"ExtendedExampleModel"`. <br>
-
-Configurations can be saved and loaded, a file-explorer view for the current workspace is made available.:
-<p align="center">
-	<!-- <img src="./configurun/examples/images/file_explorer_example.png" width="400" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/file_explorer_example.png" width="400" />
-</p>
-
-## Run Queue
-The run-queue window manages the currently running items. This could either be locally when using a [local-app](#local-app), or remotely, when using a [client-app](#client-side) and a [server-instance](#server-side) on which the actual Run-Queue is running. The Run-Queue allows us to add/remove items, pause/resume items, change the queue-order of items, and start autoprocessing, which will automatically start the next item in the queue when the current item is finished. We can set the number of processors as well, to run multiple items in parallel.
-<p align="center">
-	<!-- <img src="./configurun/examples/images/run_queue_example.png" width="1100" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/run_queue_example.png" width="1100" />
-</p>
-
-Configurations are passed to the user-provided [run-function](#run-function) in separate processes. The stdout/stderr of each of the items is captured and displayed as a selectable console-output-view in the command-line-output window:
-<p align="center">
-	<!-- <img src="./configurun/examples/images/command_line_output_example.png" width="1100" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/command_line_output_example.png" width="1100" />
-</p>
-
-## Remote-processing
-Instead of using the [local-app](#local-app) to manage and run the configurations on your own machine, we can use the [client-app](#client-side) to connect to a [server-instance](#server-side) on a remote machine. The client-app works analogous to the local-app and allows us to create and manage new configuration, but the Run-Queue runs on the connected remote Configurun-server:
-<p align="center">
-	<!-- <img src="./configurun/examples/images/network_login_example.png" width="300" /> -->
-	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/network_login_example.png" width="300" />
-</p>
-
-
-# Installation
-This package can downloaded from [this repository](https://github.com/Woutah/configurun), or can be installed directly from PyPi by using pip:
-```bash
-pip install configurun
-```
-
-# How to run?
-Creating the app is done via the `configurun.create`-module. We can create 3 different types of apps:
-- [**Local app**](#local-app) - For running everything locally on your machine
-- [**Client app**](#client-side) - For running the configurations on a remote machine, connects to a `server`-instance
-- [**Server instance**](#server-side) - Command-line instance that listens to connections from `client`-apps. If login is succesful, accepts control of the `RunQueue` from the `client`-app.
-
-On the client-side, the `options_source` should be set - the template of the settings used to create the [configuration-editor](#configuration-editor).<br>
-On the server/running-machine, the `target_function` should be set - the function that actually runs the task/experiment ([example](#run-function)).<br>
-
-## Local App
-A local app is an all-in-one app that can be used to create and run configurations locally on your machine.
-To run the example app, we can either call `run_example_app()` from `configurun.examples` or run the following code to construct the app ourselves:
-```python
-### This example will run the app with an example configuration
-# Also see `configurun/examples/example_target_function.py`
-# Also see `configurun/examples/example_deduce_new_option_class_types.py`
-import os
-from configurun.create import local_app
-from configurun.examples import example_target_function, example_deduce_new_option_classes
-
-if __name__ == "__main__": #Makes sure bootstrapping process is done when running app
-	local_app( #Create and runs a local configurun app-instance
-		target_function=example_target_function, #The function that will be called with the configuration
-		options_source=example_deduce_new_option_classes, #Template for UI-optiosn: Callable/@datclass/ArgumentParser
-		workspace_path = os.path.join( #Settings, configs and the Run-Queue will be saved/loaded from/to here
-			os.getcwd(), 
-			"LocalExampleWorkspace"
-		) 
-	)
-```
-In this example, [`example_target_function`]([./configurun/examples/example_target_function.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_target_function.py)) runs a dummy task that logs to a file for 20 seconds. We can [specify our own run-function](#run-function) to run our own scripts.
-
-We can [specify our own options source](#option-source) to create our own options-class for the configuration-editor, for example by [using an existing `ArgumentParser`-object.](#custom-options-argumentparser)
-## Client App
-We can create a client-app and use it to login to running [server](#server-instance)-instances. We can then use the client-app analogous to the [local-app](#local-app) to create new confiugrations and add/run/manage configurations on the remote machine.<br>
-
-```python
-# Opens a client-side app that we can use to connect to and control
-# the server-instance
-import os
-from configurun.create import client
-from configurun.examples import example_deduce_new_option_classes
-
-if __name__ == "__main__":
-	client(
-		options_source=example_deduce_new_option_classes,
-		workspace_path=os.path.join(os.getcwd(), "ClientExampleWorkspace"),
-	)
-```
-
-
-## Server-instance
-The server-instance is a command-line app that listens to connections from [`client`](#client-app)-instance(s) to receive new configurations and commands to manage its RunQueue. The actual run-functions are ran on this machine. <br>
-
-**NOTE:** *after* authentication, `pickle`/`dill` is used to transmit data, which indirectly enables arbitrary code execution on the server-side if the password is known. Please run the server on trusted network environments only. Run at your own risk!
-```python 
-# Opens a server-instance which tries to connect with clients and allows
-# them to add configurations to the queue to be run on this machine
-import os
-from configurun.create import server
-from configurun.examples.example_target_function import example_target_function
-
-if __name__ == "__main__":
-	# WARNING:
-	# THIS ALLOWS OTHER MACHINES THAT RESIDE ON THE SAME NETWORK
-	# TO EXECUTE ARBITRARY CODE ON THIS MACHINE IF THEY KNOW THE 
-	# PASSWORD. PLEASE RUN IN A TRUSTED NETWORK ENVIRONMENT ONLY
-	# RUN AT YOUR OWN RISK!
-	server(
-		target_function=example_target_function,
-		workspace_path=os.path.join(os.getcwd(), "ServerExampleWorkspace"),
-		password="password", #Password to connect to the server, make sure to change this!
-		port=5454 #Port to connect to the server, defaults to 5454
-	)
-```
-
-
-# Option-source
-When creating an app using the `create`-module, we can define a custom source, using the `options_source=...`, so we can construct the UI using our own options. 
-We can use the following types as an options-source:
-- [`@dataclass`-object](#custom-options-dataclass)
-- [`ArgumentParser`-object](#custom-options-argumentparser)
-- [`Callable`](#custom-options-callable)
-
-## Custom Options (`@dataclass`)
-**NOTE:** Using fields results in more control over the final UI, for a more thorough example, please see [this section](#option-metadata) and/or the example implementations in [configurun/examples/example_options/example_options.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
-
-**NOTE:**  When implementing custom option-classes, don't forget to add the `@dataclass`-decorator, and always inherit from `BaseOptions`
-```python
-import os
-from dataclasses import dataclass
-from configurun.configuration.base_options import BaseOptions
-from configurun.create import local_app
-from configurun.examples import example_target_function
-
-
-@dataclass #Don't forget to add this(!) - otherwise the app will not recognize the fields
-class MyCustomOptions(BaseOptions): #Always inherit from BaseOptions (required to run config)
-	simple_int : int = 1
-	# etc...
-
-if __name__ == "__main__":
-	local_app(
-		target_function=example_target_function,
-		options_source=MyCustomOptions, #Simple: each configuration consists of a single options-class
-		workspace_path = os.path.join(os.getcwd(), "ExampleDataclassOptions")
-	)
-
-```
-
-## Custom Options (`ArgumentParser`)
-We can use a `ArgumentParser`-object as an options source, this will internally convert the argument parser into a `@dataclass`-object, which is then used as an options-class. Certain arguments are also parsed to control the UI (e.g. `required=True`, `help="Will be displayed on hover"`).
-```python
-import argparse
-import os
-from configurun.create import local_app
-from configurun.examples import example_target_function
-
-parser = argparse.ArgumentParser()
-parser.add_argument("--required_arg", type=str, required=True, help="Required argument help")
-#... add more arguments here
-
-if __name__ == "__main__":
-	local_app(
-		target_function=example_target_function,
-		options_source=parser, #Parser is converted internally to a dataclass-class which is used as the options-class
-		workspace_path = os.path.join(os.getcwd(), "ExampleArgparseOptions")
-	)
-```
-## Custom Options (`Callable`)
-A configuration is a collection of option-instances, which are grouped toghether in a `Configuration`-wrapper, which enables us to access the attributes of all enclosed options-instances using the `configuration[attribute]`/`configuration.<attribute>`/`option_class.get(attribute, default)`. For more information, see [this section](#configuration).
-
-We define an `option`-class as a class that has the `@decorator` and inherits from the `BaseOptions`-class.
-
-As an options-source, we can create a callable which takes the current Configuration-instance as an argument and returns 1 or more new options-classes (***not** instances*) which is called every time a setting is changed. If the types-change, the UI will be updated to reflect the new templates. 
-This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. For example:
-```python
-#In this example, we will create a callable which returns new options-classes based on the 
-# current configuration
-import os
-import typing
-from dataclasses import dataclass
-from configurun.create import local_app
-from configurun.examples import example_target_function
-from configurun.configuration import BaseOptions, Configuration
-
-@dataclass #NOTE: Always use @dataclass for options
-class AlwaysTheSame(BaseOptions): #NOTE: Always use BaseOptions as base class for options
-	base_int : int = 1
-	#...
-
-@dataclass
-class CustomOptionsDefault(BaseOptions):
-	simple_int : int = 1
-	#...
-
-@dataclass
-class CustomOptionsUnderConditions(BaseOptions):
-	simple_int : int = 2
-	some_more_options : str = 'Some string'
-	#...
-
-def deduce_new_option_classes(configuration: Configuration)\
-		-> typing.Dict[str, typing.Type[BaseOptions | None]]: #Always return a dict of option 
-	 		# classes the key of the dict is the name/group of the option-class
-			# the value is the option-class (@dataclass & BaseOptions) itself 
-	if configuration.options is None or len(configuration.options) == 0:
-		pass #If initial configuration is being retrieved -> return default dict
-	elif configuration.base_int == 2 and configuration.simple_int != 1:
-		#Only return the CustomOptionsUnderConditions-class when base_int == 2 & simple_int != 1
-		#NOTE: if we're not sure if attributes exist, we can use the `.get(key, default)` method
-		return { #UI will be built using the following option-classes, each key gets a tab/window:
-			'always_the_same' : AlwaysTheSame,
-			'custom_options' : CustomOptionsUnderConditions
-		}
-	
-	return { #UI will be built using the following option-classes, each key gets a tab/window:
-		'always_the_same' : AlwaysTheSame,
-		'custom_options' : CustomOptionsDefault
-	} #NOTE: we must ALWAYS return a dictionary with at least 1 option class
-
-if __name__ == '__main__':
-	local_app(
-		target_function=example_target_function,
-		options_source=deduce_new_option_classes,
-		workspace_path = os.path.join(os.getcwd(), "ExampleCallableOptions")
-	)
-
-```
-
-
-
-# Target Function
-The target function is the function that does all the work. This is the function that is being called when an item starts "running" in the Run-Queue.
-It takes a single argument: a [`Configuration`-instance](#configuration) - instance.
-The configuration-object contains all settings as set by the user when "add to queue" was pressed.
-
-This example uses the example-configuration from [the Configurtion section](#configuration), we simply print the values of the configuration to the console:
-```python
-def target_function(configuration: Configuration):
-	#Do something with the configuration
-	print(configuration.simple_int)
-	print(configuration.some_other_int)
-	#etc.
-```
-
-If you have replaced an `argparse.Argumentparser` in the previous example, this is the place where you insert the user-provided settings to the script that uses the `ArgumentParser`-object. For example:
-```python
-# parsed_args = parser.parse_args() #will be done by user in UI
-# your_framework_that_used_parsed_args(parsed_args) #Will be called in target_function
-
-def target_function(configurtion : Configuration):
-	# Since we can use the Configuration-instance as a dict 
-	# and as configuration.<attribute> we can just
-	# pass it to the framework compatible with the ArgumentParser:
-	your_framework_that_used_parsed_args(configuration)
-
-```
-
-# Configuration
-Configurun works with `configuration`-objects. A configuration is a collection of option-instances (=`@dataclass`-instances that inherit from `BaseOptions`), which are grouped toghether in a `Configuration`-wrapper.
-We can think of the option-instances as the different groups of options we want to edit and use in our run (e.g. `GeneralOptions()`, `LogOptions()`, `ModelOptions()`, etc.).
-In the simplest case, we have 1 single option-instance which contains all the options, `AllOptions()`. 
-
-The `Configuration`-wrapper enables us to access the attributes of all enclosed options-instances using `configuration[attribute]`/`configuration.<attribute>`/`option_class.get(attribute, default)`.
-
-An example of how to use a `Configuration`-instance:
-
-``` python
-from dataclasses import dataclass
-from configurun.configuration import Configuration
-from configurun.configuration import BaseOptions
-
-@dataclass
-class GeneralOptionsClass(BaseOptions):
-	simple_int : int = 1
-	#etc.
-
-@dataclass
-class OtherOptionClass(BaseOptions):
-	some_other_int : int = 2
-	#etc.
-
-
-config = Configuration()
-config.options['general_options'] = GeneralOptionsClass()
-config.options['other_options'] = OtherOptionClass()
-
-#Accessing the options, all of the following are equivalent:
-print(config['simple_int'])
-print(config.simple_int)
-print(config.get('simple_int', -1)))
-
-#These are also equivalent:
-print(config['some_other_int'])
-print(config.some_other_int)
-print(config.get('some_other_int', -1)))
-
-# Note that we can use the config.<attr>-notation to our advantage
-# when we want to use autocomplete in our editor. For example:
-# def target_function(configuration: GeneralOptionsClass)
-# Would result in our editor of choice recognizing/autocompleting
-# the `configuration.simple_hint` way of accessing `simple_hint`
-```
-
-
-
-# Option metadata
-The UI is mainly built around the [`field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.field) functionality of python-`dataclass`, which allows the display-model to make use of the default values, type hints and other information. 
-For each attribute in our `option`-definition, we can provide additional information in the `metadata` attribute of `field()`. This provides additional information to the UI, which is used to determine the editor-type, constraints etc. <br>
-
-For example:
-```python
-from configurun.configuration import base_options
-from dataclasses import field, dataclass
-#Used to constrain the editors: (can also be imported from sklearn)
-from pyside6_utils.utility.constraints import Interval 
-
-@dataclass
-class TestOptions(BaseOptions):
-	test_int_property : int | None = field(
-		default=None, #The default value used in the UI
-		metadata=dict( #Contains additional information for the UI
-			display_name="Test property", #The display-name
-			help="This is a test property that can also be none", #On-hover help-messagem
-			required=True, #If required, the field is red if not filled in
-			constraints = [ #Limit editors (min/max, options, etc.)
-				#The following constrains the editor to have value > 1
-				Interval(type=int, left=1, right=None, closed="both"), 
-				None #Or value can be None
-			] 
-			# etc...
-		)
-)
-```
-For more examples, please see the [example-options](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py). 
-
-The following metadata-keys are supported:
-
-| Metadata Key | Type | Description |
-| --- | --- | --- |
-| `"display_name"` | `str` | Name to display for this attribute in the view - defaults to the variable name itself |
-| `"display_path"` | `str` | Path to display this attribute - we can group/structure items. If parent does not exist, creates folders. Format as "|
-| `"help"` | `str` | Help-message which will be shown when the user hovers over this item - empty by default|
-| `"constraints"` | `List[constraint]` | Additional constraints on which the editor will be determined to apply to the field**, if none provided, use typehint of the field|
-| `"required"` | `bool` | Whether this field is required to be filled in - if true - a red background will appear if the value is not set|
-| `"editable"` | `bool` | Whether this field is editable - if false - the editor will be disabled|
-
-**: Constraints are sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into the [pyside6-utils](https://github.com/Woutah/pyside6-utils) package under [`utility.constraints`](https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/utility/constraints.py). The following constraints are supported:
-| Constraint | Description | Editor Type
-| --- | --- | --- |
-| `type` | The type of the value should match the type of the constraint | based on type |
-| `Options` / `Container` | The value should be one of the options provided in the constraint | `QComboBox` |
-| `StrOptions` | The value should be one of the str-options provided in the constraint | `QComboBox` |
-| `Interval` | The value should be within the interval provided in the constraint | `QSpinBox` or `QDoubleSpinBox` (limited) |
-| `None` | `None` is a valid value for this field (same as `typing.Optional`) | Adds reset-button to editor |
-| `Range` | The value should be within the range provided in the constraint | `QSpinBox` (limited) |
-
+Metadata-Version: 2.1
+Name: configurun
+Version: 0.2.0
+Summary: PySide6 based user-interface tools to create and manage machine learning training/testing-configurations and run them automatically and/or remotely..
+Home-page: https://github.com/Woutah/configurun
+Author: Wouter Stokman
+License: LGPLv2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Configurun
+
+Configurun is a cross-platform PySide6-based package that implements an application for managing, creating and (remotely) running python configurations.
+It was designed mainly with machine-learning tasks in mind, but can be used for any python script that takes arguments as an input. The editor-UI is created automatically using either an `argparse.Argumentparser` or python-`@dataclass`(es).
+
+The Configurun-app is especially useful for scripts/experiments that require a lot of arguments to be tweaked across many experiment-runs. It also makes the process of running experiments remotely much easier by enabling the user to edit, add and schedule tasks on any running Configurun server-instance reachable via a network connection.
+
+This package was created in tandem with [pyside6-utils](https://github.com/Woutah/pyside6-utils/).
+
+<p align="center">
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/main_window_example.png" width="1200" />
+</p>
+
+# Table of contents
+
+- [Configurun](#configurun)
+- [Table of contents](#table-of-contents)
+- [Features](#features)
+	- [Configuration Editor](#configuration-editor)
+	- [Run Queue](#run-queue)
+	- [Remote-processing](#remote-processing)
+- [Installation](#installation)
+- [How to run?](#how-to-run)
+	- [Local App](#local-app)
+	- [Client App](#client-app)
+	- [Server-instance](#server-instance)
+- [Option-source](#option-source)
+	- [Custom Options (`@dataclass`)](#custom-options-dataclass)
+	- [Custom Options (`ArgumentParser`)](#custom-options-argumentparser)
+	- [Custom Options (`Callable`)](#custom-options-callable)
+- [Target Function](#target-function)
+- [Configuration](#configuration)
+- [Option metadata](#option-metadata)
+- [SSH-tunneling](#ssh-tunneling)
+	- [No-hop](#no-hop)
+	- [Hopping](#hopping)
+
+# Features
+
+## Configuration Editor
+
+The configuration editor allows the user to specify a configuration-template using either (groups of) [`@dataclass`-class](#custom-options-dataclass) or an [`ArgumentParser`-instance](#custom-options-dataclass). The editor will then automatically create a UI based on the provided template. Editors are specifically created for each option-property based on provided template-types (and [extra constraints](#option-metadata)). 
+Help-messages are displayed on hover, required arguments are highlighted when not filled in, etc.
+<p align="center">
+	<!-- <img src="./configurun/examples/images/configuration_editor_example.png" width="600" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/configuration_editor_example.png" width="600" />
+</p>
+
+More complex typehints using `List` / `Union` / `Literal` are supported and are automatically built into widgets that allow the user to add/remove items and switch input-types:
+
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./configurun/examples/images/string_float_list_example.png" width=300/> -->
+</p>
+
+We can also define our own [option-source-method](#custom-options-callable) to dynamically create new option-groups based on the current configuration. This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. E.g: only show `ExtendedExampleModel`-options if property `model_type` in `MainOptions` is set to `"ExtendedExampleModel"`. <br>
+
+Configurations can be saved and loaded, a file-explorer view for the current workspace is made available.:
+<p align="center">
+	<!-- <img src="./configurun/examples/images/file_explorer_example.png" width="400" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/file_explorer_example.png" width="400" />
+</p>
+
+## Run Queue
+
+The run-queue window manages the currently running items. This could either be locally when using a [local-app](#local-app), or remotely, when using a [client-app](#client-app) and a [server-instance](#server-instance) on which the actual Run-Queue is running. The Run-Queue allows us to add/remove items, pause/resume items, change the queue-order of items, and start autoprocessing, which will automatically start the next item in the queue when the current item is finished. We can set the number of processors as well, to run multiple items in parallel.
+<p align="center">
+	<!-- <img src="./configurun/examples/images/run_queue_example.png" width="1100" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/run_queue_example.png" width="1100" />
+</p>
+
+Configurations are passed to the user-provided [target-function](#target-function) in separate processes. The stdout/stderr of each of the items is captured and displayed as a selectable console-output-view in the command-line-output window:
+<p align="center">
+	<!-- <img src="./configurun/examples/images/command_line_output_example.png" width="1100" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/command_line_output_example.png" width="1100" />
+</p>
+
+## Remote-processing
+
+Instead of using the [local-app](#local-app) to manage and run the configurations on your own machine, we can use the [client-app](#client-app) to connect to a [server-instance](#server-instance) on a remote machine. The client-app works analogous to the local-app and allows us to create and manage new configuration, but the Run-Queue runs on the connected remote Configurun-server:
+<p align="center">
+	<!-- <img src="./configurun/examples/images/network_login_example.png" width="300" /> -->
+	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/network_login_example.png" width="300" />
+</p>
+
+# Installation
+
+This package can downloaded from [this repository](https://github.com/Woutah/configurun), or can be installed directly from PyPi by using pip:
+
+``` bash
+pip install configurun
+```
+
+# How to run?
+
+Creating the app is done via the `configurun.create`-module. We can create 3 different types of apps:
+
+- [**Local app**](#local-app) - For running everything locally on your machine
+- [**Client app**](#client-app) - For running the configurations on a remote machine, connects to a `server`-instance
+- [**Server instance**](#server-instance) - Command-line instance that listens to connections from `client`-apps. If login is succesful, accepts control of the `RunQueue` from the `client`-app.
+
+On the client-side, the `options_source` should be set - the template of the settings used to create the [configuration-editor](#configuration-editor).<br>
+On the server/running-machine, the `target_function` should be set - the function that actually runs the task/experiment ([example](#target-function)).<br>
+
+## Local App
+
+A local app is an all-in-one app that can be used to create and run configurations locally on your machine.
+To run the example app, we can either call `run_example_app()` from `configurun.examples` or run the following code to construct the app ourselves:
+
+```python
+### This example will run the app with an example configuration
+# Also see `configurun/examples/example_target_function.py`
+# Also see `configurun/examples/example_deduce_new_option_class_types.py`
+import os
+from configurun.app import run_local
+from configurun.examples import example_target_function, example_deduce_new_option_classes
+
+if __name__ == "__main__": #Makes sure bootstrapping process is done when running app
+	run_local( #Create and runs a local configurun app-instance
+		target_function=example_target_function, #The function that will be called with the configuration
+		options_source=example_deduce_new_option_classes, #Template for UI-optiosn: Callable/@datclass/ArgumentParser
+		workspace_path = os.path.join( #Settings, configs and the Run-Queue will be saved/loaded from/to here
+			os.getcwd(),
+			"LocalExampleWorkspace"
+		)
+	)
+```
+
+In this example, [`example_target_function`](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_target_function.py) runs a dummy task that logs to a file for 20 seconds. We can [specify our own target-function](#target-function) to run our own scripts.
+
+We can [specify our own options source](#option-source) to create our own options-class for the configuration-editor, for example by [using an existing `ArgumentParser`-object.](#custom-options-argumentparser)
+
+## Client App
+
+We can create a client-app and use it to login to running [server](#server-instance)-instances. We can then use the client-app analogous to the [local-app](#local-app) to create new confiugrations and add/run/manage configurations on the remote machine.<br>
+
+```python
+# Opens a client-side app that we can use to connect to and control
+# the server-instance
+import os
+from configurun.app import run_client
+from configurun.examples import example_deduce_new_option_classes
+
+if __name__ == "__main__":
+	run_client(
+		options_source=example_deduce_new_option_classes,
+		workspace_path=os.path.join(os.getcwd(), "ClientExampleWorkspace"),
+	)
+```
+
+## Server-instance
+
+The server-instance is a command-line app that listens to connections from [`client`](#client-app)-instance(s) to receive new configurations and commands to manage its RunQueue. The actual target-functions are ran on this machine. <br>
+
+**NOTE:** *after* authentication, `pickle`/`dill` is used to transmit data, which indirectly enables arbitrary code execution on the server-side if the password is known. Please run the server on trusted network environments only. Run at your own risk!
+
+```python
+# Opens a server-instance which tries to connect with clients and allows
+# them to add configurations to the queue to be run on this machine
+import os
+from configurun.server import run_server
+from configurun.examples.example_target_function import example_target_function
+
+if __name__ == "__main__":
+	# WARNING:
+	# THIS ALLOWS OTHER MACHINES THAT RESIDE ON THE SAME NETWORK
+	# TO EXECUTE ARBITRARY CODE ON THIS MACHINE IF THEY KNOW THE
+	# PASSWORD. PLEASE RUN IN A TRUSTED NETWORK ENVIRONMENT ONLY
+	# RUN AT YOUR OWN RISK!
+	run_server(
+		target_function=example_target_function,
+		workspace_path=os.path.join(os.getcwd(), "ServerExampleWorkspace"),
+		password="password", #Password to connect to the server, make sure to change this!
+		port=5454 #Port to connect to the server, defaults to 5454
+	)
+```
+
+# Option-source
+
+When creating an app using the `create`-module, we can define a custom source, using the `options_source=...`, so we can construct the UI using our own options.
+We can use the following types as an options-source:
+
+- [`@dataclass`-object](#custom-options-dataclass)
+- [`ArgumentParser`-object](#custom-options-argumentparser)
+- [`Callable`](#custom-options-callable)
+
+## Custom Options (`@dataclass`)
+
+**NOTE:** Using `@dataclass`-fields results in more control over the final UI, for a more thorough example, please see [this section](#option-metadata) and/or the example implementations in [configurun/examples/example_options/example_options.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
+
+**NOTE:**  When implementing custom option-classes, don't forget to add the `@dataclass`-decorator, and always inherit from `BaseOptions`
+
+UI-supported type-hints include `str`, `int`, `float`, `datatime`, `typing.Literal`  (and more) and combinations using `typing.List`, `typing.Union` / `|`. For example:
+
+```python
+import os
+import typing
+from dataclasses import dataclass
+from configurun.configuration.base_options import BaseOptions
+from configurun.app import run_local
+from configurun.examples import example_target_function
+
+
+@dataclass #Don't forget to add this(!) - otherwise the app will not recognize the fields
+class MyCustomOptions(BaseOptions): #Always inherit from BaseOptions (required to run config)
+	simple_int : int = 1
+	complex_property : typing.List[typing.Union[int, str]] | None = None # Union = |-notation
+	# etc...
+
+if __name__ == "__main__":
+	run_local(
+		target_function=example_target_function,
+		options_source=MyCustomOptions, #Simple: each configuration consists of a single options-class
+		workspace_path = os.path.join(os.getcwd(), "ExampleDataclassOptions")
+	)
+
+
+```
+
+## Custom Options (`ArgumentParser`)
+
+We can use a `ArgumentParser`-object as an options source, this will internally convert the argument parser into a `@dataclass`-object, which is then used as an options-class. Whenever possible, arguments are also parsed to the UI (e.g. `required=True`, `help="Will be displayed on hover"` etc.).
+
+```python
+import argparse
+import os
+from configurun.app import run_local
+from configurun.examples import example_target_function
+
+parser = argparse.ArgumentParser()
+parser.add_argument("--required_arg", type=str, required=True, help="Required argument help")
+#... add more arguments here
+
+if __name__ == "__main__":
+	run_local(
+		target_function=example_target_function,
+		options_source=parser, #Parser is converted internally to a dataclass-class which is used as the options-class
+		workspace_path = os.path.join(os.getcwd(), "ExampleArgparseOptions")
+	)
+```
+
+## Custom Options (`Callable`)
+We define an `option`-class as a class that has the `@decorator` and inherits from the `BaseOptions`-class.
+
+A configuration is a collection of option-instances, which are grouped toghether in a [`Configuration()`](#configuration)-wrapper, which enables us to access the attributes of all enclosed options-instances using the `configuration[attribute]` / `configuration.<attribute>` / `option_class.get(attribute, default)`. For more information, see [this section](#configuration).
+
+As an options-source, we can create a callable which takes the current Configuration-instance as an argument and returns 1 or more new options-classes (***not** instances*) which is called every time a setting is changed. If the types-change, the UI will be updated to reflect the new templates.
+This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. For example:
+
+```python
+#In this example, we will create a callable which returns new options-classes based on the
+# current configuration
+import os
+import typing
+from dataclasses import dataclass
+from configurun.app import run_local
+from configurun.examples import example_target_function
+from configurun.configuration import BaseOptions, Configuration
+
+@dataclass #NOTE: Always use @dataclass for options
+class AlwaysTheSame(BaseOptions): #NOTE: Always use BaseOptions as base class for options
+	base_int : int = 1
+	#...
+
+@dataclass
+class CustomOptionsDefault(BaseOptions):
+	simple_int : int = 1
+	#...
+
+@dataclass
+class CustomOptionsUnderConditions(BaseOptions):
+	simple_int : int = 2
+	some_more_options : str = 'Some string'
+	#...
+
+def deduce_new_option_classes(configuration: Configuration)\
+		-> typing.Dict[str, typing.Type[BaseOptions | None]]: #Always return a dict of option
+	 		# classes the key of the dict is the name/group of the option-class
+			# the value is the option-class (@dataclass & BaseOptions) itself
+	if configuration.options is None or len(configuration.options) == 0:
+		pass #If initial configuration is being retrieved -> return default dict
+	elif configuration.base_int == 2 and configuration.simple_int != 1:
+		#Only return the CustomOptionsUnderConditions-class when base_int == 2 & simple_int != 1
+		#NOTE: if we're not sure if attributes exist, we can use the `.get(key, default)` method
+		return { #UI will be built using the following option-classes, each key gets a tab/window:
+			'always_the_same' : AlwaysTheSame,
+			'custom_options' : CustomOptionsUnderConditions
+		}
+
+	return { #UI will be built using the following option-classes, each key gets a tab/window:
+		'always_the_same' : AlwaysTheSame,
+		'custom_options' : CustomOptionsDefault
+	} #NOTE: we must ALWAYS return a dictionary with at least 1 option class
+
+if __name__ == '__main__':
+	run_local(
+		target_function=example_target_function,
+		options_source=deduce_new_option_classes,
+		workspace_path = os.path.join(os.getcwd(), "ExampleCallableOptions")
+	)
+
+```
+
+# Target Function
+
+The target function is the function that does all the work. This is the function that is being called when an item starts "running" in the Run-Queue.
+It takes a single argument: a [`Configuration`-instance](#configuration).
+The configuration-object contains all settings as set by the user when "add to queue" was pressed. 
+
+This example uses the example-configuration from [the Configuration section](#configuration), we simply print the values of the configuration to the console:
+
+```python
+def target_function(configuration: Configuration):
+	#Do something with the configuration
+	print(configuration.simple_int)
+	print(configuration.some_other_int)
+	#etc.
+```
+
+If you have replaced an `argparse.Argumentparser`, this is the place where you insert the user-provided settings to the script that uses the `ArgumentParser`-object. For example:
+
+```python
+# parsed_args = parser.parse_args() #will be done by user in UI
+# your_framework_that_used_parsed_args(parsed_args) #Will be called in target_function
+
+def target_function(configurtion : Configuration):
+	# Since we can use the Configuration-instance as a dict
+	# and as configuration.<attribute> we can just
+	# pass it to the framework compatible with the ArgumentParser:
+	your_framework_that_used_parsed_args(configuration)
+```
+
+Of course you can also directly pass the `your_framework_that_used_parsed_args(...)`-function as the target function when creating the app:
+
+```python
+if __name__ == '__main__':
+	local_app(
+		target_function=your_framework_that_used_parsed_args,
+		options_source=deduce_new_option_classes,
+		workspace_path = os.path.join(os.getcwd(), "ExampleCallableOptions")
+	)
+```
+
+This example uses the `deduce_new_option_classes`-function from [callable option source example](#custom-options-callable) .
+
+# Configuration
+
+Configurun works with `configuration`-objects. A configuration is a collection of option-instances (=`@dataclass`-instances that inherit from `BaseOptions`), which are grouped toghether in a `Configuration`-wrapper.
+We can think of the option-instances as the different groups of options we want to edit and use in our run (e.g. `GeneralOptions()`, `LogOptions()`, `ModelOptions()`, etc.).
+In the simplest case, we have 1 single option-instance which contains all the options, for example: `AllOptions()`.
+
+The `Configuration`-wrapper enables us to access the attributes of all enclosed options-instances using `configuration[attribute]`/`configuration.<attribute>`/`option_class.get(attribute, default)`.
+
+An example of how to use a `Configuration`-instance:
+
+``` python
+from dataclasses import dataclass
+from configurun.configuration import Configuration
+from configurun.configuration import BaseOptions
+
+@dataclass
+class GeneralOptionsClass(BaseOptions):
+	simple_int : int = 1
+	#etc.
+
+@dataclass
+class OtherOptionClass(BaseOptions):
+	some_other_int : int = 2
+	#etc.
+
+
+# Normally, the following would be done by the app using the UI
+# input and/or the user-provided option-source
+config = Configuration()
+config.options['general_options'] = GeneralOptionsClass()
+config.options['other_options'] = OtherOptionClass()
+
+#Accessing the options, all of the following are equivalent:
+print(config['simple_int'])
+print(config.simple_int)
+print(config.get('simple_int', -1))) #Would return -1 if key-error occurs
+
+#These are also equivalent:
+print(config['some_other_int'])
+print(config.some_other_int)
+print(config.get('some_other_int', -1)))
+
+# Note that we can use the config.<attr>-notation to our advantage
+# when we want to use autocomplete in our editor. For example:
+# def target_function(configuration: GeneralOptionsClass)
+# Would result in our editor of choice recognizing/autocompleting
+# the `configuration.simple_hint` way of accessing `simple_hint`
+```
+
+# Option metadata
+
+The UI is mainly built around the [`field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.field) functionality of python-`dataclass`, which allows the display-model to make use of the default values, type hints and other information.
+While typehints (e.g. `int`, `str`, `typing.List[int]`, etc.) are enough to create the editors, we can also provide additional information in the `metadata`-attribute of `field()` to further constrain the editors and provide additional information to the user. <br>
+
+For example:
+
+```python
+from configurun.configuration import base_options
+from dataclasses import field, dataclass
+#Used to constrain the editors: (can also be imported from sklearn)
+from pyside6_utils.classes.constraints import Interval, ConstrainedList
+
+@dataclass
+class TestOptions(BaseOptions):
+	test_int_list_property : typing.List[int] | None = field(
+		default=None, #The default value used in the UI
+		metadata=dict( #Contains additional information for the UI
+			display_name="Test property", #The display-name
+			help="This is a test property that can also be none", #On-hover help-messagem
+			required=True, #If required, the field is red if not filled in
+			constraints = [ #Limit editors (min/max, options, etc.)
+				#The following constrains the editor to have value > 1
+				ConstrainedList([Interval(type=int, left=1, right=None, closed="both")]),
+				None #Or value can be None
+			]
+			# etc...
+		)
+)
+```
+
+For more examples, please see the [example-options](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
+
+The following metadata-keys are supported:
+
+| Metadata Key | Type | Description |
+| --- | --- | --- |
+| `"display_name"` | `str` | Name to display for this attribute in the view - defaults to the variable name itself |
+| `"display_path"` | `str` | Path to display this attribute - we can group/structure items when using a treeview - defaults to no parents|
+| `"help"` | `str` | Help-message which will be shown when the user hovers over this item - empty by default|
+| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [*](#constraintnote) , if none provided, use typehint of the field|
+| `"required"` | `bool` | Whether this field is required to be filled in - if true - a red background will appear if the value is not set|
+| `"editable"` | `bool` | Whether this field is editable - if false - the editor will be disabled|
+
+<a name="constraintnote">*=</a>Constraints are (almost entirely) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `classes.constraints`. The following constraints are supported:
+| Constraint | Description | Editor Type
+| --- | --- | --- |
+| `type` | The type of the value should match the type of the constraint | based on type |
+| `Options` / `Container` | The value should be one of the options provided in the constraint | `QComboBox` |
+| `StrOptions` | The value should be one of the str-options provided in the constraint | `QComboBox` |
+| `Interval` | The value should be within the interval provided in the constraint | `QSpinBox` or `QDoubleSpinBox` (limited) |
+| `None` | `None` is a valid value for this field, same as `typing.Optional` | Adds reset-button to editor |
+| `Range` | The value should be within the range provided in the constraint | `QSpinBox` (limited) |
+| `ConstrainedList` | [*(Custom - not part of Sklearn)](#constrainedlist) Indicates a list of of values of a constrained type | Based on type of list |
+
+<a name="constrainedlist">*=</a>For example, `ConstrainedList([Interval(float, 0.0, 1.0), StrOptions(["string1", "string2"])])` indicates a list of values that should either be a float between 0.0 and 1.0, or the string "string1" or "string2". The editor for this field would be constructed as a `WidgetList` to which the user can add `WidgetSwitcher`. The `WidgetSwitcher` would then have two widgets, one with a `QSpinBox` and one with a `QComboBox` as the editor. **NOTE:** the same editor would be parsed from a `Typing.List[typing.Union[float, Typing.Literal["string1", "string2"]]]` typehint, minus the bounded-interval constraint on the float:
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/string_float_list_example.png" width=300/> -->
+</p>
+
+# SSH-tunneling
+
+This section contains a quick tutorial on how to use SSH-tunnels to connect to a remote server-instance in case we're not running client and server on the same machine/network.
+
+## No-hop
+
+A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without opening up any ports on the server-side.
+If we can directly SSH into the target machine, we can connect the ports as follows (assuming we're using the default `5454`-port in both the server and client configuration):
+
+```bash
+ssh -L 5454:localhost:5454 user@remote_host
+```
+
+On the client-side, we can then connect to the server-instance by using `localhost:5454` as the host and the password we set in the server-instance.
+
+## Hopping
+
+If we cannot directly access the remote-machine, we can use a 2-step SSH-tunnel to connect to the server-instance.
+This example assumes we have:
+
+- `remote1`: directly accessible from our machine
+- `remote2`: only accessible from `remote1`
+- Using default Configurun-port `5454` on both the client and server-side
+
+We can then connect to `remote2` from our machine using the following command:
+
+```bash
+ssh -L 5454:localhost:61521 <username>@<remote1-ip> ssh -L 61521:localhost:5454 -N <remote2-ip>
+```
+
+This example forwards `localhost:5454`->`remote1:61521`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
```

### Comparing `configurun-0.1.0/configurun/classes/method_call_interceptor.py` & `configurun-0.2.0/configurun/classes/method_call_interceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Can be used to create a 'virtual'-instance of a class on which calls
 can be forwarded to a server on which the "actual" instance of the class is running
 """
 
 from abc import abstractmethod
 from types import FunctionType
 import inspect
-import PySide6.QtCore as QtCore
 
 
 def get_class_implemented_methods(obj : type, exclude_parent_methods : bool = True) -> list[str]:
 	"""
 	Get all non-dunder methods of an object
 	"""
 	parent_methods = set()
@@ -43,15 +42,15 @@
 		returns:
 			Any : return value of the function
 
 		"""
 		raise NotImplementedError()
 
 
-class MethodCallInterceptedMeta(type(QtCore.QObject)):
+class MethodCallInterceptedMeta(type):
 	"""
 	Metaclass that intercepts all calls to the method-list provided by the user and sends them to
 	the function: _interceptor instead. This allows the user to create a proxy-instance of a
 	class which passes all function calls on to a remote server on which the actual instance of the
 	class is running.
 
 	NOTE: the interceptor-method (_interceptor) should be implemented in the class that uses this
```

### Comparing `configurun-0.1.0/configurun/classes/run_queue.py` & `configurun-0.2.0/configurun/classes/run_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 from datetime import datetime
 from enum import Enum
 
 import dill
 import multiprocess  # NOTE: we use multiprocess instead of multiprocessing because it allows more flexibility in pickling
 import multiprocess.managers as managers  # Same here, use multiprocess
 import multiprocess.queues
+import PySignal
 
-from PySide6 import QtCore
+from configurun.configuration.configuration import Configuration
 
+# from PySide6 import QtCore
 
-from configurun.configuration.configuration_model import Configuration
 
 
 class RunQueueHasRunningItemsException(Exception):
 	"""
 	Exception raised when trying to load a queue from file that contains running items when its allow flag is set to
 	False.
 	"""
@@ -227,20 +228,21 @@
 
 CustomManager.register(RunQueueItem.__name__, RunQueueItem, CustomProxy)
 	#Register the class so that it can be shared
 	#  between processes NOTE: making changes in the config itself will not be propagated - only if the whole object is
 	# replaced (https://docs.python.org/3/library/multiprocessing.html#multiprocessing-proxy-objects)
 
 
-class CommandlineQueueEmitter(QtCore.QObject):
+class CommandlineQueueEmitter():
 	"""
 	A class that keeps track of a command-line-queue and emits a signal each time an item is added to the queue.
 	Enables the use of multiple threads, while still logging to the UI without polling files.
 	"""
-	commandLineOutput = QtCore.Signal(int, str, str, datetime, int, str) #id, name, output_path, dt, filepos, new_msg
+	# commandLineOutput = QtCore.Signal(int, str, str, datetime, int, str) #id, name, output_path, dt, filepos, new_msg
+	commandLineOutput = PySignal.ClassSignal() #int, str, str, datetime, int, str
 
 	def __init__(self, monitored_queue : typing.Union[queue.Queue, multiprocess.queues.Queue]) -> None:
 		super().__init__()
 		self._monitored_queue = monitored_queue
 		self.stop_flag = False
 
 	def run(self):
@@ -255,41 +257,65 @@
 				pass
 			except BrokenPipeError:
 				log.warning("Broken pipe error in CommandlineQueueEmitter - if this occured while app was closing, you can "
 	      				"ignore this warning. Queue-emitter will now stop monitoring the command-line output queue.")
 				self.stop_flag = True
 
 
-class RunQueue(QtCore.QObject):
+class RunQueue():
 	"""
 	A class in which we can queue configurations to run tasks. The Configurations are ran in separate processes.
 	We can turn on automatic processing, which will automatically start processing items in the queue if the number
 	of processes allows for it.
 
 	TODO: We should also be able to manually start processing items in the queue.
 	"""
-	queueChanged = QtCore.Signal(object) #Emits a snapshot of the current queue when the queue changes (list of ints)
-	# runListChanged = QtCore.Signal(object) #Emits a snapshot of the all_list when the all_list changes
+
+
+	######################### OLD PYSIDE 6 VERSION #########################
+	# queueChanged = QtCore.Signal(object) #Emits a snapshot of the current queue when the queue changes (list of ints)
+	# # runListChanged = QtCore.Signal(object) #Emits a snapshot of the all_list when the all_list changes
+	# # 		# type is (typing.Dict[int, RunQueueItem])
+	# allItemsDictInsertion = QtCore.Signal(list, object) #Emits a list of id(s) and the new item-dict when new item(s) are
+	# 	# inserted we can utilize this in qt-models to update (Tree/Table) models by just inserting rows instead of resetting
+	# allItemsDictRemoval = QtCore.Signal(list, object) #Emits a list of id(s) and the new all_dict when item(s) is/are
+	# 	# removed we can utilize this in qt-models to update (Tree/Table) models by just removing rows instead of resetting
+
+	# itemDataChanged = QtCore.Signal(int, object) #Emits an id with the new RunQueueItem when a single item in the
+	# 		# all_dict has been changed
+
+	# queueRunStateChanged = QtCore.Signal(bool) #True if the queue is running, False if it is no longer running
+	# autoProcessingStateChanged = QtCore.Signal(bool) #Emits True if autoprocessing is enabled, False if it is disabled
+
+	# #TODO: implement a thread that keeps watch of a separate thread in which a queue with log-updates is processed
+	# newCommandLineOutput = QtCore.Signal(int, str, str, datetime, int, str) #id, name, output_path, dt, filepos, new_msg
+	# currentlyRunningIdsChanged = QtCore.Signal(object) #Emits a list of ids that are currently running
+	# resetTriggered = QtCore.Signal() #Emitted when the queue is reset (indicates that all models should be reset)
+	####################################################################################
+	
+
+	############################New version without pyside6 dependency#######################
+	queueChanged = PySignal.ClassSignal() #Emits a snapshot of the current queue when the queue changes (list of ints)
+	# runListChanged = PySignal.ClassSignal(object) #Emits a snapshot of the all_list when the all_list changes
 	# 		# type is (typing.Dict[int, RunQueueItem])
-	allItemsDictInsertion = QtCore.Signal(list, object) #Emits a list of id(s) and the new item-dict when new item(s) are
+	allItemsDictInsertion = PySignal.ClassSignal() #Emits a list of id(s) and the new item-dict when new item(s) are
 		# inserted we can utilize this in qt-models to update (Tree/Table) models by just inserting rows instead of resetting
-	allItemsDictRemoval = QtCore.Signal(list, object) #Emits a list of id(s) and the new all_dict when item(s) is/are
+	allItemsDictRemoval = PySignal.ClassSignal() #Emits a list of id(s) and the new all_dict when item(s) is/are
 		# removed we can utilize this in qt-models to update (Tree/Table) models by just removing rows instead of resetting
 
-	itemDataChanged = QtCore.Signal(int, object) #Emits an id with the new RunQueueItem when a single item in the
+	itemDataChanged = PySignal.ClassSignal() #Emits an id with the new RunQueueItem when a single item in the
 			# all_dict has been changed
 
-	queueRunStateChanged = QtCore.Signal(bool) #True if the queue is running, False if it is no longer running
-	autoProcessingStateChanged = QtCore.Signal(bool) #Emits True if autoprocessing is enabled, False if it is disabled
+	queueRunStateChanged = PySignal.ClassSignal() #True if the queue is running, False if it is no longer running
+	autoProcessingStateChanged = PySignal.ClassSignal() #Emits True if autoprocessing is enabled, False if it is disabled
 
 	#TODO: implement a thread that keeps watch of a separate thread in which a queue with log-updates is processed
-	newCommandLineOutput = QtCore.Signal(int, str, str, datetime, int, str) #id, name, output_path, dt, filepos, new_msg
-	currentlyRunningIdsChanged = QtCore.Signal(object) #Emits a list of ids that are currently running
-
-	resetTriggered = QtCore.Signal() #Emitted when the queue is reset (indicates that all models should be reset)
+	newCommandLineOutput = PySignal.ClassSignal() #int, str, str, datetime, int, str = id, name, output_path, dt, filepos, new_msg
+	currentlyRunningIdsChanged = PySignal.ClassSignal() #Emits a list of ids that are currently running
+	resetTriggered = PySignal.ClassSignal() #Emitted when the queue is reset (indicates that all models should be reset)
 
 	def __init__(self,
 	      		target_function : typing.Callable[[Configuration], typing.Any],
 				n_processes : int = 1,
 				log_location : str= "",
 				log_location_make_dirs : bool = True
 			) -> None:
@@ -364,30 +390,47 @@
 			# Dictionary that keeps track of the output file for each process
 		self._cmd_id_name_path_dict_mutex = multiprocess.Lock() #Lock for the cmd_id_path_dict
 		#Queue that keeps track of outputs to the command line for each running process.
 		self._command_line_output_queue = self._manager.Queue()
 
 
 
+		#OLD version with pyside6 dependency
+		# self.queue_emitter = CommandlineQueueEmitter(self._command_line_output_queue)
+		# self.queue_emitter_thread = QtCore.QThread()
+		# self.queue_emitter.moveToThread(self.queue_emitter_thread)
+		# self.queue_emitter_thread.started.connect(self.queue_emitter.run)
+		# self.queue_emitter_thread.start()
+		# self.queue_emitter.commandLineOutput.connect(self.newCommandLineOutput)
+
+
+		#New version without pyside6 dependency
 		self.queue_emitter = CommandlineQueueEmitter(self._command_line_output_queue)
-		self.queue_emitter_thread = QtCore.QThread()
-		self.queue_emitter.moveToThread(self.queue_emitter_thread)
-		self.queue_emitter_thread.started.connect(self.queue_emitter.run)
+		self.queue_emitter_thread = threading.Thread(target=self.queue_emitter.run)
+		self.queue_emitter.commandLineOutput.connect(lambda *args: self.newCommandLineOutput.emit(*args))
+		# self.queue_emitter.commandLineOutput.connect(
+		# 	lambda *args: print(f"Command line changed{', '.join([str(i) for i in args])}"))
 		self.queue_emitter_thread.start()
-		self.queue_emitter.commandLineOutput.connect(self.newCommandLineOutput.emit)
-		# self.queue_emitter.commandLineOutput.connect(lambda *args: print(f"Got command line output: {args}"))
+
+
+	def handle_command_line_output(self, item_id : int, name , output_path, dt , filepos, new_msg):
+		self.newCommandLineOutput.emit(item_id, name, output_path, dt, filepos, new_msg)
 
 	def stop_command_line_queue_emitter(self):
 		"""
 		Stop the queue-emitter thread - should be called when terminating the queue
 		TODO: create and explicit cleanup function
 		"""
 		self.queue_emitter.stop_flag = True
-		self.queue_emitter_thread.quit()
-		self.queue_emitter_thread.wait()
+		#Pyside6-version
+		# self.queue_emitter_thread.quit()
+		# self.queue_emitter_thread.wait()
+
+		#Non-pyside6-version
+		self.queue_emitter_thread.join()
 
 
 	@staticmethod
 	def set_workspace_lock(workspace_path : str, lock_filename = WORKSPACE_LOCK_FILE_NAME):
 		"""
 		Lock the workspace by creating a lockfile in the workspace directory.
```

### Comparing `configurun-0.1.0/configurun/classes/run_queue_client.py` & `configurun-0.2.0/configurun/classes/run_queue_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,68 +4,69 @@
 
 import logging
 import queue
 import socket
 import threading
 import traceback
 
+import PySignal
 from Crypto.Cipher import PKCS1_OAEP
 from Crypto.PublicKey import RSA
-from PySide6 import QtCore
 
 from configurun.classes.method_call_interceptor import (
     MethodCallInterceptedMeta, get_class_implemented_methods)
 from configurun.classes.run_queue import RunQueue
 from configurun.classes.run_queue_datatypes import (
     RSA_KEY_SIZE_BITS, AESSessionKeyTransmissionData, AuthenticationException,
     LoginTransmissionData, PickledDataType, PickleTransmissionData,
     PubKeyTransmissionData, StateMsgType, StateTransmissionData, Transmission,
     TransmissionType)
 
 log = logging.getLogger(__name__)
 
 
-def get_pyqt_signal_names(the_object : type) -> list[QtCore.SignalInstance]:
+def get_pysignal_names(the_object : type) -> list[PySignal.ClassSignal]:
 	"""
-	Get all PySide6.QtCore.signals of an arbitrary object (by name)
+	Get all PySignal.ClassSignal instances of an arbitrary object (by name)	
 	"""
 	signals = []
-
 	for signal_name in the_object.__dict__:
-		if isinstance(the_object.__dict__[signal_name], QtCore.Signal):
+		if isinstance(the_object.__dict__[signal_name], PySignal.ClassSignal):
 			signals.append(signal_name)
+	return signals
 
 
-	return signals
 
 def no_function(*args, **kwargs): #pylint: disable=unused-argument
 	"""Dummy function that does nothing"""
 	pass #pylint: disable=unnecessary-pass
 
 class NoAuthenticatedConnectionException(Exception):
 	"""Exception raised when a function is called on a RunQueueClient that is not connected to a server"""
 
-class RunQueueClient(RunQueue,
-		    metaclass=MethodCallInterceptedMeta,
-			intercept_list=get_class_implemented_methods(RunQueue),
-			skip_intercept_list=get_pyqt_signal_names(RunQueue)):
+class RunQueueClient(
+		RunQueue,
+		metaclass=MethodCallInterceptedMeta,
+		intercept_list=get_class_implemented_methods(RunQueue),
+		skip_intercept_list=get_pysignal_names(RunQueue)
+	):
 	"""
 	Each clients acts as if it is a runQueue - connecting to a server on which the actual runQueue is running.
 	Each function of the runQueue is intercepted by this class and sent to the server (except the signals).
 
 	NOTE: this class uses ```RunQueue```- which uses pyqt signals - make sure a main event loop is running
 	(e.g. app.exec()) when using instances of this class
 
 	NOTE: if the client is not connected to a server - the method-interceptor instead returns None (and logs a warning)
 
 	As soon as a connection is established, the client will start listening to the server for signals and method calls.
 	Also, the reset-signal is emitted from the queue, indicating that all models should be reset.
 	"""
 
-	authenConnectionStateChanged = QtCore.Signal(bool) #Emitted when the authenticated connection state changes -
+	authenConnectionStateChanged = PySignal.ClassSignal() #Bool emitted when the authenticated connection state changes -
 		# True if connected and authenticated, False if either disconnected or not yet authenticated
 
 
 	def __init__(
 			self
 		) -> None:
 		"""Initializes the RunQueueClient
@@ -84,16 +85,14 @@
 		self._rsa_key : RSA.RsaKey = RSA.generate(RSA_KEY_SIZE_BITS)
 		self._public_key = self._rsa_key.publickey()
 		self._private_key = self._rsa_key
 		self._private_rsa_cipher = PKCS1_OAEP.new(self._rsa_key)
 
 		#Created based on the session key received from the server
 		self._listen_thread = None
-
-		self._test_thread = None
 		self._aes_session_key = None
 
 		# self._method_return_queue = queue.Queue() #When the server responds - the listener thread will put the
 			# result in this queue - should
 		self._method_response_dict : dict[int, queue.Queue] = {} #When the server responds - the listener thread will
 			#put the result in this queue - keys are method ids, values are the result of the method call
 		self._method_reponse_dict_lock = threading.Lock()
@@ -175,15 +174,17 @@
 		"""
 		Wait for server response after a function call. Response is automatically put in reponse_dict by the server-
 		listener. If, after timeout, no response is received in this dict, a TimeoutError is raised.
 		"""
 		return_queue = self._method_response_dict[function_response_id]
 		try:
 			ret = return_queue.get(block=True, timeout=timeout)
-			log.info(f"Received response from server for method call with id {function_response_id}, response: {ret}")
+			log.info(f"Received response from server for method call with id {function_response_id}, response: {ret} "
+	    		f"of type {type(ret)}"
+			)
 		except (TimeoutError, queue.Empty) as exception: #If the queue is empty, then the server did not respond in time
 			raise TimeoutError(f"Timeout while waiting ({timeout}s) for response of method call with \
 		    	id {function_response_id}") from exception
 		finally: #Always clean up the queue to no longer listen for this id
 			with self._method_reponse_dict_lock:
 				del self._method_response_dict[function_response_id]
 
@@ -324,18 +325,14 @@
 			self.resetTriggered.emit() #Emit the reset signal so all models re-request all data
 			log.info("Connected to server and authenticated. Can now request/receive/transmit data from/to server.")
 		except Exception as exception:
 			#Just pass on the exception
 			self.disconnect_clean_server() #Clean up
 			raise exception
 
-		# self._test_thread = threading.Thread(target=self._send_to_server)
-		# self._test_thread.start()
-
-
 
 	def _listen_to_server(self):
 		"""
 		Start listening to the server for Transmissions. E.g.:
 		- StateTransmissionData -> Server is sending a state message
 		- PickleTransmissionData -> Server is sending a pickled object - for example - a result of a function call or
 			a Signal object
@@ -374,20 +371,20 @@
 								self._method_response_dict[function_call_id].put(result, block=True)
 						elif unpickled_data[0] == PickledDataType.SIGNAL_EMIT:
 							#The server is sending a signal
 							#Unpack the data
 							signal_name, args = unpickled_data[1]
 
 							#Get signal by name
-							signal : QtCore.SignalInstance = getattr(self, signal_name)
+							signal : PySignal.Signal = getattr(self, signal_name) #NOT QT SIGNAL (actually classignal)
 							log.debug(
 								f"Received signal {signal_name} from server - resulting in a re-transmit of signal"
 									f"{signal} of type {type(signal)}"
 							)
-							assert isinstance(signal, QtCore.SignalInstance)
+							assert isinstance(signal, PySignal.Signal)
 							#Emit the signal
 							signal.emit(*args) #type: ignore
 						else:
 							log.error(f"Received pickled data of type {unpickled_data[0].name} - which is not "
 		 						"supported (at the client side)")
 					except Exception as exception: # pylint: disable=broad-exception-caught
 						log.error(f"Error while unpickling pickle-transmission from server - {type(exception)}: "
```

### Comparing `configurun-0.1.0/configurun/classes/run_queue_datatypes.py` & `configurun-0.2.0/configurun/classes/run_queue_datatypes.py`

 * *Files identical despite different names*

### Comparing `configurun-0.1.0/configurun/classes/run_queue_server.py` & `configurun-0.2.0/configurun/classes/run_queue_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import time
 import typing
 
 import dill
 from Crypto.Cipher import PKCS1_OAEP
 from Crypto.PublicKey import RSA
 from Crypto.Random import get_random_bytes
-from PySide6 import QtCore
+import PySignal
 
 from configurun.classes.run_queue import (WORKSPACE_RUN_QUEUE_SAVE_NAME,
                                           RunQueue, WorkspaceInUseException)
 from configurun.classes.run_queue_datatypes import (
     AES_EMPTY_KEY, RSA_KEY_SIZE_BITS, AESSessionKeyTransmissionData,
     AuthenticationException, ClientData, LoginTransmissionData,
     PickledDataType, PickleTransmissionData, PubKeyTransmissionData,
@@ -88,21 +88,15 @@
 					#re-raise the exception
 					raise
 				else:
 					print("Invalid choice - please enter 'y' or 'n'")
 
 		self._initial_run_queue_load() #Load the run-queue from the workspace- might ask for user input if problem arises
 
-		self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-		used_host_name = socket.gethostname() if (hostname is None or len(hostname) == 0) else hostname
-		log.info(f"Binding server to {used_host_name}:{port}")
-		self._socket.bind(( #Bind the socket to the given hostname and port
-				used_host_name,
-				port
-		))
+		self._socket = None
 
 		#Generate a public/private key pair for the server
 		self._rsa_key : RSA.RsaKey = RSA.generate(RSA_KEY_SIZE_BITS)
 
 		self._public_key = self._rsa_key.publickey().export_key()
 		self._private_key = self._rsa_key.export_key()
 		self._private_cipher = PKCS1_OAEP.new(self._rsa_key) #Used to decrypt data sent by the clients
@@ -113,21 +107,23 @@
 		self.set_password_hash(self.get_password_hash(password=password))
 
 		self._client_dict : dict[socket.socket, ClientData]= {}
 		self._client_dict_lock = threading.Lock()
 
 		self._connection_listener_thread = None
 		self._is_terminating = False #To check whether the server is terminating (don't start doing new stuff)
-		self._server_stop_flag = threading.Event() #To stop the server from running (does not always indicate full termination)
+		self._server_stop_flag = threading.Event() #To stop the server from running (does not always indicate termination)
 
+		self._hostname = hostname
+		self._port = port
 
 		#============= Manage signal-triggered events =============
-		#Go over all signal (QtCore.Signal) and link them to emit_signal
 		for signal_name in self._run_queue.__class__.__dict__:
-			if isinstance(self._run_queue.__class__.__dict__[signal_name], QtCore.Signal):
+			# if isinstance(self._run_queue.__class__.__dict__[signal_name], QtCore.Signal): #Previous version used qt
+			if isinstance(self._run_queue.__class__.__dict__[signal_name], PySignal.ClassSignal): #Use pysignal for server-side
 				target_signal = getattr(self._run_queue, signal_name)
 				target_signal.connect(lambda *args, signal_name=signal_name: self.emit_signal(signal_name, *args))
 
 		log.info("Initialized RunQueueServer")
 
 	def terminate(self):
 		"""
@@ -218,14 +214,23 @@
 	def run(self):
 		"""Starts the server and listens for connections
 		"""
 		if self._is_terminating:
 			raise RuntimeError("Server is terminating - cannot start running the server now...")
 		if self._connection_listener_thread is not None:
 			raise RuntimeError("Server is already running")
+		if self._socket is not None:
+			raise RuntimeError("Server is already running - socket already exists")
+		self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+		used_host_name = socket.gethostname() if (self._hostname is None or len(self._hostname) == 0) else self._hostname
+		log.info(f"Binding server to {used_host_name}:{self._port}")
+		self._socket.bind(( #Bind the socket to the given hostname and port
+				used_host_name,
+				self._port
+		))
 		self._connection_listener_thread = threading.Thread(target=self._listen_for_connections)
 		self._connection_listener_thread.start()
 		self._server_stop_flag.clear()
 		# self._listen_for_connections()
 
 	def emit_signal(self, signal_name: str, *args):
 		"""Emits a QtCore.Signal to the server
@@ -600,29 +605,29 @@
 			with self._client_dict_lock: #Remove the client from the list of authenticated clients
 				del self._client_dict[client]
 			client.close() #Try to close connection (if not already closed)
 
 
 def run_example_server(password : str = "password", port : int = 5454, log_level : int = logging.INFO):
 	"""
-	Runs an example-instance of the server, using the example_target_function from configurun/examples/example_target_function.py
-	and the passed password as well as the default workspace path (~/Configurun-Server)
+	Runs an example-instance of the server, using the example_target_function from 
+	configurun/examples/example_target_function.py and the passed password as well as the default
+	workspace path (~/Configurun-Server)
 
 	Args:
 		password (str, optional): The password to connect to the server. Defaults to "password".
 	"""
 	#pylint: disable=import-outside-toplevel
-	from configurun.create import server
+	from configurun.server.create_server import run_server
 	import tempfile
-	from configurun.windows.main_window import APP_NAME
 	from configurun.examples.example_target_function import example_target_function
 	tempdir = tempfile.gettempdir()
-	workspace_path = os.path.join(tempdir, APP_NAME, "Configurun-Server-Example")
+	workspace_path = os.path.join(tempdir, "Configurun", "Configurun-Server-Example")
 
-	server(
+	run_server(
 		target_function=example_target_function,
 		workspace_path=workspace_path,
 		password=password,
 		port=port,
 		log_level=log_level
 	)
```

### Comparing `configurun-0.1.0/configurun/configuration/argparse_to_dataclass.py` & `configurun-0.2.0/configurun/configuration/argparse_to_dataclass.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 import argparse
 import logging
 import sys
 from dataclasses import field, make_dataclass
 
-from pyside6_utils.utility.constraints import (Interval, Options)
+from pyside6_utils.classes.constraints import (Interval, Options)
 
 from configurun.configuration.base_options import BaseOptions
 
 log = logging.getLogger(__name__)
 
 
 def argparse_to_dataclass(
@@ -93,14 +93,14 @@
 	new_dataclass.__module__ = module #Set the module attribute of the new class to the module of the caller #type:ignore
 	globals()[dataclass_name] = new_dataclass #Also add class to global scope to enable pickling from this module
 		# note that it is probably easier to make use of dill
 	return new_dataclass
 
 
 if __name__ == "__main__":
-	from configurun.create import local_app
+	from configurun.app.create_run import run_local
 	from configurun.examples.example_argparse import parser_example
 	test_dataclass = argparse_to_dataclass(parser_example)
-	local_app(
+	run_local(
 		target_function = lambda x, *_: print(x),
 		options_source = test_dataclass
 	)
```

### Comparing `configurun-0.1.0/configurun/configuration/base_options.py` & `configurun-0.2.0/configurun/configuration/base_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """ 
 Implements the base-options from which all user-defined options should inherit
 """
 
 
 import logging
 from dataclasses import dataclass
-
-from pyside6_utils.utility import Serializable
-
+from pyside6_utils.classes import Serializable #Absolute import to avoid import PySide6
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class BaseOptions(Serializable, object):
 	"""The base-option class, all other options classes should inherit from this class
 	A configuration is built by using 1 or more of these options classes.
```

### Comparing `configurun-0.1.0/configurun/configuration/configuration.py` & `configurun-0.2.0/configurun/configuration/configuration.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 	A Configuration object is built up using several (sub-configuration / option) dataclass instances.
 	This class is a wrapper around a dict of these sub-options classes. The __getattr__ function is used to
 	allow the user to access any of the sub-options classes using the . operator.
 
 	The individual option-instances are stored in the 'options' dict. The keys of this dict are the names of the
 	sub-options classes, e.g. "model_options", "dataset_options", "training_options", etc.
 
-	
-	NOTE: due to the way the __getattr__ function is implemented, the sub-options classes must not have overlapping 
+
+	NOTE: due to the way the __getattr__ function is implemented, the sub-options classes must not have overlapping
 	attribute names.
 	"""
 	#Use factory to create empty dict
 	options : typing.Dict[str, BaseOptions | None] = field(default_factory=dict)
 	 #Dict in which the sub-option dataclasses are stored. Example of a
 		# A possible configuration of this dict is:
 		# {
@@ -45,14 +45,20 @@
 				"model_options": SklearnModelOptions,
 				"dataset_options": BaseDatasetOptions,
 				"training_options": SklearnTrainingOptions
 			}
 		"""
 		return {key: type(value) for key, value in self.options.items()}
 
+	def hasinstance(self, instance_type: type) -> bool:
+		"""
+		Check if Configuration.options has an instance of the given type
+		E.g.
+		"""
+		return any(isinstance(value, instance_type) for value in self.options.values())
 
 	def hasattr(self, key):
 		"""
 		Check if one of the sub-options classes has the given attribute
 		"""
 
 		for options_class in self.options:
@@ -72,47 +78,72 @@
 			#Do something with config.model_type
 
 
 		NOTE: the limitation to this is that the suboptions classes must not have overlapping attribute names
 		This is why validateSubOptions should be called when chaning suboptions
 		TODO: check for overlapping attribute names in the __init__ function?
 		"""
-
 		if key.startswith("__"): #Return special/internal attributes, otherwise things like copy will go wrong
 			raise AttributeError(f"Attribute {key} not found in any of the options classes")
 
 		for options_instance in self.options.values():
 			if hasattr(options_instance, key):
 				return getattr(options_instance, key)
 
 		raise AttributeError(f"Attribute {key} not found in any of the options classes")
-	
+
 	def __getitem__(self, key):
 		return self.__getattr__(key)
 
 	def get(self, key : str, default : typing.Any):
 		"""
 		A safe alternative to the __getattr__ function. This function will return the default value if the given
-		key is not found.  
+		key is not found.
 
 		Args:
 			key (str): The attribute to look for
 			default (typing.Any): The default value to return if the attribute is not found
 		"""
+		if key is None:
+			return default
 		try:
-			return getattr(self, key)
+			return self.__getattr__(key)
 		except AttributeError:
 			return default
 
 
 	def get_dict(self):
 		"""
-		Return the sub-options instances as a dictionary
+		Return the full configuration as a dict. 
+		"""
+		new_dict = {}
+		for key, value in self.options.items(): #Convert all sub-options instances to dicts
+			new_dict[key] = value.__dict__
+		return new_dict
+
+	@staticmethod
+	def get_configuration_from_passed_options(*args) -> 'Configuration':
 		"""
-		return self.options
+		Create a new Configuration instance from the passed options. 
+
+		Args:
+			*args (typing.List[BaseOptions]): A list of options to add to the new configuration. ALL instances must 
+				inherit from BaseOptions and must have the @dataclass-decorator to be fully compatible with 
+				the Configuration-ui app. If directly used for the attribute-lookup function of this class,
+				this is not neccesry. 
+
+				NOTE: all options must have unique attribute names, otherwise the attribute-lookup function will
+				return the first attribute it finds with the given name.
+
+				#TODO: enforce this in the __init__ function of this class?
+		"""
+		new_config = Configuration()
+		for options in args:
+			new_config.add_options(options)
+		return new_config
 
 
 if __name__ == "__main__":
 	#Run some tests on the ConfigurationData class to see whether lookup is working
 	from copy import deepcopy
 	test_config = Configuration()
```

### Comparing `configurun-0.1.0/configurun/configuration/configuration_model.py` & `configurun-0.2.0/configurun/configuration/configuration_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,19 @@
 		for i, (option_name, option_class) in enumerate(type_dict.items()):
 			if option_name not in self._configuration.options: #If key doesn't yet exist
 				self._configuration.options[option_name] = None #Create key #type: ignore
 				self._option_proxy_model_dict[option_name] = QtCore.QSortFilterProxyModel()
 				proxy_models_changed = True
 			elif option_class is None or isinstance(option_class, type(None)): #If None or Nonetype -> empty
 				pass
-			elif type(self._configuration.options[option_name]) != option_class: #If the option class changed #pylint: disable=unidiomatic-typecheck
+			# elif type(self._configuration.options[option_name]) != option_class: #If the option class changed #pylint: disable=unidiomatic-typecheck
+			elif type(self._configuration.options[option_name]).__name__ != option_class.__name__: #If the option class changed #pylint: disable=unidiomatic-typecheck
+				#NOTE: this only checks the type NAME not the actual type. This makes us more flexible when saving/loading
+				# dill pickles, but might result in issues if the user uses class names interchangeably. 
+				# Note that on-load, we check for any attributes that are missing, so this might not be an issue.
 				pass
 			else:  #If everything is the same, skip
 				continue
 
 			#If we arrived here, we're changing the options-instance
 
 			#First cache current options instance (if enabled)
@@ -559,20 +563,32 @@
 		if len(option_group_mismatches) > 0:
 			class_group_names = ", ".join(cur_class_types.keys())
 			deduced_group_names = ", ".join(deduced_types.keys())
 			error_msgs.append(f"The configuration has option-names that differ from the deduced names.\n"
 				f"Current option-names:\n{class_group_names}\n"
 				f"Deduced option-names:\n{deduced_group_names}\n"
 				)
-		option_type_mismatches = set.symmetric_difference(set(cur_class_types.values()), set(deduced_types.values()))
+		#NOTE: only check name-equivalence, not strong type-equivalence
+
+		class_type_names = [i.__name__ for i in cur_class_types.values()]
+		deduced_type_names = [i.__name__ for i in deduced_types.values()]
+		option_type_mismatches = set.symmetric_difference(set(class_type_names), set(deduced_type_names))
+
+		
+		# option_type_mismatches = set.symmetric_difference(set(cur_class_types.values()), set(deduced_types.values()))
+		#NOTE: dill pickles by value if defined in the __main__ module -> if errors are reported here when loading
+		# this could be the issue... Probably best to first try to construct the class by deducing the types and 
+		# copying attributes over. We currently only check the type-names. This makes us more flexible but might 
+		# result in issues (though we're checking attributes when loading/saving the items so it might not be an issue)
+
 
 		if len(option_type_mismatches) > 0:
 			current_type_names = ", ".join([i.__name__ for i in cur_class_types.values()])
 			deduced_type_names = ", ".join([i.__name__ for i in deduced_types.values()])
-			option_type_mismatch_names = ", ".join([i.__name__ for i in option_type_mismatches])
+			option_type_mismatch_names = ", ".join([i for i in option_type_mismatches])
 			error_msgs.append(f"The configuration has types that differ "
 				f"differ from the expected (deduced) types.\n\n"
 				f"Current Types:\n{current_type_names}\n\n"
 				f"Deduced Types:\n{deduced_type_names}\n\n"
 				f"Difference (should be none):\n{option_type_mismatch_names}")
 		if len(error_msgs) > 0:
 			raise OptionTypesMismatch("\n\n".join(error_msgs))
@@ -627,8 +643,8 @@
 			self.proxyModelDictChanged.emit(self._option_proxy_model_dict)
 
 		if self.undo_stack:
 			# self.undo_stack.clear()
 			self.undo_stack.setActive(True)
 
 		if validate_after_setting:
-			self.validate_current_configuration()
+			self.validate_current_configuration()
```

### Comparing `configurun-0.1.0/configurun/create.py` & `configurun-0.2.0/configurun/app/create_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 
 """
-Convenience function to quickly create a local or networked app-instance (server/client/both) with the specified
+Convenience functions to quickly create & run local or networked app-instances (client/local_app) with the specified
 target function and option source.
 """
 import argparse
 import logging
 import os
-import signal
 import sys
 import typing
 
 from PySide6 import QtCore, QtWidgets
 
 from configurun.classes.run_queue import RunQueue
 from configurun.classes.run_queue_client import RunQueueClient
-from configurun.classes.run_queue_server import RunQueueServer
 from configurun.configuration.base_options import BaseOptions
 from configurun.configuration.configuration import Configuration
 from configurun.configuration.configuration_model import ConfigurationModel
-from configurun.windows.main_window import APP_NAME, MainWindow
-from configurun.windows.network_main_window import NetworkMainWindow
+from configurun.app.main_window import APP_NAME, MainWindow
+from configurun.app.network_main_window import NetworkMainWindow
 from configurun.configuration.argparse_to_dataclass import argparse_to_dataclass
 
 log = logging.getLogger(__name__)
 
 
 def _get_option_function(option_source:\
 			typing.Callable[[Configuration], typing.Dict[str, typing.Type[BaseOptions] | typing.Type[None]]] | \
@@ -53,31 +51,31 @@
 		return option_source
 	else:
 		raise ValueError(f"Invalid option_source: {option_source} of type {type(option_source)}")
 
 
 
 
-def local_app(
+def run_local(
 		target_function : typing.Callable,
 		options_source : \
 			typing.Callable[[Configuration], typing.Dict[str, typing.Type[BaseOptions] | typing.Type[None]]] | \
 			argparse.ArgumentParser | \
 			typing.Type[BaseOptions]
 				,
 		workspace_path : str = "",
 		create_workspace_path : bool = True, #Whether to create the workspace path if it does not exist
 		run_queue_n_processes : int = 1,
 		log_level : int = logging.INFO,
 		run_queue_kwargs : typing.Optional[typing.Dict[str, typing.Any]] = None,
 		config_model_kwargs : typing.Optional[typing.Dict[str, typing.Any]] = None,
 
 	):
-	"""Convenience function that constructs a local instance of the app with the specified target function and option
-	source. Workspace path is option, if none is provided, uses '~/Configurun/'.
+	"""Convenience function that creates and runs a local instance of the app with the specified target function and 
+	option source. Workspace path is option, if none is provided, uses '~/Configurun/'.
 
 	Args:
 		target_function (typing.Callable): The target function on which tasks will be run, this function should take
 			a configuration as the first argument, and the rest of the arguments should be the arguments passed to the
 			```RunQueue._process_queue_item()```-method.
 
 		options_source (typing.Callable[[Configuration], typing.Dict[str, typing.Type[BaseOptions]
@@ -114,15 +112,15 @@
 	handler.setFormatter(formatter)
 	logging.basicConfig(
 		handlers=[handler],
 		level=log_level) #Without time
 	root_logger = logging.getLogger()
 	root_logger.setLevel(log_level)
 
-	
+
 	if run_queue_kwargs is None:
 		run_queue_kwargs = {}
 	if config_model_kwargs is None:
 		config_model_kwargs = {}
 
 	app = QtWidgets.QApplication(sys.argv)
 
@@ -159,151 +157,56 @@
 		window=main_window,
 		workspace_path=workspace_path
 	)
 
 	main_window.show() #Show the window
 	app.exec()
 
-
-def _cleanup_server(app : QtCore.QCoreApplication, run_queue_server : RunQueueServer):
-	"""
-	Callback function to, on process end (Ctrl+C), cleanup the server and close the app
-
-	Args:
-		app (QtCore.QCoreApplication): The app in which the server is running
-		run_queue_server (RunQueueServer): The runqueue-server instance
-	"""
-	log.info("Received shutdown signal, now attempting to cleaning up server and close app")
-	run_queue_server.terminate() #Disconnect all, stop running and save progress
-	app.quit()
-	
-	log.info("Server cleanup complete, exiting")
-
-def server(
-			target_function : typing.Callable,
-			workspace_path : str = "",
-			run_queue_n_processes : int = 1,
-			password : str = "",
-			hostname : str = "localhost",
-			port : int = 5454,
-			log_level : int = logging.INFO,
-			run_queue_kwargs : typing.Optional[typing.Dict[str, typing.Any]] = None
-		):
-	"""
-	WARNING: RUNNING A SERVER ALLOWS OTHER MACHINES ON THIS NETWORK TO EXECUTE ARBITRARY CODE IF THEY KNOW THE PASSWORD
-	PLEASE RUN THIS IN A TRUSTED NETWORK ENVIRONEMENT. Run at your own risk.
-
-	Convenience function that constructs a local instance of the runqueue-server with the specified target function.
-	It then runs the server in a QtCore app.
-
-	Args:
-		target_function (typing.Callable): The target function on which tasks will be run, this function should take
-			a configuration as the first argument, and the rest of the arguments should be the arguments passed to the
-			```RunQueue._process_queue_item()```-method.
-
-		workspace_path (str, optional): The path to the workspace folder. Attempts to load progress from here, also saves
-			progress to here. Defaults to "". If empty/default, the default workspace folder is used (~/Configurun-server/)
-
-		run_queue_n_processes (int, optional): The number of processes to use in the run queue. Defaults to 1.
-
-		run_queue_kwargs (typing.Dict[str, typing.Any], optional): The keyword arguments passed to the
-			RunQueue constructor. Defaults to {}.
-			Possible kwargs:
-				log_location (str) : The path where the log file should be outputted (should be a folder)
-					if blank, use default location using TEMP folder
-	"""
-	#=========== Initialize logger ===========
-	formatter = logging.Formatter("[{pathname:>90s}:{lineno:<4}]  {levelname:<7s}   {message}", style='{')
-	handler = logging.StreamHandler()
-	handler.setFormatter(formatter)
-	logging.basicConfig(
-		handlers=[handler],
-		level=log_level) #Without time
-	root_logger = logging.getLogger()
-	root_logger.setLevel(log_level)
-
-
-
-	if run_queue_kwargs is None:
-		run_queue_kwargs = {}
-
-	assert len(password) > 0, "Password for server cannot be empty"
-
-	if workspace_path == "" or workspace_path is None:
-		workspace_path = os.path.join(os.path.expanduser("~"), APP_NAME+"-Server")
-		log.info(f"No workspace path provided, using default: {workspace_path}")
-
-	os.makedirs(workspace_path, exist_ok=True) #Create the workspace folder if it does not exist yet
-	QtCore.QDir.setCurrent(workspace_path) #Set the current working directory to the workspace path
-
-
-	runqueue = RunQueue(
-		target_function=target_function,
-		n_processes=run_queue_n_processes,
-		log_location=os.path.join(workspace_path, "logs"),
-		**run_queue_kwargs
-	)
-
-	run_queue_server = RunQueueServer(
-			run_queue=runqueue,
-			password=password,
-			hostname=hostname,
-			port=port,
-			workspace_path=workspace_path
-	)
-
-	app = QtCore.QCoreApplication(sys.argv) #Run the main event-loop (used for signals)
-	#Create a runqueue client to run the runqueue in
-	run_queue_server.run()
-	log.info("Server started, listening for client connections...")
-
-	timer = QtCore.QTimer()
-	timer.start(500)
-	timer.timeout.connect(lambda: None)  # Let the interpreter run each 500 ms to catch signals
-	signal.signal(signal.SIGINT, lambda *_: _cleanup_server(app, run_queue_server)) #Cleanup on Ctrl+C
-	app.exec()
-
-
-def client(
+def run_client(
 			options_source : \
 				typing.Callable[[Configuration], typing.Dict[str, typing.Type[BaseOptions] | typing.Type[None]]] | \
 				argparse.ArgumentParser | \
 				typing.Type[BaseOptions],
 			workspace_path : str = "",
 			create_workspace_path : bool = True, #Whether to create the workspace path if it does not exist
 			log_level : int = logging.INFO,
 			config_model_kwargs : typing.Optional[typing.Dict[str, typing.Any]] = None,
 		):
 
 	"""
-	options_source (typing.Callable[[Configuration], typing.Dict[str, typing.Type[BaseOptions]
-			|  typing.Type[None]]]
-			|, optional):
-		The source of the options in the ui. This can either be:
-			- A function returning a dict of option (dataclass) objects,
-			- A single BaseOptions object
-			- An argparse.ArgumentParser object
-		Defaults to None.
-	
-	workspace_path (str, optional): The path to the workspace folder. Attempts to load progress from here, also saves
-		configs/logs/settings to here. Defaults to "". If empty/default, the default workspace folder is used
-		(~/Configurun-Client/)
-
-	create_workspace_path (bool, optional): Whether to create the workspace path if it does not exist.
-		Defaults to True.
-
-	config_model_kwargs (typing.Dict[str, typing.Any], optional): The keyword arguments passed to the
-		ConfigurationModel constructor. Defaults to {}.
-		E.g.:
-		- use_cache (bool): Whether to use the cache or not to temporarily save configurations. This makes it so
-			option-group settings are remembered when switching back/forth (for example between 2 model-options).
-			Defaults to True. If true undo_stack is also used
-		- use_undo_stack (bool): Whether to use the undo stack or not. Defaults to True
-	
-	log_level (int, optional): The log level to use. Defaults to logging.INFO
+	Convenience function that creates and runs a client instance of the app with the specified option source. 
+	Differs from local_app in that no target_function is provided as this should be provided on the server-side.
+	Workspace path is optional, if none is provided, uses '~/Configurun/'.
+
+	Args:
+		options_source (typing.Callable[[Configuration], typing.Dict[str, typing.Type[BaseOptions]
+				|  typing.Type[None]]]
+				|, optional):
+			The source of the options in the ui. This can either be:
+				- A function returning a dict of option (dataclass) objects,
+				- A single BaseOptions object
+				- An argparse.ArgumentParser object
+			Defaults to None.
+
+		workspace_path (str, optional): The path to the workspace folder. Attempts to load progress from here, also saves
+			configs/logs/settings to here. Defaults to "". If empty/default, the default workspace folder is used
+			(~/Configurun-Client/)
+
+		create_workspace_path (bool, optional): Whether to create the workspace path if it does not exist.
+			Defaults to True.
+
+		config_model_kwargs (typing.Dict[str, typing.Any], optional): The keyword arguments passed to the
+			ConfigurationModel constructor. Defaults to {}.
+			E.g.:
+			- use_cache (bool): Whether to use the cache or not to temporarily save configurations. This makes it so
+				option-group settings are remembered when switching back/forth (for example between 2 model-options).
+				Defaults to True. If true undo_stack is also used
+			- use_undo_stack (bool): Whether to use the undo stack or not. Defaults to True
+
+		log_level (int, optional): The log level to use. Defaults to logging.INFO
 	"""
 	#=========== Initialize logger ===========
 	formatter = logging.Formatter("[{pathname:>90s}:{lineno:<4}]  {levelname:<7s}   {message}", style='{')
 	handler = logging.StreamHandler()
 	handler.setFormatter(formatter)
 	logging.basicConfig(
 		handlers=[handler],
@@ -330,32 +233,35 @@
 
 	#Select a config-model, pass the deduce_new_option_class_types function to the constructor
 	config_model = ConfigurationModel(option_type_deduction_function=options_function, **config_model_kwargs)
 
 	#Create the Qt-main window in which the app will be placed
 	main_window = QtWidgets.QMainWindow()
 
-	run_queue_client = RunQueueClient(	
+	run_queue_client = RunQueueClient(
 	)
 
 
 	#Create the actual app
 	NetworkMainWindow(
 		configuration_model=config_model,
 		run_queue_client=run_queue_client,
 		window=main_window,
 		workspace_path=workspace_path,
 	)
 
 	main_window.show() #Show the window
 	app.exec()
+	exit(0)
+
+
 
 if __name__ == "__main__":
 	from configurun.examples.example_configuration import \
 	    example_deduce_new_option_classes
 	from configurun.examples.example_target_function import example_target_function
-	local_app(
+	run_local(
 		target_function=example_target_function,
 		options_source=example_deduce_new_option_classes,
 		run_queue_n_processes=1,
 		log_level=logging.DEBUG
 	)
```

### Comparing `configurun-0.1.0/configurun/examples/example_argparse.py` & `configurun-0.2.0/configurun/examples/example_argparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 	"""
 	Runs an example local app with the example argparse options
 	"""
 	# pylint: disable=import-outside-toplevel
 	import os
 	import tempfile
 
-	from configurun.create import local_app
-	from configurun.windows.main_window import APP_NAME
-	
+	from configurun.app.create_run import run_local
+	from configurun.app.main_window import APP_NAME
+
 	tempdir = tempfile.gettempdir()
 	workspace_path = os.path.join(tempdir, APP_NAME, "Configurun-Argparse-Example")
-	local_app(
+	run_local(
 		target_function = lambda x, *_: print(x),
 		options_source = parser_example,
 		workspace_path=workspace_path
 	)
 
 if __name__ == "__main__":
-	run_argparse_example()
+	run_argparse_example()
```

### Comparing `configurun-0.1.0/configurun/examples/example_configuration.py` & `configurun-0.2.0/configurun/examples/example_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,25 +71,25 @@
 	return ret_dict
 
 
 def run_example_app(log_level=logging.INFO):
 	"""Run an example instance of the Configurun-App using the example run function and example-option-deducer
 	"""
 	# pylint: disable=import-outside-toplevel
-	from configurun.create import \
-	    local_app
+	from configurun.app.create_run import \
+	    run_local
 	import os
-	from configurun.windows.main_window import APP_NAME
+	from configurun.app.main_window import APP_NAME
 	import tempfile
 
 	#=========================== Create the app using the example ===========================
 	tempdir = tempfile.gettempdir()
 	workspace_path = os.path.join(tempdir, APP_NAME, "Configurun-Local-Example")
 	log.info(f"Saving example app workspace to {workspace_path}")
-	local_app(
+	run_local(
 		target_function=example_target_function,
 		options_source=example_deduce_new_option_classes,
 		workspace_path=workspace_path,
 		log_level=log_level
 	)
```

### Comparing `configurun-0.1.0/configurun/examples/example_configuration_sklearn.py` & `configurun-0.2.0/configurun/examples/example_configuration_sklearn.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,25 +52,25 @@
 def run_sklearn_example(log_level : int = logging.INFO):
 	"""
 	Starts the example-app using a dynimically created sklearn-model-options class
 	"""
 	# pylint: disable=import-outside-toplevel
 	import os
 	import tempfile
-	from configurun.create import local_app
+	from configurun.app.create_run import run_local
 	from configurun.examples.example_target_function import example_target_function
-	from configurun.windows.main_window import APP_NAME
+	from configurun.app.main_window import APP_NAME
 	log.info("Starting the example implementation, including Sklearn models")
 	tempdir = tempfile.gettempdir()
 	workspace_path = os.path.join(tempdir, APP_NAME, "Configurun-Sklearn-Example")
-	local_app(
+	run_local(
 		target_function = example_target_function,
 		options_source = SklearnMainOptions,
 		workspace_path=workspace_path,
 		log_level=log_level
 
 	)
 
 
 
 if __name__ == "__main__":
-	run_sklearn_example(log_level=logging.DEBUG)
+	run_sklearn_example(log_level=logging.DEBUG)
```

### Comparing `configurun-0.1.0/configurun/examples/example_options/example_options.py` & `configurun-0.2.0/configurun/examples/example_options/example_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 """
 Implements several option-dataclasses to show how to use this framework.
 """
 import typing
 from dataclasses import dataclass, field
 
-from pyside6_utils.utility.constraints import (Interval, StrOptions)
+from pyside6_utils.classes.constraints import (Interval, StrOptions, ConstrainedList)
 
 from configurun.configuration.base_options import BaseOptions
 
 
 @dataclass
 class ExampleDatasetOptions(BaseOptions):
 	"""Example dataset options
 	"""
 
 	dataset_name : str | None = field(default=None, metadata=dict(
 			display_name="Dataset Name",
 			help="Name of the dataset to be used, is used for logging purposes and keeping track of the results",
 			constraints = [str, None]
+		)
 	)
+
+
+	indexes : typing.List[int] | None = field(
+		default=None,
+		metadata=dict(
+			display_name="Indexes",
+			help="Indexes of the dataset to be used (list of ints > 0)",
+			constraints = [ConstrainedList([Interval(int, 0, None, closed='both')]), None]
+		)
 	)
 
 
 	test_ratio : float = field(
 		default=0,
 		metadata=dict(
 			display_name="Test Ratio",
@@ -81,21 +91,21 @@
 	)
 
 
 
 @dataclass
 class ExtendedExampleDatasetOptions(ExampleDatasetOptions):
 	"""Extends the example dataset options with some more options"""
-	labels : str | None = field(
+	labels : typing.List[str] | None = field(
 		default=None,
 		metadata=dict(
 			display_name="Labels",
 			help=("In case a dataset contains several labels (multi-task), "
 				   "which type of labels should be used in regression or classification, the name of column(s)."),
-			constraints = [str, None] #TODO: list of strings?
+			constraints = [ConstrainedList([str]), None] #TODO: list of strings?
 	))
 	normalization : typing.Literal['standardization', 'minmax', 'per_sample_std', 'per_sample_minmax'] = field(
 		default='standardization',
 		metadata=dict(
 			display_name="Normalization",
 			help="If specified, will apply normalization on the dataset.",
 			display_path="Normalization",
@@ -145,29 +155,28 @@
 		default='',
 		metadata=dict(
 			display_name="Comment",
 			help="A comment/description for this experiment."
 		)
 	)
 
-
-
 	print_interval : int = field(
 		default=1,
 		metadata=dict(
 			display_name="Print Interval",
 			help="Print every x interval"
 		)
 	)
 
-	gpu_index : str =  field(
-		default='0',
+	gpu_indexes : typing.List[int] | None = field(
+		default=None,
 		metadata=dict(
-			display_name="GPU Index",
-			help="GPU index"
+			display_name="GPU indexes",
+			help="Indexes of the videocards to use - None for CPU, -1 for all",
+			constraints = [ConstrainedList([Interval(int, -1, None, closed='both')]), None]
 		)
 	)
 
 	processes : int = field(
 		default=-1,
 		metadata=dict(
 			display_name="Number of processes",
```

### Comparing `configurun-0.1.0/configurun/examples/example_options/example_sklearn_options.py` & `configurun-0.2.0/configurun/examples/example_options/example_sklearn_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import sys
 import typing
 from dataclasses import dataclass, field, make_dataclass
 
 # import dill
 from numpydoc.docscrape import NumpyDocString
-from pyside6_utils.utility.constraints import StrOptions
+from pyside6_utils.classes.constraints import StrOptions
 from sklearn.ensemble import AdaBoostClassifier, RandomForestClassifier
 from sklearn.gaussian_process import GaussianProcessClassifier
 # from sklearn.gaussian_process.kernels import RBF
 from sklearn.linear_model import RidgeClassifierCV
 from sklearn.naive_bayes import GaussianNB
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.neural_network import MLPClassifier
```

### Comparing `configurun-0.1.0/configurun/examples/example_target_function.py` & `configurun-0.2.0/configurun/examples/example_target_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,7 @@
 	log.info("We will now be simulating a task that takes about 20 seconds to complete")
 
 	for i in range(20):
 		log.info(f"Progress: {i}/20")
 		time.sleep(1)
 
 	log.info("Done with the example run function... Now exiting...")
-
```

### Comparing `configurun-0.1.0/configurun/res/app_resources_rc.py` & `configurun-0.2.0/configurun/res/app_resources_rc.py`

 * *Files identical despite different names*

### Comparing `configurun-0.1.0/configurun/windows/main_window.py` & `configurun-0.2.0/configurun/app/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 from configurun.classes.run_queue import \
 	ConfigurationIsFirmException, RunQueue, WORKSPACE_RUN_QUEUE_SAVE_NAME, WorkspaceInUseException
 from configurun.configuration.configuration import Configuration
 from configurun.configuration.configuration_model import (
     ConfigurationModel, NoClassTypesError, OptionTypesMismatch,
     UnkownOptionClassError)
-from configurun.windows.models.run_queue_console_model import \
+from configurun.app.models.run_queue_console_model import \
     RunQueueConsoleModel
-from configurun.windows.models.run_queue_table_model import RunQueueTableModel
-from configurun.windows.ui.main_window_ui import Ui_MainWindow
+from configurun.app.models.run_queue_table_model import RunQueueTableModel
+from configurun.app.ui.main_window_ui import Ui_MainWindow
 
 
 log = logging.getLogger(__name__)
 
 APP_NAME = "Configurun" #The name of the app, used for the settings file
 
 class OptionsSource(Enum):
@@ -263,17 +263,14 @@
 		self.ui.saveCurrentConfigBtn.clicked.connect(self.save_config_triggered)
 		self.ui.OpenFileLocationBtn.clicked.connect(self.open_save_location_in_explorer)
 
 
 		###### Run Queue Actions ########
 		# self.ui.menuRun_Queue.mousePressEvent().triggered.connect(self.ui.runQueueWidget.show)
 		self.ui.menuRun_Queue.aboutToShow.connect(self.expand_run_queue_view_filter_options)
-		# self.ui.actionViewRunQueueFilter.triggered.connect(lambda *_: self.expand_run_queue_view_filter_options())
-		# self.ui.actionViewRunQueueFilter.triggered.connect(lambda *_: print("kaas"))
-		# self.ui.actionBackupRunQueue.triggered.connect(self.runQu
 		self.ui.actionBackupRunQueue.triggered.connect(lambda *_: self.ui.runQueueWidget.save_to_file_popup())
 		self.ui.actionLoadRunQueue.triggered.connect(lambda *_: self.ui.runQueueWidget.load_from_file_popup())
 
 		###### Buttom-config editor buttons ########
 		self.ui.addToQueueButton.clicked.connect(self.add_to_queue_triggered)
 		self.ui.saveToQueueItemBtn.clicked.connect(self.save_to_queue_item_triggered)
 
@@ -615,16 +612,17 @@
 			ignore_modified_window (bool, optional): Whether to ignore the current modified window state. If true,
 				overwrites the current config without asking the user. Defaults to False.
 		"""
 		if self.window.isWindowModified() and not ignore_modified_window:
 			if not self._ask_overwrite_unsaved_changes():
 				return
 
-			self._config_file_picker_model.set_highlight_using_path(self._cur_file_path) #Hightlight path -> original
-			return
+			# self._config_file_picker_model.set_highlight_using_path(self._cur_file_path) #Hightlight path -> original
+			self.set_source(OptionsSource.FILE)
+			self._cur_file_path = None
 
 		self.window.setWindowModified(False)
 		self._cur_file_path = None
 		self._config_file_picker_model.reset_highlight()
 		self._configuration_model.reset_configuration_data_to_default()
 
 	def load_from_file(self,
@@ -747,16 +745,14 @@
 					self._configuration_model.validate_current_configuration()
 				except OptionTypesMismatch as exception:
 					msg = QtWidgets.QMessageBox()
 					msg.setWindowTitle("Warning")
 					msg.setIcon(QtWidgets.QMessageBox.Icon.Warning)
 					msg.setText(f"The loaded configuration from <tt>{new_path}</tt> is not stable.")
 					replaced_exception = str(exception).replace("\n", "<br>")
-					print("kaas", replaced_exception)
-					print("frikandel", exception)
 					msg.setInformativeText((f"<b>{type(exception).__name__}:</b> {replaced_exception}<br><br>"
 			     			"This could be the result of a change in the settings format, the type-deducer, "
 							"the option-names, or due to file corruption. <br>"
 							"You can continue using the configuration, but any changes to the config will overwrite the "
 							" option-subgroup(s) mentioned above.<br>"))
 					msg.setStandardButtons(QtWidgets.QMessageBox.StandardButton.Ok)
 					msg.setDefaultButton(QtWidgets.QMessageBox.StandardButton.Ok)
@@ -953,19 +949,19 @@
 
 def run_example_local_app(log_level : int=logging.INFO):
 	"""Runs the example app"""
 	#pylint: disable=import-outside-toplevel
 	from configurun.examples.example_target_function import example_target_function
 	from configurun.examples.example_configuration import example_deduce_new_option_classes
 	import tempfile
-	from configurun.create import local_app
+	from configurun.app.create_run import run_local
 
 	tempdir = tempfile.gettempdir()
 	workspace_path = os.path.join(tempdir, APP_NAME, "Configurun-Local-Example")
-	local_app(
+	run_local(
 		target_function=example_target_function,
 		options_source=example_deduce_new_option_classes,
 		workspace_path=workspace_path,
 		log_level=log_level
 	)
 
 if __name__ == "__main__":
```

### Comparing `configurun-0.1.0/configurun/windows/models/run_queue_console_model.py` & `configurun-0.2.0/configurun/app/models/run_queue_console_model.py`

 * *Files identical despite different names*

### Comparing `configurun-0.1.0/configurun/windows/models/run_queue_table_model.py` & `configurun-0.2.0/configurun/app/models/run_queue_table_model.py`

 * *Files identical despite different names*

### Comparing `configurun-0.1.0/configurun/windows/network_main_window.py` & `configurun-0.2.0/configurun/app/network_main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from PySide6 import QtCore, QtGui, QtWidgets
 from pyside6_utils.utility.catch_show_exception_in_popup_decorator import \
     catch_show_exception_in_popup_decorator
 
 from configurun.classes.run_queue_client import RunQueueClient
 from configurun.configuration.configuration_model import ConfigurationModel
-from configurun.windows.main_window import MainWindow
-from configurun.windows.widgets.network_login_widget import NetworkLoginWidget
+from configurun.app.main_window import MainWindow
+from configurun.app.widgets.network_login_widget import NetworkLoginWidget
 
 log = logging.getLogger(__name__)
 
 class NetworkMainWindow(MainWindow):
 	"""
 	The main QT window for this app which provides the user with several tools to edit/manage/run machine learning
 	settings.
@@ -60,14 +60,15 @@
 			window=window,
 			workspace_path=workspace_path,
 			settings_in_workspace_path=settings_in_workspace_path
 		)
 
 		# assert(type(self._run_queue) == RunQueueClient) #Make sure we're using the right type of queue
 		self._run_queue : RunQueueClient = self._run_queue #For Type hinting
+		assert(isinstance(self._run_queue, RunQueueClient)) #Make sure we're using the right type of queue
 
 		#=================== Network UI ======================
 		self.reconnect_button_1, self._task_queue_overlay_msg = self.get_connection_overlay_ui()
 		self.reconnect_button_2, self._console_overlay_msg = self.get_connection_overlay_ui()
 
 
 		self.ml_overlay_widget = self.ui.runQueueOverlayWidget
@@ -205,22 +206,22 @@
 	Runs an example-client that can connect to a running server. Uses the example_deduce_new_option_classes to
 	generate example options for the client
 	"""
 
 	#pylint: disable=import-outside-toplevel
 	import os
 	import tempfile
-	from configurun.create import client
+	from configurun.app.create_run import run_client
 	from configurun.examples import example_deduce_new_option_classes
-	from configurun.windows.main_window import APP_NAME
+	from configurun.app.main_window import APP_NAME
 
 	tempdir = tempfile.gettempdir()
 	workspace_path = os.path.join(tempdir, APP_NAME, "Configurun-Client-App-Example")
 
-	client(
+	run_client(
 		options_source=example_deduce_new_option_classes,
 		workspace_path=workspace_path,
 		log_level=log_level
 	)
 
 
 if __name__ == "__main__":
```

### Comparing `configurun-0.1.0/configurun/windows/ui/main_window_ui.py` & `configurun-0.2.0/configurun/app/ui/main_window_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     QPainter, QPalette, QPixmap, QRadialGradient,
     QTransform)
 from PySide6.QtWidgets import (QApplication, QDockWidget, QGridLayout, QHBoxLayout,
     QHeaderView, QMainWindow, QMenu, QMenuBar,
     QPushButton, QSizePolicy, QStatusBar, QToolButton,
     QUndoView, QVBoxLayout, QWidget)
 
-from configurun.windows.widgets.run_queue_widget import RunQueueWidget
+from configurun.app.widgets.run_queue_widget import RunQueueWidget
 from pyside6_utils.widgets.console_widget import ConsoleWidget
 from pyside6_utils.widgets.extended_mdi_area import ExtendedMdiArea
 from pyside6_utils.widgets.file_explorer_view import FileExplorerView
 from pyside6_utils.widgets.overlay_widget import OverlayWidget
 from pyside6_utils.widgets.square_frame import SquareFrame
 import configurun.res.app_resources_rc
```

### Comparing `configurun-0.1.0/configurun/windows/ui/network_login_widget_ui.py` & `configurun-0.2.0/configurun/app/ui/network_login_widget_ui.py`

 * *Files identical despite different names*

### Comparing `configurun-0.1.0/configurun/windows/ui/run_queue_widget_ui.py` & `configurun-0.2.0/configurun/app/ui/run_queue_widget_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     QFont, QFontDatabase, QGradient, QIcon,
     QImage, QKeySequence, QLinearGradient, QPainter,
     QPalette, QPixmap, QRadialGradient, QTransform)
 from PySide6.QtWidgets import (QApplication, QHBoxLayout, QHeaderView, QPushButton,
     QSizePolicy, QSpacerItem, QToolButton, QVBoxLayout,
     QWidget)
 
-from configurun.windows.views.run_queue_tree_view import RunQueueTreeView
+from configurun.app.views.run_queue_tree_view import RunQueueTreeView
 from pyside6_utils.widgets.square_frame import SquareFrame
 import configurun.res.app_resources_rc
 
 class Ui_RunQueueWidget(object):
     def setupUi(self, RunQueueWidget):
         if not RunQueueWidget.objectName():
             RunQueueWidget.setObjectName(u"RunQueueWidget")
```

### Comparing `configurun-0.1.0/configurun/windows/views/run_queue_tree_view.py` & `configurun-0.2.0/configurun/app/views/run_queue_tree_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import typing
 
 from PySide6 import QtCore, QtWidgets
 from pyside6_utils.models import ExtendedSortFilterProxyModel
 
 from configurun.classes.run_queue import (RunQueue, RunQueueItemActions,
                                           RunQueueItemStatus)
-from configurun.windows.models.run_queue_table_model import RunQueueTableModel
+from configurun.app.models.run_queue_table_model import RunQueueTableModel
 
 log = logging.getLogger(__name__)
 
 class RunQueueTreeView(QtWidgets.QTreeView):
 	"""
 	Treeview-equivalent used for run-queue items (MLQueueItems)
 	"""
```

### Comparing `configurun-0.1.0/configurun/windows/widgets/network_login_widget.py` & `configurun-0.2.0/configurun/app/widgets/network_login_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Implements a widget for logging in to a server
 """
 
 
 from PySide6 import QtCore, QtWidgets
 
-from configurun.windows.ui.network_login_widget_ui import Ui_NetworkLoginWidget
+from configurun.app.ui.network_login_widget_ui import Ui_NetworkLoginWidget
 
 
 
 class NetworkLoginWidget(QtWidgets.QWidget):
 	"""A widget to control connection to a server:
 		Input-fields: IP, port, password
 		Buttons: connect, disconnect, cancel
```

### Comparing `configurun-0.1.0/configurun/windows/widgets/run_queue_widget.py` & `configurun-0.2.0/configurun/app/widgets/run_queue_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import logging
 
 from PySide6 import QtCore, QtGui, QtWidgets
 from pyside6_utils.utility.catch_show_exception_in_popup_decorator import \
     catch_show_exception_in_popup_decorator
 
 from configurun.classes.run_queue import RunQueueItemActions
-from configurun.windows.models.run_queue_table_model import RunQueueTableModel
-from configurun.windows.ui.run_queue_widget_ui import Ui_RunQueueWidget
+from configurun.app.models.run_queue_table_model import RunQueueTableModel
+from configurun.app.ui.run_queue_widget_ui import Ui_RunQueueWidget
 from configurun.classes.run_queue import RunQueueItemStatus
 
 log = logging.getLogger(__name__)
 
 
 
 class RunQueueWidget(QtWidgets.QWidget):
```

### Comparing `configurun-0.1.0/configurun.egg-info/PKG-INFO` & `configurun-0.2.0/configurun.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: configurun
-Version: 0.1.0
+Version: 0.2.0
 Summary: PySide6 based user-interface tools to create and manage machine learning training/testing-configurations and run them automatically and/or remotely..
 Home-page: https://github.com/Woutah/configurun
 Author: Wouter Stokman
 License: LGPLv2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Configurun
-Configurun is a cross-platform PySide6-based package that implements an application for managing, creating and (remotely) running python configurations. 
-It was designed mainly with machine-learning tasks in mind, but can be used for any python script that takes arguments as an input. The editor-UI is created automatically using either an `argparse.Argumentparser` or python-`@dataclass`(es).
 
+Configurun is a cross-platform PySide6-based package that implements an application for managing, creating and (remotely) running python configurations.
+It was designed mainly with machine-learning tasks in mind, but can be used for any python script that takes arguments as an input. The editor-UI is created automatically using either an `argparse.Argumentparser` or python-`@dataclass`(es).
 
 The Configurun-app is especially useful for scripts/experiments that require a lot of arguments to be tweaked across many experiment-runs. It also makes the process of running experiments remotely much easier by enabling the user to edit, add and schedule tasks on any running Configurun server-instance reachable via a network connection.
 
 This package was created in tandem with [pyside6-utils](https://github.com/Woutah/pyside6-utils/).
 
-
 <p align="center">
 	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/main_window_example.png" width="1200" />
 </p>
 
 # Table of contents
+
 - [Configurun](#configurun)
 - [Table of contents](#table-of-contents)
 - [Features](#features)
 	- [Configuration Editor](#configuration-editor)
 	- [Run Queue](#run-queue)
 	- [Remote-processing](#remote-processing)
 - [Installation](#installation)
@@ -37,202 +37,237 @@
 - [Option-source](#option-source)
 	- [Custom Options (`@dataclass`)](#custom-options-dataclass)
 	- [Custom Options (`ArgumentParser`)](#custom-options-argumentparser)
 	- [Custom Options (`Callable`)](#custom-options-callable)
 - [Target Function](#target-function)
 - [Configuration](#configuration)
 - [Option metadata](#option-metadata)
-
+- [SSH-tunneling](#ssh-tunneling)
+	- [No-hop](#no-hop)
+	- [Hopping](#hopping)
 
 # Features
+
 ## Configuration Editor
-The configuration editor allows the user to specify a configuration-template using either (groups of) [`@dataclass`-class](#custom-options-dataclass) or an [`ArgumentParser`-instance](#custom-options-dataclass). The editor will then automatically create a UI based on the provided template. Editors are specifically created for each option-property based on provided template-types (and [extra constraints](#option-metadata)). Help-messages are displayed on hover, required arguments are highlighted when not filled in, etc.
+
+The configuration editor allows the user to specify a configuration-template using either (groups of) [`@dataclass`-class](#custom-options-dataclass) or an [`ArgumentParser`-instance](#custom-options-dataclass). The editor will then automatically create a UI based on the provided template. Editors are specifically created for each option-property based on provided template-types (and [extra constraints](#option-metadata)). 
+Help-messages are displayed on hover, required arguments are highlighted when not filled in, etc.
 <p align="center">
 	<!-- <img src="./configurun/examples/images/configuration_editor_example.png" width="600" /> -->
 	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/configuration_editor_example.png" width="600" />
 </p>
 
+More complex typehints using `List` / `Union` / `Literal` are supported and are automatically built into widgets that allow the user to add/remove items and switch input-types:
+
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./configurun/examples/images/string_float_list_example.png" width=300/> -->
+</p>
+
 We can also define our own [option-source-method](#custom-options-callable) to dynamically create new option-groups based on the current configuration. This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. E.g: only show `ExtendedExampleModel`-options if property `model_type` in `MainOptions` is set to `"ExtendedExampleModel"`. <br>
 
 Configurations can be saved and loaded, a file-explorer view for the current workspace is made available.:
 <p align="center">
 	<!-- <img src="./configurun/examples/images/file_explorer_example.png" width="400" /> -->
 	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/file_explorer_example.png" width="400" />
 </p>
 
 ## Run Queue
-The run-queue window manages the currently running items. This could either be locally when using a [local-app](#local-app), or remotely, when using a [client-app](#client-side) and a [server-instance](#server-side) on which the actual Run-Queue is running. The Run-Queue allows us to add/remove items, pause/resume items, change the queue-order of items, and start autoprocessing, which will automatically start the next item in the queue when the current item is finished. We can set the number of processors as well, to run multiple items in parallel.
+
+The run-queue window manages the currently running items. This could either be locally when using a [local-app](#local-app), or remotely, when using a [client-app](#client-app) and a [server-instance](#server-instance) on which the actual Run-Queue is running. The Run-Queue allows us to add/remove items, pause/resume items, change the queue-order of items, and start autoprocessing, which will automatically start the next item in the queue when the current item is finished. We can set the number of processors as well, to run multiple items in parallel.
 <p align="center">
 	<!-- <img src="./configurun/examples/images/run_queue_example.png" width="1100" /> -->
 	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/run_queue_example.png" width="1100" />
 </p>
 
-Configurations are passed to the user-provided [run-function](#run-function) in separate processes. The stdout/stderr of each of the items is captured and displayed as a selectable console-output-view in the command-line-output window:
+Configurations are passed to the user-provided [target-function](#target-function) in separate processes. The stdout/stderr of each of the items is captured and displayed as a selectable console-output-view in the command-line-output window:
 <p align="center">
 	<!-- <img src="./configurun/examples/images/command_line_output_example.png" width="1100" /> -->
 	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/command_line_output_example.png" width="1100" />
 </p>
 
 ## Remote-processing
-Instead of using the [local-app](#local-app) to manage and run the configurations on your own machine, we can use the [client-app](#client-side) to connect to a [server-instance](#server-side) on a remote machine. The client-app works analogous to the local-app and allows us to create and manage new configuration, but the Run-Queue runs on the connected remote Configurun-server:
+
+Instead of using the [local-app](#local-app) to manage and run the configurations on your own machine, we can use the [client-app](#client-app) to connect to a [server-instance](#server-instance) on a remote machine. The client-app works analogous to the local-app and allows us to create and manage new configuration, but the Run-Queue runs on the connected remote Configurun-server:
 <p align="center">
 	<!-- <img src="./configurun/examples/images/network_login_example.png" width="300" /> -->
 	<img src="https://raw.githubusercontent.com/Woutah/configurun/main/configurun/examples/images/network_login_example.png" width="300" />
 </p>
 
-
 # Installation
+
 This package can downloaded from [this repository](https://github.com/Woutah/configurun), or can be installed directly from PyPi by using pip:
-```bash
+
+``` bash
 pip install configurun
 ```
 
 # How to run?
+
 Creating the app is done via the `configurun.create`-module. We can create 3 different types of apps:
+
 - [**Local app**](#local-app) - For running everything locally on your machine
-- [**Client app**](#client-side) - For running the configurations on a remote machine, connects to a `server`-instance
-- [**Server instance**](#server-side) - Command-line instance that listens to connections from `client`-apps. If login is succesful, accepts control of the `RunQueue` from the `client`-app.
+- [**Client app**](#client-app) - For running the configurations on a remote machine, connects to a `server`-instance
+- [**Server instance**](#server-instance) - Command-line instance that listens to connections from `client`-apps. If login is succesful, accepts control of the `RunQueue` from the `client`-app.
 
 On the client-side, the `options_source` should be set - the template of the settings used to create the [configuration-editor](#configuration-editor).<br>
-On the server/running-machine, the `target_function` should be set - the function that actually runs the task/experiment ([example](#run-function)).<br>
+On the server/running-machine, the `target_function` should be set - the function that actually runs the task/experiment ([example](#target-function)).<br>
 
 ## Local App
+
 A local app is an all-in-one app that can be used to create and run configurations locally on your machine.
 To run the example app, we can either call `run_example_app()` from `configurun.examples` or run the following code to construct the app ourselves:
+
 ```python
 ### This example will run the app with an example configuration
 # Also see `configurun/examples/example_target_function.py`
 # Also see `configurun/examples/example_deduce_new_option_class_types.py`
 import os
-from configurun.create import local_app
+from configurun.app import run_local
 from configurun.examples import example_target_function, example_deduce_new_option_classes
 
 if __name__ == "__main__": #Makes sure bootstrapping process is done when running app
-	local_app( #Create and runs a local configurun app-instance
+	run_local( #Create and runs a local configurun app-instance
 		target_function=example_target_function, #The function that will be called with the configuration
 		options_source=example_deduce_new_option_classes, #Template for UI-optiosn: Callable/@datclass/ArgumentParser
 		workspace_path = os.path.join( #Settings, configs and the Run-Queue will be saved/loaded from/to here
-			os.getcwd(), 
+			os.getcwd(),
 			"LocalExampleWorkspace"
-		) 
+		)
 	)
 ```
-In this example, [`example_target_function`]([./configurun/examples/example_target_function.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_target_function.py)) runs a dummy task that logs to a file for 20 seconds. We can [specify our own run-function](#run-function) to run our own scripts.
+
+In this example, [`example_target_function`](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_target_function.py) runs a dummy task that logs to a file for 20 seconds. We can [specify our own target-function](#target-function) to run our own scripts.
 
 We can [specify our own options source](#option-source) to create our own options-class for the configuration-editor, for example by [using an existing `ArgumentParser`-object.](#custom-options-argumentparser)
+
 ## Client App
+
 We can create a client-app and use it to login to running [server](#server-instance)-instances. We can then use the client-app analogous to the [local-app](#local-app) to create new confiugrations and add/run/manage configurations on the remote machine.<br>
 
 ```python
 # Opens a client-side app that we can use to connect to and control
 # the server-instance
 import os
-from configurun.create import client
+from configurun.app import run_client
 from configurun.examples import example_deduce_new_option_classes
 
 if __name__ == "__main__":
-	client(
+	run_client(
 		options_source=example_deduce_new_option_classes,
 		workspace_path=os.path.join(os.getcwd(), "ClientExampleWorkspace"),
 	)
 ```
 
-
 ## Server-instance
-The server-instance is a command-line app that listens to connections from [`client`](#client-app)-instance(s) to receive new configurations and commands to manage its RunQueue. The actual run-functions are ran on this machine. <br>
+
+The server-instance is a command-line app that listens to connections from [`client`](#client-app)-instance(s) to receive new configurations and commands to manage its RunQueue. The actual target-functions are ran on this machine. <br>
 
 **NOTE:** *after* authentication, `pickle`/`dill` is used to transmit data, which indirectly enables arbitrary code execution on the server-side if the password is known. Please run the server on trusted network environments only. Run at your own risk!
-```python 
+
+```python
 # Opens a server-instance which tries to connect with clients and allows
 # them to add configurations to the queue to be run on this machine
 import os
-from configurun.create import server
+from configurun.server import run_server
 from configurun.examples.example_target_function import example_target_function
 
 if __name__ == "__main__":
 	# WARNING:
 	# THIS ALLOWS OTHER MACHINES THAT RESIDE ON THE SAME NETWORK
-	# TO EXECUTE ARBITRARY CODE ON THIS MACHINE IF THEY KNOW THE 
+	# TO EXECUTE ARBITRARY CODE ON THIS MACHINE IF THEY KNOW THE
 	# PASSWORD. PLEASE RUN IN A TRUSTED NETWORK ENVIRONMENT ONLY
 	# RUN AT YOUR OWN RISK!
-	server(
+	run_server(
 		target_function=example_target_function,
 		workspace_path=os.path.join(os.getcwd(), "ServerExampleWorkspace"),
 		password="password", #Password to connect to the server, make sure to change this!
 		port=5454 #Port to connect to the server, defaults to 5454
 	)
 ```
 
-
 # Option-source
-When creating an app using the `create`-module, we can define a custom source, using the `options_source=...`, so we can construct the UI using our own options. 
+
+When creating an app using the `create`-module, we can define a custom source, using the `options_source=...`, so we can construct the UI using our own options.
 We can use the following types as an options-source:
+
 - [`@dataclass`-object](#custom-options-dataclass)
 - [`ArgumentParser`-object](#custom-options-argumentparser)
 - [`Callable`](#custom-options-callable)
 
 ## Custom Options (`@dataclass`)
-**NOTE:** Using fields results in more control over the final UI, for a more thorough example, please see [this section](#option-metadata) and/or the example implementations in [configurun/examples/example_options/example_options.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
+
+**NOTE:** Using `@dataclass`-fields results in more control over the final UI, for a more thorough example, please see [this section](#option-metadata) and/or the example implementations in [configurun/examples/example_options/example_options.py](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
 
 **NOTE:**  When implementing custom option-classes, don't forget to add the `@dataclass`-decorator, and always inherit from `BaseOptions`
+
+UI-supported type-hints include `str`, `int`, `float`, `datatime`, `typing.Literal`  (and more) and combinations using `typing.List`, `typing.Union` / `|`. For example:
+
 ```python
 import os
+import typing
 from dataclasses import dataclass
 from configurun.configuration.base_options import BaseOptions
-from configurun.create import local_app
+from configurun.app import run_local
 from configurun.examples import example_target_function
 
 
 @dataclass #Don't forget to add this(!) - otherwise the app will not recognize the fields
 class MyCustomOptions(BaseOptions): #Always inherit from BaseOptions (required to run config)
 	simple_int : int = 1
+	complex_property : typing.List[typing.Union[int, str]] | None = None # Union = |-notation
 	# etc...
 
 if __name__ == "__main__":
-	local_app(
+	run_local(
 		target_function=example_target_function,
 		options_source=MyCustomOptions, #Simple: each configuration consists of a single options-class
 		workspace_path = os.path.join(os.getcwd(), "ExampleDataclassOptions")
 	)
 
+
 ```
 
 ## Custom Options (`ArgumentParser`)
-We can use a `ArgumentParser`-object as an options source, this will internally convert the argument parser into a `@dataclass`-object, which is then used as an options-class. Certain arguments are also parsed to control the UI (e.g. `required=True`, `help="Will be displayed on hover"`).
+
+We can use a `ArgumentParser`-object as an options source, this will internally convert the argument parser into a `@dataclass`-object, which is then used as an options-class. Whenever possible, arguments are also parsed to the UI (e.g. `required=True`, `help="Will be displayed on hover"` etc.).
+
 ```python
 import argparse
 import os
-from configurun.create import local_app
+from configurun.app import run_local
 from configurun.examples import example_target_function
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--required_arg", type=str, required=True, help="Required argument help")
 #... add more arguments here
 
 if __name__ == "__main__":
-	local_app(
+	run_local(
 		target_function=example_target_function,
 		options_source=parser, #Parser is converted internally to a dataclass-class which is used as the options-class
 		workspace_path = os.path.join(os.getcwd(), "ExampleArgparseOptions")
 	)
 ```
-## Custom Options (`Callable`)
-A configuration is a collection of option-instances, which are grouped toghether in a `Configuration`-wrapper, which enables us to access the attributes of all enclosed options-instances using the `configuration[attribute]`/`configuration.<attribute>`/`option_class.get(attribute, default)`. For more information, see [this section](#configuration).
 
+## Custom Options (`Callable`)
 We define an `option`-class as a class that has the `@decorator` and inherits from the `BaseOptions`-class.
 
-As an options-source, we can create a callable which takes the current Configuration-instance as an argument and returns 1 or more new options-classes (***not** instances*) which is called every time a setting is changed. If the types-change, the UI will be updated to reflect the new templates. 
+A configuration is a collection of option-instances, which are grouped toghether in a [`Configuration()`](#configuration)-wrapper, which enables us to access the attributes of all enclosed options-instances using the `configuration[attribute]` / `configuration.<attribute>` / `option_class.get(attribute, default)`. For more information, see [this section](#configuration).
+
+As an options-source, we can create a callable which takes the current Configuration-instance as an argument and returns 1 or more new options-classes (***not** instances*) which is called every time a setting is changed. If the types-change, the UI will be updated to reflect the new templates.
 This can be useful if we want to group options together, and only show certain groups when an attribute of another group is set to a certain value. For example:
+
 ```python
-#In this example, we will create a callable which returns new options-classes based on the 
+#In this example, we will create a callable which returns new options-classes based on the
 # current configuration
 import os
 import typing
 from dataclasses import dataclass
-from configurun.create import local_app
+from configurun.app import run_local
 from configurun.examples import example_target_function
 from configurun.configuration import BaseOptions, Configuration
 
 @dataclass #NOTE: Always use @dataclass for options
 class AlwaysTheSame(BaseOptions): #NOTE: Always use BaseOptions as base class for options
 	base_int : int = 1
 	#...
@@ -245,74 +280,88 @@
 @dataclass
 class CustomOptionsUnderConditions(BaseOptions):
 	simple_int : int = 2
 	some_more_options : str = 'Some string'
 	#...
 
 def deduce_new_option_classes(configuration: Configuration)\
-		-> typing.Dict[str, typing.Type[BaseOptions | None]]: #Always return a dict of option 
+		-> typing.Dict[str, typing.Type[BaseOptions | None]]: #Always return a dict of option
 	 		# classes the key of the dict is the name/group of the option-class
-			# the value is the option-class (@dataclass & BaseOptions) itself 
+			# the value is the option-class (@dataclass & BaseOptions) itself
 	if configuration.options is None or len(configuration.options) == 0:
 		pass #If initial configuration is being retrieved -> return default dict
 	elif configuration.base_int == 2 and configuration.simple_int != 1:
 		#Only return the CustomOptionsUnderConditions-class when base_int == 2 & simple_int != 1
 		#NOTE: if we're not sure if attributes exist, we can use the `.get(key, default)` method
 		return { #UI will be built using the following option-classes, each key gets a tab/window:
 			'always_the_same' : AlwaysTheSame,
 			'custom_options' : CustomOptionsUnderConditions
 		}
-	
+
 	return { #UI will be built using the following option-classes, each key gets a tab/window:
 		'always_the_same' : AlwaysTheSame,
 		'custom_options' : CustomOptionsDefault
 	} #NOTE: we must ALWAYS return a dictionary with at least 1 option class
 
 if __name__ == '__main__':
-	local_app(
+	run_local(
 		target_function=example_target_function,
 		options_source=deduce_new_option_classes,
 		workspace_path = os.path.join(os.getcwd(), "ExampleCallableOptions")
 	)
 
 ```
 
-
-
 # Target Function
+
 The target function is the function that does all the work. This is the function that is being called when an item starts "running" in the Run-Queue.
-It takes a single argument: a [`Configuration`-instance](#configuration) - instance.
-The configuration-object contains all settings as set by the user when "add to queue" was pressed.
+It takes a single argument: a [`Configuration`-instance](#configuration).
+The configuration-object contains all settings as set by the user when "add to queue" was pressed. 
+
+This example uses the example-configuration from [the Configuration section](#configuration), we simply print the values of the configuration to the console:
 
-This example uses the example-configuration from [the Configurtion section](#configuration), we simply print the values of the configuration to the console:
 ```python
 def target_function(configuration: Configuration):
 	#Do something with the configuration
 	print(configuration.simple_int)
 	print(configuration.some_other_int)
 	#etc.
 ```
 
-If you have replaced an `argparse.Argumentparser` in the previous example, this is the place where you insert the user-provided settings to the script that uses the `ArgumentParser`-object. For example:
+If you have replaced an `argparse.Argumentparser`, this is the place where you insert the user-provided settings to the script that uses the `ArgumentParser`-object. For example:
+
 ```python
 # parsed_args = parser.parse_args() #will be done by user in UI
 # your_framework_that_used_parsed_args(parsed_args) #Will be called in target_function
 
 def target_function(configurtion : Configuration):
-	# Since we can use the Configuration-instance as a dict 
+	# Since we can use the Configuration-instance as a dict
 	# and as configuration.<attribute> we can just
 	# pass it to the framework compatible with the ArgumentParser:
 	your_framework_that_used_parsed_args(configuration)
+```
+
+Of course you can also directly pass the `your_framework_that_used_parsed_args(...)`-function as the target function when creating the app:
 
+```python
+if __name__ == '__main__':
+	local_app(
+		target_function=your_framework_that_used_parsed_args,
+		options_source=deduce_new_option_classes,
+		workspace_path = os.path.join(os.getcwd(), "ExampleCallableOptions")
+	)
 ```
 
+This example uses the `deduce_new_option_classes`-function from [callable option source example](#custom-options-callable) .
+
 # Configuration
+
 Configurun works with `configuration`-objects. A configuration is a collection of option-instances (=`@dataclass`-instances that inherit from `BaseOptions`), which are grouped toghether in a `Configuration`-wrapper.
 We can think of the option-instances as the different groups of options we want to edit and use in our run (e.g. `GeneralOptions()`, `LogOptions()`, `ModelOptions()`, etc.).
-In the simplest case, we have 1 single option-instance which contains all the options, `AllOptions()`. 
+In the simplest case, we have 1 single option-instance which contains all the options, for example: `AllOptions()`.
 
 The `Configuration`-wrapper enables us to access the attributes of all enclosed options-instances using `configuration[attribute]`/`configuration.<attribute>`/`option_class.get(attribute, default)`.
 
 An example of how to use a `Configuration`-instance:
 
 ``` python
 from dataclasses import dataclass
@@ -326,81 +375,122 @@
 
 @dataclass
 class OtherOptionClass(BaseOptions):
 	some_other_int : int = 2
 	#etc.
 
 
+# Normally, the following would be done by the app using the UI
+# input and/or the user-provided option-source
 config = Configuration()
 config.options['general_options'] = GeneralOptionsClass()
 config.options['other_options'] = OtherOptionClass()
 
 #Accessing the options, all of the following are equivalent:
 print(config['simple_int'])
 print(config.simple_int)
-print(config.get('simple_int', -1)))
+print(config.get('simple_int', -1))) #Would return -1 if key-error occurs
 
 #These are also equivalent:
 print(config['some_other_int'])
 print(config.some_other_int)
 print(config.get('some_other_int', -1)))
 
 # Note that we can use the config.<attr>-notation to our advantage
 # when we want to use autocomplete in our editor. For example:
 # def target_function(configuration: GeneralOptionsClass)
 # Would result in our editor of choice recognizing/autocompleting
 # the `configuration.simple_hint` way of accessing `simple_hint`
 ```
 
-
-
 # Option metadata
-The UI is mainly built around the [`field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.field) functionality of python-`dataclass`, which allows the display-model to make use of the default values, type hints and other information. 
-For each attribute in our `option`-definition, we can provide additional information in the `metadata` attribute of `field()`. This provides additional information to the UI, which is used to determine the editor-type, constraints etc. <br>
+
+The UI is mainly built around the [`field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.field) functionality of python-`dataclass`, which allows the display-model to make use of the default values, type hints and other information.
+While typehints (e.g. `int`, `str`, `typing.List[int]`, etc.) are enough to create the editors, we can also provide additional information in the `metadata`-attribute of `field()` to further constrain the editors and provide additional information to the user. <br>
 
 For example:
+
 ```python
 from configurun.configuration import base_options
 from dataclasses import field, dataclass
 #Used to constrain the editors: (can also be imported from sklearn)
-from pyside6_utils.utility.constraints import Interval 
+from pyside6_utils.classes.constraints import Interval, ConstrainedList
 
 @dataclass
 class TestOptions(BaseOptions):
-	test_int_property : int | None = field(
+	test_int_list_property : typing.List[int] | None = field(
 		default=None, #The default value used in the UI
 		metadata=dict( #Contains additional information for the UI
 			display_name="Test property", #The display-name
 			help="This is a test property that can also be none", #On-hover help-messagem
 			required=True, #If required, the field is red if not filled in
 			constraints = [ #Limit editors (min/max, options, etc.)
 				#The following constrains the editor to have value > 1
-				Interval(type=int, left=1, right=None, closed="both"), 
+				ConstrainedList([Interval(type=int, left=1, right=None, closed="both")]),
 				None #Or value can be None
-			] 
+			]
 			# etc...
 		)
 )
 ```
-For more examples, please see the [example-options](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py). 
+
+For more examples, please see the [example-options](https://github.com/Woutah/configurun/blob/main/configurun/examples/example_options/example_options.py).
 
 The following metadata-keys are supported:
 
 | Metadata Key | Type | Description |
 | --- | --- | --- |
 | `"display_name"` | `str` | Name to display for this attribute in the view - defaults to the variable name itself |
-| `"display_path"` | `str` | Path to display this attribute - we can group/structure items. If parent does not exist, creates folders. Format as "|
+| `"display_path"` | `str` | Path to display this attribute - we can group/structure items when using a treeview - defaults to no parents|
 | `"help"` | `str` | Help-message which will be shown when the user hovers over this item - empty by default|
-| `"constraints"` | `List[constraint]` | Additional constraints on which the editor will be determined to apply to the field**, if none provided, use typehint of the field|
+| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [*](#constraintnote) , if none provided, use typehint of the field|
 | `"required"` | `bool` | Whether this field is required to be filled in - if true - a red background will appear if the value is not set|
 | `"editable"` | `bool` | Whether this field is editable - if false - the editor will be disabled|
 
-**: Constraints are sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into the [pyside6-utils](https://github.com/Woutah/pyside6-utils) package under [`utility.constraints`](https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/utility/constraints.py). The following constraints are supported:
+<a name="constraintnote">*=</a>Constraints are (almost entirely) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `classes.constraints`. The following constraints are supported:
 | Constraint | Description | Editor Type
 | --- | --- | --- |
 | `type` | The type of the value should match the type of the constraint | based on type |
 | `Options` / `Container` | The value should be one of the options provided in the constraint | `QComboBox` |
 | `StrOptions` | The value should be one of the str-options provided in the constraint | `QComboBox` |
 | `Interval` | The value should be within the interval provided in the constraint | `QSpinBox` or `QDoubleSpinBox` (limited) |
-| `None` | `None` is a valid value for this field (same as `typing.Optional`) | Adds reset-button to editor |
+| `None` | `None` is a valid value for this field, same as `typing.Optional` | Adds reset-button to editor |
 | `Range` | The value should be within the range provided in the constraint | `QSpinBox` (limited) |
+| `ConstrainedList` | [*(Custom - not part of Sklearn)](#constrainedlist) Indicates a list of of values of a constrained type | Based on type of list |
+
+<a name="constrainedlist">*=</a>For example, `ConstrainedList([Interval(float, 0.0, 1.0), StrOptions(["string1", "string2"])])` indicates a list of values that should either be a float between 0.0 and 1.0, or the string "string1" or "string2". The editor for this field would be constructed as a `WidgetList` to which the user can add `WidgetSwitcher`. The `WidgetSwitcher` would then have two widgets, one with a `QSpinBox` and one with a `QComboBox` as the editor. **NOTE:** the same editor would be parsed from a `Typing.List[typing.Union[float, Typing.Literal["string1", "string2"]]]` typehint, minus the bounded-interval constraint on the float:
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/string_float_list_example.png" width=300/> -->
+</p>
+
+# SSH-tunneling
+
+This section contains a quick tutorial on how to use SSH-tunnels to connect to a remote server-instance in case we're not running client and server on the same machine/network.
+
+## No-hop
+
+A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without opening up any ports on the server-side.
+If we can directly SSH into the target machine, we can connect the ports as follows (assuming we're using the default `5454`-port in both the server and client configuration):
+
+```bash
+ssh -L 5454:localhost:5454 user@remote_host
+```
+
+On the client-side, we can then connect to the server-instance by using `localhost:5454` as the host and the password we set in the server-instance.
+
+## Hopping
+
+If we cannot directly access the remote-machine, we can use a 2-step SSH-tunnel to connect to the server-instance.
+This example assumes we have:
+
+- `remote1`: directly accessible from our machine
+- `remote2`: only accessible from `remote1`
+- Using default Configurun-port `5454` on both the client and server-side
+
+We can then connect to `remote2` from our machine using the following command:
+
+```bash
+ssh -L 5454:localhost:61521 <username>@<remote1-ip> ssh -L 61521:localhost:5454 -N <remote2-ip>
+```
 
+This example forwards `localhost:5454`->`remote1:61521`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
```

### Comparing `configurun-0.1.0/setup.py` & `configurun-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+"""The setup script."""
 from setuptools import setup, find_packages
 
+
 setup(
 	name = "configurun",
-	version= "0.1.0",
+	version= "0.2.0",
 	packages=find_packages('.'),
-    description="PySide6 based user-interface tools to create and manage machine learning training/testing-configurations and run them automatically and/or remotely..",
-    long_description=open('README.md').read(),
+    description=("PySide6 based user-interface tools to create and manage machine learning "
+                 "training/testing-configurations and run them automatically and/or remotely.."),
+    long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author="Wouter Stokman",
     url="https://github.com/Woutah/configurun",
     license="LGPLv2",
     include_package_data=True,
     install_requires=[ #Generated using pipreqs
         'PySide6>=6.0.0', # Qt for Python, works for 6.5.1.1
         'pathos>=0.3.0', #Works for 0.3.0
         'setuptools>=65.0.0', #Works for 65.5.0
 		'dill>=0.3.0', #Works for 0.3.6
 		'multiprocess>=0.70.00', #Works for 0.70.14
 		'numpydoc>=1.4.0', #Works for 1.5.0
 		'pycryptodome>=3.10.0', #Works for 3.18.0
-        'pyside6-utils==1.1.0'
+        'pyside6-utils==1.2.0',
+        'PySignal>=1.1.1' #Works for 1.1.1,
 	]
-)
+)
```

