# Comparing `tmp/django_slugify_processor-1.3.1.tar.gz` & `tmp/django-slugify-processor-1.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_slugify_processor-1.3.1.tar", max compression
+gzip compressed data, was "django-slugify-processor-1.3.1a0.tar", max compression
```

## Comparing `django_slugify_processor-1.3.1.tar` & `django-slugify-processor-1.3.1a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1057 2023-07-04 18:45:20.671768 django_slugify_processor-1.3.1/LICENSE
--rw-r--r--   0        0        0     8112 2023-07-04 18:45:20.671768 django_slugify_processor-1.3.1/README.md
--rw-r--r--   0        0        0     3963 2023-07-04 18:45:20.675768 django_slugify_processor-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      580 2023-07-04 18:45:20.675768 django_slugify_processor-1.3.1/src/django_slugify_processor/__about__.py
--rw-r--r--   0        0        0        0 2023-07-04 18:45:20.675768 django_slugify_processor-1.3.1/src/django_slugify_processor/__init__.py
--rw-r--r--   0        0        0       62 2023-07-04 18:45:20.675768 django_slugify_processor-1.3.1/src/django_slugify_processor/settings.py
--rw-r--r--   0        0        0        0 2023-07-04 18:45:20.675768 django_slugify_processor-1.3.1/src/django_slugify_processor/templatetags/__init__.py
--rw-r--r--   0        0        0      652 2023-07-04 18:45:20.675768 django_slugify_processor-1.3.1/src/django_slugify_processor/templatetags/slugify_processor.py
--rw-r--r--   0        0        0     1881 2023-07-04 18:45:20.679768 django_slugify_processor-1.3.1/src/django_slugify_processor/text.py
--rw-r--r--   0        0        0        0 2023-07-04 18:45:20.679768 django_slugify_processor-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0      191 2023-07-04 18:45:20.679768 django_slugify_processor-1.3.1/tests/settings.py
--rw-r--r--   0        0        0      981 2023-07-04 18:45:20.679768 django_slugify_processor-1.3.1/tests/test_filters.py
--rw-r--r--   0        0        0      599 2023-07-04 18:45:20.679768 django_slugify_processor-1.3.1/tests/test_test_project.py
--rw-r--r--   0        0        0      358 2023-07-04 18:45:20.679768 django_slugify_processor-1.3.1/tests/test_text.py
--rw-r--r--   0        0        0     9890 1970-01-01 00:00:00.000000 django_slugify_processor-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/LICENSE
+-rw-r--r--   0        0        0     8165 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/README.md
+-rw-r--r--   0        0        0     3110 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0      582 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/src/django_slugify_processor/__about__.py
+-rw-r--r--   0        0        0        0 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/src/django_slugify_processor/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/src/django_slugify_processor/templatetags/__init__.py
+-rw-r--r--   0        0        0      652 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/src/django_slugify_processor/templatetags/slugify_processor.py
+-rw-r--r--   0        0        0     1881 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/src/django_slugify_processor/text.py
+-rw-r--r--   0        0        0        0 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/tests/__init__.py
+-rw-r--r--   0        0        0      155 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/tests/settings.py
+-rw-r--r--   0        0        0      981 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/tests/test_filters.py
+-rw-r--r--   0        0        0      600 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/tests/test_test_project.py
+-rw-r--r--   0        0        0      358 2022-09-18 20:51:48.819617 django-slugify-processor-1.3.1a0/tests/test_text.py
+-rw-r--r--   0        0        0     9356 2022-09-18 20:52:09.194120 django-slugify-processor-1.3.1a0/setup.py
+-rw-r--r--   0        0        0     9916 2022-09-18 20:52:09.194733 django-slugify-processor-1.3.1a0/PKG-INFO
```

### Comparing `django_slugify_processor-1.3.1/LICENSE` & `django-slugify-processor-1.3.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_slugify_processor-1.3.1/README.md` & `django-slugify-processor-1.3.1a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,16 @@
   ([github](https://github.com/django-extensions/django-extensions))
 
 # The problem
 
 This project is based on an article from [devel.tech](https://devel.tech) covering
 [django's import strings](https://devel.tech/tips/n/djms3tTe/how-django-uses-deferred-imports-to-scale/).
 
-Corner cases exist with slugification. For instance:
+Corner cases exist with slugification. For instance: Corner cases exist with slugification. For
+instance:
 
 | Term | [`django.utils.text.slugify`] | What you want |
 | ---- | ----------------------------- | ------------- |
 | C    | c (correct)                   | n/a           |
 | C++  | c                             | cpp           |
 | C#   | c                             | c-sharp       |
```

### Comparing `django_slugify_processor-1.3.1/pyproject.toml` & `django-slugify-processor-1.3.1a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-slugify-processor"
-version = "1.3.1"
+version = "1.3.1a0"
 description = "pipeline for slugification edgecases in django"
 
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Environment :: Web Environment',
   'Framework :: Django',
   'Framework :: Django :: 2.2',
@@ -16,15 +16,14 @@
   'Operating System :: OS Independent',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
-  'Programming Language :: Python :: 3.11',
   'Programming Language :: Python :: Implementation :: CPython',
   'Programming Language :: Python :: Implementation :: PyPy',
   'Topic :: Utilities',
 ]
 
 license = "MIT"
 
@@ -50,44 +49,49 @@
 Changes = "https://github.com/tony/django-slugify-processor/blob/master/CHANGES"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 django-extensions = { version = "*", optional = true }
 Django = ">=2.2"
 
-[tool.poetry.group.dev.dependencies]
+[tool.poetry.dev-dependencies]
 ### Docs ###
 sphinx = "*"
 furo = "*"
-gp-libs = "~0.0.1a12"
+gp-libs = "~0.0.1a9"
 sphinx-autobuild = "*"
 sphinx-autodoc-typehints = "*"
-sphinx-inline-tabs = "<2023.4.21"  # For Python 3.7 support
-sphinxext-opengraph = "<0.8"  # https://github.com/wpilibsuite/sphinxext-opengraph/issues/100
+sphinx-inline-tabs = { version = "*", python = "^3.7" }
+sphinxext-opengraph = "*"
 sphinx-copybutton = "*"
 sphinxext-rediraffe = "*"
-myst_parser = ">=0.18.1"
+myst_parser = "*"
 
 ### Testing ###
 pytest = "*"
 pytest-rerunfailures = "*"
 pytest-django = "*"
-pytest-watcher = "*"
+pytest-watcher = "^0.2.3"
 django-extensions = "*"
 
 ### Coverage ###
 codecov = "*"
 coverage = "*"
 pytest-cov = "*"
 
-### Lint ###
+### Format ###
 black = "*"
-ruff = "*"
+isort = "*"
+
+### Lint ###
+flake8 = "*"
+flake8-bugbear = "^22.8.23"
+flake8-comprehensions = "^3.10.0"
 mypy = "*"
-django-stubs = "*"
+django-stubs = "^1.12.0"
 
 [tool.poetry.extras]
 docs = [
   "sphinx",
   "sphinx-autodoc-typehints",
   "sphinx-autobuild",
   "sphinx-copybutton",
@@ -102,81 +106,31 @@
   "pytest",
   "pytest-rerunfailures",
   "pytest-django",
   "pytest-watcher",
   "django-extensions",
 ]
 coverage = ["codecov", "coverage", "pytest-cov"]
+format = ["black", "isort"]
 lint = [
-  "black",
-  "ruff",
+  "flake8",
+  "flake8-bugbear",
+  "flake8-comprehensions",
   "mypy",
   "django-stubs",
 ]
 
 [tool.mypy]
 plugins = ["mypy_django_plugin.main"]
-files = [
-  "src/",
-  "tests/",
-]
 
 [tool.django-stubs]
 django_settings_module = "tests.settings"
 
 [[tool.mypy.overrides]]
 module = [
   "django_extensions.*",
 ]
 ignore_missing_imports = true
 
-[tool.coverage.run]
-branch = true
-parallel = true
-omit = [
-  "*/_compat.py",
-  "docs/conf.py",
-]
-
-[tool.coverage.report]
-show_missing = true
-skip_covered = true
-exclude_lines = [
-  "pragma: no cover",
-  "def __repr__",
-  "raise NotImplementedError",
-  "return NotImplemented",
-  "def parse_args",
-  "if TYPE_CHECKING:",
-  "if t.TYPE_CHECKING:",
-  "@overload( |$)",
-]
-
-[tool.ruff]
-target-version = "py37"
-select = [
-  "E", # pycodestyle
-  "F", # pyflakes
-  "I", # isort
-  "UP",  # pyupgrade
-  "B", # flake8-bugbear
-  "C4", # flake8-comprehensions
-  "Q", # flake8-quotes
-  "PTH", # flake8-use-pathlib
-  "SIM",  # flake8-simplify
-  "TRY", # Trycertatops
-  "PERF", # Perflint
-  "RUF" # Ruff-specific rules
-]
-
-[tool.ruff.isort]
-known-first-party = [
-  "django_slugify_processor"
-]
-combine-as-imports = true
-
-[tool.ruff.per-file-ignores]
-"*/__init__.py" = ["F401"]
-
 [build-system]
 requires = ["poetry_core>=1.0.0", "poetry>=1.1.12"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_slugify_processor-1.3.1/src/django_slugify_processor/__about__.py` & `django-slugify-processor-1.3.1a0/src/django_slugify_processor/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __title__ = "django-slugify-processor"
 __package_name__ = "django_slugify_processor"
-__version__ = "1.3.1"
+__version__ = "1.3.1a0"
 __description__ = "pipeline for slugification edgecases in django"
 __email__ = "tony@git-pull.com"
 __pypi__ = "https://pypi.python.org/pypi/django-slugify-processor"
 __github__ = "http://github.com/tony/django-slugify-processor/"
 __docs__ = "https://django-slugify-processor.git-pull.com"
 __tracker__ = "https://github.com/tony/django-slugify-processor/issues"
 __author__ = "Tony Narlock"
```

### Comparing `django_slugify_processor-1.3.1/src/django_slugify_processor/templatetags/slugify_processor.py` & `django-slugify-processor-1.3.1a0/src/django_slugify_processor/templatetags/slugify_processor.py`

 * *Files identical despite different names*

### Comparing `django_slugify_processor-1.3.1/src/django_slugify_processor/text.py` & `django-slugify-processor-1.3.1a0/src/django_slugify_processor/text.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
         SLUGIFY_PROCESSORS = [
             'project.app.slugify_programming_languages',
             'project.app.slugify_geo_acronyms',
             'project.app.slugify_us_currency',
         ]
     """
-    slugify_processors = getattr(settings, "SLUGIFY_PROCESSORS", [])
-    for slugify_fn_str in slugify_processors:
-        slugify_fn_ = import_string(slugify_fn_str)
-        value = slugify_fn_(value)
+    if hasattr(settings, "SLUGIFY_PROCESSORS"):
+        for slugify_fn_str in settings.SLUGIFY_PROCESSORS:
+            slugify_fn_ = import_string(slugify_fn_str)
+            value = slugify_fn_(value)
 
     return django_slugify(value, allow_unicode)
```

### Comparing `django_slugify_processor-1.3.1/tests/test_filters.py` & `django-slugify-processor-1.3.1a0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django_slugify_processor-1.3.1/tests/test_test_project.py` & `django-slugify-processor-1.3.1a0/tests/test_test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from django.apps import apps
 
 
 @pytest.mark.django_db
 def test_models_passthrough(settings):
     MyModel = apps.get_model("test_app.MyModel")
     entered = "c++"
```

### Comparing `django_slugify_processor-1.3.1/PKG-INFO` & `django-slugify-processor-1.3.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-slugify-processor
-Version: 1.3.1
+Version: 1.3.1a0
 Summary: pipeline for slugification edgecases in django
 Home-page: https://django-slugify-processor.git-pull.com
 License: MIT
 Keywords: django,slug,text
 Author: Tony Narlock
 Author-email: tony@git-pull.com
 Requires-Python: >=3.7,<4.0
@@ -16,28 +16,28 @@
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Provides-Extra: coverage
 Provides-Extra: docs
+Provides-Extra: format
 Provides-Extra: lint
 Provides-Extra: test
 Requires-Dist: Django (>=2.2)
-Requires-Dist: django-extensions ; extra == "test"
+Requires-Dist: django-extensions; extra == "test"
 Project-URL: Bug Tracker, https://github.com/tony/django-slugify-processor/issues
 Project-URL: Changes, https://github.com/tony/django-slugify-processor/blob/master/CHANGES
 Project-URL: Documentation, https://django-slugify-processor.git-pull.com
 Project-URL: Repository, https://github.com/tony/django-slugify-processor
 Description-Content-Type: text/markdown
 
 # django-slugify-processor
@@ -72,15 +72,16 @@
   ([github](https://github.com/django-extensions/django-extensions))
 
 # The problem
 
 This project is based on an article from [devel.tech](https://devel.tech) covering
 [django's import strings](https://devel.tech/tips/n/djms3tTe/how-django-uses-deferred-imports-to-scale/).
 
-Corner cases exist with slugification. For instance:
+Corner cases exist with slugification. For instance: Corner cases exist with slugification. For
+instance:
 
 | Term | [`django.utils.text.slugify`] | What you want |
 | ---- | ----------------------------- | ------------- |
 | C    | c (correct)                   | n/a           |
 | C++  | c                             | cpp           |
 | C#   | c                             | c-sharp       |
```

