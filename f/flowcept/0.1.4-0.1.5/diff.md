# Comparing `tmp/flowcept-0.1.4.tar.gz` & `tmp/flowcept-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowcept-0.1.4.tar", last modified: Fri Jun 30 20:18:59 2023, max compression
+gzip compressed data, was "flowcept-0.1.5.tar", last modified: Mon Jul  3 22:11:45 2023, max compression
```

## Comparing `flowcept-0.1.4.tar` & `flowcept-0.1.5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-30 20:18:48.000000 flowcept-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-30 20:18:59.247320 flowcept-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-30 20:18:48.000000 flowcept-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept/commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept/commons/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/daos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/daos/document_db_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/daos/mq_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/flowcept_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowcept_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_api/consumer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_api/task_query_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowcept_webserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowcept_webserver/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/resources/query_rsrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/resources/task_messages_rsrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/consumers/consumer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/consumers/document_inserter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/base_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/base_settings_dataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/interceptor_state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/interception_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/settings_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/tensorboard_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/telemetry_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-30 20:18:49.000000 flowcept-0.1.4/flowcept/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 20:18:48.000000 flowcept-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:18:59.247320 flowcept-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-30 20:18:48.000000 flowcept-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/api/query_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/doc_db_inserter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/doc_db_inserter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/doc_db_inserter/doc_db_inserter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/log_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/log_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/log_tests/log_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/log_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/test_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/test_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/test_zambeze.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/telemetry_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.169906 flowcept-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-03 22:11:34.000000 flowcept-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-03 22:11:45.169906 flowcept-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-03 22:11:34.000000 flowcept-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.157905 flowcept-0.1.5/flowcept/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept/commons/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/daos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/daos/document_db_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/daos/mq_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept/commons/flowcept_dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/flowcept_dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/flowcept_dataclasses/task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/flowcept_dataclasses/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/flowcept_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/commons/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept/flowcept_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowcept_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowcept_api/consumer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowcept_api/task_query_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept/flowcept_webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowcept_webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowcept_webserver/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept/flowcept_webserver/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowcept_webserver/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowcept_webserver/resources/query_rsrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowcept_webserver/resources/task_messages_rsrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept/flowceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept/flowceptor/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/consumers/consumer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/consumers/document_inserter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/flowcept/flowceptor/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/base_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/base_settings_dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/flowcept/flowceptor/plugins/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/dask/dask_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/dask/dask_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/dask/dask_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/interceptor_state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/interception_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/settings_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/flowcept/flowceptor/plugins/tensorboard/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/tensorboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/tensorboard/tensorboard_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/flowcept/flowceptor/plugins/zambeze/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/zambeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/flowceptor/telemetry_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-03 22:11:34.000000 flowcept-0.1.5/flowcept/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 22:11:35.000000 flowcept-0.1.5/flowcept/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.161905 flowcept-0.1.5/flowcept.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-03 22:11:45.000000 flowcept-0.1.5/flowcept.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-03 22:11:45.000000 flowcept-0.1.5/flowcept.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:11:45.000000 flowcept-0.1.5/flowcept.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-03 22:11:45.000000 flowcept-0.1.5/flowcept.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 22:11:45.000000 flowcept-0.1.5/flowcept.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 22:11:34.000000 flowcept-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:11:45.169906 flowcept-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-03 22:11:34.000000 flowcept-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/api/query_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/tests/doc_db_inserter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/doc_db_inserter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/doc_db_inserter/doc_db_inserter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.165906 flowcept-0.1.5/tests/log_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/log_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/log_tests/log_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/log_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:45.169906 flowcept-0.1.5/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/plugins/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/plugins/test_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/plugins/test_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/plugins/test_zambeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-03 22:11:34.000000 flowcept-0.1.5/tests/telemetry_test.py
```

### Comparing `flowcept-0.1.4/LICENSE` & `flowcept-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/PKG-INFO` & `flowcept-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowcept
-Version: 0.1.4
+Version: 0.1.5
 Summary: FlowCept is a runtime data integration system that empowers any data processing system to capture and query workflow provenance data using data observability, requiring minimal or no changes in the target system code. It seamlessly integrates data from multiple workflows, enabling users to comprehend complex, heterogeneous, and large-scale data from various sources in federated environments.
 Home-page: https://github.com/ORNL/flowcept
 Author: Oak Ridge National Laboratory
 License: MIT
 Keywords: ai,ml,machine-learning,provenance,lineage,responsible-ai,databases,big-data,provenance,tensorboard,data-integration,scientific-workflows,dask,reproducibility,workflows,parallel-processing,lineage,model-management,mlflow,responsible-ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flowcept-0.1.4/README.md` & `flowcept-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/__init__.py` & `flowcept-0.1.5/flowcept/__init__.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/commons/daos/document_db_dao.py` & `flowcept-0.1.5/flowcept/commons/daos/document_db_dao.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/commons/daos/mq_dao.py` & `flowcept-0.1.5/flowcept/commons/daos/mq_dao.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/task_message.py` & `flowcept-0.1.5/flowcept/commons/flowcept_dataclasses/task_message.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/commons/flowcept_logger.py` & `flowcept-0.1.5/flowcept/commons/flowcept_logger.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/commons/utils.py` & `flowcept-0.1.5/flowcept/commons/utils.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/configs.py` & `flowcept-0.1.5/flowcept/configs.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowcept_api/consumer_api.py` & `flowcept-0.1.5/flowcept/flowcept_api/consumer_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from typing import List, Union
 from time import sleep
-import random
 
 from flowcept.commons.daos.mq_dao import MQDao
-from flowcept.configs import (
-    REDIS_INSERTION_BUFFER_TIME,
-    MONGO_INSERTION_BUFFER_TIME,
-)
 from flowcept.flowceptor.consumers.document_inserter import DocumentInserter
 from flowcept.commons.flowcept_logger import FlowceptLogger
 from flowcept.flowceptor.plugins.base_interceptor import BaseInterceptor
 
 
 class FlowceptConsumerAPI(object):
     def __init__(
```

### Comparing `flowcept-0.1.4/flowcept/flowcept_api/task_query_api.py` & `flowcept-0.1.5/flowcept/flowcept_api/task_query_api.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowcept_webserver/app.py` & `flowcept-0.1.5/flowcept/flowcept_webserver/app.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowcept_webserver/resources/query_rsrc.py` & `flowcept-0.1.5/flowcept/flowcept_webserver/resources/query_rsrc.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowcept_webserver/resources/task_messages_rsrc.py` & `flowcept-0.1.5/flowcept/flowcept_webserver/resources/task_messages_rsrc.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/consumers/consumer_utils.py` & `flowcept-0.1.5/flowcept/flowceptor/consumers/consumer_utils.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/consumers/document_inserter.py` & `flowcept-0.1.5/flowcept/flowceptor/consumers/document_inserter.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/base_interceptor.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/base_interceptor.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     EXTRA_METADATA,
 )
 from flowcept.commons.flowcept_logger import FlowceptLogger
 from flowcept.commons.daos.mq_dao import MQDao
 from flowcept.commons.flowcept_dataclasses.task_message import TaskMessage
 from flowcept.flowceptor.plugins.settings_factory import get_settings
 
+from flowcept.flowceptor.telemetry_capture import TelemetryCapture
+
 from flowcept.version import __version__
 
 
 def _enrich_task_message(settings_key, task_msg: TaskMessage):
     if task_msg.utc_timestamp is None:
         task_msg.utc_timestamp = get_utc_now()
 
@@ -59,32 +61,35 @@
 
 
 class BaseInterceptor(object, metaclass=ABCMeta):
     def __init__(self, plugin_key):
         self.logger = FlowceptLogger().get_logger()
         self.settings = get_settings(plugin_key)
         self._mq_dao = MQDao()
+        self.telemetry_capture = TelemetryCapture()
 
     def prepare_task_msg(self, *args, **kwargs) -> TaskMessage:
         raise NotImplementedError()
 
     def start(self) -> "BaseInterceptor":
         """
         Starts an interceptor
         :return:
         """
         self._mq_dao.start_time_based_flushing()
+        self.telemetry_capture.init_gpu_telemetry()
         return self
 
     def stop(self) -> bool:
         """
         Gracefully stops an interceptor
         :return:
         """
         self._mq_dao.stop()
+        self.telemetry_capture.shutdown_gpu_telemetry()
 
     def observe(self, *args, **kwargs):
         """
         This method implements data observability over a data channel
          (e.g., a file, a DBMS, an MQ)
         :return:
         """
```

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_interceptor.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/dask/dask_interceptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     Status,
 )
 from flowcept.flowceptor.plugins.base_interceptor import (
     BaseInterceptor,
 )
 from flowcept.commons.utils import get_utc_now
 from flowcept.configs import TELEMETRY_CAPTURE
-from flowcept.flowceptor.telemetry_capture import capture_telemetry
 
 
 def get_run_spec_data(task_msg: TaskMessage, run_spec):
     def _get_arg(arg_name):
         if type(run_spec) == dict:
             return run_spec.get(arg_name, None)
         elif hasattr(run_spec, arg_name):
@@ -144,39 +143,45 @@
             ts = self._worker.state.tasks[task_id]
 
             task_msg = TaskMessage()
             task_msg.task_id = task_id
 
             if ts.state == "executing":
                 if TELEMETRY_CAPTURE is not None:
-                    task_msg.telemetry_at_start = capture_telemetry()
+                    task_msg.telemetry_at_start = (
+                        self.telemetry_capture.capture()
+                    )
                 task_msg.status = Status.RUNNING
                 task_msg.address = self._worker.worker_address
                 if self.settings.worker_create_timestamps:
                     task_msg.started_at = get_utc_now()
             elif ts.state == "memory":
                 task_msg.status = Status.FINISHED
                 if self.settings.worker_create_timestamps:
                     task_msg.ended_at = get_utc_now()
                 else:
                     get_times_from_task_state(task_msg, ts)
                 if TELEMETRY_CAPTURE is not None:
-                    task_msg.telemetry_at_end = capture_telemetry()
+                    task_msg.telemetry_at_end = (
+                        self.telemetry_capture.capture()
+                    )
             elif ts.state == "error":
                 task_msg.status = Status.ERROR
                 if self.settings.worker_create_timestamps:
                     task_msg.ended_at = get_utc_now()
                 else:
                     get_times_from_task_state(task_msg, ts)
                 task_msg.stderr = {
                     "exception": ts.exception_text,
                     "traceback": ts.traceback_text,
                 }
                 if TELEMETRY_CAPTURE is not None:
-                    task_msg.telemetry_at_end = capture_telemetry()
+                    task_msg.telemetry_at_end = (
+                        self.telemetry_capture.capture()
+                    )
             else:
                 return
 
             if self.settings.worker_should_get_input:
                 if hasattr(ts, "run_spec"):
                     get_run_spec_data(task_msg, ts.run_spec)
```

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_plugins.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/dask/dask_plugins.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/interceptor_state_manager.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/interceptor_state_manager.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/settings_factory.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/settings_factory.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py` & `flowcept-0.1.5/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept/main.py` & `flowcept-0.1.5/flowcept/main.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept.egg-info/PKG-INFO` & `flowcept-0.1.5/flowcept.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowcept
-Version: 0.1.4
+Version: 0.1.5
 Summary: FlowCept is a runtime data integration system that empowers any data processing system to capture and query workflow provenance data using data observability, requiring minimal or no changes in the target system code. It seamlessly integrates data from multiple workflows, enabling users to comprehend complex, heterogeneous, and large-scale data from various sources in federated environments.
 Home-page: https://github.com/ORNL/flowcept
 Author: Oak Ridge National Laboratory
 License: MIT
 Keywords: ai,ml,machine-learning,provenance,lineage,responsible-ai,databases,big-data,provenance,tensorboard,data-integration,scientific-workflows,dask,reproducibility,workflows,parallel-processing,lineage,model-management,mlflow,responsible-ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flowcept-0.1.4/flowcept.egg-info/SOURCES.txt` & `flowcept-0.1.5/flowcept.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/flowcept.egg-info/requires.txt` & `flowcept-0.1.5/flowcept.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 PyYAML==6.0
 redis==4.4.2
 psutil==5.9.5
+nvidia-ml-py==11.525.131
 
 [dask]
 tomli==1.1.0
 dask[distributed]==2022.12.0
 
 [full]
 PyYAML==6.0
 redis==4.4.2
 psutil==5.9.5
+nvidia-ml-py==11.525.131
 pika==1.3.1
 mlflow-skinny==2.1.1
 SQLAlchemy==1.4.42
 alembic==1.8.1
 watchdog==2.2.1
 pandas==1.5.1
 tensorboard==2.11.0
```

### Comparing `flowcept-0.1.4/setup.py` & `flowcept-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     "responsible-ai",
 ]
 
 short_description, long_description = get_descriptions()
 
 
 setup(
-    name="flowcept",
+    name=PROJECT_NAME,
     version=version,
     license="MIT",
     author="Oak Ridge National Laboratory",
     # author_email="support@flowcept.org",
     description=short_description,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `flowcept-0.1.4/tests/api/query_test.py` & `flowcept-0.1.5/tests/api/query_test.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/tests/doc_db_inserter/doc_db_inserter_test.py` & `flowcept-0.1.5/tests/doc_db_inserter/doc_db_inserter_test.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/tests/log_tests/log_test.py` & `flowcept-0.1.5/tests/log_tests/log_test.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/tests/plugins/test_dask.py` & `flowcept-0.1.5/tests/plugins/test_dask.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/tests/plugins/test_mlflow.py` & `flowcept-0.1.5/tests/plugins/test_mlflow.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/tests/plugins/test_tensorboard.py` & `flowcept-0.1.5/tests/plugins/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.4/tests/plugins/test_zambeze.py` & `flowcept-0.1.5/tests/plugins/test_zambeze.py`

 * *Files identical despite different names*

