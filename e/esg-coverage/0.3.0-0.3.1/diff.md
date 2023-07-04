# Comparing `tmp/esg_coverage-0.3.0.tar.gz` & `tmp/esg_coverage-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esg_coverage-0.3.0.tar", max compression
+gzip compressed data, was "esg_coverage-0.3.1.tar", max compression
```

## Comparing `esg_coverage-0.3.0.tar` & `esg_coverage-0.3.1.tar`

### file list

```diff
@@ -1,60 +1,65 @@
--rw-r--r--   0        0        0     1071 2023-06-27 05:48:31.523220 esg_coverage-0.3.0/LICENSE
--rw-r--r--   0        0        0     2873 2023-06-27 05:48:31.523220 esg_coverage-0.3.0/README.md
--rw-r--r--   0        0        0     2996 2023-06-27 05:49:00.071653 esg_coverage-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/__cli__.py
--rw-r--r--   0        0        0      485 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/__init__.py
--rw-r--r--   0        0        0       22 2023-06-27 05:49:00.023653 esg_coverage-0.3.0/src/esgcov/_version.py
--rw-r--r--   0        0        0        0 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/__init__.py
--rw-r--r--   0        0        0      288 2023-06-27 05:49:00.023653 esg_coverage-0.3.0/src/esgcov/conf/about/__init__.yaml
--rw-r--r--   0        0        0      435 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      167 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0       83 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/path/__default__.yaml
--rw-r--r--   0        0        0     1719 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/path/__init__.yaml
--rw-r--r--   0        0        0      412 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/path/__task__.yaml
--rw-r--r--   0        0        0       76 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       72 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       74 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       85 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/__external__.yaml
--rw-r--r--   0        0        0      119 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       51 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/__instance__.yaml
--rw-r--r--   0        0        0       49 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/__lambda__.yaml
--rw-r--r--   0        0        0      237 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      108 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/preprocessing_esg_coverage.yaml
--rw-r--r--   0        0        0      107 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/preprocessing_esg_ratings.yaml
--rw-r--r--   0        0        0      242 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       92 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       19 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipeline/__test__.yaml
--rw-r--r--   0        0        0      706 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/pipeline/dataset_preprocessing.yaml
--rw-r--r--   0        0        0      742 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/project/__init__.yaml
--rw-r--r--   0        0        0      168 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/project/__test__.yaml
--rw-r--r--   0        0        0      200 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/project/esgcov.yaml
--rw-r--r--   0        0        0       36 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/running/__init__.yaml
--rw-r--r--   0        0        0      176 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      319 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/task/__init__.yaml
--rw-r--r--   0        0        0      311 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/task/__test__.yaml
--rw-r--r--   0        0        0      322 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/task/datasets.yaml
--rw-r--r--   0        0        0       97 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       97 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0       95 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/conf/workflow/datasets.yaml
--rw-r--r--   0        0        0        0 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/datasets/__init__.py
--rw-r--r--   0        0        0     3421 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/datasets/preprocessing.py
--rw-r--r--   0        0        0        0 2023-06-27 05:48:31.527220 esg_coverage-0.3.0/src/esgcov/py.typed
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 esg_coverage-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 07:33:40.418196 esg_coverage-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2873 2023-07-04 07:33:40.418196 esg_coverage-0.3.1/README.md
+-rw-r--r--   0        0        0     2995 2023-07-04 07:34:04.246021 esg_coverage-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/__cli__.py
+-rw-r--r--   0        0        0      379 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-04 07:34:04.206021 esg_coverage-0.3.1/src/esgcov/_version.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-04 07:34:04.206021 esg_coverage-0.3.1/src/esgcov/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      427 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      167 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0       83 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      785 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      166 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       85 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__external__.yaml
+-rw-r--r--   0        0        0       70 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       51 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__instance__.yaml
+-rw-r--r--   0        0        0       49 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__lambda__.yaml
+-rw-r--r--   0        0        0      236 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      108 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/preprocessing_esg_coverage.yaml
+-rw-r--r--   0        0        0      107 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/preprocessing_esg_ratings.yaml
+-rw-r--r--   0        0        0      241 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/__test__.yaml
+-rw-r--r--   0        0        0      388 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      706 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/dataset_preprocessing.yaml
+-rw-r--r--   0        0        0      744 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/project/__test__.yaml
+-rw-r--r--   0        0        0      200 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/project/esgcov.yaml
+-rw-r--r--   0        0        0       38 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      178 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      351 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      395 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/task/__test__.yaml
+-rw-r--r--   0        0        0      324 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/task/datasets.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0       97 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/workflow/datasets.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/datasets/__init__.py
+-rw-r--r--   0        0        0     3421 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/datasets/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/py.typed
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 esg_coverage-0.3.1/PKG-INFO
```

### Comparing `esg_coverage-0.3.0/LICENSE` & `esg_coverage-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/README.md` & `esg_coverage-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/pyproject.toml` & `esg_coverage-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "esg-coverage"
-version = "0.3.0"
+version = "0.3.1"
 description = "The Role of Analyst Coverage in Translating ESG Ratings into Stock Performance"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://esg-coverage.entelecheia.ai"
 repository = "https://github.com/entelecheia/esg-coverage"
 readme = "README.md"
 packages = [{ include = "esgcov", from = "src" }]
 
 [tool.poetry.scripts]
 esgcov = 'esgcov.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.15.0"
+hyfi = "^1.0.2"
 tabulate = "^0.9.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
```

### Comparing `esg_coverage-0.3.0/src/esgcov/conf/copier/conf.yaml` & `esg_coverage-0.3.1/src/esgcov/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/src/esgcov/conf/dotenv/__init__.yaml` & `esg_coverage-0.3.1/src/esgcov/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/src/esgcov/conf/hydra/help/help.yaml` & `esg_coverage-0.3.1/src/esgcov/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/src/esgcov/conf/mode/__init__.yaml` & `esg_coverage-0.3.1/src/esgcov/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/src/esgcov/conf/path/__default__.yaml` & `esg_coverage-0.3.1/src/esgcov/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/src/esgcov/conf/pipeline/dataset_preprocessing.yaml` & `esg_coverage-0.3.1/src/esgcov/conf/pipeline/dataset_preprocessing.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/src/esgcov/conf/project/__init__.yaml` & `esg_coverage-0.3.1/src/esgcov/conf/project/__init__.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
-config_name: __init__
+_config_name_: __init__
 project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
 project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
 project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
 global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
 global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
 num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
```

### Comparing `esg_coverage-0.3.0/src/esgcov/datasets/preprocessing.py` & `esg_coverage-0.3.1/src/esgcov/datasets/preprocessing.py`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.0/PKG-INFO` & `esg_coverage-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: esg-coverage
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Role of Analyst Coverage in Translating ESG Ratings into Stock Performance
 Home-page: https://esg-coverage.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.15.0,<0.16.0)
+Requires-Dist: hyfi (>=1.0.2,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/entelecheia/esg-coverage
 Description-Content-Type: text/markdown
 
 # The Analyst Pathway in ESG
 
 [![pypi-image]][pypi-url]
```

