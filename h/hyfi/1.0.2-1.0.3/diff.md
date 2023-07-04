# Comparing `tmp/hyfi-1.0.2.tar.gz` & `tmp/hyfi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.0.2.tar", max compression
+gzip compressed data, was "hyfi-1.0.3.tar", max compression
```

## Comparing `hyfi-1.0.2.tar` & `hyfi-1.0.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1071 2023-07-04 06:55:39.646139 hyfi-1.0.2/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-04 06:55:39.646139 hyfi-1.0.2/README.md
--rw-r--r--   0        0        0     4862 2023-07-04 06:56:18.886321 hyfi-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4267 2023-07-04 06:55:39.650138 hyfi-1.0.2/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2550 2023-07-04 06:55:39.650138 hyfi-1.0.2/src/hyfi/__click__.py
--rw-r--r--   0        0        0      788 2023-07-04 06:55:39.650138 hyfi-1.0.2/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9245 2023-07-04 06:55:39.650138 hyfi-1.0.2/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-04 06:56:18.774320 hyfi-1.0.2/src/hyfi/_version.py
--rw-r--r--   0        0        0     1890 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7229 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    31944 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7331 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/composer/extended.py
--rw-r--r--   0        0        0        0 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-04 06:56:18.778320 hyfi-1.0.2/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      427 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      785 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      166 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      178 2023-07-04 06:55:39.654139 hyfi-1.0.2/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      351 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      395 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6548 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     5915 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4228 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    50188 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     7754 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0      782 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      434 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     4261 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8085 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5155 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/py.typed
--rw-r--r--   0        0        0     4268 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     6518 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30058 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6568 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     3769 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20157 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-04 06:55:39.658139 hyfi-1.0.2/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-04 06:55:39.662139 hyfi-1.0.2/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-04 06:55:39.662139 hyfi-1.0.2/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      753 2023-07-04 06:55:39.662139 hyfi-1.0.2/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 hyfi-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 19:41:41.468381 hyfi-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-04 19:41:41.468381 hyfi-1.0.3/README.md
+-rw-r--r--   0        0        0     4864 2023-07-04 19:42:07.112452 hyfi-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4267 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2550 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      788 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9245 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      733 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-04 19:42:07.036452 hyfi-1.0.3/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1890 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    32839 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7331 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/composer/extended.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-04 19:42:07.036452 hyfi-1.0.3/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      427 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      785 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-04 19:41:41.472380 hyfi-1.0.3/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      166 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      178 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      351 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      395 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6548 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5915 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4228 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    50188 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     7754 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0      782 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      434 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     4261 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8085 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5155 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     6577 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30058 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     3769 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-04 19:41:41.476381 hyfi-1.0.3/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.0.3/PKG-INFO
```

### Comparing `hyfi-1.0.2/LICENSE` & `hyfi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/README.md` & `hyfi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/pyproject.toml` & `hyfi-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.0.2"
+version = "1.0.3"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
@@ -13,15 +13,15 @@
 hyfi = 'hyfi.__cli__:hydra_main'
 hyfi-run = 'hyfi.__click__:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.12"
 hydra-core = "^1.3.2"
 hydra-colorlog = "^1.2.0"
-pydantic = "^2.0"
+pydantic = "^2.0.1"
 chardet = "<=5.1.0"
 pandas = ">=1.5.3,<=2.0.2"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
 numpy = "<=1.24.4"
 python-dotenv = "^1.0.0"
 requests = "^2.27.1"
```

### Comparing `hyfi-1.0.2/src/hyfi/__cli__.py` & `hyfi-1.0.3/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/__click__.py` & `hyfi-1.0.3/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/__global__/__init__.py` & `hyfi-1.0.3/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/__global__/config.py` & `hyfi-1.0.3/src/hyfi/__global__/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/__init__.py` & `hyfi-1.0.3/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/about/__init__.py` & `hyfi-1.0.3/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/batch/__init__.py` & `hyfi-1.0.3/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/__init__.py` & `hyfi-1.0.3/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.0.3/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/cache_file.py` & `hyfi-1.0.3/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/common.py` & `hyfi-1.0.3/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/file_lock.py` & `hyfi-1.0.3/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/meta.py` & `hyfi-1.0.3/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/progress.py` & `hyfi-1.0.3/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.0.3/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.0.3/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.0.3/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.0.3/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.0.3/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/testing.py` & `hyfi-1.0.3/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/cached_path/util.py` & `hyfi-1.0.3/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/composer/__init__.py` & `hyfi-1.0.3/src/hyfi/composer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -779,24 +779,26 @@
     _config_name_: str = "__init__"
     _config_group_: str = ""
     verbose: bool = False
 
     _init_args_: Dict[str, Any] = {}
     _exclude_: Set[str] = set()
     _property_set_methods_: Dict[str, str] = {}
+    _subconfigs_: Dict[str, Any] = {}
 
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         extra="allow",
         validate_assignment=False,
     )  # type: ignore
 
     def __init__(self, **config_kwargs):
         logger.debug("init %s with %s", self.__class__.__name__, config_kwargs)
         super().__init__(**config_kwargs)
+        self.initialize_subconfigs(config_kwargs)
 
     def __setattr__(self, key, val):
         """
         Overrides the default __setattr__ method to allow for custom property set methods.
 
         Args:
             key (str): The name of the attribute to set.
@@ -809,15 +811,15 @@
                 val if isinstance(val, (str, int)) else type(val),
             )
             getattr(self, method)(val)
         super().__setattr__(key, val)
 
     @model_validator(mode="before")
     def validate_model_config_before(cls, data):
-        logger.debug("validate_model_config_before: %s", data)
+        # logger.debug("Validating model config before validating each field.")
         _config_name_ = data.get("_config_name_", getattr(cls._config_name_, "default", "__init__"))  # type: ignore
         _config_group_ = data.get("_config_group_", getattr(cls._config_group_, "default"))  # type: ignore
         _class_name_ = cls.__name__  # type: ignore
         if not _config_group_:
             logger.debug("There is no config group specified.")
             return data
         # Initialize the config with the given config_name.
@@ -834,14 +836,33 @@
         return data
 
     # @model_validator(mode="after")  # type: ignore
     # def validate_model_config_after(cls, model):
     #     logger.debug("validate_model_config_after")
     #     return model
 
+    def initialize_subconfigs(self, config_kwargs):
+        """
+        Initializes subconfigs with the given config data.
+        The function updates the object's dictionary with the given config data,
+        after excluding any attributes specified in the object's `exclude` list.
+
+        Args:
+            **config_kwargs: The config data to update the object with.
+
+        Returns:
+            None
+        """
+        self._subconfigs_ = self._subconfigs_ or {}
+        for name, config in self._subconfigs_.items():
+            if name in config_kwargs and isinstance(config_kwargs[name], dict):
+                cfg = config_kwargs[name]
+                logger.debug("Initializing subconfig %s with %s", name, cfg)
+                setattr(self, name, config.model_validate(cfg))
+
     def export_config(
         self,
         exclude: Optional[Union[str, List[str], Set[str], None]] = None,
         exclude_none: bool = True,
         only_include: Optional[Union[str, List[str], Set[str], None]] = None,
     ) -> Dict[str, Any]:
         """
```

### Comparing `hyfi-1.0.2/src/hyfi/composer/extended.py` & `hyfi-1.0.3/src/hyfi/composer/extended.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.0.3/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.0.3/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.0.3/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.0.3/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.0.3/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.0.3/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/copier/__init__.py` & `hyfi-1.0.3/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/dotenv/__init__.py` & `hyfi-1.0.3/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/graphics/collage.py` & `hyfi-1.0.3/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/graphics/motion.py` & `hyfi-1.0.3/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/graphics/utils.py` & `hyfi-1.0.3/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/joblib/__init__.py` & `hyfi-1.0.3/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/joblib/batch/apply.py` & `hyfi-1.0.3/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.0.3/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.0.3/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/main/__init__.py` & `hyfi-1.0.3/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/path/__init__.py` & `hyfi-1.0.3/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/path/batch.py` & `hyfi-1.0.3/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/path/task.py` & `hyfi-1.0.3/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/pipe/__init__.py` & `hyfi-1.0.3/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/pipe/test.py` & `hyfi-1.0.3/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/pipeline/__init__.py` & `hyfi-1.0.3/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/pipeline/configs.py` & `hyfi-1.0.3/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/project/__init__.py` & `hyfi-1.0.3/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/task/__init__.py` & `hyfi-1.0.3/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/task/batch.py` & `hyfi-1.0.3/src/hyfi/task/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,23 @@
         _property_set_methods_ (Dict[str, str]): A dictionary of property set methods.
     """
 
     _config_name_: str = "__batch__"
     _config_group_: str = "task"
 
     batch_name: str = "demo"
-    batch: BatchConfig = None  # type: ignore
+    batch: Optional[BatchConfig] = None
 
     _property_set_methods_ = {
         "task_name": "set_task_name",
         "task_root": "set_task_root",
         "batch_name": "set_batch_name",
         "batch_num": "set_batch_num",
     }
+    _subconfigs_ = {"batch": BatchConfig}
 
     def set_batch_name(self, val):
         if not self.batch_name or self.batch_name != val:
             if self.path:
                 self.path.batch_name = val
             if self.batch:
                 self.batch.batch_name = val
@@ -183,15 +184,16 @@
                 cfg = XC.merge(cfg, batch_cfg)
             else:
                 logger.info("No config file found at %s", filepath)
         if self.verbose:
             logger.info("Updating config with config_kwargs: %s", config_kwargs)
         cfg = XC.update(XC.to_dict(cfg), config_kwargs)
 
-        # TODO: initialize self with the config
+        # initialize self with the config
+        self.__init__(**cfg)
 
         return self.model_dump()
 
     def print_config(
         self,
         batch_name: Optional[str] = None,
         batch_num: Optional[int] = None,
```

### Comparing `hyfi-1.0.2/src/hyfi/utils/contexts.py` & `hyfi-1.0.3/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/utils/datasets.py` & `hyfi-1.0.3/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/utils/envs.py` & `hyfi-1.0.3/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/utils/funcs.py` & `hyfi-1.0.3/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/utils/gpumon.py` & `hyfi-1.0.3/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/utils/iolibs.py` & `hyfi-1.0.3/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/utils/logging.py` & `hyfi-1.0.3/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/utils/notebooks.py` & `hyfi-1.0.3/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/utils/packages.py` & `hyfi-1.0.3/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/src/hyfi/workflow/__init__.py` & `hyfi-1.0.3/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.2/PKG-INFO` & `hyfi-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: joblib (<=1.3.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (<=1.24.4)
 Requires-Dist: pandas (>=1.5.3,<=2.0.2)
 Requires-Dist: pathspec (>=0.9.0)
 Requires-Dist: pyarrow (<=12.0.1)
-Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic (>=2.0.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=12.1,<14.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi
```

