# Comparing `tmp/dbt_quicksight_lineage-0.0.0.tar.gz` & `tmp/dbt_quicksight_lineage-0.0.2.tar.gz`

## Comparing `dbt_quicksight_lineage-0.0.0.tar` & `dbt_quicksight_lineage-0.0.2.tar`

### file list

```diff
@@ -1,73 +1,52 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.DS_Store
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.envrc
--rw-r--r--   0        0        0    21487 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.pylintrc
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.python-version
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.tagpr
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/requirements-dev.lock
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/requirements.lock
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.github/dependabot.yaml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.github/release.yml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.github/workflows/reviewdog.yaml
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.github/workflows/tagpr.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.vscode/launch.json
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.vscode/settings.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/.gitignore
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/.user.yml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/Makefile
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/README.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/dbt_project.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/docker-compose.yaml
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/fuga.json
--rw-r--r--   0        0        0    57618 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/hoge.json
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/profiles.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/analyses/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/macros/.gitkeep
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/models/example/my_first_dbt_model.sql
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/models/example/my_second_dbt_model.sql
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/models/example/schema.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/my-local/tests/.gitkeep
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/__main__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/cli/__init__.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/cli/main.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/cli/requires.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/core/__init__.py
--rw-r--r--   0        0        0    23636 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/core/app.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/core/dbt.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/core/test_app.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/core/test_dbt.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/describe_data_set_output.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/expected_schema.yml
--rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/manifest.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/modified_data_set.json
--rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/partial_parse.msgpack
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/schema.yml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/models/example/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/models/example/.gitkeep
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/models/example/schema.yml
--rw-r--r--   0        0        0   302245 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/my-local/manifest.json
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/.gitignore
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/.user.yml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/Makefile
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/README.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/dbt_project.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/docker-compose.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/profiles.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/analyses/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/macros/.gitkeep
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/models/example/schema.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/tests/data/test_project/tests/.gitkeep
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/LICENSE
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/README.md
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    21487 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.pylintrc
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.python-version
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.tagpr
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/requirements-dev.lock
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/requirements.lock
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/dependabot.yaml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/release.yml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/workflows/reviewdog.yaml
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/workflows/tagpr.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/docs/images/dataset.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/__main__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/__init__.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/main.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/requires.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/__init__.py
+-rw-r--r--   0        0        0    23636 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/app.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/dbt.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/core/test_app.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/core/test_dbt.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/describe_data_set_output.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/expected_schema.yml
+-rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/manifest.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/modified_data_set.json
+-rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/partial_parse.msgpack
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/schema.yml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/models/example/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/models/example/.gitkeep
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/.gitignore
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/.user.yml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/Makefile
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/README.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/dbt_project.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/docker-compose.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/profiles.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/analyses/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/macros/.gitkeep
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/models/example/schema.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/tests/data/test_project/tests/.gitkeep
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/README.md
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.0.2/PKG-INFO
```

### Comparing `dbt_quicksight_lineage-0.0.0/.pylintrc` & `dbt_quicksight_lineage-0.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/.tagpr` & `dbt_quicksight_lineage-0.0.2/.tagpr`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/requirements-dev.lock` & `dbt_quicksight_lineage-0.0.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/requirements.lock` & `dbt_quicksight_lineage-0.0.2/requirements.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/my-local/README.md` & `dbt_quicksight_lineage-0.0.2/tests/data/test_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/my-local/dbt_project.yml` & `dbt_quicksight_lineage-0.0.2/tests/data/test_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/my-local/models/example/schema.yml` & `dbt_quicksight_lineage-0.0.2/tests/data/expected_schema.yml`

 * *Files 24% similar despite different names*

```diff
@@ -3,37 +3,28 @@
 models:
   - name: my_first_dbt_model
     description: "A starter dbt model"
     meta:
       quicksight:
         logical_table_name: My First DBT Model
         data_sets:
-          - id: ac03c417-5111-43d2-83bc-ba376ff5a8ea
-            data_source_arn: arn:aws:quicksight:ap-northeast-1:572273579432:datasource/05745d42-1c46-432b-b66e-4b5d6d98e02c
+          - id: 00000000-0000-0000-0000-000000000000
+            data_source_arn: arn:aws:quicksight:ap-northeast-1:123456789012:datasource/00000000-0000-0000-0000-000000000000
     columns:
       - name: id
         description: "The primary key for this table"
         meta:
           quicksight:
             field_name: ID
             folder: Key
         tests:
           - unique
           - not_null
 
   - name: my_second_dbt_model
     description: "A starter dbt model"
-    meta:
-      quicksight:
-        logical_table_name: "My Second DBT Model"
-        data_sets:
-          - id: "11111111-1111-1111-1111-111111111111"
-            data_source: "arn:aws:quicksight:ap-northeast-1:123456789012:datasource/11111111-1111-1111-1111-111111111111"
     columns:
       - name: id
         description: "The primary key for this table"
-        meta:
-          quicksight:
-            field_name: "ID"
         tests:
           - unique
           - not_null
```

### Comparing `dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/cli/main.py` & `dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/cli/requires.py` & `dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/core/app.py` & `dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/app.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/src/dbt_quicksight_lineage/core/dbt.py` & `dbt_quicksight_lineage-0.0.2/src/dbt_quicksight_lineage/core/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/tests/core/test_app.py` & `dbt_quicksight_lineage-0.0.2/tests/core/test_app.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/tests/core/test_dbt.py` & `dbt_quicksight_lineage-0.0.2/tests/core/test_dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/tests/data/describe_data_set_output.json` & `dbt_quicksight_lineage-0.0.2/tests/data/describe_data_set_output.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/tests/data/manifest.json` & `dbt_quicksight_lineage-0.0.2/tests/data/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/tests/data/modified_data_set.json` & `dbt_quicksight_lineage-0.0.2/tests/data/modified_data_set.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/tests/data/partial_parse.msgpack` & `dbt_quicksight_lineage-0.0.2/tests/data/partial_parse.msgpack`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/tests/data/test_project/models/example/schema.yml` & `dbt_quicksight_lineage-0.0.2/tests/data/test_project/models/example/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/.gitignore` & `dbt_quicksight_lineage-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/LICENSE` & `dbt_quicksight_lineage-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.0.0/pyproject.toml` & `dbt_quicksight_lineage-0.0.2/pyproject.toml`

 * *Files identical despite different names*

