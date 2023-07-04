# Comparing `tmp/sotai-0.0.0.tar.gz` & `tmp/sotai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotai-0.0.0.tar", last modified: Thu Jun 29 19:53:50 2023, max compression
+gzip compressed data, was "sotai-0.1.0.tar", last modified: Tue Jul  4 21:17:51 2023, max compression
```

## Comparing `sotai-0.0.0.tar` & `sotai-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:50.224500 sotai-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-29 19:53:34.000000 sotai-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-29 19:53:50.224500 sotai-0.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:50.220500 sotai-0.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-29 19:53:34.000000 sotai-0.0.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-29 19:53:34.000000 sotai-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:53:50.224500 sotai-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:50.220500 sotai-0.0.0/sotai/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:50.220500 sotai-0.0.0/sotai/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/layers/categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/layers/numerical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-29 19:53:34.000000 sotai-0.0.0/sotai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:50.220500 sotai-0.0.0/sotai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-29 19:53:50.000000 sotai-0.0.0/sotai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 19:53:50.000000 sotai-0.0.0/sotai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:53:50.000000 sotai-0.0.0/sotai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-29 19:53:50.000000 sotai-0.0.0/sotai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 19:53:50.000000 sotai-0.0.0/sotai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:53:50.224500 sotai-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-29 19:53:34.000000 sotai-0.0.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-29 19:53:34.000000 sotai-0.0.0/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-29 19:53:34.000000 sotai-0.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-29 19:53:34.000000 sotai-0.0.0/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.031257 sotai-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 21:17:39.000000 sotai-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-04 21:17:51.031257 sotai-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.027257 sotai-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-04 21:17:39.000000 sotai-0.1.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-04 21:17:39.000000 sotai-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:17:51.031257 sotai-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.027257 sotai-0.1.0/sotai/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.027257 sotai-0.1.0/sotai/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/layers/categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/layers/numerical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/trained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.027257 sotai-0.1.0/sotai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.031257 sotai-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_trained_model.py
```

### Comparing `sotai-0.0.0/LICENSE` & `sotai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/PKG-INFO` & `sotai-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.0.0
+Version: 0.1.0
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
 Project-URL: Bug Reports, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,15 +24,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">SOTAI</h1>
 
 <p align='center'>
 <a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
-<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=dev" /></a>
+<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
 </p>
 
 A Library For Interpretable Machine Learning. This library is a PyTorch implementation of modeling techniques found in [Monotonic Calibrated Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-243.pdf).
 
 Installling the package:
 
 ```shell
@@ -41,22 +41,22 @@
 
 Importing the package:
 
 ```python
 import sotai
 ```
 
-## Documentation
+## SOTAI Web-App User Documentation
 
-All documentation is hosted at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk).
+You can find documentation for how to use the hosted web-app at [https://docs.sotai.ai/app](https://docs.sotai.ai/app)
 
 ## Contribution Guidelines
 
-See the guide on [contributing](https://docs.sotai.ai/sdk/contributing) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
+See the guide on [contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
 
 ## Examples
 
-For detailed examples on how to use the library, see [Examples](https://docs.sotai.ai/sdk/examples).
+For detailed examples on how to use the library, see [examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples).
 
 ## License
 
-[MIT](https://github.com/SOTAI-Labs/sdk/blob/dev/LICENSE)
+[MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: sotai Version: 0.0.0 Summary: A Python Library For
+Metadata-Version: 2.1 Name: sotai Version: 0.1.0 Summary: A Python Library For
 Calibrated Modeling Built With PyTorch Author-email: SOTAI
 sotai.ai> Maintainer-email: SOTAI
 sotai.ai> License: MIT Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-
 calibrated/issues Project-URL: Bug Reports, https://github.com/SOTAI-Labs/
-pytorch-calibrated/issues Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE
+pytorch-calibrated/issues Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Requires-Python: <3.11,>=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE
                               ****** SOTAI ******
   [https://img.shields.io/pypi/v/sotai] [https://github.com/SOTAI-Labs/sotai/
-               actions/workflows/tests.yml/badge.svg?branch=dev]
+              actions/workflows/tests.yml/badge.svg?branch=main]
 A Library For Interpretable Machine Learning. This library is a PyTorch
 implementation of modeling techniques found in [Monotonic Calibrated
 Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-
 243.pdf). Installling the package: ```shell pip install sotai ``` Importing the
-package: ```python import sotai ``` ## Documentation All documentation is
-hosted at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk). ##
-Contribution Guidelines See the guide on [contributing](https://docs.sotai.ai/
-sdk/contributing) for full details on how to contribute to the library. For any
+package: ```python import sotai ``` ## SOTAI Web-App User Documentation You can
+find documentation for how to use the hosted web-app at [https://docs.sotai.ai/
+app](https://docs.sotai.ai/app) ## Contribution Guidelines See the guide on
+[contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/
+CONTRIBUTING.md) for full details on how to contribute to the library. For any
 feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/
 sotai/issues). ## Examples For detailed examples on how to use the library, see
-[Examples](https://docs.sotai.ai/sdk/examples). ## License [MIT](https://
-github.com/SOTAI-Labs/sdk/blob/dev/LICENSE)
+[examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples). ##
+License [MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
```

### Comparing `sotai-0.0.0/docs/README.md` & `sotai-0.1.0/docs/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <h1 align="center">SOTAI</h1>
 
 <p align='center'>
 <a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
-<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=dev" /></a>
+<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
 </p>
 
 A Library For Interpretable Machine Learning. This library is a PyTorch implementation of modeling techniques found in [Monotonic Calibrated Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-243.pdf).
 
 Installling the package:
 
 ```shell
@@ -15,22 +15,22 @@
 
 Importing the package:
 
 ```python
 import sotai
 ```
 
-## Documentation
+## SOTAI Web-App User Documentation
 
-All documentation is hosted at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk).
+You can find documentation for how to use the hosted web-app at [https://docs.sotai.ai/app](https://docs.sotai.ai/app)
 
 ## Contribution Guidelines
 
-See the guide on [contributing](https://docs.sotai.ai/sdk/contributing) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
+See the guide on [contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
 
 ## Examples
 
-For detailed examples on how to use the library, see [Examples](https://docs.sotai.ai/sdk/examples).
+For detailed examples on how to use the library, see [examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples).
 
 ## License
 
-[MIT](https://github.com/SOTAI-Labs/sdk/blob/dev/LICENSE)
+[MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
                               ****** SOTAI ******
   [https://img.shields.io/pypi/v/sotai] [https://github.com/SOTAI-Labs/sotai/
-               actions/workflows/tests.yml/badge.svg?branch=dev]
+              actions/workflows/tests.yml/badge.svg?branch=main]
 A Library For Interpretable Machine Learning. This library is a PyTorch
 implementation of modeling techniques found in [Monotonic Calibrated
 Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-
 243.pdf). Installling the package: ```shell pip install sotai ``` Importing the
-package: ```python import sotai ``` ## Documentation All documentation is
-hosted at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk). ##
-Contribution Guidelines See the guide on [contributing](https://docs.sotai.ai/
-sdk/contributing) for full details on how to contribute to the library. For any
+package: ```python import sotai ``` ## SOTAI Web-App User Documentation You can
+find documentation for how to use the hosted web-app at [https://docs.sotai.ai/
+app](https://docs.sotai.ai/app) ## Contribution Guidelines See the guide on
+[contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/
+CONTRIBUTING.md) for full details on how to contribute to the library. For any
 feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/
 sotai/issues). ## Examples For detailed examples on how to use the library, see
-[Examples](https://docs.sotai.ai/sdk/examples). ## License [MIT](https://
-github.com/SOTAI-Labs/sdk/blob/dev/LICENSE)
+[examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples). ##
+License [MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
```

### Comparing `sotai-0.0.0/pyproject.toml` & `sotai-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 [project]
 name = "sotai"
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release. Use Semantic Versioning.
 #
 # NOTE: as part of the release flow, update this version immediately after release.
-version = "0.0.0"
+version = "0.1.0"
 description = "A Python Library For Calibrated Modeling Built With PyTorch"
 readme = "docs/README.md"
 license = {text = "MIT"}
 authors = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 maintainers = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 classifiers=[
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `sotai-0.0.0/sotai/data.py` & `sotai-0.1.0/sotai/data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/sotai/enums.py` & `sotai-0.1.0/sotai/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     CLASSIFICATION = "classification"
     REGRESSION = "regression"
 
 
 class LossType(_Enum):
     """The type of loss function to use."""
 
-    BINARY_CROSSENTROPY = "binary_crossentropy"
+    BINARY_CROSSENTROPY = "binary"
     HINGE = "hinge"
     HUBER = "huber"
     MAE = "mae"
     MSE = "mse"
 
 
 class Metric(_Enum):
@@ -58,16 +58,16 @@
     """The type of input keypoints to use.
 
     - FIXED: the input keypoints will be fixed during initialization.
     - LEARNED: the input keypoints will be learned during training after initialization.
     """
 
     FIXED = "fixed"
-    # Note: learned is only available for TFL currently.
-    LEARNED = "learned_interior"
+    # TODO: add learned interior functionality
+    # LEARNED = "learned_interior"
 
 
 class FeatureType(_Enum):
     """Type of feature.
 
     - UNKNOWN: a feature with a type that our system does not currently support.
     - NUMERICAL: a numerical feature that should be calibrated using an instance of
```

### Comparing `sotai-0.0.0/sotai/features.py` & `sotai-0.1.0/sotai/features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/sotai/layers/categorical_calibrator.py` & `sotai-0.1.0/sotai/layers/categorical_calibrator.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/sotai/layers/linear.py` & `sotai-0.1.0/sotai/layers/linear.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/sotai/layers/numerical_calibrator.py` & `sotai-0.1.0/sotai/layers/numerical_calibrator.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/sotai/models.py` & `sotai-0.1.0/sotai/models.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/sotai/pipeline.py` & `sotai-0.1.0/sotai/pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 import logging
 import os
 import pickle
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
-import torch
-from pydantic import BaseModel, Field
 
-from .data import CSVData, determine_feature_types, replace_missing_values
+from .api import (
+    get_api_key,
+    post_pipeline,
+    post_pipeline_config,
+    post_pipeline_feature_configs,
+    post_trained_model_analysis,
+)
+from .constants import SOTAI_API_ENDPOINT
+from .data import determine_feature_types, replace_missing_values
 from .enums import FeatureType, LossType, Metric, TargetType
-from .models import CalibratedLinear
+from .trained_model import TrainedModel
 from .training import train_and_evaluate_model
 from .types import (
     CategoricalFeatureConfig,
     Dataset,
     DatasetSplit,
     LinearConfig,
     NumericalFeatureConfig,
     PipelineConfig,
     PreparedData,
     TrainingConfig,
-    TrainingResults,
 )
 
 
 class Pipeline:  # pylint: disable=too-many-instance-attributes
     """A pipeline for calibrated modeling.
 
     The pipeline defines the configuration for training a calibrated model. The
@@ -107,14 +112,17 @@
         self.dataset_split: DatasetSplit = DatasetSplit(train=80, val=10, test=10)
 
         # Maps a pipeline config id to its corresponding `PipelineConfig`` instance.
         self.configs: Dict[int, PipelineConfig] = {}
         # Maps a dataset id to its corresponding `Dataset`` instance.
         self.datasets: Dict[int, Dataset] = {}
 
+        # Tracks
+        self.pipeline_uuid = None
+
     def prepare(  # pylint: disable=too-many-locals
         self,
         data: pd.DataFrame,
         pipeline_config_id: Optional[int] = None,
     ) -> Tuple[Dataset, PipelineConfig]:
         """Prepares the data and versions it along with the current pipeline config.
 
@@ -255,14 +263,83 @@
             A `Pipeline` instance.
         """
         with open(os.path.join(filepath, "pipeline.pkl"), "rb") as file:
             pipeline = pickle.load(file)
 
         return pipeline
 
+    def publish(self) -> Optional[str]:
+        """Uploads the pipeline to the SOTAI web client.
+
+        Returns:
+            If the pipeline was successfully uploaded, the pipeline UUID.
+            Otherwise, None.
+
+        """
+        self.pipeline_uuid = post_pipeline(self)
+        return self.pipeline_uuid
+
+    def analysis(self, trained_model: TrainedModel) -> Optional[str]:
+        """Charts the results for the specified trained model in the SOTAI web client.
+
+        This function requires an internet connection and a SOTAI account. The trained
+        model will be uploaded to the SOTAI web client for analysis.
+
+        If you would like to analyze the results for a trained model without uploading
+        it to the SOTAI web client, the data is available in `training_results`.
+        """
+        if trained_model.analysis_url:  # early exit if analysis has already been run.
+            return trained_model.analysis_url
+
+        if not get_api_key():
+            raise ValueError(
+                "You must have an API key to run analysis."
+                " Please visit app.sotai.ai to get an API key."
+            )
+
+        if self.pipeline_uuid is None:
+            self.pipeline_uuid = self.publish()
+
+        if self.pipeline_uuid is None:
+            return None
+
+        pipeline_config_uuid = post_pipeline_config(
+            self.pipeline_uuid, trained_model.pipeline_config
+        )
+
+        if pipeline_config_uuid is None:
+            return None
+
+        trained_model.pipeline_config.pipeline_config_uuid = pipeline_config_uuid
+
+        feature_config_response = post_pipeline_feature_configs(
+            pipeline_config_uuid, trained_model.pipeline_config.feature_configs
+        )
+
+        if feature_config_response is None:
+            return None
+
+        analysis_results = post_trained_model_analysis(
+            pipeline_config_uuid, trained_model
+        )
+
+        if analysis_results is None:
+            return None
+
+        trained_model.trained_model_uuid = analysis_results["trainedModelMetadataUuid"]
+
+        # TODO: update to use response analysisUrl once no longer broken.
+        analysis_url = (
+            f"{SOTAI_API_ENDPOINT}/pipelines/{self.pipeline_uuid}"
+            f"/trained-models/{trained_model.trained_model_uuid}"
+        )
+        trained_model.analysis_url = analysis_url
+
+        return analysis_url
+
     ############################################################################
     #                            Private Methods                               #
     ############################################################################
 
     def _version_pipeline_config(self, data: pd.DataFrame, pipeline_config_id: int):
         """Returns a new `PipelineConfig` instance verisoned from the current config."""
         pipeline_config = PipelineConfig(
@@ -302,107 +379,7 @@
                 logging.info(
                     "Removing feature %s because its data type is not supported.",
                     feature_name,
                 )
                 pipeline_config.feature_configs.pop(feature_name)
 
         return pipeline_config
-
-
-class TrainedModel(BaseModel):
-    """A trained calibrated model.
-
-    This model is a container for a trained calibrated model that provides useful
-    methods for using the model. The trained calibrated model is the result of running
-    the `train` method of a `Pipeline` instance.
-
-    Example:
-
-    ```python
-    data = pd.read_csv("data.csv")
-    predictions = trained_model.predict(data)
-    trained_model.analyze()
-    ```
-    """
-
-    dataset_id: int = Field(...)
-    pipeline_config: PipelineConfig = Field(...)
-    model_config: LinearConfig = Field(...)
-    training_config: TrainingConfig = Field(...)
-    training_results: TrainingResults = Field(...)
-    model: CalibratedLinear = Field(...)
-
-    class Config:  # pylint: disable=missing-class-docstring,too-few-public-methods
-        arbitrary_types_allowed = True
-
-    def predict(self, data: pd.DataFrame) -> np.ndarray:
-        """Returns predictions for the given data.
-
-        Args:
-            data: The data to be used for prediction. Must have all columns used for
-                training the model to be used.
-
-        Returns:
-            If the target type is regression, a numpy array of predictions. If the
-            target type is classification, a tuple containing a numpy array of
-            predictions (logits) and a numpy array of probabilities.
-        """
-        data = data.loc[:, list(self.pipeline_config.feature_configs.keys())]
-        data = replace_missing_values(data, self.pipeline_config.feature_configs)
-
-        csv_data = CSVData(data)
-        csv_data.prepare(self.model.features, None)
-        inputs = list(csv_data.batch(csv_data.num_examples))[0]
-        with torch.no_grad():
-            predictions = self.model(inputs).numpy()
-
-        if self.pipeline_config.target_type == TargetType.REGRESSION:
-            return predictions
-
-        return predictions, 1.0 / (1.0 + np.exp(-predictions))
-
-    def analysis(self):
-        """Charts the results for the specified trained model in the SOTAI web client.
-
-        This function requires an internet connection and a SOTAI account. The trained
-        model will be uploaded to the SOTAI web client for analysis.
-
-        If you would like to analyze the results for a trained model without uploading
-        it to the SOTAI web client, the data is available in `training_results`.
-        """
-        raise NotImplementedError()
-
-    def save(self, filepath: str):
-        """Saves the trained model to the specified directory.
-
-        Args:
-            filepath: The directory to save the trained model to. If the directory does
-                not exist, this function will attempt to create it. If the directory
-                already exists, this function will overwrite any existing content with
-                conflicting filenames.
-        """
-        if not os.path.exists(filepath):
-            os.makedirs(filepath)
-        with open(os.path.join(filepath, "trained_model_metadata.pkl"), "wb") as file:
-            pickle.dump(self.dict(exclude={"model"}), file)
-        model_path = f"{filepath}/trained_ptcm_model.pt"
-        torch.save(self.model, model_path)
-
-    @classmethod
-    def load(cls, filepath: str) -> TrainedModel:
-        """Loads a trained model from the specified filepath.
-
-        Args:
-            filepath: The filepath to load the trained model from. The filepath should
-                point to a file created by the `save` method of a `TrainedModel`
-                instance.
-
-        Returns:
-            A `TrainedModel` instance.
-        """
-        with open(os.path.join(filepath, "trained_model_metadata.pkl"), "rb") as file:
-            trained_model_metadata = pickle.load(file)
-        model_path = f"{filepath}/trained_ptcm_model.pt"
-        model = torch.load(model_path)
-        model.eval()
-
-        return TrainedModel(**trained_model_metadata, model=model)
```

### Comparing `sotai-0.0.0/sotai/training.py` & `sotai-0.1.0/sotai/training.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/sotai/types.py` & `sotai-0.1.0/sotai/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,26 +228,29 @@
         super().__init__(**kwargs)
 
 
 class PipelineConfig(BaseModel):
     """A configuration object for a `Pipeline`.
 
     Attributes:
+        id: The ID of the pipeline config.
+        pipeline_uuid: The UUID of the pipeline.
         target: The column name for the target.
         target_type: The type of the target.
         primary_metric: The primary metric to use for training and evaluation.
         feature_configs: A dictionary mapping the column name for a feature to its
             config.
         shuffle_data: Whether to shuffle the data before splitting it into train,
             validation, and test sets.
         drop_empty_percentage: Rows will be dropped if they are this percentage empty.
         dataset_split: The split of the dataset into train, validation, and test sets.
     """
 
     id: int = Field(...)
+    pipeline_config_uuid: Optional[str] = None
     target: str = Field(...)
     target_type: TargetType = Field(...)
     primary_metric: Metric = Field(...)
     feature_configs: Dict[
         str, Union[NumericalFeatureConfig, CategoricalFeatureConfig]
     ] = Field(...)
     shuffle_data: bool = Field(...)
```

### Comparing `sotai-0.0.0/sotai.egg-info/PKG-INFO` & `sotai-0.1.0/sotai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.0.0
+Version: 0.1.0
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
 Project-URL: Bug Reports, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,15 +24,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">SOTAI</h1>
 
 <p align='center'>
 <a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
-<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=dev" /></a>
+<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
 </p>
 
 A Library For Interpretable Machine Learning. This library is a PyTorch implementation of modeling techniques found in [Monotonic Calibrated Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-243.pdf).
 
 Installling the package:
 
 ```shell
@@ -41,22 +41,22 @@
 
 Importing the package:
 
 ```python
 import sotai
 ```
 
-## Documentation
+## SOTAI Web-App User Documentation
 
-All documentation is hosted at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk).
+You can find documentation for how to use the hosted web-app at [https://docs.sotai.ai/app](https://docs.sotai.ai/app)
 
 ## Contribution Guidelines
 
-See the guide on [contributing](https://docs.sotai.ai/sdk/contributing) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
+See the guide on [contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
 
 ## Examples
 
-For detailed examples on how to use the library, see [Examples](https://docs.sotai.ai/sdk/examples).
+For detailed examples on how to use the library, see [examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples).
 
 ## License
 
-[MIT](https://github.com/SOTAI-Labs/sdk/blob/dev/LICENSE)
+[MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: sotai Version: 0.0.0 Summary: A Python Library For
+Metadata-Version: 2.1 Name: sotai Version: 0.1.0 Summary: A Python Library For
 Calibrated Modeling Built With PyTorch Author-email: SOTAI
 sotai.ai> Maintainer-email: SOTAI
 sotai.ai> License: MIT Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-
 calibrated/issues Project-URL: Bug Reports, https://github.com/SOTAI-Labs/
-pytorch-calibrated/issues Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE
+pytorch-calibrated/issues Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Requires-Python: <3.11,>=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE
                               ****** SOTAI ******
   [https://img.shields.io/pypi/v/sotai] [https://github.com/SOTAI-Labs/sotai/
-               actions/workflows/tests.yml/badge.svg?branch=dev]
+              actions/workflows/tests.yml/badge.svg?branch=main]
 A Library For Interpretable Machine Learning. This library is a PyTorch
 implementation of modeling techniques found in [Monotonic Calibrated
 Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-
 243.pdf). Installling the package: ```shell pip install sotai ``` Importing the
-package: ```python import sotai ``` ## Documentation All documentation is
-hosted at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk). ##
-Contribution Guidelines See the guide on [contributing](https://docs.sotai.ai/
-sdk/contributing) for full details on how to contribute to the library. For any
+package: ```python import sotai ``` ## SOTAI Web-App User Documentation You can
+find documentation for how to use the hosted web-app at [https://docs.sotai.ai/
+app](https://docs.sotai.ai/app) ## Contribution Guidelines See the guide on
+[contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/
+CONTRIBUTING.md) for full details on how to contribute to the library. For any
 feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/
 sotai/issues). ## Examples For detailed examples on how to use the library, see
-[Examples](https://docs.sotai.ai/sdk/examples). ## License [MIT](https://
-github.com/SOTAI-Labs/sdk/blob/dev/LICENSE)
+[examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples). ##
+License [MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
```

### Comparing `sotai-0.0.0/sotai.egg-info/SOURCES.txt` & `sotai-0.1.0/sotai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 LICENSE
 pyproject.toml
 docs/README.md
 sotai/__init__.py
+sotai/api.py
 sotai/constants.py
 sotai/data.py
 sotai/enums.py
 sotai/features.py
 sotai/models.py
 sotai/pipeline.py
+sotai/trained_model.py
 sotai/training.py
 sotai/types.py
 sotai.egg-info/PKG-INFO
 sotai.egg-info/SOURCES.txt
 sotai.egg-info/dependency_links.txt
 sotai.egg-info/requires.txt
 sotai.egg-info/top_level.txt
 sotai/layers/__init__.py
 sotai/layers/categorical_calibrator.py
 sotai/layers/linear.py
 sotai/layers/numerical_calibrator.py
+tests/test_api.py
 tests/test_data.py
 tests/test_features.py
 tests/test_models.py
-tests/test_pipeline.py
+tests/test_pipeline.py
+tests/test_trained_model.py
```

### Comparing `sotai-0.0.0/tests/test_data.py` & `sotai-0.1.0/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,14 @@
     }
 
 
 def test_replace_missing_values(data, feature_configs):
     """Tests that missing values are properly replaced."""
     data["numerical"].values[-1] = np.nan
     data = replace_missing_values(data, feature_configs)
-    print(data["categorical"])
     assert data["categorical"].values[-1] == MISSING_CATEGORY_VALUE
     assert data["numerical"].values[-1] == MISSING_NUMERICAL_VALUE
 
 
 def test_determine_feature_types(data, unknown_data):
     """Tests the determination of feature types from data."""
     data[unknown_data["header"]] = unknown_data["data"]
@@ -130,16 +129,14 @@
         data.to_csv(datapath, index=False)
         csv_data = CSVData(datapath)
         assert csv_data.dataset == datapath
     else:
         csv_data = CSVData(data)
         assert csv_data.dataset.equals(data)
 
-    print(csv_data.data)
-    print(data)
     assert csv_data.data.equals(data)
     assert csv_data.headers == list(data.columns)
     assert csv_data.num_examples == len(data)
     assert csv_data.prepared_data is None
     # pylint: disable=protected-access
     assert csv_data._prepared_data_tensor is None
     assert csv_data._targets_tensor is None
```

### Comparing `sotai-0.0.0/tests/test_features.py` & `sotai-0.1.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/tests/test_models.py` & `sotai-0.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `sotai-0.0.0/tests/test_pipeline.py` & `sotai-0.1.0/tests/test_pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,32 @@
 """Tests for Pipeline."""
 
-import numpy as np
-import pandas as pd
 import pytest
 
-from sotai import (
-    CategoricalFeatureConfig,
-    FeatureType,
-    Metric,
-    NumericalFeatureConfig,
-    Pipeline,
-    TargetType,
-    TrainedModel,
-)
-from sotai.models import CalibratedLinear
-
-from .utils import construct_trained_model
-
-
-@pytest.fixture(name="test_target")
-def fixture_test_target():
-    """Returns a test target."""
-    return "target"
-
-
-@pytest.fixture(name="test_categories")
-def fixture_test_categories():
-    """Returns a list of test categories."""
-    return ["a", "b", "c", "d"]
-
+from sotai import FeatureType, Metric, Pipeline, TargetType
 
-@pytest.fixture(name="test_data")
-def fixture_test_data(test_categories, test_target):
-    """Returns a test dataset."""
-    return pd.DataFrame(
-        {
-            "numerical": np.random.rand(100),
-            "categorical": np.random.choice(test_categories, 100),
-            test_target: np.random.randint(0, 2, 100),
-        }
-    )
-
-
-@pytest.fixture(name="test_feature_names")
-def fixture_test_feature_names(test_data, test_target):
-    """Returns a list of test feature names."""
-    return test_data.columns.drop(test_target).to_list()
-
-
-@pytest.fixture(name="test_feature_configs")
-def fixture_test_feature_configs(test_categories):
-    """Returns a list of test features."""
-    return {
-        "numerical": NumericalFeatureConfig(name="numerical"),
-        "categorical": CategoricalFeatureConfig(
-            name="categorical", categories=test_categories
-        ),
-    }
+from .fixtures import (  # pylint: disable=unused-import
+    fixture_test_categories,
+    fixture_test_data,
+    fixture_test_feature_configs,
+    fixture_test_feature_names,
+    fixture_test_target,
+)
 
 
 @pytest.mark.parametrize(
     "target_type,expected_primary_metric",
     [(TargetType.CLASSIFICATION, Metric.AUC), (TargetType.REGRESSION, Metric.MSE)],
 )
-def test_init(test_feature_names, test_target, target_type, expected_primary_metric):
+def test_init(
+    test_feature_names: fixture_test_feature_names,
+    test_target: fixture_test_target,
+    target_type,
+    expected_primary_metric,
+):
     """Tests pipeline initialization for a classification target."""
     pipeline = Pipeline(test_feature_names, test_target, target_type)
     assert pipeline.name == f"{test_target}_{target_type}"
     assert pipeline.target == test_target
     assert pipeline.target_type == target_type
     assert pipeline.primary_metric == expected_primary_metric
     assert len(pipeline.feature_configs) == 2
@@ -76,29 +35,38 @@
     assert numerical_config.type == FeatureType.NUMERICAL
     categorical_config = pipeline.feature_configs["categorical"]
     assert categorical_config.name == "categorical"
     # Note: we expect the default config to be numerical if not specified.
     assert categorical_config.type == FeatureType.NUMERICAL
 
 
-def test_init_with_categories(test_feature_names, test_target, test_categories):
+def test_init_with_categories(
+    test_feature_names: fixture_test_feature_names,
+    test_target: fixture_test_target,
+    test_categories: fixture_test_categories,
+):
     """Tests pipeline initialization with specified categories."""
     pipeline = Pipeline(
         test_feature_names,
         test_target,
         TargetType.CLASSIFICATION,
         categories={"categorical": test_categories},
     )
     categorical_config = pipeline.feature_configs["categorical"]
     assert categorical_config.name == "categorical"
     assert categorical_config.type == FeatureType.CATEGORICAL
     assert categorical_config.categories == test_categories
 
 
-def test_prepare(test_data, test_feature_names, test_target, test_categories):
+def test_prepare(
+    test_data: fixture_test_data,
+    test_feature_names: fixture_test_feature_names,
+    test_target: fixture_test_target,
+    test_categories: fixture_test_target,
+):
     """Tests the pipeline prepare function."""
     pipeline = Pipeline(
         test_feature_names, test_target, target_type=TargetType.CLASSIFICATION
     )
     # We set shuffle to false to ensure the data is split in the same way.
     pipeline.shuffle_data = False
     pipeline.dataset_split.train = 80
@@ -128,15 +96,18 @@
     "target_type",
     [
         (TargetType.CLASSIFICATION),
         (TargetType.REGRESSION),
     ],
 )
 def test_train_calibrated_linear_model(
-    test_data, test_feature_names, test_target, target_type
+    test_data,
+    test_feature_names: fixture_test_feature_names,
+    test_target: fixture_test_target,
+    target_type,
 ):
     """Tests pipeline training for calibrated linear regression model."""
     pipeline = Pipeline(test_feature_names, test_target, target_type)
     pipeline.shuffle_data = False
     pipeline.dataset_split.train = 60
     pipeline.dataset_split.val = 20
     pipeline.dataset_split.test = 20
@@ -146,15 +117,20 @@
     assert trained_model
     assert trained_model.dataset_id == 0
     assert pipeline.datasets[trained_model.dataset_id]
     assert trained_model.pipeline_config.id == 0
     assert pipeline.configs[trained_model.pipeline_config.id]
 
 
-def test_pipeline_save_load(test_data, test_feature_names, test_target, tmp_path):
+def test_pipeline_save_load(
+    test_data: fixture_test_data,
+    test_feature_names: fixture_test_feature_names,
+    test_target: fixture_test_target,
+    tmp_path,
+):
     """Tests that an instance of `Pipeline` can be successfully saved and loaded."""
     pipeline = Pipeline(test_feature_names, test_target, TargetType.CLASSIFICATION)
     _ = pipeline.train(test_data)
     pipeline.save(tmp_path)
     loaded_pipeline = Pipeline.load(tmp_path)
     assert isinstance(loaded_pipeline, Pipeline)
     assert loaded_pipeline.name == pipeline.name
@@ -166,43 +142,7 @@
     for dataset_id, loaded_dataset in loaded_pipeline.datasets.items():
         dataset = pipeline.datasets[dataset_id]
         assert loaded_dataset.id == dataset.id
         assert loaded_dataset.pipeline_config_id == dataset.pipeline_config_id
         assert loaded_dataset.prepared_data.train.equals(dataset.prepared_data.train)
         assert loaded_dataset.prepared_data.val.equals(dataset.prepared_data.val)
         assert loaded_dataset.prepared_data.test.equals(dataset.prepared_data.test)
-
-
-def test_trained_classification_model_predict(test_data, test_feature_configs):
-    """Tests the predict function on a trained model."""
-    trained_model = construct_trained_model(
-        TargetType.CLASSIFICATION, test_data, test_feature_configs
-    )
-    predictions, probabilities = trained_model.predict(test_data)
-    assert isinstance(predictions, np.ndarray)
-    assert len(predictions) == len(test_data)
-    assert isinstance(probabilities, np.ndarray)
-    assert len(probabilities) == len(test_data)
-
-
-def test_trained_regression_model_predict(test_data, test_feature_configs):
-    """Tests the predict function on a trained model."""
-    trained_model = construct_trained_model(
-        TargetType.REGRESSION, test_data, test_feature_configs
-    )
-    predictions = trained_model.predict(test_data)
-    assert isinstance(predictions, np.ndarray)
-    assert len(predictions) == len(test_data)
-
-
-def test_trained_model_save_load(test_data, test_feature_configs, tmp_path):
-    """Tests that a `TrainedModel` can be successfully saved and then loaded."""
-    trained_model = construct_trained_model(
-        TargetType.CLASSIFICATION, test_data, test_feature_configs
-    )
-    trained_model.save(tmp_path)
-    loaded_trained_model = TrainedModel.load(tmp_path)
-    assert isinstance(loaded_trained_model, TrainedModel)
-    assert loaded_trained_model.dict(exclude={"model"}) == trained_model.dict(
-        exclude={"model"}
-    )
-    assert isinstance(loaded_trained_model.model, CalibratedLinear)
```

