# Comparing `tmp/dbt_quicksight_lineage-0.1.0.tar.gz` & `tmp/dbt_quicksight_lineage-0.1.1.tar.gz`

## Comparing `dbt_quicksight_lineage-0.1.0.tar` & `dbt_quicksight_lineage-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    21487 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.pylintrc
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.python-version
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.tagpr
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/requirements.lock
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/dependabot.yaml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/release.yml
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/workflows/reviewdog.yaml
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/workflows/tagpr.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/docs/images/dataset.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/__main__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/__init__.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/main.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/requires.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/__init__.py
--rw-r--r--   0        0        0    23636 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/app.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/dbt.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/core/test_app.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/core/test_dbt.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/describe_data_set_output.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/expected_schema.yml
--rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/manifest.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/modified_data_set.json
--rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/partial_parse.msgpack
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/schema.yml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/models/example/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/models/example/.gitkeep
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/.gitignore
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/.user.yml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/Makefile
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/README.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/dbt_project.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/docker-compose.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/profiles.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/analyses/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/macros/.gitkeep
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/models/example/schema.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/tests/data/test_project/tests/.gitkeep
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/LICENSE
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/README.md
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    21487 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.pylintrc
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.python-version
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.tagpr
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/dependabot.yaml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/release.yml
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/workflows/reviewdog.yaml
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/workflows/tagpr.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/docs/images/dataset.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/__main__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/__init__.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/main.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/requires.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/core/__init__.py
+-rw-r--r--   0        0        0    23636 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/core/app.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/core/dbt.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/core/test_app.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/core/test_dbt.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/describe_data_set_output.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/expected_schema.yml
+-rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/manifest.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/modified_data_set.json
+-rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/partial_parse.msgpack
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/schema.yml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/models/example/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/models/example/.gitkeep
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/.gitignore
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/.user.yml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/Makefile
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/README.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/dbt_project.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/docker-compose.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/profiles.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/analyses/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/macros/.gitkeep
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/models/example/schema.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/tests/data/test_project/tests/.gitkeep
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/README.md
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.1.1/PKG-INFO
```

### Comparing `dbt_quicksight_lineage-0.1.0/.pylintrc` & `dbt_quicksight_lineage-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/.tagpr` & `dbt_quicksight_lineage-0.1.1/.tagpr`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/requirements-dev.lock` & `dbt_quicksight_lineage-0.1.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/requirements.lock` & `dbt_quicksight_lineage-0.1.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/.github/workflows/reviewdog.yaml` & `dbt_quicksight_lineage-0.1.1/.github/workflows/reviewdog.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         run: |
           pip install -r requirements-dev.lock
       - uses: reviewdog/action-setup@v1
       - name: Run reviewdog
         env:
           REVIEWDOG_GITHUB_API_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
-          pylint --rcfile=.pylintrc src/dbt_quicksight_lineage tests" | reviewdog -efm="%f:%l:%c: %m" -reporter=github-pr-review
+          pylint --rcfile=.pylintrc src/dbt_quicksight_lineage tests | reviewdog -efm="%f:%l:%c: %m" -reporter=github-pr-review
   actionlint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3.1.0
       - uses: reviewdog/action-actionlint@v1
         with:
           fail_on_error: true
```

### Comparing `dbt_quicksight_lineage-0.1.0/.github/workflows/tagpr.yaml` & `dbt_quicksight_lineage-0.1.1/.github/workflows/tagpr.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     env:
       GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
     steps:
       - uses: actions/checkout@v3
       - id: tagpr
         uses: Songmu/tagpr@main
       - name: Adding summary
-        run: echo '### ${{steps.tagpr.outputs.tag}}' >> $GITHUB_STEP_SUMMARY
+        run: echo "### ${{steps.tagpr.outputs.tag}}" >> "$GITHUB_STEP_SUMMARY"
         if: ${{ steps.tagpr.outputs.tag != '' }}
       - uses: actions/checkout@v3
         if: ${{ steps.tagpr.outputs.tag != '' }}
         with:
           ref: ${{ steps.tagpr.outputs.tag }}
           fetch-depth: 0
       - name: Set up Python
```

### Comparing `dbt_quicksight_lineage-0.1.0/docs/images/dataset.png` & `dbt_quicksight_lineage-0.1.1/docs/images/dataset.png`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/main.py` & `dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/cli/requires.py` & `dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/app.py` & `dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/core/app.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/src/dbt_quicksight_lineage/core/dbt.py` & `dbt_quicksight_lineage-0.1.1/src/dbt_quicksight_lineage/core/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/core/test_app.py` & `dbt_quicksight_lineage-0.1.1/tests/core/test_app.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/core/test_dbt.py` & `dbt_quicksight_lineage-0.1.1/tests/core/test_dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/data/describe_data_set_output.json` & `dbt_quicksight_lineage-0.1.1/tests/data/describe_data_set_output.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/data/expected_schema.yml` & `dbt_quicksight_lineage-0.1.1/tests/data/expected_schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/data/manifest.json` & `dbt_quicksight_lineage-0.1.1/tests/data/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/data/modified_data_set.json` & `dbt_quicksight_lineage-0.1.1/tests/data/modified_data_set.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/data/partial_parse.msgpack` & `dbt_quicksight_lineage-0.1.1/tests/data/partial_parse.msgpack`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/data/test_project/README.md` & `dbt_quicksight_lineage-0.1.1/tests/data/test_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/data/test_project/dbt_project.yml` & `dbt_quicksight_lineage-0.1.1/tests/data/test_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/tests/data/test_project/models/example/schema.yml` & `dbt_quicksight_lineage-0.1.1/tests/data/test_project/models/example/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/.gitignore` & `dbt_quicksight_lineage-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/LICENSE` & `dbt_quicksight_lineage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.1.0/README.md` & `dbt_quicksight_lineage-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # dbt_quicksight_lineage
 
 [![PyPI - Version](https://img.shields.io/pypi/v/dbt-quicksight-lineage.svg)](https://pypi.org/project/dbt-quicksight-lineage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-quicksight-lineage.svg)](https://pypi.org/project/dbt-quicksight-lineage)
 
 -----
 PyPI: https://pypi.org/project/dbt-quicksight-lineage/
+Target DBT Version: 1.5.*
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
```

### Comparing `dbt_quicksight_lineage-0.1.0/pyproject.toml` & `dbt_quicksight_lineage-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,39 +12,36 @@
 keywords = []
 authors = [
   { name = "mashiike", email = "ikeda-masashi@kayac.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "click~=8.1.3",
-    "dbt-core~=1.5.2",
+    "dbt-core==1.5.*",
     "boto3~=1.26.164",
     "colorlog~=6.7.0",
     "ruamel.yaml~=0.17.32",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "hatch~=1.7.0",
     "mkdocs~=1.4.3",
-    "dbt-postgres~=1.5.2",
+    "dbt-postgres==1.5.*",
     "pytest~=7.4.0",
     "moto~=4.1.12",
     "dbt-redshift~=1.5.6",
     "mock~=5.0.2",
     "pylint~=2.17.4",
 ]
```

### Comparing `dbt_quicksight_lineage-0.1.0/PKG-INFO` & `dbt_quicksight_lineage-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 Metadata-Version: 2.1
 Name: dbt-quicksight-lineage
-Version: 0.1.0
+Version: 0.1.1
 Project-URL: Documentation, https://github.com/mashiike/dbt-quicksight-lineage#readme
 Project-URL: Issues, https://github.com/mashiike/dbt-quicksight-lineage/issues
 Project-URL: Source, https://github.com/mashiike/dbt-quicksight-lineage
 Author-email: mashiike <ikeda-masashi@kayac.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: boto3~=1.26.164
 Requires-Dist: click~=8.1.3
 Requires-Dist: colorlog~=6.7.0
-Requires-Dist: dbt-core~=1.5.2
+Requires-Dist: dbt-core==1.5.*
 Requires-Dist: ruamel-yaml~=0.17.32
 Description-Content-Type: text/markdown
 
 # dbt_quicksight_lineage
 
 [![PyPI - Version](https://img.shields.io/pypi/v/dbt-quicksight-lineage.svg)](https://pypi.org/project/dbt-quicksight-lineage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-quicksight-lineage.svg)](https://pypi.org/project/dbt-quicksight-lineage)
 
 -----
 PyPI: https://pypi.org/project/dbt-quicksight-lineage/
+Target DBT Version: 1.5.*
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
```

