# Comparing `tmp/jupyterlab_translate-1.3.2.tar.gz` & `tmp/jupyterlab_translate-1.3.3.tar.gz`

## Comparing `jupyterlab_translate-1.3.2.tar` & `jupyterlab_translate-1.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/RELEASE.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/package.json
--rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/yarn.lock
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/.github/workflows/release_publish.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/__init__.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/api.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/cli.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/constants.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/contributors.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/converters.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/finder.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/gettext_extract.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/hooks.py
--rwxr-xr-x   0        0        0  3617291 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/index.js
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/plugin.py
--rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/pybabel_config.cfg
--rw-r--r--   0        0        0    22145 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/jupyterlab_translate/utils.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/tests/dummy_pkg.patch
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/tests/example.json
--rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/tests/test_hatch_hook.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/tests/test_utils.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/tests/dummy_pkg/locale/dummy_pkg.pot
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/tests/dummy_pkg/src/documentwidget.ts
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/LICENSE.txt
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/README.md
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/RELEASE.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/package.json
+-rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/yarn.lock
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/.github/workflows/release_publish.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/__init__.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/api.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/cli.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/constants.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/contributors.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/converters.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/finder.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/gettext_extract.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/hooks.py
+-rwxr-xr-x   0        0        0  3617291 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/index.js
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/plugin.py
+-rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/pybabel_config.cfg
+-rw-r--r--   0        0        0    22145 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/jupyterlab_translate/utils.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/tests/dummy_pkg.patch
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/tests/example.json
+-rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/tests/test_hatch_hook.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/tests/test_utils.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/tests/dummy_pkg/locale/dummy_pkg.pot
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/tests/dummy_pkg/src/documentwidget.ts
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/LICENSE.txt
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.3/PKG-INFO
```

### Comparing `jupyterlab_translate-1.3.2/CONTRIBUTING.md` & `jupyterlab_translate-1.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/package.json` & `jupyterlab_translate-1.3.3/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/yarn.lock` & `jupyterlab_translate-1.3.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/.github/workflows/release_publish.yml` & `jupyterlab_translate-1.3.3/.github/workflows/release_publish.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/.github/workflows/tests.yml` & `jupyterlab_translate-1.3.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/api.py` & `jupyterlab_translate-1.3.3/jupyterlab_translate/api.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/cli.py` & `jupyterlab_translate-1.3.3/jupyterlab_translate/cli.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/constants.py` & `jupyterlab_translate-1.3.3/jupyterlab_translate/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/contributors.py` & `jupyterlab_translate-1.3.3/jupyterlab_translate/contributors.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/converters.py` & `jupyterlab_translate-1.3.3/jupyterlab_translate/converters.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/finder.py` & `jupyterlab_translate-1.3.3/jupyterlab_translate/finder.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/index.js` & `jupyterlab_translate-1.3.3/jupyterlab_translate/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/plugin.py` & `jupyterlab_translate-1.3.3/jupyterlab_translate/plugin.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/jupyterlab_translate/utils.py` & `jupyterlab_translate-1.3.3/jupyterlab_translate/utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/tests/dummy_pkg.patch` & `jupyterlab_translate-1.3.3/tests/dummy_pkg.patch`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/tests/example.json` & `jupyterlab_translate-1.3.3/tests/example.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/tests/test_hatch_hook.py` & `jupyterlab_translate-1.3.3/tests/test_hatch_hook.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/tests/test_utils.py` & `jupyterlab_translate-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/tests/dummy_pkg/src/documentwidget.ts` & `jupyterlab_translate-1.3.3/tests/dummy_pkg/src/documentwidget.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/.gitignore` & `jupyterlab_translate-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/LICENSE.txt` & `jupyterlab_translate-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/README.md` & `jupyterlab_translate-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.2/pyproject.toml` & `jupyterlab_translate-1.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "click",
     "copier>=7.0.0",
     "copier-templates-extensions",
     "crowdin-api-client",
     "hatchling>=1.5",
     "jinja2-time",
     "polib",
+    "pydantic<2.0.0",
     "requests"
 ]
 
 [project.optional-dependencies]
 test = [
     "hatch",
     "pre-commit",
```

### Comparing `jupyterlab_translate-1.3.2/PKG-INFO` & `jupyterlab_translate-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-translate
-Version: 1.3.2
+Version: 1.3.3
 Summary: JupyterLab Language Pack Translations Helper
 Project-URL: homepage, https://github.com/jupyterlab/jupyterlab-translate
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2020 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -45,14 +45,15 @@
 Requires-Dist: copier-templates-extensions
 Requires-Dist: copier>=7.0.0
 Requires-Dist: crowdin-api-client
 Requires-Dist: hatchling>=1.5
 Requires-Dist: importlib-metadata>=4.8.3; python_version < '3.10'
 Requires-Dist: jinja2-time
 Requires-Dist: polib
+Requires-Dist: pydantic<2.0.0
 Requires-Dist: requests
 Provides-Extra: test
 Requires-Dist: hatch; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

