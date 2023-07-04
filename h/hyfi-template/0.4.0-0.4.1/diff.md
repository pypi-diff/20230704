# Comparing `tmp/hyfi_template-0.4.0.tar.gz` & `tmp/hyfi_template-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.4.0.tar", max compression
+gzip compressed data, was "hyfi_template-0.4.1.tar", max compression
```

## Comparing `hyfi_template-0.4.0.tar` & `hyfi_template-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1071 2023-07-02 10:37:47.927365 hyfi_template-0.4.0/LICENSE
--rw-r--r--   0        0        0     2215 2023-07-02 10:37:47.927365 hyfi_template-0.4.0/README.md
--rw-r--r--   0        0        0     3013 2023-07-02 10:38:13.819762 hyfi_template-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      286 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/__cli__.py
--rw-r--r--   0        0        0      379 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/__init__.py
--rw-r--r--   0        0        0       22 2023-07-02 10:38:13.763761 hyfi_template-0.4.0/src/hyfit/_version.py
--rw-r--r--   0        0        0        0 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/__init__.py
--rw-r--r--   0        0        0      249 2023-07-02 10:38:13.763761 hyfi_template-0.4.0/src/hyfit/conf/about/__init__.yaml
--rw-r--r--   0        0        0      435 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/path/__init__.yaml
--rw-r--r--   0        0        0      446 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/path/__task__.yaml
--rw-r--r--   0        0        0       76 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       72 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       74 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       65 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       67 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      119 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      237 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      242 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       92 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/project/__test__.yaml
--rw-r--r--   0        0        0       36 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/running/__init__.yaml
--rw-r--r--   0        0        0      178 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      321 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/task/__init__.yaml
--rw-r--r--   0        0        0      381 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0        0 2023-07-02 10:37:47.931365 hyfi_template-0.4.0/src/hyfit/py.typed
--rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 hyfi_template-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 01:09:19.699847 hyfi_template-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2215 2023-07-04 01:09:19.703848 hyfi_template-0.4.1/README.md
+-rw-r--r--   0        0        0     3012 2023-07-04 01:09:50.821982 hyfi_template-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-07-04 01:09:19.703848 hyfi_template-0.4.1/src/hyfit/__cli__.py
+-rw-r--r--   0        0        0      379 2023-07-04 01:09:19.703848 hyfi_template-0.4.1/src/hyfit/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-04 01:09:50.753978 hyfi_template-0.4.1/src/hyfit/_version.py
+-rw-r--r--   0        0        0        0 2023-07-04 01:09:19.703848 hyfi_template-0.4.1/src/hyfit/conf/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-04 01:09:50.753978 hyfi_template-0.4.1/src/hyfit/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      427 2023-07-04 01:09:19.703848 hyfi_template-0.4.1/src/hyfit/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 01:09:19.703848 hyfi_template-0.4.1/src/hyfit/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-04 01:09:19.703848 hyfi_template-0.4.1/src/hyfit/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      785 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      166 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      237 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      242 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      178 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      351 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      381 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 01:09:19.707848 hyfi_template-0.4.1/src/hyfit/py.typed
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 hyfi_template-0.4.1/PKG-INFO
```

### Comparing `hyfi_template-0.4.0/LICENSE` & `hyfi_template-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.0/README.md` & `hyfi_template-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.0/pyproject.toml` & `hyfi_template-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.4.0"
+version = "0.4.1"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfit", from = "src" }]
 
 [tool.poetry.scripts]
 hyfit = 'hyfit.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.16.3"
+hyfi = "^1.0.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `hyfi_template-0.4.0/src/hyfit/conf/copier/conf.yaml` & `hyfi_template-0.4.1/src/hyfit/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.0/src/hyfit/conf/dotenv/__init__.yaml` & `hyfi_template-0.4.1/src/hyfit/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.0/src/hyfit/conf/hydra/help/help.yaml` & `hyfi_template-0.4.1/src/hyfit/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.0/src/hyfit/conf/mode/__init__.yaml` & `hyfi_template-0.4.1/src/hyfit/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.0/src/hyfit/conf/project/__init__.yaml` & `hyfi_template-0.4.1/src/hyfit/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.0/PKG-INFO` & `hyfi_template-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.4.0
+Version: 0.4.1
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.16.3,<0.17.0)
+Requires-Dist: hyfi (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-template
 Description-Content-Type: text/markdown
 
 # HyFI Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

