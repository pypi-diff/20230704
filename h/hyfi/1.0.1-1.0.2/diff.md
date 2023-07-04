# Comparing `tmp/hyfi-1.0.1.tar.gz` & `tmp/hyfi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.0.1.tar", max compression
+gzip compressed data, was "hyfi-1.0.2.tar", max compression
```

## Comparing `hyfi-1.0.1.tar` & `hyfi-1.0.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1071 2023-07-04 04:57:08.966086 hyfi-1.0.1/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-04 04:57:08.966086 hyfi-1.0.1/README.md
--rw-r--r--   0        0        0     4862 2023-07-04 04:57:35.845891 hyfi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4267 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2550 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__click__.py
--rw-r--r--   0        0        0      788 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9245 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-04 04:57:35.769891 hyfi-1.0.1/src/hyfi/_version.py
--rw-r--r--   0        0        0     1890 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7229 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    31944 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7331 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/composer/extended.py
--rw-r--r--   0        0        0        0 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-04 04:57:35.769891 hyfi-1.0.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      427 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      785 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      166 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      178 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      351 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      395 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6548 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     5915 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4474 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13831 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    50188 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     7754 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0      782 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      434 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     4261 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8085 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5155 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/py.typed
--rw-r--r--   0        0        0     4268 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     6518 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30058 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6568 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     3769 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20157 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-04 04:57:08.978087 hyfi-1.0.1/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-04 04:57:08.978087 hyfi-1.0.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      753 2023-07-04 04:57:08.978087 hyfi-1.0.1/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 hyfi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 06:55:39.646139 hyfi-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-04 06:55:39.646139 hyfi-1.0.2/README.md
+-rw-r--r--   0        0        0     4862 2023-07-04 06:56:18.886321 hyfi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4267 2023-07-04 06:55:39.650138 hyfi-1.0.2/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2550 2023-07-04 06:55:39.650138 hyfi-1.0.2/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      788 2023-07-04 06:55:39.650138 hyfi-1.0.2/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9245 2023-07-04 06:55:39.650138 hyfi-1.0.2/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      733 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-04 06:56:18.774320 hyfi-1.0.2/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1890 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    31944 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7331 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/composer/extended.py
+-rw-r--r--   0        0        0        0 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-04 06:56:18.778320 hyfi-1.0.2/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      427 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      785 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      166 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      178 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      351 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      395 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6548 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5915 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4228 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    50188 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     7754 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0      782 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      434 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     4261 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8085 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5155 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     6518 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30058 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     3769 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-04 06:55:39.662139 hyfi-1.0.2/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-04 06:55:39.662139 hyfi-1.0.2/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-04 06:55:39.662139 hyfi-1.0.2/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 hyfi-1.0.2/PKG-INFO
```

### Comparing `hyfi-1.0.1/LICENSE` & `hyfi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/README.md` & `hyfi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/pyproject.toml` & `hyfi-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.0.1"
+version = "1.0.2"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.0.1/src/hyfi/__cli__.py` & `hyfi-1.0.2/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/__click__.py` & `hyfi-1.0.2/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/__global__/__init__.py` & `hyfi-1.0.2/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/__global__/config.py` & `hyfi-1.0.2/src/hyfi/__global__/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/__init__.py` & `hyfi-1.0.2/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/about/__init__.py` & `hyfi-1.0.2/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/batch/__init__.py` & `hyfi-1.0.2/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/__init__.py` & `hyfi-1.0.2/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.0.2/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/cache_file.py` & `hyfi-1.0.2/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/common.py` & `hyfi-1.0.2/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/file_lock.py` & `hyfi-1.0.2/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/meta.py` & `hyfi-1.0.2/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/progress.py` & `hyfi-1.0.2/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.0.2/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.0.2/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.0.2/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.0.2/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.0.2/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/testing.py` & `hyfi-1.0.2/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/cached_path/util.py` & `hyfi-1.0.2/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/composer/__init__.py` & `hyfi-1.0.2/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/composer/extended.py` & `hyfi-1.0.2/src/hyfi/composer/extended.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.0.2/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.0.2/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.0.2/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.0.2/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.0.2/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.0.2/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/copier/__init__.py` & `hyfi-1.0.2/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/dotenv/__init__.py` & `hyfi-1.0.2/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/graphics/collage.py` & `hyfi-1.0.2/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/graphics/motion.py` & `hyfi-1.0.2/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/graphics/utils.py` & `hyfi-1.0.2/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/joblib/__init__.py` & `hyfi-1.0.2/src/hyfi/joblib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,79 @@
 from typing import Callable, Mapping, Optional, Sequence, Union
 
 import pandas as pd
-from pydantic import BaseModel, PrivateAttr
+from pydantic import PrivateAttr
 from tqdm.auto import tqdm
 
 from hyfi import __global__
 from hyfi.composer import BaseConfig
 from hyfi.joblib.batch import batcher
 from hyfi.joblib.batch.apply import decorator_apply
 from hyfi.joblib.batch.batcher import Batcher
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
-class DistFramworkConfig(BaseModel):
-    """Distributed Framework Configuration"""
-
-    backend: str = "joblib"
-    initialize: bool = False
-    num_workers: int = 1
-
-
-class BatcherConfig(BaseModel):
-    """Batcher Configuration"""
-
-    procs: int = 1
-    minibatch_size: int = 1_000
-    backend: str = "joblib"
-    task_num_cpus: int = 1
-    task_num_gpus: int = 0
-    verbose: int = 10
-
-
 class JobLibConfig(BaseConfig):
     """JobLib Configuration"""
 
     _config_name_: str = "__init__"
     _config_group_: str = "joblib"
 
+    backend: str = "joblib"
+    initialize_backend: bool = False
+    minibatch_size: int = 1_000
     num_workers: int = 1
-    distributed_framework: DistFramworkConfig = DistFramworkConfig()
-    batcher: BatcherConfig = BatcherConfig()
+    task_num_gpus: int = 0
+
     _initilized_: bool = PrivateAttr(False)
     _batcher_instance_: Optional[Batcher] = PrivateAttr(None)
 
     def initialize(self):
         self.init_backend()
 
     def init_backend(
         self,
     ):
         """Initialize the backend for joblib"""
-        if self.distributed_framework.initialize:
+        if self.initialize_backend:
             backend_handle = None
-            backend = self.distributed_framework.backend
+            backend = self.backend
 
             if backend == "ray":
                 import ray  # type: ignore
 
-                ray_cfg = {"num_cpus": self.distributed_framework.num_workers}
+                ray_cfg = {"num_cpus": self.num_workers}
                 logger.debug(f"initializing ray with {ray_cfg}")
                 ray.init(**ray_cfg)
                 backend_handle = ray
 
             __global__._batcher_instance_ = batcher.Batcher(
-                backend_handle=backend_handle, **self.batcher.model_dump()
+                backend_handle=backend_handle,
+                backend=self.backend,
+                procs=self.num_workers,
+                minibatch_size=self.minibatch_size,
+                task_num_cpus=self.num_workers,
+                task_num_gpus=self.task_num_gpus,
+                verbose=self.verbose,
             )
             self._batcher_instance_ = __global__._batcher_instance_
             logger.debug("initialized batcher with %s", __global__._batcher_instance_)
         self._initilized_ = True
 
     def stop_backend(self):
         """Stop the backend for joblib"""
-        backend = self.distributed_framework.backend
+        backend = self.backend
         if __global__._batcher_instance_:
             logger.debug("stopping batcher")
             del __global__._batcher_instance_
 
         logger.debug("stopping distributed framework")
-        if self.distributed_framework.initialize and backend == "ray":
+        if self.initialize_backend and backend == "ray":
             try:
                 import ray  # type: ignore
 
                 if ray.is_initialized():
                     ray.shutdown()
                     logger.debug("shutting down ray")
             except ImportError:
```

### Comparing `hyfi-1.0.1/src/hyfi/joblib/batch/apply.py` & `hyfi-1.0.2/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.0.2/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.0.2/src/hyfi/joblib/batch/batcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
             data (list):
                 List of minibatches to merge
 
         Returns:
             data (list, numpy.ndarray, scipy.sparse.csr_matrix, pandas.DataFrame):
                 Single complete list-like data merged from given batches
         """
+        print(data)
         if isinstance(data[0], ssp.csr_matrix):  # type: ignore
             return ssp.vstack(data)  # type: ignore
         if isinstance(data[0], (pd.DataFrame, pd.Series)):
             return pd.concat(data)
         return [item for sublist in data for item in sublist]
 
     def process_batches(
@@ -232,15 +233,15 @@
             task_num_cpus = self.task_num_cpus
         if task_num_gpus is None:
             task_num_gpus = self.task_num_gpus
         if verbose is None:
             verbose = self.verbose
         # if verbose > 1:
         logger.debug(
-            " backend: %s  minibatch_size: %s  procs: %s  input_split: %s  merge_output: %s  len(data): %s len(args): %s",
+            "backend: %s, minibatch_size: %s, procs: %s, input_split: %s, merge_output: %s, len(data): %s, len(args): %s",
             backend,
             self.minibatch_size,
             procs,
             input_split,
             merge_output,
             len(data),
             len(args),
@@ -258,16 +259,15 @@
         if not (input_split):
             paral_params = [
                 [data_batch] + args
                 for data_batch in self.split_batches(data, minibatch_size)
             ]
         else:
             paral_params = [[data_batch] + args for data_batch in data]
-        if verbose > 1:
-            logger.debug("Start task, len(paral_params): %s", len(paral_params))
+        logger.debug("Start task, len(paral_params): %s", len(paral_params))
         results = []
         if backend == "serial":
             results = [
                 task(minibatch) for minibatch in tqdm(paral_params, desc=description)
             ]
         else:
             if backend == "multiprocessing":
```

### Comparing `hyfi-1.0.1/src/hyfi/main/__init__.py` & `hyfi-1.0.2/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/path/__init__.py` & `hyfi-1.0.2/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/path/batch.py` & `hyfi-1.0.2/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/path/task.py` & `hyfi-1.0.2/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/pipe/__init__.py` & `hyfi-1.0.2/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/pipe/test.py` & `hyfi-1.0.2/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/pipeline/__init__.py` & `hyfi-1.0.2/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/pipeline/configs.py` & `hyfi-1.0.2/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/project/__init__.py` & `hyfi-1.0.2/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/task/__init__.py` & `hyfi-1.0.2/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/task/batch.py` & `hyfi-1.0.2/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/contexts.py` & `hyfi-1.0.2/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/datasets.py` & `hyfi-1.0.2/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/envs.py` & `hyfi-1.0.2/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/funcs.py` & `hyfi-1.0.2/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/gpumon.py` & `hyfi-1.0.2/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/iolibs.py` & `hyfi-1.0.2/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/logging.py` & `hyfi-1.0.2/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/notebooks.py` & `hyfi-1.0.2/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/utils/packages.py` & `hyfi-1.0.2/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/src/hyfi/workflow/__init__.py` & `hyfi-1.0.2/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.1/PKG-INFO` & `hyfi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

