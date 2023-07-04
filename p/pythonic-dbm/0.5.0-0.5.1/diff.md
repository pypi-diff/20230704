# Comparing `tmp/pythonic-dbm-0.5.0.tar.gz` & `tmp/pythonic-dbm-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonic-dbm-0.5.0.tar", last modified: Mon Jul  3 18:12:27 2023, max compression
+gzip compressed data, was "pythonic-dbm-0.5.1.tar", last modified: Tue Jul  4 06:29:06 2023, max compression
```

## Comparing `pythonic-dbm-0.5.0.tar` & `pythonic-dbm-0.5.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/docs/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.723841 pythonic-dbm-0.5.0/docs/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/docs/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/overrides/assets/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/tutorial/field-types.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/tutorial/model-config.md
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/tutorial/models.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/tutorial/validators.md
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.723841 pythonic-dbm-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/database/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/database/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/data_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/data_types/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/inspect_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/models/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/models/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/fields/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/models/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/validators/builtin_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/validators/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/typing_extra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/database/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/models/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/models/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/validators/test_builtin_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/validators/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/test_inspect_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.518000 pythonic-dbm-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-04 06:29:06.518000 pythonic-dbm-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.505999 pythonic-dbm-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.505999 pythonic-dbm-0.5.1/docs/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.501999 pythonic-dbm-0.5.1/docs/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.505999 pythonic-dbm-0.5.1/docs/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/overrides/assets/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.505999 pythonic-dbm-0.5.1/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/tutorial/field-types.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/tutorial/model-config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/tutorial/models.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/docs/tutorial/validators.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-04 06:29:06.518000 pythonic-dbm-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.501999 pythonic-dbm-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.509999 pythonic-dbm-0.5.1/src/pydbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.509999 pythonic-dbm-0.5.1/src/pydbm/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.509999 pythonic-dbm-0.5.1/src/pydbm/database/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/database/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/database/data_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/database/data_types/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/inspect_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.509999 pythonic-dbm-0.5.1/src/pydbm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.509999 pythonic-dbm-0.5.1/src/pydbm/models/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/fields/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.509999 pythonic-dbm-0.5.1/src/pydbm/models/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/validators/builtin_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/models/validators/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/src/pydbm/typing_extra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.514000 pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-04 06:29:06.000000 pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-04 06:29:06.000000 pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:29:06.000000 pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-04 06:29:06.000000 pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 06:29:06.000000 pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:29:06.000000 pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.514000 pythonic-dbm-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.514000 pythonic-dbm-0.5.1/tests/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/database/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.514000 pythonic-dbm-0.5.1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.514000 pythonic-dbm-0.5.1/tests/models/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/fields/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/fields/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/fields/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/fields/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/fields/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:29:06.518000 pythonic-dbm-0.5.1/tests/models/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/validators/test_builtin_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/models/validators/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/test_inspect_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-04 06:28:47.000000 pythonic-dbm-0.5.1/tox.ini
```

### Comparing `pythonic-dbm-0.5.0/.gitignore` & `pythonic-dbm-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/.pre-commit-config.yaml` & `pythonic-dbm-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/LICENSE` & `pythonic-dbm-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/Makefile` & `pythonic-dbm-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/PKG-INFO` & `pythonic-dbm-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonic-dbm
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pydbm is a more pythonic way to use dbm.
 Home-page: https://pydbm.hakancelik.dev/
 Author: Hakan Celik
 Author-email: hakancelikdev@gmail.com
 License: GPL-3.0
 Project-URL: Documentation, https://pydbm.hakancelik.dev/
 Project-URL: Issues, https://github.com/hakancelikdev/pydbm/issues/
```

### Comparing `pythonic-dbm-0.5.0/README.md` & `pythonic-dbm-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/docs/CHANGELOG.md` & `pythonic-dbm-0.5.1/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 ## [Unreleased] - YYYY-MM-DD
 
+## [0.5.1] - 2023-07-04
+### Fixed
+- Fix objects.all and filter does not work properly [#46](https://github.com/hakancelikdev/pydbm/issues/46)
+
+
+
 ## [0.5.0] - 2023-07-03
 
 ### Added
 - EmptyModelError exception added
 - Implement UnnecessaryParamsError [#41](https://github.com/hakancelikdev/pydbm/pull/41)
   Throw an exception when a non-existent field is entered on the model.
 - Add count method to get model's data count. [#44](https://github.com/hakancelikdev/pydbm/pull/44)
```

### Comparing `pythonic-dbm-0.5.0/docs/CONTRIBUTING.md` & `pythonic-dbm-0.5.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/docs/index.md` & `pythonic-dbm-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/docs/overrides/assets/images/logo.png` & `pythonic-dbm-0.5.1/docs/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/docs/overrides/main.html` & `pythonic-dbm-0.5.1/docs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/docs/tutorial/field-types.md` & `pythonic-dbm-0.5.1/docs/tutorial/field-types.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/docs/tutorial/models.md` & `pythonic-dbm-0.5.1/docs/tutorial/models.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/docs/tutorial/validators.md` & `pythonic-dbm-0.5.1/docs/tutorial/validators.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/pyproject.toml` & `pythonic-dbm-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/setup.cfg` & `pythonic-dbm-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pythonic-dbm
-version = 0.5.0
+version = 0.5.1
 url = https://pydbm.hakancelik.dev/
 author = Hakan Celik
 author_email = hakancelikdev@gmail.com
 description = Pydbm is a more pythonic way to use dbm.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPL-3.0
```

### Comparing `pythonic-dbm-0.5.0/src/pydbm/__init__.py` & `pythonic-dbm-0.5.1/src/pydbm/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/database/data_types/base.py` & `pythonic-dbm-0.5.1/src/pydbm/database/data_types/base.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/database/data_types/types.py` & `pythonic-dbm-0.5.1/src/pydbm/database/data_types/types.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/database/manager.py` & `pythonic-dbm-0.5.1/src/pydbm/database/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     __slots__ = (
         "model",
         "table_name",
         "db_path",
         "db",
         DATABASE_HEADER_NAME,
-        "__key",
+        "_keys",
     )
 
     def __init__(self, *, model: typing.Type[DbmModel], table_name: str) -> None:  # TODO: table_name -> db_name
         self.model = model
         self.table_name = table_name
 
         self.db_path = DATABASE_PATH / f"{self.table_name}.{DATABASE_EXTENSION}"
@@ -92,25 +92,28 @@
         self.delete(pk=pk)
 
     def __contains__(self, pk: str) -> bool:
         with self as db:
             return pk in db
 
     def __iter__(self: Self) -> Self:
-        self.__key: bytes = DATABASE_HEADER_NAME.encode()  # NOTE: this is the first key in the database
+        with self as db:
+            # TODO: take key one by one to improve performance
+            self._keys: typing.Iterator[bytes] = iter(db.keys())
         return self
 
     def __next__(self) -> str:
-        with self as db:
-            self.__key: bytes | None = db.nextkey(self.__key)  # type: ignore
-
-        if self.__key is not None:
-            return self.__key.decode("utf-8")
+        _key: bytes | None = next(self._keys, None)
+        if _key is not None:
+            key: str = _key.decode("utf-8")
+            if key == DATABASE_HEADER_NAME:
+                return next(self)
+            return key
         else:
-            del self.__key
+            del self._keys
             raise StopIteration
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(model={self.model!r}, table_name={self.table_name!r})"
 
     def open(self):
         Path(DATABASE_PATH).mkdir(parents=True, exist_ok=True)
```

### Comparing `pythonic-dbm-0.5.0/src/pydbm/exceptions.py` & `pythonic-dbm-0.5.1/src/pydbm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/inspect_extra.py` & `pythonic-dbm-0.5.1/src/pydbm/inspect_extra.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/logging.py` & `pythonic-dbm-0.5.1/src/pydbm/logging.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/models/__init__.py` & `pythonic-dbm-0.5.1/src/pydbm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/models/base.py` & `pythonic-dbm-0.5.1/src/pydbm/models/base.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/models/fields/auto.py` & `pythonic-dbm-0.5.1/src/pydbm/models/fields/auto.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/models/fields/base.py` & `pythonic-dbm-0.5.1/src/pydbm/models/fields/base.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/models/meta.py` & `pythonic-dbm-0.5.1/src/pydbm/models/meta.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/models/validators/__init__.py` & `pythonic-dbm-0.5.1/src/pydbm/models/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/models/validators/builtin_types.py` & `pythonic-dbm-0.5.1/src/pydbm/models/validators/builtin_types.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/models/validators/compare.py` & `pythonic-dbm-0.5.1/src/pydbm/models/validators/compare.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pydbm/typing_extra.py` & `pythonic-dbm-0.5.1/src/pydbm/typing_extra.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/PKG-INFO` & `pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonic-dbm
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pydbm is a more pythonic way to use dbm.
 Home-page: https://pydbm.hakancelik.dev/
 Author: Hakan Celik
 Author-email: hakancelikdev@gmail.com
 License: GPL-3.0
 Project-URL: Documentation, https://pydbm.hakancelik.dev/
 Project-URL: Issues, https://github.com/hakancelikdev/pydbm/issues/
```

### Comparing `pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/SOURCES.txt` & `pythonic-dbm-0.5.1/src/pythonic_dbm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/database/test_manager.py` & `pythonic-dbm-0.5.1/tests/database/test_manager.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/fields/test_auto.py` & `pythonic-dbm-0.5.1/tests/models/fields/test_auto.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/fields/test_base.py` & `pythonic-dbm-0.5.1/tests/models/fields/test_base.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/fields/test_bool.py` & `pythonic-dbm-0.5.1/tests/models/fields/test_bool.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/fields/test_date.py` & `pythonic-dbm-0.5.1/tests/models/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/fields/test_numeric.py` & `pythonic-dbm-0.5.1/tests/models/fields/test_numeric.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/fields/test_sequence.py` & `pythonic-dbm-0.5.1/tests/models/fields/test_sequence.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/test_base.py` & `pythonic-dbm-0.5.1/tests/models/test_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -181,22 +181,25 @@
     model = Example.objects.create(str="str")
     model.update(str="new_str")
 
     assert model.str == "new_str"
     assert Example.objects.get(pk=model.pk).str == "new_str"
 
 
-def test_base_all(teardown_db):
+def test_base_all_and_filter(teardown_db):
     class Example(DbmModel):
-        str: str
-
-    assert Example.objects.create(str="str") == Example(str="str")
-    assert Example.objects.create(str="another str") == Example(str="another str")
+        field1: str
+        field2: int
 
-    assert list(Example.objects.all()) == [Example(str="another str"), Example(str="str")]
+    assert Example.objects.create(field1="str", field2=1) == Example(field1="str", field2=1)
+    assert Example.objects.create(field1="another str", field2=2) == Example(field1="another str", field2=2)
+    assert len(list(Example.objects.all())) == Example.objects.count()
+    assert list(Example.objects.all()) == [Example(field1="another str", field2=2), Example(field1="str", field2=1)]
+    assert list(Example.objects.filter()) == [Example(field1="another str", field2=2), Example(field1="str", field2=1)]
+    assert list(Example.objects.filter(field2=1)) == [Example(field1="str", field2=1)]
 
 
 def test_base_filter(teardown_db):
     class Example(DbmModel):
         str: str
 
     Example.objects.create(str="str")
```

### Comparing `pythonic-dbm-0.5.0/tests/models/test_meta.py` & `pythonic-dbm-0.5.1/tests/models/test_meta.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/validators/test_builtin_types.py` & `pythonic-dbm-0.5.1/tests/models/validators/test_builtin_types.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/models/validators/test_compare.py` & `pythonic-dbm-0.5.1/tests/models/validators/test_compare.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/test_exception.py` & `pythonic-dbm-0.5.1/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/test_inspect_extra.py` & `pythonic-dbm-0.5.1/tests/test_inspect_extra.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tests/test_logging.py` & `pythonic-dbm-0.5.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.5.0/tox.ini` & `pythonic-dbm-0.5.1/tox.ini`

 * *Files identical despite different names*

