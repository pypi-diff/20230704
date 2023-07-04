# Comparing `tmp/hyfi-1.0.0.tar.gz` & `tmp/hyfi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.0.0.tar", max compression
+gzip compressed data, was "hyfi-1.0.1.tar", max compression
```

## Comparing `hyfi-1.0.0.tar` & `hyfi-1.0.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1071 2023-07-04 01:01:20.590560 hyfi-1.0.0/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-04 01:01:20.590560 hyfi-1.0.0/README.md
--rw-r--r--   0        0        0     4862 2023-07-04 01:01:49.699067 hyfi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4267 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2550 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      788 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9245 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-04 01:01:49.623065 hyfi-1.0.0/src/hyfi/_version.py
--rw-r--r--   0        0        0     1890 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7229 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    31944 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7331 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/composer/extended.py
--rw-r--r--   0        0        0        0 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-04 01:01:49.623065 hyfi-1.0.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      427 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      785 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      166 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      237 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      242 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      178 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      351 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      381 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6548 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     5911 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4474 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13831 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    50188 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     7754 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0      782 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      434 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     4261 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     7985 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5155 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     4268 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     6518 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30058 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6568 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     3769 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20157 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      762 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 hyfi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 04:57:08.966086 hyfi-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-04 04:57:08.966086 hyfi-1.0.1/README.md
+-rw-r--r--   0        0        0     4862 2023-07-04 04:57:35.845891 hyfi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4267 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2550 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      788 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9245 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      733 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-04 04:57:35.769891 hyfi-1.0.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1890 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    31944 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7331 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/composer/extended.py
+-rw-r--r--   0        0        0        0 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-04 04:57:35.769891 hyfi-1.0.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      427 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-04 04:57:08.970086 hyfi-1.0.1/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      785 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      166 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      178 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      351 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      395 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6548 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5915 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4474 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13831 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    50188 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     7754 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0      782 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      434 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     4261 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8085 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5155 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     6518 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30058 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     3769 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-04 04:57:08.974087 hyfi-1.0.1/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-04 04:57:08.978087 hyfi-1.0.1/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-04 04:57:08.978087 hyfi-1.0.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-04 04:57:08.978087 hyfi-1.0.1/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 hyfi-1.0.1/PKG-INFO
```

### Comparing `hyfi-1.0.0/LICENSE` & `hyfi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/README.md` & `hyfi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/pyproject.toml` & `hyfi-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.0.0"
+version = "1.0.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.0.0/src/hyfi/__cli__.py` & `hyfi-1.0.1/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/__click__.py` & `hyfi-1.0.1/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/__global__/__init__.py` & `hyfi-1.0.1/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/__global__/config.py` & `hyfi-1.0.1/src/hyfi/__global__/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/__init__.py` & `hyfi-1.0.1/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/about/__init__.py` & `hyfi-1.0.1/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/batch/__init__.py` & `hyfi-1.0.1/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/__init__.py` & `hyfi-1.0.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.0.1/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/cache_file.py` & `hyfi-1.0.1/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/common.py` & `hyfi-1.0.1/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/file_lock.py` & `hyfi-1.0.1/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/meta.py` & `hyfi-1.0.1/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/progress.py` & `hyfi-1.0.1/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.0.1/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.0.1/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.0.1/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.0.1/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.0.1/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/testing.py` & `hyfi-1.0.1/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/cached_path/util.py` & `hyfi-1.0.1/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/composer/__init__.py` & `hyfi-1.0.1/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/composer/extended.py` & `hyfi-1.0.1/src/hyfi/composer/extended.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.0.1/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.0.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.0.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.0.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.0.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.0.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/copier/__init__.py` & `hyfi-1.0.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/dotenv/__init__.py` & `hyfi-1.0.1/src/hyfi/dotenv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,13 +122,13 @@
             env_settings,
             file_secret_settings,
             init_settings,
         )
 
     @model_validator(mode="after")  # type: ignore
     def check_and_set_values(cls, m: "DotEnvConfig"):
-        return ENVs.check_and_set_osenv_vars(m.__dict__)
+        return ENVs.check_and_set_osenv_vars(m.model_dump())
 
     @property
     def os(self):
         """Returns the OS environment variables."""
         return os.environ
```

### Comparing `hyfi-1.0.0/src/hyfi/graphics/collage.py` & `hyfi-1.0.1/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/graphics/motion.py` & `hyfi-1.0.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/graphics/utils.py` & `hyfi-1.0.1/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/joblib/__init__.py` & `hyfi-1.0.1/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/joblib/batch/apply.py` & `hyfi-1.0.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.0.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.0.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/main/__init__.py` & `hyfi-1.0.1/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/path/__init__.py` & `hyfi-1.0.1/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/path/batch.py` & `hyfi-1.0.1/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/path/task.py` & `hyfi-1.0.1/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/pipe/__init__.py` & `hyfi-1.0.1/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/pipe/test.py` & `hyfi-1.0.1/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/pipeline/__init__.py` & `hyfi-1.0.1/src/hyfi/pipeline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,17 +206,17 @@
             task: The task to get the pipelines for
 
         Returns:
             A list of PipelineConfig objects
         """
         task.pipelines = task.pipelines or []
         pipelines: Pipelines = [
-            PipelineConfig(**task.__dict__[name])
+            PipelineConfig(**getattr(task, name))
             for name in task.pipelines
-            if name in task.__dict__ and isinstance(task.__dict__[name], dict)
+            if isinstance(name, str) and isinstance(getattr(task, name), dict)
         ]
         return pipelines
 
     @staticmethod
     def run_task(task: TaskConfig, project: Optional[ProjectConfig] = None):
         """
         Run pipelines specified in the task
@@ -225,14 +225,16 @@
             task: TaskConfig to run pipelines for
             project: ProjectConfig to run pipelines
         """
         # Set project to the project.
         if project:
             task.project = project
         # Run all pipelines in the pipeline.
+        if task.verbose:
+            logger.info("Running %s pipelines", len(task.pipelines or []))
         for pipeline in PIPELINEs.get_pipelines(task):
             if task.verbose:
                 logger.info("Running pipeline: %s", pipeline.model_dump())
             initial_object = task if pipeline.use_task_as_initial_object else None
             PIPELINEs.run_pipeline(pipeline, initial_object, task)
 
     @staticmethod
```

### Comparing `hyfi-1.0.0/src/hyfi/pipeline/configs.py` & `hyfi-1.0.1/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/project/__init__.py` & `hyfi-1.0.1/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/task/__init__.py` & `hyfi-1.0.1/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/task/batch.py` & `hyfi-1.0.1/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/contexts.py` & `hyfi-1.0.1/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/datasets.py` & `hyfi-1.0.1/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/envs.py` & `hyfi-1.0.1/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/funcs.py` & `hyfi-1.0.1/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/gpumon.py` & `hyfi-1.0.1/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/iolibs.py` & `hyfi-1.0.1/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/logging.py` & `hyfi-1.0.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/notebooks.py` & `hyfi-1.0.1/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/utils/packages.py` & `hyfi-1.0.1/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.0/src/hyfi/workflow/__init__.py` & `hyfi-1.0.1/src/hyfi/workflow/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     _config_group_: str = "workflow"
 
     project: Optional[ProjectConfig] = None
     tasks: Optional[List[Union[str, Dict]]] = []
 
     def get_tasks(self) -> Tasks:
         self.tasks = self.tasks or []
-        config = self.__dict__
+
         tasks: Tasks = [
-            TaskConfig(**config[name])
+            TaskConfig(**getattr(self, name))
             for name in self.tasks
-            if name in config and isinstance(config[name], dict)
+            if isinstance(name, str) and isinstance(getattr(self, name), dict)
         ]
         return tasks
```

### Comparing `hyfi-1.0.0/PKG-INFO` & `hyfi-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

