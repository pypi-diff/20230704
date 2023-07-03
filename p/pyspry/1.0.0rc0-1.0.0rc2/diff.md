# Comparing `tmp/pyspry-1.0.0rc0.tar.gz` & `tmp/pyspry-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspry-1.0.0rc0.tar", max compression
+gzip compressed data, was "pyspry-1.0.0rc2.tar", max compression
```

## Comparing `pyspry-1.0.0rc0.tar` & `pyspry-1.0.0rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-07-01 19:57:03.179964 pyspry-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0     5242 2023-07-03 00:17:22.979343 pyspry-1.0.0rc0/README.md
--rw-r--r--   0        0        0    27664 2023-07-03 12:11:45.183821 pyspry-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0      375 2023-07-01 18:54:07.756522 pyspry-1.0.0rc0/src/pyspry/__init__.py
--rw-r--r--   0        0        0    11194 2023-07-02 20:42:19.229950 pyspry-1.0.0rc0/src/pyspry/base.py
--rw-r--r--   0        0        0    13459 2023-07-02 20:51:01.386695 pyspry-1.0.0rc0/src/pyspry/nested_dict.py
--rw-r--r--   0        0        0        0 2023-07-01 18:40:11.133731 pyspry-1.0.0rc0/src/pyspry/py.typed
--rw-r--r--   0        0        0      462 2023-07-01 18:54:29.506834 pyspry-1.0.0rc0/src/pyspry/settings.py
--rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 pyspry-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-03 22:16:39.925292 pyspry-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     5835 2023-07-03 22:16:39.925292 pyspry-1.0.0rc2/README.md
+-rw-r--r--   0        0        0    27664 2023-07-03 22:16:51.182292 pyspry-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      375 2023-07-03 22:16:39.927292 pyspry-1.0.0rc2/src/pyspry/__init__.py
+-rw-r--r--   0        0        0    11194 2023-07-03 22:16:39.927292 pyspry-1.0.0rc2/src/pyspry/base.py
+-rw-r--r--   0        0        0    13459 2023-07-03 22:16:39.927292 pyspry-1.0.0rc2/src/pyspry/nested_dict.py
+-rw-r--r--   0        0        0        0 2023-07-03 22:16:39.998292 pyspry-1.0.0rc2/src/pyspry/py.typed
+-rw-r--r--   0        0        0      462 2023-07-03 22:16:39.927292 pyspry-1.0.0rc2/src/pyspry/settings.py
+-rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 pyspry-1.0.0rc2/PKG-INFO
```

### Comparing `pyspry-1.0.0rc0/LICENSE` & `pyspry-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspry-1.0.0rc0/README.md` & `pyspry-1.0.0rc2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # A Springy Little Configuration Reader
 
-[![latest release](https://gitlab.com/bryant.finney/pyspry/-/badges/release.svg)](https://gitlab.com/bryant.finney/pyspry/-/releases)
-[![pipeline status](https://gitlab.com/bryant.finney/pyspry/badges/main/pipeline.svg)](https://gitlab.com/bryant.finney/pyspry/-/commits/main)
-[![coverage report](https://gitlab.com/bryant.finney/pyspry/badges/main/coverage.svg)](https://gitlab.com/bryant.finney/pyspry/-/commits/main)
+[![latest release](https://gitlab.com/bfosi/pyspry/-/badges/release.svg)](https://gitlab.com/bfosi/pyspry/-/releases)
+[![pipeline status](https://gitlab.com/bfosi/pyspry/badges/main/pipeline.svg)](https://gitlab.com/bfosi/pyspry/-/pipelines/latest)
+[![coverage report](https://gitlab.com/bfosi/pyspry/badges/main/coverage.svg)](https://bfosi.gitlab.io/pyspry/reports/pytest-html)
 [![Maintainability](https://api.codeclimate.com/v1/badges/996a01b1ab2df27571d5/maintainability)](https://codeclimate.com/github/bryant-finney/pyspry/maintainability)
-[![pylint](docs/reports/pylint.svg)](https://)
+[![pylint](https://bfosi.gitlab.io/pyspry/reports/pylint.svg)](https://bfosi.gitlab.io/pyspry/reports/pylint-gitlab.html)
 [![PyPI version](https://badge.fury.io/py/pyspry.svg)](https://badge.fury.io/py/pyspry)
+[![Downloads](https://static.pepy.tech/badge/pyspry)](https://pepy.tech/project/pyspry)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![docs: pdoc](https://img.shields.io/badge/docs-pdoc-blueviolet)](https://bfosi.gitlab.io/pyspry)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://bfosi.gitlab.io/pyspry/reports/mypy-html)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/bryant-finney/pyspry/main.svg)](https://results.pre-commit.ci/latest/github/bryant-finney/pyspry/main)
 
 Influenced by [Spring Boot's YAML configuration features](https://docs.spring.io/spring-boot/docs/1.1.0.M1/reference/html/boot-features-external-config.html#boot-features-external-config-yaml),
 this library reads system configuration settings from environment variables and YAML files.
 
 ## Installation
 
 To install using `pip`:
@@ -160,10 +164,10 @@
   lab                   Run Jupyter Lab
   lint                  Lint this package
   test                  Test this package and report coverage
 ```
 
 ## Reports
 
-- [`bandit`](docs/reports/bandit.html)
-- [`mypy`](docs/reports/mypy-html/index.html)
-- [`pytest` coverage](docs/reports/pytest-html/index.html)
+- [`bandit`](https://bfosi.gitlab.io/pyspry/reports/bandit.html)
+- [`mypy`](https://bfosi.gitlab.io/pyspry/reports/mypy-html/index.html)
+- [`pytest` coverage](https://bfosi.gitlab.io/pyspry/reports/pytest-html/index.html)
```

### Comparing `pyspry-1.0.0rc0/pyproject.toml` & `pyspry-1.0.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 # https://python-poetry.org/docs/pyproject/
 name = "pyspry"
-version = "1.0.0rc0"
+version = "1.0.0rc2"
 description = "A springy little configuration reader"
 authors = ["Bryant Finney <finney.bp@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/bryant.finney/pyspry"
 exclude = ["src/pyspry/conftest.py"]
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `pyspry-1.0.0rc0/src/pyspry/base.py` & `pyspry-1.0.0rc2/src/pyspry/base.py`

 * *Files identical despite different names*

### Comparing `pyspry-1.0.0rc0/src/pyspry/nested_dict.py` & `pyspry-1.0.0rc2/src/pyspry/nested_dict.py`

 * *Files identical despite different names*

### Comparing `pyspry-1.0.0rc0/PKG-INFO` & `pyspry-1.0.0rc2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspry
-Version: 1.0.0rc0
+Version: 1.0.0rc2
 Summary: A springy little configuration reader
 Home-page: https://gitlab.com/bryant.finney/pyspry
 Author: Bryant Finney
 Author-email: finney.bp@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -13,21 +13,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://gitlab.com/bryant.finney/pyspry
 Description-Content-Type: text/markdown
 
 # A Springy Little Configuration Reader
 
-[![latest release](https://gitlab.com/bryant.finney/pyspry/-/badges/release.svg)](https://gitlab.com/bryant.finney/pyspry/-/releases)
-[![pipeline status](https://gitlab.com/bryant.finney/pyspry/badges/main/pipeline.svg)](https://gitlab.com/bryant.finney/pyspry/-/commits/main)
-[![coverage report](https://gitlab.com/bryant.finney/pyspry/badges/main/coverage.svg)](https://gitlab.com/bryant.finney/pyspry/-/commits/main)
+[![latest release](https://gitlab.com/bfosi/pyspry/-/badges/release.svg)](https://gitlab.com/bfosi/pyspry/-/releases)
+[![pipeline status](https://gitlab.com/bfosi/pyspry/badges/main/pipeline.svg)](https://gitlab.com/bfosi/pyspry/-/pipelines/latest)
+[![coverage report](https://gitlab.com/bfosi/pyspry/badges/main/coverage.svg)](https://bfosi.gitlab.io/pyspry/reports/pytest-html)
 [![Maintainability](https://api.codeclimate.com/v1/badges/996a01b1ab2df27571d5/maintainability)](https://codeclimate.com/github/bryant-finney/pyspry/maintainability)
-[![pylint](docs/reports/pylint.svg)](https://)
+[![pylint](https://bfosi.gitlab.io/pyspry/reports/pylint.svg)](https://bfosi.gitlab.io/pyspry/reports/pylint-gitlab.html)
 [![PyPI version](https://badge.fury.io/py/pyspry.svg)](https://badge.fury.io/py/pyspry)
+[![Downloads](https://static.pepy.tech/badge/pyspry)](https://pepy.tech/project/pyspry)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![docs: pdoc](https://img.shields.io/badge/docs-pdoc-blueviolet)](https://bfosi.gitlab.io/pyspry)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://bfosi.gitlab.io/pyspry/reports/mypy-html)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/bryant-finney/pyspry/main.svg)](https://results.pre-commit.ci/latest/github/bryant-finney/pyspry/main)
 
 Influenced by [Spring Boot's YAML configuration features](https://docs.spring.io/spring-boot/docs/1.1.0.M1/reference/html/boot-features-external-config.html#boot-features-external-config-yaml),
 this library reads system configuration settings from environment variables and YAML files.
 
 ## Installation
 
 To install using `pip`:
@@ -177,11 +181,11 @@
   lab                   Run Jupyter Lab
   lint                  Lint this package
   test                  Test this package and report coverage
 ```
 
 ## Reports
 
-- [`bandit`](docs/reports/bandit.html)
-- [`mypy`](docs/reports/mypy-html/index.html)
-- [`pytest` coverage](docs/reports/pytest-html/index.html)
+- [`bandit`](https://bfosi.gitlab.io/pyspry/reports/bandit.html)
+- [`mypy`](https://bfosi.gitlab.io/pyspry/reports/mypy-html/index.html)
+- [`pytest` coverage](https://bfosi.gitlab.io/pyspry/reports/pytest-html/index.html)
```

