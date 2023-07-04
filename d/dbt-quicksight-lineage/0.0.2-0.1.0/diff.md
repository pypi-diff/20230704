# Comparing `tmp/dbt_quicksight_lineage-0.0.2.tar.gz` & `tmp/dbt_quicksight_lineage-0.1.0.tar.gz`

## Comparing `dbt_quicksight_lineage-0.0.2.tar` & `dbt_quicksight_lineage-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    21487 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.pylintrc
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.python-version
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.tagpr
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/requirements-dev.lock
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/requirements.lock
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/dependabot.yaml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/release.yml
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/workflows/reviewdog.yaml
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/workflows/tagpr.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/docs/images/dataset.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/__main__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/__init__.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/main.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/requires.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/__init__.py
--rw-r--r--   0        0        0    23636 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/app.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/dbt.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/core/test_app.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/core/test_dbt.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/describe_data_set_output.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/expected_schema.yml
--rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/manifest.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/modified_data_set.json
--rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/partial_parse.msgpack
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/schema.yml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/models/example/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/models/example/.gitkeep
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/.gitignore
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/.user.yml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/Makefile
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/README.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/dbt_project.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/docker-compose.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/profiles.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/analyses/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/macros/.gitkeep
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/models/example/schema.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/tests/.gitkeep
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/LICENSE
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/README.md
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    21487 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.pylintrc
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.python-version
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.tagpr
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/requirements.lock
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/release.yml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/workflows/reviewdog.yaml
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/workflows/tagpr.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/docs/images/dataset.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/__main__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/__init__.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/main.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/requires.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/__init__.py
+-rw-r--r--   0        0        0    23636 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/app.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/dbt.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/core/test_app.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/core/test_dbt.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/describe_data_set_output.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/expected_schema.yml
+-rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/manifest.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/modified_data_set.json
+-rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/partial_parse.msgpack
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/schema.yml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/models/example/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/models/example/.gitkeep
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/.gitignore
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/.user.yml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/Makefile
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/README.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/dbt_project.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/docker-compose.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/profiles.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/analyses/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/macros/.gitkeep
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/models/example/schema.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/tests/.gitkeep
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/README.md
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/PKG-INFO
```

### Comparing `dbt_quicksight_lineage-0.0.2/.pylintrc` & `dbt_quicksight_lineage-0.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/.tagpr` & `dbt_quicksight_lineage-0.1.0/.tagpr`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/requirements-dev.lock` & `dbt_quicksight_lineage-0.1.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/requirements.lock` & `dbt_quicksight_lineage-0.1.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/.github/workflows/reviewdog.yaml` & `dbt_quicksight_lineage-0.1.0/.github/workflows/reviewdog.yaml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/.github/workflows/tagpr.yaml` & `dbt_quicksight_lineage-0.1.0/.github/workflows/tagpr.yaml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/docs/images/dataset.png` & `dbt_quicksight_lineage-0.1.0/docs/images/dataset.png`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/main.py` & `dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/requires.py` & `dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/app.py` & `dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/app.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/dbt.py` & `dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/core/test_app.py` & `dbt_quicksight_lineage-0.1.0/tests/core/test_app.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/core/test_dbt.py` & `dbt_quicksight_lineage-0.1.0/tests/core/test_dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/data/describe_data_set_output.json` & `dbt_quicksight_lineage-0.1.0/tests/data/describe_data_set_output.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/data/expected_schema.yml` & `dbt_quicksight_lineage-0.1.0/tests/data/expected_schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/data/manifest.json` & `dbt_quicksight_lineage-0.1.0/tests/data/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/data/modified_data_set.json` & `dbt_quicksight_lineage-0.1.0/tests/data/modified_data_set.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/data/partial_parse.msgpack` & `dbt_quicksight_lineage-0.1.0/tests/data/partial_parse.msgpack`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/data/test_project/README.md` & `dbt_quicksight_lineage-0.1.0/tests/data/test_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/data/test_project/dbt_project.yml` & `dbt_quicksight_lineage-0.1.0/tests/data/test_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/tests/data/test_project/models/example/schema.yml` & `dbt_quicksight_lineage-0.1.0/tests/data/test_project/models/example/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/.gitignore` & `dbt_quicksight_lineage-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/LICENSE` & `dbt_quicksight_lineage-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/README.md` & `dbt_quicksight_lineage-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # dbt_quicksight_lineage
 
 [![PyPI - Version](https://img.shields.io/pypi/v/dbt-quicksight-lineage.svg)](https://pypi.org/project/dbt-quicksight-lineage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-quicksight-lineage.svg)](https://pypi.org/project/dbt-quicksight-lineage)
 
 -----
+PyPI: https://pypi.org/project/dbt-quicksight-lineage/
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
```

### Comparing `dbt_quicksight_lineage-0.0.2/pyproject.toml` & `dbt_quicksight_lineage-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.2/PKG-INFO` & `dbt_quicksight_lineage-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-quicksight-lineage
-Version: 0.0.2
+Version: 0.1.0
 Project-URL: Documentation, https://github.com/mashiike/dbt-quicksight-lineage#readme
 Project-URL: Issues, https://github.com/mashiike/dbt-quicksight-lineage/issues
 Project-URL: Source, https://github.com/mashiike/dbt-quicksight-lineage
 Author-email: mashiike <ikeda-masashi@kayac.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -26,14 +26,15 @@
 
 # dbt_quicksight_lineage
 
 [![PyPI - Version](https://img.shields.io/pypi/v/dbt-quicksight-lineage.svg)](https://pypi.org/project/dbt-quicksight-lineage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-quicksight-lineage.svg)](https://pypi.org/project/dbt-quicksight-lineage)
 
 -----
+PyPI: https://pypi.org/project/dbt-quicksight-lineage/
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
```

