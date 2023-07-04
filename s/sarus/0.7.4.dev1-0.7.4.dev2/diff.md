# Comparing `tmp/sarus-0.7.4.dev1.tar.gz` & `tmp/sarus-0.7.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.7.4.dev1.tar", last modified: Fri Jun 30 06:58:25 2023, max compression
+gzip compressed data, was "sarus-0.7.4.dev2.tar", last modified: Mon Jul  3 19:54:27 2023, max compression
```

## Comparing `sarus-0.7.4.dev1.tar` & `sarus-0.7.4.dev2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.470848 sarus-0.7.4.dev1/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-06-30 06:58:25.470848 sarus-0.7.4.dev1/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.7.4.dev1/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.7.4.dev1/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.450842 sarus-0.7.4.dev1/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      549 2023-06-29 16:42:31.000000 sarus-0.7.4.dev1/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.454844 sarus-0.7.4.dev1/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13990 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.454844 sarus-0.7.4.dev1/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.454844 sarus-0.7.4.dev1/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.458845 sarus-0.7.4.dev1/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.458845 sarus-0.7.4.dev1/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8719 2023-06-22 14:51:31.000000 sarus-0.7.4.dev1/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.458845 sarus-0.7.4.dev1/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    20506 2023-06-29 16:42:31.000000 sarus-0.7.4.dev1/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.462846 sarus-0.7.4.dev1/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.462846 sarus-0.7.4.dev1/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.462846 sarus-0.7.4.dev1/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.462846 sarus-0.7.4.dev1/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    43166 2023-06-22 14:49:08.000000 sarus-0.7.4.dev1/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.462846 sarus-0.7.4.dev1/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.466847 sarus-0.7.4.dev1/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.466847 sarus-0.7.4.dev1/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.470848 sarus-0.7.4.dev1/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.470848 sarus-0.7.4.dev1/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-06-07 13:55:59.000000 sarus-0.7.4.dev1/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.470848 sarus-0.7.4.dev1/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.7.4.dev1/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.454844 sarus-0.7.4.dev1/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-06-30 06:58:25.000000 sarus-0.7.4.dev1/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1965 2023-06-30 06:58:25.000000 sarus-0.7.4.dev1/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-30 06:58:25.000000 sarus-0.7.4.dev1/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.7.4.dev1/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      359 2023-06-30 06:58:25.000000 sarus-0.7.4.dev1/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-06-30 06:58:25.000000 sarus-0.7.4.dev1/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1321 2023-06-30 06:58:25.470848 sarus-0.7.4.dev1/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      111 2023-06-29 16:42:31.000000 sarus-0.7.4.dev1/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 06:58:25.470848 sarus-0.7.4.dev1/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.7.4.dev1/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.7.4.dev2/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.7.4.dev2/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.182402 sarus-0.7.4.dev2/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      549 2023-07-03 19:53:43.000000 sarus-0.7.4.dev2/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13990 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8719 2023-06-22 14:51:31.000000 sarus-0.7.4.dev2/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    20367 2023-07-03 19:53:57.000000 sarus-0.7.4.dev2/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    43166 2023-06-22 14:49:08.000000 sarus-0.7.4.dev2/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.198402 sarus-0.7.4.dev2/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.198402 sarus-0.7.4.dev2/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1965 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.7.4.dev2/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      364 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1326 2023-07-03 19:54:27.206402 sarus-0.7.4.dev2/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      111 2023-07-03 19:53:24.000000 sarus-0.7.4.dev2/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.7.4.dev2/tests/test_sanity.py
```

### Comparing `sarus-0.7.4.dev1/PKG-INFO` & `sarus-0.7.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.7.4.dev1
+Version: 0.7.4.dev2
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.7.4.dev1/README.rst` & `sarus-0.7.4.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/__init__.py` & `sarus-0.7.4.dev2/sarus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.7.4-dev1"
+VERSION = "0.7.4.dev2"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.7.4.dev1/sarus/config.yaml` & `sarus-0.7.4.dev2/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/context/local_sdk.py` & `sarus-0.7.4.dev2/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/dataspec_wrapper.py` & `sarus-0.7.4.dev2/sarus/dataspec_wrapper.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/debug.py` & `sarus-0.7.4.dev2/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/imblearn/over_sampling.py` & `sarus-0.7.4.dev2/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/imblearn/pipeline.py` & `sarus-0.7.4.dev2/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/imblearn/under_sampling.py` & `sarus-0.7.4.dev2/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/legacy/tensorflow/dataset.py` & `sarus-0.7.4.dev2/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/legacy/tensorflow/model.py` & `sarus-0.7.4.dev2/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/arrow_local.py` & `sarus-0.7.4.dev2/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/arrow_remote.py` & `sarus-0.7.4.dev2/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/base_remote.py` & `sarus-0.7.4.dev2/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/cache_scalar_local.py` & `sarus-0.7.4.dev2/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/dataspec_api.py` & `sarus-0.7.4.dev2/sarus/manager/dataspec_api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/ops/api.py` & `sarus-0.7.4.dev2/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/parquet_local.py` & `sarus-0.7.4.dev2/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/sdk_manager.py` & `sarus-0.7.4.dev2/sarus/manager/sdk_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,18 +141,16 @@
         # `select_sql` transforms are delegated, whether mock or not
         if dataspec.is_transformed():
             transform = dataspec.transform()
             if transform.protobuf().spec.HasField(
                 "select_sql"
             ) or transform.protobuf().spec.HasField("dp_select_sql"):
                 computation_graph = self.computation_graph(dataspec)
-                referrables = (
-                    list(computation_graph["dataspecs"])
-                    + list(computation_graph["transforms"])
-                    + list(computation_graph["attributes"])
+                referrables = list(computation_graph["dataspecs"]) + list(
+                    computation_graph["transforms"]
                 )
                 api.push_dataspec_graph(self._client, referrables)
 
         ds = api.get_dataspec(self.client(), dataspec.uuid())
         return ds is not None
 
     def is_big_data(self, dataset: st.Dataset) -> bool:
@@ -180,18 +178,16 @@
                 IS_BIG_DATA
             ] == str(True)
         return super().is_big_data(dataset)
 
     def push(self, dataspec: st.DataSpec) -> None:
         """Push a Dataspec's computation graph on the server."""
         computation_graph = self.computation_graph(dataspec)
-        referrables = (
-            list(computation_graph["dataspecs"])
-            + list(computation_graph["transforms"])
-            + list(computation_graph["attributes"])
+        referrables = list(computation_graph["dataspecs"]) + list(
+            computation_graph["transforms"]
         )
         api.push_dataspec_graph(self.client(), referrables)
 
     def compile(
         self, dataspec: st.DataSpec, target_epsilon: t.Optional[float] = None
     ) -> t.Tuple[st.DataSpec, DataspecPrivacyPolicy]:
         """Compile an alternative Dataspec."""
@@ -238,15 +234,16 @@
             dataspec, name=PYTHON_TYPE, properties={PYTHON_TYPE: type_str}
         )
         return type_str
 
     Edge = t.Tuple[st.DataSpec, st.DataSpec, st.Transform]
 
     def computation_graph(
-        self, dataspec: st.DataSpec
+        self,
+        dataspec: st.DataSpec,
     ) -> t.Dict[str, t.Union[st.DataSpec, st.Transform, st.Attribute, Edge]]:
         """Retreive all items necessary to compute a DataSpec.
 
         This function is used intensively to post DataSpecs, draw dot
         representationss, fetch statuses, and so on.
         """
         storage = self.storage()
```

### Comparing `sarus-0.7.4.dev1/sarus/manager/typing.py` & `sarus-0.7.4.dev2/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/value_local.py` & `sarus-0.7.4.dev2/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/manager/value_remote.py` & `sarus-0.7.4.dev2/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/numpy/scalars.py` & `sarus-0.7.4.dev2/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/pandas/core.py` & `sarus-0.7.4.dev2/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/pandas/dataframe.py` & `sarus-0.7.4.dev2/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sarus.py` & `sarus-0.7.4.dev2/sarus/sarus.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/scripts/generate_op_list.py` & `sarus-0.7.4.dev2/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/__init__.py` & `sarus-0.7.4.dev2/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/cluster.py` & `sarus-0.7.4.dev2/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/compose.py` & `sarus-0.7.4.dev2/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/decomposition.py` & `sarus-0.7.4.dev2/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/ensemble.py` & `sarus-0.7.4.dev2/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/impute.py` & `sarus-0.7.4.dev2/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/linear_model.py` & `sarus-0.7.4.dev2/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/model_selection.py` & `sarus-0.7.4.dev2/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/pipeline.py` & `sarus-0.7.4.dev2/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/preprocessing.py` & `sarus-0.7.4.dev2/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/sklearn/svm.py` & `sarus-0.7.4.dev2/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/skopt/searchcv.py` & `sarus-0.7.4.dev2/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/std/types.py` & `sarus-0.7.4.dev2/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/typing.py` & `sarus-0.7.4.dev2/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/utils.py` & `sarus-0.7.4.dev2/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/wrapper_factory.py` & `sarus-0.7.4.dev2/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus/xgboost/xgboost.py` & `sarus-0.7.4.dev2/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/sarus.egg-info/PKG-INFO` & `sarus-0.7.4.dev2/sarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.7.4.dev1
+Version: 0.7.4.dev2
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.7.4.dev1/sarus.egg-info/SOURCES.txt` & `sarus-0.7.4.dev2/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev1/setup.cfg` & `sarus-0.7.4.dev2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.5.5
+	sarus-data-spec-public==3.5.8.dev1
 	cloudpickle>=1.2, <2.1
 	pyarrow >= 11.0
 	protobuf >= 3.20.3
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.2.2
```

