# Comparing `tmp/opswork-0.2.0.tar.gz` & `tmp/opswork-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opswork-0.2.0.tar", last modified: Mon Jul  3 15:44:14 2023, max compression
+gzip compressed data, was "opswork-0.3.0.tar", last modified: Tue Jul  4 10:47:13 2023, max compression
```

## Comparing `opswork-0.2.0.tar` & `opswork-0.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.156586 opswork-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.148586 opswork-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-03 15:43:46.000000 opswork-0.2.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 15:43:46.000000 opswork-0.2.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 15:43:46.000000 opswork-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 15:43:46.000000 opswork-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-03 15:43:46.000000 opswork-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 15:43:46.000000 opswork-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-03 15:43:46.000000 opswork-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 15:43:46.000000 opswork-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-03 15:43:46.000000 opswork-0.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-03 15:43:46.000000 opswork-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-03 15:43:46.000000 opswork-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 15:43:46.000000 opswork-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-03 15:43:46.000000 opswork-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-03 15:44:14.156586 opswork-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-03 15:43:46.000000 opswork-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 15:43:46.000000 opswork-0.2.0/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-03 15:43:46.000000 opswork-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.144586 opswork-0.2.0/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/recipe/motd/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-03 15:43:46.000000 opswork-0.2.0/recipe/motd/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-03 15:43:46.000000 opswork-0.2.0/recipe/motd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-03 15:43:46.000000 opswork-0.2.0/recipe/nginx/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/recipe/ping/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-03 15:43:46.000000 opswork-0.2.0/recipe/ping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 15:43:46.000000 opswork-0.2.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-03 15:44:14.156586 opswork-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-03 15:43:46.000000 opswork-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.148586 opswork-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/src/opswork/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/src/opswork/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/command/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.156586 opswork-0.2.0/src/opswork/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.156586 opswork-0.2.0/src/opswork/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.156586 opswork-0.2.0/src/opswork/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-03 15:43:46.000000 opswork-0.2.0/src/opswork/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.152586 opswork-0.2.0/src/opswork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-03 15:44:14.000000 opswork-0.2.0/src/opswork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-03 15:44:14.000000 opswork-0.2.0/src/opswork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:44:14.000000 opswork-0.2.0/src/opswork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 15:44:14.000000 opswork-0.2.0/src/opswork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:44:13.000000 opswork-0.2.0/src/opswork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 15:44:14.000000 opswork-0.2.0/src/opswork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 15:44:14.000000 opswork-0.2.0/src/opswork.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.156586 opswork-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 15:43:46.000000 opswork-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:14.156586 opswork-0.2.0/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:46.000000 opswork-0.2.0/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-03 15:43:46.000000 opswork-0.2.0/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-03 15:43:46.000000 opswork-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.741717 opswork-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.741717 opswork-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-04 10:46:47.000000 opswork-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-04 10:46:47.000000 opswork-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-04 10:46:47.000000 opswork-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 10:46:47.000000 opswork-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-04 10:46:47.000000 opswork-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-04 10:46:47.000000 opswork-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 10:46:47.000000 opswork-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-04 10:46:47.000000 opswork-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-04 10:47:13.749717 opswork-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-04 10:46:47.000000 opswork-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 10:46:47.000000 opswork-0.3.0/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-04 10:46:47.000000 opswork-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.741717 opswork-0.3.0/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/recipe/motd/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 10:46:47.000000 opswork-0.3.0/recipe/motd/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-04 10:46:47.000000 opswork-0.3.0/recipe/motd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-04 10:46:47.000000 opswork-0.3.0/recipe/nginx/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/recipe/ping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 10:46:47.000000 opswork-0.3.0/recipe/ping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 10:46:47.000000 opswork-0.3.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-04 10:47:13.749717 opswork-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 10:46:47.000000 opswork-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.741717 opswork-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/command/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-04 10:46:47.000000 opswork-0.3.0/src/opswork/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/src/opswork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 10:47:13.000000 opswork-0.3.0/src/opswork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-04 10:46:47.000000 opswork-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:47:13.745717 opswork-0.3.0/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:46:47.000000 opswork-0.3.0/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-04 10:46:47.000000 opswork-0.3.0/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-04 10:46:47.000000 opswork-0.3.0/tox.ini
```

### Comparing `opswork-0.2.0/.github/workflows/release.yml` & `opswork-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/.gitignore` & `opswork-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/CODE_OF_CONDUCT.md` & `opswork-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/CONTRIBUTING.rst` & `opswork-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/LICENSE.txt` & `opswork-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/Makefile` & `opswork-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/PKG-INFO` & `opswork-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opswork
-Version: 0.2.0
+Version: 0.3.0
 Summary: OpsWork Swiss Knife.
 Home-page: https://github.com/clivern/opswork/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/clivern/opswork/
 Project-URL: Source, https://github.com/clivern/opswork/
@@ -149,12 +149,12 @@
     $ opswork host delete <host_name>
 
 
 15. Run a recipe towards a host
 
 .. code-block::
 
-    $ opswork recipe run <recipe_name> -h <host_name>
+    $ opswork recipe run <recipe_name> -h <host_name> -v key=value
 
     # Some examples
     $ opswork recipe run clivern/nginx -h example.com
     $ opswork recipe run clivern/ping -h localhost
```

### Comparing `opswork-0.2.0/README.rst` & `opswork-0.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -129,12 +129,12 @@
     $ opswork host delete <host_name>
 
 
 15. Run a recipe towards a host
 
 .. code-block::
 
-    $ opswork recipe run <recipe_name> -h <host_name>
+    $ opswork recipe run <recipe_name> -h <host_name> -v key=value
 
     # Some examples
     $ opswork recipe run clivern/nginx -h example.com
     $ opswork recipe run clivern/ping -h localhost
```

### Comparing `opswork-0.2.0/recipe/motd/recipe.yml` & `opswork-0.3.0/recipe/motd/recipe.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 vars:
-  version: v0.4
+  version: v0.3
 
 templates:
   motd.j2: motd.j2
 
 tasks:
   - name: check mandatory variables
     assert:
```

### Comparing `opswork-0.2.0/recipe/nginx/recipe.yml` & `opswork-0.3.0/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/recipe/ping/recipe.yml` & `opswork-0.3.0/recipe/ping/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/setup.cfg` & `opswork-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/setup.py` & `opswork-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/__init__.py` & `opswork-0.3.0/src/opswork/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/cli.py` & `opswork-0.3.0/src/opswork/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,16 +218,17 @@
     "-t",
     "--tag",
     "tag",
     type=click.STRING,
     default="",
     help="Hosts tag to run recipe towards",
 )
-def run(name, host, tag):
-    return Recipes().init().run(name, host, tag)
+@click.option("--var", "-v", multiple=True)
+def run(name, host, tag, var):
+    return Recipes().init().run(name, host, tag, var)
 
 
 # Manage configs command
 @click.group(help="Manage configs")
 def config():
     pass
```

### Comparing `opswork-0.2.0/src/opswork/command/__init__.py` & `opswork-0.3.0/src/opswork/command/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/command/configs.py` & `opswork-0.3.0/src/opswork/command/configs.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/command/hosts.py` & `opswork-0.3.0/src/opswork/command/hosts.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/command/random.py` & `opswork-0.3.0/src/opswork/command/random.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/command/recipes.py` & `opswork-0.3.0/src/opswork/command/recipes.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
     def delete(self, name):
         """Delete a Recipe"""
         self.database.delete_recipe(name)
 
         click.echo(f"Recipe with name {name} got deleted")
 
-    def run(self, name, host_name, tag):
+    def run(self, name, host_name, tag, var):
         """Run a Recipe towards a host"""
         hosts = []
         found = ""
         recipe = self.database.get_recipe(name)
 
         if recipe is None:
             raise click.ClickException(f"Recipe with name {name} not found")
@@ -171,14 +171,26 @@
                 if tag not in item.tags or found == item.id:
                     continue
                 hosts.append(item)
 
         if len(hosts) == 0:
             raise click.ClickException(f"No hosts matching!")
 
+        var_override = {}
+
+        for item in var:
+            if "=" not in item:
+                continue
+            data = item.split("=")
+            var_override[data[0]] = data[1]
+
         playbook = Playbook(
-            str(uuid.uuid4()), self._configs["cache"]["path"].rstrip("/"), hosts, recipe
+            str(uuid.uuid4()),
+            self._configs["cache"]["path"].rstrip("/"),
+            hosts,
+            recipe,
+            var_override,
         )
 
         playbook.build()
         playbook.run()
         playbook.cleanup()
```

### Comparing `opswork-0.2.0/src/opswork/exception/__init__.py` & `opswork-0.3.0/src/opswork/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/model/__init__.py` & `opswork-0.3.0/src/opswork/model/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/model/host.py` & `opswork-0.3.0/src/opswork/model/host.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/model/recipe.py` & `opswork-0.3.0/src/opswork/model/recipe.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/model/task.py` & `opswork-0.3.0/src/opswork/model/task.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/module/__init__.py` & `opswork-0.3.0/src/opswork/module/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/module/config.py` & `opswork-0.3.0/src/opswork/module/config.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/module/database.py` & `opswork-0.3.0/src/opswork/module/database.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/module/file_system.py` & `opswork-0.3.0/src/opswork/module/file_system.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/module/logger.py` & `opswork-0.3.0/src/opswork/module/logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/module/output.py` & `opswork-0.3.0/src/opswork/module/output.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/src/opswork/module/playbook.py` & `opswork-0.3.0/src/opswork/module/playbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,21 @@
 
 from opswork.module.file_system import FileSystem
 
 
 class Playbook:
     """Playbook Class"""
 
-    def __init__(self, id, cache, hosts, recipe):
+    def __init__(self, id, cache, hosts, recipe, var):
         """Class Constructor"""
         self._id = id
         self._cache = cache
         self._hosts = hosts
         self._recipe = recipe
+        self._var = var
         self._file_system = FileSystem()
 
     def build(self):
         """Build Playbook"""
         self._file_system.create_dirs("{}/{}".format(self._cache, self._id))
         self._file_system.create_dirs("{}/{}/cache".format(self._cache, self._id))
 
@@ -80,14 +81,18 @@
                 for key in item.keys():
                     self._file_system.write_file(
                         "{}/{}/{}".format(self._cache, self._id, key), item[key]
                     )
 
             del data["templates"]
 
+        # Override vars
+        if "vars" in data.keys():
+            data["vars"].update(self._var)
+
         base = {
             "hosts": "remote",
         }
 
         base.update(data)
         playbook = [base]
         self._file_system.write_file(
```

### Comparing `opswork-0.2.0/src/opswork.egg-info/PKG-INFO` & `opswork-0.3.0/src/opswork.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opswork
-Version: 0.2.0
+Version: 0.3.0
 Summary: OpsWork Swiss Knife.
 Home-page: https://github.com/clivern/opswork/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/clivern/opswork/
 Project-URL: Source, https://github.com/clivern/opswork/
@@ -149,12 +149,12 @@
     $ opswork host delete <host_name>
 
 
 15. Run a recipe towards a host
 
 .. code-block::
 
-    $ opswork recipe run <recipe_name> -h <host_name>
+    $ opswork recipe run <recipe_name> -h <host_name> -v key=value
 
     # Some examples
     $ opswork recipe run clivern/nginx -h example.com
     $ opswork recipe run clivern/ping -h localhost
```

### Comparing `opswork-0.2.0/src/opswork.egg-info/SOURCES.txt` & `opswork-0.3.0/src/opswork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/tests/__init__.py` & `opswork-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/tests/module/test_logger.py` & `opswork-0.3.0/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.2.0/tox.ini` & `opswork-0.3.0/tox.ini`

 * *Files identical despite different names*

