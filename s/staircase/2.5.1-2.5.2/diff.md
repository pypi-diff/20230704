# Comparing `tmp/staircase-2.5.1.tar.gz` & `tmp/staircase-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staircase-2.5.1.tar", max compression
+gzip compressed data, was "staircase-2.5.2.tar", max compression
```

## Comparing `staircase-2.5.1.tar` & `staircase-2.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1074 2023-04-25 05:39:05.351480 staircase-2.5.1/LICENSE
--rw-r--r--   0        0        0     8425 2023-04-25 05:39:05.351480 staircase-2.5.1/README.md
--rw-r--r--   0        0        0     2713 2023-04-25 05:39:05.363480 staircase-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     1044 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/__init__.py
--rw-r--r--   0        0        0      255 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/_typing.py
--rw-r--r--   0        0        0      806 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/constants.py
--rw-r--r--   0        0        0        0 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/__init__.py
--rw-r--r--   0        0        0      756 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/accessor.py
--rw-r--r--   0        0        0     2439 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/arrays/__init__.py
--rw-r--r--   0        0        0     2183 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/arrays/accessor.py
--rw-r--r--   0        0        0    21413 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/arrays/docstrings.py
--rw-r--r--   0        0        0     9629 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/arrays/extension.py
--rw-r--r--   0        0        0      409 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/exceptions/__init__.py
--rw-r--r--   0        0        0     6496 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/layering.py
--rw-r--r--   0        0        0     1890 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/__init__.py
--rw-r--r--   0        0        0     5454 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/arithmetic.py
--rw-r--r--   0        0        0     4217 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/common.py
--rw-r--r--   0        0        0    13779 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/docstrings.py
--rw-r--r--   0        0        0     3615 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/logical.py
--rw-r--r--   0        0        0     6875 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/masking.py
--rw-r--r--   0        0        0     4785 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/ops/relational.py
--rw-r--r--   0        0        0     1097 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/ops/rops.py
--rw-r--r--   0        0        0     3420 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/sampling.py
--rw-r--r--   0        0        0     6651 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/slicing.py
--rw-r--r--   0        0        0    25237 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stairs.py
--rw-r--r--   0        0        0      721 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stats/__init__.py
--rw-r--r--   0        0        0     4001 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stats/distribution.py
--rw-r--r--   0        0        0    11489 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stats/docstrings.py
--rw-r--r--   0        0        0     9555 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stats/statistic.py
--rw-r--r--   0        0        0     2377 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/docstrings/__init__.py
--rw-r--r--   0        0        0     7256 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/docstrings/examples.py
--rw-r--r--   0        0        0     9798 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/docstrings/slicing.py
--rw-r--r--   0        0        0        0 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/io/json.py
--rw-r--r--   0        0        0        0 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/io/pickle.py
--rw-r--r--   0        0        0        0 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/plotting/__init__.py
--rw-r--r--   0        0        0      959 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/plotting/accessor.py
--rw-r--r--   0        0        0      826 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/plotting/docstrings.py
--rw-r--r--   0        0        0     3081 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/plotting/matplotlib.py
--rw-r--r--   0        0        0     4185 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/test_data.py
--rw-r--r--   0        0        0     1498 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/util/__init__.py
--rw-r--r--   0        0        0     1630 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/util/_decorators.py
--rw-r--r--   0        0        0    10381 1970-01-01 00:00:00.000000 staircase-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-04 10:48:56.842075 staircase-2.5.2/LICENSE
+-rw-r--r--   0        0        0     8425 2023-07-04 10:48:56.842075 staircase-2.5.2/README.md
+-rw-r--r--   0        0        0     2849 2023-07-04 10:48:56.850075 staircase-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1044 2023-07-04 10:48:56.850075 staircase-2.5.2/staircase/__init__.py
+-rw-r--r--   0        0        0      255 2023-07-04 10:48:56.850075 staircase-2.5.2/staircase/_typing.py
+-rw-r--r--   0        0        0      806 2023-07-04 10:48:56.850075 staircase-2.5.2/staircase/constants.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:48:56.850075 staircase-2.5.2/staircase/core/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-04 10:48:56.850075 staircase-2.5.2/staircase/core/accessor.py
+-rw-r--r--   0        0        0     2439 2023-07-04 10:48:56.850075 staircase-2.5.2/staircase/core/arrays/__init__.py
+-rw-r--r--   0        0        0     2183 2023-07-04 10:48:56.850075 staircase-2.5.2/staircase/core/arrays/accessor.py
+-rw-r--r--   0        0        0    21413 2023-07-04 10:48:56.850075 staircase-2.5.2/staircase/core/arrays/docstrings.py
+-rw-r--r--   0        0        0     9629 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/arrays/extension.py
+-rw-r--r--   0        0        0      409 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     6496 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/layering.py
+-rw-r--r--   0        0        0     1890 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/ops/__init__.py
+-rw-r--r--   0        0        0     5454 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/ops/arithmetic.py
+-rw-r--r--   0        0        0     4217 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/ops/common.py
+-rw-r--r--   0        0        0    13779 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/ops/docstrings.py
+-rw-r--r--   0        0        0     3615 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/ops/logical.py
+-rw-r--r--   0        0        0     6875 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/ops/masking.py
+-rw-r--r--   0        0        0     4785 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/ops/relational.py
+-rw-r--r--   0        0        0     1097 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/ops/rops.py
+-rw-r--r--   0        0        0     3420 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/sampling.py
+-rw-r--r--   0        0        0     6651 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/slicing.py
+-rw-r--r--   0        0        0    25237 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/stairs.py
+-rw-r--r--   0        0        0      721 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/stats/__init__.py
+-rw-r--r--   0        0        0     4001 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/stats/distribution.py
+-rw-r--r--   0        0        0    11489 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/stats/docstrings.py
+-rw-r--r--   0        0        0     9555 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/core/stats/statistic.py
+-rw-r--r--   0        0        0     2377 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/docstrings/__init__.py
+-rw-r--r--   0        0        0     7256 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/docstrings/examples.py
+-rw-r--r--   0        0        0     9798 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/docstrings/slicing.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/io/json.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/io/pickle.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/plotting/__init__.py
+-rw-r--r--   0        0        0      959 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/plotting/accessor.py
+-rw-r--r--   0        0        0      826 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/plotting/docstrings.py
+-rw-r--r--   0        0        0     3081 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/plotting/matplotlib.py
+-rw-r--r--   0        0        0     4185 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/test_data.py
+-rw-r--r--   0        0        0     1498 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/util/__init__.py
+-rw-r--r--   0        0        0     1630 2023-07-04 10:48:56.854075 staircase-2.5.2/staircase/util/_decorators.py
+-rw-r--r--   0        0        0    10276 1970-01-01 00:00:00.000000 staircase-2.5.2/PKG-INFO
```

### Comparing `staircase-2.5.1/LICENSE` & `staircase-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/README.md` & `staircase-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/pyproject.toml` & `staircase-2.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "staircase"
-version = "2.5.1"
+version = "2.5.2"
 description = "A data analysis package based on modelling and manipulation of mathematical step functions. Strongly aligned with pandas."
 readme = "README.md"
 authors = ["Riley Clement <venaturum@gmail.com>"]
 maintainers = ["Riley Clement <venaturum@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/staircase-dev/staircase"
 homepage = "https://staircase.dev"
@@ -40,15 +40,14 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/staircase-dev/staircase/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-matplotlib = ">=2"
 pytz = "*"
 typing-extensions = "^4.4.0"
 
 [[tool.poetry.dependencies.pandas]]
 python = ">=3.7,<3.10"
 version = "^1"
 
@@ -60,14 +59,22 @@
 python = ">=3.7,<3.10"
 version = "^1.15"
 
 [[tool.poetry.dependencies.numpy]]
 python = "^3.10"
 version = "^1.21.2"
 
+[[tool.poetry.dependencies.matplotlib]]
+python = ">=3.7,<3.11"
+version = ">=2"
+
+[[tool.poetry.dependencies.matplotlib]]
+python = "^3.11"
+version = "^3.6"
+
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6"
 pytest = "^6"
 pytest-cov = "*"
 sphinx = "*"
 nbsphinx = ">=0.8.5"
```

### Comparing `staircase-2.5.1/staircase/__init__.py` & `staircase-2.5.2/staircase/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/constants.py` & `staircase-2.5.2/staircase/constants.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/accessor.py` & `staircase-2.5.2/staircase/core/accessor.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/arrays/__init__.py` & `staircase-2.5.2/staircase/core/arrays/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/arrays/accessor.py` & `staircase-2.5.2/staircase/core/arrays/accessor.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/arrays/docstrings.py` & `staircase-2.5.2/staircase/core/arrays/docstrings.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/arrays/extension.py` & `staircase-2.5.2/staircase/core/arrays/extension.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/layering.py` & `staircase-2.5.2/staircase/core/layering.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/ops/__init__.py` & `staircase-2.5.2/staircase/core/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/ops/arithmetic.py` & `staircase-2.5.2/staircase/core/ops/arithmetic.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/ops/common.py` & `staircase-2.5.2/staircase/core/ops/common.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/ops/docstrings.py` & `staircase-2.5.2/staircase/core/ops/docstrings.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/ops/logical.py` & `staircase-2.5.2/staircase/core/ops/logical.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/ops/masking.py` & `staircase-2.5.2/staircase/core/ops/masking.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/ops/relational.py` & `staircase-2.5.2/staircase/core/ops/relational.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/ops/rops.py` & `staircase-2.5.2/staircase/core/ops/rops.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/sampling.py` & `staircase-2.5.2/staircase/core/sampling.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/slicing.py` & `staircase-2.5.2/staircase/core/slicing.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/stairs.py` & `staircase-2.5.2/staircase/core/stairs.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/stats/__init__.py` & `staircase-2.5.2/staircase/core/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/stats/distribution.py` & `staircase-2.5.2/staircase/core/stats/distribution.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/stats/docstrings.py` & `staircase-2.5.2/staircase/core/stats/docstrings.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/core/stats/statistic.py` & `staircase-2.5.2/staircase/core/stats/statistic.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/docstrings/__init__.py` & `staircase-2.5.2/staircase/docstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/docstrings/examples.py` & `staircase-2.5.2/staircase/docstrings/examples.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/docstrings/slicing.py` & `staircase-2.5.2/staircase/docstrings/slicing.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/plotting/accessor.py` & `staircase-2.5.2/staircase/plotting/accessor.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/plotting/docstrings.py` & `staircase-2.5.2/staircase/plotting/docstrings.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/plotting/matplotlib.py` & `staircase-2.5.2/staircase/plotting/matplotlib.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/test_data.py` & `staircase-2.5.2/staircase/test_data.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/util/__init__.py` & `staircase-2.5.2/staircase/util/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/staircase/util/_decorators.py` & `staircase-2.5.2/staircase/util/_decorators.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.1/PKG-INFO` & `staircase-2.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staircase
-Version: 2.5.1
+Version: 2.5.2
 Summary: A data analysis package based on modelling and manipulation of mathematical step functions. Strongly aligned with pandas.
 Home-page: https://staircase.dev
 License: MIT
 Keywords: Staircase,Step Functions,Mathematics,Data Analysis,Analysis,Data Structures,Time Signal,Simulation Output
 Author: Riley Clement
 Author-email: venaturum@gmail.com
 Maintainer: Riley Clement
@@ -15,22 +15,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: codecov
-Requires-Dist: matplotlib (>=2)
+Requires-Dist: matplotlib (>=2) ; python_version >= "3.7" and python_version < "3.11"
+Requires-Dist: matplotlib (>=3.6,<4.0) ; python_version >= "3.11" and python_version < "4.0"
 Requires-Dist: numpy (>=1.15,<2.0) ; python_version >= "3.7" and python_version < "3.10"
 Requires-Dist: numpy (>=1.21.2,<2.0.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: pandas (>=1,<2) ; python_version >= "3.7" and python_version < "3.10"
 Requires-Dist: pandas (>=1.3.4,<3) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: pytz
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/staircase-dev/staircase/issues
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: staircase Version: 2.5.1 Summary: A data analysis
+Metadata-Version: 2.1 Name: staircase Version: 2.5.2 Summary: A data analysis
 package based on modelling and manipulation of mathematical step functions.
 Strongly aligned with pandas. Home-page: https://staircase.dev License: MIT
 Keywords: Staircase,Step Functions,Mathematics,Data Analysis,Analysis,Data
 Structures,Time Signal,Simulation Output Author: Riley Clement Author-email:
 venaturum@gmail.com Maintainer: Riley Clement Maintainer-email:
 venaturum@gmail.com Requires-Python: >=3.7,<4.0 Classifier: Intended Audience
 :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Scientific/Engineering Provides-Extra: codecov Requires-Dist:
-matplotlib (>=2) Requires-Dist: numpy (>=1.15,<2.0) ; python_version >= "3.7"
-and python_version < "3.10" Requires-Dist: numpy (>=1.21.2,<2.0.0) ;
-python_version >= "3.10" and python_version < "4.0" Requires-Dist: pandas
-(>=1,<2) ; python_version >= "3.7" and python_version < "3.10" Requires-Dist:
-pandas (>=1.3.4,<3) ; python_version >= "3.10" and python_version < "4.0"
-Requires-Dist: pytz Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) Project-
-URL: Bug Tracker, https://github.com/staircase-dev/staircase/issues Project-
-URL: Documentation, https://staircase.dev Project-URL: Repository, https://
-github.com/staircase-dev/staircase Description-Content-Type: text/markdown
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering Provides-Extra: codecov Requires-Dist: matplotlib (>=2) ;
+python_version >= "3.7" and python_version < "3.11" Requires-Dist: matplotlib
+(>=3.6,<4.0) ; python_version >= "3.11" and python_version < "4.0" Requires-
+Dist: numpy (>=1.15,<2.0) ; python_version >= "3.7" and python_version < "3.10"
+Requires-Dist: numpy (>=1.21.2,<2.0.0) ; python_version >= "3.10" and
+python_version < "4.0" Requires-Dist: pandas (>=1,<2) ; python_version >= "3.7"
+and python_version < "3.10" Requires-Dist: pandas (>=1.3.4,<3) ; python_version
+>= "3.10" and python_version < "4.0" Requires-Dist: pytz Requires-Dist: typing-
+extensions (>=4.4.0,<5.0.0) Project-URL: Bug Tracker, https://github.com/
+staircase-dev/staircase/issues Project-URL: Documentation, https://
+staircase.dev Project-URL: Repository, https://github.com/staircase-dev/
+staircase Description-Content-Type: text/markdown
                                [staircase_logo]
  [https://pepy.tech/badge/staircase] [https://img.shields.io/pypi/pyversions/
   staircase] [https://img.shields.io/pypi/v/staircase] [https://anaconda.org/
  conda-forge/staircase/badges/version.svg?branch=master&kill_cache=1] [http://
             img.shields.io/:license-mit-blue.svg?style=flat-square]
   Github CI"> [https://github.com/staircase-dev/staircase/actions/workflows/
                                ci.yml/badge.svg]
```

