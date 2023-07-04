# Comparing `tmp/uedition-0.6.0.tar.gz` & `tmp/uedition-0.6.1.tar.gz`

## Comparing `uedition-0.6.0.tar` & `uedition-0.6.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 uedition-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.6.0/tox.ini
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 uedition-0.6.0/.github/workflows/codestyle.yml
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.6.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.6.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.6.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/test_about.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/test_build.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/test_check.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/test_settings.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/basic/uEdition.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/empty/.gitkeep
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/invalid_core_files/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/invalid_core_files/en/_config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/invalid_core_files/en/_toc.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_core_files/uEdition.yaml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_files/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_files/references.bib
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_files/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_files/en/_config.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_files/en/_toc.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_files/en/intro.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_toc_root/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_toc_root/en/_config.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_toc_root/en/_toc.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_toc_root_file/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_toc_root_file/en/_config.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/missing_toc_root_file/en/_toc.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/references.bib
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/toc.yml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/uEdition.yaml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/de/_config.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/de/_toc.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/de/a-1-page.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/de/a-2-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/de/a-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/de/b-page.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/de/intro.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/en/_config.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/en/_toc.yml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/en/a-1-page.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/en/a-2-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/en/a-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/en/b-page.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/multilang/en/intro.md
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 uedition-0.6.0/tests/fixtures/yaml/uEdition.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/__about__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/__main__.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/settings.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/cli/__init__.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/cli/build.py
--rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/cli/check.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/cli/create.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/cli/language.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/cli/serve.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/cli/update.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/ext/__init__.py
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/ext/config.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/ext/language_switcher.js
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/ext/language_switcher.py
--rw-r--r--   0        0        0    11380 2020-02-02 00:00:00.000000 uedition-0.6.0/uedition/ext/tei.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.6.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.6.0/README.md
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 uedition-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 uedition-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 uedition-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.6.1/tox.ini
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 uedition-0.6.1/.github/workflows/codestyle.yml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.6.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.6.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/test_about.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/test_build.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/test_check.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/test_settings.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/basic/uEdition.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/empty/.gitkeep
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/invalid_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/invalid_core_files/en/_config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/invalid_core_files/en/_toc.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_files/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_files/references.bib
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_files/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_files/en/_config.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_files/en/_toc.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_files/en/intro.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_toc_root/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_toc_root/en/_config.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_toc_root/en/_toc.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_toc_root_file/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_toc_root_file/en/_config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/missing_toc_root_file/en/_toc.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/references.bib
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/toc.yml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/uEdition.yaml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/de/_config.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/de/_toc.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/de/a-1-page.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/de/a-2-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/de/a-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/de/b-page.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/de/intro.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/en/_config.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/en/_toc.yml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/en/a-1-page.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/en/a-2-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/en/a-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/en/b-page.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/multilang/en/intro.md
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 uedition-0.6.1/tests/fixtures/yaml/uEdition.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/__about__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/__main__.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/settings.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/cli/__init__.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/cli/build.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/cli/check.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/cli/create.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/cli/language.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/cli/serve.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/cli/update.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/ext/__init__.py
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/ext/config.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/ext/language_switcher.js
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/ext/language_switcher.py
+-rw-r--r--   0        0        0    11380 2020-02-02 00:00:00.000000 uedition-0.6.1/uedition/ext/tei.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.6.1/README.md
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 uedition-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 uedition-0.6.1/PKG-INFO
```

### Comparing `uedition-0.6.0/.github/workflows/coverage.yml` & `uedition-0.6.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/.github/workflows/release.yml` & `uedition-0.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/.github/workflows/tests.yml` & `uedition-0.6.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/tests/conftest.py` & `uedition-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/tests/test_build.py` & `uedition-0.6.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/tests/test_check.py` & `uedition-0.6.1/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/tests/test_settings.py` & `uedition-0.6.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/tests/fixtures/missing_files/references.bib` & `uedition-0.6.1/tests/fixtures/missing_files/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/tests/fixtures/missing_files/en/_config.yml` & `uedition-0.6.1/tests/fixtures/missing_files/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/tests/fixtures/multilang/references.bib` & `uedition-0.6.1/tests/fixtures/multilang/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/uedition/settings.py` & `uedition-0.6.1/uedition/settings.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/uedition/cli/__init__.py` & `uedition-0.6.1/uedition/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/uedition/cli/build.py` & `uedition-0.6.1/uedition/cli/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             elif isinstance(value, list):
                 output[key] = [walk(item) for item in value]
             else:
                 output[key] = value
         return output
 
     with open(path.join(lang["path"], "_toc.yml"), "w") as out_f:
-        safe_dump(walk(toc), out_f)
+        safe_dump(walk(toc), out_f, encoding="utf-8")
 
 
 def config_build(lang: dict) -> None:
     """Build the language-specific JupyterBook config based on the main config."""
     config = deepcopy(settings["jb_config"])
     config["author"] = settings["author"]["name"]
     # Set the language-specific title
@@ -131,15 +131,15 @@
     # Add the uEdition extension
     if "extra_extensions" not in config["sphinx"]:
         config["sphinx"]["extra_extensions"] = []
     if "uedition" not in config["sphinx"]["extra_extensions"]:
         config["sphinx"]["extra_extensions"].append("uedition")
 
     with open(path.join(lang["path"], "_config.yml"), "w") as out_f:
-        safe_dump(config, out_f)
+        safe_dump(config, out_f, encoding="utf-8")
 
 
 def full_build(lang: dict) -> None:
     """Run the full build process for a single language."""
     reload_settings()
     landing_build()
     toc_build(lang)
```

### Comparing `uedition-0.6.0/uedition/cli/check.py` & `uedition-0.6.1/uedition/cli/check.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/uedition/cli/language.py` & `uedition-0.6.1/uedition/cli/language.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/uedition/cli/serve.py` & `uedition-0.6.1/uedition/cli/serve.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/uedition/ext/config.py` & `uedition-0.6.1/uedition/ext/config.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/uedition/ext/language_switcher.js` & `uedition-0.6.1/uedition/ext/language_switcher.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,14 @@
 (function() {
     async function setup() {
         try {
-            const buttonContainer = document.querySelector('.article-header-buttons');
+            let buttonContainer = document.querySelector('.article-header-buttons');
+            if (!buttonContainer) {
+                buttonContainer = document.querySelector('.navbar-header-items__end .navbar-item.navbar-persistent--container');
+            }
             if (!buttonContainer) {
                 return;
             }
             // Create the dropdown container
             const container = document.createElement('div');
             container.classList.add('dropdown');
             // Create the button and its icon
```

### Comparing `uedition-0.6.0/uedition/ext/language_switcher.py` & `uedition-0.6.1/uedition/ext/language_switcher.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/uedition/ext/tei.py` & `uedition-0.6.1/uedition/ext/tei.py`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/LICENSE.txt` & `uedition-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/README.md` & `uedition-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/pyproject.toml` & `uedition-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uedition-0.6.0/PKG-INFO` & `uedition-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uEdition
-Version: 0.6.0
+Version: 0.6.1
 Project-URL: Documentation, https://github.com/unknown/uedition#readme
 Project-URL: Issues, https://github.com/unknown/uedition/issues
 Project-URL: Source, https://github.com/unknown/uedition
 Author-email: Mark Hall <mark.hall@work.room3b.eu>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

