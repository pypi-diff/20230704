# Comparing `tmp/django-better-repr-1.0.4.tar.gz` & `tmp/django-better-repr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-better-repr-1.0.4.tar", last modified: Sat Jul  1 16:33:49 2023, max compression
+gzip compressed data, was "django-better-repr-1.0.5.tar", last modified: Mon Jul  3 23:56:06 2023, max compression
```

## Comparing `django-better-repr-1.0.4.tar` & `django-better-repr-1.0.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.976361 django-better-repr-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.952361 django-better-repr-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.960361 django-better-repr-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-01 16:33:49.976361 django-better-repr-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.964361 django-better-repr-1.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.964361 django-better-repr-1.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/pyscaffold.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-01 16:33:49.980361 django-better-repr-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.956361 django-better-repr-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.964361 django-better-repr-1.0.4/src/django_better_repr/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.968361 django-better-repr-1.0.4/src/django_better_repr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.972361 django-better-repr-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.972361 django-better-repr-1.0.4/tests/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.972361 django-better-repr-1.0.4/tests/example_project/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.976361 django-better-repr-1.0.4/tests/example_project/myapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.976361 django-better-repr-1.0.4/tests/example_project/myapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/test_better_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.091435 django-better-repr-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.063435 django-better-repr-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.075435 django-better-repr-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-03 23:56:06.091435 django-better-repr-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.079435 django-better-repr-1.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.079435 django-better-repr-1.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/pyscaffold.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-03 23:56:06.091435 django-better-repr-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.067435 django-better-repr-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.083435 django-better-repr-1.0.5/src/django_better_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/src/django_better_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/src/django_better_repr/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/src/django_better_repr/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/src/django_better_repr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/src/django_better_repr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/src/django_better_repr/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.087435 django-better-repr-1.0.5/src/django_better_repr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-03 23:56:06.000000 django-better-repr-1.0.5/src/django_better_repr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-03 23:56:06.000000 django-better-repr-1.0.5/src/django_better_repr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:56:06.000000 django-better-repr-1.0.5/src/django_better_repr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:56:05.000000 django-better-repr-1.0.5/src/django_better_repr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 23:56:06.000000 django-better-repr-1.0.5/src/django_better_repr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 23:56:06.000000 django-better-repr-1.0.5/src/django_better_repr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.087435 django-better-repr-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.087435 django-better-repr-1.0.5/tests/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.087435 django-better-repr-1.0.5/tests/example_project/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/example_project/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/example_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/example_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/example_project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.091435 django-better-repr-1.0.5/tests/example_project/myapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/myapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/myapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/myapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:56:06.091435 django-better-repr-1.0.5/tests/example_project/myapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/myapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/myapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/myapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/myapp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/example_project/myapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tests/test_better_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-03 23:55:20.000000 django-better-repr-1.0.5/tox.ini
```

### Comparing `django-better-repr-1.0.4/.coveragerc` & `django-better-repr-1.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/.github/workflows/ci.yml` & `django-better-repr-1.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/.gitignore` & `django-better-repr-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/.pre-commit-config.yaml` & `django-better-repr-1.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/.readthedocs.yml` & `django-better-repr-1.0.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/CONTRIBUTING.rst` & `django-better-repr-1.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/LICENSE.txt` & `django-better-repr-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/PKG-INFO` & `django-better-repr-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: django-better-repr
-Version: 1.0.4
+Version: 1.0.5
 Summary: Django model reprs for humans!
 Home-page: https://github.com/MrSage/django-better-repr
 Author: Collin Sage
 Author-email: 3229549+MrSage@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://github.com/MrSage/django-better-repr
 Project-URL: Source, https://github.com/MrSage/django-better-repr
+Project-URL: Download, https://pypi.org/project/django-better-repr/#files
+Project-URL: Tracker, https://github.com/MrSage/django-better-repr/issues
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
@@ -24,30 +27,33 @@
         :target: https://cirrus-ci.com/github/<USER>/django-better-repr
     .. image:: https://readthedocs.org/projects/django-better-repr/badge/?version=latest
         :alt: ReadTheDocs
         :target: https://django-better-repr.readthedocs.io/en/stable/
     .. image:: https://img.shields.io/coveralls/github/<USER>/django-better-repr/main.svg
         :alt: Coveralls
         :target: https://coveralls.io/r/<USER>/django-better-repr
-    .. image:: https://img.shields.io/pypi/v/django-better-repr.svg
-        :alt: PyPI-Server
-        :target: https://pypi.org/project/django-better-repr/
     .. image:: https://img.shields.io/conda/vn/conda-forge/django-better-repr.svg
         :alt: Conda-Forge
         :target: https://anaconda.org/conda-forge/django-better-repr
     .. image:: https://pepy.tech/badge/django-better-repr/month
         :alt: Monthly Downloads
         :target: https://pepy.tech/project/django-better-repr
     .. image:: https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter
         :alt: Twitter
         :target: https://twitter.com/django-better-repr
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
+.. image:: https://img.shields.io/pypi/v/django-better-repr.svg
+    :alt: PyPI-Server
+    :target: https://pypi.org/project/django-better-repr/
+.. image:: https://pepy.tech/badge/django-better-repr/month
+    :alt: Monthly Downloads
+    :target: https://pepy.tech/project/django-better-repr
 
 |
 
 ==================
 django-better-repr
 ==================
```

### Comparing `django-better-repr-1.0.4/README.rst` & `django-better-repr-1.0.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,33 @@
         :target: https://cirrus-ci.com/github/<USER>/django-better-repr
     .. image:: https://readthedocs.org/projects/django-better-repr/badge/?version=latest
         :alt: ReadTheDocs
         :target: https://django-better-repr.readthedocs.io/en/stable/
     .. image:: https://img.shields.io/coveralls/github/<USER>/django-better-repr/main.svg
         :alt: Coveralls
         :target: https://coveralls.io/r/<USER>/django-better-repr
-    .. image:: https://img.shields.io/pypi/v/django-better-repr.svg
-        :alt: PyPI-Server
-        :target: https://pypi.org/project/django-better-repr/
     .. image:: https://img.shields.io/conda/vn/conda-forge/django-better-repr.svg
         :alt: Conda-Forge
         :target: https://anaconda.org/conda-forge/django-better-repr
     .. image:: https://pepy.tech/badge/django-better-repr/month
         :alt: Monthly Downloads
         :target: https://pepy.tech/project/django-better-repr
     .. image:: https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter
         :alt: Twitter
         :target: https://twitter.com/django-better-repr
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
+.. image:: https://img.shields.io/pypi/v/django-better-repr.svg
+    :alt: PyPI-Server
+    :target: https://pypi.org/project/django-better-repr/
+.. image:: https://pepy.tech/badge/django-better-repr/month
+    :alt: Monthly Downloads
+    :target: https://pepy.tech/project/django-better-repr
 
 |
 
 ==================
 django-better-repr
 ==================
```

### Comparing `django-better-repr-1.0.4/docs/Makefile` & `django-better-repr-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/docs/conf.py` & `django-better-repr-1.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/docs/index.rst` & `django-better-repr-1.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/manage.py` & `django-better-repr-1.0.5/manage.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/setup.cfg` & `django-better-repr-1.0.5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/MrSage/django-better-repr
 project_urls = 
 	Documentation = https://github.com/MrSage/django-better-repr
 	Source = https://github.com/MrSage/django-better-repr
+	Download = https://pypi.org/project/django-better-repr/#files
+	Tracker = https://github.com/MrSage/django-better-repr/issues
 platforms = any
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
+	Framework :: Django :: 4.2
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
```

### Comparing `django-better-repr-1.0.4/setup.py` & `django-better-repr-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/src/django_better_repr/__init__.py` & `django-better-repr-1.0.5/src/django_better_repr/__init__.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/src/django_better_repr/bases.py` & `django-better-repr-1.0.5/src/django_better_repr/bases.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/src/django_better_repr/config.py` & `django-better-repr-1.0.5/src/django_better_repr/config.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/src/django_better_repr.egg-info/PKG-INFO` & `django-better-repr-1.0.5/src/django_better_repr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: django-better-repr
-Version: 1.0.4
+Version: 1.0.5
 Summary: Django model reprs for humans!
 Home-page: https://github.com/MrSage/django-better-repr
 Author: Collin Sage
 Author-email: 3229549+MrSage@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://github.com/MrSage/django-better-repr
 Project-URL: Source, https://github.com/MrSage/django-better-repr
+Project-URL: Download, https://pypi.org/project/django-better-repr/#files
+Project-URL: Tracker, https://github.com/MrSage/django-better-repr/issues
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
@@ -24,30 +27,33 @@
         :target: https://cirrus-ci.com/github/<USER>/django-better-repr
     .. image:: https://readthedocs.org/projects/django-better-repr/badge/?version=latest
         :alt: ReadTheDocs
         :target: https://django-better-repr.readthedocs.io/en/stable/
     .. image:: https://img.shields.io/coveralls/github/<USER>/django-better-repr/main.svg
         :alt: Coveralls
         :target: https://coveralls.io/r/<USER>/django-better-repr
-    .. image:: https://img.shields.io/pypi/v/django-better-repr.svg
-        :alt: PyPI-Server
-        :target: https://pypi.org/project/django-better-repr/
     .. image:: https://img.shields.io/conda/vn/conda-forge/django-better-repr.svg
         :alt: Conda-Forge
         :target: https://anaconda.org/conda-forge/django-better-repr
     .. image:: https://pepy.tech/badge/django-better-repr/month
         :alt: Monthly Downloads
         :target: https://pepy.tech/project/django-better-repr
     .. image:: https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter
         :alt: Twitter
         :target: https://twitter.com/django-better-repr
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
+.. image:: https://img.shields.io/pypi/v/django-better-repr.svg
+    :alt: PyPI-Server
+    :target: https://pypi.org/project/django-better-repr/
+.. image:: https://pepy.tech/badge/django-better-repr/month
+    :alt: Monthly Downloads
+    :target: https://pepy.tech/project/django-better-repr
 
 |
 
 ==================
 django-better-repr
 ==================
```

### Comparing `django-better-repr-1.0.4/src/django_better_repr.egg-info/SOURCES.txt` & `django-better-repr-1.0.5/src/django_better_repr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/tests/example_project/__main__.py` & `django-better-repr-1.0.5/tests/example_project/__main__.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/tests/example_project/example_project/settings.py` & `django-better-repr-1.0.5/tests/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/tests/example_project/example_project/urls.py` & `django-better-repr-1.0.5/tests/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/tests/example_project/myapp/migrations/0001_initial.py` & `django-better-repr-1.0.5/tests/example_project/myapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/tests/example_project/myapp/models.py` & `django-better-repr-1.0.5/tests/example_project/myapp/models.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/tests/test_better_repr.py` & `django-better-repr-1.0.5/tests/test_better_repr.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.4/tox.ini` & `django-better-repr-1.0.5/tox.ini`

 * *Files identical despite different names*

