# Comparing `tmp/aa-taskmonitor-0.9.0.tar.gz` & `tmp/aa-taskmonitor-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-taskmonitor-0.9.0.tar", last modified: Tue Jan 31 21:51:35 2023, max compression
+gzip compressed data, was "aa-taskmonitor-0.9.1.tar", last modified: Wed Feb  1 18:57:55 2023, max compression
```

## Comparing `aa-taskmonitor-0.9.0.tar` & `aa-taskmonitor-0.9.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.148627 aa-taskmonitor-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7324 2023-01-31 21:51:35.148627 aa-taskmonitor-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6457 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.136627 aa-taskmonitor-0.9.0/aa_taskmonitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7324 2023-01-31 21:51:34.000000 aa-taskmonitor-0.9.0/aa_taskmonitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2326 2023-01-31 21:51:35.000000 aa-taskmonitor-0.9.0/aa_taskmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 21:51:34.000000 aa-taskmonitor-0.9.0/aa_taskmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-01-31 21:51:35.000000 aa-taskmonitor-0.9.0/aa_taskmonitor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-31 21:51:35.000000 aa-taskmonitor-0.9.0/aa_taskmonitor.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-01-31 21:51:35.152627 aa-taskmonitor-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.140627 aa-taskmonitor-0.9.0/taskmonitor/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5786 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.140627 aa-taskmonitor-0.9.0/taskmonitor/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9941 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/core/cached_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3629 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/core/celery_queues.py
--rw-rw-rw-   0 root         (0) root         (0)     4158 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/core/task_logs.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/core/task_records.py
--rw-rw-rw-   0 root         (0) root         (0)     2453 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     6536 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.140627 aa-taskmonitor-0.9.0/taskmonitor/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1719 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/migrations/0002_taskreport.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/migrations/0003_queuedtask.py
--rw-rw-rw-   0 root         (0) root         (0)     4380 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/migrations/0004_store_task_params_and_results.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5687 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.132627 aa-taskmonitor-0.9.0/taskmonitor/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.132627 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.140627 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/css/
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/css/admin.css
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/css/reports.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.140627 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/js/
--rw-rw-rw-   0 root         (0) root         (0)     4894 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/js/highcharts_defaults.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.132627 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.144627 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/vendor/highcharts/
--rw-rw-rw-   0 root         (0) root         (0)   302871 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/vendor/highcharts/highcharts.js
--rw-rw-rw-   0 root         (0) root         (0)   704148 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/vendor/highcharts/highcharts.js.map
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.132627 aa-taskmonitor-0.9.0/taskmonitor/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.132627 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.132627 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.144627 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/queuedtask/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/queuedtask/change_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.148627 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/
--rw-rw-rw-   0 root         (0) root         (0)      943 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/change_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/chart_throughput_partial.html
--rw-rw-rw-   0 root         (0) root         (0)     1498 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/report_barchart_partial.html
--rw-rw-rw-   0 root         (0) root         (0)     1828 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/report_piechart_partial.html
--rw-rw-rw-   0 root         (0) root         (0)      982 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/report_table_partial.html
--rw-rw-rw-   0 root         (0) root         (0)     7342 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/reports.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.148627 aa-taskmonitor-0.9.0/taskmonitor/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/templatetags/taskmonitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.148627 aa-taskmonitor-0.9.0/taskmonitor/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 21:51:35.148627 aa-taskmonitor-0.9.0/taskmonitor/tests/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/core/test_cached_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/core/test_celery_queues.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/core/test_task_records.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/generate_queued_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/generate_task_logs.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     4937 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5296 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    15155 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.0/taskmonitor/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.950993 aa-taskmonitor-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7418 2023-02-01 18:57:55.950993 aa-taskmonitor-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6551 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.934993 aa-taskmonitor-0.9.1/aa_taskmonitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7418 2023-02-01 18:57:55.000000 aa-taskmonitor-0.9.1/aa_taskmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-02-01 18:57:55.000000 aa-taskmonitor-0.9.1/aa_taskmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 18:57:55.000000 aa-taskmonitor-0.9.1/aa_taskmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-02-01 18:57:55.000000 aa-taskmonitor-0.9.1/aa_taskmonitor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-01 18:57:55.000000 aa-taskmonitor-0.9.1/aa_taskmonitor.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-02-01 18:57:55.950993 aa-taskmonitor-0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.938993 aa-taskmonitor-0.9.1/taskmonitor/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6051 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/auth_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.938993 aa-taskmonitor-0.9.1/taskmonitor/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9941 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/core/cached_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     5590 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/core/celery_queues.py
+-rw-rw-rw-   0 root         (0) root         (0)     4158 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/core/task_logs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/core/task_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     2453 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6497 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.942993 aa-taskmonitor-0.9.1/taskmonitor/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/migrations/0002_taskreport.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/migrations/0003_queuedtask.py
+-rw-rw-rw-   0 root         (0) root         (0)     4380 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/migrations/0004_store_task_params_and_results.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5687 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.930993 aa-taskmonitor-0.9.1/taskmonitor/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.930993 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.942993 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/css/
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/css/admin.css
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/css/reports.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.942993 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/js/
+-rw-rw-rw-   0 root         (0) root         (0)     4894 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/js/highcharts_defaults.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.930993 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.942993 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/vendor/highcharts/
+-rw-rw-rw-   0 root         (0) root         (0)   302871 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/vendor/highcharts/highcharts.js
+-rw-rw-rw-   0 root         (0) root         (0)   704148 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/vendor/highcharts/highcharts.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.930993 aa-taskmonitor-0.9.1/taskmonitor/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.930993 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.930993 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.946993 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/queuedtask/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/queuedtask/change_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.946993 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/
+-rw-rw-rw-   0 root         (0) root         (0)      943 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/change_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/chart_throughput_partial.html
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/report_barchart_partial.html
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/report_piechart_partial.html
+-rw-rw-rw-   0 root         (0) root         (0)      982 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/report_table_partial.html
+-rw-rw-rw-   0 root         (0) root         (0)     7342 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/reports.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.946993 aa-taskmonitor-0.9.1/taskmonitor/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/templatetags/taskmonitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.950993 aa-taskmonitor-0.9.1/taskmonitor/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 18:57:55.950993 aa-taskmonitor-0.9.1/taskmonitor/tests/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/core/test_cached_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/core/test_celery_queues.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/core/test_task_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/generate_queued_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/generate_task_logs.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4937 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/test_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5296 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)    15155 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-01-31 21:41:57.000000 aa-taskmonitor-0.9.1/taskmonitor/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     3627 2023-02-01 18:41:00.000000 aa-taskmonitor-0.9.1/taskmonitor/views.py
```

### Comparing `aa-taskmonitor-0.9.0/LICENSE` & `aa-taskmonitor-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/PKG-INFO` & `aa-taskmonitor-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-taskmonitor
-Version: 0.9.0
+Version: 0.9.1
 Summary: Alliance Auth plugin for monitoring celery tasks
 Home-page: https://gitlab.com/ErikKalkoken/aa-taskmonitor
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -114,14 +114,15 @@
 
 Note that all settings are optional and the app will use the documented default settings if they are not used.
 
 Name | Description | Default
 -- | -- | --
 `TASKMONITOR_DATA_MAX_AGE`| Max age of logged tasks in hours. Older logs be deleted automatically. | `24`
 `TASKMONITOR_HOUSEKEEPING_FREQUENCY`| Frequency of house keeping runs in minutes. | `15`
+`TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT`| Timeout for caching queued tasks in seconds. | `60`
 `TASKMONITOR_REPORTS_MAX_AGE`| Max age of cached reports in minutes. | `15`
 `TASKMONITOR_REPORTS_MAX_TOP`| Max items to show in the top reports. e.g. 10 will shop the top ten items. | `15`
 `TASKMONITOR_TRUNCATE_NESTED_DATA`| Whether deeply nested task params and results are truncated. Please see FAQ for details. | `True`
 
 ## FAQ
 
 ### Is it possible to store task logs longer then for just 24 hours?
```

### Comparing `aa-taskmonitor-0.9.0/README.md` & `aa-taskmonitor-0.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
 Note that all settings are optional and the app will use the documented default settings if they are not used.
 
 Name | Description | Default
 -- | -- | --
 `TASKMONITOR_DATA_MAX_AGE`| Max age of logged tasks in hours. Older logs be deleted automatically. | `24`
 `TASKMONITOR_HOUSEKEEPING_FREQUENCY`| Frequency of house keeping runs in minutes. | `15`
+`TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT`| Timeout for caching queued tasks in seconds. | `60`
 `TASKMONITOR_REPORTS_MAX_AGE`| Max age of cached reports in minutes. | `15`
 `TASKMONITOR_REPORTS_MAX_TOP`| Max items to show in the top reports. e.g. 10 will shop the top ten items. | `15`
 `TASKMONITOR_TRUNCATE_NESTED_DATA`| Whether deeply nested task params and results are truncated. Please see FAQ for details. | `True`
 
 ## FAQ
 
 ### Is it possible to store task logs longer then for just 24 hours?
```

### Comparing `aa-taskmonitor-0.9.0/aa_taskmonitor.egg-info/PKG-INFO` & `aa-taskmonitor-0.9.1/aa_taskmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-taskmonitor
-Version: 0.9.0
+Version: 0.9.1
 Summary: Alliance Auth plugin for monitoring celery tasks
 Home-page: https://gitlab.com/ErikKalkoken/aa-taskmonitor
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -114,14 +114,15 @@
 
 Note that all settings are optional and the app will use the documented default settings if they are not used.
 
 Name | Description | Default
 -- | -- | --
 `TASKMONITOR_DATA_MAX_AGE`| Max age of logged tasks in hours. Older logs be deleted automatically. | `24`
 `TASKMONITOR_HOUSEKEEPING_FREQUENCY`| Frequency of house keeping runs in minutes. | `15`
+`TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT`| Timeout for caching queued tasks in seconds. | `60`
 `TASKMONITOR_REPORTS_MAX_AGE`| Max age of cached reports in minutes. | `15`
 `TASKMONITOR_REPORTS_MAX_TOP`| Max items to show in the top reports. e.g. 10 will shop the top ten items. | `15`
 `TASKMONITOR_TRUNCATE_NESTED_DATA`| Whether deeply nested task params and results are truncated. Please see FAQ for details. | `True`
 
 ## FAQ
 
 ### Is it possible to store task logs longer then for just 24 hours?
```

### Comparing `aa-taskmonitor-0.9.0/aa_taskmonitor.egg-info/SOURCES.txt` & `aa-taskmonitor-0.9.1/aa_taskmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/setup.py` & `aa-taskmonitor-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/admin.py` & `aa-taskmonitor-0.9.1/taskmonitor/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 from typing import Optional
 
 from django.contrib import admin
 from django.shortcuts import get_object_or_404, redirect
 from django.utils import html, safestring, timezone
 
+from .app_settings import TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT
+from .core import celery_queues
 from .models import QueuedTask, TaskLog, TaskReport
 
 
 @admin.register(QueuedTask)
 class QueuedTaskAdmin(admin.ModelAdmin):
 
     list_display = (
@@ -29,18 +31,20 @@
         return False
 
     def has_delete_permission(self, *args, **kwargs):
         return False
 
     def changelist_view(self, request, extra_context=None):
         extra_context = extra_context or {}
+        cache_created_at = celery_queues.local_cache.created_at() or timezone.now()
         context = {
             "title": "Currently queued tasks",
-            "now": timezone.now(),
+            "cache_created_at": cache_created_at,
             "task_count": QueuedTask.objects.count(),
+            "cache_timeout": TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT,
         }
         extra_context.update(context)
         return super().changelist_view(request, extra_context)
 
 
 @admin.register(TaskReport)
 class TaskReportAdmin(admin.ModelAdmin):
```

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/app_settings.py` & `aa-taskmonitor-0.9.1/taskmonitor/app_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,7 +14,12 @@
 TASKMONITOR_REPORTS_MAX_TOP = clean_setting("TASKMONITOR_REPORTS_MAX_TOP", 20)
 """Max items to show in the top reports. e.g. 10 will shop the top ten items."""
 
 TASKMONITOR_TRUNCATE_NESTED_DATA = clean_setting(
     "TASKMONITOR_TRUNCATE_NESTED_DATA", True
 )
 """Whether deeply nested task params and results are truncated."""
+
+TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT = clean_setting(
+    "TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT", 60
+)
+"""Timeout for caching queued tasks in seconds."""
```

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/core/cached_reports.py` & `aa-taskmonitor-0.9.1/taskmonitor/core/cached_reports.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/core/celery_queues.py` & `aa-taskmonitor-0.9.1/taskmonitor/core/celery_queues.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 """API for working with celery task queue."""
 
 import concurrent.futures
+import datetime as dt
 import functools
 import itertools
 import json
 from collections import defaultdict
-from typing import List, NamedTuple
+from typing import List, NamedTuple, Optional
 
 import redis
 
 from django.conf import settings
+from django.core.cache import cache
+from django.utils import timezone
 
-from taskmonitor.helpers import extract_app_name
-
-# from pympler import asizeof
+from allianceauth.services.hooks import get_extension_logger
+from app_utils.logging import LoggerAddTag
 
+from taskmonitor import __title__
+from taskmonitor.app_settings import TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT
+from taskmonitor.helpers import extract_app_name
 
 PRIORITY_SEP = "\x06\x16"
 DEFAULT_PRIORITY_STEPS = range(10)
+QUEUED_TASKS_CACHE_KEY = "queued-tasks-cache-key"
+
+logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class QueuedTaskShort(NamedTuple):
     """DTO for queued tasks, optimized for size."""
 
     app_name: str
     id: int
@@ -40,14 +48,50 @@
             app_name=extract_app_name(task_name),
             id=headers["id"],
             name=task_name,
             priority=properties.get("priority"),
         )
 
 
+class QueuedTaskCacheEntry(NamedTuple):
+    """Wrapper for storing queued tasks in cache with additional data."""
+
+    tasks: List[QueuedTaskShort]
+    created_at: dt.datetime
+
+
+class CacheApi:
+    """API for working with the cache for queued tasks."""
+
+    def get(self) -> Optional[QueuedTaskCacheEntry]:
+        """Retrieve content of cache or None if cache is expired or invalid."""
+        return cache.get(QUEUED_TASKS_CACHE_KEY)
+
+    def set(self, tasks: List[QueuedTaskShort]) -> QueuedTaskCacheEntry:
+        """Store given tasks in cache."""
+        data = QueuedTaskCacheEntry(tasks=tasks, created_at=timezone.now())
+        cache.set(
+            QUEUED_TASKS_CACHE_KEY,
+            data,
+            timeout=TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT,
+        )
+        return data
+
+    def clear(self):
+        """Clear the cache."""
+        cache.delete(QUEUED_TASKS_CACHE_KEY)
+
+    def created_at(self) -> Optional[dt.datetime]:
+        """Return date when cache was created or None when cache is invalid."""
+        data = self.get()
+        if data is None:
+            return None
+        return data.created_at
+
+
 def _redis_client():
     """Fetch the Redis client for the celery broker."""
     return redis.from_url(settings.BROKER_URL)
 
 
 def default_queue_name() -> str:
     """Default name of celery queue in AA."""
@@ -67,47 +111,60 @@
 
 def queue_length() -> int:
     """Length of the celery queue."""
     r = _redis_client()
     return sum(r.llen(name) for name in _redis_queue_names())
 
 
-def _fetch_tasks_from_queue(
+def fetch_tasks() -> List[QueuedTaskShort]:
+    """Fetch tasks from queues
+    and return as ordered list with oldest task in first position.
+    """
+    data = local_cache.get()
+    if data is None:
+        logger.debug("Cache is stale. Fetching new tasks from queue.")
+        tasks = _fetch_task_from_all_queues()
+        local_cache.set(tasks)
+    else:
+        tasks = data.tasks
+        logger.debug("Returning tasks from cache.")
+    return tasks
+
+
+def _fetch_task_from_all_queues() -> List[QueuedTaskShort]:
+    """Coordinate fetching tasks from all priority queues."""
+    _fetch_func = functools.partial(_fetch_tasks_from_redis, _redis_client())
+    redis_queue_names = _redis_queue_names()
+    with concurrent.futures.ThreadPoolExecutor(
+        max_workers=len(redis_queue_names)
+    ) as executor:
+        tasks_raw = executor.map(_fetch_func, redis_queue_names)
+    return list(itertools.chain(*tasks_raw))
+
+
+def _fetch_tasks_from_redis(
     r: redis.Redis, redis_queue_name: str
 ) -> List[QueuedTaskShort]:
-    """Fetch tasks from given queue and return ordered
-    with oldest task in first position.
-    """
+    """Fetch tasks from redis."""
     tasks = []
     for obj_encoded in r.lrange(redis_queue_name, 0, -1):
         obj = json.loads(obj_encoded.decode("utf8"))
         try:
             tasks.append(QueuedTaskShort.from_dict(obj))
         except ValueError:
             pass
     return reversed(tasks)
 
 
-def fetch_tasks() -> List[QueuedTaskShort]:
-    """Fetch all tasks from queues and return as combined list."""
-    _fetch_func = functools.partial(_fetch_tasks_from_queue, _redis_client())
-    redis_queue_names = _redis_queue_names()
-    with concurrent.futures.ThreadPoolExecutor(
-        max_workers=len(redis_queue_names)
-    ) as executor:
-        tasks_raw = executor.map(_fetch_func, redis_queue_names)
-    tasks = list(itertools.chain(*tasks_raw))
-    return tasks
-
-
 def clear_tasks(queue_name: str = None):
     """Clear tasks from all queues."""
     r = _redis_client()
     for redis_queue_name in _redis_queue_names(queue_name):
         r.delete(redis_queue_name)
+    local_cache.clear()
 
 
 def add_tasks(queue_name: str, raw_tasks: list):
     """Push fake tasks to task queue."""
     r = _redis_client()
     if not queue_name:
         queue_name = default_queue_name()
@@ -116,7 +173,10 @@
         priority = task["properties"]["priority"]
         tasks_by_priority[priority].append(task)
     for priority, tasks in tasks_by_priority.items():
         raw_tasks_str = [json.dumps(obj) for obj in tasks]
         queue_name_raw = f"{queue_name}{PRIORITY_SEP}{priority}"
         r.lpush(queue_name_raw, *raw_tasks_str)
     del tasks_by_priority
+
+
+local_cache = CacheApi()
```

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/core/task_logs.py` & `aa-taskmonitor-0.9.1/taskmonitor/core/task_logs.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/core/task_records.py` & `aa-taskmonitor-0.9.1/taskmonitor/core/task_records.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/helpers.py` & `aa-taskmonitor-0.9.1/taskmonitor/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/managers.py` & `aa-taskmonitor-0.9.1/taskmonitor/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,21 @@
 
     def __init__(self, *args, model, distinct=False, **kwargs):
         self.model = model
         self.query = QuerySetQueryStub()
         self.distinct_enabled = distinct
         super().__init__(*args, **kwargs)
         self._id_mapper = {str(obj.id): n for n, obj in enumerate(self)}
+        self._list_size = len(self)
 
     def get(self, *args, **kwargs):
-        if "id" in kwargs:
-            try:
-                return self[self._id_mapper[str(kwargs["id"])]]
-            except KeyError:
-                raise self.model.DoesNotExist from None
-        raise self.model.DoesNotExist
+        try:
+            return self[self._id_mapper[str(kwargs["id"])]]
+        except KeyError:
+            raise self.model.DoesNotExist from None
 
     def distinct(self):
         return ListAsQuerySet(list(set(self)), model=self.model, distinct=True)
 
     def values(self, *args):
         result = [
             {k: v for k, v in obj.__dict__.items() if not args or k in args}
@@ -84,15 +83,15 @@
                     prop = prop[1:]
                 else:
                     reverse = False
                 self.sort(key=lambda d: getattr(d, prop), reverse=reverse)
         return self
 
     def count(self):
-        return len(self)
+        return self._list_size
 
     def _clone(self):
         return self
 
 
 class QueuedTaskQuerySet(models.QuerySet):
     def count(self):
```

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/migrations/0001_initial.py` & `aa-taskmonitor-0.9.1/taskmonitor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/migrations/0002_taskreport.py` & `aa-taskmonitor-0.9.1/taskmonitor/migrations/0002_taskreport.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/migrations/0003_queuedtask.py` & `aa-taskmonitor-0.9.1/taskmonitor/migrations/0003_queuedtask.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/migrations/0004_store_task_params_and_results.py` & `aa-taskmonitor-0.9.1/taskmonitor/migrations/0004_store_task_params_and_results.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/models.py` & `aa-taskmonitor-0.9.1/taskmonitor/models.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/signals.py` & `aa-taskmonitor-0.9.1/taskmonitor/signals.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/js/highcharts_defaults.js` & `aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/js/highcharts_defaults.js`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/vendor/highcharts/highcharts.js` & `aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/vendor/highcharts/highcharts.js`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/static/taskmonitor/vendor/highcharts/highcharts.js.map` & `aa-taskmonitor-0.9.1/taskmonitor/static/taskmonitor/vendor/highcharts/highcharts.js.map`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tasks.py` & `aa-taskmonitor-0.9.1/taskmonitor/tasks.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/change_form.html` & `aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/change_form.html`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/chart_throughput_partial.html` & `aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/chart_throughput_partial.html`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/report_barchart_partial.html` & `aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/report_barchart_partial.html`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/report_piechart_partial.html` & `aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/report_piechart_partial.html`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/report_table_partial.html` & `aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/report_table_partial.html`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/templates/admin/taskmonitor/tasklog/reports.html` & `aa-taskmonitor-0.9.1/taskmonitor/templates/admin/taskmonitor/tasklog/reports.html`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/core/test_cached_reports.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/core/test_cached_reports.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/core/test_celery_queues.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/core/test_celery_queues.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from unittest import mock
 
 from django.test import TestCase
 
 from taskmonitor.core import celery_queues
-from taskmonitor.core.celery_queues import QueuedTaskShort
+from taskmonitor.core.celery_queues import QueuedTaskShort, local_cache
 
 from ..factories import QueuedTaskRawFactory
 
 CELERY_QUEUE_NAME = "test_task_monitor_celery"
 MODULE_PATH = "taskmonitor.core.celery_queues"
 
 
+@mock.patch(MODULE_PATH + ".TASKMONITOR_QUEUED_TASKS_CACHE_TIMEOUT", 10)
 @mock.patch(MODULE_PATH + ".default_queue_name")
 class TestCeleryQueues(TestCase):
     def setUp(self):
         celery_queues.clear_tasks(CELERY_QUEUE_NAME)
 
     def tearDown(self):
         celery_queues.clear_tasks(CELERY_QUEUE_NAME)
@@ -41,13 +42,34 @@
         # given
         mock_queue_base_name.return_value = CELERY_QUEUE_NAME
         raw_task_1 = QueuedTaskRawFactory(properties__priority=4)
         raw_task_2 = QueuedTaskRawFactory(properties__priority=4)
         raw_task_3 = QueuedTaskRawFactory(properties__priority=3)
         celery_queues.add_tasks(CELERY_QUEUE_NAME, [raw_task_1, raw_task_2, raw_task_3])
         # when
-        result = celery_queues.fetch_tasks()
+        with mock.patch(MODULE_PATH + ".cache") as m:
+            m.get.return_value = None
+            result = celery_queues.fetch_tasks()
         # then
         self.assertEqual(len(result), 3)
         self.assertEqual(result[0], QueuedTaskShort.from_dict(raw_task_3))
         self.assertEqual(result[1], QueuedTaskShort.from_dict(raw_task_1))
         self.assertEqual(result[2], QueuedTaskShort.from_dict(raw_task_2))
+
+    def test_should_retrieve_tasks_from_cache(self, mock_queue_base_name):
+        # given
+        tasks = [QueuedTaskShort.from_dict(QueuedTaskRawFactory())]
+        local_cache.set(tasks)
+        # when
+        result = celery_queues.fetch_tasks()
+        # then
+        self.assertEqual(result, tasks)
+
+    def test_should_retrieve_tasks_from_redis_when_no_cache(self, mock_queue_base_name):
+        # given
+        mock_queue_base_name.return_value = CELERY_QUEUE_NAME
+        tasks = [QueuedTaskRawFactory()]
+        celery_queues.add_tasks(CELERY_QUEUE_NAME, tasks)
+        # when
+        result = celery_queues.fetch_tasks()
+        # then
+        self.assertEqual(result[0], QueuedTaskShort.from_dict(tasks[0]))
```

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/core/test_task_records.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/core/test_task_records.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/factories.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/generate_queued_tasks.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/generate_queued_tasks.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,14 +16,23 @@
 django.setup()
 
 """MAIN"""
 from taskmonitor.core import celery_queues
 from taskmonitor.tests.factories import QueuedTaskRawFactory
 
 TASK_AMOUNT = 1_000
+MAX_CHUNK_SIZE = 50_000  # upper limit to safe memory consumption
+
+
+def generate_tasks(amount: int):
+    tasks = (QueuedTaskRawFactory() for _ in range(amount))
+    celery_queues.add_tasks(q_name, tasks)
+
 
 print(f"Started adding {TASK_AMOUNT:,} tasks to queued tasks...")
 q_name = celery_queues.default_queue_name()
-tasks = (QueuedTaskRawFactory() for _ in range(TASK_AMOUNT))
-celery_queues.add_tasks(q_name, tasks)
+for _ in range(TASK_AMOUNT // MAX_CHUNK_SIZE):
+    generate_tasks(MAX_CHUNK_SIZE)
+generate_tasks(TASK_AMOUNT % MAX_CHUNK_SIZE)
 print(f"Using queue name: {q_name}")
 print(f"Added {TASK_AMOUNT:,} to queued tasks.")
+celery_queues.local_cache.clear()
```

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/generate_task_logs.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/generate_task_logs.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/test_admin.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/test_helpers.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/test_integration.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/test_models.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/test_tasks.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/tests/test_views.py` & `aa-taskmonitor-0.9.1/taskmonitor/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/urls.py` & `aa-taskmonitor-0.9.1/taskmonitor/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,8 +31,13 @@
         name="admin_taskmonitor_report_data",
     ),
     path(
         "admin_queued_task_purge",
         views.admin_queued_task_purge,
         name="admin_queued_task_purge",
     ),
+    path(
+        "admin_queued_task_clear_cache",
+        views.admin_queued_task_clear_cache,
+        name="admin_queued_task_clear_cache",
+    ),
 ]
```

### Comparing `aa-taskmonitor-0.9.0/taskmonitor/views.py` & `aa-taskmonitor-0.9.1/taskmonitor/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,7 +97,15 @@
 @staff_member_required
 def admin_queued_task_purge(request):
     """Purge the task queue."""
     queue_length = celery_queues.queue_length()
     celery_queues.clear_tasks()
     messages.info(request, f"Purged queue with {queue_length:,} tasks.")
     return redirect("admin:taskmonitor_queuedtask_changelist")
+
+
+@login_required
+@staff_member_required
+def admin_queued_task_clear_cache(request):
+    """Clear the cache for queued tasks."""
+    celery_queues.local_cache.clear()
+    return redirect("admin:taskmonitor_queuedtask_changelist")
```

