# Comparing `tmp/pyside6_utils-1.1.0.tar.gz` & `tmp/pyside6_utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside6_utils-1.1.0.tar", last modified: Thu Jun 29 01:30:36 2023, max compression
+gzip compressed data, was "pyside6_utils-1.2.0.tar", last modified: Tue Jul  4 18:59:59 2023, max compression
```

## Comparing `pyside6_utils-1.1.0.tar` & `pyside6_utils-1.2.0.tar`

### file list

```diff
@@ -1,73 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.992275 pyside6_utils-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-06-29 01:30:36.992275 pyside6_utils-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.980275 pyside6_utils-1.1.0/pyside6_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.980275 pyside6_utils-1.1.0/pyside6_utils/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/examples/example_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/examples/run_qt_designer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/examples/run_widgets_example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.980275 pyside6_utils-1.1.0/pyside6_utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1090754 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/icons/app_resources_rc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.984275 pyside6_utils-1.1.0/pyside6_utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.984275 pyside6_utils-1.1.0/pyside6_utils/models/console_widget_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/console_widget_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/console_widget_models/console_from_file_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/console_widget_models/console_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/dataclass_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/dataclass_tree_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/extended_sort_filter_proxy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/file_explorer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/models/pandas_table_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.988275 pyside6_utils-1.1.0/pyside6_utils/registrars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/register_collapsible_group_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/register_console_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/register_extended_mdi_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/register_file_explorer_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/register_overlay_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/register_pandas_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/register_range_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/registrars/register_square_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.988275 pyside6_utils-1.1.0/pyside6_utils/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/ui/ConsoleWidget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/ui/FramelessMdiWindow_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/ui/allWidgets_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.988275 pyside6_utils-1.1.0/pyside6_utils/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/utility/catch_show_exception_in_popup_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27499 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/utility/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/utility/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/utility/signal_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/utility/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.992275 pyside6_utils-1.1.0/pyside6_utils/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/collapsible_group_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/console_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/dataclass_tree_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.992275 pyside6_utils-1.1.0/pyside6_utils/widgets/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/delegates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/delegates/console_widget_delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/delegates/dataclass_editors_delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/extended_mdi_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/file_explorer_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/frameless_mdi_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/overlay_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/pandas_table_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    20274 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/range_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/pyside6_utils/widgets/square_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:30:36.980275 pyside6_utils-1.1.0/pyside6_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-06-29 01:30:36.000000 pyside6_utils-1.1.0/pyside6_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-29 01:30:36.000000 pyside6_utils-1.1.0/pyside6_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:30:36.000000 pyside6_utils-1.1.0/pyside6_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 01:30:36.000000 pyside6_utils-1.1.0/pyside6_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 01:30:36.000000 pyside6_utils-1.1.0/pyside6_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:30:36.992275 pyside6_utils-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-29 01:30:22.000000 pyside6_utils-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.967009 pyside6_utils-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-04 18:59:59.967009 pyside6_utils-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.951009 pyside6_utils-1.2.0/pyside6_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.955009 pyside6_utils-1.2.0/pyside6_utils/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31714 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/classes/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/classes/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.955009 pyside6_utils-1.2.0/pyside6_utils/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/examples/example_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/examples/run_qt_designer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/examples/run_widgets_example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.955009 pyside6_utils-1.2.0/pyside6_utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1090754 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/icons/app_resources_rc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.959009 pyside6_utils-1.2.0/pyside6_utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.959009 pyside6_utils-1.2.0/pyside6_utils/models/console_widget_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/console_widget_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/console_widget_models/console_from_file_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/console_widget_models/console_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20865 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/dataclass_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/dataclass_tree_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/extended_sort_filter_proxy_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/file_explorer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/models/pandas_table_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.963009 pyside6_utils-1.2.0/pyside6_utils/registrars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_collapsible_group_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_console_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_extended_mdi_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_file_explorer_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_overlay_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_pandas_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_range_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_square_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_widget_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/registrars/register_widget_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.963009 pyside6_utils-1.2.0/pyside6_utils/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/ui/ConsoleWidget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/ui/FramelessMdiWindow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/ui/allWidgets_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.963009 pyside6_utils-1.2.0/pyside6_utils/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/utility/catch_show_exception_in_popup_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/utility/signal_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/utility/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.967009 pyside6_utils-1.2.0/pyside6_utils/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/collapsible_group_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/console_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/dataclass_tree_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.967009 pyside6_utils-1.2.0/pyside6_utils/widgets/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/delegates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/delegates/console_widget_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/delegates/dataclass_editors_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/extended_mdi_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/file_explorer_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/frameless_mdi_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/overlay_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/pandas_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20274 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/range_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/square_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/widget_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/pyside6_utils/widgets/widget_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:59:59.955009 pyside6_utils-1.2.0/pyside6_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-04 18:59:59.000000 pyside6_utils-1.2.0/pyside6_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-04 18:59:59.000000 pyside6_utils-1.2.0/pyside6_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:59:59.000000 pyside6_utils-1.2.0/pyside6_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-04 18:59:59.000000 pyside6_utils-1.2.0/pyside6_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 18:59:59.000000 pyside6_utils-1.2.0/pyside6_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:59:59.967009 pyside6_utils-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-04 18:59:48.000000 pyside6_utils-1.2.0/setup.py
```

### Comparing `pyside6_utils-1.1.0/LICENSE` & `pyside6_utils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/PKG-INFO` & `pyside6_utils-1.2.0/pyside6_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,207 +1,283 @@
 Metadata-Version: 2.1
-Name: pyside6_utils
-Version: 1.1.0
+Name: pyside6-utils
+Version: 1.2.0
 Summary: A collection of useful widgets and utilities for PySide6 compatible with pyside6-designer.
 Home-page: https://github.com/Woutah/pyside6-utils
 Author: Wouter Stokman
 License: LPGPLv2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySide6 - Utils
+
 `pyside6-utils` implements several useful PySide6 widgets, models and delegates as well as some utility functions.
-The package contains registrars for these widgets, which can be [used to register the widgets in QtDesigner](#Qt-Designer) to quickly build UI's.
+The package contains registrars for these widgets, which can be [used to register the widgets in QtDesigner](#qt-designer) to quickly build UI's.
+
+This package was mainly developed around the python Dataclass-functionality. It was created in tandem with the following package: [Configurun - A tool to create and manage machine learning training/testing-configurations and run them automatically and/or remotely.](https://github.com/Woutah/configurun).
 
-This package was mainly developed around the python Dataclass-functionality. It was created in tandem with the following package: [Configurun - A tool to create and manage machine learning training/testing-configurations and run them automatically and/or remotely.](https://github.com/Woutah/configurun). 
+# Table of contents
 
+- [PySide6 - Utils](#pyside6---utils)
+- [Table of contents](#table-of-contents)
+- [Features](#features)
+	- [Installation](#installation)
+	- [Qt-Designer](#qt-designer)
+- [Widgets](#widgets)
+	- [`DataclassTreeview`](#dataclasstreeview)
+	- [`PandasTableView` (and `PandasTableModel`)](#pandastableview-and-pandastablemodel)
+	- [`ExtendedMdiArea` / `FramelessMdiWindow`](#extendedmdiarea--framelessmdiwindow)
+	- [`CollapsibleGroupBox`](#collapsiblegroupbox)
+	- [`Console Widget`](#console-widget)
+	- [`FileExplorerView`](#fileexplorerview)
+	- [`OverlayWidget`](#overlaywidget)
+	- [`RangeSelector`](#rangeselector)
+	- [`SquareFrame`](#squareframe)
+	- [`WidgetList`](#widgetlist)
+	- [`WidgetSwitcher`](#widgetswitcher)
+- [Utility](#utility)
+- [Classes](#classes)
+- [Models](#models)
+- [Acknowledgements](#acknowledgements)
+
+# Features
 
 A quick list of the main widgets:
-- [`DataclassTreeview` (and `DataClassModel` & `DataClassEditorDelegate`)](#DataclassTreeview)
+
+- [`DataclassTreeview` (and `DataClassModel` & `DataClassEditorDelegate`)](#dataclasstreeview)
   - A view/model/delegate combination which mirrors a python dataclass (`@dataclass`) object and provides editors for each of the types defined. Edits are propagated to the dataclass object. We can use [`dataclasses.field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.Field) to customize how attributes are displayed and to change the editor-type and constraints.
-- [`PandasTableView` (and `PandasTableModel`)](#PandasTableView)
+- [`PandasTableView` (and `PandasTableModel`)](#pandastableview-and-pandastablemodel)
   - Provide an easy way to show and edit pandas dataframes
-- [`CollapsibleGroupBox`](#CollapsibleGroupBox)
+- [`CollapsibleGroupBox`](#collapsiblegroupbox)
   - A groupbox that acts as a layout, when the user check/unchecks the groupbox, the contents collapse
-- [`ConsoleWidget`](#ConsoleWidget)
+- [`ConsoleWidget`](#console-widget)
   - A console-like widget to which multiple files can be mirorred, user can select the items to view the consoleitem-contens
-- [`ExtendedMdiArea` / `FramelessMdiWindow`](#ExtendedMdiArea)
-  - Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. A custom UI example is provided in `./ui/FrameslessMdiWindow.ui` 
-- [`FileExplorerView`](#FileExplorerView)
+- [`ExtendedMdiArea` / `FramelessMdiWindow`](#extendedmdiarea--framelessmdiwindow)
+  - Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. A custom UI example is provided in `./ui/FrameslessMdiWindow.ui`
+- [`FileExplorerView`](#fileexplorerview)
   - Built around the use of a QFileSystemModel - enables right-click operations and undo/redo actions, as well as the possibility to set a "highlighted" file
-- [`OverlayWidget`](#OverlayWidget)
+- [`OverlayWidget`](#overlaywidget)
   - Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s)
-- [`SquareFrame`](#SquareFrame)
+- [`SquareFrame`](#squareframe)
   - A small widget wrapper that enforces squareness. Useful when designing UI's in QtDesigner.
-- [`RangeSelector`](#RangeSelector)
+- [`RangeSelector`](#rangeselector)
   - Widget to select a range of float/int/datetime, provides extra styling if ticks are provided.
-
+- [`WidgetList`](#widgetlist)
+  - Widget to which we can pass a widget-factory or widget-type. The user can then add/remove widgets of this type to the list.
+- [`WidgetSwitcher`](#widgetswitcher)
+  - Wrapper around [`QtWidgets.QStackedWidget`](https://doc.qt.io/qt-6/qstackedwidget.html), provides a way to switch between multiple widgets.
 
 ## Installation
+
 The easiest way to install this package is using pip install:
-```
+
+``` bash
 pip install pyside6-utils
 ```
 
 The package can also be manually installed by downloading this repository, extracting it to the desired install location and running:
-```
+
+``` bash
 pip install <install_path>
 ```
 
 ## Qt-Designer
+
 This package provides registrars for the implemented widgets, which means that the widgets can be made available directly in qt-designer (note that `pyside6-designer` should be used).
 To enable this, the environment variable `PYSIDE_DESIGNER_PLUGINS` should be set to the `../pyside6_utils/registrars`-folder.
 
 Alternatively, we can automatically set environment variables by using the provided pyside6 launch script. We can use this script by running `pyside6_utils/examples/run_qt_designer.py` or by importing and running the `run_qt_designer()`-function using:
-```python
+
+``` python
 from pyside6_utilities.examples import run_qt_designer
 run_qt_designer()
 ```
 
 If all is well, this should result in the widgets showing up in the left-hand side of Qt-designer, e.g. for the views it should look like this:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/Qt_designer_loaded_widgets_example.png?raw=True" width="800" />
 </p>
 
 # Widgets
+
 **NOTE: every widget-module contains a `run_example_app()` function, which starts a qt app and an example-instance of the widget in question, the following example-widget-images are pictures of these examples. Example:**
+
 ```python
 from pyside6_utils.widgets.data_class_tree_view import run_example_app
 DataclassTreeview.run_example_app()
 ```
 
-
 ## `DataclassTreeview`
+
 `DataclassTreeview`, `DataClassModel` and `DataClassEditorDelegate` are a view/model/delegate combination (resp.) which mirror a python dataclass (`@dataclass`) object and provides editors for each of the types defined.
 
 The model is mainly built around the `field()` functionality of dataclasses, which allows the model to make use of the default values, type hints and other information provided by the dataclass.
 For each field, we can provide additional information in the `metadata` attribute of `field()`, this information is used by the model to determine the editor/limits to use for the field.
 The following metadata is supported:
 
 | Metadata Key | Type | Description |
 | --- | --- | --- |
 | `"display_name"` | `str` | Name to display for this attribute in the view - defaults to the variable name itself |
 | `"display_path"` | `str` | Path to display this attribute - we can group/structure items when using a treeview - defaults to no parents|
 | `"help"` | `str` | Help-message which will be shown when the user hovers over this item - empty by default|
-| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [^constraintnote] , if none provided, use typehint of the field|
+| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [*](#constraintnote) , if none provided, use typehint of the field|
 | `"required"` | `bool` | Whether this field is required to be filled in - if true - a red background will appear if the value is not set|
 | `"editable"` | `bool` | Whether this field is editable - if false - the editor will be disabled|
 
-[^constraintnote] Constraints are (almost fully) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `utility.constraints`. The following constraints are supported:
+<a name="constraintnote">*</a>Constraints are (almost fully) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `classes.constraints`. The following constraints are supported:
 | Constraint | Description | Editor Type
 | --- | --- | --- |
 | `type` | The type of the value should match the type of the constraint | based on type |
 | `Options` / `Container` | The value should be one of the options provided in the constraint | `QComboBox` |
 | `StrOptions` | The value should be one of the str-options provided in the constraint | `QComboBox` |
 | `Interval` | The value should be within the interval provided in the constraint | `QSpinBox` or `QDoubleSpinBox` (limited) |
 | `None` | `None` is a valid value for this field `typing.Optional` | Adds reset-button to editor |
 | `Range` | The value should be within the range provided in the constraint | `QSpinBox` (limited) |
-| `TODO` | Maybe more? |
+| `ConstrainedList` | [*(Custom - not part of Sklearn)](#constrainedlist) Indicates a list of of values of a constrained type | Based on type of list |
+
+<a name="constrainedlist">*=</a>For example, `ConstrainedList([Interval(float, 0.0, 1.0), StrOptions(["string1", "string2"])])` indicates a list of values that should either be a float between 0.0 and 1.0, or the string "string1" or "string2". The editor for this field would be constructed as a [`WidgetList`](#widgetlist) with a [`WidgetSwitcher`](#widgetswitcher) as the factory-widget. The `WidgetSwitcher` would then have two widgets, one with a `QSpinBox` and one with a `QComboBox` as the editor. **NOTE:** the same editor would be the result of a `Typing.List[typing.Union[float, str]]` typehint, minus the bounded-interval constraint on the float:
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/string_float_list_example.png" width=300/> -->
+</p>
 
 Default values are saved and can be reset using right-click context menu. Values that have changed from default will appear in bold.
 
 An example of a dataclass-view is shown below:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/dataclass_view.png?raw=True" width="800" />
 </p>
 
-The dataclass from which this example was generated can be found under `./examples/example_dataclass.py`.  
+The dataclass from which this example was generated can be found under `./examples/example_dataclass.py`.
 
 ## `PandasTableView` (and `PandasTableModel`)
+
 Provide an easy way to show and edit pandas dataframes. Pandas-table model adds the possibility to copy/paste data from excel, as well as current selection information (e.g. selected cells, average, total and sum).
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/pandas_table_view.png?raw=True" width="800" />
 </p>
 
-
-
 ## `ExtendedMdiArea` / `FramelessMdiWindow`
+
 Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. The ui used by default is provided in `./ui/FrameslessMdiWindow.ui`.
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/extended_mdi_area.png?raw=True" width="800" />
 </p>
 
 We can drag, resize and move the windows as we would expect from a normal window. The windows can also be maximized and minimized using the buttons in the top-right corner. A custom UI can be provided, all functionality will be retained if the ui contains the following widgets:
 
 - `contentLayout` (`QtWidgets.QLayout`): The layout that will be used to add the content-widget
 - `titleBar` (`QtWidgets.QWidget`): The widget that will be used as the title bar, we can drag the window by using this, the parent-mdi area context menu will also be made available when right-clicking this widget
 	- `titleLabel` (`QtWidgets.QLabel`): The label that will be used to display the title
 	- `zoomButton` (`QtWidget.QButtton`): If pressed, set window to fullscreen
 	- `minimizeButton` (`QtWidget.QButtton`): If pressed, minimize the window
 
-
-
 ## `CollapsibleGroupBox`
+
 A QtWidgets.QGroupbox that acts as a layout, when the user check/unchecks the groupbox, the contents collapse
 When opened:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/collapsible_group_box_open.png?raw=True" width="800" />
 </p>
 When collapsed:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/collapsible_group_box_collapsed.png?raw=True" width="800" />
 </p>
 
 ## `Console Widget`
+
 We can import `console_from_file_item` from `pyside6_utils.models.console_widget_models` to create console items which mirror a text-output file. We can then add these items to the console-widget using `ConsoleWidget.add_item`.
 
-The user can then scroll between the various console-outputs, which are updated every time the target file changes. This is especially useful for managing multiple output-files. 
+The user can then scroll between the various console-outputs, which are updated every time the target file changes. This is especially useful for managing multiple output-files.
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/console_widget.png?raw=True" width="900" />
 </p>
 
 ## `FileExplorerView`
+
 Built around the use of a QFileSystemModel - enables right-click operations and undo/redo actions, as well as the possibility to set a "highlighted" file
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/file_explorer_view.png?raw=True" width="500" />
 </p>
 
 ## `OverlayWidget`
-Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s). 
+
+Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s).
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/overlay_widget.png?raw=True" width="400" />
 </p>
 
-## `RangeSelector` 
+## `RangeSelector`
+
 Widget to select a range of float/int/datetime etc. Can drag in the middle to change both, or drag on the edges to change only min/max.
 Provides extra styling when ticks are enabled.
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/range_selector.png?raw=True" width="400" />
 </p>
 
+## `SquareFrame`
+
+Enforces squareness of the widget inside. Useful when designing UI's in QtDesigner.
+<p align="center">
+	<!-- <img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/square_widget.png?raw=True" width="400" /> -->
+	<img src="./pyside6_utils/examples/images/square_widget.png" width=400/>
+</p>
+
+## `WidgetList`
+
+Widget to which we can pass a widget-factory or widget-type. The user can then add/remove widgets of this type to the list.
+A value-getter can be specified to easily get the values of all widgets in the list.
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/widget_list.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/widget_list.png" width=300/> -->
+</p>
+
+## `WidgetSwitcher`
+
+Wrapper around [`QtWidgets.QStackedWidget`](https://doc.qt.io/qt-6/qstackedwidget.html), provides a way to switch between multiple widgets. A context menu can be accessed via right click or via the small triangle in the right-bottom corner, which allows the user to switch between the widgets.
+
+Especially useful in combination with [`WidgetList`](#widgetlist). Provides the same value-getter functionality as `WidgetList`.
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/widget_switcher.png?raw=True" width="500" />
+	<!-- <img src="./pyside6_utils/examples/images/widget_switcher.png" width=500/> -->
+</p>
 
 # Utility
-The utility submodule provides the following:
+
+The utility submodule provides the following UI-based utility items:
+
 - `catch_show_exception_in_popup_decorator`
   - A decorator that catches exceptions and shows them in a popup
-- `constraints`
-  - Sklearn constraints, used for `DataClassModel` to constrain the editor-type based on the type-hint of the field
-- `Serializable`
-  - Base-class mainly targeted towards dataclasses - enable serialization to json. 
-- `SignalBlocker` 
-  - Enables us to temporarily block PySide6 signals using a `with` statement 
+- `SignalBlocker`
+  - Enables us to temporarily block PySide6 signals using a `with` statement
 - `utility_functions`
   - Several smaller utility functions used in this package
 
+# Classes
+The classes submodule provides several useful classes that do not depend on PySide6:
+
+- `constraints`
+  - Sklearn constraints, used for `DataClassModel` to constrain the editor-type based on the type-hint of the field
+- `Serializable`
+  - Mainly useful for `@dataclass`-like classes to parse from/to json
 
 # Models
+
 The models submodule provides an implementation of the following:
-- `ConsoleFromFileItem` / `ConsoleModel` 
+
+- `ConsoleFromFileItem` / `ConsoleModel`
   - Also see `ConsoleFromFileWidget` - A model/item combination that mirrors a text-file, used in `ConsoleWidget`. Use the `addItem()` method of `ConsoleModel` to add a new file to the model.
 - `DataclassModel`
   - Also see `DataclassTreeview` - A model that mirrors a python dataclass (`@dataclass`) object and provides editors for each of the types defined. Edits are propagated to the dataclass object.
 - `ExtendedSortFilterProxyModel`
   - Implements more advanced sorting (using multiple columns) and a `set_filter_function(...)` that can be used to use (multiple) custom methods to filter the model.
 - `FileExplorerModel`
-  - Also see `FileExplorerView` - Enabled highlighting items 
+  - Also see `FileExplorerView` - Enabled highlighting items
 - `PandasTableModel`
   - Also see `PandasTableView` - Mirrors pandas dataframe to a Qt tablemodel
 
-
-
 # Acknowledgements
-This package uses icons from (and based off) the Tango Desktop Project:
-http://tango.freedesktop.org/Tango_Desktop_Project
 
+This package uses icons from (and based off) the [Tango Desktop Project](http://tango.freedesktop.org/Tango_Desktop_Project).
```

### Comparing `pyside6_utils-1.1.0/README.md` & `pyside6_utils-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,197 +1,273 @@
 # PySide6 - Utils
+
 `pyside6-utils` implements several useful PySide6 widgets, models and delegates as well as some utility functions.
-The package contains registrars for these widgets, which can be [used to register the widgets in QtDesigner](#Qt-Designer) to quickly build UI's.
+The package contains registrars for these widgets, which can be [used to register the widgets in QtDesigner](#qt-designer) to quickly build UI's.
+
+This package was mainly developed around the python Dataclass-functionality. It was created in tandem with the following package: [Configurun - A tool to create and manage machine learning training/testing-configurations and run them automatically and/or remotely.](https://github.com/Woutah/configurun).
 
-This package was mainly developed around the python Dataclass-functionality. It was created in tandem with the following package: [Configurun - A tool to create and manage machine learning training/testing-configurations and run them automatically and/or remotely.](https://github.com/Woutah/configurun). 
+# Table of contents
 
+- [PySide6 - Utils](#pyside6---utils)
+- [Table of contents](#table-of-contents)
+- [Features](#features)
+	- [Installation](#installation)
+	- [Qt-Designer](#qt-designer)
+- [Widgets](#widgets)
+	- [`DataclassTreeview`](#dataclasstreeview)
+	- [`PandasTableView` (and `PandasTableModel`)](#pandastableview-and-pandastablemodel)
+	- [`ExtendedMdiArea` / `FramelessMdiWindow`](#extendedmdiarea--framelessmdiwindow)
+	- [`CollapsibleGroupBox`](#collapsiblegroupbox)
+	- [`Console Widget`](#console-widget)
+	- [`FileExplorerView`](#fileexplorerview)
+	- [`OverlayWidget`](#overlaywidget)
+	- [`RangeSelector`](#rangeselector)
+	- [`SquareFrame`](#squareframe)
+	- [`WidgetList`](#widgetlist)
+	- [`WidgetSwitcher`](#widgetswitcher)
+- [Utility](#utility)
+- [Classes](#classes)
+- [Models](#models)
+- [Acknowledgements](#acknowledgements)
+
+# Features
 
 A quick list of the main widgets:
-- [`DataclassTreeview` (and `DataClassModel` & `DataClassEditorDelegate`)](#DataclassTreeview)
+
+- [`DataclassTreeview` (and `DataClassModel` & `DataClassEditorDelegate`)](#dataclasstreeview)
   - A view/model/delegate combination which mirrors a python dataclass (`@dataclass`) object and provides editors for each of the types defined. Edits are propagated to the dataclass object. We can use [`dataclasses.field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.Field) to customize how attributes are displayed and to change the editor-type and constraints.
-- [`PandasTableView` (and `PandasTableModel`)](#PandasTableView)
+- [`PandasTableView` (and `PandasTableModel`)](#pandastableview-and-pandastablemodel)
   - Provide an easy way to show and edit pandas dataframes
-- [`CollapsibleGroupBox`](#CollapsibleGroupBox)
+- [`CollapsibleGroupBox`](#collapsiblegroupbox)
   - A groupbox that acts as a layout, when the user check/unchecks the groupbox, the contents collapse
-- [`ConsoleWidget`](#ConsoleWidget)
+- [`ConsoleWidget`](#console-widget)
   - A console-like widget to which multiple files can be mirorred, user can select the items to view the consoleitem-contens
-- [`ExtendedMdiArea` / `FramelessMdiWindow`](#ExtendedMdiArea)
-  - Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. A custom UI example is provided in `./ui/FrameslessMdiWindow.ui` 
-- [`FileExplorerView`](#FileExplorerView)
+- [`ExtendedMdiArea` / `FramelessMdiWindow`](#extendedmdiarea--framelessmdiwindow)
+  - Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. A custom UI example is provided in `./ui/FrameslessMdiWindow.ui`
+- [`FileExplorerView`](#fileexplorerview)
   - Built around the use of a QFileSystemModel - enables right-click operations and undo/redo actions, as well as the possibility to set a "highlighted" file
-- [`OverlayWidget`](#OverlayWidget)
+- [`OverlayWidget`](#overlaywidget)
   - Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s)
-- [`SquareFrame`](#SquareFrame)
+- [`SquareFrame`](#squareframe)
   - A small widget wrapper that enforces squareness. Useful when designing UI's in QtDesigner.
-- [`RangeSelector`](#RangeSelector)
+- [`RangeSelector`](#rangeselector)
   - Widget to select a range of float/int/datetime, provides extra styling if ticks are provided.
-
+- [`WidgetList`](#widgetlist)
+  - Widget to which we can pass a widget-factory or widget-type. The user can then add/remove widgets of this type to the list.
+- [`WidgetSwitcher`](#widgetswitcher)
+  - Wrapper around [`QtWidgets.QStackedWidget`](https://doc.qt.io/qt-6/qstackedwidget.html), provides a way to switch between multiple widgets.
 
 ## Installation
+
 The easiest way to install this package is using pip install:
-```
+
+``` bash
 pip install pyside6-utils
 ```
 
 The package can also be manually installed by downloading this repository, extracting it to the desired install location and running:
-```
+
+``` bash
 pip install <install_path>
 ```
 
 ## Qt-Designer
+
 This package provides registrars for the implemented widgets, which means that the widgets can be made available directly in qt-designer (note that `pyside6-designer` should be used).
 To enable this, the environment variable `PYSIDE_DESIGNER_PLUGINS` should be set to the `../pyside6_utils/registrars`-folder.
 
 Alternatively, we can automatically set environment variables by using the provided pyside6 launch script. We can use this script by running `pyside6_utils/examples/run_qt_designer.py` or by importing and running the `run_qt_designer()`-function using:
-```python
+
+``` python
 from pyside6_utilities.examples import run_qt_designer
 run_qt_designer()
 ```
 
 If all is well, this should result in the widgets showing up in the left-hand side of Qt-designer, e.g. for the views it should look like this:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/Qt_designer_loaded_widgets_example.png?raw=True" width="800" />
 </p>
 
 # Widgets
+
 **NOTE: every widget-module contains a `run_example_app()` function, which starts a qt app and an example-instance of the widget in question, the following example-widget-images are pictures of these examples. Example:**
+
 ```python
 from pyside6_utils.widgets.data_class_tree_view import run_example_app
 DataclassTreeview.run_example_app()
 ```
 
-
 ## `DataclassTreeview`
+
 `DataclassTreeview`, `DataClassModel` and `DataClassEditorDelegate` are a view/model/delegate combination (resp.) which mirror a python dataclass (`@dataclass`) object and provides editors for each of the types defined.
 
 The model is mainly built around the `field()` functionality of dataclasses, which allows the model to make use of the default values, type hints and other information provided by the dataclass.
 For each field, we can provide additional information in the `metadata` attribute of `field()`, this information is used by the model to determine the editor/limits to use for the field.
 The following metadata is supported:
 
 | Metadata Key | Type | Description |
 | --- | --- | --- |
 | `"display_name"` | `str` | Name to display for this attribute in the view - defaults to the variable name itself |
 | `"display_path"` | `str` | Path to display this attribute - we can group/structure items when using a treeview - defaults to no parents|
 | `"help"` | `str` | Help-message which will be shown when the user hovers over this item - empty by default|
-| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [^constraintnote] , if none provided, use typehint of the field|
+| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [*](#constraintnote) , if none provided, use typehint of the field|
 | `"required"` | `bool` | Whether this field is required to be filled in - if true - a red background will appear if the value is not set|
 | `"editable"` | `bool` | Whether this field is editable - if false - the editor will be disabled|
 
-[^constraintnote] Constraints are (almost fully) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `utility.constraints`. The following constraints are supported:
+<a name="constraintnote">*</a>Constraints are (almost fully) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `classes.constraints`. The following constraints are supported:
 | Constraint | Description | Editor Type
 | --- | --- | --- |
 | `type` | The type of the value should match the type of the constraint | based on type |
 | `Options` / `Container` | The value should be one of the options provided in the constraint | `QComboBox` |
 | `StrOptions` | The value should be one of the str-options provided in the constraint | `QComboBox` |
 | `Interval` | The value should be within the interval provided in the constraint | `QSpinBox` or `QDoubleSpinBox` (limited) |
 | `None` | `None` is a valid value for this field `typing.Optional` | Adds reset-button to editor |
 | `Range` | The value should be within the range provided in the constraint | `QSpinBox` (limited) |
-| `TODO` | Maybe more? |
+| `ConstrainedList` | [*(Custom - not part of Sklearn)](#constrainedlist) Indicates a list of of values of a constrained type | Based on type of list |
+
+<a name="constrainedlist">*=</a>For example, `ConstrainedList([Interval(float, 0.0, 1.0), StrOptions(["string1", "string2"])])` indicates a list of values that should either be a float between 0.0 and 1.0, or the string "string1" or "string2". The editor for this field would be constructed as a [`WidgetList`](#widgetlist) with a [`WidgetSwitcher`](#widgetswitcher) as the factory-widget. The `WidgetSwitcher` would then have two widgets, one with a `QSpinBox` and one with a `QComboBox` as the editor. **NOTE:** the same editor would be the result of a `Typing.List[typing.Union[float, str]]` typehint, minus the bounded-interval constraint on the float:
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/string_float_list_example.png" width=300/> -->
+</p>
 
 Default values are saved and can be reset using right-click context menu. Values that have changed from default will appear in bold.
 
 An example of a dataclass-view is shown below:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/dataclass_view.png?raw=True" width="800" />
 </p>
 
-The dataclass from which this example was generated can be found under `./examples/example_dataclass.py`.  
+The dataclass from which this example was generated can be found under `./examples/example_dataclass.py`.
 
 ## `PandasTableView` (and `PandasTableModel`)
+
 Provide an easy way to show and edit pandas dataframes. Pandas-table model adds the possibility to copy/paste data from excel, as well as current selection information (e.g. selected cells, average, total and sum).
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/pandas_table_view.png?raw=True" width="800" />
 </p>
 
-
-
 ## `ExtendedMdiArea` / `FramelessMdiWindow`
+
 Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. The ui used by default is provided in `./ui/FrameslessMdiWindow.ui`.
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/extended_mdi_area.png?raw=True" width="800" />
 </p>
 
 We can drag, resize and move the windows as we would expect from a normal window. The windows can also be maximized and minimized using the buttons in the top-right corner. A custom UI can be provided, all functionality will be retained if the ui contains the following widgets:
 
 - `contentLayout` (`QtWidgets.QLayout`): The layout that will be used to add the content-widget
 - `titleBar` (`QtWidgets.QWidget`): The widget that will be used as the title bar, we can drag the window by using this, the parent-mdi area context menu will also be made available when right-clicking this widget
 	- `titleLabel` (`QtWidgets.QLabel`): The label that will be used to display the title
 	- `zoomButton` (`QtWidget.QButtton`): If pressed, set window to fullscreen
 	- `minimizeButton` (`QtWidget.QButtton`): If pressed, minimize the window
 
-
-
 ## `CollapsibleGroupBox`
+
 A QtWidgets.QGroupbox that acts as a layout, when the user check/unchecks the groupbox, the contents collapse
 When opened:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/collapsible_group_box_open.png?raw=True" width="800" />
 </p>
 When collapsed:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/collapsible_group_box_collapsed.png?raw=True" width="800" />
 </p>
 
 ## `Console Widget`
+
 We can import `console_from_file_item` from `pyside6_utils.models.console_widget_models` to create console items which mirror a text-output file. We can then add these items to the console-widget using `ConsoleWidget.add_item`.
 
-The user can then scroll between the various console-outputs, which are updated every time the target file changes. This is especially useful for managing multiple output-files. 
+The user can then scroll between the various console-outputs, which are updated every time the target file changes. This is especially useful for managing multiple output-files.
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/console_widget.png?raw=True" width="900" />
 </p>
 
 ## `FileExplorerView`
+
 Built around the use of a QFileSystemModel - enables right-click operations and undo/redo actions, as well as the possibility to set a "highlighted" file
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/file_explorer_view.png?raw=True" width="500" />
 </p>
 
 ## `OverlayWidget`
-Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s). 
+
+Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s).
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/overlay_widget.png?raw=True" width="400" />
 </p>
 
-## `RangeSelector` 
+## `RangeSelector`
+
 Widget to select a range of float/int/datetime etc. Can drag in the middle to change both, or drag on the edges to change only min/max.
 Provides extra styling when ticks are enabled.
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/range_selector.png?raw=True" width="400" />
 </p>
 
+## `SquareFrame`
+
+Enforces squareness of the widget inside. Useful when designing UI's in QtDesigner.
+<p align="center">
+	<!-- <img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/square_widget.png?raw=True" width="400" /> -->
+	<img src="./pyside6_utils/examples/images/square_widget.png" width=400/>
+</p>
+
+## `WidgetList`
+
+Widget to which we can pass a widget-factory or widget-type. The user can then add/remove widgets of this type to the list.
+A value-getter can be specified to easily get the values of all widgets in the list.
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/widget_list.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/widget_list.png" width=300/> -->
+</p>
+
+## `WidgetSwitcher`
+
+Wrapper around [`QtWidgets.QStackedWidget`](https://doc.qt.io/qt-6/qstackedwidget.html), provides a way to switch between multiple widgets. A context menu can be accessed via right click or via the small triangle in the right-bottom corner, which allows the user to switch between the widgets.
+
+Especially useful in combination with [`WidgetList`](#widgetlist). Provides the same value-getter functionality as `WidgetList`.
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/widget_switcher.png?raw=True" width="500" />
+	<!-- <img src="./pyside6_utils/examples/images/widget_switcher.png" width=500/> -->
+</p>
 
 # Utility
-The utility submodule provides the following:
+
+The utility submodule provides the following UI-based utility items:
+
 - `catch_show_exception_in_popup_decorator`
   - A decorator that catches exceptions and shows them in a popup
-- `constraints`
-  - Sklearn constraints, used for `DataClassModel` to constrain the editor-type based on the type-hint of the field
-- `Serializable`
-  - Base-class mainly targeted towards dataclasses - enable serialization to json. 
-- `SignalBlocker` 
-  - Enables us to temporarily block PySide6 signals using a `with` statement 
+- `SignalBlocker`
+  - Enables us to temporarily block PySide6 signals using a `with` statement
 - `utility_functions`
   - Several smaller utility functions used in this package
 
+# Classes
+The classes submodule provides several useful classes that do not depend on PySide6:
+
+- `constraints`
+  - Sklearn constraints, used for `DataClassModel` to constrain the editor-type based on the type-hint of the field
+- `Serializable`
+  - Mainly useful for `@dataclass`-like classes to parse from/to json
 
 # Models
+
 The models submodule provides an implementation of the following:
-- `ConsoleFromFileItem` / `ConsoleModel` 
+
+- `ConsoleFromFileItem` / `ConsoleModel`
   - Also see `ConsoleFromFileWidget` - A model/item combination that mirrors a text-file, used in `ConsoleWidget`. Use the `addItem()` method of `ConsoleModel` to add a new file to the model.
 - `DataclassModel`
   - Also see `DataclassTreeview` - A model that mirrors a python dataclass (`@dataclass`) object and provides editors for each of the types defined. Edits are propagated to the dataclass object.
 - `ExtendedSortFilterProxyModel`
   - Implements more advanced sorting (using multiple columns) and a `set_filter_function(...)` that can be used to use (multiple) custom methods to filter the model.
 - `FileExplorerModel`
-  - Also see `FileExplorerView` - Enabled highlighting items 
+  - Also see `FileExplorerView` - Enabled highlighting items
 - `PandasTableModel`
   - Also see `PandasTableView` - Mirrors pandas dataframe to a Qt tablemodel
 
-
-
 # Acknowledgements
-This package uses icons from (and based off) the Tango Desktop Project:
-http://tango.freedesktop.org/Tango_Desktop_Project
 
+This package uses icons from (and based off) the [Tango Desktop Project](http://tango.freedesktop.org/Tango_Desktop_Project).
```

### Comparing `pyside6_utils-1.1.0/pyside6_utils/examples/run_qt_designer.py` & `pyside6_utils-1.2.0/pyside6_utils/examples/run_qt_designer.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/examples/run_widgets_example_app.py` & `pyside6_utils-1.2.0/pyside6_utils/examples/run_widgets_example_app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""Run a window with examples for the widgets in this package."""
-
-import sys
-
-import pandas as pd
-from PySide6.QtWidgets import QApplication, QMainWindow
-
-from pyside6_utils.models.pandas_table_model import PandasTableModel
-from pyside6_utils.ui.AllWidgets_ui import Ui_MainWindow
-
-
-def run_widgets_example_app():
-	"""Creates a qt app and shows a window with all a couple of small widgets in this package.
-	TODO: create buttons for the large widgets? 
-	"""
-	app = QApplication(sys.argv)
-	example_window = QMainWindow()
-	example_ui = Ui_MainWindow()
-	example_ui.setupUi(example_window)
-
-	#====== Example df for PandasTableView ======
-	example_df = pd.DataFrame({
-		"Column 1": [1, 2, 3, 4, 5],
-		"Column 2": [10, 20, 30, 40, 50],
-		"Column 3": [100, 200, 300, 400, 500],
-		"Column 4": [1000, 2000, 3000, 4000, 5000],
-		"Column 5": [10000, 20000, 30000, 40000, 50000],
-	})
-	example_df_model = PandasTableModel(example_df)
-	example_ui.pandasTableView.setModel(example_df_model)
-	example_ui.pandasTableView.set_status_bar(example_window.statusBar())
-
-	example_window.show()
-	sys.exit(app.exec())
-
-
-if __name__ == "__main__":
-	run_widgets_example_app()
+"""Run a window with examples for the widgets in this package."""
+
+import sys
+
+import pandas as pd
+from PySide6.QtWidgets import QApplication, QMainWindow
+
+from pyside6_utils.models.pandas_table_model import PandasTableModel
+from pyside6_utils.ui.allWidgets_ui import Ui_MainWindow
+
+
+def run_widgets_example_app():
+	"""Creates a qt app and shows a window with all a couple of small widgets in this package.
+	TODO: create buttons for the large widgets? 
+	"""
+	app = QApplication(sys.argv)
+	example_window = QMainWindow()
+	example_ui = Ui_MainWindow()
+	example_ui.setupUi(example_window)
+
+	#====== Example df for PandasTableView ======
+	example_df = pd.DataFrame({
+		"Column 1": [1, 2, 3, 4, 5],
+		"Column 2": [10, 20, 30, 40, 50],
+		"Column 3": [100, 200, 300, 400, 500],
+		"Column 4": [1000, 2000, 3000, 4000, 5000],
+		"Column 5": [10000, 20000, 30000, 40000, 50000],
+	})
+	example_df_model = PandasTableModel(example_df)
+	example_ui.pandasTableView.setModel(example_df_model)
+	example_ui.pandasTableView.set_status_bar(example_window.statusBar())
+
+	example_window.show()
+	sys.exit(app.exec())
+
+
+if __name__ == "__main__":
+	run_widgets_example_app()
```

### Comparing `pyside6_utils-1.1.0/pyside6_utils/icons/app_resources_rc.py` & `pyside6_utils-1.2.0/pyside6_utils/icons/app_resources_rc.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/models/console_widget_models/console_from_file_item.py` & `pyside6_utils-1.2.0/pyside6_utils/models/console_widget_models/console_from_file_item.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/models/console_widget_models/console_model.py` & `pyside6_utils-1.2.0/pyside6_utils/models/console_widget_models/console_model.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/models/dataclass_model.py` & `pyside6_utils-1.2.0/pyside6_utils/models/dataclass_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import dataclasses
 import datetime
 import logging
 import typing
 from dataclasses import fields, is_dataclass
-
+import enum
 from PySide6 import QtCore, QtGui, QtWidgets
 
 from pyside6_utils.models.dataclass_tree_item import DataclassTreeItem
 
 log = logging.getLogger(__name__)
 
 class SetDataCommand(QtGui.QUndoCommand):
@@ -41,15 +41,16 @@
 
 	def undo(self):
 		self._model._set_data(self._index, self._old_value, self._role) #pylint: disable=protected-access
 
 	def redo(self):
 		self._model._set_data(self._index, self._new_value, self._role) #pylint: disable=protected-access
 
-
+class HasNoDefaultError(Exception):
+	"""Raised when a field has no default value"""
 
 class DataclassModel(QtCore.QAbstractItemModel):
 	"""
 	A model that can be used to display a dataclass as a QT tree view.
 	Meant to be used with a QTreeView, but can also be used with a QTableView. Edits are propagated to the dataclass and
 	are undoable/redoable if an undo stack is provided.
 
@@ -58,16 +59,24 @@
 		- display_path: The path to the field in the tree view. If not specified, the field is displayed at the root of
 			the tree.
 		- help: A tooltip that is displayed when hovering over the field in the tree view.
 		- editable: Whether the field is editable in the tree view. Defaults to True.
 		- constraints: A list of constraints that are displayed in the tooltip. Defaults to None.
 
 	"""
-	FIELD_ROLE = QtCore.Qt.ItemDataRole.UserRole + 1 #Role for the field
-	TYPE_ROLE = QtCore.Qt.ItemDataRole.UserRole #Returns the type of the field
+	# FIELD_ROLE = QtCore.Qt.ItemDataRole.UserRole + 1 #Role for the field
+	# TYPE_ROLE = QtCore.Qt.ItemDataRole.UserRole #Returns the type of the field
+	class CustomDataRoles(enum.IntEnum):
+		"""The custom roles for getting data of dataclass-fields"""
+		#pylint: disable=invalid-name #Allow Qt-style names
+		TypeRole = QtCore.Qt.ItemDataRole.UserRole #Returns the type of the field
+		FieldRole = QtCore.Qt.ItemDataRole.UserRole + 1 #Role for the field
+		DefaultValueRole = QtCore.Qt.ItemDataRole.UserRole + 2 #Role for the default value of the field
+		AttributeNameRole = QtCore.Qt.ItemDataRole.UserRole + 3 #Role for the name of the attribute
+		TreeItemRole = QtCore.Qt.ItemDataRole.UserRole + 4 #Role for the tree item
 
 	def __init__(self, dataclass_instance : object,
 					parent: typing.Optional[QtCore.QObject] = None,
 					undo_stack : QtGui.QUndoStack | None = None,
 					allow_non_field_attrs : bool = False
 				) -> None:
 		"""
@@ -215,14 +224,26 @@
 					return "Value"
 			else:
 				return section
 		else:
 			return None
 
 
+	def get_default_value(self, data_class_field : dataclasses.Field) -> typing.Any:
+		"""Get default value of item using the passed field, raises hasNoDefaultError if no default value is available
+
+		Raises HasNoDefaultError: If no default value is available
+		"""
+		if hasattr(data_class_field, "default") \
+				and data_class_field.default != dataclasses.MISSING: #If default value is defined
+			return data_class_field.default
+		elif hasattr(data_class_field, "default_factory"):
+			return data_class_field.default_factory() #type: ignore
+		else:
+			raise HasNoDefaultError(f"Could not get default value for field {data_class_field.name}")
 
 
 	def data(self, index: QtCore.QModelIndex, role: int = QtCore.Qt.ItemDataRole.DisplayRole) -> typing.Any:
 		"""
 		Returns the data stored under the given role for the item referred to by the index.
 		"""
 		try:
@@ -240,19 +261,20 @@
 					except (IndexError, KeyError, AttributeError):
 						return node.name
 				else:
 					ret_val = self._dataclass.__dict__.get(node.name, None)
 					if ret_val is None:
 						return ""
 					elif isinstance(ret_val, datetime.datetime):
-						return ret_val.strftime("%Y-%m-%d %H:%M:%S")
+						return ret_val.strftime("%d-%m-%Y %H:%M:%S")
 					elif isinstance(ret_val, bool):
 						return str(ret_val).capitalize()
+					elif isinstance(ret_val, list):
+						return ", ".join([str(item) for item in ret_val])
 					return ret_val
-
 			elif role == QtCore.Qt.ItemDataRole.EditRole:
 				return self._dataclass.__dict__.get(node.name, None)
 			elif role == QtCore.Qt.ItemDataRole.ToolTipRole:
 				if name_field_dict.get(node.name, None) is None:
 					return node.name #If only a header (no data)
 				result_str = ""
 				result_str += name_field_dict[node.name].metadata.get("help", "")
@@ -261,52 +283,67 @@
 					result_str += " <b style='color:red'>(required)</b>"
 				try:
 					item_type_name = name_field_dict[node.name].type.__name__
 				except AttributeError: #E.g. uniontype has no __name__ attribute
 					item_type_name = str(name_field_dict[node.name].type)
 				result_str += f" (type: {item_type_name[:20]})"
 
-					
-				if hasattr(name_field_dict[node.name], "default"):
-					result_str += f" (default: {str(name_field_dict[node.name].default)[:20]})"
+
+				try:
+					result_str += f" (default: {str(self.get_default_value(name_field_dict[node.name]))[:20]})"
+				except HasNoDefaultError:
+					pass
+
 				return result_str
-			elif role == DataclassModel.TYPE_ROLE: #Get type role #TODO: maybe create Enum with more descriptive names.
+			elif role == DataclassModel.CustomDataRoles.TypeRole: #Get type role
 					#NOTE: if we just use an enum, we get an error in ModelIndex.data due to the enum not being an instance
 					# of Qt.ItemDataRole.DisplayRole
 				result = name_field_dict.get(node.name, None) #Get field
 				if result:
 					return result.type #If field is available -> return type
 				else:
 					return None
-			elif role == DataclassModel.FIELD_ROLE: #Field role
+			elif role == DataclassModel.CustomDataRoles.AttributeNameRole: #Get attribute name role
+				return node.name
+			elif role == DataclassModel.CustomDataRoles.FieldRole: #Field role
 				result = name_field_dict.get(node.name, None) #Get field
 				return result
+			elif role == DataclassModel.CustomDataRoles.DefaultValueRole: #Default value role
+				if name_field_dict.get(node.name, None) is None:
+					raise HasNoDefaultError(f"Field {node.name} is not a field of the dataclass")
+				return self.get_default_value(name_field_dict[node.name])
+			elif role == DataclassModel.CustomDataRoles.TreeItemRole: #Tree item role
+				return node
 			elif role == QtCore.Qt.ItemDataRole.FontRole:
 				if name_field_dict.get(node.name, None) is None:
 					return None #If only a header (no data)
-				if hasattr(name_field_dict[node.name], "default"):
-					default_val = name_field_dict[node.name].default
-					#If current value is not equal to the default value, make the font bold
-					if self._dataclass.__dict__.get(node.name, None) != default_val:
-						font = QtGui.QFont()
-						font.setBold(True)
-						return font
+
+				default_val = None
+
+				default_val = self.get_default_value(name_field_dict[node.name]) #Catch hasnodefaulterror later
+				cur_val = self._dataclass.__dict__.get(node.name, None)
+
+				if cur_val != default_val:
+					font = QtGui.QFont()
+					font.setBold(True)
+					return font
 				return None
 			elif role == QtCore.Qt.ItemDataRole.BackgroundRole: #If required and empty, make background red
 				if name_field_dict.get(node.name, None) is None:
 					return None #If only a header (no data)
 				if hasattr(name_field_dict[node.name], "metadata"):
 					is_required =  name_field_dict[node.name].metadata.get("required", False)
 					if is_required and self._dataclass.__dict__.get(node.name, None) is None:
 						return QtGui.QBrush(QtGui.QColor(255, 0, 0, 50))
 				return None
-			
-		except Exception as exception: #pylint: disable=broad-except
+
+		except Exception as exception:
 			log.warning(f"Error while retrieving data at index ({index.row()},{index.column()}) - "
 	       		f"{type(exception).__name__} : {exception}")
+			raise #Re-raise exception so we can use it in caller if we're using data() ourselves
 
 		return None
 
 
 	def _set_data(self, index: QtCore.QModelIndex | QtCore.QPersistentModelIndex,
 					value: typing.Any,
 					role: int = QtCore.Qt.ItemDataRole.EditRole) -> bool:
@@ -316,39 +353,58 @@
 		if role == QtCore.Qt.ItemDataRole.EditRole:
 			tree_item = index.internalPointer()
 			assert isinstance(tree_item, DataclassTreeItem)
 			self._dataclass.__dict__[tree_item.name] = value
 			# self.dataChanged.emit(index, self.index(index.row(), 2, index.parent())) #TODO: this seems to cause issues?
 			self.dataChanged.emit(index, index)
 			return True
+		if role == DataclassModel.CustomDataRoles.DefaultValueRole: #If setting back to default
+			tree_item = index.internalPointer()
+			assert isinstance(tree_item, DataclassTreeItem), "Can't get default value for non-treeitem"
+			assert tree_item.field is not None, "Can't get default value for property without field"
+			self._dataclass.__dict__[tree_item.name] = self.get_default_value(tree_item.field)
 		return False
 
 
 
 	def setData(self,
 				index: QtCore.QModelIndex,
 				value: typing.Any,
 				role: int = QtCore.Qt.ItemDataRole.EditRole
 			) -> bool:
 		"""
 		Sets the role data for the item at index to value.
 		"""
-		log.debug(f"Setting data at index {index} to {value} of type {type(value)}")
+		# log.debug(f"Setting data at index {index} to {value} of type {type(value)}")
 
 
 		if not self._undo_stack:
 			return self._set_data(index, value, role)
 
 		if role == QtCore.Qt.ItemDataRole.EditRole:
 			dataclass_item = index.internalPointer()
 			assert isinstance(dataclass_item, DataclassTreeItem)
 			if self._dataclass.__dict__[dataclass_item.name] == value: #If the value is different from the current value
 				return False #Do nothing
 			self._undo_stack.push(SetDataCommand(self, index, value, role)) #Push the command to the undo-stack
 			return True
+		elif role == DataclassModel.CustomDataRoles.DefaultValueRole: #If setting back to default
+			tree_item = index.internalPointer()
+			assert isinstance(tree_item, DataclassTreeItem), "Can't get default value for non-treeitem"
+			assert tree_item.field is not None, "Can't get default value for property without field"
+			if self._dataclass.__dict__[tree_item.name] == self.get_default_value(tree_item.field):
+				return False
+			self._undo_stack.push(
+				SetDataCommand(
+					self,
+					index,
+					self.get_default_value(tree_item.field),
+					role=QtCore.Qt.ItemDataRole.EditRole #Make sure we get old/new value using editRole
+				)
+			)
 		return False
 
 	def flags(self, index: QtCore.QModelIndex) -> QtCore.Qt.ItemFlag:
 		if index.column() == 0:
 			return QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
 		else:
 			if index.internalPointer():
@@ -366,17 +422,16 @@
 		if not index.isValid():
 			return
 		tree_item = index.internalPointer()
 		assert isinstance(tree_item, DataclassTreeItem)
 		field = tree_item.field
 		if field is None:
 			return
-		if hasattr(field, "default"):
-			default_value = field.default
-			self.setData(index, default_value, QtCore.Qt.ItemDataRole.EditRole)
+		default_value = self.get_default_value(field)
+		self.setData(index, default_value, QtCore.Qt.ItemDataRole.EditRole)
 
 	def has_default(self, index: QtCore.QModelIndex) -> bool:
 		"""Returns whether the given index has a default value"""
 		if not index.isValid():
 			return False
 		tree_item = index.internalPointer()
 		assert isinstance(tree_item, DataclassTreeItem)
```

### Comparing `pyside6_utils-1.1.0/pyside6_utils/models/dataclass_tree_item.py` & `pyside6_utils-1.2.0/pyside6_utils/models/dataclass_tree_item.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/models/extended_sort_filter_proxy_model.py` & `pyside6_utils-1.2.0/pyside6_utils/models/extended_sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/models/file_explorer_model.py` & `pyside6_utils-1.2.0/pyside6_utils/models/file_explorer_model.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/models/pandas_table_model.py` & `pyside6_utils-1.2.0/pyside6_utils/models/pandas_table_model.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/registrars/register_collapsible_group_box.py` & `pyside6_utils-1.2.0/pyside6_utils/registrars/register_collapsible_group_box.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/registrars/register_console_widget.py` & `pyside6_utils-1.2.0/pyside6_utils/registrars/register_console_widget.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/registrars/register_extended_mdi_area.py` & `pyside6_utils-1.2.0/pyside6_utils/registrars/register_extended_mdi_area.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/registrars/register_file_explorer_view.py` & `pyside6_utils-1.2.0/pyside6_utils/registrars/register_file_explorer_view.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/registrars/register_overlay_widget.py` & `pyside6_utils-1.2.0/pyside6_utils/registrars/register_overlay_widget.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/registrars/register_pandas_table.py` & `pyside6_utils-1.2.0/pyside6_utils/registrars/register_pandas_table.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/registrars/register_range_selector.py` & `pyside6_utils-1.2.0/pyside6_utils/registrars/register_range_selector.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/registrars/register_square_frame.py` & `pyside6_utils-1.2.0/pyside6_utils/registrars/register_square_frame.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/ui/ConsoleWidget_ui.py` & `pyside6_utils-1.2.0/pyside6_utils/ui/ConsoleWidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/ui/FramelessMdiWindow_ui.py` & `pyside6_utils-1.2.0/pyside6_utils/ui/FramelessMdiWindow_ui.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/ui/allWidgets_ui.py` & `pyside6_utils-1.2.0/pyside6_utils/ui/allWidgets_ui.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/utility/catch_show_exception_in_popup_decorator.py` & `pyside6_utils-1.2.0/pyside6_utils/utility/catch_show_exception_in_popup_decorator.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/utility/constraints.py` & `pyside6_utils-1.2.0/pyside6_utils/classes/constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,971 +1,1047 @@
-"""
-Copied module from sklearn.utils.validation and sklearn.utils._validation for framework not to be dependent on whole sklearn library
-==========================License:================================
-BSD 3-Clause License
-
-Copyright (c) 2007-2023 The scikit-learn developers.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-"""
-
-
-from abc import ABC
-from abc import abstractmethod
-from collections.abc import Iterable
-import functools
-import math
-from inspect import signature
-from numbers import Integral
-from numbers import Real
-import operator
-import re
-import warnings
-
-import numpy as np
-# from scipy.sparse import issparse 
-# from scipy.sparse import csr_matrix 
-
-# from .validation import _is_arraylike_not_scalar
-def _is_arraylike(x):
-	"""Returns whether the input is array-like."""
-	return hasattr(x, "__len__") or hasattr(x, "shape") or hasattr(x, "__array__")
-
-
-def _is_arraylike_not_scalar(array):
-	"""Return True if array is array-like and not a scalar"""
-	return _is_arraylike(array) and not np.isscalar(array)
-
-
-class InvalidParameterError(ValueError, TypeError):
-	"""Custom exception to be raised when the parameter of a class/method/function
-	does not have a valid type or value.
-	"""
-
-	# Inherits from ValueError and TypeError to keep backward compatibility.
-
-
-def validate_parameter_constraints(parameter_constraints, params, caller_name):
-	"""Validate types and values of given parameters.
-
-	Parameters
-	----------
-	parameter_constraints : dict or {"no_validation"}
-		If "no_validation", validation is skipped for this parameter.
-
-		If a dict, it must be a dictionary `param_name: list of constraints`.
-		A parameter is valid if it satisfies one of the constraints from the list.
-		Constraints can be:
-		- an Interval object, representing a continuous or discrete range of numbers
-		- the string "array-like"
-		- the string "sparse matrix"
-		- the string "random_state"
-		- callable
-		- None, meaning that None is a valid value for the parameter
-		- any type, meaning that any instance of this type is valid
-		- an Options object, representing a set of elements of a given type
-		- a StrOptions object, representing a set of strings
-		- the string "boolean"
-		- the string "verbose"
-		- the string "cv_object"
-		- the string "missing_values"
-		- a HasMethods object, representing method(s) an object must have
-		- a Hidden object, representing a constraint not meant to be exposed to the user
-
-	params : dict
-		A dictionary `param_name: param_value`. The parameters to validate against the
-		constraints.
-
-	caller_name : str
-		The name of the estimator or function or method that called this function.
-	"""
-	for param_name, param_val in params.items():
-		# We allow parameters to not have a constraint so that third party estimators
-		# can inherit from sklearn estimators without having to necessarily use the
-		# validation tools.
-		if param_name not in parameter_constraints:
-			continue
-
-		constraints = parameter_constraints[param_name]
-
-		if constraints == "no_validation":
-			continue
-
-		constraints = [make_constraint(constraint) for constraint in constraints]
-
-		for constraint in constraints:
-			if constraint.is_satisfied_by(param_val):
-				# this constraint is satisfied, no need to check further.
-				break
-		else:
-			# No constraint is satisfied, raise with an informative message.
-
-			# Ignore constraints that we don't want to expose in the error message,
-			# i.e. options that are for internal purpose or not officially supported.
-			constraints = [
-				constraint for constraint in constraints if not constraint.hidden
-			]
-
-			if len(constraints) == 1:
-				constraints_str = f"{constraints[0]}"
-			else:
-				constraints_str = (
-					f"{', '.join([str(c) for c in constraints[:-1]])} or"
-					f" {constraints[-1]}"
-				)
-
-			raise InvalidParameterError(
-				f"The {param_name!r} parameter of {caller_name} must be"
-				f" {constraints_str}. Got {param_val!r} instead."
-			)
-
-
-def make_constraint(constraint):
-	"""Convert the constraint into the appropriate Constraint object.
-
-	Parameters
-	----------
-	constraint : object
-		The constraint to convert.
-
-	Returns
-	-------
-	constraint : instance of _Constraint
-		The converted constraint.
-	"""
-	if isinstance(constraint, str) and constraint == "array-like":
-		return _ArrayLikes()
-	if isinstance(constraint, str) and constraint == "sparse matrix":
-		return _SparseMatrices()
-	if isinstance(constraint, str) and constraint == "random_state":
-		return _RandomStates()
-	if constraint is callable:
-		return _Callables()
-	if constraint is None:
-		return _NoneConstraint()
-	if isinstance(constraint, type):
-		return _InstancesOf(constraint)
-	if isinstance(constraint, (Interval, StrOptions, Options, HasMethods)):
-		return constraint
-	if isinstance(constraint, str) and constraint == "boolean":
-		return _Booleans()
-	if isinstance(constraint, str) and constraint == "verbose":
-		return _VerboseHelper()
-	if isinstance(constraint, str) and constraint == "missing_values":
-		return _MissingValues()
-	if isinstance(constraint, str) and constraint == "cv_object":
-		return _CVObjects()
-	if isinstance(constraint, Hidden):
-		constraint = make_constraint(constraint.constraint)
-		constraint.hidden = True
-		return constraint
-	raise ValueError(f"Unknown constraint type: {constraint}")
-
-
-def validate_params(parameter_constraints):
-	"""Decorator to validate types and values of functions and methods.
-
-	Parameters
-	----------
-	parameter_constraints : dict
-		A dictionary `param_name: list of constraints`. See the docstring of
-		`validate_parameter_constraints` for a description of the accepted constraints.
-
-		Note that the *args and **kwargs parameters are not validated and must not be
-		present in the parameter_constraints dictionary.
-
-	Returns
-	-------
-	decorated_function : function or method
-		The decorated function.
-	"""
-
-	def decorator(func):
-		# The dict of parameter constraints is set as an attribute of the function
-		# to make it possible to dynamically introspect the constraints for
-		# automatic testing.
-		setattr(func, "_skl_parameter_constraints", parameter_constraints)
-
-		@functools.wraps(func)
-		def wrapper(*args, **kwargs):
-
-			func_sig = signature(func)
-
-			# Map *args/**kwargs to the function signature
-			params = func_sig.bind(*args, **kwargs)
-			params.apply_defaults()
-
-			# ignore self/cls and positional/keyword markers
-			to_ignore = [
-				p.name
-				for p in func_sig.parameters.values()
-				if p.kind in (p.VAR_POSITIONAL, p.VAR_KEYWORD)
-			]
-			to_ignore += ["self", "cls"]
-			params = {k: v for k, v in params.arguments.items() if k not in to_ignore}
-
-			validate_parameter_constraints(
-				parameter_constraints, params, caller_name=func.__qualname__
-			)
-
-			try:
-				return func(*args, **kwargs)
-			except InvalidParameterError as exception:
-				# When the function is just a wrapper around an estimator, we allow
-				# the function to delegate validation to the estimator, but we replace
-				# the name of the estimator by the name of the function in the error
-				# message to avoid confusion.
-				msg = re.sub(
-					r"parameter of \w+ must be",
-					f"parameter of {func.__qualname__} must be",
-					str(exception),
-				)
-				raise InvalidParameterError(msg) from exception
-
-		return wrapper
-
-	return decorator
-
-
-def _type_name(t):
-	"""Convert type into human readable string."""
-	module = t.__module__
-	qualname = t.__qualname__
-	if module == "builtins":
-		return qualname
-	elif t == Real:
-		return "float"
-	elif t == Integral:
-		return "int"
-	return f"{module}.{qualname}"
-
-
-class _Constraint(ABC):
-	"""Base class for the constraint objects."""
-
-	def __init__(self):
-		self.hidden = False
-
-	@abstractmethod
-	def is_satisfied_by(self, val):
-		"""Whether or not a value satisfies the constraint.
-
-		Parameters
-		----------
-		val : object
-			The value to check.
-
-		Returns
-		-------
-		is_satisfied : bool
-			Whether or not the constraint is satisfied by this value.
-		"""
-
-	@abstractmethod
-	def __str__(self):
-		"""A human readable representational string of the constraint."""
-
-
-class _InstancesOf(_Constraint):
-	"""Constraint representing instances of a given type.
-
-	Parameters
-	----------
-	type : type
-		The valid type.
-	"""
-
-	def __init__(self, type):
-		super().__init__()
-		self.type = type
-
-	def is_satisfied_by(self, val):
-		return isinstance(val, self.type)
-
-	def __str__(self):
-		return f"an instance of {_type_name(self.type)!r}"
-
-
-class _NoneConstraint(_Constraint):
-	"""Constraint representing the None singleton."""
-
-	def is_satisfied_by(self, val):
-		return val is None
-
-	def __str__(self):
-		return "None"
-
-
-class _NanConstraint(_Constraint):
-	"""Constraint representing the indicator `np.nan`."""
-
-	def is_satisfied_by(self, val):
-		return isinstance(val, Real) and math.isnan(val)
-
-	def __str__(self):
-		return "numpy.nan"
-
-
-class _PandasNAConstraint(_Constraint):
-	"""Constraint representing the indicator `pd.NA`."""
-
-	def is_satisfied_by(self, val):
-		try:
-			import pandas as pd
-
-			return isinstance(val, type(pd.NA)) and pd.isna(val)
-		except ImportError:
-			return False
-
-	def __str__(self):
-		return "pandas.NA"
-
-
-class Options(_Constraint):
-	"""Constraint representing a finite set of instances of a given type.
-
-	Parameters
-	----------
-	type : type
-
-	options : set
-		The set of valid scalars.
-
-	deprecated : set or None, default=None
-		A subset of the `options` to mark as deprecated in the string
-		representation of the constraint.
-	"""
-
-	def __init__(self, type, options, *, deprecated=None):
-		super().__init__()
-		self.type = type
-		self.options = options
-		self.deprecated = deprecated or set()
-
-		if self.deprecated - self.options:
-			raise ValueError("The deprecated options must be a subset of the options.")
-
-	def is_satisfied_by(self, val):
-		return isinstance(val, self.type) and val in self.options
-
-	def _mark_if_deprecated(self, option):
-		"""Add a deprecated mark to an option if needed."""
-		option_str = f"{option!r}"
-		if option in self.deprecated:
-			option_str = f"{option_str} (deprecated)"
-		return option_str
-
-	def __str__(self):
-		options_str = (
-			f"{', '.join([self._mark_if_deprecated(o) for o in self.options])}"
-		)
-		return f"a {_type_name(self.type)} among {{{options_str}}}"
-
-
-class StrOptions(Options):
-	"""Constraint representing a finite set of strings.
-
-	Parameters
-	----------
-	options : set of str
-		The set of valid strings.
-
-	deprecated : set of str or None, default=None
-		A subset of the `options` to mark as deprecated in the string
-		representation of the constraint.
-	"""
-
-	def __init__(self, options, *, deprecated=None):
-		super().__init__(type=str, options=options, deprecated=deprecated)
-
-
-class Interval(_Constraint):
-	"""Constraint representing a typed interval.
-
-	Parameters
-	----------
-	type : {numbers.Integral, numbers.Real}
-		The set of numbers in which to set the interval.
-
-	left : float or int or None
-		The left bound of the interval. None means left bound is -∞.
-
-	right : float, int or None
-		The right bound of the interval. None means right bound is +∞.
-
-	closed : {"left", "right", "both", "neither"}
-		Whether the interval is open or closed. Possible choices are:
-
-		- `"left"`: the interval is closed on the left and open on the right.
-		  It is equivalent to the interval `[ left, right )`.
-		- `"right"`: the interval is closed on the right and open on the left.
-		  It is equivalent to the interval `( left, right ]`.
-		- `"both"`: the interval is closed.
-		  It is equivalent to the interval `[ left, right ]`.
-		- `"neither"`: the interval is open.
-		  It is equivalent to the interval `( left, right )`.
-
-	Notes
-	-----
-	Setting a bound to `None` and setting the interval closed is valid. For instance,
-	strictly speaking, `Interval(Real, 0, None, closed="both")` corresponds to
-	`[0, +∞) U {+∞}`.
-	"""
-
-	@validate_params(
-		{
-			"type": [type],
-			"left": [Integral, Real, None],
-			"right": [Integral, Real, None],
-			"closed": [StrOptions({"left", "right", "both", "neither"})],
-		}
-	)
-	def __init__(self, type, left, right, *, closed):
-		super().__init__()
-		self.type = type
-		self.left = left
-		self.right = right
-		self.closed = closed
-
-		self._check_params()
-
-	def _check_params(self):
-		if self.type is Integral:
-			suffix = "for an interval over the integers."
-			if self.left is not None and not isinstance(self.left, Integral):
-				raise TypeError(f"Expecting left to be an int {suffix}")
-			if self.right is not None and not isinstance(self.right, Integral):
-				raise TypeError(f"Expecting right to be an int {suffix}")
-			if self.left is None and self.closed in ("left", "both"):
-				raise ValueError(
-					f"left can't be None when closed == {self.closed} {suffix}"
-				)
-			if self.right is None and self.closed in ("right", "both"):
-				raise ValueError(
-					f"right can't be None when closed == {self.closed} {suffix}"
-				)
-
-		if self.right is not None and self.left is not None and self.right <= self.left:
-			raise ValueError(
-				f"right can't be less than left. Got left={self.left} and "
-				f"right={self.right}"
-			)
-
-	def __contains__(self, val):
-		if np.isnan(val):
-			return False
-
-		left_cmp = operator.lt if self.closed in ("left", "both") else operator.le
-		right_cmp = operator.gt if self.closed in ("right", "both") else operator.ge
-
-		left = -np.inf if self.left is None else self.left
-		right = np.inf if self.right is None else self.right
-
-		if left_cmp(val, left):
-			return False
-		if right_cmp(val, right):
-			return False
-		return True
-
-	def is_satisfied_by(self, val):
-		if not isinstance(val, self.type):
-			return False
-
-		return val in self
-
-	def __str__(self):
-		type_str = "an int" if self.type is Integral else "a float"
-		left_bracket = "[" if self.closed in ("left", "both") else "("
-		left_bound = "-inf" if self.left is None else self.left
-		right_bound = "inf" if self.right is None else self.right
-		right_bracket = "]" if self.closed in ("right", "both") else ")"
-		return (
-			f"{type_str} in the range "
-			f"{left_bracket}{left_bound}, {right_bound}{right_bracket}"
-		)
-
-
-class _ArrayLikes(_Constraint):
-	"""Constraint representing array-likes"""
-
-	def is_satisfied_by(self, val):
-		return _is_arraylike_not_scalar(val)
-
-	def __str__(self):
-		return "an array-like"
-
-
-class _SparseMatrices(_Constraint):
-	"""Constraint representing sparse matrices."""
-
-	def is_satisfied_by(self, val):
-		return issparse(val) #type:ignore #NOTE: to use, import from scipy.sparse import issparse 
-
-	def __str__(self):
-		return "a sparse matrix"
-
-
-class _Callables(_Constraint):
-	"""Constraint representing callables."""
-
-	def is_satisfied_by(self, val):
-		return callable(val)
-
-	def __str__(self):
-		return "a callable"
-
-
-class _RandomStates(_Constraint):
-	"""Constraint representing random states.
-
-	Convenience class for
-	[Interval(Integral, 0, 2**32 - 1, closed="both"), np.random.RandomState, None]
-	"""
-
-	def __init__(self):
-		super().__init__()
-		self._constraints = [
-			Interval(Integral, 0, 2**32 - 1, closed="both"),
-			_InstancesOf(np.random.RandomState),
-			_NoneConstraint(),
-		]
-
-	def is_satisfied_by(self, val):
-		return any(c.is_satisfied_by(val) for c in self._constraints)
-
-	def __str__(self):
-		return (
-			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
-			f" {self._constraints[-1]}"
-		)
-
-
-class _Booleans(_Constraint):
-	"""Constraint representing boolean likes.
-
-	Convenience class for
-	[bool, np.bool_, Integral (deprecated)]
-	"""
-
-	def __init__(self):
-		super().__init__()
-		self._constraints = [
-			_InstancesOf(bool),
-			_InstancesOf(np.bool_),
-			_InstancesOf(Integral),
-		]
-
-	def is_satisfied_by(self, val):
-		# TODO(1.4) remove support for Integral.
-		if isinstance(val, Integral) and not isinstance(val, bool):
-			warnings.warn(
-				"Passing an int for a boolean parameter is deprecated in version 1.2 "
-				"and won't be supported anymore in version 1.4.",
-				FutureWarning,
-			)
-
-		return any(c.is_satisfied_by(val) for c in self._constraints)
-
-	def __str__(self):
-		return (
-			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
-			f" {self._constraints[-1]}"
-		)
-
-
-class _VerboseHelper(_Constraint):
-	"""Helper constraint for the verbose parameter.
-
-	Convenience class for
-	[Interval(Integral, 0, None, closed="left"), bool, numpy.bool_]
-	"""
-
-	def __init__(self):
-		super().__init__()
-		self._constraints = [
-			Interval(Integral, 0, None, closed="left"),
-			_InstancesOf(bool),
-			_InstancesOf(np.bool_),
-		]
-
-	def is_satisfied_by(self, val):
-		return any(c.is_satisfied_by(val) for c in self._constraints)
-
-	def __str__(self):
-		return (
-			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
-			f" {self._constraints[-1]}"
-		)
-
-
-class _MissingValues(_Constraint):
-	"""Helper constraint for the `missing_values` parameters.
-
-	Convenience for
-	[
-		Integral,
-		Interval(Real, None, None, closed="both"),
-		str,
-		None,
-		_NanConstraint(),
-		_PandasNAConstraint(),
-	]
-	"""
-
-	def __init__(self):
-		super().__init__()
-		self._constraints = [
-			_InstancesOf(Integral),
-			# we use an interval of Real to ignore np.nan that has its own constraint
-			Interval(Real, None, None, closed="both"),
-			_InstancesOf(str),
-			_NoneConstraint(),
-			_NanConstraint(),
-			_PandasNAConstraint(),
-		]
-
-	def is_satisfied_by(self, val):
-		return any(c.is_satisfied_by(val) for c in self._constraints)
-
-	def __str__(self):
-		return (
-			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
-			f" {self._constraints[-1]}"
-		)
-
-
-class HasMethods(_Constraint):
-	"""Constraint representing objects that expose specific methods.
-
-	It is useful for parameters following a protocol and where we don't want to impose
-	an affiliation to a specific module or class.
-
-	Parameters
-	----------
-	methods : str or list of str
-		The method(s) that the object is expected to expose.
-	"""
-
-	@validate_params({"methods": [str, list]})
-	def __init__(self, methods):
-		super().__init__()
-		if isinstance(methods, str):
-			methods = [methods]
-		self.methods = methods
-
-	def is_satisfied_by(self, val):
-		return all(callable(getattr(val, method, None)) for method in self.methods)
-
-	def __str__(self):
-		if len(self.methods) == 1:
-			methods = f"{self.methods[0]!r}"
-		else:
-			methods = (
-				f"{', '.join([repr(m) for m in self.methods[:-1]])} and"
-				f" {self.methods[-1]!r}"
-			)
-		return f"an object implementing {methods}"
-
-
-class _IterablesNotString(_Constraint):
-	"""Constraint representing iterables that are not strings."""
-
-	def is_satisfied_by(self, val):
-		return isinstance(val, Iterable) and not isinstance(val, str)
-
-	def __str__(self):
-		return "an iterable"
-
-
-class _CVObjects(_Constraint):
-	"""Constraint representing cv objects.
-
-	Convenient class for
-	[
-		Interval(Integral, 2, None, closed="left"),
-		HasMethods(["split", "get_n_splits"]),
-		_IterablesNotString(),
-		None,
-	]
-	"""
-
-	def __init__(self):
-		super().__init__()
-		self._constraints = [
-			Interval(Integral, 2, None, closed="left"),
-			HasMethods(["split", "get_n_splits"]),
-			_IterablesNotString(),
-			_NoneConstraint(),
-		]
-
-	def is_satisfied_by(self, val):
-		return any(c.is_satisfied_by(val) for c in self._constraints)
-
-	def __str__(self):
-		return (
-			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
-			f" {self._constraints[-1]}"
-		)
-
-
-class Hidden:
-	"""Class encapsulating a constraint not meant to be exposed to the user.
-
-	Parameters
-	----------
-	constraint : str or _Constraint instance
-		The constraint to be used internally.
-	"""
-
-	def __init__(self, constraint):
-		self.constraint = constraint
-
-
-def generate_invalid_param_val(constraint, constraints=None):
-	"""Return a value that does not satisfy the constraint.
-
-	Raises a NotImplementedError if there exists no invalid value for this constraint.
-
-	This is only useful for testing purpose.
-
-	Parameters
-	----------
-	constraint : _Constraint instance
-		The constraint to generate a value for.
-
-	constraints : list of _Constraint instances or None, default=None
-		The list of all constraints for this parameter. If None, the list only
-		containing `constraint` is used.
-
-	Returns
-	-------
-	val : object
-		A value that does not satisfy the constraint.
-	"""
-	if isinstance(constraint, StrOptions):
-		return f"not {' or '.join(constraint.options)}"
-
-	if isinstance(constraint, _MissingValues):
-		return np.array([1, 2, 3])
-
-	if isinstance(constraint, _VerboseHelper):
-		return -1
-
-	if isinstance(constraint, HasMethods):
-		return type("HasNotMethods", (), {})()
-
-	if isinstance(constraint, _IterablesNotString):
-		return "a string"
-
-	if isinstance(constraint, _CVObjects):
-		return "not a cv object"
-
-	if not isinstance(constraint, Interval):
-		raise NotImplementedError
-
-	# constraint is an interval
-	constraints = [constraint] if constraints is None else constraints
-	return _generate_invalid_param_val_interval(constraint, constraints)
-
-
-def _generate_invalid_param_val_interval(interval, constraints):
-	"""Return a value that does not satisfy an interval constraint.
-
-	Generating an invalid value for an integer interval depends on the other constraints
-	since an int is a real, meaning that it can be valid for a real interval.
-	Assumes that there can be at most 2 interval constraints: one integer interval
-	and/or one real interval.
-
-	This is only useful for testing purpose.
-
-	Parameters
-	----------
-	interval : Interval instance
-		The interval to generate a value for.
-
-	constraints : list of _Constraint instances
-		The list of all constraints for this parameter.
-
-	Returns
-	-------
-	val : object
-		A value that does not satisfy the interval constraint.
-	"""
-	if interval.type is Real:
-		# generate a non-integer value such that it can't be valid even if there's also
-		# an integer interval constraint.
-		if interval.left is None and interval.right is None:
-			if interval.closed in ("left", "neither"):
-				return np.inf
-			elif interval.closed in ("right", "neither"):
-				return -np.inf
-			else:
-				raise NotImplementedError
-
-		if interval.left is not None:
-			return np.floor(interval.left) - 0.5
-		else:  # right is not None
-			return np.ceil(interval.right) + 0.5
-
-	else:  # interval.type is Integral
-		if interval.left is None and interval.right is None:
-			raise NotImplementedError
-
-		# We need to check if there's also a real interval constraint to generate a
-		# value that is not valid for any of the 2 interval constraints.
-		real_intervals = [
-			i for i in constraints if isinstance(i, Interval) and i.type is Real
-		]
-		real_interval = real_intervals[0] if real_intervals else None
-
-		if real_interval is None:
-			# Only the integer interval constraint -> easy
-			if interval.left is not None:
-				return interval.left - 1
-			else:  # interval.right is not None
-				return interval.right + 1
-
-		# There's also a real interval constraint. Try to find a value left to both or
-		# right to both or in between them.
-
-		# redefine left and right bounds to be smallest and largest valid integers in
-		# both intervals.
-		int_left = interval.left
-		if int_left is not None and interval.closed in ("right", "neither"):
-			int_left = int_left + 1
-
-		int_right = interval.right
-		if int_right is not None and interval.closed in ("left", "neither"):
-			int_right = int_right - 1
-
-		real_left = real_interval.left
-		if real_interval.left is not None:
-			real_left = int(np.ceil(real_interval.left))
-			if real_interval.closed in ("right", "neither"):
-				real_left = real_left + 1
-
-		real_right = real_interval.right
-		if real_interval.right is not None:
-			real_right = int(np.floor(real_interval.right))
-			if real_interval.closed in ("left", "neither"):
-				real_right = real_right - 1
-
-		if int_left is not None and real_left is not None:
-			# there exists an int left to both intervals
-			return min(int_left, real_left) - 1
-
-		if int_right is not None and real_right is not None:
-			# there exists an int right to both intervals
-			return max(int_right, real_right) + 1
-
-		if int_left is not None:
-			if real_right is not None and int_left - real_right >= 2:
-				# there exists an int between the 2 intervals
-				return int_left - 1
-			else:
-				raise NotImplementedError
-		else:  # int_right is not None
-			if real_left is not None and real_left - int_right >= 2:
-				# there exists an int between the 2 intervals
-				return int_right + 1
-			else:
-				raise NotImplementedError
-
-
-def generate_valid_param(constraint):
-	"""Return a value that does satisfy a constraint.
-
-	This is only useful for testing purpose.
-
-	Parameters
-	----------
-	constraint : Constraint instance
-		The constraint to generate a value for.
-
-	Returns
-	-------
-	val : object
-		A value that does satisfy the constraint.
-	"""
-	if isinstance(constraint, _ArrayLikes):
-		return np.array([1, 2, 3])
-
-	if isinstance(constraint, _SparseMatrices):
-		#NOTE: to use, import scipy.sparse import issparse: from scipy.sparse import csr_matrix 
-		# Chose to comment this to make this module work without scipy
-		return csr_matrix([[0, 1], [1, 0]]) #pylint: disable=undefined-variable #type:ignore
-
-	if isinstance(constraint, _RandomStates):
-		return np.random.RandomState(42)
-
-	if isinstance(constraint, _Callables):
-		return lambda x: x
-
-	if isinstance(constraint, _NoneConstraint):
-		return None
-
-	if isinstance(constraint, _InstancesOf):
-		return constraint.type()
-
-	if isinstance(constraint, _Booleans):
-		return True
-
-	if isinstance(constraint, _VerboseHelper):
-		return 1
-
-	if isinstance(constraint, _MissingValues):
-		return np.nan
-
-	if isinstance(constraint, HasMethods):
-		return type(
-			"ValidHasMethods", (), {m: lambda self: None for m in constraint.methods}
-		)()
-
-	if isinstance(constraint, _IterablesNotString):
-		return [1, 2, 3]
-
-	if isinstance(constraint, _CVObjects):
-		return 5
-
-	if isinstance(constraint, Options):  # includes StrOptions
-		for option in constraint.options:
-			return option
-
-	if isinstance(constraint, Interval):
-		interval = constraint
-		if interval.left is None and interval.right is None:
-			return 0
-		elif interval.left is None:
-			return interval.right - 1
-		elif interval.right is None:
-			return interval.left + 1
-		else:
-			if interval.type is Real:
-				return (interval.left + interval.right) / 2
-			else:
-				return interval.left + 1
-
-	raise ValueError(f"Unknown constraint type: {constraint}")
+"""
+Module largely sourced from sklearn.utils.validation and sklearn.utils._validation for framework
+not to be dependent on whole sklearn library
+
+Also added ConstrainedList - this indicates that an item contains a list of items, each constrained by the same 
+constraint e.g.:
+
+ConstrainedList([None, Interval(int, 0,10, closed='both')]) indicates a list of items, each of which is either None or
+an int between 0 and 10
+
+==========================License:================================
+BSD 3-Clause License
+
+Copyright (c) 2007-2023 The scikit-learn developers.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+"""
+#pylint: disable=redefined-builtin
+
+from abc import ABC
+from abc import abstractmethod
+from collections.abc import Iterable
+import functools
+import math
+from inspect import signature
+from numbers import Integral
+from numbers import Real
+import operator
+import re
+import copy
+import sys
+import warnings
+import typing
+
+import numpy as np
+# from scipy.sparse import issparse
+# from scipy.sparse import csr_matrix
+
+# from .validation import _is_arraylike_not_scalar
+def _is_arraylike(x): #pylint: disable=invalid-name
+	"""Returns whether the input is array-like."""
+	return hasattr(x, "__len__") or hasattr(x, "shape") or hasattr(x, "__array__")
+
+
+def _is_arraylike_not_scalar(array):
+	"""Return True if array is array-like and not a scalar"""
+	return _is_arraylike(array) and not np.isscalar(array)
+
+
+class InvalidParameterError(ValueError, TypeError):
+	"""Custom exception to be raised when the parameter of a class/method/function
+	does not have a valid type or value.
+	"""
+
+	# Inherits from ValueError and TypeError to keep backward compatibility.
+
+
+def validate_parameter_constraints(parameter_constraints, params, caller_name):
+	"""Validate types and values of given parameters.
+
+	Parameters
+	----------
+	parameter_constraints : dict or {"no_validation"}
+		If "no_validation", validation is skipped for this parameter.
+
+		If a dict, it must be a dictionary `param_name: list of constraints`.
+		A parameter is valid if it satisfies one of the constraints from the list.
+		Constraints can be:
+		- an Interval object, representing a continuous or discrete range of numbers
+		- the string "array-like"
+		- the string "sparse matrix"
+		- the string "random_state"
+		- callable
+		- None, meaning that None is a valid value for the parameter
+		- any type, meaning that any instance of this type is valid
+		- an Options object, representing a set of elements of a given type
+		- a StrOptions object, representing a set of strings
+		- the string "boolean"
+		- the string "verbose"
+		- the string "cv_object"
+		- the string "missing_values"
+		- a HasMethods object, representing method(s) an object must have
+		- a Hidden object, representing a constraint not meant to be exposed to the user
+
+	params : dict
+		A dictionary `param_name: param_value`. The parameters to validate against the
+		constraints.
+
+	caller_name : str
+		The name of the estimator or function or method that called this function.
+	"""
+	for param_name, param_val in params.items():
+		# We allow parameters to not have a constraint so that third party estimators
+		# can inherit from sklearn estimators without having to necessarily use the
+		# validation tools.
+		if param_name not in parameter_constraints:
+			continue
+
+		constraints = parameter_constraints[param_name]
+
+		if constraints == "no_validation":
+			continue
+
+		constraints = [make_constraint(constraint) for constraint in constraints]
+
+		for constraint in constraints:
+			if constraint.is_satisfied_by(param_val):
+				# this constraint is satisfied, no need to check further.
+				break
+		else:
+			# No constraint is satisfied, raise with an informative message.
+
+			# Ignore constraints that we don't want to expose in the error message,
+			# i.e. options that are for internal purpose or not officially supported.
+			constraints = [
+				constraint for constraint in constraints if not constraint.hidden
+			]
+
+			if len(constraints) == 1:
+				constraints_str = f"{constraints[0]}"
+			else:
+				constraints_str = (
+					f"{', '.join([str(c) for c in constraints[:-1]])} or"
+					f" {constraints[-1]}"
+				)
+
+			raise InvalidParameterError(
+				f"The {param_name!r} parameter of {caller_name} must be"
+				f" {constraints_str}. Got {param_val!r} instead."
+			)
+
+
+
+def make_constraint(constraint):
+	"""Convert the constraint into the appropriate Constraint object.
+
+	Parameters
+	----------
+	constraint : object
+		The constraint to convert.
+
+	Returns
+	-------
+	constraint : instance of _Constraint
+		The converted constraint.
+	"""
+	#NOTE: added 2023.07.03 to allow for arbitrary Constraint-objects to be passed
+	#Check if module of constraint is sklearn.utils._param_validation -> if so, we can't use isistance as is
+	if constraint is not None and \
+			hasattr(constraint, "__module__") and\
+			constraint.__module__ == "sklearn.utils._param_validation": 
+		#recreate the constraint in the current module by name 
+		#NOTE: this is a bit hacky, but it works
+		# cur_class = getattr(sys.modules[__name__], type(constraint).__name__)\
+		if type(constraint).__name__ not in dir(sys.modules[__name__]):
+			raise ValueError(f"Unknown constraint type: {constraint} - maybe the constraint module is out of date "
+		    	"compared to its sklearn.utils._param_validation equivalent?")
+		cur_class = getattr(sys.modules[__name__], type(constraint).__name__)
+		thecopy = copy.deepcopy(constraint)
+		thecopy.__class__ = cur_class
+		constraint = thecopy
+
+	if isinstance(constraint, _Constraint): #If already a constraint, just return it
+		return constraint
+
+	if isinstance(constraint, str) and constraint == "array-like":
+		return _ArrayLikes()
+	if isinstance(constraint, str) and constraint == "sparse matrix":
+		return _SparseMatrices()
+	if isinstance(constraint, str) and constraint == "random_state":
+		return _RandomStates()
+	if constraint is callable:
+		return _Callables()
+	if constraint is None:
+		return _NoneConstraint()
+	if isinstance(constraint, type):
+		return _InstancesOf(constraint)
+	if isinstance(constraint, (Interval, StrOptions, Options, HasMethods, ConstrainedList)): #Added constrainedlist here
+		return constraint
+	if isinstance(constraint, str) and constraint == "boolean":
+		return _Booleans()
+	if isinstance(constraint, str) and constraint == "verbose":
+		return _VerboseHelper()
+	if isinstance(constraint, str) and constraint == "missing_values":
+		return _MissingValues()
+	if isinstance(constraint, str) and constraint == "cv_object":
+		return _CVObjects()
+	if isinstance(constraint, Hidden):
+		constraint = make_constraint(constraint.constraint)
+		constraint.hidden = True
+		return constraint
+	raise ValueError(f"Unknown constraint type: {constraint}")
+
+
+def validate_params(parameter_constraints):
+	"""Decorator to validate types and values of functions and methods.
+
+	Parameters
+	----------
+	parameter_constraints : dict
+		A dictionary `param_name: list of constraints`. See the docstring of
+		`validate_parameter_constraints` for a description of the accepted constraints.
+
+		Note that the *args and **kwargs parameters are not validated and must not be
+		present in the parameter_constraints dictionary.
+
+	Returns
+	-------
+	decorated_function : function or method
+		The decorated function.
+	"""
+
+	def decorator(func):
+		# The dict of parameter constraints is set as an attribute of the function
+		# to make it possible to dynamically introspect the constraints for
+		# automatic testing.
+		setattr(func, "_skl_parameter_constraints", parameter_constraints)
+
+		@functools.wraps(func)
+		def wrapper(*args, **kwargs):
+
+			func_sig = signature(func)
+
+			# Map *args/**kwargs to the function signature
+			params = func_sig.bind(*args, **kwargs)
+			params.apply_defaults()
+
+			# ignore self/cls and positional/keyword markers
+			to_ignore = [
+				p.name
+				for p in func_sig.parameters.values()
+				if p.kind in (p.VAR_POSITIONAL, p.VAR_KEYWORD)
+			]
+			to_ignore += ["self", "cls"]
+			params = {k: v for k, v in params.arguments.items() if k not in to_ignore}
+
+			validate_parameter_constraints(
+				parameter_constraints, params, caller_name=func.__qualname__
+			)
+
+			try:
+				return func(*args, **kwargs)
+			except InvalidParameterError as exception:
+				# When the function is just a wrapper around an estimator, we allow
+				# the function to delegate validation to the estimator, but we replace
+				# the name of the estimator by the name of the function in the error
+				# message to avoid confusion.
+				msg = re.sub(
+					r"parameter of \w+ must be",
+					f"parameter of {func.__qualname__} must be",
+					str(exception),
+				)
+				raise InvalidParameterError(msg) from exception
+
+		return wrapper
+
+	return decorator
+
+
+def _type_name(t): #pylint: disable=invalid-name
+	"""Convert type into human readable string."""
+	module = t.__module__
+	qualname = t.__qualname__
+	if module == "builtins":
+		return qualname
+	elif t == Real:
+		return "float"
+	elif t == Integral:
+		return "int"
+	return f"{module}.{qualname}"
+
+
+class _Constraint(ABC):
+	"""Base class for the constraint objects."""
+
+	def __init__(self):
+		self.hidden = False
+
+	@abstractmethod
+	def is_satisfied_by(self, val):
+		"""Whether or not a value satisfies the constraint.
+
+		Parameters
+		----------
+		val : object
+			The value to check.
+
+		Returns
+		-------
+		is_satisfied : bool
+			Whether or not the constraint is satisfied by this value.
+		"""
+
+	@abstractmethod
+	def __str__(self):
+		"""A human readable representational string of the constraint."""
+
+
+class _InstancesOf(_Constraint):
+	"""Constraint representing instances of a given type.
+
+	Parameters
+	----------
+	type : type
+		The valid type.
+	"""
+
+	def __init__(self, type):
+		super().__init__()
+		self.type = type
+
+	def is_satisfied_by(self, val):
+		return isinstance(val, self.type)
+
+	def __str__(self):
+		return f"an instance of {_type_name(self.type)!r}"
+
+
+class _NoneConstraint(_Constraint):
+	"""Constraint representing the None singleton."""
+
+	def is_satisfied_by(self, val):
+		return val is None
+
+	def __str__(self):
+		return "None"
+
+
+class _NanConstraint(_Constraint):
+	"""Constraint representing the indicator `np.nan`."""
+
+	def is_satisfied_by(self, val):
+		return isinstance(val, Real) and math.isnan(val)
+
+	def __str__(self):
+		return "numpy.nan"
+
+
+class _PandasNAConstraint(_Constraint):
+	"""Constraint representing the indicator `pd.NA`."""
+
+	def is_satisfied_by(self, val):
+		try:
+			import pandas as pd #pylint: disable=import-outside-toplevel
+			return isinstance(val, type(pd.NA)) and pd.isna(val)
+		except ImportError:
+			return False
+
+	def __str__(self):
+		return "pandas.NA"
+
+
+class Options(_Constraint):
+	"""Constraint representing a finite set of instances of a given type.
+
+	Parameters
+	----------
+	type : type
+
+	options : set
+		The set of valid scalars.
+
+	deprecated : set or None, default=None
+		A subset of the `options` to mark as deprecated in the string
+		representation of the constraint.
+	"""
+
+	def __init__(self, type, options, *, deprecated=None):
+		super().__init__()
+		self.type = type
+		self.options = options
+		self.deprecated = deprecated or set()
+
+		if self.deprecated - self.options:
+			raise ValueError("The deprecated options must be a subset of the options.")
+
+	def is_satisfied_by(self, val):
+		return isinstance(val, self.type) and val in self.options
+
+	def _mark_if_deprecated(self, option):
+		"""Add a deprecated mark to an option if needed."""
+		option_str = f"{option!r}"
+		if option in self.deprecated:
+			option_str = f"{option_str} (deprecated)"
+		return option_str
+
+	def __str__(self):
+		options_str = (
+			f"{', '.join([self._mark_if_deprecated(o) for o in self.options])}"
+		)
+		return f"a {_type_name(self.type)} among {{{options_str}}}"
+
+
+class StrOptions(Options):
+	"""Constraint representing a finite set of strings.
+
+	Parameters
+	----------
+	options : set of str
+		The set of valid strings.
+
+	deprecated : set of str or None, default=None
+		A subset of the `options` to mark as deprecated in the string
+		representation of the constraint.
+	"""
+
+	def __init__(self, options, *, deprecated=None):
+		super().__init__(type=str, options=options, deprecated=deprecated)
+
+
+class Interval(_Constraint):
+	"""Constraint representing a typed interval.
+
+	Parameters
+	----------
+	type : {numbers.Integral, numbers.Real}
+		The set of numbers in which to set the interval.
+
+	left : float or int or None
+		The left bound of the interval. None means left bound is -∞.
+
+	right : float, int or None
+		The right bound of the interval. None means right bound is +∞.
+
+	closed : {"left", "right", "both", "neither"}
+		Whether the interval is open or closed. Possible choices are:
+
+		- `"left"`: the interval is closed on the left and open on the right.
+		  It is equivalent to the interval `[ left, right )`.
+		- `"right"`: the interval is closed on the right and open on the left.
+		  It is equivalent to the interval `( left, right ]`.
+		- `"both"`: the interval is closed.
+		  It is equivalent to the interval `[ left, right ]`.
+		- `"neither"`: the interval is open.
+		  It is equivalent to the interval `( left, right )`.
+
+	Notes
+	-----
+	Setting a bound to `None` and setting the interval closed is valid. For instance,
+	strictly speaking, `Interval(Real, 0, None, closed="both")` corresponds to
+	`[0, +∞) U {+∞}`.
+	"""
+
+	@validate_params(
+		{
+			"type": [type],
+			"left": [Integral, Real, None],
+			"right": [Integral, Real, None],
+			"closed": [StrOptions({"left", "right", "both", "neither"})],
+		}
+	)
+	def __init__(self, type, left, right, *, closed):
+		super().__init__()
+		self.type = type
+		self.left = left
+		self.right = right
+		self.closed = closed
+
+		self._check_params()
+
+	def _check_params(self):
+		if self.type is Integral:
+			suffix = "for an interval over the integers."
+			if self.left is not None and not isinstance(self.left, Integral):
+				raise TypeError(f"Expecting left to be an int {suffix}")
+			if self.right is not None and not isinstance(self.right, Integral):
+				raise TypeError(f"Expecting right to be an int {suffix}")
+			if self.left is None and self.closed in ("left", "both"):
+				raise ValueError(
+					f"left can't be None when closed == {self.closed} {suffix}"
+				)
+			if self.right is None and self.closed in ("right", "both"):
+				raise ValueError(
+					f"right can't be None when closed == {self.closed} {suffix}"
+				)
+
+		if self.right is not None and self.left is not None and self.right <= self.left:
+			raise ValueError(
+				f"right can't be less than left. Got left={self.left} and "
+				f"right={self.right}"
+			)
+
+	def __contains__(self, val):
+		if np.isnan(val):
+			return False
+
+		left_cmp = operator.lt if self.closed in ("left", "both") else operator.le
+		right_cmp = operator.gt if self.closed in ("right", "both") else operator.ge
+
+		left = -np.inf if self.left is None else self.left
+		right = np.inf if self.right is None else self.right
+
+		if left_cmp(val, left):
+			return False
+		if right_cmp(val, right):
+			return False
+		return True
+
+	def is_satisfied_by(self, val):
+		if not isinstance(val, self.type):
+			return False
+
+		return val in self
+
+	def __str__(self):
+		type_str = "an int" if self.type is Integral else "a float"
+		left_bracket = "[" if self.closed in ("left", "both") else "("
+		left_bound = "-inf" if self.left is None else self.left
+		right_bound = "inf" if self.right is None else self.right
+		right_bracket = "]" if self.closed in ("right", "both") else ")"
+		return (
+			f"{type_str} in the range "
+			f"{left_bracket}{left_bound}, {right_bound}{right_bracket}"
+		)
+
+
+class ConstrainedList(_Constraint):
+	"""
+	Added to allow for more control over constraints inside of a list of items 
+
+	This class indicates that an item contains a list of items, each constrained by the same constraint.
+	Has overlap with array-like constraint, but is more specific in that it indicates that the list is constrained
+	by the same constraint, rather than just being array-like
+
+	e.g.:
+	ConstrainedList([None, Interval(int, 0,10, closed='both')]) indicates a list of items, each of which is either None or
+	an int between 0 and 10
+	"""
+
+	def __init__(self, constraints):
+		super().__init__()
+		self.constraints : typing.List[_Constraint] = \
+			[make_constraint(constraint) for constraint in constraints] #Make constraints
+
+	@staticmethod
+	def create_using_constraint_objects(constraints : typing.List[_Constraint]):
+		"""Create a constrained list using a list of constraint objects.
+		The normal constructor expects a list of types, this one a list of constraint objects
+		"""
+		constrained_list = ConstrainedList([])
+		constrained_list.constraints = constraints
+		return constrained_list
+
+	def is_satisfied_by(self, val):
+		"""
+		Goes over all items in the list and checks if all constraints are satisfied by each item
+		"""
+		if not isinstance(val, list): #Must be list
+			return False
+
+		for cur_val in val:
+			for constraint in self.constraints:
+				if not constraint.is_satisfied_by(cur_val):
+					return False
+		return True
+
+	def __str__(self):
+		return f"a list of values, each {', '.join([str(c) for c in self.constraints])}"
+
+
+
+class _ArrayLikes(_Constraint):
+	"""Constraint representing array-likes"""
+
+	def is_satisfied_by(self, val):
+		return _is_arraylike_not_scalar(val)
+
+	def __str__(self):
+		return "an array-like"
+
+
+class _SparseMatrices(_Constraint):
+	"""Constraint representing sparse matrices."""
+
+	def is_satisfied_by(self, val):
+		#NOTE: to use, import from scipy.sparse import issparse #type:ignore
+		return issparse(val) #type:ignore #pylint: disable=undefined-variable
+
+	def __str__(self):
+		return "a sparse matrix"
+
+
+class _Callables(_Constraint):
+	"""Constraint representing callables."""
+
+	def is_satisfied_by(self, val):
+		return callable(val)
+
+	def __str__(self):
+		return "a callable"
+
+
+class _RandomStates(_Constraint):
+	"""Constraint representing random states.
+
+	Convenience class for
+	[Interval(Integral, 0, 2**32 - 1, closed="both"), np.random.RandomState, None]
+	"""
+
+	def __init__(self):
+		super().__init__()
+		self._constraints = [
+			Interval(Integral, 0, 2**32 - 1, closed="both"),
+			_InstancesOf(np.random.RandomState), #pylint: disable=no-member
+			_NoneConstraint(),
+		]
+
+	def is_satisfied_by(self, val):
+		return any(c.is_satisfied_by(val) for c in self._constraints)
+
+	def __str__(self):
+		return (
+			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
+			f" {self._constraints[-1]}"
+		)
+
+
+class _Booleans(_Constraint):
+	"""Constraint representing boolean likes.
+
+	Convenience class for
+	[bool, np.bool_, Integral (deprecated)]
+	"""
+
+	def __init__(self):
+		super().__init__()
+		self._constraints = [
+			_InstancesOf(bool),
+			_InstancesOf(np.bool_),
+			_InstancesOf(Integral),
+		]
+
+	def is_satisfied_by(self, val):
+		# TODO(1.4) remove support for Integral.
+		if isinstance(val, Integral) and not isinstance(val, bool):
+			warnings.warn(
+				"Passing an int for a boolean parameter is deprecated in version 1.2 "
+				"and won't be supported anymore in version 1.4.",
+				FutureWarning,
+			)
+
+		return any(c.is_satisfied_by(val) for c in self._constraints)
+
+	def __str__(self):
+		return (
+			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
+			f" {self._constraints[-1]}"
+		)
+
+
+class _VerboseHelper(_Constraint):
+	"""Helper constraint for the verbose parameter.
+
+	Convenience class for
+	[Interval(Integral, 0, None, closed="left"), bool, numpy.bool_]
+	"""
+
+	def __init__(self):
+		super().__init__()
+		self._constraints = [
+			Interval(Integral, 0, None, closed="left"),
+			_InstancesOf(bool),
+			_InstancesOf(np.bool_),
+		]
+
+	def is_satisfied_by(self, val):
+		return any(c.is_satisfied_by(val) for c in self._constraints)
+
+	def __str__(self):
+		return (
+			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
+			f" {self._constraints[-1]}"
+		)
+
+
+class _MissingValues(_Constraint):
+	"""Helper constraint for the `missing_values` parameters.
+
+	Convenience for
+	[
+		Integral,
+		Interval(Real, None, None, closed="both"),
+		str,
+		None,
+		_NanConstraint(),
+		_PandasNAConstraint(),
+	]
+	"""
+
+	def __init__(self):
+		super().__init__()
+		self._constraints = [
+			_InstancesOf(Integral),
+			# we use an interval of Real to ignore np.nan that has its own constraint
+			Interval(Real, None, None, closed="both"),
+			_InstancesOf(str),
+			_NoneConstraint(),
+			_NanConstraint(),
+			_PandasNAConstraint(),
+		]
+
+	def is_satisfied_by(self, val):
+		return any(c.is_satisfied_by(val) for c in self._constraints)
+
+	def __str__(self):
+		return (
+			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
+			f" {self._constraints[-1]}"
+		)
+
+
+class HasMethods(_Constraint):
+	"""Constraint representing objects that expose specific methods.
+
+	It is useful for parameters following a protocol and where we don't want to impose
+	an affiliation to a specific module or class.
+
+	Parameters
+	----------
+	methods : str or list of str
+		The method(s) that the object is expected to expose.
+	"""
+
+	@validate_params({"methods": [str, list]})
+	def __init__(self, methods):
+		super().__init__()
+		if isinstance(methods, str):
+			methods = [methods]
+		self.methods = methods
+
+	def is_satisfied_by(self, val):
+		return all(callable(getattr(val, method, None)) for method in self.methods)
+
+	def __str__(self):
+		if len(self.methods) == 1:
+			methods = f"{self.methods[0]!r}"
+		else:
+			methods = (
+				f"{', '.join([repr(m) for m in self.methods[:-1]])} and"
+				f" {self.methods[-1]!r}"
+			)
+		return f"an object implementing {methods}"
+
+
+class _IterablesNotString(_Constraint):
+	"""Constraint representing iterables that are not strings."""
+
+	def is_satisfied_by(self, val):
+		return isinstance(val, Iterable) and not isinstance(val, str)
+
+	def __str__(self):
+		return "an iterable"
+
+
+class _CVObjects(_Constraint):
+	"""Constraint representing cv objects.
+
+	Convenient class for
+	[
+		Interval(Integral, 2, None, closed="left"),
+		HasMethods(["split", "get_n_splits"]),
+		_IterablesNotString(),
+		None,
+	]
+	"""
+
+	def __init__(self):
+		super().__init__()
+		self._constraints = [
+			Interval(Integral, 2, None, closed="left"),
+			HasMethods(["split", "get_n_splits"]),
+			_IterablesNotString(),
+			_NoneConstraint(),
+		]
+
+	def is_satisfied_by(self, val):
+		return any(c.is_satisfied_by(val) for c in self._constraints)
+
+	def __str__(self):
+		return (
+			f"{', '.join([str(c) for c in self._constraints[:-1]])} or"
+			f" {self._constraints[-1]}"
+		)
+
+
+class Hidden:
+	"""Class encapsulating a constraint not meant to be exposed to the user.
+
+	Parameters
+	----------
+	constraint : str or _Constraint instance
+		The constraint to be used internally.
+	"""
+
+	def __init__(self, constraint):
+		self.constraint = constraint
+
+
+def generate_invalid_param_val(constraint, constraints=None):
+	"""Return a value that does not satisfy the constraint.
+
+	Raises a NotImplementedError if there exists no invalid value for this constraint.
+
+	This is only useful for testing purpose.
+
+	Parameters
+	----------
+	constraint : _Constraint instance
+		The constraint to generate a value for.
+
+	constraints : list of _Constraint instances or None, default=None
+		The list of all constraints for this parameter. If None, the list only
+		containing `constraint` is used.
+
+	Returns
+	-------
+	val : object
+		A value that does not satisfy the constraint.
+	"""
+	if isinstance(constraint, StrOptions):
+		return f"not {' or '.join(constraint.options)}"
+
+	if isinstance(constraint, _MissingValues):
+		return np.array([1, 2, 3])
+
+	if isinstance(constraint, _VerboseHelper):
+		return -1
+
+	if isinstance(constraint, HasMethods):
+		return type("HasNotMethods", (), {})()
+
+	if isinstance(constraint, _IterablesNotString):
+		return "a string"
+
+	if isinstance(constraint, _CVObjects):
+		return "not a cv object"
+
+	if not isinstance(constraint, Interval):
+		raise NotImplementedError
+
+	# constraint is an interval
+	constraints = [constraint] if constraints is None else constraints
+	return _generate_invalid_param_val_interval(constraint, constraints)
+
+
+def _generate_invalid_param_val_interval(interval, constraints):
+	"""Return a value that does not satisfy an interval constraint.
+
+	Generating an invalid value for an integer interval depends on the other constraints
+	since an int is a real, meaning that it can be valid for a real interval.
+	Assumes that there can be at most 2 interval constraints: one integer interval
+	and/or one real interval.
+
+	This is only useful for testing purpose.
+
+	Parameters
+	----------
+	interval : Interval instance
+		The interval to generate a value for.
+
+	constraints : list of _Constraint instances
+		The list of all constraints for this parameter.
+
+	Returns
+	-------
+	val : object
+		A value that does not satisfy the interval constraint.
+	"""
+	if interval.type is Real:
+		# generate a non-integer value such that it can't be valid even if there's also
+		# an integer interval constraint.
+		if interval.left is None and interval.right is None:
+			if interval.closed in ("left", "neither"):
+				return np.inf
+			elif interval.closed in ("right", "neither"):
+				return -np.inf
+			else:
+				raise NotImplementedError
+
+		if interval.left is not None:
+			return np.floor(interval.left) - 0.5
+		else:  # right is not None
+			return np.ceil(interval.right) + 0.5
+
+	else:  # interval.type is Integral
+		if interval.left is None and interval.right is None:
+			raise NotImplementedError
+
+		# We need to check if there's also a real interval constraint to generate a
+		# value that is not valid for any of the 2 interval constraints.
+		real_intervals = [
+			i for i in constraints if isinstance(i, Interval) and i.type is Real
+		]
+		real_interval = real_intervals[0] if real_intervals else None
+
+		if real_interval is None:
+			# Only the integer interval constraint -> easy
+			if interval.left is not None:
+				return interval.left - 1
+			else:  # interval.right is not None
+				return interval.right + 1
+
+		# There's also a real interval constraint. Try to find a value left to both or
+		# right to both or in between them.
+
+		# redefine left and right bounds to be smallest and largest valid integers in
+		# both intervals.
+		int_left = interval.left
+		if int_left is not None and interval.closed in ("right", "neither"):
+			int_left = int_left + 1
+
+		int_right = interval.right
+		if int_right is not None and interval.closed in ("left", "neither"):
+			int_right = int_right - 1
+
+		real_left = real_interval.left
+		if real_interval.left is not None:
+			real_left = int(np.ceil(real_interval.left))
+			if real_interval.closed in ("right", "neither"):
+				real_left = real_left + 1
+
+		real_right = real_interval.right
+		if real_interval.right is not None:
+			real_right = int(np.floor(real_interval.right))
+			if real_interval.closed in ("left", "neither"):
+				real_right = real_right - 1
+
+		if int_left is not None and real_left is not None:
+			# there exists an int left to both intervals
+			return min(int_left, real_left) - 1
+
+		if int_right is not None and real_right is not None:
+			# there exists an int right to both intervals
+			return max(int_right, real_right) + 1
+
+		if int_left is not None:
+			if real_right is not None and int_left - real_right >= 2:
+				# there exists an int between the 2 intervals
+				return int_left - 1
+			else:
+				raise NotImplementedError
+		else:  # int_right is not None
+			if real_left is not None and real_left - int_right >= 2:
+				# there exists an int between the 2 intervals
+				return int_right + 1
+			else:
+				raise NotImplementedError
+
+
+def generate_valid_param(constraint):
+	"""Return a value that does satisfy a constraint.
+
+	This is only useful for testing purpose.
+
+	Parameters
+	----------
+	constraint : Constraint instance
+		The constraint to generate a value for.
+
+	Returns
+	-------
+	val : object
+		A value that does satisfy the constraint.
+	"""
+	if isinstance(constraint, _ArrayLikes):
+		return np.array([1, 2, 3])
+
+	if isinstance(constraint, _SparseMatrices):
+		#NOTE: to use, import scipy.sparse import issparse: from scipy.sparse import csr_matrix
+		# Chose to comment this to make this module work without scipy
+		return csr_matrix([[0, 1], [1, 0]]) #pylint: disable=undefined-variable #type:ignore
+
+	if isinstance(constraint, _RandomStates):
+		return np.random.RandomState(42) #pylint: disable=no-member
+
+	if isinstance(constraint, _Callables):
+		return lambda x: x
+
+	if isinstance(constraint, _NoneConstraint):
+		return None
+
+	if isinstance(constraint, _InstancesOf):
+		return constraint.type()
+
+	if isinstance(constraint, _Booleans):
+		return True
+
+	if isinstance(constraint, _VerboseHelper):
+		return 1
+
+	if isinstance(constraint, _MissingValues):
+		return np.nan
+
+	if isinstance(constraint, HasMethods):
+		return type(
+			"ValidHasMethods", (), {m: lambda self: None for m in constraint.methods}
+		)()
+
+	if isinstance(constraint, _IterablesNotString):
+		return [1, 2, 3]
+
+	if isinstance(constraint, _CVObjects):
+		return 5
+
+	if isinstance(constraint, Options):  # includes StrOptions
+		for option in constraint.options:
+			return option
+
+	if isinstance(constraint, Interval):
+		interval = constraint
+		if interval.left is None and interval.right is None:
+			return 0
+		elif interval.left is None:
+			return interval.right - 1
+		elif interval.right is None:
+			return interval.left + 1
+		else:
+			if interval.type is Real:
+				return (interval.left + interval.right) / 2
+			else:
+				return interval.left + 1
+
+	raise ValueError(f"Unknown constraint type: {constraint}")
```

### Comparing `pyside6_utils-1.1.0/pyside6_utils/utility/serializable.py` & `pyside6_utils-1.2.0/pyside6_utils/classes/serializable.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/utility/signal_blocker.py` & `pyside6_utils-1.2.0/pyside6_utils/utility/signal_blocker.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/__init__.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-"""Make all widgets importable using <package>.widgets.<widget>"""
-from pyside6_utils.widgets.collapsible_group_box import CollapsibleGroupBox
-from pyside6_utils.widgets.console_widget import ConsoleWidget
-from pyside6_utils.widgets.dataclass_tree_view import DataClassTreeView
-from pyside6_utils.widgets.extended_mdi_area import ExtendedMdiArea
-from pyside6_utils.widgets.file_explorer_view import FileExplorerView
-from pyside6_utils.widgets.frameless_mdi_window import FramelessMdiWindow
-from pyside6_utils.widgets.overlay_widget import OverlayWidget
-from pyside6_utils.widgets.pandas_table_view import PandasTableView
-from pyside6_utils.widgets.range_selector import RangeSelector
-from pyside6_utils.widgets.square_frame import SquareFrame
+"""Make all widgets importable using <package>.widgets.<widget>"""
+from pyside6_utils.widgets.collapsible_group_box import CollapsibleGroupBox
+from pyside6_utils.widgets.console_widget import ConsoleWidget
+from pyside6_utils.widgets.dataclass_tree_view import DataClassTreeView
+from pyside6_utils.widgets.extended_mdi_area import ExtendedMdiArea
+from pyside6_utils.widgets.file_explorer_view import FileExplorerView
+from pyside6_utils.widgets.frameless_mdi_window import FramelessMdiWindow
+from pyside6_utils.widgets.overlay_widget import OverlayWidget
+from pyside6_utils.widgets.pandas_table_view import PandasTableView
+from pyside6_utils.widgets.range_selector import RangeSelector
+from pyside6_utils.widgets.square_frame import SquareFrame
+from pyside6_utils.widgets.widget_list import WidgetList
```

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/collapsible_group_box.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/collapsible_group_box.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/console_widget.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/console_widget.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/delegates/console_widget_delegate.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/delegates/console_widget_delegate.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/extended_mdi_area.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/extended_mdi_area.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/file_explorer_view.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/file_explorer_view.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/frameless_mdi_window.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/frameless_mdi_window.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,334 +1,334 @@
-"""Implements a frameless Qt MDI window while retaining the move/resize controls.
-A custom UI can be used, for more information, see the class documentation
-"""
-import enum
-import logging
-
-from PySide6 import QtCore, QtGui, QtWidgets
-
-from pyside6_utils.ui.FramelessMdiWindow_ui import Ui_FramelessMidiWindow
-
-log = logging.getLogger(__name__)
-
-class SideGrip(QtWidgets.QWidget):
-	""" Implements a grip for the sides of a window/mdi-window. Based on:
-	https://stackoverflow.com/questions/62807295/how-to-resize-a-window-from-the-edges-after-adding-the-property-qtcore-qt-framel
-	@musicamante
-
-	Adapter for use with a QMdiSubWindow. The parent of this widget should be the QMdiSubWindow.
-
-	TODO: also pass other window-rects to snap to edges?
-	"""
-	def __init__(self, parent, edge):
-		QtWidgets.QWidget.__init__(self, parent)
-		if edge == QtCore.Qt.Edge.LeftEdge:
-			self.setCursor(QtCore.Qt.CursorShape.SizeHorCursor)
-			self.resize_func = self.resize_left
-		elif edge == QtCore.Qt.Edge.TopEdge:
-			self.setCursor(QtCore.Qt.CursorShape.SizeVerCursor)
-			self.resize_func = self.resize_top
-		elif edge == QtCore.Qt.Edge.RightEdge:
-			self.setCursor(QtCore.Qt.CursorShape.SizeHorCursor)
-			self.resize_func = self.resize_right
-		else:
-			self.setCursor(QtCore.Qt.CursorShape.SizeVerCursor)
-			self.resize_func = self.resize_bottom
-		self.mouse_pos = None
-
-	def resize_left(self, delta):
-		"""Resize the window to the left"""
-		window = self.parent()
-		assert isinstance(window, QtWidgets.QMdiSubWindow)
-		width = max(window.minimumWidth(), window.width() - delta.x()) #TODO: minimumsize does not seem to work?
-		geo = window.geometry()
-		geo.setLeft(geo.right() - width)
-		window.setGeometry(geo)
-
-	def resize_top(self, delta):
-		"""Resize the window to the top"""
-		window = self.parent()
-		assert isinstance(window, QtWidgets.QMdiSubWindow)
-		height = max(window.minimumHeight(), window.height() - delta.y())
-		geo = window.geometry()
-		geo.setTop(geo.bottom() - height)
-		window.setGeometry(geo)
-
-	def resize_right(self, delta):
-		"""Resize the window to the right"""
-		window = self.parent()
-		assert isinstance(window, QtWidgets.QMdiSubWindow)
-		width = max(window.minimumWidth(), window.width() + delta.x())
-		window.resize(width, window.height())
-
-	def resize_bottom(self, delta):
-		"""Resize the window to the bottom"""
-		window = self.parent()
-		assert isinstance(window, QtWidgets.QMdiSubWindow)
-		height = max(window.minimumHeight(), window.height() + delta.y())
-		window.resize(window.width(), height)
-
-	def mousePressEvent(self, event):
-		if event.button() == QtCore.Qt.MouseButton.LeftButton:
-			self.mouse_pos = event.position()
-
-	def mouseMoveEvent(self, event):
-		if self.mouse_pos is not None:
-			delta = event.position() - self.mouse_pos
-			self.resize_func(delta)
-
-	def mouseReleaseEvent(self, event): #pylint: disable=unused-argument
-		self.mouse_pos = None
-
-class FramelessMdiWindow(QtWidgets.QMdiSubWindow):
-	"""Implementation of a borderless Mdi-window using a custom UI.
-
-	Note that the following items should be present in the passed ui, if using a custom ui:
-		- contentLayout (QtWidgets.QLayout): The layout that will be used to add the content-widget
-		- titleBar (QtWidgets.QWidget): The widget that will be used as the title bar, should contain the following:
-			- titleLabel (QtWidgets.QLabel): The label that will be used to display the title
-			- zoomButton (QtWidget.QButtton): If pressed, set window to fullscreen
-			- minimizeButton (QtWidget.QButtton): If pressed, minimize the window
-
-
-	If the parent of the window is ExtendedMdiArea, the following functionality will be added:
-		- Right-clicking the titlebar will show the context menu for the mdi-area
-		- When tabbified, the titlebar and grips will be hidden and window will be unmovable
-
-	"""
-	class DragType(enum.Enum):
-		"""When a click-move is considered a Mdi-window-move"""
-		TITLE_BAR = 0
-		EVERYWHERE = enum.auto()
-
-	def __init__(self,
-	      		parent: QtWidgets.QWidget | None = None,
-		  		flags: QtCore.Qt.WindowType = ..., #pylint: disable=unused-argument
-		  		drag_type: DragType = DragType.TITLE_BAR,
-				ui_class : type[Ui_FramelessMidiWindow | None] = Ui_FramelessMidiWindow,
-				keep_inside_mdi_area : bool = True,
-				resizeable_pix_size : int = 8, #The size of the resizeable area in pixels (around the edges), 0 for off
-				moveable = True
-			) -> None:
-		super().__init__(parent)
-
-		self.content = QtWidgets.QWidget()
-
-		if ui_class is type(None):
-			self.ui =  Ui_FramelessMidiWindow() #pylint: disable=invalid-name
-		else:
-			self.ui : Ui_FramelessMidiWindow = ui_class() #type: ignore
-
-		assert self.ui is not None
-		self.ui.setupUi(self.content)
-		super().setWidget(self.content)
-		self.setGeometry(self.content.geometry()) #Copy over initial geometry of the window
-
-		self.setWindowFlags(QtCore.Qt.WindowType.FramelessWindowHint)
-		self.start_mouse_pos = None
-		self.start_window_pos = None
-		self._drag_type = drag_type
-		self._widget = None
-		self._keep_inside_mdi_area = keep_inside_mdi_area
-		self._resizable_pix_size = resizeable_pix_size
-		self._moveable = moveable
-
-		self.corner_grips : list[QtWidgets.QSizeGrip]= []
-		for _ in range(4):
-			grip = QtWidgets.QSizeGrip(self)
-			grip.resize(self._resizable_pix_size, self._resizable_pix_size)
-			grip.setStyleSheet("QSizeGrip { image: None;}") #Disable grip icon
-			grip.setWindowFlag(QtCore.Qt.WindowType.WindowStaysOnTopHint)
-			self.corner_grips.append(grip)
-
-		self._edge_grips : dict[QtCore.Qt.Edge, SideGrip] = {}
-		for edge in [QtCore.Qt.Edge.LeftEdge, QtCore.Qt.Edge.TopEdge, QtCore.Qt.Edge.RightEdge, QtCore.Qt.Edge.BottomEdge]:
-			self._edge_grips[edge] = SideGrip(self, edge)
-			self._edge_grips[edge].setWindowFlag(QtCore.Qt.WindowType.WindowStaysOnTopHint)
-
-		self.ui.titleBar.setContextMenuPolicy(QtCore.Qt.ContextMenuPolicy.CustomContextMenu)
-		self.ui.titleBar.customContextMenuRequested.connect(self.mdi_context_menu_requested)
-
-		self.ui.zoomButton.clicked.connect(self.toggle_zoom)
-		self.ui.MinimizeButton.clicked.connect(self.showMinimized)
-
-	def set_moveable(self, moveable: bool) -> None:
-		"""Sets whether the window can be moved"""
-		self._moveable = moveable
-		if not moveable: #Also rest the current start positions
-			self.start_mouse_pos = None
-			self.start_window_pos = None
-
-	def setWindowTitle(self, arg__1: str) -> None:
-		self.ui.titleLabel.setText(arg__1)
-		return super().setWindowTitle(arg__1)
-
-	def showNormal(self) -> None:
-		"""When showing normal -> enable grips"""
-		for grip in self.corner_grips:
-			grip.show()
-		for grip in self._edge_grips.values():
-			grip.show()
-		return super().showNormal()
-
-	def showMaximized(self) -> None:
-		"""When showing maximized -> disable grips"""
-		for grip in self.corner_grips:
-			grip.hide()
-		for grip in self._edge_grips.values():
-			grip.hide()
-		return super().showMaximized()
-
-	def toggle_zoom(self):
-		"""Zooms in/out on the window"""
-		if self.isMaximized():
-			self.showNormal()
-		else:
-			self.showMaximized()
-
-	def set_tabbed_mode(self, tabbed: bool) -> None:
-		"""Sets the tabbed mode of this item, hiding the titlebar and grips/buttons"""
-		self.ui.titleBar.setEnabled(not tabbed)
-		self.ui.titleBar.setVisible(not tabbed)
-		for grip in self.corner_grips:
-			grip.setEnabled(not tabbed)
-		for grip in self._edge_grips.values():
-			grip.setEnabled(not tabbed)
-		self.set_moveable(not tabbed)
-
-	def mdi_context_menu_requested(self, pos: QtCore.QPoint) -> None:
-		"""Pass on context menu to parent (QMdiArea) - tile/cascade etc. 
-		"""
-		parent = self.mdiArea()
-		pos = self.ui.titleBar.mapToGlobal(pos)
-		pos = parent.mapFromGlobal(pos)
-		try:
-			parent.context_menu_requested(pos)
-		except AttributeError:
-			log.debug("Parent of FramelessMdiWindow is not an ExtendedMdiArea, context menu not shown")
-
-	def resizeEvent(self, resizeEvent: QtGui.QResizeEvent) -> None:
-		"""Upon resize, make sure that all grips are at the right position"""
-		super().resizeEvent(resizeEvent)
-		rect = self.rect()
-		self.corner_grips[0].move(rect.topLeft()) # + QtCore.QPoint(self., self._resizable_pix_size))
-		self.corner_grips[1].move(rect.topRight() + QtCore.QPoint(-self._resizable_pix_size, 0))
-		self.corner_grips[2].move(rect.bottomLeft() - QtCore.QPoint(0, self._resizable_pix_size))
-		self.corner_grips[3].move(rect.bottomRight() - QtCore.QPoint(self._resizable_pix_size, self._resizable_pix_size))
-
-		#Also resize/move the edge-grips
-		self._edge_grips[QtCore.Qt.Edge.LeftEdge].setGeometry(
-			0,
-			self._resizable_pix_size,
-			self._resizable_pix_size,
-			self.height() - 2*self._resizable_pix_size
-		)
-		self._edge_grips[QtCore.Qt.Edge.TopEdge].setGeometry(
-			self._resizable_pix_size,
-			0,
-			self.width() - 2*self._resizable_pix_size,
-			self._resizable_pix_size
-		)
-		self._edge_grips[QtCore.Qt.Edge.RightEdge].setGeometry(
-			self.width() - self._resizable_pix_size,
-			self._resizable_pix_size,
-			self._resizable_pix_size,
-			self.height() - 2*self._resizable_pix_size
-		)
-		self._edge_grips[QtCore.Qt.Edge.BottomEdge].setGeometry(
-			self._resizable_pix_size,
-			self.height() - self._resizable_pix_size,
-			self.width() - 2*self._resizable_pix_size,
-			self._resizable_pix_size
-		)
-
-
-
-	def setWidget(self, widget: QtWidgets.QWidget) -> None:
-		if self._widget is not None: #Set new content
-			self.ui.contentLayout.removeWidget(self._widget)
-		self.ui.contentLayout.insertWidget(0, widget) #Always insert at 0, so we can add a spacer to the bottom
-		self._widget = widget
-		self._widget.lower()
-		# self._widget.setParent(self)
-		self._widget.show()
-
-
-	def mousePressEvent(self, event: QtGui.QMouseEvent) -> bool:
-		global_mouse_pos = event.globalPosition() #mouse move results in movement so use global position to
-			#avoid shaking motion
-		if not self._moveable:
-			return super().mousePressEvent(event) #type: ignore
-		#If left-click, check if on titlebar
-		if event.button() == QtCore.Qt.MouseButton.LeftButton:
-			if self._drag_type == self.DragType.TITLE_BAR and\
-					self.ui.titleBar.rect().contains(self.ui.titleBar.mapFromGlobal(global_mouse_pos).toPoint()):
-				self.start_mouse_pos = event.globalPosition().toPoint()
-				self.start_window_pos = self.pos()
-			elif self._drag_type == self.DragType.EVERYWHERE:
-				self.start_mouse_pos = event.globalPosition().toPoint()
-				self.start_window_pos = self.pos()
-		elif event.button() == QtCore.Qt.MouseButton.RightButton and\
-				self.ui.titleBar.rect().contains(self.ui.titleBar.mapFromGlobal(global_mouse_pos).toPoint()):
-			self.mdi_context_menu_requested(event.position().toPoint())
-		return True
-
-	def mouseReleaseEvent(self, mouseEvent: QtGui.QMouseEvent) -> bool: #pylint: disable=unused-argument
-		self.start_mouse_pos = None
-		self.start_window_pos = None
-		return True
-
-	def mouseMoveEvent(self, event: QtGui.QMouseEvent) -> None:
-		if self.start_mouse_pos is None or self.start_window_pos is None: #If
-			return
-		delta = QtCore.QPoint(event.globalPosition().toPoint() - self.start_mouse_pos)
-		new_window_pos = self.start_window_pos + delta
-		#Check if outside of mdi-area, if so, move to edge
-		if self._keep_inside_mdi_area:
-			parent = self.mdiArea()
-			if parent is not None and issubclass(type(parent), QtWidgets.QMdiArea):
-				assert isinstance(parent, QtWidgets.QMdiArea)
-				#Check if outside of parent
-				new_bottom_right = new_window_pos + self.rect().bottomRight()
-				if not parent.rect().contains(new_window_pos) or not parent.rect().contains(new_bottom_right):
-					new_window_pos = QtCore.QPoint(
-						min(max(parent.rect().left(), new_window_pos.x()), parent.rect().right() - self.width()),
-						min(max(parent.rect().top(), new_window_pos.y()), parent.rect().bottom() - self.height())
-					)
-					self.move(new_window_pos)
-					# self.start_mouse_pos = event.globalPosition().toPoint()
-					return
-		self.move(new_window_pos)
-
-def run_example_app():
-	"""Show example frameless window in a normal mdi area - for more functionality, see extended_mdi_area.py"""
-	#pylint: disable=import-outside-toplevel
-	import sys
-	app = QtWidgets.QApplication(sys.argv)
-	mdi_area = QtWidgets.QMdiArea()
-	mdi_area.show()
-	test_window = FramelessMdiWindow()
-	# test_window = QtWidgets.QMdiSubWindow()
-	label = QtWidgets.QLabel(" Test \n Test \n Test ")
-	label.setFont(QtGui.QFont("Arial", 50))
-	test_window.setWidget(label)
-	mdi_area.addSubWindow(test_window)
-	test_window.show()
-
-	#center window to screen
-	screen = app.primaryScreen()
-	screen_size = screen.size()
-	window_size = mdi_area.size()
-	mdi_area.move((screen_size.width() - window_size.width()) // 2,
-				(screen_size.height() - window_size.height()) // 2)
-	sys.exit(app.exec())
-
-
-
-if __name__ == "__main__":
-	formatter = logging.Formatter("[{pathname:>90s}:{lineno:<4}]  {levelname:<7s}   {message}", style='{')
-	handler = logging.StreamHandler()
-	handler.setFormatter(formatter)
-	logging.basicConfig(
-		handlers=[handler],
-		level=logging.DEBUG) #Without time
+"""Implements a frameless Qt MDI window while retaining the move/resize controls.
+A custom UI can be used, for more information, see the class documentation
+"""
+import enum
+import logging
+
+from PySide6 import QtCore, QtGui, QtWidgets
+
+from pyside6_utils.ui.FramelessMdiWindow_ui import Ui_FramelessMidiWindow
+
+log = logging.getLogger(__name__)
+
+class SideGrip(QtWidgets.QWidget):
+	""" Implements a grip for the sides of a window/mdi-window. Based on:
+	https://stackoverflow.com/questions/62807295/how-to-resize-a-window-from-the-edges-after-adding-the-property-qtcore-qt-framel
+	@musicamante
+
+	Adapter for use with a QMdiSubWindow. The parent of this widget should be the QMdiSubWindow.
+
+	TODO: also pass other window-rects to snap to edges?
+	"""
+	def __init__(self, parent, edge):
+		QtWidgets.QWidget.__init__(self, parent)
+		if edge == QtCore.Qt.Edge.LeftEdge:
+			self.setCursor(QtCore.Qt.CursorShape.SizeHorCursor)
+			self.resize_func = self.resize_left
+		elif edge == QtCore.Qt.Edge.TopEdge:
+			self.setCursor(QtCore.Qt.CursorShape.SizeVerCursor)
+			self.resize_func = self.resize_top
+		elif edge == QtCore.Qt.Edge.RightEdge:
+			self.setCursor(QtCore.Qt.CursorShape.SizeHorCursor)
+			self.resize_func = self.resize_right
+		else:
+			self.setCursor(QtCore.Qt.CursorShape.SizeVerCursor)
+			self.resize_func = self.resize_bottom
+		self.mouse_pos = None
+
+	def resize_left(self, delta):
+		"""Resize the window to the left"""
+		window = self.parent()
+		assert isinstance(window, QtWidgets.QMdiSubWindow)
+		width = max(window.minimumWidth(), window.width() - delta.x()) #TODO: minimumsize does not seem to work?
+		geo = window.geometry()
+		geo.setLeft(geo.right() - width)
+		window.setGeometry(geo)
+
+	def resize_top(self, delta):
+		"""Resize the window to the top"""
+		window = self.parent()
+		assert isinstance(window, QtWidgets.QMdiSubWindow)
+		height = max(window.minimumHeight(), window.height() - delta.y())
+		geo = window.geometry()
+		geo.setTop(geo.bottom() - height)
+		window.setGeometry(geo)
+
+	def resize_right(self, delta):
+		"""Resize the window to the right"""
+		window = self.parent()
+		assert isinstance(window, QtWidgets.QMdiSubWindow)
+		width = max(window.minimumWidth(), window.width() + delta.x())
+		window.resize(width, window.height())
+
+	def resize_bottom(self, delta):
+		"""Resize the window to the bottom"""
+		window = self.parent()
+		assert isinstance(window, QtWidgets.QMdiSubWindow)
+		height = max(window.minimumHeight(), window.height() + delta.y())
+		window.resize(window.width(), height)
+
+	def mousePressEvent(self, event):
+		if event.button() == QtCore.Qt.MouseButton.LeftButton:
+			self.mouse_pos = event.position()
+
+	def mouseMoveEvent(self, event):
+		if self.mouse_pos is not None:
+			delta = event.position() - self.mouse_pos
+			self.resize_func(delta)
+
+	def mouseReleaseEvent(self, event): #pylint: disable=unused-argument
+		self.mouse_pos = None
+
+class FramelessMdiWindow(QtWidgets.QMdiSubWindow):
+	"""Implementation of a borderless Mdi-window using a custom UI.
+
+	Note that the following items should be present in the passed ui, if using a custom ui:
+		- contentLayout (QtWidgets.QLayout): The layout that will be used to add the content-widget
+		- titleBar (QtWidgets.QWidget): The widget that will be used as the title bar, should contain the following:
+			- titleLabel (QtWidgets.QLabel): The label that will be used to display the title
+			- zoomButton (QtWidget.QButtton): If pressed, set window to fullscreen
+			- minimizeButton (QtWidget.QButtton): If pressed, minimize the window
+
+
+	If the parent of the window is ExtendedMdiArea, the following functionality will be added:
+		- Right-clicking the titlebar will show the context menu for the mdi-area
+		- When tabbified, the titlebar and grips will be hidden and window will be unmovable
+
+	"""
+	class DragType(enum.Enum):
+		"""When a click-move is considered a Mdi-window-move"""
+		TITLE_BAR = 0
+		EVERYWHERE = enum.auto()
+
+	def __init__(self,
+	      		parent: QtWidgets.QWidget | None = None,
+		  		flags: QtCore.Qt.WindowType = ..., #pylint: disable=unused-argument
+		  		drag_type: DragType = DragType.TITLE_BAR,
+				ui_class : type[Ui_FramelessMidiWindow | None] = Ui_FramelessMidiWindow,
+				keep_inside_mdi_area : bool = True,
+				resizeable_pix_size : int = 8, #The size of the resizeable area in pixels (around the edges), 0 for off
+				moveable = True
+			) -> None:
+		super().__init__(parent)
+
+		self.content = QtWidgets.QWidget()
+
+		if ui_class is type(None):
+			self.ui =  Ui_FramelessMidiWindow() #pylint: disable=invalid-name
+		else:
+			self.ui : Ui_FramelessMidiWindow = ui_class() #type: ignore
+
+		assert self.ui is not None
+		self.ui.setupUi(self.content)
+		super().setWidget(self.content)
+		self.setGeometry(self.content.geometry()) #Copy over initial geometry of the window
+
+		self.setWindowFlags(QtCore.Qt.WindowType.FramelessWindowHint)
+		self.start_mouse_pos = None
+		self.start_window_pos = None
+		self._drag_type = drag_type
+		self._widget = None
+		self._keep_inside_mdi_area = keep_inside_mdi_area
+		self._resizable_pix_size = resizeable_pix_size
+		self._moveable = moveable
+
+		self.corner_grips : list[QtWidgets.QSizeGrip]= []
+		for _ in range(4):
+			grip = QtWidgets.QSizeGrip(self)
+			grip.resize(self._resizable_pix_size, self._resizable_pix_size)
+			grip.setStyleSheet("QSizeGrip { image: None;}") #Disable grip icon
+			grip.setWindowFlag(QtCore.Qt.WindowType.WindowStaysOnTopHint)
+			self.corner_grips.append(grip)
+
+		self._edge_grips : dict[QtCore.Qt.Edge, SideGrip] = {}
+		for edge in [QtCore.Qt.Edge.LeftEdge, QtCore.Qt.Edge.TopEdge, QtCore.Qt.Edge.RightEdge, QtCore.Qt.Edge.BottomEdge]:
+			self._edge_grips[edge] = SideGrip(self, edge)
+			self._edge_grips[edge].setWindowFlag(QtCore.Qt.WindowType.WindowStaysOnTopHint)
+
+		self.ui.titleBar.setContextMenuPolicy(QtCore.Qt.ContextMenuPolicy.CustomContextMenu)
+		self.ui.titleBar.customContextMenuRequested.connect(self.mdi_context_menu_requested)
+
+		self.ui.zoomButton.clicked.connect(self.toggle_zoom)
+		self.ui.MinimizeButton.clicked.connect(self.showMinimized)
+
+	def set_moveable(self, moveable: bool) -> None:
+		"""Sets whether the window can be moved"""
+		self._moveable = moveable
+		if not moveable: #Also rest the current start positions
+			self.start_mouse_pos = None
+			self.start_window_pos = None
+
+	def setWindowTitle(self, arg__1: str) -> None:
+		self.ui.titleLabel.setText(arg__1)
+		return super().setWindowTitle(arg__1)
+
+	def showNormal(self) -> None:
+		"""When showing normal -> enable grips"""
+		for grip in self.corner_grips:
+			grip.show()
+		for grip in self._edge_grips.values():
+			grip.show()
+		return super().showNormal()
+
+	def showMaximized(self) -> None:
+		"""When showing maximized -> disable grips"""
+		for grip in self.corner_grips:
+			grip.hide()
+		for grip in self._edge_grips.values():
+			grip.hide()
+		return super().showMaximized()
+
+	def toggle_zoom(self):
+		"""Zooms in/out on the window"""
+		if self.isMaximized():
+			self.showNormal()
+		else:
+			self.showMaximized()
+
+	def set_tabbed_mode(self, tabbed: bool) -> None:
+		"""Sets the tabbed mode of this item, hiding the titlebar and grips/buttons"""
+		self.ui.titleBar.setEnabled(not tabbed)
+		self.ui.titleBar.setVisible(not tabbed)
+		for grip in self.corner_grips:
+			grip.setEnabled(not tabbed)
+		for grip in self._edge_grips.values():
+			grip.setEnabled(not tabbed)
+		self.set_moveable(not tabbed)
+
+	def mdi_context_menu_requested(self, pos: QtCore.QPoint) -> None:
+		"""Pass on context menu to parent (QMdiArea) - tile/cascade etc. 
+		"""
+		parent = self.mdiArea()
+		pos = self.ui.titleBar.mapToGlobal(pos)
+		pos = parent.mapFromGlobal(pos)
+		try:
+			parent.context_menu_requested(pos) #type: ignore
+		except AttributeError:
+			log.debug("Parent of FramelessMdiWindow is not an ExtendedMdiArea, context menu not shown")
+
+	def resizeEvent(self, resizeEvent: QtGui.QResizeEvent) -> None:
+		"""Upon resize, make sure that all grips are at the right position"""
+		super().resizeEvent(resizeEvent)
+		rect = self.rect()
+		self.corner_grips[0].move(rect.topLeft()) # + QtCore.QPoint(self., self._resizable_pix_size))
+		self.corner_grips[1].move(rect.topRight() + QtCore.QPoint(-self._resizable_pix_size, 0))
+		self.corner_grips[2].move(rect.bottomLeft() - QtCore.QPoint(0, self._resizable_pix_size))
+		self.corner_grips[3].move(rect.bottomRight() - QtCore.QPoint(self._resizable_pix_size, self._resizable_pix_size))
+
+		#Also resize/move the edge-grips
+		self._edge_grips[QtCore.Qt.Edge.LeftEdge].setGeometry(
+			0,
+			self._resizable_pix_size,
+			self._resizable_pix_size,
+			self.height() - 2*self._resizable_pix_size
+		)
+		self._edge_grips[QtCore.Qt.Edge.TopEdge].setGeometry(
+			self._resizable_pix_size,
+			0,
+			self.width() - 2*self._resizable_pix_size,
+			self._resizable_pix_size
+		)
+		self._edge_grips[QtCore.Qt.Edge.RightEdge].setGeometry(
+			self.width() - self._resizable_pix_size,
+			self._resizable_pix_size,
+			self._resizable_pix_size,
+			self.height() - 2*self._resizable_pix_size
+		)
+		self._edge_grips[QtCore.Qt.Edge.BottomEdge].setGeometry(
+			self._resizable_pix_size,
+			self.height() - self._resizable_pix_size,
+			self.width() - 2*self._resizable_pix_size,
+			self._resizable_pix_size
+		)
+
+
+
+	def setWidget(self, widget: QtWidgets.QWidget) -> None:
+		if self._widget is not None: #Set new content
+			self.ui.contentLayout.removeWidget(self._widget)
+		self.ui.contentLayout.insertWidget(0, widget) #Always insert at 0, so we can add a spacer to the bottom
+		self._widget = widget
+		self._widget.lower()
+		# self._widget.setParent(self)
+		self._widget.show()
+
+
+	def mousePressEvent(self, event: QtGui.QMouseEvent) -> bool:
+		global_mouse_pos = event.globalPosition() #mouse move results in movement so use global position to
+			#avoid shaking motion
+		if not self._moveable:
+			return super().mousePressEvent(event) #type: ignore
+		#If left-click, check if on titlebar
+		if event.button() == QtCore.Qt.MouseButton.LeftButton:
+			if self._drag_type == self.DragType.TITLE_BAR and\
+					self.ui.titleBar.rect().contains(self.ui.titleBar.mapFromGlobal(global_mouse_pos).toPoint()):
+				self.start_mouse_pos = event.globalPosition().toPoint()
+				self.start_window_pos = self.pos()
+			elif self._drag_type == self.DragType.EVERYWHERE:
+				self.start_mouse_pos = event.globalPosition().toPoint()
+				self.start_window_pos = self.pos()
+		elif event.button() == QtCore.Qt.MouseButton.RightButton and\
+				self.ui.titleBar.rect().contains(self.ui.titleBar.mapFromGlobal(global_mouse_pos).toPoint()):
+			self.mdi_context_menu_requested(event.position().toPoint())
+		return True
+
+	def mouseReleaseEvent(self, mouseEvent: QtGui.QMouseEvent) -> bool: #pylint: disable=unused-argument
+		self.start_mouse_pos = None
+		self.start_window_pos = None
+		return True
+
+	def mouseMoveEvent(self, event: QtGui.QMouseEvent) -> None:
+		if self.start_mouse_pos is None or self.start_window_pos is None: #If
+			return
+		delta = QtCore.QPoint(event.globalPosition().toPoint() - self.start_mouse_pos)
+		new_window_pos = self.start_window_pos + delta
+		#Check if outside of mdi-area, if so, move to edge
+		if self._keep_inside_mdi_area:
+			parent = self.mdiArea()
+			if parent is not None and issubclass(type(parent), QtWidgets.QMdiArea):
+				assert isinstance(parent, QtWidgets.QMdiArea)
+				#Check if outside of parent
+				new_bottom_right = new_window_pos + self.rect().bottomRight()
+				if not parent.rect().contains(new_window_pos) or not parent.rect().contains(new_bottom_right):
+					new_window_pos = QtCore.QPoint(
+						min(max(parent.rect().left(), new_window_pos.x()), parent.rect().right() - self.width()),
+						min(max(parent.rect().top(), new_window_pos.y()), parent.rect().bottom() - self.height())
+					)
+					self.move(new_window_pos)
+					# self.start_mouse_pos = event.globalPosition().toPoint()
+					return
+		self.move(new_window_pos)
+
+def run_example_app():
+	"""Show example frameless window in a normal mdi area - for more functionality, see extended_mdi_area.py"""
+	#pylint: disable=import-outside-toplevel
+	import sys
+	app = QtWidgets.QApplication(sys.argv)
+	mdi_area = QtWidgets.QMdiArea()
+	mdi_area.show()
+	test_window = FramelessMdiWindow()
+	# test_window = QtWidgets.QMdiSubWindow()
+	label = QtWidgets.QLabel(" Test \n Test \n Test ")
+	label.setFont(QtGui.QFont("Arial", 50))
+	test_window.setWidget(label)
+	mdi_area.addSubWindow(test_window)
+	test_window.show()
+
+	#center window to screen
+	screen = app.primaryScreen()
+	screen_size = screen.size()
+	window_size = mdi_area.size()
+	mdi_area.move((screen_size.width() - window_size.width()) // 2,
+				(screen_size.height() - window_size.height()) // 2)
+	sys.exit(app.exec())
+
+
+
+if __name__ == "__main__":
+	formatter = logging.Formatter("[{pathname:>90s}:{lineno:<4}]  {levelname:<7s}   {message}", style='{')
+	handler = logging.StreamHandler()
+	handler.setFormatter(formatter)
+	logging.basicConfig(
+		handlers=[handler],
+		level=logging.DEBUG) #Without time
 	run_example_app()
```

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/overlay_widget.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/overlay_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,146 @@
-"""Implements an overlay widget that acts as a container but allows displaying another widget on top of it."""
-
-import logging
-
-from PySide6 import QtCore, QtGui, QtWidgets
-from PySide6.QtCore import Qt
-
-log = logging.getLogger(__name__)
-
-class OverlayWidget(QtWidgets.QWidget):
-	"""
-	Container-like widget which allows the user to overlay another widget on top of it. Switching on/off the overlay
-	widget is done by setting the overlayHidden property.
-	"""
-
-	DESCRIPTION = "Basic QtWidget that allows displaying another widget on top of it using setOverlayWidget."
-
-
-	def __init__(self, parent: QtWidgets.QWidget | None) -> None:
-		super().__init__(parent)
-
-		self._display_overlay = False
-		self._overlay_widget = None
-		self._overlay_widget_container: QtWidgets.QWidget = QtWidgets.QWidget(self)
-		self._overlay_widget_container.setParent(self)
-		self._overlay_widget_container.setWindowFlags(Qt.WindowType.Widget | Qt.WindowType.FramelessWindowHint)
-		self._overlay_widget_container.setAutoFillBackground(True)
-		self._overlay_widget_container.setContentsMargins(0, 0, 0, 0)
-		self._overlay_widget_container.raise_()
-
-		self._cur_background_color = None
-		self.set_overlay_mouse_block(True)
-		self.set_background_color(QtGui.QColor(200, 200, 200, 150))
-
-
-	def set_overlay_mouse_block(self, block: bool) -> None:
-		"""Sets whether the overlay widget should block mouse events from reaching the underlying widget."""
-		self._overlay_widget_container.setAttribute(Qt.WidgetAttribute.WA_TransparentForMouseEvents, not block)
-
-	def get_overlay_mouse_block(self) -> bool:
-		"""Returns whether the overlay widget blocks mouse events from reaching the underlying widget."""
-		return self._overlay_widget_container.testAttribute(Qt.WidgetAttribute.WA_TransparentForMouseEvents)
-
-	def showEvent(self, event: QtGui.QShowEvent) -> None:
-		"""On show, raise the overlay widget to make sure it is on top."""
-		self._overlay_widget_container.raise_() #Make sure the overlay widget is on top
-		return super().showEvent(event)
-
-
-	def set_overlay_widget(self, overlay_widget: QtWidgets.QWidget) -> None:
-		"""
-		Sets the overlay widget to display on top of this widget.
-		"""
-		self._overlay_widget = overlay_widget
-		self._overlay_widget_container.setLayout(QtWidgets.QVBoxLayout()) #Reset the layout to remove any previous
-		self._overlay_widget_container.layout().addWidget(overlay_widget)
-		self._overlay_widget_container.resize(self.size())
-		self._overlay_widget_container.layout().setAlignment(Qt.AlignmentFlag.AlignCenter)
-		self._overlay_widget_container.raise_()
-
-
-	def resizeEvent(self, event: QtGui.QResizeEvent) -> None:
-		"""
-		#On resize, update the overlay widget size
-		"""
-		super().resizeEvent(event)
-		self._overlay_widget_container.resize(self.size())
-
-	def set_overlay_hidden(self, hidden: bool) -> None:
-		"""
-		Sets the overlay widget to be hidden or visible.
-		"""
-		self._overlay_widget_container.setHidden(hidden)
-
-	def get_overlay_hidden(self) -> bool:
-		"""
-		Returns whether the overlay widget is hidden or visible.
-		"""
-		return self._overlay_widget_container.isHidden()
-
-
-	def set_background_color(self, color: QtGui.QColor) -> None:
-		"""
-		Sets the background color of the overlay widget.
-		"""
-		self._cur_background_color = color
-		style = QtWidgets.QApplication.style()
-		palette = style.standardPalette()
-		palette.setColor(QtGui.QPalette.ColorRole.Window, color) #Background color
-		self._overlay_widget_container.setPalette(palette)
-	def get_background_color(self) -> QtGui.QColor | None:
-		"""
-		Returns the background color of the overlay widget.
-		"""
-		return self._cur_background_color
-
-	overlayHidden = QtCore.Property(bool, get_overlay_hidden, set_overlay_hidden)
-	overlayBlocksMouse = QtCore.Property(bool, get_overlay_mouse_block, set_overlay_mouse_block)
-
-	overlayBackgroundColor = QtCore.Property(QtGui.QColor, get_background_color, set_background_color)
-
-
-
-def run_example_app():
-	"""Creates a qt-app instance and runs the example"""
-	log.info(f"Running example app for {OverlayWidget.__name__}...")
-
-	app = QtWidgets.QApplication([])
-	widget = OverlayWidget(None)
-
-	#Some buttons for behind the overlay
-	buttons = QtWidgets.QPushButton("Hello")
-	buttons2 = QtWidgets.QPushButton("Hello2")
-	buttons3 = QtWidgets.QPushButton("Hello3")
-
-	buttons.setFixedSize(300, 100)
-	buttons2.setFixedSize(300, 100)
-	buttons3.setFixedSize(300, 100)
-	widget.setLayout(QtWidgets.QVBoxLayout())
-	widget.layout().addWidget(buttons)
-	widget.layout().addWidget(buttons2)
-	widget.layout().addWidget(buttons3)
-
-	#Create overlay and create button to hide it
-	overlay = QtWidgets.QWidget(None)
-	overlay.setFixedSize(300, 100)
-	overlay.setLayout(QtWidgets.QVBoxLayout())
-	overlay.layout().addWidget(QtWidgets.QLabel("This is an overlay widget with a button to hide it"))
-	btn = QtWidgets.QPushButton("Hide overlay")
-	btn.clicked.connect(lambda: widget.set_overlay_hidden(True))
-	overlay.layout().addWidget(btn)
-	widget.set_overlay_widget(overlay)
-	widget.show()
-
-	app.exec()
-	log.info("Done!")
-
-
-if __name__ == "__main__":
-	formatter = logging.Formatter("[{pathname:>90s}:{lineno:<4}]  {levelname:<7s}   {message}", style='{')
-	handler = logging.StreamHandler()
-	handler.setFormatter(formatter)
-	logging.basicConfig(
-		handlers=[handler],
-		level=logging.DEBUG) #Without time
-	log.info("Now running overlay widget example...")
-	run_example_app()
+"""Implements an overlay widget that acts as a container but allows displaying another widget on top of it."""
+
+import logging
+
+from PySide6 import QtCore, QtGui, QtWidgets
+from PySide6.QtCore import Qt
+
+log = logging.getLogger(__name__)
+
+class OverlayWidget(QtWidgets.QWidget):
+	"""
+	Container-like widget which allows the user to overlay another widget on top of it. Switching on/off the overlay
+	widget is done by setting the overlayHidden property.
+	"""
+
+	DESCRIPTION = "Basic QtWidget that allows displaying another widget on top of it using setOverlayWidget."
+
+
+	def __init__(self, parent: QtWidgets.QWidget | None) -> None:
+		super().__init__(parent)
+
+		self._display_overlay = False
+		self._overlay_widget = None
+		self._overlay_widget_container: QtWidgets.QWidget = QtWidgets.QWidget(self)
+		self._overlay_widget_container.setParent(self)
+		self._overlay_widget_container.setWindowFlags(Qt.WindowType.Widget | Qt.WindowType.FramelessWindowHint)
+		self._overlay_widget_container.setAutoFillBackground(True)
+		self._overlay_widget_container.setContentsMargins(0, 0, 0, 0)
+		self._overlay_widget_container.raise_()
+
+		self._cur_background_color = None
+		self.set_overlay_mouse_block(True)
+		self.set_background_color(QtGui.QColor(200, 200, 200, 150))
+
+
+	def set_overlay_mouse_block(self, block: bool) -> None:
+		"""Sets whether the overlay widget should block mouse events from reaching the underlying widget."""
+		self._overlay_widget_container.setAttribute(Qt.WidgetAttribute.WA_TransparentForMouseEvents, not block)
+
+	def get_overlay_mouse_block(self) -> bool:
+		"""Returns whether the overlay widget blocks mouse events from reaching the underlying widget."""
+		return self._overlay_widget_container.testAttribute(Qt.WidgetAttribute.WA_TransparentForMouseEvents)
+
+	def showEvent(self, event: QtGui.QShowEvent) -> None:
+		"""On show, raise the overlay widget to make sure it is on top."""
+		self._overlay_widget_container.raise_() #Make sure the overlay widget is on top
+		return super().showEvent(event)
+
+
+	def set_overlay_widget(self, overlay_widget: QtWidgets.QWidget) -> None:
+		"""
+		Sets the overlay widget to display on top of this widget.
+		"""
+		self._overlay_widget = overlay_widget
+		self._overlay_widget_container.setLayout(QtWidgets.QVBoxLayout()) #Reset the layout to remove any previous
+		self._overlay_widget_container.layout().addWidget(overlay_widget)
+		self._overlay_widget_container.resize(self.size())
+		self._overlay_widget_container.layout().setAlignment(Qt.AlignmentFlag.AlignCenter)
+		self._overlay_widget_container.raise_()
+
+
+	def resizeEvent(self, event: QtGui.QResizeEvent) -> None:
+		"""
+		#On resize, update the overlay widget size
+		"""
+		super().resizeEvent(event)
+		self._overlay_widget_container.resize(self.size())
+
+	def set_overlay_hidden(self, hidden: bool) -> None:
+		"""
+		Sets the overlay widget to be hidden or visible.
+		"""
+		self._overlay_widget_container.setHidden(hidden)
+
+	def get_overlay_hidden(self) -> bool:
+		"""
+		Returns whether the overlay widget is hidden or visible.
+		"""
+		return self._overlay_widget_container.isHidden()
+
+
+	def set_background_color(self, color: QtGui.QColor) -> None:
+		"""
+		Sets the background color of the overlay widget.
+		"""
+		self._cur_background_color = color
+		style = QtWidgets.QApplication.style()
+		palette = style.standardPalette()
+		palette.setColor(QtGui.QPalette.ColorRole.Window, color) #Background color
+		self._overlay_widget_container.setPalette(palette)
+	def get_background_color(self) -> QtGui.QColor | None:
+		"""
+		Returns the background color of the overlay widget.
+		"""
+		return self._cur_background_color
+
+	overlayHidden = QtCore.Property(bool, get_overlay_hidden, set_overlay_hidden)
+	overlayBlocksMouse = QtCore.Property(bool, get_overlay_mouse_block, set_overlay_mouse_block)
+	overlayBackgroundColor = QtCore.Property(QtGui.QColor, get_background_color, set_background_color)
+
+
+
+def run_example_app():
+	"""Creates a qt-app instance and runs the example"""
+	log.info(f"Running example app for {OverlayWidget.__name__}...")
+
+	app = QtWidgets.QApplication([])
+	widget = OverlayWidget(None)
+
+	#Some buttons for behind the overlay
+	buttons = QtWidgets.QPushButton("Hello")
+	buttons2 = QtWidgets.QPushButton("Hello2")
+	buttons3 = QtWidgets.QPushButton("Hello3")
+
+	buttons.setFixedSize(300, 100)
+	buttons2.setFixedSize(300, 100)
+	buttons3.setFixedSize(300, 100)
+	widget.setLayout(QtWidgets.QVBoxLayout())
+	widget.layout().addWidget(buttons)
+	widget.layout().addWidget(buttons2)
+	widget.layout().addWidget(buttons3)
+
+	#Create overlay and create button to hide it
+	overlay = QtWidgets.QWidget(None)
+	overlay.setFixedSize(300, 100)
+	overlay.setLayout(QtWidgets.QVBoxLayout())
+	overlay.layout().addWidget(QtWidgets.QLabel("This is an overlay widget with a button to hide it"))
+	btn = QtWidgets.QPushButton("Hide overlay")
+	btn.clicked.connect(lambda: widget.set_overlay_hidden(True))
+	overlay.layout().addWidget(btn)
+	widget.set_overlay_widget(overlay)
+	widget.show()
+
+	app.exec()
+	log.info("Done!")
+
+
+if __name__ == "__main__":
+	formatter = logging.Formatter("[{pathname:>90s}:{lineno:<4}]  {levelname:<7s}   {message}", style='{')
+	handler = logging.StreamHandler()
+	handler.setFormatter(formatter)
+	logging.basicConfig(
+		handlers=[handler],
+		level=logging.DEBUG) #Without time
+	log.info("Now running overlay widget example...")
+	run_example_app()
```

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/pandas_table_view.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/pandas_table_view.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/range_selector.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/range_selector.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils/widgets/square_frame.py` & `pyside6_utils-1.2.0/pyside6_utils/widgets/square_frame.py`

 * *Files identical despite different names*

### Comparing `pyside6_utils-1.1.0/pyside6_utils.egg-info/PKG-INFO` & `pyside6_utils-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,207 +1,283 @@
 Metadata-Version: 2.1
-Name: pyside6-utils
-Version: 1.1.0
+Name: pyside6_utils
+Version: 1.2.0
 Summary: A collection of useful widgets and utilities for PySide6 compatible with pyside6-designer.
 Home-page: https://github.com/Woutah/pyside6-utils
 Author: Wouter Stokman
 License: LPGPLv2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySide6 - Utils
+
 `pyside6-utils` implements several useful PySide6 widgets, models and delegates as well as some utility functions.
-The package contains registrars for these widgets, which can be [used to register the widgets in QtDesigner](#Qt-Designer) to quickly build UI's.
+The package contains registrars for these widgets, which can be [used to register the widgets in QtDesigner](#qt-designer) to quickly build UI's.
+
+This package was mainly developed around the python Dataclass-functionality. It was created in tandem with the following package: [Configurun - A tool to create and manage machine learning training/testing-configurations and run them automatically and/or remotely.](https://github.com/Woutah/configurun).
 
-This package was mainly developed around the python Dataclass-functionality. It was created in tandem with the following package: [Configurun - A tool to create and manage machine learning training/testing-configurations and run them automatically and/or remotely.](https://github.com/Woutah/configurun). 
+# Table of contents
 
+- [PySide6 - Utils](#pyside6---utils)
+- [Table of contents](#table-of-contents)
+- [Features](#features)
+	- [Installation](#installation)
+	- [Qt-Designer](#qt-designer)
+- [Widgets](#widgets)
+	- [`DataclassTreeview`](#dataclasstreeview)
+	- [`PandasTableView` (and `PandasTableModel`)](#pandastableview-and-pandastablemodel)
+	- [`ExtendedMdiArea` / `FramelessMdiWindow`](#extendedmdiarea--framelessmdiwindow)
+	- [`CollapsibleGroupBox`](#collapsiblegroupbox)
+	- [`Console Widget`](#console-widget)
+	- [`FileExplorerView`](#fileexplorerview)
+	- [`OverlayWidget`](#overlaywidget)
+	- [`RangeSelector`](#rangeselector)
+	- [`SquareFrame`](#squareframe)
+	- [`WidgetList`](#widgetlist)
+	- [`WidgetSwitcher`](#widgetswitcher)
+- [Utility](#utility)
+- [Classes](#classes)
+- [Models](#models)
+- [Acknowledgements](#acknowledgements)
+
+# Features
 
 A quick list of the main widgets:
-- [`DataclassTreeview` (and `DataClassModel` & `DataClassEditorDelegate`)](#DataclassTreeview)
+
+- [`DataclassTreeview` (and `DataClassModel` & `DataClassEditorDelegate`)](#dataclasstreeview)
   - A view/model/delegate combination which mirrors a python dataclass (`@dataclass`) object and provides editors for each of the types defined. Edits are propagated to the dataclass object. We can use [`dataclasses.field()`](https://docs.python.org/3/library/dataclasses.html#dataclasses.Field) to customize how attributes are displayed and to change the editor-type and constraints.
-- [`PandasTableView` (and `PandasTableModel`)](#PandasTableView)
+- [`PandasTableView` (and `PandasTableModel`)](#pandastableview-and-pandastablemodel)
   - Provide an easy way to show and edit pandas dataframes
-- [`CollapsibleGroupBox`](#CollapsibleGroupBox)
+- [`CollapsibleGroupBox`](#collapsiblegroupbox)
   - A groupbox that acts as a layout, when the user check/unchecks the groupbox, the contents collapse
-- [`ConsoleWidget`](#ConsoleWidget)
+- [`ConsoleWidget`](#console-widget)
   - A console-like widget to which multiple files can be mirorred, user can select the items to view the consoleitem-contens
-- [`ExtendedMdiArea` / `FramelessMdiWindow`](#ExtendedMdiArea)
-  - Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. A custom UI example is provided in `./ui/FrameslessMdiWindow.ui` 
-- [`FileExplorerView`](#FileExplorerView)
+- [`ExtendedMdiArea` / `FramelessMdiWindow`](#extendedmdiarea--framelessmdiwindow)
+  - Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. A custom UI example is provided in `./ui/FrameslessMdiWindow.ui`
+- [`FileExplorerView`](#fileexplorerview)
   - Built around the use of a QFileSystemModel - enables right-click operations and undo/redo actions, as well as the possibility to set a "highlighted" file
-- [`OverlayWidget`](#OverlayWidget)
+- [`OverlayWidget`](#overlaywidget)
   - Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s)
-- [`SquareFrame`](#SquareFrame)
+- [`SquareFrame`](#squareframe)
   - A small widget wrapper that enforces squareness. Useful when designing UI's in QtDesigner.
-- [`RangeSelector`](#RangeSelector)
+- [`RangeSelector`](#rangeselector)
   - Widget to select a range of float/int/datetime, provides extra styling if ticks are provided.
-
+- [`WidgetList`](#widgetlist)
+  - Widget to which we can pass a widget-factory or widget-type. The user can then add/remove widgets of this type to the list.
+- [`WidgetSwitcher`](#widgetswitcher)
+  - Wrapper around [`QtWidgets.QStackedWidget`](https://doc.qt.io/qt-6/qstackedwidget.html), provides a way to switch between multiple widgets.
 
 ## Installation
+
 The easiest way to install this package is using pip install:
-```
+
+``` bash
 pip install pyside6-utils
 ```
 
 The package can also be manually installed by downloading this repository, extracting it to the desired install location and running:
-```
+
+``` bash
 pip install <install_path>
 ```
 
 ## Qt-Designer
+
 This package provides registrars for the implemented widgets, which means that the widgets can be made available directly in qt-designer (note that `pyside6-designer` should be used).
 To enable this, the environment variable `PYSIDE_DESIGNER_PLUGINS` should be set to the `../pyside6_utils/registrars`-folder.
 
 Alternatively, we can automatically set environment variables by using the provided pyside6 launch script. We can use this script by running `pyside6_utils/examples/run_qt_designer.py` or by importing and running the `run_qt_designer()`-function using:
-```python
+
+``` python
 from pyside6_utilities.examples import run_qt_designer
 run_qt_designer()
 ```
 
 If all is well, this should result in the widgets showing up in the left-hand side of Qt-designer, e.g. for the views it should look like this:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/Qt_designer_loaded_widgets_example.png?raw=True" width="800" />
 </p>
 
 # Widgets
+
 **NOTE: every widget-module contains a `run_example_app()` function, which starts a qt app and an example-instance of the widget in question, the following example-widget-images are pictures of these examples. Example:**
+
 ```python
 from pyside6_utils.widgets.data_class_tree_view import run_example_app
 DataclassTreeview.run_example_app()
 ```
 
-
 ## `DataclassTreeview`
+
 `DataclassTreeview`, `DataClassModel` and `DataClassEditorDelegate` are a view/model/delegate combination (resp.) which mirror a python dataclass (`@dataclass`) object and provides editors for each of the types defined.
 
 The model is mainly built around the `field()` functionality of dataclasses, which allows the model to make use of the default values, type hints and other information provided by the dataclass.
 For each field, we can provide additional information in the `metadata` attribute of `field()`, this information is used by the model to determine the editor/limits to use for the field.
 The following metadata is supported:
 
 | Metadata Key | Type | Description |
 | --- | --- | --- |
 | `"display_name"` | `str` | Name to display for this attribute in the view - defaults to the variable name itself |
 | `"display_path"` | `str` | Path to display this attribute - we can group/structure items when using a treeview - defaults to no parents|
 | `"help"` | `str` | Help-message which will be shown when the user hovers over this item - empty by default|
-| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [^constraintnote] , if none provided, use typehint of the field|
+| `"constraints"` | `List[sklearn_param_validation constraints]` | Additional constraints on which the editor will be determined to apply to the field [*](#constraintnote) , if none provided, use typehint of the field|
 | `"required"` | `bool` | Whether this field is required to be filled in - if true - a red background will appear if the value is not set|
 | `"editable"` | `bool` | Whether this field is editable - if false - the editor will be disabled|
 
-[^constraintnote] Constraints are (almost fully) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `utility.constraints`. The following constraints are supported:
+<a name="constraintnote">*</a>Constraints are (almost fully) sourced from the `sklearn.utils._validation` module and provides a way to constrain the dataclass fields such that the user can only enter valid values. They are also packed into this package under `classes.constraints`. The following constraints are supported:
 | Constraint | Description | Editor Type
 | --- | --- | --- |
 | `type` | The type of the value should match the type of the constraint | based on type |
 | `Options` / `Container` | The value should be one of the options provided in the constraint | `QComboBox` |
 | `StrOptions` | The value should be one of the str-options provided in the constraint | `QComboBox` |
 | `Interval` | The value should be within the interval provided in the constraint | `QSpinBox` or `QDoubleSpinBox` (limited) |
 | `None` | `None` is a valid value for this field `typing.Optional` | Adds reset-button to editor |
 | `Range` | The value should be within the range provided in the constraint | `QSpinBox` (limited) |
-| `TODO` | Maybe more? |
+| `ConstrainedList` | [*(Custom - not part of Sklearn)](#constrainedlist) Indicates a list of of values of a constrained type | Based on type of list |
+
+<a name="constrainedlist">*=</a>For example, `ConstrainedList([Interval(float, 0.0, 1.0), StrOptions(["string1", "string2"])])` indicates a list of values that should either be a float between 0.0 and 1.0, or the string "string1" or "string2". The editor for this field would be constructed as a [`WidgetList`](#widgetlist) with a [`WidgetSwitcher`](#widgetswitcher) as the factory-widget. The `WidgetSwitcher` would then have two widgets, one with a `QSpinBox` and one with a `QComboBox` as the editor. **NOTE:** the same editor would be the result of a `Typing.List[typing.Union[float, str]]` typehint, minus the bounded-interval constraint on the float:
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/string_float_list_example.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/string_float_list_example.png" width=300/> -->
+</p>
 
 Default values are saved and can be reset using right-click context menu. Values that have changed from default will appear in bold.
 
 An example of a dataclass-view is shown below:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/dataclass_view.png?raw=True" width="800" />
 </p>
 
-The dataclass from which this example was generated can be found under `./examples/example_dataclass.py`.  
+The dataclass from which this example was generated can be found under `./examples/example_dataclass.py`.
 
 ## `PandasTableView` (and `PandasTableModel`)
+
 Provide an easy way to show and edit pandas dataframes. Pandas-table model adds the possibility to copy/paste data from excel, as well as current selection information (e.g. selected cells, average, total and sum).
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/pandas_table_view.png?raw=True" width="800" />
 </p>
 
-
-
 ## `ExtendedMdiArea` / `FramelessMdiWindow`
+
 Based on PySide6.QtWidgets.QMdiArea, provides a way to load frameless windows with a custom UI, while also retaining resize/move/etc. The ui used by default is provided in `./ui/FrameslessMdiWindow.ui`.
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/extended_mdi_area.png?raw=True" width="800" />
 </p>
 
 We can drag, resize and move the windows as we would expect from a normal window. The windows can also be maximized and minimized using the buttons in the top-right corner. A custom UI can be provided, all functionality will be retained if the ui contains the following widgets:
 
 - `contentLayout` (`QtWidgets.QLayout`): The layout that will be used to add the content-widget
 - `titleBar` (`QtWidgets.QWidget`): The widget that will be used as the title bar, we can drag the window by using this, the parent-mdi area context menu will also be made available when right-clicking this widget
 	- `titleLabel` (`QtWidgets.QLabel`): The label that will be used to display the title
 	- `zoomButton` (`QtWidget.QButtton`): If pressed, set window to fullscreen
 	- `minimizeButton` (`QtWidget.QButtton`): If pressed, minimize the window
 
-
-
 ## `CollapsibleGroupBox`
+
 A QtWidgets.QGroupbox that acts as a layout, when the user check/unchecks the groupbox, the contents collapse
 When opened:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/collapsible_group_box_open.png?raw=True" width="800" />
 </p>
 When collapsed:
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/collapsible_group_box_collapsed.png?raw=True" width="800" />
 </p>
 
 ## `Console Widget`
+
 We can import `console_from_file_item` from `pyside6_utils.models.console_widget_models` to create console items which mirror a text-output file. We can then add these items to the console-widget using `ConsoleWidget.add_item`.
 
-The user can then scroll between the various console-outputs, which are updated every time the target file changes. This is especially useful for managing multiple output-files. 
+The user can then scroll between the various console-outputs, which are updated every time the target file changes. This is especially useful for managing multiple output-files.
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/console_widget.png?raw=True" width="900" />
 </p>
 
 ## `FileExplorerView`
+
 Built around the use of a QFileSystemModel - enables right-click operations and undo/redo actions, as well as the possibility to set a "highlighted" file
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/file_explorer_view.png?raw=True" width="500" />
 </p>
 
 ## `OverlayWidget`
-Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s). 
+
+Provides a container-widget to which another widget can be provided, when turning the overlay-mode of this widget on, this widget will be overlayed over the contained widget(s).
 
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/overlay_widget.png?raw=True" width="400" />
 </p>
 
-## `RangeSelector` 
+## `RangeSelector`
+
 Widget to select a range of float/int/datetime etc. Can drag in the middle to change both, or drag on the edges to change only min/max.
 Provides extra styling when ticks are enabled.
 <p align="center">
 	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/range_selector.png?raw=True" width="400" />
 </p>
 
+## `SquareFrame`
+
+Enforces squareness of the widget inside. Useful when designing UI's in QtDesigner.
+<p align="center">
+	<!-- <img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/square_widget.png?raw=True" width="400" /> -->
+	<img src="./pyside6_utils/examples/images/square_widget.png" width=400/>
+</p>
+
+## `WidgetList`
+
+Widget to which we can pass a widget-factory or widget-type. The user can then add/remove widgets of this type to the list.
+A value-getter can be specified to easily get the values of all widgets in the list.
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/widget_list.png?raw=True" width="300" />
+	<!-- <img src="./pyside6_utils/examples/images/widget_list.png" width=300/> -->
+</p>
+
+## `WidgetSwitcher`
+
+Wrapper around [`QtWidgets.QStackedWidget`](https://doc.qt.io/qt-6/qstackedwidget.html), provides a way to switch between multiple widgets. A context menu can be accessed via right click or via the small triangle in the right-bottom corner, which allows the user to switch between the widgets.
+
+Especially useful in combination with [`WidgetList`](#widgetlist). Provides the same value-getter functionality as `WidgetList`.
+<p align="center">
+	<img src="https://github.com/Woutah/pyside6-utils/blob/main/pyside6_utils/examples/images/widget_switcher.png?raw=True" width="500" />
+	<!-- <img src="./pyside6_utils/examples/images/widget_switcher.png" width=500/> -->
+</p>
 
 # Utility
-The utility submodule provides the following:
+
+The utility submodule provides the following UI-based utility items:
+
 - `catch_show_exception_in_popup_decorator`
   - A decorator that catches exceptions and shows them in a popup
-- `constraints`
-  - Sklearn constraints, used for `DataClassModel` to constrain the editor-type based on the type-hint of the field
-- `Serializable`
-  - Base-class mainly targeted towards dataclasses - enable serialization to json. 
-- `SignalBlocker` 
-  - Enables us to temporarily block PySide6 signals using a `with` statement 
+- `SignalBlocker`
+  - Enables us to temporarily block PySide6 signals using a `with` statement
 - `utility_functions`
   - Several smaller utility functions used in this package
 
+# Classes
+The classes submodule provides several useful classes that do not depend on PySide6:
+
+- `constraints`
+  - Sklearn constraints, used for `DataClassModel` to constrain the editor-type based on the type-hint of the field
+- `Serializable`
+  - Mainly useful for `@dataclass`-like classes to parse from/to json
 
 # Models
+
 The models submodule provides an implementation of the following:
-- `ConsoleFromFileItem` / `ConsoleModel` 
+
+- `ConsoleFromFileItem` / `ConsoleModel`
   - Also see `ConsoleFromFileWidget` - A model/item combination that mirrors a text-file, used in `ConsoleWidget`. Use the `addItem()` method of `ConsoleModel` to add a new file to the model.
 - `DataclassModel`
   - Also see `DataclassTreeview` - A model that mirrors a python dataclass (`@dataclass`) object and provides editors for each of the types defined. Edits are propagated to the dataclass object.
 - `ExtendedSortFilterProxyModel`
   - Implements more advanced sorting (using multiple columns) and a `set_filter_function(...)` that can be used to use (multiple) custom methods to filter the model.
 - `FileExplorerModel`
-  - Also see `FileExplorerView` - Enabled highlighting items 
+  - Also see `FileExplorerView` - Enabled highlighting items
 - `PandasTableModel`
   - Also see `PandasTableView` - Mirrors pandas dataframe to a Qt tablemodel
 
-
-
 # Acknowledgements
-This package uses icons from (and based off) the Tango Desktop Project:
-http://tango.freedesktop.org/Tango_Desktop_Project
 
+This package uses icons from (and based off) the [Tango Desktop Project](http://tango.freedesktop.org/Tango_Desktop_Project).
```

### Comparing `pyside6_utils-1.1.0/pyside6_utils.egg-info/SOURCES.txt` & `pyside6_utils-1.2.0/pyside6_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 pyside6_utils/__init__.py
 pyside6_utils/constants.py
 pyside6_utils.egg-info/PKG-INFO
 pyside6_utils.egg-info/SOURCES.txt
 pyside6_utils.egg-info/dependency_links.txt
 pyside6_utils.egg-info/requires.txt
 pyside6_utils.egg-info/top_level.txt
+pyside6_utils/classes/__init__.py
+pyside6_utils/classes/constraints.py
+pyside6_utils/classes/serializable.py
 pyside6_utils/examples/__init__.py
 pyside6_utils/examples/example_dataclass.py
 pyside6_utils/examples/run_qt_designer.py
 pyside6_utils/examples/run_widgets_example_app.py
 pyside6_utils/icons/__init__.py
 pyside6_utils/icons/app_resources_rc.py
 pyside6_utils/models/__init__.py
@@ -29,31 +32,33 @@
 pyside6_utils/registrars/register_console_widget.py
 pyside6_utils/registrars/register_extended_mdi_area.py
 pyside6_utils/registrars/register_file_explorer_view.py
 pyside6_utils/registrars/register_overlay_widget.py
 pyside6_utils/registrars/register_pandas_table.py
 pyside6_utils/registrars/register_range_selector.py
 pyside6_utils/registrars/register_square_frame.py
+pyside6_utils/registrars/register_widget_list.py
+pyside6_utils/registrars/register_widget_switcher.py
 pyside6_utils/ui/ConsoleWidget_ui.py
 pyside6_utils/ui/FramelessMdiWindow_ui.py
 pyside6_utils/ui/__init__.py
 pyside6_utils/ui/allWidgets_ui.py
 pyside6_utils/utility/__init__.py
 pyside6_utils/utility/catch_show_exception_in_popup_decorator.py
-pyside6_utils/utility/constraints.py
-pyside6_utils/utility/serializable.py
 pyside6_utils/utility/signal_blocker.py
 pyside6_utils/utility/utility_functions.py
 pyside6_utils/widgets/__init__.py
 pyside6_utils/widgets/collapsible_group_box.py
 pyside6_utils/widgets/console_widget.py
 pyside6_utils/widgets/dataclass_tree_view.py
 pyside6_utils/widgets/extended_mdi_area.py
 pyside6_utils/widgets/file_explorer_view.py
 pyside6_utils/widgets/frameless_mdi_window.py
 pyside6_utils/widgets/overlay_widget.py
 pyside6_utils/widgets/pandas_table_view.py
 pyside6_utils/widgets/range_selector.py
 pyside6_utils/widgets/square_frame.py
+pyside6_utils/widgets/widget_list.py
+pyside6_utils/widgets/widget_switcher.py
 pyside6_utils/widgets/delegates/__init__.py
 pyside6_utils/widgets/delegates/console_widget_delegate.py
 pyside6_utils/widgets/delegates/dataclass_editors_delegate.py
```

### Comparing `pyside6_utils-1.1.0/setup.py` & `pyside6_utils-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = "pyside6_utils",
-	version= "1.1.0",
+	version= "1.2.0",
 	packages=find_packages('.'),
     description="A collection of useful widgets and utilities for PySide6 compatible with pyside6-designer.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown", #Long description is in markdown
     author="Wouter Stokman",
     url="https://github.com/Woutah/pyside6-utils",
     license="LPGPLv2",
```

