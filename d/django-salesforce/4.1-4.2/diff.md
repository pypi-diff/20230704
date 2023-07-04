# Comparing `tmp/django-salesforce-4.1.tar.gz` & `tmp/django-salesforce-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-salesforce-4.1.tar", last modified: Thu Aug  4 22:40:04 2022, max compression
+gzip compressed data, was "django-salesforce-4.2.tar", last modified: Tue Jul  4 13:52:27 2023, max compression
```

## Comparing `django-salesforce-4.1.tar` & `django-salesforce-4.2.tar`

### file list

```diff
@@ -1,238 +1,244 @@
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.938191 django-salesforce-4.1/
--rw-r--r--   0 philchristensen   (502) staff       (20)      475 2021-10-11 22:52:49.000000 django-salesforce-4.1/.coveragerc
--rw-r--r--   0 philchristensen   (502) staff       (20)      263 2020-04-22 12:21:48.000000 django-salesforce-4.1/.editorconfig
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.916065 django-salesforce-4.1/.github/
--rw-r--r--   0 philchristensen   (502) staff       (20)       64 2020-04-22 12:21:48.000000 django-salesforce-4.1/.github/FUNDING.yml
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.916182 django-salesforce-4.1/.github/workflows/
--rw-r--r--   0 philchristensen   (502) staff       (20)     1909 2021-11-24 22:24:08.000000 django-salesforce-4.1/.github/workflows/main.yml
--rw-r--r--   0 philchristensen   (502) staff       (20)     1509 2022-08-04 22:27:47.000000 django-salesforce-4.1/.travis.yml
--rw-r--r--   0 philchristensen   (502) staff       (20)      604 2020-04-22 12:21:48.000000 django-salesforce-4.1/AUTHORS.md
--rw-r--r--   0 philchristensen   (502) staff       (20)    14219 2022-08-04 22:27:47.000000 django-salesforce-4.1/CHANGELOG.rst
--rw-r--r--   0 philchristensen   (502) staff       (20)     3217 2020-04-22 12:21:48.000000 django-salesforce-4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     1572 2020-04-22 12:21:48.000000 django-salesforce-4.1/CONTRIBUTING.md
--rwxr-xr-x   0 philchristensen   (502) staff       (20)     1099 2020-04-22 12:21:48.000000 django-salesforce-4.1/LICENSE.md
--rw-r--r--   0 philchristensen   (502) staff       (20)       67 2020-04-22 12:21:48.000000 django-salesforce-4.1/MANIFEST.in
--rw-r--r--   0 philchristensen   (502) staff       (20)    15343 2022-08-04 22:40:04.938337 django-salesforce-4.1/PKG-INFO
--rw-r--r--   0 philchristensen   (502) staff       (20)    14876 2022-08-04 22:27:47.000000 django-salesforce-4.1/README.rst
--rwxr-xr-x   0 philchristensen   (502) staff       (20)     2313 2021-10-11 22:52:49.000000 django-salesforce-4.1/coverage_run.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.916888 django-salesforce-4.1/django_salesforce.egg-info/
--rw-r--r--   0 philchristensen   (502) staff       (20)    15343 2022-08-04 22:40:04.000000 django-salesforce-4.1/django_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 philchristensen   (502) staff       (20)     6015 2022-08-04 22:40:04.000000 django-salesforce-4.1/django_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 philchristensen   (502) staff       (20)        1 2022-08-04 22:40:04.000000 django-salesforce-4.1/django_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 philchristensen   (502) staff       (20)        1 2020-05-08 14:00:41.000000 django-salesforce-4.1/django_salesforce.egg-info/not-zip-safe
--rw-r--r--   0 philchristensen   (502) staff       (20)       40 2022-08-04 22:40:04.000000 django-salesforce-4.1/django_salesforce.egg-info/requires.txt
--rw-r--r--   0 philchristensen   (502) staff       (20)       11 2022-08-04 22:40:04.000000 django-salesforce-4.1/django_salesforce.egg-info/top_level.txt
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.917014 django-salesforce-4.1/docs/
--rw-r--r--   0 philchristensen   (502) staff       (20)      956 2021-11-24 22:24:08.000000 django-salesforce-4.1/docs/details.rst
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      477 2020-04-22 12:21:48.000000 django-salesforce-4.1/manage.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      281 2020-05-08 13:55:20.000000 django-salesforce-4.1/mypy.ini
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      148 2021-10-11 22:52:49.000000 django-salesforce-4.1/pylint.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)    12617 2021-10-11 23:01:08.000000 django-salesforce-4.1/pylintrc
--rw-r--r--   0 philchristensen   (502) staff       (20)      133 2021-10-11 22:52:49.000000 django-salesforce-4.1/requirements.txt
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.918288 django-salesforce-4.1/salesforce/
--rw-r--r--   0 philchristensen   (502) staff       (20)      709 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      353 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      286 2020-05-08 13:55:20.000000 django-salesforce-4.1/salesforce/apps.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    26586 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/auth.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.920296 django-salesforce-4.1/salesforce/backend/
--rw-r--r--   0 philchristensen   (502) staff       (20)     2214 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/backend/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4465 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/backend/base.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      649 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/backend/client.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    24959 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/backend/compiler.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1466 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/backend/creation.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2690 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/backend/features.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2050 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/backend/indep.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    21617 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/backend/introspection.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2758 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/backend/manager.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2758 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/backend/models_lookups.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     6197 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/backend/models_sql_query.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4694 2021-11-24 22:24:08.000000 django-salesforce-4.1/salesforce/backend/operations.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     9938 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/backend/query.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1395 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/backend/schema.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      827 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/backend/test_helpers.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    17530 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/backend/utils.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      348 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/backend/validation.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.921004 django-salesforce-4.1/salesforce/dbapi/
--rw-r--r--   0 philchristensen   (502) staff       (20)     4265 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/dbapi/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1991 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/dbapi/common.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    40689 2021-11-24 22:24:08.000000 django-salesforce-4.1/salesforce/dbapi/driver.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     7963 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/dbapi/exceptions.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    14555 2021-11-24 22:24:08.000000 django-salesforce-4.1/salesforce/dbapi/subselect.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     5470 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/dbapi/test_helpers.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     8104 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/defaults.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    12816 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/fields.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.921122 django-salesforce-4.1/salesforce/management/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/management/__init__.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.921319 django-salesforce-4.1/salesforce/management/commands/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/management/commands/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     6842 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/management/commands/inspectdb.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    11076 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4823 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/models_extend.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2076 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/models_template.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     3887 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/router.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.921990 django-salesforce-4.1/salesforce/testrunner/
--rw-r--r--   0 philchristensen   (502) staff       (20)      143 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/__init__.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.923069 django-salesforce-4.1/salesforce/testrunner/example/
--rw-r--r--   0 philchristensen   (502) staff       (20)      143 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/example/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      531 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/example/admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      245 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/example/forms.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    18722 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/testrunner/example/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2049 2020-05-08 13:55:20.000000 django-salesforce-4.1/salesforce/testrunner/example/models_template.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.923314 django-salesforce-4.1/salesforce/testrunner/example/templates/
--rw-r--r--   0 philchristensen   (502) staff       (20)      444 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/example/templates/list-accounts.html
--rw-r--r--   0 philchristensen   (502) staff       (20)      717 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/example/templates/search-accounts.html
--rw-r--r--   0 philchristensen   (502) staff       (20)      363 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/example/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1260 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/example/universal_admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      339 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/testrunner/example/urls.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1020 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/example/views.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      668 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/local_settings.py.sample
--rw-r--r--   0 philchristensen   (502) staff       (20)     6667 2021-10-11 23:01:08.000000 django-salesforce-4.1/salesforce/testrunner/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      999 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/testrunner/test_patch.diff
--rw-r--r--   0 philchristensen   (502) staff       (20)      279 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/testrunner/urls.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.924716 django-salesforce-4.1/salesforce/tests/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/tests/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1761 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/tests/test_auth.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      817 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/tests/test_basic.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1249 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/tests/test_browser.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     8625 2021-11-24 22:24:08.000000 django-salesforce-4.1/salesforce/tests/test_bulk.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      331 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/tests/test_doc_tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2432 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/tests/test_indep.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    63768 2021-11-24 22:24:08.000000 django-salesforce-4.1/salesforce/tests/test_integration.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    12583 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/tests/test_unit.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2731 2021-10-11 22:52:49.000000 django-salesforce-4.1/salesforce/tests/test_utils.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.924940 django-salesforce-4.1/salesforce/tests/unit_tests/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/tests/unit_tests/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     3042 2020-04-22 12:21:48.000000 django-salesforce-4.1/salesforce/tests/unit_tests/test_qparser.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4502 2022-08-04 22:27:47.000000 django-salesforce-4.1/salesforce/utils.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      253 2022-08-04 22:40:04.938730 django-salesforce-4.1/setup.cfg
--rw-r--r--   0 philchristensen   (502) staff       (20)     2401 2021-10-11 22:52:49.000000 django-salesforce-4.1/setup.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.925625 django-salesforce-4.1/tests/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2139 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/clean_test_data.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.926442 django-salesforce-4.1/tests/inspectdb/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/inspectdb/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      138 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/inspectdb/admin.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.926926 django-salesforce-4.1/tests/inspectdb/dependent_model/
--rw-r--r--   0 philchristensen   (502) staff       (20)      236 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/inspectdb/dependent_model/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      349 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/inspectdb/dependent_model/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      450 2022-08-04 22:27:47.000000 django-salesforce-4.1/tests/inspectdb/dependent_model/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      463 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/inspectdb/dependent_model/test.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      357 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/inspectdb/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     5343 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/inspectdb/slow_test.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)     1800 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/inspectdb/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     3913 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/inspectdb/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      118 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/inspectdb/urls.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      440 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/mypy.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.927466 django-salesforce-4.1/tests/no_django_dbapi/
--rw-r--r--   0 philchristensen   (502) staff       (20)       76 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/no_django_dbapi/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)       33 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/no_django_dbapi/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2649 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/no_django_dbapi/test.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      114 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/no_django_dbapi/test.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.927991 django-salesforce-4.1/tests/no_salesforce/
--rw-r--r--   0 philchristensen   (502) staff       (20)       79 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/no_salesforce/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      586 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/no_salesforce/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      944 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/no_salesforce/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      939 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/no_salesforce/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)       48 2022-08-04 22:27:47.000000 django-salesforce-4.1/tests/no_urls.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.928748 django-salesforce-4.1/tests/t_debug_toolbar/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/t_debug_toolbar/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/t_debug_toolbar/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      392 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/t_debug_toolbar/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       96 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/t_debug_toolbar/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     3407 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/t_debug_toolbar/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      332 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/t_debug_toolbar/urls.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      418 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/t_debug_toolbar/views.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.929071 django-salesforce-4.1/tests/test_app_label/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_app_label/__init__.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.929516 django-salesforce-4.1/tests/test_app_label/salesforce/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_app_label/salesforce/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      187 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_app_label/salesforce/apps.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      413 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_app_label/salesforce/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      303 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/test_app_label/salesforce/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      450 2022-08-04 22:27:47.000000 django-salesforce-4.1/tests/test_app_label/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       96 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_app_label/test.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.930089 django-salesforce-4.1/tests/test_compatibility/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_compatibility/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1930 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_compatibility/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      343 2022-08-04 22:27:47.000000 django-salesforce-4.1/tests/test_compatibility/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      102 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_compatibility/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1872 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/test_compatibility/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.930663 django-salesforce-4.1/tests/test_default_db/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_default_db/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2091 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_default_db/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      367 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/test_default_db/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      351 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_default_db/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     5346 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_default_db/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.931185 django-salesforce-4.1/tests/test_dynamic_auth/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_dynamic_auth/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_dynamic_auth/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      525 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/test_dynamic_auth/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      100 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_dynamic_auth/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1619 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/test_dynamic_auth/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.931631 django-salesforce-4.1/tests/test_general/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_general/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      126 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_general/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      108 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_general/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     4073 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_general/test_helpers.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.932172 django-salesforce-4.1/tests/test_lazy_connect/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_lazy_connect/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_lazy_connect/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      653 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_lazy_connect/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      100 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_lazy_connect/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1039 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_lazy_connect/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.932712 django-salesforce-4.1/tests/test_managers/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/test_managers/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      850 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/test_managers/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      415 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_managers/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       92 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/test_managers/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1306 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/test_managers/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.933268 django-salesforce-4.1/tests/test_migrate/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_migrate/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      881 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/test_migrate/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      558 2022-08-04 22:27:47.000000 django-salesforce-4.1/tests/test_migrate/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)     1116 2021-11-24 22:24:08.000000 django-salesforce-4.1/tests/test_migrate/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1182 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/test_migrate/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.933831 django-salesforce-4.1/tests/test_mixin/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_mixin/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2469 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mixin/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      322 2022-08-04 22:27:47.000000 django-salesforce-4.1/tests/test_mixin/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       86 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_mixin/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1651 2020-05-08 13:55:20.000000 django-salesforce-4.1/tests/test_mixin/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.934406 django-salesforce-4.1/tests/test_mock/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/test_mock/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    18727 2022-08-04 22:27:47.000000 django-salesforce-4.1/tests/test_mock/mocksf.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      525 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     7670 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock/test_data.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4641 2021-11-24 22:24:08.000000 django-salesforce-4.1/tests/test_mock/test_mocksf.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.935083 django-salesforce-4.1/tests/test_mock2/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock2/__init__.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.935376 django-salesforce-4.1/tests/test_mock2/migrations/
--rw-r--r--   0 philchristensen   (502) staff       (20)     4372 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock2/migrations/0001_initial.py
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock2/migrations/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1694 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock2/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      177 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock2/mypy.ini
--rw-r--r--   0 philchristensen   (502) staff       (20)      808 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock2/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       95 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock2/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     5589 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/test_mock2/test_rec.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      268 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/tests.sh
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      175 2020-04-22 12:21:48.000000 django-salesforce-4.1/tests/tests_no_django.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.936323 django-salesforce-4.1/tests/tooling/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/tooling/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      138 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/tooling/admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      366 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/tooling/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     9767 2022-08-04 22:27:47.000000 django-salesforce-4.1/tests/tooling/slow_test.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      605 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/tooling/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1871 2020-07-09 19:30:00.000000 django-salesforce-4.1/tests/tooling/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      140 2021-10-11 22:52:49.000000 django-salesforce-4.1/tests/tooling/urls.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4439 2022-08-04 22:27:47.000000 django-salesforce-4.1/tox.ini
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2022-08-04 22:40:04.938025 django-salesforce-4.1/wiki/
--rw-r--r--   0 philchristensen   (502) staff       (20)      548 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Documents-and-Attachments.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     3078 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Empty-strings-in-filters.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     4902 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Error-messages.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     6979 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Experimental-Features.rest
--rw-r--r--   0 philchristensen   (502) staff       (20)     2938 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Foreign-Key-Support.rest
--rw-r--r--   0 philchristensen   (502) staff       (20)     2505 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Home.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     7981 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Introspection-and-Special-Attributes-of-Fields.rest
--rw-r--r--   0 philchristensen   (502) staff       (20)     2120 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Lead-Conversion.rest
--rw-r--r--   0 philchristensen   (502) staff       (20)     1528 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/Release-Process.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     1977 2020-07-09 19:30:00.000000 django-salesforce-4.1/wiki/SalesforceModels-used-with-local-databases.md
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.677727 django-salesforce-4.2/
+-rw-r--r--   0 philchristensen   (502) staff       (20)      475 2021-10-11 22:52:49.000000 django-salesforce-4.2/.coveragerc
+-rw-r--r--   0 philchristensen   (502) staff       (20)      263 2020-04-22 12:21:48.000000 django-salesforce-4.2/.editorconfig
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.644432 django-salesforce-4.2/.github/
+-rw-r--r--   0 philchristensen   (502) staff       (20)       64 2020-04-22 12:21:48.000000 django-salesforce-4.2/.github/FUNDING.yml
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.644675 django-salesforce-4.2/.github/workflows/
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1935 2023-07-04 13:35:06.000000 django-salesforce-4.2/.github/workflows/main.yml
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1791 2023-07-04 13:35:06.000000 django-salesforce-4.2/.travis.yml
+-rw-r--r--   0 philchristensen   (502) staff       (20)      604 2020-04-22 12:21:48.000000 django-salesforce-4.2/AUTHORS.md
+-rw-r--r--   0 philchristensen   (502) staff       (20)    14702 2023-07-04 13:52:16.000000 django-salesforce-4.2/CHANGELOG.rst
+-rw-r--r--   0 philchristensen   (502) staff       (20)     3217 2020-04-22 12:21:48.000000 django-salesforce-4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1572 2020-04-22 12:21:48.000000 django-salesforce-4.2/CONTRIBUTING.md
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)     1392 2023-07-04 13:35:06.000000 django-salesforce-4.2/LICENSE.md
+-rw-r--r--   0 philchristensen   (502) staff       (20)       67 2020-04-22 12:21:48.000000 django-salesforce-4.2/MANIFEST.in
+-rw-r--r--   0 philchristensen   (502) staff       (20)    17145 2023-07-04 13:52:27.677832 django-salesforce-4.2/PKG-INFO
+-rw-r--r--   0 philchristensen   (502) staff       (20)    16694 2023-07-04 13:35:06.000000 django-salesforce-4.2/README.rst
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)     2313 2023-07-04 13:35:06.000000 django-salesforce-4.2/coverage_run.sh
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.645565 django-salesforce-4.2/django_salesforce.egg-info/
+-rw-r--r--   0 philchristensen   (502) staff       (20)    17145 2023-07-04 13:52:27.000000 django-salesforce-4.2/django_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 philchristensen   (502) staff       (20)     6164 2023-07-04 13:52:27.000000 django-salesforce-4.2/django_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 philchristensen   (502) staff       (20)        1 2023-07-04 13:52:27.000000 django-salesforce-4.2/django_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 philchristensen   (502) staff       (20)        1 2020-05-08 14:00:41.000000 django-salesforce-4.2/django_salesforce.egg-info/not-zip-safe
+-rw-r--r--   0 philchristensen   (502) staff       (20)       40 2023-07-04 13:52:27.000000 django-salesforce-4.2/django_salesforce.egg-info/requires.txt
+-rw-r--r--   0 philchristensen   (502) staff       (20)       11 2023-07-04 13:52:27.000000 django-salesforce-4.2/django_salesforce.egg-info/top_level.txt
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.645688 django-salesforce-4.2/docs/
+-rw-r--r--   0 philchristensen   (502) staff       (20)      956 2021-11-24 22:24:08.000000 django-salesforce-4.2/docs/details.rst
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      428 2023-07-04 13:35:06.000000 django-salesforce-4.2/manage.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      281 2023-05-23 16:17:25.000000 django-salesforce-4.2/mypy.ini
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      148 2021-10-11 22:52:49.000000 django-salesforce-4.2/pylint.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)    12617 2021-10-11 23:01:08.000000 django-salesforce-4.2/pylintrc
+-rw-r--r--   0 philchristensen   (502) staff       (20)      133 2021-10-11 22:52:49.000000 django-salesforce-4.2/requirements.txt
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.647460 django-salesforce-4.2/salesforce/
+-rw-r--r--   0 philchristensen   (502) staff       (20)      660 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      304 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/admin.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      286 2020-05-08 13:55:20.000000 django-salesforce-4.2/salesforce/apps.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    26537 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/auth.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.649998 django-salesforce-4.2/salesforce/backend/
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2232 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4642 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/base.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      600 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/client.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    25481 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/compiler.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1417 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/creation.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2885 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/enterprise.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     3237 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/features.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2050 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/backend/indep.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    21748 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/introspection.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2516 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/manager.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2894 2023-05-23 16:17:25.000000 django-salesforce-4.2/salesforce/backend/models_lookups.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     6328 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/models_sql_query.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4602 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/operations.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     9862 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/query.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1395 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/backend/schema.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1043 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/test_helpers.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    17864 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/utils.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     3406 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/backend/validation.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.651764 django-salesforce-4.2/salesforce/dbapi/
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4265 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/dbapi/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2074 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/dbapi/common.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    40689 2021-11-24 22:24:08.000000 django-salesforce-4.2/salesforce/dbapi/driver.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     8012 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/dbapi/exceptions.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    14558 2023-05-23 16:17:25.000000 django-salesforce-4.2/salesforce/dbapi/subselect.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     5470 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/dbapi/test_helpers.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     8104 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/defaults.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    12767 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/fields.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.652004 django-salesforce-4.2/salesforce/management/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/management/__init__.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.652217 django-salesforce-4.2/salesforce/management/commands/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/management/commands/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     7020 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/management/commands/inspectdb.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    11027 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4823 2022-08-04 22:27:47.000000 django-salesforce-4.2/salesforce/models_extend.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2076 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/models_template.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4143 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/router.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.652907 django-salesforce-4.2/salesforce/testrunner/
+-rw-r--r--   0 philchristensen   (502) staff       (20)       94 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/__init__.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.654773 django-salesforce-4.2/salesforce/testrunner/example/
+-rw-r--r--   0 philchristensen   (502) staff       (20)       94 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/example/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      482 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/example/admin.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      196 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/example/forms.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    18673 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/example/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2049 2020-05-08 13:55:20.000000 django-salesforce-4.2/salesforce/testrunner/example/models_template.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.655357 django-salesforce-4.2/salesforce/testrunner/example/templates/
+-rw-r--r--   0 philchristensen   (502) staff       (20)      444 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/testrunner/example/templates/list-accounts.html
+-rw-r--r--   0 philchristensen   (502) staff       (20)      717 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/testrunner/example/templates/search-accounts.html
+-rw-r--r--   0 philchristensen   (502) staff       (20)      314 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/example/tests.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1260 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/testrunner/example/universal_admin.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      290 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/example/urls.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      971 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/example/views.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      668 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/testrunner/local_settings.py.sample
+-rw-r--r--   0 philchristensen   (502) staff       (20)     6819 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/testrunner/settings.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      999 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/testrunner/test_patch.diff
+-rw-r--r--   0 philchristensen   (502) staff       (20)      279 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/testrunner/urls.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.657674 django-salesforce-4.2/salesforce/tests/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/tests/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1712 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/tests/test_auth.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      817 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/tests/test_basic.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1249 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/tests/test_browser.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     8625 2021-11-24 22:24:08.000000 django-salesforce-4.2/salesforce/tests/test_bulk.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      331 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/tests/test_doc_tests.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2432 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/tests/test_indep.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    63601 2023-07-04 13:35:06.000000 django-salesforce-4.2/salesforce/tests/test_integration.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    12583 2022-08-04 22:27:47.000000 django-salesforce-4.2/salesforce/tests/test_unit.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2731 2021-10-11 22:52:49.000000 django-salesforce-4.2/salesforce/tests/test_utils.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.658020 django-salesforce-4.2/salesforce/tests/unit_tests/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/tests/unit_tests/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     3042 2020-04-22 12:21:48.000000 django-salesforce-4.2/salesforce/tests/unit_tests/test_qparser.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4502 2022-08-04 22:27:47.000000 django-salesforce-4.2/salesforce/utils.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      253 2023-07-04 13:52:27.678129 django-salesforce-4.2/setup.cfg
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2336 2023-07-04 13:35:06.000000 django-salesforce-4.2/setup.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.660694 django-salesforce-4.2/tests/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2139 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/clean_test_data.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)   303104 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/db.sqlite3
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.661913 django-salesforce-4.2/tests/inspectdb/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/inspectdb/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      138 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/inspectdb/admin.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.662536 django-salesforce-4.2/tests/inspectdb/dependent_model/
+-rw-r--r--   0 philchristensen   (502) staff       (20)      236 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/inspectdb/dependent_model/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      349 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/inspectdb/dependent_model/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      450 2022-08-04 22:27:47.000000 django-salesforce-4.2/tests/inspectdb/dependent_model/settings.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      463 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/inspectdb/dependent_model/test.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      357 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/inspectdb/settings.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     5340 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/inspectdb/slow_test.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)     1800 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/inspectdb/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     3913 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/inspectdb/tests.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      118 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/inspectdb/urls.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      636 2023-05-23 16:17:25.000000 django-salesforce-4.2/tests/mypy.sh
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.663323 django-salesforce-4.2/tests/no_django_dbapi/
+-rw-r--r--   0 philchristensen   (502) staff       (20)       76 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/no_django_dbapi/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)       33 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/no_django_dbapi/settings.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     3124 2023-05-23 16:17:25.000000 django-salesforce-4.2/tests/no_django_dbapi/test.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      114 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/no_django_dbapi/test.sh
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.663905 django-salesforce-4.2/tests/no_salesforce/
+-rw-r--r--   0 philchristensen   (502) staff       (20)       79 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/no_salesforce/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      586 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/no_salesforce/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      944 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/no_salesforce/settings.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      939 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/no_salesforce/tests.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)       48 2022-08-04 22:27:47.000000 django-salesforce-4.2/tests/no_urls.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.664904 django-salesforce-4.2/tests/t_debug_toolbar/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/t_debug_toolbar/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/t_debug_toolbar/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      392 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/t_debug_toolbar/settings.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.665200 django-salesforce-4.2/tests/t_debug_toolbar/small_app/
+-rw-r--r--   0 philchristensen   (502) staff       (20)      348 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/t_debug_toolbar/small_app/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      271 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/t_debug_toolbar/small_app/urls.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)       96 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/t_debug_toolbar/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     3407 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/t_debug_toolbar/tests.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      332 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/t_debug_toolbar/urls.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      418 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/t_debug_toolbar/views.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.665664 django-salesforce-4.2/tests/test_app_label/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_app_label/__init__.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.666237 django-salesforce-4.2/tests/test_app_label/salesforce/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_app_label/salesforce/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      187 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_app_label/salesforce/apps.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      413 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_app_label/salesforce/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      303 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/test_app_label/salesforce/tests.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      450 2022-08-04 22:27:47.000000 django-salesforce-4.2/tests/test_app_label/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)       96 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_app_label/test.sh
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.666987 django-salesforce-4.2/tests/test_compatibility/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_compatibility/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1930 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_compatibility/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      343 2022-08-04 22:27:47.000000 django-salesforce-4.2/tests/test_compatibility/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      102 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_compatibility/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1872 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/test_compatibility/tests.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.667643 django-salesforce-4.2/tests/test_default_db/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_default_db/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2091 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_default_db/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      381 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/test_default_db/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      351 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_default_db/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     5346 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_default_db/tests.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.668435 django-salesforce-4.2/tests/test_dynamic_auth/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_dynamic_auth/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_dynamic_auth/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      525 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/test_dynamic_auth/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      100 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_dynamic_auth/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1619 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/test_dynamic_auth/tests.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.668998 django-salesforce-4.2/tests/test_general/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_general/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      126 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_general/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      108 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_general/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4073 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_general/test_helpers.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.669705 django-salesforce-4.2/tests/test_lazy_connect/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_lazy_connect/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_lazy_connect/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      653 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_lazy_connect/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      100 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_lazy_connect/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1039 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_lazy_connect/tests.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.670429 django-salesforce-4.2/tests/test_managers/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/test_managers/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      850 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/test_managers/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      447 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/test_managers/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)       92 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/test_managers/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1453 2023-05-23 16:17:25.000000 django-salesforce-4.2/tests/test_managers/tests.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.671215 django-salesforce-4.2/tests/test_migrate/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_migrate/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      881 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/test_migrate/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      558 2022-08-04 22:27:47.000000 django-salesforce-4.2/tests/test_migrate/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)     1116 2021-11-24 22:24:08.000000 django-salesforce-4.2/tests/test_migrate/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1182 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/test_migrate/tests.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.672122 django-salesforce-4.2/tests/test_mixin/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_mixin/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2469 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mixin/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      322 2022-08-04 22:27:47.000000 django-salesforce-4.2/tests/test_mixin/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)       86 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_mixin/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1651 2020-05-08 13:55:20.000000 django-salesforce-4.2/tests/test_mixin/tests.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.673105 django-salesforce-4.2/tests/test_mock/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/test_mock/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    18727 2022-08-04 22:27:47.000000 django-salesforce-4.2/tests/test_mock/mocksf.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      525 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock/settings.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     7670 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock/test_data.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4641 2021-11-24 22:24:08.000000 django-salesforce-4.2/tests/test_mock/test_mocksf.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.674003 django-salesforce-4.2/tests/test_mock2/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock2/__init__.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.674399 django-salesforce-4.2/tests/test_mock2/migrations/
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4372 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock2/migrations/0001_initial.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock2/migrations/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1694 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock2/models.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      177 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock2/mypy.ini
+-rw-r--r--   0 philchristensen   (502) staff       (20)      826 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/test_mock2/settings.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)       95 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock2/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     5589 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/test_mock2/test_rec.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      268 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/tests.sh
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      175 2020-04-22 12:21:48.000000 django-salesforce-4.2/tests/tests_no_django.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1001 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/to_mock.py
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.675509 django-salesforce-4.2/tests/tooling/
+-rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/tooling/__init__.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      138 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/tooling/admin.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      366 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/tooling/settings.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)    10373 2023-07-04 13:35:06.000000 django-salesforce-4.2/tests/tooling/slow_test.py
+-rwxr-xr-x   0 philchristensen   (502) staff       (20)      605 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/tooling/test.sh
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1871 2020-07-09 19:30:00.000000 django-salesforce-4.2/tests/tooling/tests.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)      140 2021-10-11 22:52:49.000000 django-salesforce-4.2/tests/tooling/urls.py
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4341 2023-07-04 13:35:06.000000 django-salesforce-4.2/tox.ini
+drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2023-07-04 13:52:27.677518 django-salesforce-4.2/wiki/
+-rw-r--r--   0 philchristensen   (502) staff       (20)      548 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/Documents-and-Attachments.md
+-rw-r--r--   0 philchristensen   (502) staff       (20)     3078 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/Empty-strings-in-filters.md
+-rw-r--r--   0 philchristensen   (502) staff       (20)     4902 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/Error-messages.md
+-rw-r--r--   0 philchristensen   (502) staff       (20)     6979 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/Experimental-Features.rest
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2939 2023-07-04 13:35:06.000000 django-salesforce-4.2/wiki/Foreign-Key-Support.rest
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2505 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/Home.md
+-rw-r--r--   0 philchristensen   (502) staff       (20)     7981 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/Introspection-and-Special-Attributes-of-Fields.rest
+-rw-r--r--   0 philchristensen   (502) staff       (20)     2120 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/Lead-Conversion.rest
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1528 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/Release-Process.md
+-rw-r--r--   0 philchristensen   (502) staff       (20)     1977 2020-07-09 19:30:00.000000 django-salesforce-4.2/wiki/SalesforceModels-used-with-local-databases.md
```

### Comparing `django-salesforce-4.1/.github/workflows/main.yml` & `django-salesforce-4.2/.github/workflows/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 name: django-salesforce test
 
 on:
   push:
-    branches: [ actions ]
+    branches: [ 'actions*', main ]
   # pull_request:
   #   branches: [ main ]
 # # prefer to teminate some queued jobs only manually, "max-parallel: 1" works enough
 # concurrency:
 #   group: one-job-at-a-time
 #   cancel-in-progress: true
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 1
       matrix:
-        python-version: [3.8, "3.10", 3.6, 3.9]
+        python-version: [3.8, 3.11, "3.10", 3.7, 3.9]
     timeout-minutes: 20
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install Dependencies, Customize local_settings
       run: |
         python${{ matrix.python-version }} -V
         pip install --upgrade pip
         pip install tox
         # this should be used only for a capitalized primary key 'Id' with migrations
         # sed -i -e "s/'id', salesforce/'Id', salesforce/" salesforce/testrunner/example/migrations/0*.py
     - name: Run Tests
       env:
-        TOX_TESTENV_PASSENV: "SF_CONSUMER_KEY SF_CONSUMER_SECRET SF_USER SF_PASSWORD SF_HOST"
+        DJSF_LICENSE_KEY: ${{ secrets.DJSF_LICENSE_KEY }}
         SF_CONSUMER_KEY: ${{ secrets.SF_CONSUMER_KEY }}
         SF_CONSUMER_SECRET: ${{ secrets.SF_CONSUMER_SECRET }}
         SF_USER: ${{ secrets.SF_USER }}
         SF_PASSWORD: ${{ secrets.SF_PASSWORD }}
         SF_HOST: ${{ secrets.SF_HOST }}
 
         TOXENV_38:  "docs_style,typing,clean,dj22-py38,dj32-py38"
+        TOXENV_311: "dj42-py311"
         TOXENV_310: "dj40-py310"
-        TOXENV_36:  "dj20-py36,dj30-py36"
+        TOXENV_37:  "dj20-py37,dj30-py37"
         TOXENV_39:  "no_django-py39,debug_toolbar-dj32-py39"
       run: |
         TOXENV_NAME=$(echo TOXENV_${{ matrix.python-version }} | sed 's/\.//')
         cat > salesforce/testrunner/local_settings.py <<'-- end local_settings --'
         SF_PK = 'Id'
         SF_LAZY_CONNECT = False
         -- end local_settings --
         echo "tox -e ${!TOXENV_NAME}"
-        tox -e ${!TOXENV_NAME}
+        tox -e ${!TOXENV_NAME} --colored yes
```

### Comparing `django-salesforce-4.1/.travis.yml` & `django-salesforce-4.2/.travis.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # It is important to set "Limit concurrent jobs" to "1" in repository settings in Travis-CI
 language: python
-# Ubuntu 20.04 Focal Fossa (has a default Python 3.8, suported 3.5 - 3.9)
-dist: focal
-if: branch = main
+# Ubuntu 22.04 Jammy Jellyfish (has a default Python 3.10, suported 3.7 - 3.10)
+dist: jammy
+if: branch in (main, travis)
 env:
   global:
     - secure: "Z6wS6a/YcyT8w5l+2HfMItbn2mbv+f1W43WixoqB4QkgiocjBWvmAQD6PN1sEgWVmZlRvWCABK8FcGG+Y6RPFeNdCE0U1h9hEgOiAnhUpWWH/AhOYDZ0PnFwA3/iRrHS2VFPmhdkjw1BUEfqXaJfDYtlZLgpMMfRvEjIJ8Uqq6M="
     - secure: "JJGGbExBKyXkAltrc4rRLG56ks20/GfGcfugI9mqjeHgQ7IcDvhnouqAIjfbNlhgclyAkWHwJRs7taaM0T9a9AcEQujs2B0JJYOLQSBGnWJSCbsDspWAdlT92U+PzhnZrDm7apg1iBk/c8KtofBo6DqsTveBocFnYXTjeqbSVuY="
     - secure: "TrsYtntXQWgjrXPFaL3aUPoyPtR7pBVqsRx5dIj0yhrPuZR0L2bFi0MOA8cXflaYucx+xa+PEyrPO6FfLl+ri8I2WiXeDLbXlUC614UW6Od1kCklZ7/gk5wor7RwfEtIAtxh5erljUw2N2O9utkRFBDCuASRaQCqBzMItgcUOhA="
     - secure: "CZWsHsATIIAdvAWoHM1niGa8KGfcDR9p49vr/um6DU2wDWt3SVxOei+Z+X8lvIJs4JXiJHzIo6H4qrqf8qxf3hDWjx4TIERz35+5osAWstLkCAxcaWV8JlomxVI+P8tU7dCgZdBeLkVi1O+H8+B2bAVXdK77gcQkSttGh/ykm48="
-    - TOX_TESTENV_PASSENV="SF_CONSUMER_KEY SF_CONSUMER_SECRET SF_USER SF_PASSWORD SF_HOST"
+    - secure: "hKRKQDaS4H9h1S67nx2znqAEMuDxFynidXa0pzNHqF3N02caUA/TdHPG7Vp78a9TmNoXAC4V2efEg5JfdqUzyrkJzfDX1rWIYSJq37nAroCBQhnNwKbWCGqgfQm6Sb2tXevYhZwqe2Klt7XRx+7c8wavEsrCYLD4m4KjpQ+sekI="
 cache:
   directories:
     - $HOME/.pip-cache/
 install:
   - pip install tox
 script:
   - echo -e "SF_PK = 'Id'" > salesforce/testrunner/local_settings.py
   - tox
 jobs:
   include:
-    - python: 3.6
+    - python: 3.8
       before_install:
-        - python3.6 -V
         - python3.8 -V
-      env: TOXENV=docs_style,typing,dj20-py36,dj22-py38,dj30-py36,dj32-py38
+        - python3.10 -V
+      env: TOXENV=docs_style,typing,dj41-py310,dj32-py38
     - python: 3.9
-      env: TOXENV=dj41-py39,dj40-py39,no_django-py39,debug_toolbar-dj32-py39
+      before_install:
+        - python3.9 -V
+        - pip3.9 install -U setuptools
+      env: TOXENV=dj40-py39,dj30-py39,no_django-py39,debug_toolbar-dj32-py39
+    - python: 3.7
+      before_install:
+        - python3.7 -V
+      env: TOXENV=dj20-py37,dj22-py37
```

### Comparing `django-salesforce-4.1/AUTHORS.md` & `django-salesforce-4.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/CHANGELOG.rst` & `django-salesforce-4.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,29 @@
 some undocumented internal code that could yet have been used by
 someone. Not related e.g. to examples and tests,
 but a new feature can be referred by a test name if not documented yet.
 Some items here can be marked as "internal": not ready enough or
 experimental.
 
 
-[4.1] Unpublished
------------------
+[4.2] 2023-07-04
+-------------------
+* Add: Basic diagnostics after installation can be done by command
+  ``python manage.py check --database=salesforce``
+* Change: Use with Django 4.2 requires an enterprise license key.
+* Add: Support for Django 4.2
+* Use API 58.0 Summer '23
+* Add: Support for Django Database caching #315
+* Fix: Configurable max introspected pick-list size
+  SF_MAX_INSPECTDB_PICKLIST_LENGTH #312
+  Some people need to introspect huge picklists, some don't want.
+
+
+[4.1] 2022-08-05
+----------------
 * Add: Support for Django 4.1
 * Add: Command ``inspectdb`` can introspect actual default values
   of fields from a ``defaultValueFormula`` if it is a simple constant
   like a number or a string.
 * Fix: A default value ``DefaultedOnCreate(value)`` is no longer created
   by ``inspectdb`` in favour of a simple ``value``. If a simple default value
   can not be known then a generic ``DEFAULTED_ON_CREATE`` is still used rarely
```

### Comparing `django-salesforce-4.1/CODE_OF_CONDUCT.md` & `django-salesforce-4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/CONTRIBUTING.md` & `django-salesforce-4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/LICENSE.md` & `django-salesforce-4.2/LICENSE.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+Copyright (c) 2023 Hynek Cernoch and Phil Christensen <br>- Modified MIT License -<br> Please do not remove the the code that requires a license key for some "enterprise" features, but become a sponsor or use our similar package django-salesforce-agpl with an AGPL license or use only the standard features. <br> Everything other is like in the MIT license: <br>- - -
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `django-salesforce-4.1/PKG-INFO` & `django-salesforce-4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 Metadata-Version: 2.1
 Name: django-salesforce
-Version: 4.1
+Version: 4.2
 Summary: a Salesforce backend for Django's ORM
 Home-page: https://github.com/django-salesforce/django-salesforce
-Author: Freelancers Union
-Author-email: devs@freelancersunion.org
+Author: Hynek Cernoch
+Author-email: hynek@sdb.cz
 Maintainer: Phil Christensen
 Maintainer-email: phil@bubblehouse.org
-License: MIT
+License: AGPL
 Keywords: django salesforce orm backend
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.md
 
 django-salesforce
 =================
 
-.. image:: https://travis-ci.com/django-salesforce/django-salesforce.svg?branch=master
-   :target: https://travis-ci.com/django-salesforce/django-salesforce
+.. image:: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml
 
 .. image:: https://badge.fury.io/py/django-salesforce.svg
    :target: https://pypi.python.org/pypi/django-salesforce
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue
    :target: https://www.python.org/
 
-.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1-blue.svg
+.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2-blue.svg
    :target: https://www.djangoproject.com/
 
 This library allows you to load, edit and query the objects in any Salesforce instance
 using Django models. The integration is fairly complete, and generally seamless
 for most uses. It works by integrating with the Django ORM, allowing access to
 the objects in your SFDC instance (Salesforce .com) as if they were in a
 traditional database.
 
-Python 3.6 to 3.10, Django 2.0 to 4.1. (Tested also with Python 3.11 beta 4)
+Python 3.7 to 3.11, Django 2.0 to 4.2. (Tested also with Python 3.12 beta 3)
+
+Use with Django 4.2 currently requires an enteprise license key DJSF_LICENSE_KEY
+available to sponsors, or to accept an AGPL license if you install our equivalent
+package "django-salesforce-agpl" instead.
 
 
 Quick Start
 -----------
 
 Install, configure a Salesforce connection, create a Salesforce model and run.
 
-1. Install django-salesforce: ``pip install django-salesforce``
+1. **Install** django-salesforce: ``pip install django-salesforce``
 
-2. Add a salesforce connection to your ``DATABASES`` setting::
+2. Add a Salesforce **connection** to your ``DATABASES`` **setting**::
 
     'salesforce': {
         'ENGINE': 'salesforce.backend',
         'CONSUMER_KEY': '',                # 'client_id'   in OAuth2 terminology
         'CONSUMER_SECRET': '',             # 'client_secret'
         'USER': '',
         'PASSWORD': '',
@@ -59,44 +63,33 @@
    In the example above, all fields should be populated as follows:
 
    * ``CONSUMER_KEY`` and ``CONSUMER_SECRET`` values are for the app used to
      connect to your Salesforce account. Instructions for how get these are in
      the Salesforce REST API Documentation. Key and secret can be created on
      web by:
 
-     - Salesforce Classic > Setup > App Setup > Create > Apps > Connected apps >
+     - SalesForce **Lightning** > Setup > Apps > App Manager > New Connected App or by
+       Salesforce **Classic** > Setup > App Setup > Create > Apps > Connected apps >
        New.  
-       or SalesForce Lightning > Setup > Apps > App Manager > New Connected App.
      - Click "Enable OAuth Settings" in API, then select "Access and manage
        your data (api)" from available OAuth Scopes.
      - Other red marked fields must be filled, but are not relevant for Django
        with password authentication. ("Callback URL" should be a safe URL
-       that maybe doesn't exist, but is under your control and doesn't redirect,
-       for the case that you accidentally activate other OAuth mode later.)
+       that maybe doesn't exist now, but its path is under your control and
+       doesn't redirect. This would be important if you activate other OAuth
+       mode later.)
    * ``USER`` is the username used to connect.
    * ``PASSWORD`` is a concatenation of the user's password and security token.
      Security token can be set by My Settings / Personal / Reset My Security Token
      or an new token is received by email after every password change.
      Security token can be omitted if the local IP address has been
      whitelisted in Security Controls / Network Access.
    * ``HOST`` is ``https://test.salesforce.com`` to access a sandbox, or
-     ``https://login.salesforce.com`` to access production.
-
-   If an error occurs in a request to Salesforce, review the received error message
-   that is exactly copied between braces ``{...}`` from the
-   Salesforce response to a Python exception to assist debugging.
-
-   See also: `Information on settings up Salesforce connected apps
-   <https://help.salesforce.com/apex/HTViewHelpDoc?id=connected_app_create.htm>`_
-   if necessary.
-
-   **Note about permissions**: Administrator rights are only required to run
-   the full suite of unit tests; otherwise, as long as the account has rights to
-   read or modify the chosen object, everything should work properly.
-   Introspection by ``inspectdb`` doesn't require any object permissions.
+     ``https://login.salesforce.com`` to access production or your domain
+     ``https://MyDomainName.my.salesforce.com``.
 
 3. Add ``salesforce.router.ModelRouter`` to your ``DATABASE_ROUTERS``
    setting::
 
     DATABASE_ROUTERS = [
         "salesforce.router.ModelRouter"
     ]
@@ -115,79 +108,106 @@
         "salesforce"
     }
 
    (This is necessary for running Salesforce extensions in the command
    ``inspectdb --database=salesforce`` in development, otherwise it is
    not important.)
 
+5. Add a setting ``DJSF_LICENSE_KEY = "Your Name or Company / email //our.signature=="``
+   if you need it for Django 4.2 now.
+
+6. **Verify** that everything important is configured correctly by running
+   the command ``python manage.py check --database=salesforce``.
+   You get eventualy the important information about problems related to the previous
+   steps. (clearly without tracebacks)
+
+   That is useful again after you define your database model or if you customize your
+   configuration later and e.g. you configure multiple Salesforce databases.
 
-5. Define a model that extends ``salesforce.models.Model`` (alias ``SalesforceModel``)
+7. Define a **model** that extends ``salesforce.models.Model`` (alias ``SalesforceModel``)
    or export the complete SF schema by ``python manage.py inspectdb --database=salesforce``
-   and simplify it to what you need. The full models file is about 2 MB with 500 models
+   and simplify it to what you need. The full models file is about 1.5 MB with 500 models
    and the export takes 2 minutes, but it is a valid models module that works without
    modification. The output of command ``inspectdb`` can be restricted by a list
    of table_names on the command line, but also ForeignKey fields to omitted models
    must be pruned to get a valid complete small model.
 
-6. **(optional)** To override the default timeout of 15 seconds,
-   define ``SALESFORCE_QUERY_TIMEOUT`` in your settings file.
-   It can be one number or better a tuple with a short value for connection
-   timeout and a longer value that includes time for running a query.
-   It never need be longer than 30 seconds::
+8. **You're all done!** Just use your model like a normal Django model.
 
-    SALESFORCE_QUERY_TIMEOUT = (4, 15)  # default (connect timeout, data timeout)
+   If an error occurs in a request to Salesforce, review the received error message
+   that is exactly copied between braces ``{...}`` from the
+   Salesforce response to a Python exception to assist debugging.
+
+   See also: `Information on settings up Salesforce connected apps
+   <https://help.salesforce.com/apex/HTViewHelpDoc?id=connected_app_create.htm>`_
+   if necessary.
+
+   **Note about permissions**: Administrator profile are only required to run
+   the full suite of unit tests of this framework; otherwise, as long as
+   the account has rights to read or modify the chosen object, everything
+   should work properly. Introspection by ``inspectdb`` doesn't require any
+   additional object permissions.
+
+
+Optional small features
+-----------------------
 
-7. **(optional)** If you want to use another name for your Salesforce DB
+-  **Salesforce alias** If you want to use another name for your Salesforce DB
    connection, define ``SALESFORCE_DB_ALIAS`` in your settings file::
 
     SALESFORCE_DB_ALIAS = 'salesforce'  # default
 
-8. You're all done! Just use your model like a normal Django model.
+-  **Timeout settings** To override the default timeout of 15 seconds,
+   define ``SALESFORCE_QUERY_TIMEOUT`` in your settings file.
+   It can be one number or better a tuple with a short value for connection
+   timeout and a longer value that includes time for running a query.
+   It never need be longer than 30 seconds::
 
-9. **(optional)** Create a normal Django ``admin.py`` module for your Salesforce models
+    SALESFORCE_QUERY_TIMEOUT = (4, 15)  # default (connect timeout, data timeout)
+
+-  **Automatic stupid admin** Create a normal Django ``admin.py`` module for your Salesforce models
    and you can register a minimalistic admin for all omitted Admin classes::
 
     from salesforce.testrunner.example.universal_admin import register_omitted_classes
     # some admin classes that you wrote manually yet
     # ...
     # end of file
     register_omitted_classes(your_application.models)
 
    This is a rudimentary way to verify that every model works in a sandbox, before
    hand-writing all admin classes. (Foreign keys to huge tables in the production
    require a customized admin e.g. with search widgets.)
     
-10. **(optional)** By default, the Django ORM connects to all DBs at startup. To delay
+-   **Lazy connect** By default, the Django ORM connects to all DBs at startup. To delay
     SFDC connections until they are actually required, define ``SF_LAZY_CONNECT=True``
     in your settings file. Be careful when using this setting; since it won't fail during
     the application boot, it's possible for a bad password to be sent repeatedly,
     requiring an account reset to fix.
 
-Primary Key
------------
-Salesforce doesn't allow you to define custom primary keys, so django-salesforce
-will add them automatically in all cases. You can override only capitalization and use
-a primary key ``Id`` by configuring ``SF_PK='Id'`` in your project settings
-if you prefer Salesforce capitalized field name conventions instead of Django
-default ``id``.
+-  **Configurable Primary Key**
+   Salesforce doesn't allow you to define custom primary keys, so django-salesforce
+   will add them automatically in all cases. You can override only capitalization and use
+   a primary key ``Id`` by configuring ``SF_PK='Id'`` in your project settings
+   if you prefer Salesforce capitalized field name conventions instead of Django
+   default ``id``.
 
 Advanced usage
 --------------
 -  **Multiple Inheritance from Abstract Models** - Many Salesforce models use
    the same sets of fields, but using a single inheritance tree would be too
    complicated and fragile. Proxy models and mixins are also supported.
 
 -  **Testing** - By default, tests will be run against the SFDC connection
    specified in settings.py, which will substantially increase testing time.
 
    One way to speed this up is to change the SALESFORCE_DB_ALIAS to point to
    another DB connection (preferably SQLite) during testing using the
    ``TEST`` settings variable. Such simple tests can run without any network
-   access. Django unit tests without SalesforceModel
-   are fast everytimes. Special read only fields that are updated only by SFDC
+   access. Django unit tests without SalesforceModel are fast everytimes.
+   Special read only fields (with ``sf_read_only=...``) that are updated only by SFDC
    e.g. ``last_modified_date`` need more parameters to be possible to save them
    into an alternate database, e.g. by ``auto_now=True`` or to play with
    ``null=True`` or ``default=...``.
    
 -  **Multiple SFDC connections** - In most cases, a single connection is all
    that most apps require, so the default DB connection to use for Salesforce
    is defined by the ``SALESFORCE_DB_ALIAS`` settings variable. This behavior
@@ -242,23 +262,27 @@
    exceptions are raised by Django-Salesforce to get more useful information.
    General exceptions are ``SalesforceError`` or a more general custom
    ``DatabaseError``. They can be imported from ``salesforce.dbapi.exceptions``
    if database errors should be handled specifically in your app.
 
 Foreign Key Support
 -------------------
-Foreign key relationships should work as expected, but mapping
-Salesforce SOQL to a purely-relational mapper is a leaky abstraction. For the
-gory details, see `Foreign Key Support <https://github.com/django-salesforce/django-salesforce/wiki/Foreign-Key-Support>`__
+Foreign key relationships should work as expected, especially relationships
+from child to parents are well supported in querysets, but mapping
+Salesforce SOQL to a purely-relational mapper is a leaky abstraction
+and some knowledge about limitations of SOQL is useful. Some rejected
+queries should be usually rewritten to two simpler queries.
+For the gory details, see
+`Foreign Key Support <https://github.com/django-salesforce/django-salesforce/wiki/Foreign-Key-Support>`__
 on the Django-Salesforce wiki.
 
 Introspection and special attributes of fields
 ----------------------------------------------
 Some Salesforce fields can not be fully used without special attributes, namely
-read-only and default value fields. Further details can be found in
+read-only fields and some default values. Further details can be found in
 `Introspection and Special Attributes of Fields <https://github.com/django-salesforce/django-salesforce/wiki/Introspection-and-Special-Attributes-of-Fields>`__
 
 Caveats
 -------
 
 The ultimate goal of development of this package is to support reasonable
 new features of the Salesforce platform and of new Django versions,
@@ -273,26 +297,34 @@
    very simplified only for example and documentation purposes and for tests.)
 -  **Inheritance** — When using the default router, all models Salesforce
    must extend salesforce.models.SalesforceModel. The model router checks
    for this to determine which models to handle through the Salesforce
    connection.
 -  **Database Migrations** — ``migrate`` will create new tables only in non-SF
    databases (useful for unit tests); SFDC tables are assumed to already
-   exist with the appropriate permissions.
+   exist with the appropriate permissions. (A very incomplete implementation
+   of migrations in Salesforce has been in a development repository around
+   for two years. I am satisfied for my purposes. Development for better
+   general usability is the main reason why am I trying to get sponsors.)
 
 -  **Unsupported methods**: Queryset methods ``union()``, ``difference()``,
-    ``intersection()`` and ``distinct()``
-    are e.g. not supported because SOQL doesn't support corresponding operators:
-    UNION, EXCEPT, INTERSECT and DISTINCT.
+   ``intersection()`` and ``distinct()``
+   are e.g. not supported because SOQL doesn't support corresponding operators:
+   UNION, EXCEPT, INTERSECT and DISTINCT.
 
 Backwards-incompatible changes
 ------------------------------
 
 The most important:
 
+-  v4.2: Some new features implemented after June 2023 can require a license key
+   (sponsorship) or to accept the AGPL license. (AGPL is fine for exclusive open source
+   contribution or for education, but impossible if you do not share all your
+   source codes.)
+
 -  v4.0: Removed support for Python 3.5
 
 -  v3.2: Removed support for Django 1.11
 
 -  v1.0: The object ``salesforce.backend.operations.DefaultedOnCreate`` in an incidental
    old migration should be rewritten to new ``salesforce.fields.DefaultedOnCreate``, but
    old migrations are unnecessary usually.
```

### Comparing `django-salesforce-4.1/README.rst` & `django-salesforce-4.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 django-salesforce
 =================
 
-.. image:: https://travis-ci.com/django-salesforce/django-salesforce.svg?branch=master
-   :target: https://travis-ci.com/django-salesforce/django-salesforce
+.. image:: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml
 
 .. image:: https://badge.fury.io/py/django-salesforce.svg
    :target: https://pypi.python.org/pypi/django-salesforce
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue
    :target: https://www.python.org/
 
-.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1-blue.svg
+.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2-blue.svg
    :target: https://www.djangoproject.com/
 
 This library allows you to load, edit and query the objects in any Salesforce instance
 using Django models. The integration is fairly complete, and generally seamless
 for most uses. It works by integrating with the Django ORM, allowing access to
 the objects in your SFDC instance (Salesforce .com) as if they were in a
 traditional database.
 
-Python 3.6 to 3.10, Django 2.0 to 4.1. (Tested also with Python 3.11 beta 4)
+Python 3.7 to 3.11, Django 2.0 to 4.2. (Tested also with Python 3.12 beta 3)
+
+Use with Django 4.2 currently requires an enteprise license key DJSF_LICENSE_KEY
+available to sponsors, or to accept an AGPL license if you install our equivalent
+package "django-salesforce-agpl" instead.
 
 
 Quick Start
 -----------
 
 Install, configure a Salesforce connection, create a Salesforce model and run.
 
-1. Install django-salesforce: ``pip install django-salesforce``
+1. **Install** django-salesforce: ``pip install django-salesforce``
 
-2. Add a salesforce connection to your ``DATABASES`` setting::
+2. Add a Salesforce **connection** to your ``DATABASES`` **setting**::
 
     'salesforce': {
         'ENGINE': 'salesforce.backend',
         'CONSUMER_KEY': '',                # 'client_id'   in OAuth2 terminology
         'CONSUMER_SECRET': '',             # 'client_secret'
         'USER': '',
         'PASSWORD': '',
@@ -43,44 +47,33 @@
    In the example above, all fields should be populated as follows:
 
    * ``CONSUMER_KEY`` and ``CONSUMER_SECRET`` values are for the app used to
      connect to your Salesforce account. Instructions for how get these are in
      the Salesforce REST API Documentation. Key and secret can be created on
      web by:
 
-     - Salesforce Classic > Setup > App Setup > Create > Apps > Connected apps >
+     - SalesForce **Lightning** > Setup > Apps > App Manager > New Connected App or by
+       Salesforce **Classic** > Setup > App Setup > Create > Apps > Connected apps >
        New.  
-       or SalesForce Lightning > Setup > Apps > App Manager > New Connected App.
      - Click "Enable OAuth Settings" in API, then select "Access and manage
        your data (api)" from available OAuth Scopes.
      - Other red marked fields must be filled, but are not relevant for Django
        with password authentication. ("Callback URL" should be a safe URL
-       that maybe doesn't exist, but is under your control and doesn't redirect,
-       for the case that you accidentally activate other OAuth mode later.)
+       that maybe doesn't exist now, but its path is under your control and
+       doesn't redirect. This would be important if you activate other OAuth
+       mode later.)
    * ``USER`` is the username used to connect.
    * ``PASSWORD`` is a concatenation of the user's password and security token.
      Security token can be set by My Settings / Personal / Reset My Security Token
      or an new token is received by email after every password change.
      Security token can be omitted if the local IP address has been
      whitelisted in Security Controls / Network Access.
    * ``HOST`` is ``https://test.salesforce.com`` to access a sandbox, or
-     ``https://login.salesforce.com`` to access production.
-
-   If an error occurs in a request to Salesforce, review the received error message
-   that is exactly copied between braces ``{...}`` from the
-   Salesforce response to a Python exception to assist debugging.
-
-   See also: `Information on settings up Salesforce connected apps
-   <https://help.salesforce.com/apex/HTViewHelpDoc?id=connected_app_create.htm>`_
-   if necessary.
-
-   **Note about permissions**: Administrator rights are only required to run
-   the full suite of unit tests; otherwise, as long as the account has rights to
-   read or modify the chosen object, everything should work properly.
-   Introspection by ``inspectdb`` doesn't require any object permissions.
+     ``https://login.salesforce.com`` to access production or your domain
+     ``https://MyDomainName.my.salesforce.com``.
 
 3. Add ``salesforce.router.ModelRouter`` to your ``DATABASE_ROUTERS``
    setting::
 
     DATABASE_ROUTERS = [
         "salesforce.router.ModelRouter"
     ]
@@ -99,79 +92,106 @@
         "salesforce"
     }
 
    (This is necessary for running Salesforce extensions in the command
    ``inspectdb --database=salesforce`` in development, otherwise it is
    not important.)
 
+5. Add a setting ``DJSF_LICENSE_KEY = "Your Name or Company / email //our.signature=="``
+   if you need it for Django 4.2 now.
+
+6. **Verify** that everything important is configured correctly by running
+   the command ``python manage.py check --database=salesforce``.
+   You get eventualy the important information about problems related to the previous
+   steps. (clearly without tracebacks)
+
+   That is useful again after you define your database model or if you customize your
+   configuration later and e.g. you configure multiple Salesforce databases.
 
-5. Define a model that extends ``salesforce.models.Model`` (alias ``SalesforceModel``)
+7. Define a **model** that extends ``salesforce.models.Model`` (alias ``SalesforceModel``)
    or export the complete SF schema by ``python manage.py inspectdb --database=salesforce``
-   and simplify it to what you need. The full models file is about 2 MB with 500 models
+   and simplify it to what you need. The full models file is about 1.5 MB with 500 models
    and the export takes 2 minutes, but it is a valid models module that works without
    modification. The output of command ``inspectdb`` can be restricted by a list
    of table_names on the command line, but also ForeignKey fields to omitted models
    must be pruned to get a valid complete small model.
 
-6. **(optional)** To override the default timeout of 15 seconds,
-   define ``SALESFORCE_QUERY_TIMEOUT`` in your settings file.
-   It can be one number or better a tuple with a short value for connection
-   timeout and a longer value that includes time for running a query.
-   It never need be longer than 30 seconds::
+8. **You're all done!** Just use your model like a normal Django model.
 
-    SALESFORCE_QUERY_TIMEOUT = (4, 15)  # default (connect timeout, data timeout)
+   If an error occurs in a request to Salesforce, review the received error message
+   that is exactly copied between braces ``{...}`` from the
+   Salesforce response to a Python exception to assist debugging.
+
+   See also: `Information on settings up Salesforce connected apps
+   <https://help.salesforce.com/apex/HTViewHelpDoc?id=connected_app_create.htm>`_
+   if necessary.
+
+   **Note about permissions**: Administrator profile are only required to run
+   the full suite of unit tests of this framework; otherwise, as long as
+   the account has rights to read or modify the chosen object, everything
+   should work properly. Introspection by ``inspectdb`` doesn't require any
+   additional object permissions.
+
+
+Optional small features
+-----------------------
 
-7. **(optional)** If you want to use another name for your Salesforce DB
+-  **Salesforce alias** If you want to use another name for your Salesforce DB
    connection, define ``SALESFORCE_DB_ALIAS`` in your settings file::
 
     SALESFORCE_DB_ALIAS = 'salesforce'  # default
 
-8. You're all done! Just use your model like a normal Django model.
+-  **Timeout settings** To override the default timeout of 15 seconds,
+   define ``SALESFORCE_QUERY_TIMEOUT`` in your settings file.
+   It can be one number or better a tuple with a short value for connection
+   timeout and a longer value that includes time for running a query.
+   It never need be longer than 30 seconds::
 
-9. **(optional)** Create a normal Django ``admin.py`` module for your Salesforce models
+    SALESFORCE_QUERY_TIMEOUT = (4, 15)  # default (connect timeout, data timeout)
+
+-  **Automatic stupid admin** Create a normal Django ``admin.py`` module for your Salesforce models
    and you can register a minimalistic admin for all omitted Admin classes::
 
     from salesforce.testrunner.example.universal_admin import register_omitted_classes
     # some admin classes that you wrote manually yet
     # ...
     # end of file
     register_omitted_classes(your_application.models)
 
    This is a rudimentary way to verify that every model works in a sandbox, before
    hand-writing all admin classes. (Foreign keys to huge tables in the production
    require a customized admin e.g. with search widgets.)
     
-10. **(optional)** By default, the Django ORM connects to all DBs at startup. To delay
+-   **Lazy connect** By default, the Django ORM connects to all DBs at startup. To delay
     SFDC connections until they are actually required, define ``SF_LAZY_CONNECT=True``
     in your settings file. Be careful when using this setting; since it won't fail during
     the application boot, it's possible for a bad password to be sent repeatedly,
     requiring an account reset to fix.
 
-Primary Key
------------
-Salesforce doesn't allow you to define custom primary keys, so django-salesforce
-will add them automatically in all cases. You can override only capitalization and use
-a primary key ``Id`` by configuring ``SF_PK='Id'`` in your project settings
-if you prefer Salesforce capitalized field name conventions instead of Django
-default ``id``.
+-  **Configurable Primary Key**
+   Salesforce doesn't allow you to define custom primary keys, so django-salesforce
+   will add them automatically in all cases. You can override only capitalization and use
+   a primary key ``Id`` by configuring ``SF_PK='Id'`` in your project settings
+   if you prefer Salesforce capitalized field name conventions instead of Django
+   default ``id``.
 
 Advanced usage
 --------------
 -  **Multiple Inheritance from Abstract Models** - Many Salesforce models use
    the same sets of fields, but using a single inheritance tree would be too
    complicated and fragile. Proxy models and mixins are also supported.
 
 -  **Testing** - By default, tests will be run against the SFDC connection
    specified in settings.py, which will substantially increase testing time.
 
    One way to speed this up is to change the SALESFORCE_DB_ALIAS to point to
    another DB connection (preferably SQLite) during testing using the
    ``TEST`` settings variable. Such simple tests can run without any network
-   access. Django unit tests without SalesforceModel
-   are fast everytimes. Special read only fields that are updated only by SFDC
+   access. Django unit tests without SalesforceModel are fast everytimes.
+   Special read only fields (with ``sf_read_only=...``) that are updated only by SFDC
    e.g. ``last_modified_date`` need more parameters to be possible to save them
    into an alternate database, e.g. by ``auto_now=True`` or to play with
    ``null=True`` or ``default=...``.
    
 -  **Multiple SFDC connections** - In most cases, a single connection is all
    that most apps require, so the default DB connection to use for Salesforce
    is defined by the ``SALESFORCE_DB_ALIAS`` settings variable. This behavior
@@ -226,23 +246,27 @@
    exceptions are raised by Django-Salesforce to get more useful information.
    General exceptions are ``SalesforceError`` or a more general custom
    ``DatabaseError``. They can be imported from ``salesforce.dbapi.exceptions``
    if database errors should be handled specifically in your app.
 
 Foreign Key Support
 -------------------
-Foreign key relationships should work as expected, but mapping
-Salesforce SOQL to a purely-relational mapper is a leaky abstraction. For the
-gory details, see `Foreign Key Support <https://github.com/django-salesforce/django-salesforce/wiki/Foreign-Key-Support>`__
+Foreign key relationships should work as expected, especially relationships
+from child to parents are well supported in querysets, but mapping
+Salesforce SOQL to a purely-relational mapper is a leaky abstraction
+and some knowledge about limitations of SOQL is useful. Some rejected
+queries should be usually rewritten to two simpler queries.
+For the gory details, see
+`Foreign Key Support <https://github.com/django-salesforce/django-salesforce/wiki/Foreign-Key-Support>`__
 on the Django-Salesforce wiki.
 
 Introspection and special attributes of fields
 ----------------------------------------------
 Some Salesforce fields can not be fully used without special attributes, namely
-read-only and default value fields. Further details can be found in
+read-only fields and some default values. Further details can be found in
 `Introspection and Special Attributes of Fields <https://github.com/django-salesforce/django-salesforce/wiki/Introspection-and-Special-Attributes-of-Fields>`__
 
 Caveats
 -------
 
 The ultimate goal of development of this package is to support reasonable
 new features of the Salesforce platform and of new Django versions,
@@ -257,26 +281,34 @@
    very simplified only for example and documentation purposes and for tests.)
 -  **Inheritance** — When using the default router, all models Salesforce
    must extend salesforce.models.SalesforceModel. The model router checks
    for this to determine which models to handle through the Salesforce
    connection.
 -  **Database Migrations** — ``migrate`` will create new tables only in non-SF
    databases (useful for unit tests); SFDC tables are assumed to already
-   exist with the appropriate permissions.
+   exist with the appropriate permissions. (A very incomplete implementation
+   of migrations in Salesforce has been in a development repository around
+   for two years. I am satisfied for my purposes. Development for better
+   general usability is the main reason why am I trying to get sponsors.)
 
 -  **Unsupported methods**: Queryset methods ``union()``, ``difference()``,
-    ``intersection()`` and ``distinct()``
-    are e.g. not supported because SOQL doesn't support corresponding operators:
-    UNION, EXCEPT, INTERSECT and DISTINCT.
+   ``intersection()`` and ``distinct()``
+   are e.g. not supported because SOQL doesn't support corresponding operators:
+   UNION, EXCEPT, INTERSECT and DISTINCT.
 
 Backwards-incompatible changes
 ------------------------------
 
 The most important:
 
+-  v4.2: Some new features implemented after June 2023 can require a license key
+   (sponsorship) or to accept the AGPL license. (AGPL is fine for exclusive open source
+   contribution or for education, but impossible if you do not share all your
+   source codes.)
+
 -  v4.0: Removed support for Python 3.5
 
 -  v3.2: Removed support for Django 1.11
 
 -  v1.0: The object ``salesforce.backend.operations.DefaultedOnCreate`` in an incidental
    old migration should be rewritten to new ``salesforce.fields.DefaultedOnCreate``, but
    old migrations are unnecessary usually.
```

### Comparing `django-salesforce-4.1/coverage_run.sh` & `django-salesforce-4.2/coverage_run.sh`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 $COVERAGE run -a $SOURCE manage.py inspectdb --database=salesforce Account >/dev/null
 $COVERAGE run -a $SOURCE manage.py inspectdb --database=salesforce --table-filter=Account >/dev/null
 $COVERAGE run -a $SOURCE manage.py inspectdb --database=salesforce --tooling-api >/dev/null
 $COVERAGE run -a $SOURCE manage.py makemigrations
 $COVERAGE run -a $SOURCE manage.py migrate --database=default
 $COVERAGE run -a $SOURCE manage.py check --settings=tests.tooling.settings
 
-for x in dj20-py36 dj22-py38 dj31-py39 dj40-py310; do
+for x in dj20-py37 dj22-py38 dj31-py39 dj40-py310; do
     echo "*** $x ***"
     .tox/${x}/bin/coverage run -a $SOURCE manage.py inspectdb --database=salesforce >/dev/null
     .tox/${x}/bin/coverage run -a $SOURCE manage.py test salesforce
 done
 for DIR in tests/test_* tests/no_salesforce tests/t_debug_toolbar tests/no_django_dbapi; do
     x=${DIR//\//.}
     TESTS=$(find $DIR -name \*test\*.py)
```

### Comparing `django-salesforce-4.1/django_salesforce.egg-info/PKG-INFO` & `django-salesforce-4.2/django_salesforce.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 Metadata-Version: 2.1
 Name: django-salesforce
-Version: 4.1
+Version: 4.2
 Summary: a Salesforce backend for Django's ORM
 Home-page: https://github.com/django-salesforce/django-salesforce
-Author: Freelancers Union
-Author-email: devs@freelancersunion.org
+Author: Hynek Cernoch
+Author-email: hynek@sdb.cz
 Maintainer: Phil Christensen
 Maintainer-email: phil@bubblehouse.org
-License: MIT
+License: AGPL
 Keywords: django salesforce orm backend
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.md
 
 django-salesforce
 =================
 
-.. image:: https://travis-ci.com/django-salesforce/django-salesforce.svg?branch=master
-   :target: https://travis-ci.com/django-salesforce/django-salesforce
+.. image:: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml
 
 .. image:: https://badge.fury.io/py/django-salesforce.svg
    :target: https://pypi.python.org/pypi/django-salesforce
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue
    :target: https://www.python.org/
 
-.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1-blue.svg
+.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2-blue.svg
    :target: https://www.djangoproject.com/
 
 This library allows you to load, edit and query the objects in any Salesforce instance
 using Django models. The integration is fairly complete, and generally seamless
 for most uses. It works by integrating with the Django ORM, allowing access to
 the objects in your SFDC instance (Salesforce .com) as if they were in a
 traditional database.
 
-Python 3.6 to 3.10, Django 2.0 to 4.1. (Tested also with Python 3.11 beta 4)
+Python 3.7 to 3.11, Django 2.0 to 4.2. (Tested also with Python 3.12 beta 3)
+
+Use with Django 4.2 currently requires an enteprise license key DJSF_LICENSE_KEY
+available to sponsors, or to accept an AGPL license if you install our equivalent
+package "django-salesforce-agpl" instead.
 
 
 Quick Start
 -----------
 
 Install, configure a Salesforce connection, create a Salesforce model and run.
 
-1. Install django-salesforce: ``pip install django-salesforce``
+1. **Install** django-salesforce: ``pip install django-salesforce``
 
-2. Add a salesforce connection to your ``DATABASES`` setting::
+2. Add a Salesforce **connection** to your ``DATABASES`` **setting**::
 
     'salesforce': {
         'ENGINE': 'salesforce.backend',
         'CONSUMER_KEY': '',                # 'client_id'   in OAuth2 terminology
         'CONSUMER_SECRET': '',             # 'client_secret'
         'USER': '',
         'PASSWORD': '',
@@ -59,44 +63,33 @@
    In the example above, all fields should be populated as follows:
 
    * ``CONSUMER_KEY`` and ``CONSUMER_SECRET`` values are for the app used to
      connect to your Salesforce account. Instructions for how get these are in
      the Salesforce REST API Documentation. Key and secret can be created on
      web by:
 
-     - Salesforce Classic > Setup > App Setup > Create > Apps > Connected apps >
+     - SalesForce **Lightning** > Setup > Apps > App Manager > New Connected App or by
+       Salesforce **Classic** > Setup > App Setup > Create > Apps > Connected apps >
        New.  
-       or SalesForce Lightning > Setup > Apps > App Manager > New Connected App.
      - Click "Enable OAuth Settings" in API, then select "Access and manage
        your data (api)" from available OAuth Scopes.
      - Other red marked fields must be filled, but are not relevant for Django
        with password authentication. ("Callback URL" should be a safe URL
-       that maybe doesn't exist, but is under your control and doesn't redirect,
-       for the case that you accidentally activate other OAuth mode later.)
+       that maybe doesn't exist now, but its path is under your control and
+       doesn't redirect. This would be important if you activate other OAuth
+       mode later.)
    * ``USER`` is the username used to connect.
    * ``PASSWORD`` is a concatenation of the user's password and security token.
      Security token can be set by My Settings / Personal / Reset My Security Token
      or an new token is received by email after every password change.
      Security token can be omitted if the local IP address has been
      whitelisted in Security Controls / Network Access.
    * ``HOST`` is ``https://test.salesforce.com`` to access a sandbox, or
-     ``https://login.salesforce.com`` to access production.
-
-   If an error occurs in a request to Salesforce, review the received error message
-   that is exactly copied between braces ``{...}`` from the
-   Salesforce response to a Python exception to assist debugging.
-
-   See also: `Information on settings up Salesforce connected apps
-   <https://help.salesforce.com/apex/HTViewHelpDoc?id=connected_app_create.htm>`_
-   if necessary.
-
-   **Note about permissions**: Administrator rights are only required to run
-   the full suite of unit tests; otherwise, as long as the account has rights to
-   read or modify the chosen object, everything should work properly.
-   Introspection by ``inspectdb`` doesn't require any object permissions.
+     ``https://login.salesforce.com`` to access production or your domain
+     ``https://MyDomainName.my.salesforce.com``.
 
 3. Add ``salesforce.router.ModelRouter`` to your ``DATABASE_ROUTERS``
    setting::
 
     DATABASE_ROUTERS = [
         "salesforce.router.ModelRouter"
     ]
@@ -115,79 +108,106 @@
         "salesforce"
     }
 
    (This is necessary for running Salesforce extensions in the command
    ``inspectdb --database=salesforce`` in development, otherwise it is
    not important.)
 
+5. Add a setting ``DJSF_LICENSE_KEY = "Your Name or Company / email //our.signature=="``
+   if you need it for Django 4.2 now.
+
+6. **Verify** that everything important is configured correctly by running
+   the command ``python manage.py check --database=salesforce``.
+   You get eventualy the important information about problems related to the previous
+   steps. (clearly without tracebacks)
+
+   That is useful again after you define your database model or if you customize your
+   configuration later and e.g. you configure multiple Salesforce databases.
 
-5. Define a model that extends ``salesforce.models.Model`` (alias ``SalesforceModel``)
+7. Define a **model** that extends ``salesforce.models.Model`` (alias ``SalesforceModel``)
    or export the complete SF schema by ``python manage.py inspectdb --database=salesforce``
-   and simplify it to what you need. The full models file is about 2 MB with 500 models
+   and simplify it to what you need. The full models file is about 1.5 MB with 500 models
    and the export takes 2 minutes, but it is a valid models module that works without
    modification. The output of command ``inspectdb`` can be restricted by a list
    of table_names on the command line, but also ForeignKey fields to omitted models
    must be pruned to get a valid complete small model.
 
-6. **(optional)** To override the default timeout of 15 seconds,
-   define ``SALESFORCE_QUERY_TIMEOUT`` in your settings file.
-   It can be one number or better a tuple with a short value for connection
-   timeout and a longer value that includes time for running a query.
-   It never need be longer than 30 seconds::
+8. **You're all done!** Just use your model like a normal Django model.
 
-    SALESFORCE_QUERY_TIMEOUT = (4, 15)  # default (connect timeout, data timeout)
+   If an error occurs in a request to Salesforce, review the received error message
+   that is exactly copied between braces ``{...}`` from the
+   Salesforce response to a Python exception to assist debugging.
+
+   See also: `Information on settings up Salesforce connected apps
+   <https://help.salesforce.com/apex/HTViewHelpDoc?id=connected_app_create.htm>`_
+   if necessary.
+
+   **Note about permissions**: Administrator profile are only required to run
+   the full suite of unit tests of this framework; otherwise, as long as
+   the account has rights to read or modify the chosen object, everything
+   should work properly. Introspection by ``inspectdb`` doesn't require any
+   additional object permissions.
+
+
+Optional small features
+-----------------------
 
-7. **(optional)** If you want to use another name for your Salesforce DB
+-  **Salesforce alias** If you want to use another name for your Salesforce DB
    connection, define ``SALESFORCE_DB_ALIAS`` in your settings file::
 
     SALESFORCE_DB_ALIAS = 'salesforce'  # default
 
-8. You're all done! Just use your model like a normal Django model.
+-  **Timeout settings** To override the default timeout of 15 seconds,
+   define ``SALESFORCE_QUERY_TIMEOUT`` in your settings file.
+   It can be one number or better a tuple with a short value for connection
+   timeout and a longer value that includes time for running a query.
+   It never need be longer than 30 seconds::
 
-9. **(optional)** Create a normal Django ``admin.py`` module for your Salesforce models
+    SALESFORCE_QUERY_TIMEOUT = (4, 15)  # default (connect timeout, data timeout)
+
+-  **Automatic stupid admin** Create a normal Django ``admin.py`` module for your Salesforce models
    and you can register a minimalistic admin for all omitted Admin classes::
 
     from salesforce.testrunner.example.universal_admin import register_omitted_classes
     # some admin classes that you wrote manually yet
     # ...
     # end of file
     register_omitted_classes(your_application.models)
 
    This is a rudimentary way to verify that every model works in a sandbox, before
    hand-writing all admin classes. (Foreign keys to huge tables in the production
    require a customized admin e.g. with search widgets.)
     
-10. **(optional)** By default, the Django ORM connects to all DBs at startup. To delay
+-   **Lazy connect** By default, the Django ORM connects to all DBs at startup. To delay
     SFDC connections until they are actually required, define ``SF_LAZY_CONNECT=True``
     in your settings file. Be careful when using this setting; since it won't fail during
     the application boot, it's possible for a bad password to be sent repeatedly,
     requiring an account reset to fix.
 
-Primary Key
------------
-Salesforce doesn't allow you to define custom primary keys, so django-salesforce
-will add them automatically in all cases. You can override only capitalization and use
-a primary key ``Id`` by configuring ``SF_PK='Id'`` in your project settings
-if you prefer Salesforce capitalized field name conventions instead of Django
-default ``id``.
+-  **Configurable Primary Key**
+   Salesforce doesn't allow you to define custom primary keys, so django-salesforce
+   will add them automatically in all cases. You can override only capitalization and use
+   a primary key ``Id`` by configuring ``SF_PK='Id'`` in your project settings
+   if you prefer Salesforce capitalized field name conventions instead of Django
+   default ``id``.
 
 Advanced usage
 --------------
 -  **Multiple Inheritance from Abstract Models** - Many Salesforce models use
    the same sets of fields, but using a single inheritance tree would be too
    complicated and fragile. Proxy models and mixins are also supported.
 
 -  **Testing** - By default, tests will be run against the SFDC connection
    specified in settings.py, which will substantially increase testing time.
 
    One way to speed this up is to change the SALESFORCE_DB_ALIAS to point to
    another DB connection (preferably SQLite) during testing using the
    ``TEST`` settings variable. Such simple tests can run without any network
-   access. Django unit tests without SalesforceModel
-   are fast everytimes. Special read only fields that are updated only by SFDC
+   access. Django unit tests without SalesforceModel are fast everytimes.
+   Special read only fields (with ``sf_read_only=...``) that are updated only by SFDC
    e.g. ``last_modified_date`` need more parameters to be possible to save them
    into an alternate database, e.g. by ``auto_now=True`` or to play with
    ``null=True`` or ``default=...``.
    
 -  **Multiple SFDC connections** - In most cases, a single connection is all
    that most apps require, so the default DB connection to use for Salesforce
    is defined by the ``SALESFORCE_DB_ALIAS`` settings variable. This behavior
@@ -242,23 +262,27 @@
    exceptions are raised by Django-Salesforce to get more useful information.
    General exceptions are ``SalesforceError`` or a more general custom
    ``DatabaseError``. They can be imported from ``salesforce.dbapi.exceptions``
    if database errors should be handled specifically in your app.
 
 Foreign Key Support
 -------------------
-Foreign key relationships should work as expected, but mapping
-Salesforce SOQL to a purely-relational mapper is a leaky abstraction. For the
-gory details, see `Foreign Key Support <https://github.com/django-salesforce/django-salesforce/wiki/Foreign-Key-Support>`__
+Foreign key relationships should work as expected, especially relationships
+from child to parents are well supported in querysets, but mapping
+Salesforce SOQL to a purely-relational mapper is a leaky abstraction
+and some knowledge about limitations of SOQL is useful. Some rejected
+queries should be usually rewritten to two simpler queries.
+For the gory details, see
+`Foreign Key Support <https://github.com/django-salesforce/django-salesforce/wiki/Foreign-Key-Support>`__
 on the Django-Salesforce wiki.
 
 Introspection and special attributes of fields
 ----------------------------------------------
 Some Salesforce fields can not be fully used without special attributes, namely
-read-only and default value fields. Further details can be found in
+read-only fields and some default values. Further details can be found in
 `Introspection and Special Attributes of Fields <https://github.com/django-salesforce/django-salesforce/wiki/Introspection-and-Special-Attributes-of-Fields>`__
 
 Caveats
 -------
 
 The ultimate goal of development of this package is to support reasonable
 new features of the Salesforce platform and of new Django versions,
@@ -273,26 +297,34 @@
    very simplified only for example and documentation purposes and for tests.)
 -  **Inheritance** — When using the default router, all models Salesforce
    must extend salesforce.models.SalesforceModel. The model router checks
    for this to determine which models to handle through the Salesforce
    connection.
 -  **Database Migrations** — ``migrate`` will create new tables only in non-SF
    databases (useful for unit tests); SFDC tables are assumed to already
-   exist with the appropriate permissions.
+   exist with the appropriate permissions. (A very incomplete implementation
+   of migrations in Salesforce has been in a development repository around
+   for two years. I am satisfied for my purposes. Development for better
+   general usability is the main reason why am I trying to get sponsors.)
 
 -  **Unsupported methods**: Queryset methods ``union()``, ``difference()``,
-    ``intersection()`` and ``distinct()``
-    are e.g. not supported because SOQL doesn't support corresponding operators:
-    UNION, EXCEPT, INTERSECT and DISTINCT.
+   ``intersection()`` and ``distinct()``
+   are e.g. not supported because SOQL doesn't support corresponding operators:
+   UNION, EXCEPT, INTERSECT and DISTINCT.
 
 Backwards-incompatible changes
 ------------------------------
 
 The most important:
 
+-  v4.2: Some new features implemented after June 2023 can require a license key
+   (sponsorship) or to accept the AGPL license. (AGPL is fine for exclusive open source
+   contribution or for education, but impossible if you do not share all your
+   source codes.)
+
 -  v4.0: Removed support for Python 3.5
 
 -  v3.2: Removed support for Django 1.11
 
 -  v1.0: The object ``salesforce.backend.operations.DefaultedOnCreate`` in an incidental
    old migration should be rewritten to new ``salesforce.fields.DefaultedOnCreate``, but
    old migrations are unnecessary usually.
```

### Comparing `django-salesforce-4.1/django_salesforce.egg-info/SOURCES.txt` & `django-salesforce-4.2/django_salesforce.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 salesforce/router.py
 salesforce/utils.py
 salesforce/backend/__init__.py
 salesforce/backend/base.py
 salesforce/backend/client.py
 salesforce/backend/compiler.py
 salesforce/backend/creation.py
+salesforce/backend/enterprise.py
 salesforce/backend/features.py
 salesforce/backend/indep.py
 salesforce/backend/introspection.py
 salesforce/backend/manager.py
 salesforce/backend/models_lookups.py
 salesforce/backend/models_sql_query.py
 salesforce/backend/operations.py
@@ -89,18 +90,20 @@
 salesforce/tests/test_integration.py
 salesforce/tests/test_unit.py
 salesforce/tests/test_utils.py
 salesforce/tests/unit_tests/__init__.py
 salesforce/tests/unit_tests/test_qparser.py
 tests/__init__.py
 tests/clean_test_data.py
+tests/db.sqlite3
 tests/mypy.sh
 tests/no_urls.py
 tests/tests.sh
 tests/tests_no_django.sh
+tests/to_mock.py
 tests/inspectdb/__init__.py
 tests/inspectdb/admin.py
 tests/inspectdb/settings.py
 tests/inspectdb/slow_test.py
 tests/inspectdb/test.sh
 tests/inspectdb/tests.py
 tests/inspectdb/urls.py
@@ -119,14 +122,16 @@
 tests/t_debug_toolbar/__init__.py
 tests/t_debug_toolbar/models.py
 tests/t_debug_toolbar/settings.py
 tests/t_debug_toolbar/test.sh
 tests/t_debug_toolbar/tests.py
 tests/t_debug_toolbar/urls.py
 tests/t_debug_toolbar/views.py
+tests/t_debug_toolbar/small_app/models.py
+tests/t_debug_toolbar/small_app/urls.py
 tests/test_app_label/__init__.py
 tests/test_app_label/settings.py
 tests/test_app_label/test.sh
 tests/test_app_label/salesforce/__init__.py
 tests/test_app_label/salesforce/apps.py
 tests/test_app_label/salesforce/models.py
 tests/test_app_label/salesforce/tests.py
```

### Comparing `django-salesforce-4.1/docs/details.rst` & `django-salesforce-4.2/docs/details.rst`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/pylintrc` & `django-salesforce-4.2/pylintrc`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/auth.py` & `django-salesforce-4.2/salesforce/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 oauth login support for the Salesforce API
 
 All data are ascii str.
```

### Comparing `django-salesforce-4.1/salesforce/backend/__init__.py` & `django-salesforce-4.2/salesforce/backend/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 """
 Salesforce Database backend for Django.
 
 No code in this directory is used with standard databases, even if a standard
 database is used for running some application tests on objects defined by
@@ -36,19 +35,21 @@
 DJANGO_21_PLUS = django.VERSION[:2] >= (2, 1)
 DJANGO_22_PLUS = django.VERSION[:2] >= (2, 2)
 DJANGO_30_PLUS = django.VERSION[:2] >= (3, 0)
 DJANGO_31_PLUS = django.VERSION[:2] >= (3, 1)
 DJANGO_32_PLUS = django.VERSION[:2] >= (3, 2)
 DJANGO_40_PLUS = django.VERSION[:2] >= (4, 0)
 DJANGO_41_PLUS = django.VERSION[:2] >= (4, 1)
+DJANGO_42_PLUS = django.VERSION[:2] >= (4, 2)
+max_django = (4, 2)
 is_dev_version = django.VERSION[3:] and re.match('(alpha|beta|rc)', django.VERSION[3])
-if django.VERSION[:2] < (2, 0) or django.VERSION[:2] > (4, 1) and not is_dev_version:
-    raise ImportError("Django version between 2.0 and 4.1 is required "
+if django.VERSION[:2] < (2, 0) or django.VERSION[:2] > max_django and not is_dev_version:
+    raise ImportError("Django version between 2.0 and 4.2 is required "
                       "for this django-salesforce.")
     # Usually three or more blocking issues can be expected by every
     # new major Django version. Strict check before support is better.
 
     # New Django development versions are enabled without any restriction, but
-    # new stable Django versions must be verified before they can be enabled here.
+    # new stable Django versions must be verified before they are enabled here.
 
 
 log = logging.getLogger(__name__)
```

### Comparing `django-salesforce-4.1/salesforce/backend/base.py` & `django-salesforce-4.2/salesforce/backend/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Salesforce database backend for Django.  (like django,db.backends.*.base)
 """
 
 from typing import Any, Dict, Optional, TYPE_CHECKING
 
 from django.conf import settings
 from django.db.backends.base.base import BaseDatabaseWrapper
 
+from salesforce.backend import enterprise
 from salesforce.backend.client import DatabaseClient
 from salesforce.backend.creation import DatabaseCreation
 from salesforce.backend.features import DatabaseFeatures
 from salesforce.backend.validation import DatabaseValidation
 from salesforce.backend.operations import DatabaseOperations
 from salesforce.backend.introspection import DatabaseIntrospection
 from salesforce.backend.schema import DatabaseSchemaEditor
@@ -39,16 +39,17 @@
     """
     # pylint:disable=abstract-method,too-many-instance-attributes
     #     undefined abstract methods: _start_transaction_under_autocommit, is_usable
 
     vendor = 'salesforce'
     display_name = 'Salesforce'
 
-    # Operators [contains, startswithm, endswith] are incorrectly
-    # case insensitive like sqlite3.
+    # All string operators are case insensitive in SOQL. (that can not be fixed)
+    # The relevant part here is the operator, e.g. a simple "LIKE".
+    # An optional wilcard ('%') is managed by a universal Django code for an operand.
     operators = {
         'exact': '= %s',
         'iexact': 'LIKE %s',
         'contains': 'LIKE %s',
         'icontains': 'LIKE %s',
         # 'regex': 'REGEXP %s',  # unsupported
         # 'iregex': 'REGEXP %s',
@@ -91,14 +92,15 @@
         settings_dict = self.settings_dict
         params = settings_dict.copy()
         params.update(settings_dict['OPTIONS'])
         return params
 
     @async_unsafe
     def get_new_connection(self, conn_params: Dict[str, Any]) -> Database.RawConnection:
+        enterprise.check_license_in_latest_django()
         # simulated only a connection interface without connecting really
         return Database.connect(settings_dict=conn_params, alias=self.alias)
 
     def init_connection_state(self):
         pass  # nothing to init
 
     def _set_autocommit(self, autocommit):
```

### Comparing `django-salesforce-4.1/salesforce/backend/compiler.py` & `django-salesforce-4.2/salesforce/backend/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Generate queries using the SOQL dialect.  (like django.db.models.sql.compiler and  django.db.models.sql.where)
 """
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple
@@ -13,15 +12,16 @@
 from django.core.exceptions import EmptyResultSet
 from django.db import NotSupportedError
 from django.db.models.sql import compiler as sql_compiler, where as sql_where, constants, datastructures
 from django.db.models.sql.where import AND
 from django.db.transaction import TransactionManagementError
 
 import salesforce.backend.models_lookups   # noqa pylint:disable=unused-import # required for activation of lookups
-from salesforce.backend import DJANGO_21_PLUS, DJANGO_30_PLUS, DJANGO_31_PLUS, DJANGO_40_PLUS
+from salesforce.backend import DJANGO_21_PLUS, DJANGO_30_PLUS, DJANGO_31_PLUS, DJANGO_40_PLUS, DJANGO_42_PLUS
+from salesforce.backend.utils import FullResultSet
 from salesforce.dbapi import DatabaseError
 from salesforce.dbapi.subselect import AGGREGATION_WORDS
 # pylint:disable=no-else-return,too-many-branches,too-many-locals
 
 AliasMapItems = List[Tuple[
     Optional[str],
     str,
@@ -191,16 +191,22 @@
             else:
                 distinct_fields = self.get_distinct()  # type: ignore[assignment] # noqa
 
             # This must come after 'select', 'ordering', and 'distinct' -- see
             # docstring of get_from_clause() for details.
             from_, f_params = self.get_from_clause()
 
-            where, w_params = self.compile(self.where) if self.where is not None else ("", [])
-            having, h_params = self.compile(self.having) if self.having is not None else ("", [])
+            try:
+                where, w_params = self.compile(self.where) if self.where is not None else ("", [])
+            except FullResultSet:
+                where, w_params = "", []
+            try:
+                having, h_params = self.compile(self.having) if self.having is not None else ("", [])
+            except FullResultSet:
+                having, h_params = "", []
             params = []
             result = ['SELECT']
 
             if self.query.distinct:
                 if DJANGO_21_PLUS:
                     distinct_result, distinct_params = self.connection.ops.distinct_sql(
                         distinct_fields,
@@ -409,14 +415,16 @@
             full_needed, empty_needed = 1, len(self.children)
 
         for child in self.children:
             try:
                 sql, params = compiler.compile(child)
             except EmptyResultSet:
                 empty_needed -= 1
+            except FullResultSet:
+                full_needed -= 1
             else:
                 if sql:
 
                     # *** patch 2 (add) begin
                     # # translate the alias of child to SOQL name
                     sql = compiler.sf_fix_field(sql)
                     # *** patch 2 end
@@ -428,24 +436,30 @@
             # Check if this node matches nothing or everything.
             # First check the amount of full nodes and empty nodes
             # to make this node empty/full.
             # Now, check if this node is full/empty using the
             # counts.
             if empty_needed == 0:
                 if self.negated:
+                    if DJANGO_42_PLUS:
+                        raise FullResultSet
                     return '', []
                 else:
                     raise EmptyResultSet
             if full_needed == 0:
                 if self.negated:
                     raise EmptyResultSet
                 else:
+                    if DJANGO_42_PLUS:
+                        raise FullResultSet
                     return '', []
         conn = ' %s ' % self.connector
         sql_string = conn.join(result)
+        if DJANGO_42_PLUS and not sql_string:
+            raise FullResultSet
         if sql_string:
             if self.negated:
                 # *** patch 3 (remove) begin
                 # # Some backends (Oracle at least) need parentheses
                 # # around the inner SQL in the negated case, even if the
                 # # inner SQL contains just a single expression.
                 # sql_string = 'NOT (%s)' % sql_string
```

### Comparing `django-salesforce-4.1/salesforce/backend/creation.py` & `django-salesforce-4.2/salesforce/backend/creation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Automatic table creation is not supported by the Salesforce backend. (like django.db.backends.*.creation)
 """
 import logging
```

### Comparing `django-salesforce-4.1/salesforce/backend/features.py` & `django-salesforce-4.2/salesforce/backend/features.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 
     can_introspect_duration_field = False
     supports_partial_indexes = False
     supports_ignore_conflicts = True
 
     supports_select_for_update_with_limit = False
 
+    # support select combinators:
     supports_select_union = False
     supports_select_intersection = False
     supports_select_difference = False
 
+    supports_aggregate_filter_clause = False
+
     # features for Django 3.0
     can_create_inline_fk = False
 
     if DJANGO_30_PLUS:
         can_return_columns_from_insert = True
         can_return_rows_from_bulk_insert = True
     else:
@@ -68,7 +71,17 @@
     # django_test_expected_failures = set()  # maybe in the future
     # django_test_skips = {}
 
     supports_update_conflicts = False  # new in Django 4.1+
     supports_update_conflicts_with_target = False
     supports_logical_xor = False
     has_case_insensitive_like = True  # this is opposite to the default in Django 4.1+
+
+    allows_group_by_select_index = False  # new in Django 4.2+
+    schema_editor_uses_clientside_param_binding = False
+    requires_compound_order_by_subquery = False
+    # Does the backend support column and table comments?
+    supports_comments = False
+    # Does the backend support column comments in ADD COLUMN statements?
+    supports_comments_inline = False
+    # Does the backend support unlimited character columns?
+    supports_unlimited_charfield = False
```

### Comparing `django-salesforce-4.1/salesforce/backend/indep.py` & `django-salesforce-4.2/salesforce/backend/indep.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/backend/introspection.py` & `django-salesforce-4.2/salesforce/backend/introspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Salesforce introspection code.  (like django.db.backends.*.introspection)
 """
 
 import json
 import logging
 import re
 from collections import OrderedDict, namedtuple
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
+from django.conf import settings
 from django.db.backends.base.introspection import (
     BaseDatabaseIntrospection, FieldInfo as BaseFieldInfo, TableInfo,
 )
 from django.utils.text import camel_case_to_spaces
 from django.db.backends.utils import CursorWrapper as _Cursor  # for typing
 
 from salesforce.backend import DJANGO_22_PLUS, DJANGO_32_PLUS
@@ -222,15 +222,16 @@
         elif field['defaultedOnCreate'] and field['createable']:
             params['default'] = SymbolicModelsName('DEFAULTED_ON_CREATE')
 
         if field['inlineHelpText']:
             params['help_text'] = field['inlineHelpText']
         if field['picklistValues']:
             params['choices'] = [(x['value'], x['label']) for x in field['picklistValues'] if x['active']]
-            if len(repr(params['choices'])) < 4000:
+            max_inspectdb_picklist_picklist_length = getattr(settings, 'SF_MAX_INSPECTDB_PICKLIST_LENGTH', 4000)
+            if len(repr(params['choices'])) < max_inspectdb_picklist_picklist_length:
                 params['max_len'] = max(len(x['value']) for x in field['picklistValues'] if x['active'])
             else:
                 params['ref_comment'] = 'Too long choices skipped'
                 del params['choices']
         if field['type'] == 'reference' and not self.references_to(field):
             if not field['referenceTo']:
                 params['ref_comment'] = 'No Reference to a table'
```

### Comparing `django-salesforce-4.1/salesforce/backend/manager.py` & `django-salesforce-4.2/salesforce/backend/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Salesforce object manager. (like django.db.models.manager)
 
 Use a custom QuerySet to generate SOQL queries and results.
 
 This module requires a customized package django-stubs (django-salesforce-stubs)
 """
 
-import sys
 from typing import Generic, Optional, TypeVar
 from django.db.models import manager, Model
 from django.db.models.query import QuerySet  # pylint:disable=unused-import
 
 from salesforce import router
 from salesforce.backend import query
 
 _T = TypeVar("_T", bound=Model, covariant=True)
 
 
 class SalesforceManager(manager.Manager, Generic[_T]):
 
-    if sys.version_info[:2] < (3, 6):  # Python 3.5 - remove soon
-        # this is a fix for Generic type issue https://github.com/python/typing/issues/498
-        __copy__ = None
-
     def get_queryset(self, _alias: Optional[str] = None) -> 'QuerySet[_T]':
         """
         Returns a QuerySet which access remote SF objects.
         """
         alias_is_sf = _alias and router.is_sf_database(_alias)
         is_extended_model = getattr(self.model, '_salesforce_object', '') == 'extended'
         assert self.model is not None
```

### Comparing `django-salesforce-4.1/salesforce/backend/models_lookups.py` & `django-salesforce-4.2/salesforce/backend/models_lookups.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 Lookups  (like django.db.models.lookups, django.db.models.aggregates.Count)
 """
 from django.db import models
 from django.db.models.fields import Field
 from django.db.models import lookups
 
 
-class IsNull(models.lookups.IsNull):
+class IsNull(models.lookups.IsNull):  # pylint:disable=abstract-method
     def override_as_sql(self, compiler, connection):  # pylint:disable=unused-argument
         # it must be relabeled if used for a children rows set
         if compiler.soql_trans is None:
             compiler.get_from_clause()
         sql, params = compiler.compile(self.lhs.relabeled_clone(compiler.soql_trans))
         return ('%s %s null' % (sql, ('=' if self.rhs else '!='))), params
 
     setattr(models.lookups.IsNull, 'as_salesforce', override_as_sql)
 
 
-class Range(models.lookups.Range):
+class Range(models.lookups.Range):  # pylint:disable=abstract-method
     def override_as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
         rhs, rhs_params = self.process_rhs(compiler, connection)
         assert rhs == ('%s', '%s')
         assert len(rhs_params) == 2
         params = lhs_params + [rhs_params[0]] + lhs_params + [rhs_params[1]]
         # The symbolic parameters %s are again substituted by %s. The real
@@ -45,25 +45,25 @@
             sql = sql.replace('COUNT(DISTINCT ', 'COUNT_DISTINCT(')
         return sql, params
 
     setattr(models.aggregates.Count, 'as_salesforce', override_as_sql)
 
 
 @Field.register_lookup
-class NotIn(lookups.In):
+class NotIn(lookups.In):  # pylint:disable=abstract-method
     lookup_name = 'not_in'
 
     def get_rhs_op(self, connection, rhs):
         return 'NOT IN %s' % rhs
 
     def split_parameter_list_as_sql(self, compiler, connection):
         # this patch is a only for Oracle and never tested with it
         max_size = connection.ops.max_in_list_size()
         raise NotImplementedError("Lookup 'not_in' can't be used with lists longer then %d" % max_size)
 
 
 @Field.register_lookup
-class NotEqual(lookups.Exact):
+class NotEqual(lookups.Exact):  # pylint:disable=abstract-method
     lookup_name = 'not_eq'
 
     def get_rhs_op(self, connection, rhs):
         return '!= %s' % rhs
```

### Comparing `django-salesforce-4.1/salesforce/backend/models_sql_query.py` & `django-salesforce-4.2/salesforce/backend/models_sql_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 from typing import Any, cast, Generic, Optional, Sequence, Tuple, Type, TypeVar
 from django.conf import settings
 from django.db.models import Count, Model
 from django.db.models.sql import Query, RawQuery, constants
 import django
 
-from salesforce.backend import DJANGO_40_PLUS
+from salesforce.backend import DJANGO_40_PLUS, DJANGO_42_PLUS
 from salesforce.backend.compiler import SfParams, SQLCompiler
 from salesforce.dbapi.driver import arg_to_soql
 
 _T = TypeVar("_T", bound=Model, covariant=True)
 
 
 class SalesforceRawQuery(RawQuery):
@@ -130,12 +130,14 @@
 
     def get_count(self, using: str) -> int:
         """
         Performs a COUNT() query using the current filter constraints.
         """
         # customized because "Count('*')" is not possible with Salesforce and also not "__" in an alias
         obj = self.clone()
+        if DJANGO_42_PLUS:
+            return obj.get_aggregation(using, {"x_sf_count": Count("*")})["x_sf_count"]
         obj.add_annotation(Count('pk'), alias='x_sf_count', is_summary=True)  # pylint: disable=no-member
         number = obj.get_aggregation(using, ['x_sf_count'])['x_sf_count']  # type: Optional[int] # pylint: disable=no-member # noqa
         if number is None:
             number = 0
         return number
```

### Comparing `django-salesforce-4.1/salesforce/backend/operations.py` & `django-salesforce-4.2/salesforce/backend/operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 """
 DatabaseOperations  (like salesforce.db.backends.*.operations)
 """
 from typing import Optional
 import itertools
 import warnings
 
-import django.db.backends.utils
 from django.db.backends.base.operations import BaseDatabaseOperations
 from salesforce.backend import DJANGO_30_PLUS
 from salesforce.dbapi.exceptions import SalesforceWarning
 
 BULK_BATCH_SIZE = 200
 
 """
@@ -87,15 +85,17 @@
 
     def adapt_timefield_value(self, value):
         return value
 
     def adapt_decimalfield_value(self, value, max_digits=None, decimal_places=None):
         if hasattr(value, 'default'):  # DefaultedOnCreate
             return value
-        return django.db.backends.utils.format_number(value, max_digits, decimal_places)
+        if value is None:
+            return None
+        return float(value)
 
     def bulk_batch_size(self, fields, objs):
         return BULK_BATCH_SIZE
 
     # This SQL is not important because we currently control the insert from a Salesforce compiler,
     # but some method must exist.
     def bulk_insert_sql(self, fields, placeholder_rows):
```

### Comparing `django-salesforce-4.1/salesforce/backend/query.py` & `django-salesforce-4.2/salesforce/backend/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Salesforce object query and queryset customizations.  (like django.db.models.query)
 """
 from typing import Dict, Generic, Iterable, List, NoReturn, Optional, TYPE_CHECKING, Type, TypeVar
 import typing  # pylint:disable=unused-import
 
 from django.conf import settings
-from django.db import NotSupportedError, models
+from django.db import NotSupportedError, models, DEFAULT_DB_ALIAS
 from django.db.models import constants
 from django.db.models import query as models_query, Model
 from django.db.models.sql import where as sql_where
-from django.db.utils import DEFAULT_DB_ALIAS
 import django
 
 from salesforce.backend.indep import get_sf_alt_pk
 from salesforce.backend import compiler, DJANGO_22_PLUS, DJANGO_30_PLUS, DJANGO_40_PLUS, DJANGO_41_PLUS
 from salesforce.backend.models_sql_query import SalesforceQuery
 from salesforce.backend.operations import BULK_BATCH_SIZE
 from salesforce.router import is_sf_database
```

### Comparing `django-salesforce-4.1/salesforce/backend/schema.py` & `django-salesforce-4.2/salesforce/backend/schema.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/backend/test_helpers.py` & `django-salesforce-4.2/salesforce/backend/test_helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Common helpers for tests, like test decorators
 """
 import sys
 import uuid
 from unittest import skip, skipUnless, expectedFailure, TestCase  # NOQA pylint:disable=unused-import
+from typing import Union
 
 import django
 from django.conf import settings
 
 from salesforce import router
 from salesforce.dbapi.test_helpers import (  # NOQA pylint:disable=unused-import
     LazyTestMixin, expectedFailureIf, QuietSalesforceErrors)
@@ -15,8 +16,13 @@
 # uid strings for tests that accidentally run concurrent
 uid_random = '-' + str(uuid.uuid4())[:7]
 # this is the same as the name of tox test environment, e.g. 'dj30-py38'
 uid_version = 'dj{0}{1}-py{2}{3}'.format(*(django.VERSION[:2] + sys.version_info[:2]))
 
 sf_alias = getattr(settings, 'SALESFORCE_DB_ALIAS', 'salesforce')
 default_is_sf = router.is_sf_database(sf_alias)
-current_user = settings.DATABASES[sf_alias]['USER']
+current_user: str = settings.DATABASES[sf_alias].get('USER', '')
+
+
+def strtobool(val: Union[str, bool]) -> bool:
+    """instead of deprecated distutils.util.strtobool(...)"""
+    return str(val).lower() in ("y", "yes", "t", "true", "on", "1")
```

### Comparing `django-salesforce-4.1/salesforce/backend/utils.py` & `django-salesforce-4.2/salesforce/backend/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,27 @@
 import warnings
 from itertools import islice
 from typing import Any, Callable, Iterable, Iterator, List, Tuple, TypeVar, Union, overload
 
 from django.db import models, NotSupportedError
 from django.db.models.sql import subqueries, Query, RawQuery
 
-from salesforce.backend import DJANGO_30_PLUS
+from salesforce.backend import DJANGO_30_PLUS, DJANGO_42_PLUS
 from salesforce.dbapi.driver import (
     DatabaseError, InternalError, SalesforceWarning, merge_dict,
     register_conversion, arg_to_json)
 from salesforce.fields import NOT_UPDATEABLE, NOT_CREATEABLE
 
+if DJANGO_42_PLUS:
+    from django.core.exceptions import FullResultSet  # type: ignore[attr-defined] # pylint:disable=ungrouped-imports
+else:
+    class FullResultSet(Exception):  # type: ignore[no-redef]
+        pass
+
+
 V = TypeVar('V')
 if not DJANGO_30_PLUS:
     # a "do nothing" stub for Django < 3.0, where is no decorator @async_unsafe
     F = TypeVar('F', bound=Callable)
     F2 = TypeVar('F2', bound=Callable)
 
     @overload
@@ -278,15 +285,18 @@
                     "See docs wiki/error-messages")
                 # # alternative solution:
                 # return list(salesforce.backend.query.SalesforceQuerySet(pk.model, query=pk, using=pk._db))
 
                 sql, params = pks.get_compiler('salesforce').as_sql()
         if not sql:
             # a subquery is necessary in this case
-            where_sql, params = where.as_sql(query.get_compiler('salesforce'), self.db.connection)
+            try:
+                where_sql, params = where.as_sql(query.get_compiler('salesforce'), self.db.connection)
+            except FullResultSet:
+                where_sql, params = "", []
             sql = "SELECT Id FROM {}".format(query.model._meta.db_table)
             if where_sql:
                 sql += " WHERE {}".format(where_sql)
         with self.db.cursor() as cur:
             cur.execute(sql, params)
             assert len(cur.description) == 1 and cur.description[0][0] == 'Id'
             return [x[0] for x in cur]
```

### Comparing `django-salesforce-4.1/salesforce/dbapi/__init__.py` & `django-salesforce-4.2/salesforce/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/dbapi/common.py` & `django-salesforce-4.2/salesforce/dbapi/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,13 +53,13 @@
         self.data[domain] = t_new
         if do_call and callback:
             callback()
 
     @staticmethod
     def domain(url: str) -> str:
         match = re.match(r'^(?:https|mock)://([^/]*)/?', url)
-        assert match
+        assert match, "HOST must be including the protocol and :// like 'https://login.salesforce.com'"
         return match.groups()[0]
 
 
 time_statistics = TimeStatistics(300)
 thread_loc = threading.local()
```

### Comparing `django-salesforce-4.1/salesforce/dbapi/driver.py` & `django-salesforce-4.2/salesforce/dbapi/driver.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/dbapi/exceptions.py` & `django-salesforce-4.2/salesforce/dbapi/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,18 @@
     The messages are typically very cryptic. (probably intentionally,
     to not disclosure more information to unathorized persons)
 
     Repeated errors of this class can lock the user account temporarily.
     """
 
 
+class LicenseError(OperationalError):
+    pass
+
+
 def prepare_exception(obj: Union[Error, SalesforceWarning],
                       messages: Optional[Union[str, List[str]]] = None,
                       response: Optional[GenResponse] = None,
                       verbs: Optional[Iterable[str]] = None
                       ) -> str:
     """Prepare excetion params or only an exception message
```

### Comparing `django-salesforce-4.1/salesforce/dbapi/subselect.py` & `django-salesforce-4.2/salesforce/dbapi/subselect.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             elif issubclass(row_type, list):
                 yield [rowcount]  # originally [resp.json()['totalSize']]
             elif issubclass(row_type, tuple):
                 yield (rowcount,)
         else:
             for row_deep in records:
                 if list(row_deep.keys()) == ['explain']:
-                    yield row_deep['explain']
+                    yield (row_deep['explain'],)
                 else:
                     assert self.is_aggregation == (row_deep['attributes']['type'] == 'AggregateResult')
                     row_flat = self._make_flat(row_deep, path=(), subroots=self.subroots)
                     # TODO Will be the expression "or x['done']" really correct also for long subrequests?
                     assert all(not isinstance(x, dict) or x['done'] for x in row_flat)
                     if issubclass(row_type, dict):
                         yield {k: fix_data_type(row_flat[k.lower()]) for k in self.aliases}
```

### Comparing `django-salesforce-4.1/salesforce/dbapi/test_helpers.py` & `django-salesforce-4.2/salesforce/dbapi/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/defaults.py` & `django-salesforce-4.2/salesforce/defaults.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/fields.py` & `django-salesforce-4.2/salesforce/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Customized fields for Salesforce, especially the primary key. (like django.db.models.fields)
 """
```

### Comparing `django-salesforce-4.1/salesforce/management/commands/inspectdb.py` & `django-salesforce-4.2/salesforce/management/commands/inspectdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from typing import Any, Container, Dict, List, Mapping, Tuple
+from typing import Any, Container, Dict, List, Mapping, Optional, Tuple
 import argparse
 import re
 
 from django.core.management.commands.inspectdb import Command as InspectDBCommand
 from django.db import connections
 from salesforce.backend import introspection as sf_introspection
 
@@ -100,25 +100,28 @@
                     field_notes.append('Master Detail Relationship %s' % relationship_order)
                 field_params.update(fields_map)
         else:
             new_name, field_params, field_notes = super().normalize_col_name(col_name, used_column_names, is_relation)
         return new_name, field_params, field_notes
 
     # the parameter 'is_view' has been since Django 2.1 and 'is_partition' since Django 2.2
+    # the parameter 'comment' added in Django 4.2
     def get_meta(self, table_name: str, constraints: Any = None, column_to_field_name: Dict[str, str] = None,
-                 is_view: bool = False, is_partition: bool = False) -> List[str]:
+                 is_view: bool = False, is_partition: bool = False, comment: Optional[str] = None) -> List[str]:
         """
         Return a sequence comprising the lines of code necessary
         to construct the inner Meta class for the model corresponding
         to the given database table name.
         """
         # pylint:disable=arguments-differ,too-many-arguments,unused-argument
         meta = ["    class Meta(models.Model.Meta):",
                 "        db_table = '%s'" % table_name]
         if self.tooling_api:
             meta.append("        managed = False")
             meta.append("        sf_tooling_api_model = True")
+        if comment:
+            meta.append(f"        db_table_comment = {comment!r}")
         if self.connection.vendor == 'salesforce':
             for line in self.connection.introspection.get_additional_meta(table_name):
                 meta.append("        " + line)
         meta.append("")
         return meta
```

### Comparing `django-salesforce-4.1/salesforce/models.py` & `django-salesforce-4.2/salesforce/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Django models for accessing Salesforce objects. (like django.db.models)
 
 The Salesforce database is somewhat un-UNIXy or non-Pythonic, in that
```

### Comparing `django-salesforce-4.1/salesforce/models_extend.py` & `django-salesforce-4.2/salesforce/models_extend.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/models_template.py` & `django-salesforce-4.2/salesforce/models_template.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/router.py` & `django-salesforce-4.2/salesforce/router.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 """
 Database router for SalesforceModel objects.
 """
 
 from typing import cast, Optional, Type
 from django.apps import apps
 from django.conf import settings
-from django.db import models
+from django.db import models, DEFAULT_DB_ALIAS
 
 
 def is_sf_database(db: Optional[str], model: Optional[models.Model] = None) -> bool:
     """The alias is a Salesforce database."""
-    from django.db import connections  # pylint:disable=import-outside-toplevel
     if db is None:
         return hasattr(model, '_salesforce_object')
-    engine = cast(str, connections[db].settings_dict['ENGINE'])
-    return engine == 'salesforce.backend' or connections[db].vendor == 'salesforce'
+    # simple check to prevent a possible circular dependency
+    return 'salesforce' in settings.DATABASES[db]['ENGINE']
 
 
 class ModelRouter:
     """
     Database router for Salesforce models.
     """
     # pylint:disable=protected-access
@@ -41,55 +39,62 @@
         """
         if 'instance' in hints:
             db = hints['instance']._state.db
             if db:
                 return db
         if hasattr(model, '_salesforce_object'):
             return self.sf_alias
+        if model._meta.app_label == 'django_cache':
+            return DEFAULT_DB_ALIAS
         return None
 
     def db_for_write(self, model: models.Model, **hints: models.Model) -> Optional[str]:
         """
         If given some hints['instance'] that is saved in a db, use related
         fields from the same db. Otherwise if passed a class or instance to
         model, return the salesforce alias if it's a subclass of SalesforceModel.
         """
         if 'instance' in hints:
             db = hints['instance']._state.db
             if db:
                 return db
         if hasattr(model, '_salesforce_object'):
             return self.sf_alias
+        if model._meta.app_label == 'django_cache':
+            return DEFAULT_DB_ALIAS
         return None
 
     def allow_migrate(self, db: str, app_label: str, model_name: Optional[str] = None, **hints: Type[models.Model]
                       ) -> Optional[bool]:
         """
         Don't attempt to sync SF models to non SF databases and vice versa.
         """
         if model_name:
             try:
                 model = apps.get_model(app_label, model_name)  # type: Optional[Type[models.Model]]
             except LookupError:
+                # models that exist only in memory without 'models.py'
                 if 'model' in hints and hints['model'].__module__ == '__fake__':
                     return None
+                if 'model' in hints and hints['model']._meta.app_label == 'django_cache':
+                    return db == DEFAULT_DB_ALIAS
                 raise
         else:
             # hints are used with less priority, because many hints are dynamic
             # models made by migrations in a '__fake__' module which are not
             # SalesforceModels
             model = hints.get('model')
 
         if hasattr(model, '_salesforce_object'):
             # SF models can be migrated if SALESFORCE_DB_ALIAS is e.g.
             # a sqlite3 database or any non-SF database.
             if not (is_sf_database(db) or db == self.sf_alias):
                 return False
         else:
-            if is_sf_database(db) or self.sf_alias != 'default' and db == self.sf_alias:
+            if is_sf_database(db) or self.sf_alias != DEFAULT_DB_ALIAS and db == self.sf_alias:
                 return False
         # TODO: It is usual that "migrate" is currently disallowed for SF.
         # In the future it can be implemented to do a deep check by
         # introspection of compatibily between Django models and SF database.
         if hasattr(model, '_salesforce_object'):
             # return False
             pass
```

### Comparing `django-salesforce-4.1/salesforce/testrunner/example/models.py` & `django-salesforce-4.2/salesforce/testrunner/example/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 from typing import Optional
 import types
 
 import django
```

### Comparing `django-salesforce-4.1/salesforce/testrunner/example/models_template.py` & `django-salesforce-4.2/salesforce/testrunner/example/models_template.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/testrunner/example/templates/search-accounts.html` & `django-salesforce-4.2/salesforce/testrunner/example/templates/search-accounts.html`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/testrunner/example/universal_admin.py` & `django-salesforce-4.2/salesforce/testrunner/example/universal_admin.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/testrunner/example/views.py` & `django-salesforce-4.2/salesforce/testrunner/example/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 import logging
 
 from django import shortcuts
```

### Comparing `django-salesforce-4.1/salesforce/testrunner/local_settings.py.sample` & `django-salesforce-4.2/salesforce/testrunner/local_settings.py.sample`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/testrunner/settings.py` & `django-salesforce-4.2/salesforce/testrunner/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # If you set this to False, Django will make some optimizations so as not
 # to load the internationalization machinery.
 USE_I18N = True
 
 # If you set this to False, Django will not format dates, numbers and
 # calendars according to the current locale
-USE_L10N = True
+# USE_L10N = True  # it is deprecated since Django 4.0 and expected True
 
 # Absolute filesystem path to the directory that will hold user-uploaded files.
 # Example: "/home/media/media.lawrence.com/media/"
 MEDIA_ROOT = ''
 
 # URL that handles the media served from MEDIA_ROOT. Make sure to use a
 # trailing slash.
@@ -189,11 +189,12 @@
 # Name of primary key - by default 'id'. The value 'Id' was the default for
 # version "django-salesforce < 0.5".
 # The value SF_PK can not be changed after any migration for Salesforce has been created
 # SF_PK = 'Id'
 
 DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'  # not important for Salesforce, but for Django warnings
 
+DJSF_LICENSE_KEY = os.environ.get('DJSF_LICENSE_KEY', '')  # configure for enterprise features
 try:
     from salesforce.testrunner.local_settings import *  # noqa pylint:disable=unused-wildcard-import,wildcard-import
 except ImportError:
     pass
```

### Comparing `django-salesforce-4.1/salesforce/testrunner/test_patch.diff` & `django-salesforce-4.2/salesforce/testrunner/test_patch.diff`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/tests/test_auth.py` & `django-salesforce-4.2/salesforce/tests/test_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 import requests
 from django.test import TestCase
 from django.conf import settings
```

### Comparing `django-salesforce-4.1/salesforce/tests/test_basic.py` & `django-salesforce-4.2/salesforce/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/tests/test_browser.py` & `django-salesforce-4.2/salesforce/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/tests/test_bulk.py` & `django-salesforce-4.2/salesforce/tests/test_bulk.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/tests/test_indep.py` & `django-salesforce-4.2/salesforce/tests/test_indep.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/tests/test_integration.py` & `django-salesforce-4.2/salesforce/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 # pylint:disable=protected-access,too-many-lines,unused-variable
 
 from decimal import Decimal
-from distutils.util import strtobool  # pylint: disable=no-name-in-module,import-error # venv inst pylint false positiv
 import datetime
 import logging
 import os
 import warnings
 from typing import Any, cast, List, TypeVar
 
 import pytz
@@ -22,15 +20,15 @@
 from django.utils import timezone
 from django.utils.crypto import get_random_string
 
 import salesforce
 from salesforce import router
 from salesforce.backend import DJANGO_21_PLUS, DJANGO_22_PLUS
 from salesforce.backend.test_helpers import (  # noqa pylint:disable=unused-import
-    expectedFailure, expectedFailureIf, skip, skipUnless)
+    expectedFailure, expectedFailureIf, skip, skipUnless, strtobool)
 from salesforce.backend.test_helpers import (
     current_user, default_is_sf, sf_alias, uid_version as uid,
     QuietSalesforceErrors, LazyTestMixin)
 from salesforce.dbapi.exceptions import SalesforceWarning
 from salesforce.dbapi.test_helpers import PatchedSfConnection
 from salesforce.models import SalesforceModel
 from salesforce.testrunner.example.models import (
@@ -148,15 +146,15 @@
         """
         current_sf_user = User.objects.get(Username=current_user)
         test_contact = Contact(first_name='sf_test', last_name='my')
         test_contact.save()
         try:
             contact = Contact.objects.filter(owner=current_sf_user)[0]
             user = contact.owner
-            # This user can be e.g. 'admins@freelancersunion.org.prod001'.
+            # This user can be e.g. 'admins@example.com.prod001'.
             self.assertEqual(user.Username, current_user)
         finally:
             test_contact.delete()
 
     def test_foreign_key_column(self) -> None:
         """Verify filtering by a column of related parent object.
         """
```

### Comparing `django-salesforce-4.1/salesforce/tests/test_unit.py` & `django-salesforce-4.2/salesforce/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/tests/test_utils.py` & `django-salesforce-4.2/salesforce/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/tests/unit_tests/test_qparser.py` & `django-salesforce-4.2/salesforce/tests/unit_tests/test_qparser.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/salesforce/utils.py` & `django-salesforce-4.2/salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/setup.py` & `django-salesforce-4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # django-salesforce
 #
-# by Phil Christensen
-# (c) 2012-2013 Freelancers Union (http://www.freelancersunion.org)
+# by Hyneck Cernoch and Phil Christensen
 # See LICENSE.md for details
 #
 
 import os
 import re
 
 # disables creation of .DS_Store files inside tarballs on Mac OS X
@@ -56,22 +55,22 @@
 
         # setuptools won't auto-detect Git managed files without this
         setup_requires=[] if not with_git else ["setuptools_git >= 0.4.2"],
 
         install_requires=['django>=2.0'] + requirements_txt,
 
         # metadata for upload to PyPI
-        author="Freelancers Union",
-        author_email="devs@freelancersunion.org",
+        author="Hynek Cernoch",
+        author_email="hynek@sdb.cz",
         maintainer="Phil Christensen",
         maintainer_email="phil@bubblehouse.org",
         description="a Salesforce backend for Django's ORM",
         long_description=long_description,
         long_description_content_type="text/x-rst",
-        license="MIT",
+        license="AGPL",
         keywords="django salesforce orm backend",
         url="https://github.com/django-salesforce/django-salesforce",
     )
 
 
 if __name__ == '__main__':
     dist = autosetup()
```

### Comparing `django-salesforce-4.1/tests/clean_test_data.py` & `django-salesforce-4.2/tests/clean_test_data.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/inspectdb/slow_test.py` & `django-salesforce-4.2/tests/inspectdb/slow_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,20 +35,17 @@
     start_name = sys.argv[1] if sys.argv[1:] else ''
     n_tables = n_read = n_no_data = n_read_errors = n_write = n_write_errors = 0
     model_map = {cls._meta.db_table: cls
                  for cls in mdl.__dict__.values()
                  if isclass(cls) and issubclass(cls, django.db.models.Model)
                  }
     problematic_read = {
-        # These require specific filters (descried in their error messages)
-        'CollaborationGroupRecord', 'ContentFolderMember', 'ContentFolderItem',
-        'ContentDocumentLink', 'Idea', 'IdeaComment', 'UserProfileFeed',
-        'Vote',  # 'OpportunityPartner', 'Product2Feed',
-        # UNKNOWN_EXCEPTION:
-        'TenantUsageEntitlement',
+        # These require specific filters (described in their error messages)
+        # "MALFORMED_QUERY Implementation restriction: .* requires a filter by"
+        'ContentDocumentLink', 'ContentFolderItem', 'ContentFolderMember', 'IdeaComment', 'Vote',
         # special
         'django_migrations',
         }
     problematic_write = {
         # Cannot modify managed objects
         'ApexClass', 'ApexComponent', 'ApexTrigger', 'FieldPermissions',
         'ObjectPermissions', 'PermissionSet', 'Scontrol',
@@ -72,14 +69,16 @@
         # The Apex Class selected is not valid. An Apex Class that implements
         # the Messaging.InboundEmailHandler interface must be selected.
         'EmailServicesFunction',
         # A special user of type user_type='AutomatedProcess' exists in Users
         # since API 41.0 Winter'18.
         # That user account can not be saved because it has an invalid email.
         'User', 'UserLogin',
+        # can't set the VersionData when IsMajorVersion is true.
+        'ContentVersion',
     }
     for tab in sf.introspection.table_list_cache['sobjects']:
         db_table = tab['name']
         # More sobjects are 'queryable' and 'retrieveable' than
         # only 'retrieveable', but half of them would be problematic.
         if tab['retrieveable'] and not db_table.endswith('ChangeEvent') and db_table not in problematic_read:
             if db_table < start_name:
```

### Comparing `django-salesforce-4.1/tests/inspectdb/test.sh` & `django-salesforce-4.2/tests/inspectdb/test.sh`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/inspectdb/tests.py` & `django-salesforce-4.2/tests/inspectdb/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/no_django_dbapi/test.py` & `django-salesforce-4.2/tests/no_django_dbapi/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,7 +63,18 @@
                 self.assertEqual(cursor.fetchall(), [])
                 self.assertEqual(cursor.fetchmany(), [])
                 self.assertEqual(cursor.fetchmany(size=10), [])
                 # scroll to replay the data
                 cursor.scroll(0, 'absolute')
                 result2 = cursor.fetchall()
                 self.assertEqual(result2, result)
+
+    def test_explain(self) -> None:
+        connection = driver.get_connection('salesforce', settings_dict=settings_dict)
+        cursor = connection.cursor()
+
+        cursor.execute("EXPLAIN SELECT Name FROM Contact")
+        self.assertRegex(cursor.fetchone()[0], r"^{'plans': \[{")  # type: ignore[index]
+        last_detail = list(cursor.fetchall())[-1][0]
+        self.assertEqual(last_detail, " 'sourceQuery': 'SELECT Name FROM Contact'}")
+
+        connection.close()
```

### Comparing `django-salesforce-4.1/tests/no_salesforce/models.py` & `django-salesforce-4.2/tests/no_salesforce/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/no_salesforce/settings.py` & `django-salesforce-4.2/tests/no_salesforce/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/no_salesforce/tests.py` & `django-salesforce-4.2/tests/no_salesforce/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/t_debug_toolbar/tests.py` & `django-salesforce-4.2/tests/t_debug_toolbar/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_compatibility/models.py` & `django-salesforce-4.2/tests/test_compatibility/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_compatibility/tests.py` & `django-salesforce-4.2/tests/test_compatibility/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_default_db/models.py` & `django-salesforce-4.2/tests/test_default_db/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_default_db/tests.py` & `django-salesforce-4.2/tests/test_default_db/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_dynamic_auth/settings.py` & `django-salesforce-4.2/tests/test_dynamic_auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_dynamic_auth/tests.py` & `django-salesforce-4.2/tests/test_dynamic_auth/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_general/test_helpers.py` & `django-salesforce-4.2/tests/test_general/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_lazy_connect/settings.py` & `django-salesforce-4.2/tests/test_lazy_connect/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_lazy_connect/tests.py` & `django-salesforce-4.2/tests/test_lazy_connect/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_managers/models.py` & `django-salesforce-4.2/tests/test_managers/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_managers/tests.py` & `django-salesforce-4.2/tests/test_managers/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         try:
             # test that only one request is used for .save()
             with self.lazy_assert_n_requests(1):
                 test_cnt.save()
 
             # test again that only one request is used for .save() for a combined queryset
             wrk = Contact.objects.filter(last_name='B')
+            self.assertTrue(hasattr(wrk, 'sf'))
+            self.assertIn("Contact.Account.Name > 'A' AND Contact.LastName = 'B'", str(wrk.query))
             tmp = wrk[0]
             tmp.last_name = 'C'
             with self.lazy_assert_n_requests(1):
                 tmp.save()
 
             # check that the default queryset is not empty
             _ = Contact.objects.all()[0]
```

### Comparing `django-salesforce-4.1/tests/test_migrate/models.py` & `django-salesforce-4.2/tests/test_migrate/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_migrate/settings.py` & `django-salesforce-4.2/tests/test_migrate/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_migrate/test.sh` & `django-salesforce-4.2/tests/test_migrate/test.sh`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_migrate/tests.py` & `django-salesforce-4.2/tests/test_migrate/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mixin/models.py` & `django-salesforce-4.2/tests/test_mixin/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mixin/tests.py` & `django-salesforce-4.2/tests/test_mixin/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mock/mocksf.py` & `django-salesforce-4.2/tests/test_mock/mocksf.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mock/settings.py` & `django-salesforce-4.2/tests/test_mock/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mock/test_data.py` & `django-salesforce-4.2/tests/test_mock/test_data.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mock/test_mocksf.py` & `django-salesforce-4.2/tests/test_mock/test_mocksf.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mock2/migrations/0001_initial.py` & `django-salesforce-4.2/tests/test_mock2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mock2/models.py` & `django-salesforce-4.2/tests/test_mock2/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/test_mock2/settings.py` & `django-salesforce-4.2/tests/test_mock2/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.utils.crypto import get_random_string
-from salesforce.testrunner.settings import DATABASES  # noqa
+from salesforce.testrunner.settings import DATABASES, DJSF_LICENSE_KEY  # noqa
 
 # DATABASES = {'default': DATABASES['salesforce']}
 SECRET_KEY = get_random_string(length=32)
 # SALESFORCE_DB_ALIAS = 'default'
 # ROOT_URLCONF = None
 INSTALLED_APPS = [
     'django.contrib.auth',
```

### Comparing `django-salesforce-4.1/tests/test_mock2/test_rec.py` & `django-salesforce-4.2/tests/test_mock2/test_rec.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/tooling/slow_test.py` & `django-salesforce-4.2/tests/tooling/slow_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,21 @@
         # in API 52.0 Summer '21
         'EinsteinAgentSettings',
         # in API 54.0 Spring '22
         'EinsteinDealInsightsSettings',
         # in API 55.0 Summer '22
         'IndustriesAutomotiveSettings', 'RelatedListColumnDefinition', 'RelatedListDefinition',
         'SubscriptionManagementSettings', 'WarrantyLifecycleMgmtSettings',
+        # in API 56.0 Winter '23
+        'MfgServiceConsoleSettings',
+        # in API 57.0 Spring '23
+        'PaymentsSettings', 'Territory2SupportedObject',
+        # in API 58.0 Summer '23
+        'ConnectedApplication',  # timeout
+        'LicensingSettings',  # EXTERNAL_OBJECT_EXCEPTION
     }
     problematic_write = {
         # any SalesforceError
         'AccountIntelligenceSettings', 'AccountSettings', 'ActionsSettings',
         'AnalyticsSettings', 'ApexClass', 'ApexPage', 'ApexSettings', 'ApexTrigger',
         'AppExperienceSettings', 'BlockchainSettings', 'BusinessHoursSettings',
         'BusinessProcess', 'CampaignSettings', 'CaseSettings', 'ChatterEmailsMDSettings',
@@ -116,14 +123,20 @@
         # ExpirationDate must be in the future.
         'TraceFlag',
         # silently not updated
         'CustomApplication', 'CustomField', 'CustomTab', 'FlexiPage', 'GlobalValueSet',
         'Layout', 'QuickActionDefinition', 'RemoteProxy', 'ValidationRule',
         'WorkflowFieldUpdate', 'WorkflowRule',
         'QuickActionListItem',
+        # in API 56.0 Winter '23
+        'CustomerDataPlatformSettings', 'OauthOidcSettings',
+        # in API 58.0 Summer '23
+        'ExternalClientAppSettings',  # JSON_PARSER_ERROR
+        'FieldMappingField',  # INVALID_OR_NULL_FOR_RESTRICTED_PICKLIST
+        'StaticResource',  # FIELD_INTEGRITY_EXCEPTION
     }
 
     #  FIELD_INTEGRITY_EXCEPTION
     # Only the Metadata and FullName fields may be specified on AddressSettings, or else Metadata must be excluded.
 
     requires_filter = [
         # some of them are important, but can not be tested automatically here
```

### Comparing `django-salesforce-4.1/tests/tooling/test.sh` & `django-salesforce-4.2/tests/tooling/test.sh`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tests/tooling/tests.py` & `django-salesforce-4.2/tests/tooling/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/tox.ini` & `django-salesforce-4.2/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,136 +1,133 @@
 # The easy usage for all test environments:
 #   pip install tox
 #   tox
 
 [tox]
-# the highest version, the lowest, Django 2.2 and some versions complementary to Travis envlist
+# test the highest version, the lowest, Django 2.2 and some versions complementary to Travis envlist
 # Django 2.2 is important because some code in salesforce.backend.query is used only with exactly this version.
 envlist =
     docs_style
     typing
-    dj41-py310
+    dj42-py312
+    dj41-py311
     dj40-py310
-    dj20-py36
-    dj21-py37
-    dj22-py38
-    dj31-py39
-    # djdev-py311
-    no_django-py38
-    debug_toolbar-dj40-py38
-    # pylint-dj41-py310`
-
-# Python versions for Travis are 3.6, 3.8, 3.9 (the lowest, the default in Travis, the highest in Travis)
-# Environments tested by Travis 
-#   TOXENV=docs_style,typing,dj20-py36,dj22-py38,dj30-py36,dj32-py38
-#   TOXENV=dj40-py39,no_django-py39,debug_toolbar-dj32-py39
+    dj32-py39
+    dj30-py38
+    dj22-py37
+    dj20-py37
+    # djdev-py312
+    no_django-py311
+    debug_toolbar-dj41-py310
+    # pylint-dj42-py310`
+
+# Python versions used for Travis with Jammy are 3.7, 3.8, 3.9, 3.10 (default)
+# Environments tested by Travis:
+#   TOXENV=docs_style,typing,dj41-py310,dj32-py38
+#   TOXENV=dj40-py39,dj30-py39,no_django-py39,debug_toolbar-dj32-py39
+#   TOXENV=dj20-py37,dj22-py37
 
 [testenv]
 basepython =
-    py36: python3.6
     py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
     py311: python3.11
+    py312: python3.12
     pypy: pypy
     pypy3: pypy3
 deps =
     # minimal required versions for all supported Python versions
     dj20: Django~=2.0.0   # py34-37
     dj21: Django~=2.1.0   # py35-37
     dj22: Django~=2.2.17  # py35-37
     dj30: Django~=3.0.11  # py36-39
     dj31: Django~=3.1.3   # py36-39
     dj32: Django~=3.2.0   # py36-39
     dj40: Django~=4.0.0   # py38-310
     dj41: Django~=4.1.0   # py38-310
+    dj42: Django~=4.2.0   # py38-311
     djdev: https://github.com/django/django/archive/main.zip
     # local copy of django/origin main
-    # wget https://github.com/django/django/archive/main.zip -O django-40-dev.zip
-    # djdevlocal: django-40-dev.zip
+    # wget https://github.com/django/django/archive/main.zip -O django-42-dev.zip
+    # djdevlocal: django-42-dev.zip
     pylint: pylint~=2.8.0    # fixed version to not report too much
     pylint: pylint-django<2.5
-    debug_toolbar: django-debug-toolbar
+    # TODO incompatibility with new debug toolbar 4.1
+    debug_toolbar: django-debug-toolbar<4.1
     coverage
     # This Beatbox version works with Python 3 and 2.
     # Be hopeful, it will be soon in official repositories.
     # git+https://github.com/superfell/Beatbox@master#egg=beatbox
     # beatbox3
     git+https://github.com/hynekcer/beatbox-davisagli.git@7f628a789cba#egg=beatbox
     -rrequirements.txt
     psycopg2-binary
+allowlist_externals = {toxinidir}/tests/tests.sh
 commands =
     {envpython} manage.py test salesforce tests.test_mock
     {toxinidir}/tests/tests.sh
 setenv =
     # all bugs can be reported by the command `QUIET_KNOWN_BUGS=off tox`
     # otherwise known bugs are silent
     QUIET_KNOWN_BUGS={env:QUIET_KNOWN_BUGS:on}
-passenv = SLOW_TESTS
-
-# These other environments are tested by `tox -e ALL`:
-# (Especially useful is to add highest contra lowest Django combinations)
-[testenv:djdev-py310]
+passenv =
+    DJSF_LICENSE_KEY
+    SF_CONSUMER_KEY
+    SF_CONSUMER_SECRET
+    SF_HOST
+    SF_PASSWORD
+    SF_USER
+    SLOW_TESTS
 
 [testenv:clean]
 basepython = python3
 commands =
     {envpython} manage.py test tests.clean_test_data
 
-[testenv:debug_toolbar-dj{20,32,40}-py{36,38,39}]
+[testenv:debug_toolbar-dj{20-py37,32-py39,41-py310}]
 commands = {envpython} manage.py test tests.t_debug_toolbar --settings=tests.t_debug_toolbar.settings
 
-[testenv:pylint-dj{20,21,22,30,31,32,40,41}-py{36,38,39,310}]
+[testenv:pylint-dj{20-py37,22-py37,30-py39,32-py39,40-py310,41-py310,42-py310}]
+# Python 3.11 will require "wrapt>=1.14.1" and therefore Python between 3.7 and 3.10 is used with pylint
 setenv = DJANGO_SETTINGS_MODULE=salesforce.testrunner.settings
 commands = pylint --reports=no salesforce
 
-[testenv:no_django-py{36,38,39}]
+[testenv:no_django-py{37,39,311}]
 usedevelop=True
-allowlist_externals = rm
+allowlist_externals =
+    rm
+    {toxinidir}/tests/tests_no_django.sh
 commands =
     # remove Django because it has been installed by setup.py now if not by tox
     rm -rf {envsitepackagesdir}/django
     {toxinidir}/tests/tests_no_django.sh
 
 [testenv:docs_style]
 # check Python code style and rst syntax
 basepython = python3
 skip_install = True
 deps =
-    flake8
+    # the new flake8 ver 6.0 doesn't support type comments "# type: ..."
+    flake8<6.0
     rstcheck
 commands =
     flake8
-    rstcheck README.rst CHANGELOG.rst
+    rstcheck --recursive README.rst CHANGELOG.rst docs
 
 [testenv:typing]
 # any python >= 3.5.3, < 3.9
 basepython = python3.8
-allowlist_externals =
-    bash
-    touch
 deps =
     mypy==0.770
     git+https://github.com/hynekcer/django-salesforce-stubs.git@v1.5.0.3#django-stubs
+allowlist_externals =
+    bash
+    touch
+    {toxinidir}/tests/mypy.sh
 commands =
     touch tests/inspectdb/models.py tests/inspectdb/dependent_model/models_template.py
     bash -ec "{envpython} manage.py inspectdb --database=salesforce --tooling-api EntityDefinition FieldDefinition UserEntityAccess UserFieldAccess User >tests/tooling/models.py"
     mypy salesforce tests
     mypy salesforce/dbapi tests/test_mock tests/test_mock2 --strict
     {toxinidir}/tests/mypy.sh
-
-# === lint configurations (not tests) ===
-[flake8]
-max-line-length = 119
-exclude =
-    .git,.tox,.components,.eggs,build,migrations,models1*.py,packages_
-    tests/inspectdb/models.py
-    tests/inspectdb/dependent_model/models_template.py
-    tests/tooling/models.py
-
-[pep8]
-max-line-length = 119
-exclude=.git,.tox,.components,.eggs,build,migrations,models1*.py,packages_,tests/inspectdb/models.py,tests/tooling/models.py
-[pyflakes]
-# ignore E126 continuation line over-indented for hanging indent
-# ignore=E126
```

### Comparing `django-salesforce-4.1/wiki/Documents-and-Attachments.md` & `django-salesforce-4.2/wiki/Documents-and-Attachments.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/wiki/Empty-strings-in-filters.md` & `django-salesforce-4.2/wiki/Empty-strings-in-filters.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/wiki/Error-messages.md` & `django-salesforce-4.2/wiki/Error-messages.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/wiki/Experimental-Features.rest` & `django-salesforce-4.2/wiki/Experimental-Features.rest`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/wiki/Foreign-Key-Support.rest` & `django-salesforce-4.2/wiki/Foreign-Key-Support.rest`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     print(my_qs.query.get_compiler('default').as_sql())      # SQL
 
 ..  comment until the end of identation
     Related objects (Lookup field or Master-Detail Relationship) use two different names in
     `SOQL <http://www.salesforce.com/us/developer/docs/soql_sosl/>`__. If the
     relation is by ID the columns are named ``FieldName__c``, whereas if the relation
     is stored by object the column is named ``FieldName__r``. More details about
-    this can be found in the discussion about `#43 <https://github.com/freelancersunion/django-salesforce/issues/43>`__.
+    this can be found in the discussion about `#43 <https://github.com/django-salesforce/django-salesforce/issues/43>`__.
 
 Also Many2many relationships are possible in simple cases, like in the example models::
 
     class Opportunity(SalesforceModel):
         name = models.CharField(max_length=255)
         contacts = django.db.models.ManyToManyField(
             Contact, through='example.OpportunityContactRole',
```

### Comparing `django-salesforce-4.1/wiki/Home.md` & `django-salesforce-4.2/wiki/Home.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/wiki/Introspection-and-Special-Attributes-of-Fields.rest` & `django-salesforce-4.2/wiki/Introspection-and-Special-Attributes-of-Fields.rest`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/wiki/Lead-Conversion.rest` & `django-salesforce-4.2/wiki/Lead-Conversion.rest`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/wiki/Release-Process.md` & `django-salesforce-4.2/wiki/Release-Process.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-4.1/wiki/SalesforceModels-used-with-local-databases.md` & `django-salesforce-4.2/wiki/SalesforceModels-used-with-local-databases.md`

 * *Files identical despite different names*

