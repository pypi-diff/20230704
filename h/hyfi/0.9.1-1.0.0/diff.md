# Comparing `tmp/hyfi-0.9.1.tar.gz` & `tmp/hyfi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.9.1.tar", max compression
+gzip compressed data, was "hyfi-1.0.0.tar", max compression
```

## Comparing `hyfi-0.9.1.tar` & `hyfi-1.0.0.tar`

### file list

```diff
@@ -1,83 +1,108 @@
--rw-r--r--   0        0        0     1071 2023-06-20 09:05:25.739669 hyfi-0.9.1/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-20 09:05:25.739669 hyfi-0.9.1/README.md
--rw-r--r--   0        0        0     4652 2023-06-20 09:05:56.174588 hyfi-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3810 2023-06-20 09:05:25.743669 hyfi-0.9.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2550 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/__click__.py
--rw-r--r--   0        0        0      653 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9835 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-20 09:05:56.090579 hyfi-0.9.1/src/hyfi/_version.py
--rw-r--r--   0        0        0      783 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     3353 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3449 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0        0 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-20 09:05:56.090579 hyfi-0.9.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      435 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      141 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0      320 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      559 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      948 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      396 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      806 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      153 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      195 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0     6414 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     3050 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8363 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     6627 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0    21012 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0     7598 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0     3526 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    16595 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0     2642 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/pipe.py
--rw-r--r--   0        0        0    39697 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      225 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     2379 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0      973 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     3782 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5351 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/py.typed
--rw-r--r--   0        0        0     4042 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     5140 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     1314 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    23179 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6358 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10731 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     3769 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    19766 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     4828 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 hyfi-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 01:01:20.590560 hyfi-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-04 01:01:20.590560 hyfi-1.0.0/README.md
+-rw-r--r--   0        0        0     4862 2023-07-04 01:01:49.699067 hyfi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4267 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2550 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      788 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9245 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      733 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-04 01:01:49.623065 hyfi-1.0.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1890 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    31944 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7331 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/composer/extended.py
+-rw-r--r--   0        0        0        0 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-04 01:01:49.623065 hyfi-1.0.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      427 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      785 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      166 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      237 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      242 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-04 01:01:20.594560 hyfi-1.0.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      178 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      351 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      381 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6548 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5911 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4474 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13831 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    50188 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     7754 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0      782 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      434 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     4261 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     7985 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5155 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     6518 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30058 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     3769 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      762 2023-07-04 01:01:20.598560 hyfi-1.0.0/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 hyfi-1.0.0/PKG-INFO
```

### Comparing `hyfi-0.9.1/LICENSE` & `hyfi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/README.md` & `hyfi-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 Hydra Fast Interface (Hydra and Pydantic based interface framework)
 
 - Documentation: [https://hyfi.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/hyfi][repo-url]
 - PyPI: [https://pypi.org/project/hyfi][pypi-url]
 
-HyFI is a framework for building interfaces for Python applications. It is based on [Hydra] and [Pydantic] and provides a set of tools to build interfaces for Python applications.
+HyFI is a framework for building interfaces for Python applications. It is based on [Hydra](https://hydra.cc) and [Pydantic](https://docs.pydantic.dev/latest/) and provides a set of tools to build interfaces for Python applications.
 
 ## Changelog
 
 See the [CHANGELOG] for more information.
 
 ## Contributing
```

### Comparing `hyfi-0.9.1/pyproject.toml` & `hyfi-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.9.1"
+version = "1.0.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
@@ -13,71 +13,89 @@
 hyfi = 'hyfi.__cli__:hydra_main'
 hyfi-run = 'hyfi.__click__:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.12"
 hydra-core = "^1.3.2"
 hydra-colorlog = "^1.2.0"
-pydantic = "^1.10.7"
+pydantic = "^2.0"
 chardet = "<=5.1.0"
 pandas = ">=1.5.3,<=2.0.2"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
-numpy = "<=1.24.3"
+numpy = "<=1.24.4"
 python-dotenv = "^1.0.0"
 requests = "^2.27.1"
 tqdm = "^4.64.1"
 colorama = "^0.4.3"
 pathspec = ">=0.9.0"
 filelock = ">=3.4,<=3.12.2"
 rich = ">=12.1,<14.0"
 gdown = "<=4.6.6"
 huggingface-hub = ">=0.8.1,<=0.15.1"
 # google-cloud-storage = ">=1.32.0,<3.0"
 # boto3 = ">=1.0,<2.0"
 click = "<=8.1.3"
 pyarrow = "<=12.0.1"
-datasets = "<=2.13.0"
+datasets = "<=2.13.1"
+joblib = "<=1.3.0"
+pydantic-settings = "^2.0.0"
 
 [tool.poetry.group.ipython]
 optional = true
 
 [tool.poetry.group.ipython.dependencies]
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
 ipython = "<=8.12.2"
 ipython-autotime = "^0.3.1"
 ipywidgets = "^8.0.6"
 
-[tool.poetry.extras]
-ipython = ["ipython", "ipython-autotime", "ipywidgets"]
+[tool.poetry.group.loky]
+optional = true
+
+[tool.poetry.group.loky.dependencies]
+loky = "^3.4.1"
+
+[tool.poetry.group.ray]
+optional = true
+
+[tool.poetry.group.ray.dependencies]
+ray = "^2.5.1"
 
-[tool.poetry.group.mkdocs]
+[tool.poetry.group.p_tqdm]
 optional = true
 
-[tool.poetry.group.mkdocs.dependencies]
-mkdocs-material = "^9.1.15"
-markdown-include = "^0.8.1"
-mkdocstrings = { extras = ["python"], version = "^0.22.0" }
-mkdocs-material-extensions = ">=1.1"
-pymdown-extensions = ">=9.9.1"
+[tool.poetry.group.p_tqdm.dependencies]
+p-tqdm = "^1.4.0"
+
+[tool.poetry.group.numba]
+optional = true
+
+[tool.poetry.group.numba.dependencies]
+numba = "^0.57.1"
+
+[tool.poetry.extras]
+ipython = ["ipython", "ipython-autotime", "ipywidgets"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 ipykernel = "^6.22.0"
+flaky = "^3.7.0"
+responses = "^0.23.1"
 
 [tool.poe]
 include = [".tasks.toml", ".tasks-extra.toml"]
 
 [tool.black]
 exclude = [
     '_version.py',
```

### Comparing `hyfi-0.9.1/src/hyfi/__cli__.py` & `hyfi-1.0.0/src/hyfi/__cli__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,32 +5,23 @@
 import hydra
 from omegaconf import DictConfig
 
 from hyfi.__global__ import __about__, __hydra_version_base__
 from hyfi.__global__.config import HyfiConfig
 from hyfi.copier import Copier
 from hyfi.main import HyFI, _about
-from hyfi.utils.logging import Logging
+from hyfi.utils.logging import LOGGING
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 __config_path__ = "conf"
 __config_name__ = "config"
 
 
-def cmd(**args):
-    """
-    Run the command defined in the config file
-    Args
-        args : dict Arguments to pass to HyFI.
-    """
-    HyFI.run(args)
-
-
 def about(**args):
     """
     Print the about information for Hyfi.
     This is a wrapper around _about which takes a HyfiConfig as an argument
     """
     cfg = HyfiConfig(**args)
     _about(cfg)
@@ -46,15 +37,34 @@
     cfg = HyFI.to_dict(args["copier"])
     print(type(cfg), cfg)
     with Copier(**cfg) as worker:
         worker.run_copy()
 
 
 def run_task(**args):
-    print(args["task"].keys())
+    """
+    Run a task. This is a wrapper around HyFI
+    """
+    # Check if task is not in args
+    if "task" not in args:
+        raise ValueError("No task configuration found")
+    project = HyFI.init_project(**args["project"]) if "project" in args else None
+    task = HyFI.task_config(**args["task"])
+    HyFI.run_task(task, project=project)
+
+
+def run_workflow(**args):
+    """
+    Run a workflow. This is a wrapper around HyFI. run_workflow
+    """
+    # Raised if no workflow configuration is specified.
+    if "workflow" not in args:
+        raise ValueError("No workflow configuration found")
+    workflow = HyFI.workflow_config(**args["workflow"])
+    HyFI.run_workflow(workflow)
 
 
 def cli_main(cfg: DictConfig) -> None:
     """
     Main function for the command line interface.
     Initializes Hydra and instantiates the class.
     Prints the configuration to standard out if verbose is set to True
@@ -66,25 +76,25 @@
         None if everything went fine otherwise an error is raised
         to indicate the reason for the failure
     """
     hyfi = HyfiConfig(**cfg)  # type: ignore
     verbose = hyfi.verbose
     app_name = hyfi.about.name
     print_config = hyfi.print_config
-    print_resolved_config = hyfi.print_resolved_config
+    resolve = hyfi.resolve
 
     # Print out the command line interface for the application.
     if verbose:
         print(f"## Command Line Interface for {app_name} ##")
-    HyFI.initialize(cfg)
+    HyFI.initialize()
 
     # Print the configuration to the console.
     if print_config:
         # Prints the configuration to the console.
-        if print_resolved_config:
+        if resolve:
             logger.info("## hydra configuration resolved ##")
             HyFI.pprint(cfg)
         else:
             logger.info("## hydra configuration ##")
             print(HyFI.to_yaml(cfg))
 
     # Prints out the working directory and original working directory.
```

### Comparing `hyfi-0.9.1/src/hyfi/__click__.py` & `hyfi-1.0.0/src/hyfi/__click__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import click
 
 from hyfi.__global__ import __hyfi_path__
 from hyfi.__global__.config import HyfiConfig
 from hyfi._version import __version__
 from hyfi.copier import Copier
 from hyfi.main import _about
-from hyfi.utils.logging import Logging
+from hyfi.utils.logging import LOGGING
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 @click.group()
 @click.version_option(__version__)
 def cli():
     pass
```

### Comparing `hyfi-0.9.1/src/hyfi/__global__/config.py` & `hyfi-1.0.0/src/hyfi/__global__/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """
 Hyfi configuration file.
 """
 import os
-from typing import Any, Dict, Optional, Union
+from typing import Any, Optional, Union
 
 from omegaconf import DictConfig
-from pydantic import BaseModel, root_validator, validator
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    FieldValidationInfo,
+    PrivateAttr,
+    field_validator,
+    model_validator,
+)
 
 from hyfi.__global__ import __about__, __hydra_config__
 from hyfi.about import AboutConfig
 from hyfi.dotenv import DotEnvConfig
-from hyfi.hydra import Composer
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
-from hyfi.utils.envs import Envs
-from hyfi.utils.logging import Logging
+from hyfi.utils.envs import ENVs
+from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 def __version__():
     """
     Returns the version of Hyfi. It is used to determine the version of Hyfi.
 
 
@@ -38,240 +44,217 @@
 
     hyfi_config_path: str = __about__.config_path
     hyfi_config_module: str = __about__.config_module
     hyfi_user_config_path: str = ""
 
     debug_mode: bool = False
     print_config: bool = False
-    print_resolved_config: bool = False
+    resolve: bool = False
     verbose: bool = False
     logging_level: str = "WARNING"
 
     hydra: Optional[DictConfig] = None
 
     about: AboutConfig = AboutConfig()
     copier: Optional[DictConfig] = None
     project: Optional[ProjectConfig] = None
     task: Optional[TaskConfig] = None
 
-    __version__: str = __version__()
-    __initilized__: bool = False
+    _version_: str = PrivateAttr(__version__())
+    _initilized_: bool = PrivateAttr(False)
 
-    class Config:
-        arbitrary_types_allowed = True
-        underscore_attrs_are_private = True
-        validate_assignment = True
-        extra = "allow"
+    model_config = ConfigDict(
+        arbitrary_types_allowed=True,
+        validate_assignment=True,
+        extra="allow",
+    )  # type: ignore
 
-    @root_validator()
-    def _check_and_set_osenvs(cls, values):
+    @model_validator(mode="before")
+    def _validate_model_data(cls, data):
         """
-        Validate and set values for the config file.
+        Validate and set the model data.
 
         Args:
-                cls: Class to use for config lookup
-                values: Dictionary of values to check and set
+            cls: Class to use for config lookup
+            data: Dictionary of values to check and set
 
         Returns:
-                Same dictionary with hyfi_config
+            Validated dictionary of values
         """
         key = "hyfi_config_path"
-        val = Envs.check_and_set_osenv(key, values.get(key))
-        values[key] = val
+        val = ENVs.check_and_set_osenv_var(key, data.get(key))
         # Set the hyfi_config_module value in the configuration file.
         if val is not None:
+            data[key] = val
             key = "hyfi_config_module"
-            values[key] = Envs.check_and_set_osenv(key, val.replace("pkg://", ""))
-        return values
+            data[key] = ENVs.check_and_set_osenv_var(key, val.replace("pkg://", ""))
+        key = "hyfi_user_config_path"
+        val = data.get(key)
+        if val is None:
+            data[key] = ENVs.get_osenv(key, ".")
+        return data
 
-    @validator("hyfi_user_config_path")
+    @field_validator("hyfi_user_config_path")
     def _validate_hyfi_user_config_path(cls, v):
         """
         Validate and set hyfi_user_config_path.
 
         Args:
                 cls: Class to use for validation.
                 v: Value to set if valid.
 
         Returns:
                 True if valid False otherwise
         """
-        return Envs.check_and_set_osenv("hyfi_user_config_path", v)
+        return ENVs.check_and_set_osenv_var("hyfi_user_config_path", v)
 
-    @validator("logging_level")
-    def _validate_logging_level(cls, v, values):
+    @field_validator("logging_level")
+    def _validate_logging_level(cls, v, info: FieldValidationInfo):
         """
         Validate and set the logging level
-
-        Args:
-                cls: The class to operate on
-                v: The value to set the logging level to
-                values: The values from the config file
-
-        Returns:
-                The value that was set
         """
-        verbose = values.get("verbose", False)
+        verbose = info.data.get("verbose", False)
         # Set verbose to INFO.
         if verbose and v == "WARNING":
             v = "INFO"
         logger.setLevel(v)
         return v
 
     def __init__(self, **config_kwargs: Any):
         """
         Initialize the object with data
 
         Args:
-                data: Data to initialize the
+            config_kwargs: Dictionary of values to initialize the object with
         """
         super().__init__(**config_kwargs)
-        # self.about = __about__
 
-    def init_workspace(
+    def init_project(
         self,
         project_name: str = "",
-        task_name: str = "",
         project_description: str = "",
         project_root: str = "",
         project_workspace_name: str = "",
         global_hyfi_root: str = "",
         global_workspace_name: str = "",
         num_workers: int = -1,
         log_level: str = "",
+        reinit: bool = True,
         autotime: bool = True,
         retina: bool = True,
         verbose: Union[bool, int] = False,
         **kwargs,
     ):
         """
         Initialize and start hyfi.
 
         Args:
                 project_name: Name of the project to use.
-                task_name: Name of the task to use.
                 project_description: Description of the project that will be used.
                 project_root: Root directory of the project.
                 project_workspace_name: Name of the project's workspace directory.
                 global_hyfi_root: Root directory of the global hyfi.
                 global_workspace_name: Name of the global hierachical workspace directory.
                 num_workers: Number of workers to run.
                 log_level: Log level for the log.
                 autotime: Whether to automatically set time and / or keep track of run times.
                 retina: Whether to use retina or not.
                 verbose: Enables or disables logging
         """
-        envs = DotEnvConfig(HYFI_VERBOSE=verbose)
+        envs = DotEnvConfig(HYFI_VERBOSE=verbose)  # type: ignore
         # Set the project name environment variable HYFI_PROJECT_NAME environment variable if project_name is not set.
         if project_name:
-            envs.HYFI_PROJECT_NAME = Envs.expand_posix_vars(project_name)
-        # Set the task name environment variable HYFI_TASK_NAME to the task name.
-        if task_name:
-            envs.HYFI_TASK_NAME = Envs.expand_posix_vars(task_name)
+            envs.HYFI_PROJECT_NAME = ENVs.expand_posix_vars(project_name)
         # Set the project description environment variable HYFI_PROJECT_DESC environment variable.
         if project_description:
-            envs.HYFI_PROJECT_DESC = Envs.expand_posix_vars(project_description)
+            envs.HYFI_PROJECT_DESC = ENVs.expand_posix_vars(project_description)
         # Set environment variables HYFI_PROJECT_ROOT to the project root if project_root is set to true.
         if project_root:
-            envs.HYFI_PROJECT_ROOT = Envs.expand_posix_vars(project_root)
+            envs.HYFI_PROJECT_ROOT = ENVs.expand_posix_vars(project_root)
         # Set the project workspace name environment variable HYFI_PROJECT_WORKSPACE_NAME environment variable if project_workspace_name is set to the project workspace name.
         if project_workspace_name:
-            envs.HYFI_PROJECT_WORKSPACE_NAME = Envs.expand_posix_vars(project_workspace_name)
+            envs.HYFI_PROJECT_WORKSPACE_NAME = ENVs.expand_posix_vars(
+                project_workspace_name
+            )
         # Expand the hyfi_root environment variable.
         if global_hyfi_root:
-            envs.HYFI_GLOBAL_ROOT = Envs.expand_posix_vars(global_hyfi_root)
+            envs.HYFI_GLOBAL_ROOT = ENVs.expand_posix_vars(global_hyfi_root)
         # Set the global workspace name environment variable HYFI_GLOBAL_WORKSPACE_NAME environment variable.
         if global_workspace_name:
-            envs.HYFI_GLOBAL_WORKSPACE_NAME = Envs.expand_posix_vars(global_workspace_name)
+            envs.HYFI_GLOBAL_WORKSPACE_NAME = ENVs.expand_posix_vars(
+                global_workspace_name
+            )
         # Set the number of workers to use.
         if num_workers:
             envs.HYFI_NUM_WORKERS = num_workers
         # Set the log level to the given log level.
         if log_level:
             envs.HYFI_LOG_LEVEL = log_level
-            Logging.setLogger(log_level)
+            LOGGING.setLogger(log_level)
             logger.setLevel(log_level)
         # Load the extentions for the autotime extension.
         if autotime:
             NBs.load_extentions(exts=["autotime"])
         # Set the retina matplotlib formats.
         if retina:
             NBs.set_matplotlib_formats("retina")
-        self.initialize()
 
-    def initialize(self, config: Union[DictConfig, Dict, None] = None):
+        self.initialize(force=reinit)
+        self.project = ProjectConfig()
+
+    def initialize(self, force: bool = False) -> None:
         """
         Initialize hyfi.
 
-        Args:
-                config: Configuration dictionary or None.
-
         Returns:
-                A boolean indicating whether initialization was successful
+            A boolean indicating whether initialization was successful
         """
-        """Initialize hyfi config"""
-        # Returns the current value of the __initilized__ attribute.
-        if self.__initilized__:
+        # Returns the current value of the _initilized_ attribute.
+        if self._initilized_ and not force:
             return
-        __hydra_config__.hyfi_config_module = self.hyfi_config_module
-        __hydra_config__.hyfi_config_path = self.hyfi_config_path
+        __hydra_config__.hyfi_config_module = __about__.config_module
+        __hydra_config__.hyfi_config_path = __about__.config_path
         __hydra_config__.hyfi_user_config_path = self.hyfi_user_config_path
+        logger.debug(
+            "HyFiConfig initialized with hyfi_config_module=%s, hyfi_config_path=%s, hyfi_user_config_path=%s",
+            __hydra_config__.hyfi_config_module,
+            __hydra_config__.hyfi_config_path,
+            __hydra_config__.hyfi_user_config_path,
+        )
 
-        # If config is not set the default config is used.
-        if config is None:
-            logger.debug("Using default config.")
-            config = Composer(
-                overrides=["+project=__init__"],
-                config_module=__about__.config_module,
-            ).config_as_dict
-
-        # Skip project config initialization.
-        if "project" not in config:
-            logger.debug("No project config found, skip project config initialization.")
-            return
-        self.project = ProjectConfig(**config["project"])
-        # self.project.init_project()
-        # Initialize joblib backend if joblib is not set.
-        if self.project.joblib:
-            self.project.joblib.init_backend()
-
-        self.__initilized__ = True
+        self._initilized_ = True
 
-    def terminate(self):
+    def terminate(self) -> None:
         """
         Terminate hyfi config by stopping joblib
 
-
         Returns:
-                True if successful False
+            True if successful False
         """
-        """Terminate hyfi config"""
         # If the module is not initialized yet.
-        if not self.__initilized__:
+        if not self._initilized_:
             return
         # Stop the backend if the joblib is running.
         if self.project and self.project.joblib:
             self.project.joblib.stop_backend()
-        self.__initilized__ = False
+        self._initilized_ = False
 
     def __repr__(self):
         """
         Returns a string representation of HyFIConfig.
 
-
         Returns:
                 The string representation of HyFI
         """
         return f"HyFIConfig(project={self.project})"
 
     def __str__(self):
         """
         Returns a string representation of the object.
 
-
         Returns:
                 The string representation of the
         """
         return self.__repr__()
 
     @property
     def app_version(self):
@@ -282,19 +265,21 @@
         Returns:
                 The version of the application
         """
         return self.about.version
 
     @property
     def dotenv(self):
-        return DotEnvConfig()
+        return DotEnvConfig()  # type: ignore
 
     @property
     def osenv(self):
         return os.environ
 
 
 __global_config__ = HyfiConfig()
+__global_config__.about.version = __version__()
 
 
 def __search_package_path__():
+    """Global HyFI config path for the package to search for."""
     return __global_config__.hyfi_config_path
```

### Comparing `hyfi-0.9.1/src/hyfi/__init__.py` & `hyfi-1.0.0/src/hyfi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from hyfi.__cli__ import hydra_main
 from hyfi.__global__ import __about__ as about
 from hyfi.__global__ import __hydra_version_base__
 from hyfi.__global__.config import __global_config__ as global_config
 from hyfi.main import HyFI
 from hyfi.main import HyFI as H
 from hyfi.main import HyFI as HI
-from hyfi.utils.logging import Logging
+from hyfi.utils.logging import LOGGING
```

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/__init__.py` & `hyfi-1.0.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.0.0/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/cache_file.py` & `hyfi-1.0.0/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/common.py` & `hyfi-1.0.0/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/file_lock.py` & `hyfi-1.0.0/src/hyfi/cached_path/file_lock.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             # for in particular are permission errors, such as:
             #  - errno 1  - EPERM  - "Operation not permitted"
             #  - errno 13 - EACCES - "Permission denied"
             #  - errno 30 - EROFS  - "Read-only file system"
             if err.errno not in (1, 13, 30):
                 raise
 
-            if os.path.isfile(self._lock_file) and self._read_only_ok:
+            if os.path.isfile(self.lock_file) and self._read_only_ok:
                 warnings.warn(
-                    f"Lacking permissions required to obtain lock '{self._lock_file}'. "
+                    f"Lacking permissions required to obtain lock '{self.lock_file}'. "
                     "Race conditions are possible if other processes are writing to the same resource.",
                     UserWarning,
                 )
             else:
                 raise
```

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/meta.py` & `hyfi-1.0.0/src/hyfi/cached_path/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     @classmethod
     def new(
         cls,
         resource: PathOrStr,
         cached_path: PathOrStr,
         *,
         etag: Optional[str] = None,
-        extraction_dir: bool = False
+        extraction_dir: bool = False,
     ) -> "Meta":
         return cls(
             resource=str(resource),
             cached_path=str(cached_path),
             creation_time=time.time(),
             size=cls.get_resource_size(cached_path),
             etag=etag,
@@ -84,15 +84,15 @@
                 data["creation_time"] = os.path.getmtime(path[:-5])
             if "extraction_dir" not in data and path.endswith("-extracted.json"):
                 data["extraction_dir"] = True
             if "cached_path" not in data:
                 data["cached_path"] = path[:-5]
             if "size" not in data:
                 data["size"] = cls.get_resource_size(data["cached_path"])
-        return cls(**config_kwargs)
+        return cls(**data)
 
     @staticmethod
     def get_resource_size(path: PathOrStr) -> int:
         """
         Get the size of a file or directory.
         """
         if os.path.isfile(path):
```

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/progress.py` & `hyfi-1.0.0/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.0.0/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.0.0/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.0.0/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.0.0/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.0.0/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/testing.py` & `hyfi-1.0.0/src/hyfi/cached_path/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 
 class BaseTestClass:
     """
     A custom testing class that disables some of the more verbose
     logging and that creates and destroys a temp directory as a test fixture.
     """
 
-    PROJECT_ROOT = (Path(__file__).parent / "..").resolve()
-    MODULE_ROOT = PROJECT_ROOT / "cached_path"
-    TOOLS_ROOT = MODULE_ROOT / "tools"
+    PROJECT_ROOT = (Path(__file__).parent / "../../../").resolve()
+    MODULE_ROOT = PROJECT_ROOT / "src/hyfi/cached_path"
     TESTS_ROOT = PROJECT_ROOT / "tests"
-    FIXTURES_ROOT = PROJECT_ROOT / "test_fixtures"
+    FIXTURES_ROOT = PROJECT_ROOT / "tests/fixtures"
 
     def setup_method(self):
         logging.basicConfig(
             format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
             level=logging.DEBUG,
         )
         # Disabling some of the more verbose logging statements that typically aren't very helpful
```

### Comparing `hyfi-0.9.1/src/hyfi/cached_path/util.py` & `hyfi-1.0.0/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.0.0/src/hyfi/conf/copier/conf.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Source path where to find the template.
 src_path: conf
 # Destination path where to render the template.
-dst_path: tmp/conf
+dst_path: workspace/tmp/conf
 # Filetypes to copy.
 filetypes:
   - yaml
   - yml
   - py
 # User-chosen additional file exclusion patterns.
 exclude:
```

### Comparing `hyfi-0.9.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.0.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 DOTENV_DIR: ${oc.select:..path.runtime,.}
 DOTENV_PATH: ${.DOTENV_DIR}/${.DOTENV_FILENAME}
 # Internal
 HYFI_RESOURCE_DIR:
 HYFI_GLOBAL_ROOT:
 HYFI_GLOBAL_WORKSPACE_NAME:
 HYFI_PROJECT_NAME:
-HYFI_TASK_NAME:
 HYFI_PROJECT_DESC:
 HYFI_PROJECT_ROOT:
 HYFI_PROJECT_WORKSPACE_NAME:
 HYFI_LOG_LEVEL: WARNING
 HYFI_VERBOSE: false
 HYFI_NUM_WORKERS:
 CACHED_PATH_CACHE_ROOT:
```

### Comparing `hyfi-0.9.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.0.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.0.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @package _global_
 debug_mode: false
 print_config: false
-print_resolved_config: true
+resolve: true
 verbose: false
 ignore_warnings: true
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
 hydra_log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}/hydra
 
 hydra:
   job:
@@ -20,8 +20,8 @@
   job_logging:
     handlers:
       console:
         level: ${hydra.job_logging.root.level}
       file:
         level: ${hydra.job_logging.root.level}
     root:
-      level: ${oc.env:HYFI_LOG_LEVEL,INFO}
+      level: ${logging_level}
```

### Comparing `hyfi-0.9.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.0.0/src/hyfi/conf/project/__init__.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
+_config_name_: __init__
 project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
-task_name: ${oc.select:..task_name,${alt:${oc.env:HYFI_TASK_NAME,null},default-task}}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
 project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
 project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
 global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
 global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
 num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
 use_huggingface_hub: false
```

### Comparing `hyfi-0.9.1/src/hyfi/copier/__init__.py` & `hyfi-1.0.0/src/hyfi/copier/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 """
 
 import filecmp
 import os
 from dataclasses import field
 from pathlib import Path
 from shutil import copy2, rmtree
-from typing import List
+from typing import List, Optional, Union
 
 from pathspec import PathSpec
 from pydantic.dataclasses import dataclass
 
-from hyfi.utils.envs import Envs
-from hyfi.utils.funcs import Funcs, Style
+from hyfi.utils.envs import ENVs
+from hyfi.utils.funcs import FUNCs, Style
 
 
 @dataclass()
 class Copier:
     """Copier process state manager.
 
     This class represents the state of a copier work and contains methods to
@@ -73,16 +73,16 @@
 
         verbose:
             When `True`, show all output.
     """
 
     src_path: Path = field(default=Path("conf"))
     dst_path: Path = field(default=Path("."))
-    filetypes: List = field(default_factory=list)
-    exclude: List = field(default_factory=list)
+    filetypes: Optional[Union[List, str]] = field(default=None)
+    exclude: Optional[Union[List, str]] = field(default=None)
     skip_if_exists: bool = False
     cleanup_on_error: bool = True
     overwrite: bool = False
     dry_run: bool = False
     verbose: bool = True
 
     def __post_init__(self):
@@ -100,41 +100,43 @@
                 setattr(self, attr_name, [])
             elif not isinstance(attr_value, list):
                 setattr(self, attr_name, [attr_value])
 
         if self.filetypes is None or len(self.filetypes) == 0:
             self.filetypes = ["yaml", "yml", "py"]
 
+        if self.exclude is None or len(self.exclude) == 0:
+            self.exclude = []
         if not self.dst_path.is_absolute():
-            self.dst_path = Envs.getcwd() / self.dst_path
+            self.dst_path = ENVs.getcwd() / self.dst_path
         self.path_spec = PathSpec.from_lines("gitwildmatch", self.exclude)
         self.dst_path_existed = self.dst_path.exists()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Exit the context manager, handling cleanup if needed."""
         if exc_type is not None and not self.dst_path_existed and self.cleanup_on_error:
             rmtree(self.dst_path)
-            Funcs.printf(
+            FUNCs.printf(
                 "CLEANUP",
                 f"Removed {self.dst_path}",
                 Style.DANGER,
                 verbose=self.verbose,
             )
 
     def run_copy(self):
         """Execute the copy process.
 
         Walk through the source directory, compare YAML files with the destination
         directory, and copy files based on the specified settings.
         """
         if not Path(self.src_path).is_dir():
-            Funcs.printf(
+            FUNCs.printf(
                 "ERROR",
                 f"Source path {self.src_path} does not exist.",
                 style=Style.DANGER,
             )
             return
         for root, _, files in os.walk(self.src_path):
             for filename in files:
@@ -142,52 +144,52 @@
                     continue
 
                 src_file = Path(root, filename)
                 dst_file = self.dst_path / src_file.relative_to(self.src_path)
                 dst_file = dst_file.absolute()
 
                 if self.path_spec.match_file(src_file):
-                    Funcs.printf(
+                    FUNCs.printf(
                         "EXCLUDED", f"{src_file}", Style.WARNING, verbose=self.verbose
                     )
                     continue
 
                 if dst_file.exists():
                     if self.skip_if_exists:
-                        Funcs.printf(
+                        FUNCs.printf(
                             "SKIPPED",
                             f"{src_file}",
                             Style.WARNING,
                             verbose=self.verbose,
                         )
                         continue
 
                     if filecmp.cmp(src_file, dst_file, shallow=False):
-                        Funcs.printf(
+                        FUNCs.printf(
                             "UNCHANGED",
                             f"{src_file}",
                             Style.IGNORE,
                             verbose=self.verbose,
                         )
                         continue
 
                     answer = "Y"
                     if not self.overwrite:
                         answer = input(f"Overwrite {dst_file}? [Y/n]: ") or "Y"
                     if answer.lower() != "y":
-                        Funcs.printf(
+                        FUNCs.printf(
                             "IGNORED",
                             f"{src_file}",
                             Style.WARNING,
                             verbose=self.verbose,
                         )
                         continue
 
                 if not self.dry_run:
                     dst_file.parent.mkdir(parents=True, exist_ok=True)
                     copy2(src_file, dst_file)
-                Funcs.printf(
+                FUNCs.printf(
                     "COPIED",
                     f"{src_file} -> {dst_file}",
                     Style.OK,
                     verbose=self.verbose,
                 )
```

### Comparing `hyfi-0.9.1/src/hyfi/graphics/collage.py` & `hyfi-1.0.0/src/hyfi/graphics/collage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """Collage of images.""" ""
 import io
 import logging
 import os
 import textwrap
-from typing import List
+from typing import List, Optional, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image, ImageDraw
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from hyfi.graphics.utils import get_image_font, load_image, load_images, scale_image
 
 log = logging.getLogger(__name__)
 
 
 class Collage(BaseModel):
     """Collage of images."""
 
     image: Image.Image
     width: int
     height: int
     ncols: int
     nrows: int
-    filepath: str = None
+    filepath: Optional[str] = None
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 def collage(
     images_or_uris,
     collage_filepath=None,
     ncols=3,
     max_images=12,
@@ -40,15 +39,15 @@
     crop_to_min_size=False,
     show_filename=False,
     filename_offset=(5, 5),
     fontname=None,
     fontsize=12,
     fontcolor="#000",
     **kwargs,
-) -> Collage:
+) -> Optional[Collage]:
     """
     Create a collage of images.
     """
 
     if not isinstance(images_or_uris, list):
         images_or_uris = [images_or_uris]
     images_or_uris = [
@@ -95,15 +94,14 @@
             image,
             show_filename=show_filename,
             filename=filename,
             filename_offset=filename_offset,
             fontname=fontname,
             fontsize=fontsize,
             fontcolor=fontcolor,
-            return_as_array=False,
         )
         for image, filename in zip(images, filenames)
     ]
 
     collage = grid_of_images(images, ncols, padding, bg_color=bg_color)
     if collage_filepath is not None:
         collage_filepath = str(collage_filepath)
@@ -126,23 +124,23 @@
     xlabel_fontsize=12,
     ylabel_fontsize=12,
     dpi=100,
     fg_fontcolor="white",
     bg_color="black",
     caption=None,
     **kwargs,
-) -> str:
+) -> Collage:
     """
     Create a collage of images.
     """
     figsize = (collage.width / dpi, collage.height / dpi)
     ncols, nrows = collage.ncols, collage.nrows
 
     fig = plt.figure(figsize=figsize, dpi=dpi)
-    fig.patch.set_facecolor(bg_color)
+    fig.patch.set_facecolor(bg_color)  # type: ignore
     plt.imshow(np.array(collage.image))
     ax = plt.gca()
     plt.grid(False)
     if xlabel is None and ylabel is None:
         plt.axis("off")
     if title is not None:
         title = "\n".join(
@@ -246,40 +244,38 @@
     fig.savefig(buf, format="png", dpi=dpi, bbox_inches="tight", pad_inches=0)
     buf.seek(0)
     return Image.open(buf)
 
 
 def convert_image(
     image_or_uri,
-    show_filename=False,
-    filename=None,
-    filename_offset=(5, 5),
-    fontname=None,
-    fontsize=12,
-    fontcolor=None,
-    return_as_array=False,
-):
+    show_filename: bool = False,
+    filename: Optional[str] = None,
+    filename_offset: Tuple[float, float] = (5, 5),
+    fontname: Optional[str] = None,
+    fontsize: int = 12,
+    fontcolor: Optional[str] = None,
+) -> Image.Image:
     """
     Convert an image to a PIL Image.
     """
     img = load_image(image_or_uri)
     if isinstance(image_or_uri, str) and filename is None:
         filename = os.path.basename(image_or_uri)
     if show_filename and filename is not None:
         font = get_image_font(fontname, fontsize)
         draw = ImageDraw.Draw(img)
         draw.text(filename_offset, filename, font=font, fill=fontcolor)
 
     # img = img.convert("RGB")
-    if return_as_array:
-        img = np.array(img)
+    # img = np.array(img)
     return img
 
 
-def gallery(array, ncols=7):
+def gallery(array: np.ndarray, ncols: int = 7):
     """
     Create a gallery of images from a numpy array.
     """
     nindex, height, width, intensity = array.shape
     nrows = nindex // ncols
     assert nindex == nrows * ncols
     return (
```

### Comparing `hyfi-0.9.1/src/hyfi/graphics/motion.py` & `hyfi-1.0.0/src/hyfi/graphics/motion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Motion image processing functions."""
 import os
 import subprocess
 from pathlib import Path
 
 from hyfi.graphics.utils import load_images
-from hyfi.utils.iolibs import IOLibs
-from hyfi.utils.logging import Logging
+from hyfi.utils.iolibs import IOLIBs
+from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 def make_gif(
     image_filepaths=None,
     filename_patterns: str = "",
     base_dir: str = "",
     output_filepath: str = "",
@@ -31,15 +31,15 @@
     logger.info("Making GIF from %s", filename_patterns)
     if os.path.exists(output_filepath) and not force:
         logger.info("Skipping GIF creation, already exists: %s", output_filepath)
         logger.info("If you want to re-create the GIF, set force=True")
     else:
         if image_filepaths is None:
             image_filepaths = sorted(
-                IOLibs.get_filepaths(filename_patterns, base_dir=base_dir)
+                IOLIBs.get_filepaths(filename_patterns, base_dir=base_dir)
             )
         if not image_filepaths:
             logger.warning("no images found")
             return
         if frames := load_images(image_filepaths):
             frame_one = frames[0]
             frame_one.save(
```

### Comparing `hyfi-0.9.1/src/hyfi/graphics/utils.py` & `hyfi-1.0.0/src/hyfi/graphics/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 """Image utils."""
 import io
 import os
 import platform
 from pathlib import Path
-from typing import List
+from typing import List, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import font_manager, rc
 from PIL import Image, ImageFont
 
-from hyfi.utils.iolibs import IOLibs
-from hyfi.utils.logging import Logging
+from hyfi.utils.iolibs import IOLIBs
+from hyfi.utils.logging import LOGGING
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 def scale_image(
     image: Image.Image,
-    max_width: int = 0,
-    max_height: int = 0,
-    max_pixels: int = 0,
-    scale: float = 1.0,
-    resize_to_multiple_of: int = 8,
+    max_width: Optional[int] = 0,
+    max_height: Optional[int] = 0,
+    max_pixels: Optional[int] = 0,
+    scale: Optional[float] = 1.0,
+    resize_to_multiple_of: Optional[int] = 0,
     resample: int = Image.LANCZOS,
 ) -> Image.Image:
     """Scale image to have at most `max_pixels` pixels."""
     if resize_to_multiple_of is None:
         resize_to_multiple_of = 0
 
     w, h = image.size
 
+    max_width = max_width or 0
+    max_height = max_height or 0
+    max_pixels = max_pixels or 0
     if max_width <= 0 and max_height > 0:
         max_width = int(w * max_height / h)
     elif max_height <= 0 and max_width > 0:
         max_height = int(h * max_width / w)
 
     if max_width > 0 and max_height > 0:
         max_pixels = max_width * max_height
-    if max_pixels > 0:
-        scale = np.sqrt(max_pixels / (w * h))
 
+    scale = np.sqrt(max_pixels / (w * h)) if max_pixels > 0 else scale or 1.0
     max_width = int(w * scale)
     max_height = int(h * scale)
     if resize_to_multiple_of > 0:
         max_width = (max_width // resize_to_multiple_of) * resize_to_multiple_of
         max_height = (max_height // resize_to_multiple_of) * resize_to_multiple_of
 
     if scale < 1.0 or w > max_width or h > max_height:
         image = image.resize((max_width, max_height), resample=resample)  # type: ignore
     return image
 
 
 def load_image(
-    image_or_uri,
-    max_width: int = 0,
-    max_height: int = 0,
-    max_pixels: int = 0,
-    scale: float = 1.0,
-    resize_to_multiple_of: int = 0,
+    image_or_uri: Union[str, Image.Image],
+    max_width: Optional[int] = 0,
+    max_height: Optional[int] = 0,
+    max_pixels: Optional[int] = 0,
+    scale: Optional[float] = 1.0,
+    resize_to_multiple_of: Optional[int] = 0,
     crop_box=None,
     mode="RGB",
     **kwargs,
 ) -> Image.Image:
     """Load image from file or URI."""
     from PIL import Image
 
@@ -73,35 +75,35 @@
     if max_pixels is None:
         max_pixels = 0
     if isinstance(image_or_uri, Image.Image):
         img = image_or_uri.convert(mode)
     elif Path(image_or_uri).is_file():
         img = Image.open(image_or_uri).convert(mode)
     else:
-        img = Image.open(io.BytesIO(IOLibs.read(image_or_uri, **kwargs))).convert(mode)
+        img = Image.open(io.BytesIO(IOLIBs.read(image_or_uri, **kwargs))).convert(mode)
     img = scale_image(
         img,
         max_width=max_width,
         max_height=max_height,
         max_pixels=max_pixels,
         scale=scale,
         resize_to_multiple_of=resize_to_multiple_of,
     )
     if crop_box is not None:
         img = img.crop(crop_box)
     return img
 
 
 def load_images(
-    images_or_uris: List[str],
-    max_width: int = 0,
-    max_height: int = 0,
-    max_pixels: int = 0,
-    scale: float = 1.0,
-    resize_to_multiple_of: int = 0,
+    images_or_uris: List[Union[str, Image.Image]],
+    max_width: Optional[int] = 0,
+    max_height: Optional[int] = 0,
+    max_pixels: Optional[int] = 0,
+    scale: Optional[float] = 1.0,
+    resize_to_multiple_of: Optional[int] = 0,
     crop_to_min_size: bool = False,
     mode: str = "RGB",
     **kwargs,
 ) -> List[Image.Image]:
     """Load images from files or URIs."""
     imgs = [
         load_image(
@@ -123,23 +125,27 @@
             min_width = (min_width // resize_to_multiple_of) * resize_to_multiple_of
             min_height = (min_height // resize_to_multiple_of) * resize_to_multiple_of
         imgs = [img.crop((0, 0, min_width, min_height)) for img in imgs]
 
     return imgs
 
 
-def get_image_font(fontname: str = "", fontsize: int = 12, lang: str = "en"):
+def get_image_font(
+    fontname: Optional[str] = None,
+    fontsize: int = 12,
+    lang: str = "en",
+):
     """Get font for PIL image."""
     fontname, fontpath = get_plot_font(set_font_for_matplot=False, fontname=fontname)
     return ImageFont.truetype(fontpath, fontsize) if fontpath else None
 
 
 def get_default_system_font(
-    fontname: str = "",
-    fontpath: str = "",
+    fontname: Optional[str] = None,
+    fontpath: Optional[str] = None,
     lang: str = "ko",
     verbose: bool = False,
 ):
     if platform.system() == "Darwin":
         default_fontname = "AppleGothic.ttf" if lang == "ko" else "Arial.ttf"
         fontname = fontname or default_fontname
         fontpath = os.path.join("/System/Library/Fonts/Supplemental/", fontname)
@@ -160,16 +166,16 @@
     if verbose:
         logger.info(f"Font path: {fontpath}")
     return fontname, fontpath
 
 
 def get_plot_font(
     set_font_for_matplot: bool = True,
-    fontpath: str = "",
-    fontname: str = "",
+    fontpath: Optional[str] = None,
+    fontname: Optional[str] = None,
     lang: str = "en",
     verbose: bool = False,
 ):
     """Get font for plot"""
     if fontname and not fontname.endswith(".ttf"):
         fontname += ".ttf"
     if not fontpath:
```

### Comparing `hyfi-0.9.1/src/hyfi/hydra/main.py` & `hyfi-1.0.0/src/hyfi/composer/extended.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,76 @@
-import importlib
-import inspect
 import os
 import random
-from typing import Any, Union
+from typing import Any, Callable, Dict, Union
 
 import hydra
 from omegaconf import OmegaConf
 
 from hyfi.__global__ import __home_path__, __hyfi_path__
 from hyfi.__global__.config import __global_config__, __search_package_path__
 from hyfi.cached_path import cached_path
-from hyfi.hydra import Composer, SpecialKeys
-from hyfi.utils.envs import Envs
-from hyfi.utils.funcs import Funcs
-from hyfi.utils.iolibs import IOLibs
-from hyfi.utils.logging import Logging
+from hyfi.composer import Composer, SpecialKeys
+from hyfi.utils.envs import ENVs
+from hyfi.utils.funcs import FUNCs
+from hyfi.utils.iolibs import IOLIBs
+from hyfi.utils.logging import LOGGING
+from hyfi.utils.packages import PKGs
 
-logger = Logging.getLogger(__name__)
-
-
-# _config_ = XC.config.copy()
+logger = LOGGING.getLogger(__name__)
 
 
 class XC(Composer):
     """
     Extended Composer class
     """
 
     @staticmethod
     def partial(
-        config: Any = None,
-        config_group: Union[str, None] = None,
+        config: Union[str, Dict],
         *args: Any,
         **kwargs: Any,
-    ) -> Any:
-        if config is None and config_group is None:
-            logger.warning("No config specified")
-            return None
-        elif config_group is not None:
-            config = XC._compose(config_group=config_group)
-        kwargs[SpecialKeys.PARTIAL] = True
+    ) -> Callable:
+        """
+        Returns a callable object that is a partial version of the function or class specified in the config object.
+
+        Args:
+            config: An config object describing what to call and what params to use.
+                    In addition to the parameters, the config must contain:
+                    _target_ : target class or callable name (str)
+                    And may contain:
+                    _partial_: If True, return functools.partial wrapped method or object
+                                False by default. Configure per target.
+            args: Optional positional parameters pass-through
+            kwargs: Optional named parameters to override
+                    parameters in the config object. Parameters not present
+                    in the config objects are being passed as is to the target.
+                    IMPORTANT: dataclasses instances in kwargs are interpreted as config
+                                and cannot be used as passthrough
+        Returns:
+            A callable object that is a partial version of the function or class specified in the config object.
+        """
+        if isinstance(config, str):
+            config = {SpecialKeys.TARGET.value: config}
+        else:
+            config = XC.to_dict(config)
+        if not isinstance(config, dict):
+            raise ValueError("config must be a dict or a str")
+        config[SpecialKeys.PARTIAL.value] = True
+        rc_kwargs_ = config.pop(SpecialKeys.KWARGS, {})
+        if rc_kwargs_ and kwargs:
+            kwargs.update(rc_kwargs_)
         return XC.instantiate(config, *args, **kwargs)
 
     @staticmethod
     def instantiate(config: Any, *args: Any, **kwargs: Any) -> Any:
         """
-        :param config: An config object describing what to call and what params to use.
+        Instantiates an object using the provided config object.
+
+        Args:
+            config: An config object describing what to call and what params to use.
                     In addition to the parameters, the config must contain:
                     _target_ : target class or callable name (str)
                     And may contain:
                     _args_: List-like of positional arguments to pass to the target
                     _recursive_: Construct nested objects as well (bool).
                                     False by default.
                                     may be overridden via a _recursive_ key in
@@ -59,122 +80,89 @@
                             partial : Passed objects are converted to dict and list, with
                                     the exception of Structured Configs (and their fields).
                             all     : Passed objects are dicts, lists and primitives without
                                     a trace of OmegaConf containers
                     _partial_: If True, return functools.partial wrapped method or object
                                 False by default. Configure per target.
                     _args_: List-like of positional arguments
-        :param args: Optional positional parameters pass-through
-        :param kwargs: Optional named parameters to override
+            args: Optional positional parameters pass-through
+            kwargs: Optional named parameters to override
                     parameters in the config object. Parameters not present
                     in the config objects are being passed as is to the target.
                     IMPORTANT: dataclasses instances in kwargs are interpreted as config
                                 and cannot be used as passthrough
-        :return: if _target_ is a class name: the instantiated object
-                if _target_ is a callable: the return value of the call
+
+        Returns:
+            if _target_ is a class name: the instantiated object
+            if _target_ is a callable: the return value of the call
         """
-        verbose = config.get(SpecialKeys.VERBOSE, False)
-        if not __global_config__.__initilized__:
+        verbose = config.get("verbose", False)
+        if not __global_config__._initilized_:
             __global_config__.initialize()
         if not XC.is_instantiatable(config):
             if verbose:
                 logger.info("Config is not instantiatable, returning config")
             return config
         _recursive_ = config.get(SpecialKeys.RECURSIVE, False)
         if SpecialKeys.RECURSIVE not in kwargs:
             kwargs[SpecialKeys.RECURSIVE.value] = _recursive_
         if verbose:
             logger.info("instantiating %s ...", config.get(SpecialKeys.TARGET))
         return hydra.utils.instantiate(config, *args, **kwargs)
 
     @staticmethod
-    def run(config: Any, **kwargs: Any) -> Any:
-        config = XC.merge(config, kwargs)
-        _config_ = config.get(SpecialKeys.CONFIG)
-        if _config_ is None:
-            logger.warning("No _config_ specified in config")
-            return None
-        if isinstance(_config_, str):
-            _config_ = [_config_]
-        for _cfg_ in _config_:
-            cfg = XC.select(config, _cfg_)
-            XC.instantiate(cfg)
+    def getsource(obj: Any) -> str:
+        """
+        Return the source code of the object.
 
-    @staticmethod
-    def function(cfg: Any, _name_, return_function=False, **parms):
-        cfg = XC.to_dict(cfg)
-        if not isinstance(cfg, dict):
-            logger.info("No function defined to execute")
-            return None
-
-        if SpecialKeys.FUNC not in cfg:
-            logger.info("No function defined to execute")
-            return None
-
-        _functions_ = cfg[SpecialKeys.FUNC]
-        fn = XC.partial(_functions_[_name_])
-        if _name_ in cfg:
-            _parms = cfg[_name_]
-            _parms = {**_parms, **parms}
-        else:
-            _parms = parms
-        _exec_ = _parms.pop(SpecialKeys.EXEC) if SpecialKeys.EXEC in _parms else True
-        if _exec_:
-            if callable(fn):
-                if return_function:
-                    logger.info(f"Returning function {fn}")
-                    return fn
-                logger.info(f"Executing function {fn} with parms {_parms}")
-                return fn(**_parms)
-            else:
-                logger.info(f"Function {_name_} not callable")
-                return None
-        else:
-            logger.info(f"Skipping execute of {fn}")
-            return None
+        Args:
+            obj: The object to get the source code of.
 
-    @staticmethod
-    def getsource(obj):
-        """Return the source code of the object."""
+        Returns:
+            The source code of the object as a string.
+
+        """
         try:
+            target_string = ""
             if XC.is_config(obj):
                 if SpecialKeys.TARGET in obj:
                     target_string = obj[SpecialKeys.TARGET]
-                    mod_name, object_name = target_string.rsplit(".", 1)
-                    mod = importlib.import_module(mod_name)
-                    obj = getattr(mod, object_name)
             elif isinstance(obj, str):
-                mod_name, object_name = obj.rsplit(".", 1)
-                mod = importlib.import_module(mod_name)
-                obj = getattr(mod, object_name)
-            return inspect.getsource(obj)
+                target_string = obj
+            return PKGs.getsource(target_string) if target_string else ""
         except Exception as e:
             logger.error(f"Error getting source: {e}")
             return ""
 
     @staticmethod
-    def viewsource(obj):
-        """Print the source code of the object."""
+    def viewsource(obj: Any):
+        """
+        Print the source code of the object.
+
+        Args:
+            obj: The object to print the source code of.
+
+        """
         print(XC.getsource(obj))
 
 
 OmegaConf.register_new_resolver("__hyfi_path__", __hyfi_path__)
 OmegaConf.register_new_resolver("__search_package_path__", __search_package_path__)
 OmegaConf.register_new_resolver("__home_path__", __home_path__)
-OmegaConf.register_new_resolver("today", Funcs.today)
-OmegaConf.register_new_resolver("to_datetime", Funcs.strptime)
+OmegaConf.register_new_resolver("today", FUNCs.today)
+OmegaConf.register_new_resolver("to_datetime", FUNCs.strptime)
 OmegaConf.register_new_resolver("iif", lambda cond, t, f: t if cond else f)
 OmegaConf.register_new_resolver("alt", lambda val, alt: val or alt)
 OmegaConf.register_new_resolver("randint", random.randint, use_cache=True)
 OmegaConf.register_new_resolver("get_method", hydra.utils.get_method)
-OmegaConf.register_new_resolver("get_original_cwd", Envs.getcwd)
-OmegaConf.register_new_resolver("exists", IOLibs.exists)
-OmegaConf.register_new_resolver("join_path", IOLibs.join_path)
-OmegaConf.register_new_resolver("mkdir", IOLibs.mkdir)
+OmegaConf.register_new_resolver("get_original_cwd", ENVs.getcwd)
+OmegaConf.register_new_resolver("exists", IOLIBs.exists)
+OmegaConf.register_new_resolver("join_path", IOLIBs.join_path)
+OmegaConf.register_new_resolver("mkdir", IOLIBs.mkdir)
 OmegaConf.register_new_resolver("dirname", os.path.dirname)
 OmegaConf.register_new_resolver("basename", os.path.basename)
-OmegaConf.register_new_resolver("check_path", IOLibs.check_path)
+OmegaConf.register_new_resolver("check_path", IOLIBs.check_path)
 OmegaConf.register_new_resolver("cached_path", cached_path)
 OmegaConf.register_new_resolver(
-    "lower_case_with_underscores", Funcs.lower_case_with_underscores
+    "lower_case_with_underscores", FUNCs.lower_case_with_underscores
 )
-OmegaConf.register_new_resolver("dotenv_values", Envs.dotenv_values)
+OmegaConf.register_new_resolver("dotenv_values", ENVs.dotenv_values)
```

### Comparing `hyfi-0.9.1/src/hyfi/joblib/__init__.py` & `hyfi-1.0.0/src/hyfi/joblib/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-from typing import Any
+from typing import Callable, Mapping, Optional, Sequence, Union
 
-from pydantic import BaseModel
+import pandas as pd
+from pydantic import BaseModel, PrivateAttr
+from tqdm.auto import tqdm
 
-from hyfi.__global__ import __about__
-from hyfi.hydra import BaseConfig
+from hyfi import __global__
+from hyfi.composer import BaseConfig
 from hyfi.joblib.batch import batcher
-from hyfi.utils.logging import Logging
+from hyfi.joblib.batch.apply import decorator_apply
+from hyfi.joblib.batch.batcher import Batcher
+from hyfi.utils.logging import LOGGING
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 class DistFramworkConfig(BaseModel):
     """Distributed Framework Configuration"""
 
     backend: str = "joblib"
     initialize: bool = False
@@ -28,84 +32,103 @@
     task_num_gpus: int = 0
     verbose: int = 10
 
 
 class JobLibConfig(BaseConfig):
     """JobLib Configuration"""
 
-    config_name: str = "__init__"
-    config_group: str = "joblib"
+    _config_name_: str = "__init__"
+    _config_group_: str = "joblib"
 
     num_workers: int = 1
     distributed_framework: DistFramworkConfig = DistFramworkConfig()
     batcher: BatcherConfig = BatcherConfig()
-    __initilized__: bool = False
+    _initilized_: bool = PrivateAttr(False)
+    _batcher_instance_: Optional[Batcher] = PrivateAttr(None)
 
-    class Config:
-        extra = "allow"
-        underscore_attrs_are_private = True
-
-    def initialize_configs(self, **config_kwargs):
-        super().initialize_configs(**config_kwargs)
-        self.batcher = BatcherConfig.parse_obj(self.__dict__["batcher"])
-        self.distributed_framework = DistFramworkConfig.parse_obj(
-            self.__dict__["distributed_framework"]
-        )
+    def initialize(self):
+        self.init_backend()
 
     def init_backend(
         self,
     ):
         """Initialize the backend for joblib"""
         if self.distributed_framework.initialize:
             backend_handle = None
             backend = self.distributed_framework.backend
 
-            if backend == "dask":
-                from dask.distributed import Client  # type: ignore
-
-                dask_cfg = {"n_workers": self.distributed_framework.num_workers}
-                logger.debug(f"initializing dask client with {dask_cfg}")
-                client = Client(**dask_cfg)
-                logger.debug(client)
-
-            elif backend == "ray":
+            if backend == "ray":
                 import ray  # type: ignore
 
                 ray_cfg = {"num_cpus": self.distributed_framework.num_workers}
                 logger.debug(f"initializing ray with {ray_cfg}")
                 ray.init(**ray_cfg)
                 backend_handle = ray
 
-            batcher.batcher_instance = batcher.Batcher(
-                backend_handle=backend_handle, **self.batcher.dict()
+            __global__._batcher_instance_ = batcher.Batcher(
+                backend_handle=backend_handle, **self.batcher.model_dump()
             )
-            logger.debug(f"initialized batcher with {batcher.batcher_instance}")
-        self.__initilized__ = True
+            self._batcher_instance_ = __global__._batcher_instance_
+            logger.debug("initialized batcher with %s", __global__._batcher_instance_)
+        self._initilized_ = True
 
     def stop_backend(self):
         """Stop the backend for joblib"""
         backend = self.distributed_framework.backend
-        if batcher.batcher_instance:
+        if __global__._batcher_instance_:
             logger.debug("stopping batcher")
-            del batcher.batcher_instance
+            del __global__._batcher_instance_
 
         logger.debug("stopping distributed framework")
-        if self.distributed_framework.initialize:
-            if backend == "ray":
-                try:
-                    import ray  # type: ignore
+        if self.distributed_framework.initialize and backend == "ray":
+            try:
+                import ray  # type: ignore
 
-                    if ray.is_initialized():
-                        ray.shutdown()
-                        logger.debug("shutting down ray")
-                except ImportError:
-                    logger.warning("ray is not installed")
-
-            elif backend == "dask":
-                try:
-                    from dask.distributed import Client  # type: ignore
-
-                    if Client.initialized():
-                        Client.close()
-                        logger.debug("shutting down dask client")
-                except ImportError:
-                    logger.warning("dask is not installed")
+                if ray.is_initialized():
+                    ray.shutdown()
+                    logger.debug("shutting down ray")
+            except ImportError:
+                logger.warning("ray is not installed")
+
+
+class BATCHER:
+    """
+    A class to apply a function to a series or dataframe using joblib
+    """
+
+    @staticmethod
+    def apply(
+        func: Callable,
+        series: Union[pd.Series, pd.DataFrame, Sequence, Mapping],
+        description: Optional[str] = None,
+        use_batcher: bool = True,
+        minibatch_size: Optional[int] = None,
+        num_workers: Optional[int] = None,
+        **kwargs,
+    ):
+        batcher_instance = JobLibConfig()._batcher_instance_
+        if use_batcher and batcher_instance is not None:
+            batcher_minibatch_size = batcher_instance.minibatch_size
+            if minibatch_size is None:
+                minibatch_size = batcher_minibatch_size
+            if num_workers is not None:
+                batcher_instance.procs = int(num_workers)
+            if batcher_instance.procs > 1:
+                batcher_instance.minibatch_size = min(
+                    int(len(series) / batcher_instance.procs) + 1, minibatch_size
+                )
+                logger.info(
+                    f"Using batcher with minibatch size: {batcher_instance.minibatch_size}"
+                )
+                results = decorator_apply(
+                    func,
+                    batcher_instance,
+                    description=description,  # type: ignore
+                )(series)
+                if batcher_instance is not None:
+                    batcher_instance.minibatch_size = batcher_minibatch_size
+                return results
+
+        if batcher_instance is None:
+            logger.info("Warning: batcher not initialized")
+        tqdm.pandas(desc=description)
+        return series.progress_apply(func)  # type: ignore
```

### Comparing `hyfi-0.9.1/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.0.0/src/hyfi/joblib/batch/batcher.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,137 +1,113 @@
 """Batcher class for handling parallel jobs on minibatches"""
 import contextlib
 import multiprocessing
-import random
 from contextlib import closing
 from math import ceil
+from typing import Any, Callable, List, Optional
 
 import pandas as pd
 import scipy.sparse as ssp
 from tqdm.auto import tqdm
 
-from hyfi.utils.logging import Logging
+from hyfi.utils.logging import LOGGING
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 class Batcher(object):
     """Scheduler to handle parallel jobs on minibatches
 
-    Parameters
-    ----------
-    procs: int
-            Number of process(es)/thread(s) for executing task in parallel. Used for multiprocessing, threading and Loky
+    Attributes:
+        procs (int):
+                Number of process(es)/thread(s) for executing task in parallel. Used for multiprocessing, threading and Loky
 
-    minibatch_size: int
-            Expected size of each minibatch
-
-    backend: {'serial', 'multiprocessing', 'threading', 'loky', 'spark', 'dask', 'ray'}
-            Backend for computing the tasks
-
-                    - 'serial' sequential execution without a backend scheduler
+        minibatch_size (int):
+                Expected size of each minibatch
 
-                    - 'multiprocessing' Python standard multiprocessing library
+        backend (str): {'serial', 'multiprocessing', 'threading', 'loky', 'spark', 'dask', 'ray'}
+                Backend for computing the tasks
 
-                    - 'threading' Python standard threading library
+                        - 'serial' sequential execution without a backend scheduler
 
-                    - 'loky' Loky fork of multiprocessing library
+                        - 'multiprocessing' Python standard multiprocessing library
 
-                    - 'joblib' Joblib fork of multiprocessing library
+                        - 'threading' Python standard threading library
 
-                    - 'spark' PySpark local or distributed execution
+                        - 'loky' Loky fork of multiprocessing library
 
-                    - 'dask' Dask Distributed local or distributed execution
+                        - 'joblib' Joblib fork of multiprocessing library
 
-                    - 'ray' Ray local or distributed execution
+                        - 'ray' Ray local or distributed execution
 
-    task_num_cpus: int
-            Number of CPUs to reserve per minibatch task for Ray
+        task_num_cpus (int):
+                Number of CPUs to reserve per minibatch task for Ray
 
-    task_num_gpus: int
-            Number of GPUs to reserve per minibatch task for Ray
+        task_num_gpus (int):
+                Number of GPUs to reserve per minibatch task for Ray
 
-    backend_handle: object
-            Backend handle for sending tasks
+        backend_handle (object):
+                Backend handle for sending tasks
 
-    verbose: int
-            Verbosity level.
-            Setting verbose > 0 will display additional information depending on the specific level set.
+        verbose (int):
+                Verbosity level.
+                Setting verbose > 0 will display additional information depending on the specific level set.
     """
 
     def __init__(
         self,
-        procs=0,
-        minibatch_size=20000,
-        backend_handle=None,
-        backend="multiprocessing",
-        task_num_cpus=1,
-        task_num_gpus=0,
-        verbose=0,
+        procs: Optional[int] = 0,
+        minibatch_size: int = 20000,
+        backend_handle: Any = None,
+        backend: str = "multiprocessing",
+        task_num_cpus: int = 1,
+        task_num_gpus: int = 0,
+        verbose: int = 0,
     ):
-        if isinstance(procs, str):
-            procs = int(procs)
         if procs == 0 or procs is None:
             procs = multiprocessing.cpu_count()
         self.procs = procs
         self.verbose = verbose
         self.minibatch_size = minibatch_size
         self.backend_handle = backend_handle
         self.backend = backend
         self.task_num_cpus = task_num_cpus
         self.task_num_gpus = task_num_gpus
 
-    def list2indexedrdd(self, lst, minibatch_size=0):
-        if minibatch_size == 0:
-            minibatch_size = self.minibatch_size
-        start = 0
-        len_data = len(lst)
-        batch_count = 0
-        batches = []
-        while start < len_data:
-            batches.append([batch_count] + [lst[start : start + minibatch_size]])
-            start += minibatch_size
-            batch_count += 1
-        return self.backend_handle.parallelize(batches)
-
-    def indexedrdd2list(self, indexedrdd, sort=True):
-        batches = indexedrdd.collect()
-        if sort:
-            batches = sorted(batches)
-        return [batch[1] for batch in batches]
-
-    def split_batches(self, data, minibatch_size=None, backend=None):
+    def split_batches(
+        self,
+        data: Any,
+        minibatch_size: Optional[int] = None,
+        backend: Any = None,
+    ):
         """Split data into minibatches with a specified size
 
-        Parameters
-        ----------
-        data: iterable and indexable
-                List-like data to be split into batches. Includes backend_handleipy matrices and Pandas DataFrames.
+        Arguments:
+            data (list, tuple, dict, numpy.ndarray, scipy.sparse.csr_matrix, pandas.DataFrame):
+                List-like data to be split into batches. Includes numpy matrices and Pandas DataFrames.
 
-        minibatch_size: int
+            minibatch_size (int):
                 Expected sizes of minibatches split from the data.
 
-        backend: object
+            backend (str):
                 Backend to use, instead of the Batcher backend attribute
 
-        Returns
-        -------
-        data_split: list
+        Returns:
+            data_split (list):
                 List of minibatches, each entry is a list-like object representing the data subset in a batch.
         """
         if minibatch_size is None:
             minibatch_size = self.minibatch_size
         if backend is None:
             backend = self.backend
         if isinstance(data, (list, tuple, dict)):
             len_data = len(data)
         else:
             len_data = data.shape[0]
-        if backend == "spark":
-            return self.list2indexedrdd(data, minibatch_size)
+
         if isinstance(data, pd.DataFrame):
             data = [
                 data.iloc[x * minibatch_size : (x + 1) * minibatch_size]
                 for x in range(int(ceil(len_data / minibatch_size)))
             ]
         elif isinstance(data, dict):
             data = [
@@ -143,122 +119,109 @@
                 for x in range(int(ceil(len_data / minibatch_size)))
             ]
         else:
             data = [
                 data[x * minibatch_size : min(len_data, (x + 1) * minibatch_size)]
                 for x in range(int(ceil(len_data / minibatch_size)))
             ]
-        # if backend=="dask":  return self.backend_handle.scatter(data)
         return data
 
-    def collect_batches(self, data, backend=None, sort=True):
+    def collect_batches(self, data: Any, backend: Any = None):
         if backend is None:
             backend = self.backend
-        if backend == "spark":
-            data = self.indexedrdd2list(data, sort)
-        if backend == "dask":
-            data = self.backend_handle.gather(data)
         return data
 
-    def merge_batches(self, data):
+    def merge_batches(self, data: Any):
         """Merge a list of data minibatches into one single instance representing the data
 
-        Parameters
-        ----------
-        data: list
+        Arguments:
+            data (list):
                 List of minibatches to merge
 
-        Returns
-        -------
-        (anonymous): sparse matrix | pd.DataFrame | list
+        Returns:
+            data (list, numpy.ndarray, scipy.sparse.csr_matrix, pandas.DataFrame):
                 Single complete list-like data merged from given batches
         """
-        if isinstance(data[0], ssp.csr_matrix):
-            return ssp.vstack(data)
+        if isinstance(data[0], ssp.csr_matrix):  # type: ignore
+            return ssp.vstack(data)  # type: ignore
         if isinstance(data[0], (pd.DataFrame, pd.Series)):
             return pd.concat(data)
         return [item for sublist in data for item in sublist]
 
     def process_batches(
         self,
-        task,
-        data,
-        args,
-        backend=None,
-        backend_handle=None,
-        input_split=False,
-        merge_output=True,
-        minibatch_size=None,
-        procs=None,
-        task_num_cpus=None,
-        task_num_gpus=None,
-        verbose=None,
-        description="batch_apply",
+        task: Callable,
+        data: Any,
+        args: List[Any],
+        backend: Optional[str] = None,
+        backend_handle: Any = None,
+        input_split: bool = False,
+        merge_output: bool = True,
+        minibatch_size: Optional[int] = None,
+        procs: Optional[int] = None,
+        task_num_cpus: Optional[int] = None,
+        task_num_gpus: Optional[int] = None,
+        verbose: Optional[int] = None,
+        description: str = "batch_apply",
     ):
         """
+        Apply a function on minibatches of data in parallel
 
-        Parameters
-        ----------
-        task: function
+        Arguments:
+            task (callable):
                 Function to apply on each minibatch with other specified arguments
 
-        data: list-like
+            data (list, tuple, dict, numpy.ndarray, scipy.sparse.csr_matrix, pandas.DataFrame):
                 Samples to split into minibatches and apply the specified function on
 
-        args: list
+            args (list):
                 Arguments to pass to the specified function following the mini-batch
 
-        input_split: boolean, default False
+            input_split (bool):
                 If True, input data is already mapped into minibatches, otherwise data will be split on call.
 
-        merge_output: boolean, default True
+            merge_output (bool):
                 If True, results from minibatches will be reduced into one single instance before return.
 
-        procs: int
-                Number of process(es)/thread(s) for executing task in parallel. Used for multiprocessing, threading,
-                Loky and Ray
+            procs (int):
+                Number of process(es)/thread(s) for executing task in parallel. Used for multiprocessing, threading, Loky and Ray
 
-        minibatch_size: int
+            minibatch_size (int):
                 Expected size of each minibatch
 
-        backend: {'serial', 'multiprocessing', 'threading', 'loky', 'spark', 'dask', 'ray'}
+            backend (str): {'serial', 'multiprocessing', 'threading', 'loky', 'spark', 'dask', 'ray'}
                 Backend for computing the tasks
 
                         - 'serial' sequential execution without a backend scheduler
 
                         - 'multiprocessing' Python standard multiprocessing library
 
                         - 'threading' Python standard threading library
 
                         - 'loky' Loky fork of multiprocessing library
 
                         - 'joblib' Joblib fork of multiprocessing library
 
-                        - 'spark' PySpark local or distributed execution
-
-                        - 'dask' Dask Distributed local or distributed execution
-
                         - 'ray' Ray local or distributed execution
 
-        backend_handle: object
+            backend_handle (object):
                 Backend handle for sending tasks
 
-        task_num_cpus: int
+            task_num_cpus (int):
                 Number of CPUs to reserve per minibatch task for Ray
 
-        task_num_gpus: int
+            task_num_gpus (int):
                 Number of GPUs to reserve per minibatch task for Ray
 
-        verbose: int
+            verbose (int):
                 Verbosity level.
                 Setting verbose > 0 will display additional information depending on the specific level set.
 
-        Returns
-        -------
-        results: list-like | list of list-like
+        Returns:
+            data (list):
                 If merge_output is specified as True, this will be a list-like object representing
                 the dataset, with each entry as a sample. Otherwise this will be a list of list-like
                 objects, with each entry representing the results from a minibatch.
         """
         if procs is None:
             procs = self.procs
         if backend is None:
@@ -267,54 +230,60 @@
             backend_handle = self.backend_handle
         if task_num_cpus is None:
             task_num_cpus = self.task_num_cpus
         if task_num_gpus is None:
             task_num_gpus = self.task_num_gpus
         if verbose is None:
             verbose = self.verbose
-        if verbose > 1:
-            logger.info(
-                f" backend: {backend}  minibatch_size: {self.minibatch_size}  procs: {procs}  input_split: {input_split}  merge_output: {merge_output}  len(data): {len(data)} len(args): {len(args)}"
-            )
-
-        if verbose > 10:
-            logger.info(
-                f" len(data): {len(data)} len(args): {len(args)} [type(x) for x in data]: {[type(x) for x in data]} [type(x) for x in args]: {[type(x) for x in args]}"
-            )
+        # if verbose > 1:
+        logger.debug(
+            " backend: %s  minibatch_size: %s  procs: %s  input_split: %s  merge_output: %s  len(data): %s len(args): %s",
+            backend,
+            self.minibatch_size,
+            procs,
+            input_split,
+            merge_output,
+            len(data),
+            len(args),
+        )
+
+        # if verbose > 10:
+        logger.debug(
+            " len(data): %s len(args): %s [type(x) for x in data]: %s [type(x) for x in args]: %s",
+            len(data),
+            len(args),
+            [type(x) for x in data],
+            [type(x) for x in args],
+        )
 
         if not (input_split):
-            if backend == "spark":
-                paral_params = self.split_batches(data, minibatch_size, backend="spark")
-            else:
-                paral_params = [
-                    [data_batch] + args
-                    for data_batch in self.split_batches(data, minibatch_size)
-                ]
+            paral_params = [
+                [data_batch] + args
+                for data_batch in self.split_batches(data, minibatch_size)
+            ]
         else:
-            if backend != "spark":
-                paral_params = [[data_batch] + args for data_batch in data]
-            else:
-                paral_params = data
-        if verbose > 10:
-            print(" Start task, len(paral_params)", len(paral_params))
+            paral_params = [[data_batch] + args for data_batch in data]
+        if verbose > 1:
+            logger.debug("Start task, len(paral_params): %s", len(paral_params))
+        results = []
         if backend == "serial":
             results = [
                 task(minibatch) for minibatch in tqdm(paral_params, desc=description)
             ]
         else:
             if backend == "multiprocessing":
                 with closing(
                     multiprocessing.Pool(max(1, procs), maxtasksperchild=2)
                 ) as pool:
                     results = pool.map_async(task, paral_params)
                     pool.close()
                     pool.join()
                     results = results.get()
             elif backend == "threading":
-                with closing(multiprocessing.dummy.Pool(max(1, procs))) as pool:
+                with closing(multiprocessing.Pool(max(1, procs))) as pool:
                     results = pool.map(task, paral_params)
                     pool.close()
                     pool.join()
             elif backend == "loky":
                 from loky import get_reusable_executor
 
                 pool = get_reusable_executor(max_workers=max(1, procs))
@@ -328,26 +297,14 @@
                     results = Parallel(n_jobs=procs)(
                         delayed(task)(params) for params in paral_params
                     )
             elif backend == "p_tqdm":
                 from p_tqdm import p_map
 
                 results = p_map(task, paral_params, num_cpus=procs)
-            elif backend == "dask":
-                # if not (input_split):  data= self.scatter(data)
-                results = [
-                    self.backend_handle.submit(task, params)
-                    for params in tqdm(paral_params, desc=description)
-                ]
-            elif backend == "spark":
-
-                def apply_func_to_indexedrdd(batch):
-                    return [batch[0]] + [task([batch[1]] + args)]
-
-                results = paral_params.map(apply_func_to_indexedrdd)
             elif backend == "ray":
 
                 @self.backend_handle.remote(
                     num_cpus=task_num_cpus, num_gpus=task_num_gpus
                 )
                 def f_ray(f, data):
                     return f(data)
@@ -355,15 +312,15 @@
                 pbar = tqdm(desc=description, total=len(paral_params) + 1)
                 results = [
                     f_ray.remote(task, paral_params.pop(0))
                     for _ in range(min(len(paral_params), self.procs))
                 ]
                 uncompleted = results
                 pbar.update(len(results))
-                while len(paral_params) > 0:
+                while paral_params:
                     # More tasks than available processors. Queue the task calls
                     done, remaining = self.backend_handle.wait(
                         uncompleted, timeout=60, fetch_local=False
                     )
                     # if verbose > 5:  print("Done, len(done), len(remaining)", len(done), len(remaining))
                     if len(done) == 0:
                         continue
@@ -373,71 +330,33 @@
                         new = f_ray.remote(task, paral_params.pop(0))
                         pbar.update(1)
                         uncompleted.append(new)
                         results.append(new)
                 results = [self.backend_handle.get(x) for x in results]
                 pbar.update(1)
                 pbar.close()
-            # ppft currently not supported. Supporting arbitrary tasks requires modifications to passed arguments
-            # elif backend == "ppft":
-            #   jobs = [self.backend_handle.submit(task, (x,), (), ()) for x in paral_params]
-            # 	results = [x() for x in jobs]
 
         if merge_output:
             return self.merge_batches(self.collect_batches(results, backend=backend))
-        if verbose > 2:
-            logger.info(
-                f" Task: {task}  backend: {backend}  backend_handle: {backend_handle}  completed"
-            )
+        logger.debug(
+            "Task: %s  backend: %s  backend_handle: %s completed",
+            task,
+            backend,
+            backend_handle,
+        )
         return results
 
-    def shuffle_batch(self, texts, labels=None, seed=None):
-        """Shuffle a list of samples, as well as the labels if specified
-
-        Parameters
-        ----------
-        texts: list-like
-                List of samples to shuffle
-
-        labels: list-like (optional)
-                List of labels to shuffle, should be correspondent to the samples given
-
-        seed: int
-                The seed of the pseudo random number generator to use for shuffling
-
-        Returns
-        -------
-        texts: list
-                List of shuffled samples (texts parameters)
-
-        labels: list (optional)
-                List of shuffled labels. This will only be returned when non-None
-                labels is passed
-        """
-        if seed is not None:
-            random.seed(seed)
-        index_shuf = list(range(len(texts)))
-        random.shuffle(index_shuf)
-        texts = [texts[x] for x in index_shuf]
-        if labels is None:
-            return texts
-        labels = [labels[x] for x in index_shuf]
-        return texts, labels
-
     def __getstate__(self):
         return dict(self.__dict__.items())
 
-    def __setstate__(self, params):
+    def __setstate__(self, params: dict):
         for key in params:
             setattr(self, key, params[key])
 
 
-batcher_instance: Batcher
-
-
 @contextlib.contextmanager
 def tqdm_joblib(tqdm_object):
     """Context manager to patch joblib to report into tqdm progress bar given as argument"""
     import joblib
 
     class TqdmBatchCompletionCallBack(joblib.parallel.BatchCompletionCallBack):
         def __call__(self, *args, **kwargs):
```

### Comparing `hyfi-0.9.1/src/hyfi/main/__init__.py` & `hyfi-1.0.0/src/hyfi/main/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,286 @@
 """
     This module contains the primary class for the hyfi config package, HyFI,
     as well as various utility functions and imports.
 """
 import os
 from pathlib import Path, PosixPath, WindowsPath
-from typing import IO, Any, Dict, List, Mapping, Optional, Sequence, Tuple, Union
+from typing import (
+    IO,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import pandas as pd
 from omegaconf import DictConfig, ListConfig, SCMode
 
 from hyfi.__global__ import __home_path__, __hyfi_path__
 from hyfi.__global__.config import __global_config__
+from hyfi.composer import Composer, DictKeyType, SpecialKeys
+from hyfi.composer.extended import XC
 from hyfi.dotenv import DotEnvConfig
-from hyfi.hydra import Composer, DictKeyType, SpecialKeys
-from hyfi.hydra.main import XC
-from hyfi.joblib.pipe import PIPE
+from hyfi.joblib import BATCHER, JobLibConfig
+from hyfi.pipeline import PipelineConfig, PIPELINEs
+from hyfi.pipeline.configs import PipeConfig
 from hyfi.project import ProjectConfig
-from hyfi.utils.datasets import Datasets
-from hyfi.utils.envs import Envs
-from hyfi.utils.funcs import Funcs
+from hyfi.task import TaskConfig
+from hyfi.utils.datasets import DatasetLikeType, Datasets, DatasetType
+from hyfi.utils.envs import ENVs
+from hyfi.utils.funcs import FUNCs
 from hyfi.utils.gpumon import nvidia_smi, set_cuda
-from hyfi.utils.iolibs import IOLibs
-from hyfi.utils.logging import Logging
+from hyfi.utils.iolibs import IOLIBs
+from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
-from hyfi.utils.packages import Packages
+from hyfi.utils.packages import PKGs
 from hyfi.utils.types import PathLikeType
+from hyfi.workflow import WorkflowConfig
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 def _about(cfg):
     pkg_name = cfg.about.__package_name__
     name = cfg.about.name
     print()
-    for k, v in cfg.about.dict().items():
+    for k, v in cfg.about.model_dump().items():
         if k.startswith("_"):
             continue
         print(f"{k:11} : {v}")
     if pkg_name:
         print(f"\nExecute `{pkg_name} --help` to see what you can do with {name}")
 
 
 class HyFI:
     """Primary class for the hyfi config package"""
 
     config = __global_config__
     SpeicialKeys = SpecialKeys
-    __version__ = __global_config__.__version__
+    __version__ = __global_config__._version_
     __hyfi_path__ = __hyfi_path__()
     __home_path__ = __home_path__()
 
     def __init__(self) -> None:
         raise NotImplementedError("Use one of the static construction functions")
 
     @staticmethod
     def about() -> None:
         """Print the about information"""
         cfg = __global_config__
         _about(cfg)
 
     @staticmethod
-    def init_workspace(
+    def init_project(
         project_name: str = "",
-        task_name: str = "",
         project_description: str = "",
         project_root: str = "",
         project_workspace_name: str = "",
         global_hyfi_root: str = "",
         global_workspace_name: str = "",
         num_workers: int = -1,
         log_level: str = "",
+        reinit: bool = True,
         autotime: bool = True,
         retina: bool = True,
         verbose: Union[bool, int] = False,
         **kwargs,
     ) -> ProjectConfig:
         """
         Initialize and start hyfi.
 
         Args:
-                project_name: Name of the project to use.
-                task_name: Name of the task to use.
-                project_description: Description of the project that will be used.
-                project_root: Root directory of the project.
-                project_workspace_name: Name of the project's workspace directory.
-                global_hyfi_root: Root directory of the global hyfi.
-                global_workspace_name: Name of the global hierachical workspace directory.
-                num_workers: Number of workers to run.
-                log_level: Log level for the log.
-                autotime: Whether to automatically set time and / or keep track of run times.
-                retina: Whether to use retina or not.
-                verbose: Enables or disables logging
+            project_name: Name of the project to use.
+            project_description: Description of the project that will be used.
+            project_root: Root directory of the project.
+            project_workspace_name: Name of the project's workspace directory.
+            global_hyfi_root: Root directory of the global hyfi.
+            global_workspace_name: Name of the global hierachical workspace directory.
+            num_workers: Number of workers to run.
+            log_level: Log level for the log.
+            autotime: Whether to automatically set time and / or keep track of run times.
+            retina: Whether to use retina or not.
+            verbose: Enables or disables logging
         """
-        __global_config__.init_workspace(
+        __global_config__.init_project(
             project_name=project_name,
-            task_name=task_name,
             project_description=project_description,
             project_root=project_root,
             project_workspace_name=project_workspace_name,
             global_hyfi_root=global_hyfi_root,
             global_workspace_name=global_workspace_name,
             num_workers=num_workers,
             log_level=log_level,
+            reinit=reinit,
             autotime=autotime,
             retina=retina,
             verbose=verbose,
             **kwargs,
         )
         if __global_config__.project:
             return __global_config__.project
         else:
             raise ValueError("Project not initialized.")
 
     @staticmethod
-    def initialize(config: Union[DictConfig, Dict] = None):  # type: ignore
-        """Initialize the global config"""
-        __global_config__.initialize(config)
+    def initialize(force: bool = False) -> None:
+        """
+        Initialize the global config.
+
+        Args:
+            force: If True, force initialization even if already initialized.
+
+        Returns:
+            bool: True if initialization was successful, False otherwise.
+        """
+        __global_config__.initialize(force=force)
 
     @staticmethod
-    def terminate():
-        """Terminate the global config"""
+    def terminate() -> None:
+        """
+        Terminate the global config.
+
+        Returns:
+            bool: True if termination was successful, False otherwise.
+        """
         __global_config__.terminate()
 
     @staticmethod
-    def dotenv() -> DotEnvConfig:
-        """Return the DotEnvConfig"""
-        return DotEnvConfig()
+    def joblib(**kwargs) -> JobLibConfig:
+        """
+        Return the joblib pipe.
+
+        Args:
+            **kwargs: Additional keyword arguments to pass to the JobLibConfig constructor.
+
+        Returns:
+            JobLibConfig: An instance of the JobLibConfig class.
+        """
+        return JobLibConfig(**kwargs)
+
+    @staticmethod
+    def dotenv(**kwargs) -> DotEnvConfig:
+        """
+        Return the DotEnvConfig.
+
+        Args:
+            **kwargs: Additional keyword arguments to pass to the DotEnvConfig constructor.
+
+        Returns:
+            DotEnvConfig: An instance of the DotEnvConfig class.
+        """
+        return DotEnvConfig(**kwargs)
 
     @staticmethod
     def osenv():
-        """Return the DotEnvConfig"""
+        """
+        Return the os environment variables as a dictionary.
+
+        Returns:
+            dict: A dictionary containing the os environment variables.
+        """
         return os.environ
 
     @staticmethod
+    def pipe_config(**kwargs) -> PipeConfig:
+        """
+        Return the PipeConfig.
+
+        Args:
+            **kwargs: Additional keyword arguments to pass to the PipeConfig constructor.
+
+        Returns:
+            PipeConfig: An instance of the PipeConfig class.
+        """
+        return PipeConfig(**kwargs)
+
+    @staticmethod
+    def task_config(**kwargs) -> TaskConfig:
+        """
+        Return the TaskConfig.
+
+        Args:
+            **kwargs: Additional keyword arguments to pass to the TaskConfig constructor.
+
+        Returns:
+            TaskConfig: An instance of the TaskConfig class.
+        """
+        return TaskConfig(**kwargs)
+
+    @staticmethod
+    def workflow_config(**kwargs) -> WorkflowConfig:
+        """
+        Return the WorkflowConfig.
+
+        Args:
+            **kwargs: Additional keyword arguments to pass to the WorkflowConfig constructor.
+
+        Returns:
+            WorkflowConfig: An instance of the WorkflowConfig class.
+        """
+        return WorkflowConfig(**kwargs)
+
+    @staticmethod
+    def compose_as_dict(
+        config_group: Union[str, None] = None,
+        overrides: Union[List[str], None] = None,
+        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        throw_on_resolution_failure: bool = True,
+        throw_on_missing: bool = False,
+        root_config_name: Union[str, None] = None,
+        config_module: Union[str, None] = None,
+        global_package: bool = False,
+        verbose: bool = False,
+    ) -> Dict:
+        """
+        Compose a configuration by applying overrides and return the result as a dict(
+
+        Args:
+            config_group (Union[str, None], optional): Name of the config group to compose (`config_group=name`). Defaults to None.
+            overrides (Union[List[str], None], optional): List of config groups to apply overrides to (`overrides=["override_name"]`). Defaults to None.
+            config_data (Union[Dict[str, Any], DictConfig, None], optional): Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`). Defaults to None.
+            throw_on_resolution_failure (bool, optional): If True throw an exception if resolution fails. Defaults to True.
+            throw_on_missing (bool, optional): If True throw an exception if config_group doesn't exist. Defaults to False.
+            root_config_name (Union[str, None], optional): Name of the root config to be used (e.g. `hconf`). Defaults to None.
+            config_module (Union[str, None], optional): Name of the module containing the configuration. Defaults to None.
+            global_package (bool, optional): If True, the configuration is loaded from the global package. Defaults to False.
+            verbose (bool, optional): If True, print verbose output. Defaults to False.
+
+        Returns:
+            Dict: The composed configuration as a dictionary.
+        """
+        return Composer._compose_as_dict(
+            config_group=config_group,
+            overrides=overrides,
+            config_data=config_data,
+            throw_on_resolution_failure=throw_on_resolution_failure,
+            throw_on_missing=throw_on_missing,
+            config_name=root_config_name,
+            config_module=config_module,
+            global_package=global_package,
+            verbose=verbose,
+        )
+
+    @staticmethod
     def compose(
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
-        return_as_dict: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
         root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
-    ) -> Union[DictConfig, Dict]:
+    ) -> DictConfig:
         """
         Compose a configuration by applying overrides
 
         Args:
             config_group: Name of the config group to compose (`config_group=name`)
             overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
             config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
@@ -163,15 +295,14 @@
         Returns:
             A config object or a dictionary with the composed config
         """
         return Composer._compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
-            return_as_dict=return_as_dict,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
             config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
@@ -181,63 +312,117 @@
         cfg: Any,
         key: str,
         *,
         default: Any = None,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
     ):
+        """
+        Select a value from a configuration object using a key.
+
+        Args:
+            cfg: The configuration object to select from.
+            key: The key to use for the selection.
+            default: The default value to return if the key is not found.
+            throw_on_resolution_failure: If True, throw an exception if resolution fails.
+            throw_on_missing: If True, throw an exception if the key is not found.
+
+        Returns:
+            The selected value, or the default value if the key is not found and no exception is thrown.
+        """
         return Composer.select(
             cfg,
             key,
             default=default,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
         )
 
     @staticmethod
     def to_dict(
         cfg: Any,
     ):
+        """
+        Convert a configuration object to a dictionary.
+
+        Args:
+            cfg: The configuration object to convert.
+
+        Returns:
+            The configuration object as a dictionary.
+        """
         return Composer.to_dict(cfg)
 
     @staticmethod
     def to_config(
         cfg: Any,
     ):
+        """
+        Convert a configuration object to a Config object.
+
+        Args:
+            cfg: The configuration object to convert.
+
+        Returns:
+            The configuration object as a Config object.
+        """
         return Composer.to_config(cfg)
 
     @staticmethod
     def to_yaml(cfg: Any, resolve: bool = False, sort_keys: bool = False) -> str:
+        """
+        Convert a configuration object to a YAML string.
+
+        Args:
+            cfg: The configuration object to convert.
+            resolve: Whether to resolve references in the configuration object.
+            sort_keys: Whether to sort the keys in the resulting YAML string.
+
+        Returns:
+            The configuration object as a YAML string.
+        """
         return Composer.to_yaml(cfg, resolve=resolve, sort_keys=sort_keys)
 
     @staticmethod
     def to_container(
         cfg: Any,
         *,
         resolve: bool = False,
         throw_on_missing: bool = False,
         enum_to_str: bool = False,
         structured_config_mode: SCMode = SCMode.DICT,
     ):
+        """
+        Convert a configuration object to a structured container.
+
+        Args:
+            cfg: The configuration object to convert.
+            resolve: Whether to resolve references in the configuration object.
+            throw_on_missing: Whether to throw an error if a key is missing.
+            enum_to_str: Whether to convert enums to strings.
+            structured_config_mode: The structured config mode to use.
+
+        Returns:
+            The configuration object as a structured container.
+        """
         return Composer.to_container(
             cfg=cfg,
             resolve=resolve,
             throw_on_missing=throw_on_missing,
             enum_to_str=enum_to_str,
             structured_config_mode=structured_config_mode,
         )
 
     @staticmethod
     def partial(
-        config: Any = None,
-        config_group: Union[str, None] = None,
+        config: Union[str, Dict],
         *args: Any,
         **kwargs: Any,
-    ) -> Any:
-        return XC.partial(config=config, config_group=config_group, *args, **kwargs)
+    ) -> Callable:
+        return XC.partial(config, *args, **kwargs)
 
     @staticmethod
     def instantiate(config: Any, *args: Any, **kwargs: Any) -> Any:
         return XC.instantiate(config, *args, **kwargs)
 
     @staticmethod
     def is_config(
@@ -271,17 +456,25 @@
             Dict[DictKeyType, Any],
             List[Any],
             Tuple[Any, ...],
             Any,
         ],
     ) -> Union[ListConfig, DictConfig]:
         """
-        Merge a list of previously created configs into a single one
-        :param configs: Input configs
-        :return: the merged config object.
+        Merges multiple configurations into a single configuration.
+
+        Args:
+            *configs: One or more configurations to merge. These can be of various types, including
+                `DictConfig`, `ListConfig`, `dict`, `list`, `tuple`, or any other type that can be
+                converted to a `DictConfig` or `ListConfig`.
+
+        Returns:
+            A new configuration that is the result of merging all of the input configurations.
+            The type of the returned configuration will be the same as the type of the first input
+            configuration.
         """
         return Composer.merge(*configs)
 
     @staticmethod
     def save(config: Any, f: Union[str, Path, IO[Any]], resolve: bool = False) -> None:
         Composer.save(config, f, resolve)
 
@@ -305,26 +498,14 @@
         Composer.print(cfg, resolve=resolve, **kwargs)
 
     @staticmethod
     def print(cfg: Any, resolve: bool = True, **kwargs):
         Composer.print(cfg, resolve=resolve, **kwargs)
 
     @staticmethod
-    def methods(cfg: Any, obj: object, return_function=False):
-        return Composer.methods(cfg, obj, return_function)
-
-    @staticmethod
-    def function(cfg: Any, _name_, return_function=False, **parms):
-        return XC.function(cfg, _name_, return_function, **parms)
-
-    @staticmethod
-    def run(config: Any, **kwargs: Any) -> Any:
-        XC.run(config, **kwargs)
-
-    @staticmethod
     def ensure_list(value):
         return Composer.ensure_list(value)
 
     @staticmethod
     def ensure_kwargs(_kwargs, _fn):
         return Composer.ensure_kwargs(_kwargs, _fn)
 
@@ -340,46 +521,68 @@
     # Logging related functions
     ###############################
     @staticmethod
     def getLogger(
         name=None,
         log_level=None,
     ):
-        return Logging.getLogger(name, log_level)
+        return LOGGING.getLogger(name, log_level)
 
     @staticmethod
     def setLogger(level=None, force=True, **kwargs):
-        return Logging.setLogger(level, force, **kwargs)
+        return LOGGING.setLogger(level, force, **kwargs)
 
     ###############################
-    # Batcher related functions
+    # Pipeline related functions
     ###############################
     @staticmethod
-    def pipe(data=None, cfg=None):
-        return PIPE.pipe(data, cfg)
+    def run_task(task: TaskConfig, project: Optional[ProjectConfig] = None):
+        """Run the pipelines specified in the task"""
+        PIPELINEs.run_task(task, project)
+
+    @staticmethod
+    def run_workflow(workflow: WorkflowConfig):
+        """Run the pipelines specified in the workflow"""
+        PIPELINEs.run_workflow(workflow)
 
     @staticmethod
+    def run_pipeline(
+        config: Union[Dict, PipelineConfig],
+        initial_object: Optional[Any] = None,
+        task: Optional[TaskConfig] = None,
+    ) -> Any:
+        return PIPELINEs.run_pipeline(config, initial_object, task)
+
+    @staticmethod
+    def run_pipe(
+        obj: Any,
+        config: Union[Dict, PipeConfig],
+    ) -> Any:
+        return PIPELINEs.run_pipe(obj, config)
+
+    ###############################
+    # Batcher related functions
+    ###############################
+    @staticmethod
     def apply(
-        func,
-        series,
-        description=None,
-        use_batcher=True,
-        minibatch_size=None,
-        num_workers=None,
-        verbose=False,
+        func: Callable,
+        series: Union[pd.Series, pd.DataFrame, Sequence, Mapping],
+        description: Optional[str] = None,
+        use_batcher: bool = True,
+        minibatch_size: Optional[int] = None,
+        num_workers: Optional[int] = None,
         **kwargs,
     ):
-        return PIPE.apply(
+        return BATCHER.apply(
             func,
             series,
             description=description,
             use_batcher=use_batcher,
             minibatch_size=minibatch_size,
             num_workers=num_workers,
-            verbose=verbose,
             **kwargs,
         )
 
     ###############################
     # Dataset related functions
     ###############################
     @staticmethod
@@ -396,15 +599,15 @@
         keep_in_memory: Optional[bool] = None,
         save_infos: bool = False,
         use_auth_token: Optional[Union[bool, str]] = None,
         streaming: bool = False,
         num_proc: Optional[int] = None,
         storage_options: Optional[Dict] = None,
         **config_kwargs,
-    ) -> Any:
+    ) -> DatasetLikeType:
         """Load a dataset from the Hugging Face Hub, or a local dataset.
 
         It also allows to load a dataset from a local directory or a dataset repository on the Hugging Face Hub without dataset script.
         In this case, it automatically loads all the data files from the directory or the dataset repository.
 
         Args:
 
@@ -566,81 +769,193 @@
         nrows=None,
     ):
         return Datasets.records_to_dataframe(
             data, index, exclude, columns, coerce_float, nrows
         )
 
     @staticmethod
-    def save_data(
-        data: Union[pd.DataFrame, dict],
-        filename: str,
-        base_dir: str = "",
-        columns=None,
-        index: bool = False,
-        filetype="parquet",
-        suffix: str = "",
+    def concatenate_data(
+        data: Union[Dict[str, pd.DataFrame], Sequence[pd.DataFrame], List[DatasetType]],
+        columns: Optional[Sequence[str]] = None,
+        add_split_key_column: bool = False,
+        added_column_name: str = "_name_",
+        ignore_index: bool = True,
+        axis: int = 0,
+        split: Optional[str] = None,
         verbose: bool = False,
         **kwargs,
     ):
-        Datasets.save_data(
+        return Datasets.concatenate_data(
             data,
-            filename,
-            base_dir=base_dir,
-            columns=columns,
-            index=index,
-            filetype=filetype,
-            suffix=suffix,
-            verbose=verbose,
+            columns,
+            add_split_key_column,
+            added_column_name,
+            ignore_index,
+            axis,
+            split,
+            verbose,
             **kwargs,
         )
 
     @staticmethod
-    def load_data(filename=None, base_dir=None, filetype=None, verbose=False, **kwargs):
-        if filename is not None:
-            filename = str(filename)
-        if SpecialKeys.TARGET in kwargs:
-            return XC.instantiate(
-                kwargs,
-                filename=filename,
-                base_dir=base_dir,
-                verbose=verbose,
-                filetype=filetype,
-            )
-        if filename is None:
-            raise ValueError("filename must be specified")
+    def concatenate_dataframes(
+        data: Union[Dict[str, pd.DataFrame], Sequence[pd.DataFrame]],
+        columns: Optional[Sequence[str]] = None,
+        add_split_key_column: bool = False,
+        added_column_name: str = "_name_",
+        ignore_index: bool = True,
+        axis: int = 0,
+        verbose: bool = False,
+        **kwargs,
+    ) -> pd.DataFrame:
+        return Datasets.concatenate_dataframes(
+            data,
+            columns,
+            add_split_key_column,
+            added_column_name,
+            ignore_index,
+            axis,
+            verbose,
+            **kwargs,
+        )
+
+    @staticmethod
+    def load_data(
+        path: Optional[str] = "pandas",
+        name: Optional[str] = None,
+        data_dir: Optional[str] = "",
+        data_files: Optional[Union[str, Sequence[str]]] = None,
+        split: Optional[str] = "train",
+        filetype: Optional[str] = "",
+        concatenate: Optional[bool] = False,
+        use_cached: bool = False,
+        verbose: Optional[bool] = False,
+        **kwargs,
+    ) -> Union[Dict[str, pd.DataFrame], Dict[str, DatasetType]]:
         return Datasets.load_data(
-            filename,
-            base_dir=base_dir,
-            verbose=verbose,
-            filetype=filetype,
+            path,
+            name,
+            data_dir,
+            data_files,
+            split,
+            filetype,
+            concatenate,
+            use_cached,
+            verbose,
             **kwargs,
         )
 
     @staticmethod
-    def concat_data(
-        data,
-        columns=None,
-        add_key_as_name=False,
-        name_column="_name_",
-        ignore_index=True,
-        verbose=False,
+    def get_data_files(
+        data_files: Optional[
+            Union[str, Sequence[str], Mapping[str, Union[str, Sequence[str]]]]
+        ] = None,
+        data_dir: Optional[str] = None,
+        split: str = "",
+        recursive: bool = True,
+        use_cached: bool = False,
+        verbose: bool = False,
+        **kwargs,
+    ) -> Union[List[str], Dict[str, List[str]]]:
+        return Datasets.get_data_files(
+            data_files, data_dir, split, recursive, use_cached, verbose, **kwargs
+        )
+
+    @staticmethod
+    def load_dataframes(
+        data_files: Union[str, Sequence[str]],
+        data_dir: str = "",
+        filetype: str = "",
+        split: str = "",
+        concatenate: bool = False,
+        ignore_index: bool = False,
+        use_cached: bool = False,
+        verbose: bool = False,
+        **kwargs,
+    ) -> Union[Dict[str, pd.DataFrame], pd.DataFrame]:
+        """Load data from a file or a list of files"""
+        return Datasets.load_dataframes(
+            data_files,
+            data_dir,
+            filetype,
+            split,
+            concatenate,
+            ignore_index,
+            use_cached,
+            verbose,
+            **kwargs,
+        )
+
+    @staticmethod
+    def load_dataframe(
+        data_file: str,
+        data_dir: str = "",
+        filetype: str = "parquet",
+        columns: Optional[Sequence[str]] = None,
+        index_col: Union[str, int, Sequence[str], Sequence[int], None] = None,
+        verbose: bool = False,
+        **kwargs,
+    ) -> pd.DataFrame:
+        """Load a dataframe from a file"""
+        return Datasets.load_dataframe(
+            data_file, data_dir, filetype, columns, index_col, verbose, **kwargs
+        )
+
+    @staticmethod
+    def save_dataframe(
+        data: pd.DataFrame,
+        data_file: str,
+        data_dir: str = "",
+        columns: Optional[Sequence[str]] = None,
+        index: bool = False,
+        filetype: str = "parquet",
+        suffix: str = "",
+        verbose: bool = False,
         **kwargs,
     ):
-        return Datasets.concat_data(
+        """Save data to a file"""
+        Datasets.save_dataframes(
             data,
-            columns=columns,
-            add_key_as_name=add_key_as_name,
-            name_column=name_column,
-            ignore_index=ignore_index,
-            verbose=verbose,
+            data_file,
+            data_dir,
+            columns,
+            index,
+            filetype,
+            suffix,
+            verbose,
+            **kwargs,
+        )
+
+    @staticmethod
+    def save_dataframes(
+        data: Union[pd.DataFrame, dict],
+        data_file: str,
+        data_dir: str = "",
+        columns: Optional[Sequence[str]] = None,
+        index: bool = False,
+        filetype: str = "parquet",
+        suffix: str = "",
+        verbose: bool = False,
+        **kwargs,
+    ):
+        """Save data to a file"""
+        Datasets.save_dataframes(
+            data,
+            data_file,
+            data_dir,
+            columns,
+            index,
+            filetype,
+            suffix,
+            verbose,
             **kwargs,
         )
 
     @staticmethod
-    def is_dataframe(data):
+    def is_dataframe(data) -> bool:
         return Datasets.is_dataframe(data)
 
     @staticmethod
     def to_datetime(data, _format=None, _columns=None, **kwargs):
         return Datasets.to_datetime(data, _format, _columns, **kwargs)
 
     @staticmethod
@@ -873,33 +1188,33 @@
         Examples:
             >>> expand_posix_vars("$HOME")
             '/home/user'
             >>> expand_posix_vars("$HOME/$USER", {"USER": "testuser"})
             '/home/user/testuser'
 
         """
-        return Envs.expand_posix_vars(posix_expr, context=context)
+        return ENVs.expand_posix_vars(posix_expr, context=context)
 
     @staticmethod
     def get_osenv(key: str = "", default: Union[str, None] = None) -> Any:
         """Get the value of an environment variable or return the default value"""
-        return Envs.get_osenv(key, default=default)
+        return ENVs.get_osenv(key, default=default)
 
     @staticmethod
     def set_osenv(key, value):
-        return Envs.set_osenv(key, value)
+        return ENVs.set_osenv(key, value)
 
     @staticmethod
     def load_dotenv(
         override: bool = False,
         dotenv_dir: str = "",
         dotenv_filename: str = ".env",
         verbose: bool = False,
     ) -> None:
-        Envs.load_dotenv(
+        ENVs.load_dotenv(
             override=override,
             dotenv_filename=dotenv_filename,
             dotenv_dir=dotenv_dir,
             verbose=verbose,
         )
 
     ###############################
@@ -909,30 +1224,30 @@
     def ensure_import_module(
         name: str,
         libpath: str,
         liburi: str,
         specname: str = "",
         syspath: str = "",
     ):
-        return Packages.ensure_import_module(name, libpath, liburi, specname, syspath)
+        return PKGs.ensure_import_module(name, libpath, liburi, specname, syspath)
 
     @staticmethod
     def pip(
         name: str,
         upgrade: bool = False,
         prelease: bool = False,
         editable: bool = False,
         quiet: bool = True,
         find_links: str = "",
         requirement: bool = False,
         force_reinstall: bool = False,
         verbose: bool = False,
         **kwargs,
     ):
-        return Packages.pip(
+        return PKGs.pip(
             name,
             upgrade,
             prelease,
             editable,
             quiet,
             find_links,
             requirement,
@@ -944,65 +1259,65 @@
     @staticmethod
     def pipu(
         prelease=False,
         quiet=False,
         force_reinstall=False,
         **kwargs,
     ):
-        return Packages.pip(
+        return PKGs.pip(
             name="hyfi",
             upgrade=True,
             prelease=prelease,
             quiet=quiet,
             force_reinstall=force_reinstall,
             **kwargs,
         )
 
     ###############################
     # Files functions
     ###############################
     @staticmethod
     def exists(a, *p):
-        return IOLibs.exists(a, *p)
+        return IOLIBs.exists(a, *p)
 
     @staticmethod
     def is_file(a, *p):
-        return IOLibs.is_file(a, *p)
+        return IOLIBs.is_file(a, *p)
 
     @staticmethod
     def is_dir(a, *p):
-        return IOLibs.is_dir(a, *p)
+        return IOLIBs.is_dir(a, *p)
 
     @staticmethod
     def mkdir(_path: str):
-        return IOLibs.mkdir(_path)
+        return IOLIBs.mkdir(_path)
 
     @staticmethod
     def join_path(a, *p):
-        return IOLibs.join_path(a, *p)
+        return IOLIBs.join_path(a, *p)
 
     @staticmethod
     def get_filepaths(
         filename_patterns: Union[str, PosixPath, WindowsPath],
         base_dir: Union[str, PosixPath, WindowsPath] = "",
         recursive: bool = True,
         verbose: bool = False,
         **kwargs,
     ):
-        return IOLibs.get_filepaths(
+        return IOLIBs.get_filepaths(
             filename_patterns,
             base_dir=base_dir,
             recursive=recursive,
             verbose=verbose,
             **kwargs,
         )
 
     @staticmethod
     def read(uri, mode="rb", encoding=None, head=None, **kwargs):
-        return IOLibs.read(uri, mode, encoding, head, **kwargs)
+        return IOLIBs.read(uri, mode, encoding, head, **kwargs)
 
     @staticmethod
     def copy(
         src: PathLikeType,
         dst: PathLikeType,
         follow_symlinks: bool = True,
     ):
@@ -1011,15 +1326,15 @@
         If you need to copy an entire directory (including all of its contents), or if you need to overwrite existing files in the destination directory, shutil.copy() would be a better choice.
 
         Args:
                 src: Path to the file or directory to be copied.
                 dst: Path to the destination directory. If the destination directory does not exist it will be created.
                 follow_symlinks: Whether or not symlinks should be followed
         """
-        IOLibs.copy(src, dst, follow_symlinks=follow_symlinks)
+        IOLIBs.copy(src, dst, follow_symlinks=follow_symlinks)
 
     @staticmethod
     def copyfile(
         src: PathLikeType,
         dst: PathLikeType,
         follow_symlinks: bool = True,
     ):
@@ -1028,15 +1343,15 @@
         If you want to copy a single file from one location to another, shutil.copyfile() is the appropriate function to use.
 
         Args:
                 src: Path to the file or directory to copy.
                 dst: Path to the destination file or directory. If the destination file already exists it will be overwritten.
                 follow_symlinks: Whether to follow symbolic links or not
         """
-        IOLibs.copyfile(src, dst, follow_symlinks=follow_symlinks)
+        IOLIBs.copyfile(src, dst, follow_symlinks=follow_symlinks)
 
     @staticmethod
     def cached_path(
         url_or_filename: str,
         extract_archive: bool = False,
         force_extract: bool = False,
         return_parent_dir: bool = False,
@@ -1057,33 +1372,33 @@
 
         Raises:
             ImportError: If the required libraries 'cached_path' and 'gdown' are not imported.
 
         Returns:
             str: Path to the cached file or its parent directory, depending on the 'return_parent_dir' parameter.
         """
-        return IOLibs.cached_path(
+        return IOLIBs.cached_path(
             url_or_filename,
             extract_archive=extract_archive,
             force_extract=force_extract,
             return_parent_dir=return_parent_dir,
             cache_dir=cache_dir,
             verbose=verbose,
         )
 
     ###############################
     # Utility functions
     ###############################
     @staticmethod
     def to_dateparm(_date, _format="%Y-%m-%d"):
-        return Funcs.to_dateparm(_date, _format)
+        return FUNCs.to_dateparm(_date, _format)
 
     @staticmethod
     def dict_product(dicts):
-        return Funcs.dict_product(dicts)
+        return FUNCs.dict_product(dicts)
 
     ###############################
     # GPU Utility functions
     ###############################
     @staticmethod
     def nvidia_smi():
         return nvidia_smi()
```

### Comparing `hyfi-0.9.1/src/hyfi/project/__init__.py` & `hyfi-1.0.0/src/hyfi/project/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,70 @@
 import os
 from pathlib import Path
 from typing import Union
 
-from pydantic import validator
+from pydantic import field_validator
 
 from hyfi.__global__ import __about__
+from hyfi.composer import BaseConfig
 from hyfi.dotenv import DotEnvConfig
-from hyfi.hydra import BaseConfig
 from hyfi.joblib import JobLibConfig
 from hyfi.path import PathConfig
-from hyfi.utils.logging import Logging
+from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
 class ProjectConfig(BaseConfig):
     """Project Config"""
 
-    config_name: str = "__init__"
-    config_group: str = "project"
+    _config_name_: str = "__init__"
+    _config_group_: str = "project"
     # Project Config
     project_name: str = "hyfi-project"
-    task_name: str = ""
     project_description: str = ""
     project_root: str = ""
     project_workspace_name: str = "workspace"
     global_hyfi_root: str = ""
     global_workspace_name: str = "workspace"
     num_workers: int = 1
     use_huggingface_hub: bool = False
     use_wandb: bool = False
     verbose: Union[bool, int] = False
     # Config Classes
     dotenv: DotEnvConfig = None  # type: ignore
     joblib: JobLibConfig = None  # type: ignore
     path: PathConfig = None  # type: ignore
 
-    class Config:
-        extra = "allow"
-        arbitrary_types_allowed = True
-
-    @validator("project_name", allow_reuse=True)
+    @field_validator("project_name")
     def _validate_project_name(cls, v):
         if v is None:
             raise ValueError("Project name must be specified.")
         return v
 
-    @validator("verbose", allow_reuse=True)
+    @field_validator("verbose")
     def _validate_verbose(cls, v):
         if isinstance(v, str):
             if v.lower() in {"true", "1"}:
                 v = True
             elif v.lower() in {"false", "0"}:
                 v = False
             else:
                 raise ValueError("verbose must be a boolean or a string of 0 or 1")
         return v
 
-    def initialize_configs(self, **config_kwargs):
-        super().initialize_configs(**config_kwargs)
+    def __init__(self, **config_kwargs):
+        super().__init__(**config_kwargs)
+        self.initialize()
 
+    def initialize(self):
         self.dotenv = DotEnvConfig()
-        self.path = PathConfig.parse_obj(self.__dict__["path"])
-        self.joblib = JobLibConfig.parse_obj(self.__dict__["joblib"])
 
         self.dotenv.HYFI_PROJECT_NAME = self.project_name
-        self.dotenv.HYFI_TASK_NAME = self.task_name
         self.dotenv.HYFI_PROJECT_DESC = self.project_description
         self.dotenv.HYFI_PROJECT_ROOT = self.project_root
         self.dotenv.HYFI_PROJECT_WORKSPACE_NAME = self.project_workspace_name
         self.dotenv.HYFI_GLOBAL_ROOT = self.global_hyfi_root
         self.dotenv.HYFI_GLOBAL_WORKSPACE_NAME = self.global_workspace_name
         self.dotenv.HYFI_NUM_WORKERS = self.num_workers
         self.dotenv.HYFI_VERBOSE = self.verbose
@@ -84,16 +78,15 @@
             raise ValueError("Path object not initialized")
         if self.dotenv is None:
             raise ValueError("DotEnv object not initialized")
 
         self.dotenv.WANDB_DIR = str(self.path.log_dir)
         project_name = self.project_name.replace("/", "-").replace("\\", "-")
         self.dotenv.WANDB_PROJECT = project_name
-        task_name = self.task_name.replace("/", "-").replace("\\", "-")
-        notebook_name = self.path.log_dir / f"{task_name}-nb"
+        notebook_name = self.path.log_dir / f"{project_name}-nb"
         notebook_name.mkdir(parents=True, exist_ok=True)
         self.dotenv.WANDB_NOTEBOOK_NAME = str(notebook_name)
         self.dotenv.WANDB_SILENT = str(not self.verbose)
         if self.use_wandb:
             try:
                 import wandb  # type: ignore
 
@@ -132,21 +125,29 @@
                 )
 
     @property
     def osenv(self):
         return os.environ
 
     @property
-    def project_workspace_dir(self):
-        if self.path is None:
-            raise ValueError("Path object not initialized")
-        _p = Path(self.path.project_workspace_root)
-        _p.mkdir(parents=True, exist_ok=True)
-        return _p.absolute()
+    def root_dir(self) -> Path:
+        return self.path.root_dir if self.path else Path(self.project_root)
 
     @property
-    def project_dir(self):
-        if self.path is None:
-            raise ValueError("Path object not initialized")
-        _p = Path(self.path.project_root)
-        _p.mkdir(parents=True, exist_ok=True)
-        return _p.absolute()
+    def workspace_dir(self):
+        return (
+            self.path.workspace_dir
+            if self.path
+            else self.root_dir / self.project_workspace_name
+        )
+
+    @property
+    def global_root_dir(self):
+        return self.path.global_root_dir if self.path else Path(self.global_hyfi_root)
+
+    @property
+    def global_workspace_dir(self):
+        return (
+            self.path.global_workspace_dir
+            if self.path
+            else self.global_root_dir / self.global_workspace_name
+        )
```

### Comparing `hyfi-0.9.1/src/hyfi/utils/contexts.py` & `hyfi-1.0.0/src/hyfi/utils/contexts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import os
 from contextlib import contextmanager
 from functools import partial
 from timeit import default_timer
 
-from hyfi.utils.funcs import Funcs
+from hyfi.utils.funcs import FUNCs
 
 
 def _elapser_timer(start):
     """A function that returns the elapsed time"""
     return default_timer() - start
 
 
@@ -32,19 +32,19 @@
 
 
 @contextmanager
 def change_directory(directory):
     """Change directory and change back to original directory"""
     original = os.path.abspath(os.getcwd())
 
-    Funcs.fancy_print(f" Change directory to {directory}")
+    FUNCs.fancy_print(f" Change directory to {directory}")
     os.chdir(directory)
     try:
         yield
 
     except Exception as e:
-        Funcs.fancy_print(f" Exception: {e}")
+        FUNCs.fancy_print(f" Exception: {e}")
         raise e
 
     finally:
-        Funcs.fancy_print(f" Change directory back to {original}")
+        FUNCs.fancy_print(f" Change directory back to {original}")
         os.chdir(original)
```

### Comparing `hyfi-0.9.1/src/hyfi/utils/datasets.py` & `hyfi-1.0.0/src/hyfi/utils/datasets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,139 +1,278 @@
 import os
-from typing import Any, Dict, Mapping, Optional, Sequence, Union
+from os import PathLike
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Union
 
+import datasets as hfds
 import pandas as pd
-from datasets import Dataset, load_dataset
+from datasets import Dataset
 from datasets.dataset_dict import DatasetDict, IterableDatasetDict
 from datasets.download.download_config import DownloadConfig
 from datasets.download.download_manager import DownloadMode
 from datasets.features import Features
+from datasets.info import DatasetInfo
 from datasets.iterable_dataset import IterableDataset
-from datasets.splits import Split
+from datasets.splits import NamedSplit, Split
 from datasets.tasks import TaskTemplate
 from datasets.utils.info_utils import VerificationMode
 from datasets.utils.version import Version
 
 from hyfi.utils.contexts import elapsed_timer
-from hyfi.utils.iolibs import IOLibs
-from hyfi.utils.logging import Logging
+from hyfi.utils.iolibs import IOLIBs
+from hyfi.utils.logging import LOGGING
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
+
+DatasetType = Union[Dataset, IterableDataset]
+DatasetLikeType = Union[Dataset, IterableDataset, DatasetDict, IterableDatasetDict]
 
 
 class Datasets:
     @staticmethod
     def is_dataframe(data: Any) -> bool:
         """Check if data is a pandas dataframe"""
         return isinstance(data, pd.DataFrame)
 
     @staticmethod
-    def concat_data(
-        data,
-        columns=None,
-        add_key_as_name: bool = False,
-        name_column: str = "_name_",
+    def concatenate_data(
+        data: Union[Dict[str, pd.DataFrame], Sequence[pd.DataFrame], List[DatasetType]],
+        columns: Optional[Sequence[str]] = None,
+        add_split_key_column: bool = False,
+        added_column_name: str = "_name_",
         ignore_index: bool = True,
+        axis: int = 0,
+        split: Optional[str] = None,
+        verbose: bool = False,
         **kwargs,
-    ):
+    ) -> Union[pd.DataFrame, DatasetType]:
+        # if data is a list of datasets, concatenate them
+        if isinstance(data, list) and isinstance(data[0], Dataset):
+            return Datasets.concatenate_datasets(
+                data,
+                axis=axis,
+                split=split,
+                **kwargs,
+            )
+        else:
+            return Datasets.concatenate_dataframes(
+                data,
+                columns=columns,
+                add_split_key_column=add_split_key_column,
+                added_column_name=added_column_name,
+                ignore_index=ignore_index,
+                axis=axis,
+                verbose=verbose,
+                **kwargs,
+            )
+
+    @staticmethod
+    def concatenate_dataframes(
+        data: Union[Dict[str, pd.DataFrame], Sequence[pd.DataFrame]],
+        columns: Optional[Sequence[str]] = None,
+        add_split_key_column: bool = False,
+        added_column_name: str = "_name_",
+        ignore_index: bool = True,
+        axis: int = 0,
+        verbose: bool = False,
+        **kwargs,
+    ) -> pd.DataFrame:
         """Concatenate dataframes"""
         if isinstance(data, dict):
-            logger.info(f"Concatenating {len(data)} dataframes")
             dfs = []
-            for df_name in data:
-                df_each = data[df_name]
-                if isinstance(columns, list):
-                    _columns = [c for c in columns if c in df_each.columns]
-                    df_each = df_each[_columns]
-                if add_key_as_name:
-                    df_each[name_column] = df_name
-                dfs.append(df_each)
-            return pd.concat(dfs, ignore_index=ignore_index) if dfs else None
-        elif isinstance(data, list):
-            logger.info(f"Concatenating {len(data)} dataframes")
-            return pd.concat(data, ignore_index=ignore_index) if len(data) > 0 else None
+            for split in data:
+                df = data[split]
+                if add_split_key_column:
+                    df[added_column_name] = split
+                dfs.append(df)
+            data = dfs
+        if add_split_key_column:
+            columns.append(added_column_name)
+        if isinstance(data, list):
+            if isinstance(columns, list):
+                _columns = [c for c in columns if c in df.columns]
+                data = [df[_columns] for df in data]
+            if verbose:
+                logger.info("Concatenating %s dataframes", len(data))
+            if len(data) > 0:
+                return pd.concat(data, ignore_index=ignore_index, axis=axis)
+            else:
+                raise ValueError("No dataframes to concatenate")
         else:
             logger.warning("Warning: data is not a dict")
             return data
 
     @staticmethod
     def load_data(
-        filename,
-        base_dir=None,
-        filetype=None,
-        verbose=False,
+        path: Optional[str] = "pandas",
+        name: Optional[str] = None,
+        data_dir: Optional[str] = "",
+        data_files: Optional[Union[str, Sequence[str]]] = None,
+        split: Optional[str] = None,
+        filetype: Optional[str] = "",
+        concatenate: Optional[bool] = False,
+        use_cached: bool = False,
+        verbose: Optional[bool] = False,
         **kwargs,
-    ):
+    ) -> Union[Dict[str, pd.DataFrame], Dict[str, DatasetType]]:
         """Load data from a file or a list of files"""
-        concatenate = kwargs.pop("concatenate", False)
-        ignore_index = kwargs.pop("ignore_index", False)
-        if filename is not None:
-            filename = str(filename)
-
-        if filename.startswith("http"):
-            if not filetype:
-                filetype = filename.split(".")[-1]
-            if filetype not in ["csv", "parquet"]:
-                raise ValueError("`file` should be a csv or a parquet file.")
-            kwargs["filetype"] = filetype
-            return Datasets.load_dataframe(filename, verbose=verbose, **kwargs)
-
-        if base_dir:
-            filepaths = IOLibs.get_filepaths(filename, base_dir)
+        if path in ["dataframe", "df", "pandas"]:
+            if data := Datasets.load_dataframes(
+                data_files,
+                data_dir=data_dir,
+                filetype=filetype,
+                split=split,
+                concatenate=concatenate,
+                use_cached=use_cached,
+                verbose=verbose,
+                **kwargs,
+            ):
+                return data if isinstance(data, dict) else {split: data}
+            else:
+                return {}
         else:
-            filepaths = IOLibs.get_filepaths(filename)
-        if verbose:
-            logger.info(f"Loading {len(filepaths)} dataframes from {filepaths}")
-
-        data = {
-            os.path.basename(f): Datasets.load_dataframe(
-                f, verbose=verbose, filetype=filetype, **kwargs
+            dset = Datasets.load_dataset(
+                path,
+                name=name,
+                data_dir=data_dir,
+                data_files=data_files,
+                split=split,
+                **kwargs,
             )
-            for f in filepaths
-        }
-        data = {k: v for k, v in data.items() if v is not None}
-        if len(data) == 1:
-            return list(data.values())[0]
-        elif len(filepaths) > 1:
+            split = split or "train"
+            if isinstance(dset, (Dataset, IterableDataset)):
+                return {split: dset}
             if concatenate:
-                return pd.concat(data.values(), ignore_index=ignore_index)
+                return {split: Datasets.concatenate_datasets(dset.values())}
             else:
-                return data
+                return {k: v for k, v in dset.items() if v is not None}
+
+    @staticmethod
+    def get_data_files(
+        data_files: Optional[
+            Union[str, Sequence[str], Mapping[str, Union[str, Sequence[str]]]]
+        ] = None,
+        data_dir: Optional[str] = None,
+        split: str = "",
+        recursive: bool = True,
+        use_cached: bool = False,
+        verbose: bool = False,
+        **kwargs,
+    ) -> Union[List[str], Dict[str, List[str]]]:
+        if isinstance(data_files, dict):
+            return {
+                name: IOLIBs.get_filepaths(
+                    files,
+                    data_dir,
+                    recursive=recursive,
+                    use_cached=use_cached,
+                    verbose=verbose,
+                    **kwargs,
+                )
+                for name, files in data_files.items()
+            }
+        filepaths = IOLIBs.get_filepaths(
+            data_files,
+            data_dir,
+            recursive=recursive,
+            use_cached=use_cached,
+            verbose=verbose,
+            **kwargs,
+        )
+        return {split: filepaths} if split else filepaths
+
+    @staticmethod
+    def load_dataframes(
+        data_files: Union[str, Sequence[str]],
+        data_dir: str = "",
+        filetype: str = "",
+        split: str = "",
+        concatenate: bool = False,
+        ignore_index: bool = False,
+        use_cached: bool = False,
+        verbose: bool = False,
+        **kwargs,
+    ) -> Union[Dict[str, pd.DataFrame], pd.DataFrame]:
+        """Load data from a file or a list of files"""
+        if not data_files:
+            logger.warning("No data_files provided")
+            return {}
+
+        filepaths = Datasets.get_data_files(
+            data_files,
+            data_dir,
+            split=split,
+            use_cached=use_cached,
+            verbose=verbose,
+            **kwargs,
+        )
+
+        if isinstance(filepaths, dict):
+            data = {
+                name: pd.concat(
+                    [
+                        Datasets.load_dataframe(
+                            f, verbose=verbose, filetype=filetype, **kwargs
+                        )
+                        for f in files
+                    ],
+                    ignore_index=ignore_index,
+                )
+                for name, files in filepaths.items()
+            }
+            data = {k: v for k, v in data.items() if v is not None}
+            return data
         else:
-            logger.warning(f"No files found for {filename}")
-            return None
+            data = {
+                os.path.basename(f): Datasets.load_dataframe(
+                    f, verbose=verbose, filetype=filetype, **kwargs
+                )
+                for f in filepaths
+            }
+            data = {k: v for k, v in data.items() if v is not None}
+            if len(data) == 1:
+                data = list(data.values())[0]
+            elif len(data) > 1:
+                if concatenate or split:
+                    data = pd.concat(data.values(), ignore_index=ignore_index)
+            else:
+                logger.warning(f"No files found for {data_files}")
+                return None
+            return {split: data} if split else data
 
     @staticmethod
     def load_dataframe(
-        filename: str,
-        base_dir: str = "",
-        columns: list = None,  # type: ignore
-        index_col=None,
+        data_file: str,
+        data_dir: str = "",
+        filetype: str = "parquet",
+        columns: Optional[Sequence[str]] = None,
+        index_col: Union[str, int, Sequence[str], Sequence[int], None] = None,
         verbose: bool = False,
         **kwargs,
-    ) -> Union[pd.DataFrame, None]:
+    ) -> pd.DataFrame:
         """Load a dataframe from a file"""
         dtype = kwargs.pop("dtype", None)
         if isinstance(dtype, list):
             dtype = {k: "str" for k in dtype}
         parse_dates = kwargs.pop("parse_dates", False)
 
-        filetype = kwargs.pop("filetype", None) or "parquet"
-        if filename.startswith("http"):
-            filepath = filename
+        if data_file.startswith("http"):
+            filepath = data_file
         else:
-            fileinfo = os.path.splitext(filename)
-            filename = fileinfo[0]
-            filetype = fileinfo[1] if len(fileinfo) > 1 else filetype
-            filetype = "." + filetype.replace(".", "")
-            filename = f"{filename}{filetype}"
-            filepath = os.path.join(base_dir, filename) if base_dir else filename
+            filepath = os.path.join(data_dir, data_file) if data_dir else data_file
             if not os.path.exists(filepath):
                 logger.warning(f"File {filepath} does not exist")
-                return None
+                raise FileNotFoundError(f"File {filepath} does not exist")
+        filetype = (
+            data_file.split(".")[-1]
+            if data_file.split(".")[-1] in ["csv", "tsv", "parquet"]
+            else filetype
+        )
+        filetype = filetype.replace(".", "")
+        if filetype not in ["csv", "tsv", "parquet"]:
+            raise ValueError("`file` should be a csv or a parquet file.")
         if verbose:
             logger.info(f"Loading data from {filepath}")
         with elapsed_timer(format_time=True) as elapsed:
             if "csv" in filetype or "tsv" in filetype:
                 delimiter = kwargs.pop("delimiter", "\t") if "tsv" in filetype else None
                 data = pd.read_csv(
                     filepath,
@@ -153,47 +292,47 @@
                 columns = [c for c in columns if c in data.columns]
                 data = data[columns]
             if verbose:
                 logger.info(" >> elapsed time to load data: %s", elapsed())
         return data
 
     @staticmethod
-    def save_data(
+    def save_dataframes(
         data: Union[pd.DataFrame, dict],
-        filename: str,
-        base_dir: str = "",
-        columns=None,
+        data_file: str,
+        data_dir: str = "",
+        columns: Optional[Sequence[str]] = None,
         index: bool = False,
-        filetype="parquet",
+        filetype: str = "parquet",
         suffix: str = "",
         verbose: bool = False,
         **kwargs,
     ):
         """Save data to a file"""
-        if filename is None:
+        if data_file is None:
             raise ValueError("filename must be specified")
-        fileinfo = os.path.splitext(filename)
-        filename = fileinfo[0]
+        fileinfo = os.path.splitext(data_file)
+        data_file = fileinfo[0]
         filetype = fileinfo[1] if len(fileinfo) > 1 else filetype
         filetype = "." + filetype.replace(".", "")
         if suffix:
-            filename = f"{filename}-{suffix}{filetype}"
+            data_file = f"{data_file}-{suffix}{filetype}"
         else:
-            filename = f"{filename}{filetype}"
-        filepath = os.path.join(base_dir, filename) if base_dir else filename
-        base_dir = os.path.dirname(filepath)
-        filename = os.path.basename(filepath)
-        os.makedirs(base_dir, exist_ok=True)
+            data_file = f"{data_file}{filetype}"
+        filepath = os.path.join(data_dir, data_file) if data_dir else data_file
+        data_dir = os.path.dirname(filepath)
+        data_file = os.path.basename(filepath)
+        os.makedirs(data_dir, exist_ok=True)
 
         if isinstance(data, dict):
             for k, v in data.items():
-                Datasets.save_data(
+                Datasets.save_dataframes(
                     v,
-                    filename,
-                    base_dir=base_dir,
+                    data_file,
+                    data_dir=data_dir,
                     columns=columns,
                     index=index,
                     filetype=filetype,
                     suffix=k,
                     verbose=verbose,
                     **kwargs,
                 )
@@ -296,14 +435,50 @@
             exclude=exclude,
             columns=columns,
             coerce_float=coerce_float,
             nrows=nrows,
         )
 
     @staticmethod
+    def concatenate_datasets(
+        dsets: List[DatasetType],
+        info: Optional[DatasetInfo] = None,
+        split: Optional[NamedSplit] = None,
+        axis: int = 0,
+    ) -> DatasetType:
+        """
+        Converts a list of [`Dataset`] with the same schema into a single [`Dataset`].
+
+        Args:
+            dsets (`List[datasets.Dataset]`):
+                List of Datasets to concatenate.
+            info (`DatasetInfo`, *optional*):
+                Dataset information, like description, citation, etc.
+            split (`NamedSplit`, *optional*):
+                Name of the dataset split.
+            axis (`{0, 1}`, defaults to `0`):
+                Axis to concatenate over, where `0` means over rows (vertically) and `1` means over columns
+                (horizontally).
+
+                <Added version="1.6.0"/>
+
+        Example:
+
+        ```py
+        >>> ds3 = concatenate_datasets([ds1, ds2])
+        ```
+        """
+        return hfds.concatenate_datasets(
+            dsets=dsets,
+            info=info,
+            split=split,
+            axis=axis,
+        )
+
+    @staticmethod
     def load_dataset(
         path: str,
         name: Optional[str] = None,
         data_dir: Optional[str] = None,
         data_files: Optional[
             Union[str, Sequence[str], Mapping[str, Union[str, Sequence[str]]]]
         ] = None,
@@ -500,15 +675,15 @@
         Load an image dataset with the `ImageFolder` dataset builder:
 
         ```py
         >>> from datasets import load_dataset
         >>> ds = load_dataset('imagefolder', data_dir='/path/to/images', split='train')
         ```
         """
-        return load_dataset(
+        return hfds.load_dataset(
             path=path,
             name=name,
             data_dir=data_dir,
             data_files=data_files,
             split=split,
             cache_dir=cache_dir,
             features=features,
@@ -522,7 +697,36 @@
             use_auth_token=use_auth_token,
             task=task,
             streaming=streaming,
             num_proc=num_proc,
             storage_options=storage_options,
             **config_kwargs,
         )
+
+    @staticmethod
+    def save_to_disk(
+        dset,
+        dataset_path: PathLike,
+        max_shard_size: Optional[Union[str, int]] = None,
+        num_shards: Optional[int] = None,
+        num_proc: Optional[int] = None,
+        storage_options: Optional[dict] = None,
+    ):
+        dset.save_to_disk(
+            dataset_path=dataset_path,
+            max_shard_size=max_shard_size,
+            num_shards=num_shards,
+            num_proc=num_proc,
+            storage_options=storage_options,
+        )
+
+    @staticmethod
+    def load_from_disk(
+        dataset_path: str,
+        keep_in_memory: Optional[bool] = None,
+        storage_options: Optional[dict] = None,
+    ) -> Union[Dataset, DatasetDict]:
+        return hfds.load_from_disk(
+            dataset_path=dataset_path,
+            keep_in_memory=keep_in_memory,
+            storage_options=storage_options,
+        )
```

### Comparing `hyfi-0.9.1/src/hyfi/utils/envs.py` & `hyfi-1.0.0/src/hyfi/utils/envs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Environment variable utilities"""
 import os
 from collections import defaultdict
 from pathlib import Path
 from string import Template
-from typing import Any, Union
+from typing import Any, Dict, Union
 
 import dotenv
 import hydra
 
-from hyfi.utils.iolibs import IOLibs
-from hyfi.utils.logging import Logging
+from hyfi.utils.iolibs import IOLIBs
+from hyfi.utils.logging import LOGGING
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
-class Envs:
+class ENVs:
     @staticmethod
     def getcwd():
         """Get the original working directory before Hydra changed it.
 
         This function tries to call the `get_original_cwd` function from the `hydra.utils` module,
         which returns the original working directory if it exists. If the `get_original_cwd` function
         raises a `ValueError` exception, it means that Hydra did not change the working directory,
@@ -90,15 +90,15 @@
             dotenv_dir: Directory to look for. env file ( default cwd )
             dotenv_filename: Name of. env file to look for
             verbose: Print debug information to console
 
         Returns:
             None or a Path object for the. env file
         """
-        dotenv_dir = dotenv_dir or Envs.getcwd()
+        dotenv_dir = dotenv_dir or ENVs.getcwd()
         dotenv_path = Path(dotenv_dir, dotenv_filename)
         # Load. env files and directories.
         if dotenv_path.is_file():
             dotenv.load_dotenv(
                 dotenv_path=dotenv_path, verbose=verbose, override=override
             )
             os.environ["DOTENV_PATH"] = str(dotenv_path)
@@ -138,31 +138,37 @@
                     logger.info("No .env file found in %s", dotenv_path)
                 else:
                     logger.debug("No .env file found in %s", dotenv_path)
 
     @staticmethod
     def get_osenv(key: str = "", default: Union[str, None] = None) -> Any:
         """Get the value of an environment variable or return the default value"""
-        Envs.load_dotenv()
+        ENVs.load_dotenv()
         return os.environ.get(key, default) if key else os.environ
 
     @staticmethod
     def set_osenv(key: str, value: Any) -> None:
         """Set the value of an environment variable"""
-        if value and IOLibs.is_dir(value):
+        if value and IOLIBs.is_dir(value):
             value = os.path.abspath(value)
         if pre_val := os.environ.get(key):
             logger.info("Overwriting %s=%s with %s", key, pre_val, value)
         else:
             logger.info("Setting %s=%s", key, value)
         os.environ[key] = value
 
     @staticmethod
-    def check_and_set_osenv(key: str, value: Any) -> Any:
+    def check_and_set_osenv_var(key: str, value: Any) -> Any:
         """Check and set value to environment variable"""
         env_key = key.upper()
         if value is not None:
             old_value = os.getenv(env_key, "")
             if str(old_value).lower() != str(value).lower():
                 os.environ[env_key] = str(value)
                 logger.debug("Set environment variable %s=%s", env_key, str(value))
         return value
+
+    @staticmethod
+    def check_and_set_osenv_vars(values: Dict[str, Any]) -> Dict[str, Any]:
+        for k, v in values.items():
+            ENVs.check_and_set_osenv_var(k, v)
+        return values
```

### Comparing `hyfi-0.9.1/src/hyfi/utils/funcs.py` & `hyfi-1.0.0/src/hyfi/utils/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utility functions for hyfi"""
 import ast
 import itertools
 import re
 import sys
 from contextlib import suppress
-from typing import Any, List, Optional, TextIO, Type, Union
+from typing import Any, Dict, List, Optional, TextIO, Type, Union
 
 import chardet
 import colorama
 from pydantic import StrictBool
 
 from hyfi.utils.types import IntSeq
 
@@ -27,24 +27,28 @@
 
 INDENT = " " * 2
 HLINE = "-" * 42
 
 NO_VALUE: object = object()
 
 
-class Funcs:
+class FUNCs:
     @staticmethod
     def unescape_dict(d):
         """Unescape a dictionary"""
         return ast.literal_eval(repr(d).encode("utf-8").decode("unicode-escape"))
 
     @staticmethod
     def lower_case_with_underscores(string):
         """Converts 'CamelCased' to 'camel_cased'."""
-        return re.sub(r"\s+", "_", string.lower()).replace("-", "_")
+        return (
+            re.sub(r"\s+", "_", re.sub(r"(?<!^)(?=[A-Z])", "_", string).lower())
+            .replace("-", "_")
+            .replace("__", "_")
+        )
 
     @staticmethod
     def ordinal(num):
         """Return the ordinal of a number as a string."""
         return "%d%s" % (
             num,
             "tsnrhtdd"[(num // 10 % 10 != 1) * (num % 10 < 4) * num % 10 :: 4],
@@ -54,15 +58,15 @@
     def get_offset_ranges(count, num_workers):
         """Get offset ranges for parallel processing"""
         assert count > num_workers
         step_sz = int(count / num_workers)
         offset_ranges = [0]
         pv_cnt = 1
         for i in range(num_workers):
-            pv_cnt = count if i == num_workers - 1 else pv_cnt + step_sz
+            pv_cnt = count + 1 if i == num_workers - 1 else pv_cnt + step_sz
             offset_ranges.append(pv_cnt)
         return offset_ranges
 
     @staticmethod
     def fancy_print(*args, color=None, bold=False, **kwargs):
         """Print with color and bold"""
         if bold:
@@ -134,20 +138,20 @@
     def utf8len(s):
         """Return the length of a string in bytes"""
         return len(str(s).encode("utf-8"))
 
     @staticmethod
     def len_wospc(x):
         """Return the length of a string in bytes without spaces"""
-        return Funcs.utf8len(re.sub(r"\s", "", str(x)))
+        return FUNCs.utf8len(re.sub(r"\s", "", str(x)))
 
     @staticmethod
     def len_bytes(x):
         """Return the length of a string in bytes"""
-        return Funcs.utf8len(x)
+        return FUNCs.utf8len(x)
 
     @staticmethod
     def len_words(x):
         """Return the number of words in a string"""
         return len(x.split()) if isinstance(x, str) else 0
 
     @staticmethod
@@ -234,26 +238,26 @@
             return f"{module}.{t.__qualname__}"
         except AttributeError:
             return str(t)
 
     @staticmethod
     def readable_types_list(type_list: List[Type]) -> str:
         """Generates a useful-for-humans label for a list of types."""
-        return ", ".join(Funcs.human_readable_type_name(t) for t in type_list)
+        return ", ".join(FUNCs.human_readable_type_name(t) for t in type_list)
 
     @staticmethod
-    def dict_product(dicts):
+    def dict_product(dicts) -> List[Dict]:
         """
         >>> list(dict_product(dict(number=[1,2], character='ab')))
         [{'character': 'a', 'number': 1},
         {'character': 'a', 'number': 2},
         {'character': 'b', 'number': 1},
         {'character': 'b', 'number': 2}]
         """
-        return (dict(zip(dicts, x)) for x in itertools.product(*dicts.values()))
+        return [dict(zip(dicts, x)) for x in itertools.product(*dicts.values())]
 
     @staticmethod
     def printf(
         action: str,
         msg: Any = "",
         style: Optional[IntSeq] = None,
         indent: int = 10,
@@ -275,15 +279,15 @@
     @staticmethod
     def printf_exception(
         e: Exception, action: str, msg: str = "", indent: int = 0, quiet: bool = False
     ) -> None:
         """Print exception with common format."""
         if not quiet:
             print("", file=sys.stderr)
-            Funcs.printf(
+            FUNCs.printf(
                 action, msg=msg, style=Style.DANGER, indent=indent, file_=sys.stderr
             )
             print(HLINE, file=sys.stderr)
             print(e, file=sys.stderr)
             print(HLINE, file=sys.stderr)
 
     @staticmethod
```

### Comparing `hyfi-0.9.1/src/hyfi/utils/gpumon.py` & `hyfi-1.0.0/src/hyfi/utils/gpumon.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import contextlib
 import gc
 import os
 import time
 from threading import Thread
 
-from hyfi.utils.logging import Logging
+from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 try:
     import GPUtil  # type: ignore
 except ImportError:
     logger.debug("GPUtil not found. Please install it to use GPU utilities.")
```

### Comparing `hyfi-0.9.1/src/hyfi/utils/iolibs.py` & `hyfi-1.0.0/src/hyfi/utils/iolibs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 from pathlib import Path, PosixPath, WindowsPath
 from types import TracebackType
 from typing import Callable, List, Tuple, Union
 
 import gdown
 
 from hyfi.cached_path import _cached_path
-from hyfi.utils.logging import Logging
+from hyfi.utils.logging import LOGGING
 from hyfi.utils.types import PathLikeType
 
-logger = Logging.getLogger(__name__)
+logger = LOGGING.getLogger(__name__)
 
 
-class IOLibs:
+class IOLIBs:
     @staticmethod
     def is_valid_regex(expr: str) -> bool:
         """Check if a string is a valid regular expression"""
         try:
             if expr.startswith("r:"):
                 expr = expr[2:]
             else:
@@ -39,66 +39,77 @@
     @staticmethod
     def glob_re(
         pattern: str,
         base_dir: str,
         recursive: bool = False,
     ) -> list:
         """Glob files matching a regular expression"""
-        if IOLibs.is_valid_regex(pattern):
+        if IOLIBs.is_valid_regex(pattern):
             pattern = pattern[2:]
             rpattern = re.compile(pattern)  # type: ignore
             files = []
             if recursive:
-                for dirpath, dirnames, filenames in os.walk(base_dir):
+                for dirpath, _, filenames in os.walk(base_dir):
                     files += [
                         os.path.join(dirpath, file)
                         for file in filenames
                         if rpattern.search(file)
                     ]
             else:
                 files = [
                     os.path.join(base_dir, file)
                     for file in os.listdir(base_dir)
                     if rpattern.search(file)
                 ]
         else:
-            file = os.path.join(base_dir, pattern) if base_dir else pattern
+            file = os.path.join(base_dir, pattern)
             files = glob(file, recursive=recursive)
         return files
 
     @staticmethod
     def get_filepaths(
         filename_patterns: Union[List[PathLikeType], PathLikeType],
         base_dir: Union[str, PosixPath, WindowsPath] = "",
         recursive: bool = True,
+        use_cached: bool = False,
         verbose: bool = False,
         **kwargs,
     ) -> List[str]:
         """Get a list of filepaths from a list of filename patterns"""
         if filename_patterns is None:
             raise ValueError("filename_patterns must be specified")
         if isinstance(filename_patterns, (PosixPath, WindowsPath)):
             filename_patterns = str(filename_patterns)
         if isinstance(filename_patterns, str):
             filename_patterns = [filename_patterns]
         filepaths = []
         base_dir = str(base_dir) if base_dir else ""
-        for file in filename_patterns:
-            file = str(file)
-            filepath = os.path.join(base_dir, file) if base_dir else file
-            if os.path.exists(filepath):
-                if Path(filepath).is_file():
-                    filepaths.append(filepath)
+        for f_pattern in filename_patterns:
+            f_pattern = str(f_pattern)
+            if f_pattern.startswith("http") and not use_cached:
+                filepaths.append(f_pattern)
             else:
-                if os.path.dirname(file) != "":
-                    _dir = os.path.dirname(file)
-                    file = os.path.basename(file)
-                    base_dir = os.path.join(base_dir, _dir) if base_dir else _dir
-                filepaths += IOLibs.glob_re(file, base_dir, recursive=recursive)
-        filepaths = [fp for fp in filepaths if Path(fp).is_file()]
+                if f_pattern.startswith("http"):
+                    filepath = IOLIBs.cached_path(f_pattern, **kwargs)
+                else:
+                    filepath = os.path.join(base_dir, f_pattern)
+                if os.path.exists(filepath):
+                    if Path(filepath).is_file():
+                        filepaths.append(filepath)
+                else:
+                    if os.path.dirname(f_pattern) != "":
+                        _dir = os.path.dirname(f_pattern)
+                        f_pattern = os.path.basename(f_pattern)
+                        base_dir = os.path.join(base_dir, _dir)
+                    filepaths += IOLIBs.glob_re(
+                        f_pattern, base_dir, recursive=recursive
+                    )
+        filepaths = [
+            fp for fp in filepaths if Path(fp).is_file() or fp.startswith("http")
+        ]
         if verbose:
             logger.info(f"Processing [{len(filepaths)}] files from {filename_patterns}")
 
         return filepaths
 
     @staticmethod
     def get_files_from_archive(archive_path: str, filetype: str = ""):
@@ -221,15 +232,15 @@
         Args:
                 src: Path to the file or directory to be copied.
                 dst: Path to the destination directory. If the destination directory does not exist it will be created.
                 follow_symlinks: Whether or not symlinks should be followed
         """
         src = str(src)
         dst = str(dst)
-        IOLibs.mkdir(dst)
+        IOLIBs.mkdir(dst)
         shutil.copy(src, dst, follow_symlinks=follow_symlinks)
         logger.info(f"copied {src} to {dst}")
 
     @staticmethod
     def copyfile(
         src: PathLikeType,
         dst: PathLikeType,
@@ -407,23 +418,23 @@
                 extract_archive,
                 force_extract,
                 cache_dir,
             )
 
         try:
             if url_or_filename.startswith("gd://"):
-                _path = IOLibs.cached_gdown(
+                _path = IOLIBs.cached_gdown(
                     url_or_filename,
                     verbose=verbose,
                     extract_archive=extract_archive,
                     force_extract=force_extract,
                     cache_dir=cache_dir,
                 )
             else:
-                if _cached_path is None or gdown is None:
+                if _cached_path is None:
                     raise ImportError(
                         "Error importing required libraries 'cached-path'. "
                         "Please install them using 'pip install cached-path' and try again."
                     )
 
                 if cache_dir:
                     cache_dir = str(Path(cache_dir) / "cached_path")
@@ -507,15 +518,15 @@
             cache_path = gdown.cached_download(
                 id=id_,
                 path=cache_path.as_posix(),
                 quiet=not verbose,
             )
 
             if extract_archive:
-                extraction_path, files = IOLibs.extractall(
+                extraction_path, files = IOLIBs.extractall(
                     cache_path, force_extract=force_extract
                 )
 
                 if not fname or not files:
                     return extraction_path
                 for f in files:
                     if f.endswith(fname):
@@ -546,8 +557,8 @@
     def cleanup(self):
         """Remove directory safely."""
         if self._finalizer.detach():  # type: ignore
             self._robust_cleanup(self.name)
 
     @staticmethod
     def _robust_cleanup(name):
-        shutil.rmtree(name, ignore_errors=False, onerror=IOLibs.handle_remove_readonly)
+        shutil.rmtree(name, ignore_errors=False, onerror=IOLIBs.handle_remove_readonly)
```

### Comparing `hyfi-0.9.1/src/hyfi/utils/logging.py` & `hyfi-1.0.0/src/hyfi/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Logging utilities"""
 import logging
 import os
 import sys
 import warnings
 
 
-class Logging:
+class LOGGING:
     @staticmethod
     def setLogger(
         level=None,
         force=True,
         filterwarnings_action="ignore",
         **kwargs,
     ) -> None:
```

### Comparing `hyfi-0.9.1/src/hyfi/utils/notebooks.py` & `hyfi-1.0.0/src/hyfi/utils/notebooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utilities for working with notebooks.""" ""
 import contextlib
 import logging
 import os
 import sys
 
-from hyfi.utils.envs import Envs
-from hyfi.utils.iolibs import IOLibs
+from hyfi.utils.envs import ENVs
+from hyfi.utils.iolibs import IOLIBs
 
 logger = logging.getLogger(__name__)
 
 
 class NBs:
     @staticmethod
     def is_notebook():
@@ -305,18 +305,18 @@
         import ipywidgets as widgets
 
         # from urllib.request import urlopen
 
         if filename is None:
             url = "https://assets.entelecheia.cc/img/placeholder.png"
             # img = urlopen(url).read()
-            img = IOLibs.read(url)
+            img = IOLIBs.read(url)
             _format = "png"
         else:
-            img = IOLibs.read(filename)
+            img = IOLIBs.read(filename)
             _format = format or filename.split(".")[-1]
         return widgets.Image(
             value=img,
             format=_format,
             width=width,
             height=height,
             **kwargs,
@@ -410,14 +410,14 @@
             drive.mount(mountpoint, force_remount=force_remount, timeout_ms=timeout_ms)
 
             if project_root:
                 if not project_root.startswith(
                     os.path.sep
                 ) and not project_root.startswith(".."):
                     project_root = os.path.join(mountpoint, project_root)
-                Envs.set_osenv("HYFI_PROJECT_ROOT", project_root)
+                ENVs.set_osenv("HYFI_PROJECT_ROOT", project_root)
                 logger.info(f"Setting HYFI_PROJECT_ROOT to {project_root}")
             if project_name:
-                Envs.set_osenv("HYFI_PROJECT_NAME", project_name)
+                ENVs.set_osenv("HYFI_PROJECT_NAME", project_name)
                 logger.info(f"Setting HYFI_PROJECT_NAME to {project_name}")
         except ImportError:
             logger.warning("Google Colab not detected.")
```

### Comparing `hyfi-0.9.1/PKG-INFO` & `hyfi-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.9.1
+Version: 1.0.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -12,26 +12,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ipython
 Requires-Dist: chardet (<=5.1.0)
 Requires-Dist: click (<=8.1.3)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
-Requires-Dist: datasets (<=2.13.0)
+Requires-Dist: datasets (<=2.13.1)
 Requires-Dist: filelock (>=3.4,<=3.12.2)
 Requires-Dist: gdown (<=4.6.6)
 Requires-Dist: huggingface-hub (>=0.8.1,<=0.15.1)
 Requires-Dist: hydra-colorlog (>=1.2.0,<2.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
+Requires-Dist: joblib (<=1.3.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (<=1.24.3)
+Requires-Dist: numpy (<=1.24.4)
 Requires-Dist: pandas (>=1.5.3,<=2.0.2)
 Requires-Dist: pathspec (>=0.9.0)
 Requires-Dist: pyarrow (<=12.0.1)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic-settings (>=2.0.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=12.1,<14.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi
 Description-Content-Type: text/markdown
@@ -65,15 +67,15 @@
 
 Hydra Fast Interface (Hydra and Pydantic based interface framework)
 
 - Documentation: [https://hyfi.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/hyfi][repo-url]
 - PyPI: [https://pypi.org/project/hyfi][pypi-url]
 
-HyFI is a framework for building interfaces for Python applications. It is based on [Hydra] and [Pydantic] and provides a set of tools to build interfaces for Python applications.
+HyFI is a framework for building interfaces for Python applications. It is based on [Hydra](https://hydra.cc) and [Pydantic](https://docs.pydantic.dev/latest/) and provides a set of tools to build interfaces for Python applications.
 
 ## Changelog
 
 See the [CHANGELOG] for more information.
 
 ## Contributing
```

