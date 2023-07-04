# Comparing `tmp/pydantic-loggings-0.8.0.tar.gz` & `tmp/pydantic-loggings-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-0.8.0.tar", last modified: Mon Jul  3 16:26:50 2023, max compression
+gzip compressed data, was "pydantic-loggings-0.9.0.tar", last modified: Tue Jul  4 04:55:28 2023, max compression
```

## Comparing `pydantic-loggings-0.8.0.tar` & `pydantic-loggings-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1620 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1765 2023-07-03 16:26:39.000000 pydantic-loggings-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.935611 pydantic-loggings-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.935611 pydantic-loggings-0.8.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)      616 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/src/pydantic_loggings/base/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/loggings.py
--rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      656 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/loggings.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.935611 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      882 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/tests/
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:55:28.805405 pydantic-loggings-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-04 04:55:28.805405 pydantic-loggings-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 04:55:28.805405 pydantic-loggings-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:55:28.801405 pydantic-loggings-0.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:55:28.801405 pydantic-loggings-0.9.0/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:55:28.801405 pydantic-loggings-0.9.0/src/pydantic_loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/base/loggings.py
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:55:28.805405 pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/loggings.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:55:28.801405 pydantic-loggings-0.9.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-04 04:55:28.000000 pydantic-loggings-0.9.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-04 04:55:28.000000 pydantic-loggings-0.9.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 04:55:28.000000 pydantic-loggings-0.9.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-04 04:55:28.000000 pydantic-loggings-0.9.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-04 04:55:28.000000 pydantic-loggings-0.9.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:55:28.805405 pydantic-loggings-0.9.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/tests/test_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/tests/test_types_.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-07-04 04:55:18.000000 pydantic-loggings-0.9.0/tests/test_utils.py
```

### Comparing `pydantic-loggings-0.8.0/PKG-INFO` & `pydantic-loggings-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.8.0
+Version: 0.9.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Configure Python logging from environment variables with pydantic (settings) Model
```

### Comparing `pydantic-loggings-0.8.0/README.md` & `pydantic-loggings-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.8.0/pyproject.toml` & `pydantic-loggings-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   {name = "m9810223", email = "m9810223@gmail.com"},
 ]
 name = "pydantic-loggings"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.8.0"
+version = "0.9.0"
 
 dependencies = [
   "pydantic>=2.0",
   "pydantic-settings>=2.0",
 ]
 
 [project.urls]
@@ -24,16 +24,18 @@
 
 [tool.pdm.scripts]
 debug = {composite = ["dev"], env = {DEBUG = '1'}}
 dev = "python dev.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
-  "pytest>=7.4.0",
-  "pyright>=1.1.316",
+    "pytest>=7.4.0",
+    "pyright>=1.1.316",
+    "pytest-cov>=4.1.0",
+    "hypothesis>=6.80.0",
 ]
 [tool.black] # https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html
 skip-string-normalization = 1
 
 [tool.ruff]
 extend-select = [
   "W", # pycodestyle Warning
@@ -59,8 +61,12 @@
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/stable/reference/reference.html
 # https://docs.pytest.org/en/stable/explanation/goodpractices.html
 # https://docs.pytest.org/en/stable/example/pythoncollection.html
-addopts = "--exitfirst --failed-first -r fEsxXp --disable-warnings --showlocals --tb=short" # pytest-xdist
+addopts = "--exitfirst --failed-first -r fEsxXp --disable-warnings --showlocals --tb=short --cov=src --cov-report=term --cov-report=html:./htmlcov"
+
+# https://coverage.readthedocs.io/en/stable/config.html
+[tool.coverage.run]
+omit = ["__init__.py"]
```

### Comparing `pydantic-loggings-0.8.0/src/pydantic_loggings/base/loggings.py` & `pydantic-loggings-0.9.0/src/pydantic_loggings/base/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.8.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-0.9.0/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/formatters.py` & `pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/handlers.py` & `pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/loggers.py` & `pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/loggings.py` & `pydantic-loggings-0.9.0/src/pydantic_loggings/not_set/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-0.9.0/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.8.0
+Version: 0.9.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Configure Python logging from environment variables with pydantic (settings) Model
```

### Comparing `pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-0.9.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 src/pydantic_loggings/base/loggings.py
 src/pydantic_loggings/not_set/__init__.py
 src/pydantic_loggings/not_set/filters.py
 src/pydantic_loggings/not_set/formatters.py
 src/pydantic_loggings/not_set/handlers.py
 src/pydantic_loggings/not_set/loggers.py
 src/pydantic_loggings/not_set/loggings.py
-tests/test_main.py
+tests/test_mixin.py
+tests/test_types_.py
+tests/test_utils.py
```

