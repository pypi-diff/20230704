# Comparing `tmp/relaxed-0.2.2.tar.gz` & `tmp/relaxed-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relaxed-0.2.2.tar", last modified: Fri Oct 28 08:21:13 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `relaxed-0.2.2.tar` & `relaxed-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 08:21:13.623095 relaxed-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-28 08:21:05.000000 relaxed-0.2.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-10-28 08:21:05.000000 relaxed-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-28 08:21:05.000000 relaxed-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-10-28 08:21:05.000000 relaxed-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6944 2022-10-28 08:21:13.623095 relaxed-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5780 2022-10-28 08:21:05.000000 relaxed-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     6987 2022-10-28 08:21:05.000000 relaxed-0.2.2/list_of_operations.md
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-10-28 08:21:05.000000 relaxed-0.2.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-10-28 08:21:05.000000 relaxed-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)    32802 2022-10-28 08:21:05.000000 relaxed-0.2.2/relaxed-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-10-28 08:21:13.623095 relaxed-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-28 08:21:05.000000 relaxed-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 08:21:13.619095 relaxed-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 08:21:13.619095 relaxed-0.2.2/src/relaxed/
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-28 08:21:05.000000 relaxed-0.2.2/src/relaxed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-28 08:21:05.000000 relaxed-0.2.2/src/relaxed/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-28 08:21:13.000000 relaxed-0.2.2/src/relaxed/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-10-28 08:21:05.000000 relaxed-0.2.2/src/relaxed/dummy_pyhf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-10-28 08:21:05.000000 relaxed-0.2.2/src/relaxed/infer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-10-28 08:21:05.000000 relaxed-0.2.2/src/relaxed/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-10-28 08:21:05.000000 relaxed-0.2.2/src/relaxed/mle.py
--rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-10-28 08:21:05.000000 relaxed-0.2.2/src/relaxed/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 08:21:05.000000 relaxed-0.2.2/src/relaxed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 08:21:13.623095 relaxed-0.2.2/src/relaxed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6944 2022-10-28 08:21:13.000000 relaxed-0.2.2/src/relaxed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-28 08:21:13.000000 relaxed-0.2.2/src/relaxed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 08:21:13.000000 relaxed-0.2.2/src/relaxed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-10-28 08:21:13.000000 relaxed-0.2.2/src/relaxed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-28 08:21:13.000000 relaxed-0.2.2/src/relaxed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 08:21:13.623095 relaxed-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-10-28 08:21:05.000000 relaxed-0.2.2/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-10-28 08:21:05.000000 relaxed-0.2.2/tests/test_infer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-10-28 08:21:05.000000 relaxed-0.2.2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5997 2022-10-28 08:21:05.000000 relaxed-0.2.2/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-28 08:21:05.000000 relaxed-0.2.2/tests/test_package.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 relaxed-0.3.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relaxed-0.3.0/.gitattributes
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relaxed-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 relaxed-0.3.0/.readthedocs.yml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 relaxed-0.3.0/CITATION.cff
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 relaxed-0.3.0/list_of_operations.md
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 relaxed-0.3.0/noxfile.py
+-rw-r--r--   0        0        0    32802 2020-02-02 00:00:00.000000 relaxed-0.3.0/relaxed-logo.png
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 relaxed-0.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 relaxed-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 relaxed-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 relaxed-0.3.0/binder/postBuild
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/modules.rst
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed-101.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed.infer.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed.metrics.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed.mle.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed.ops.rst
+-rw-r--r--   0        0        0   268660 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/binning.ipynb
+-rw-r--r--   0        0        0   154655 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/cuts.ipynb
+-rw-r--r--   0        0        0    50427 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/diffable_histograms.ipynb
+-rw-r--r--   0        0        0    36294 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/neos.ipynb
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/requirements.txt
+-rw-r--r--   0        0        0   198248 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/simple-analysis-optimisation.ipynb
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/__init__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/infer.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/metrics.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/mle.py
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/ops.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/py.typed
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/_compat/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/_compat/typing.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/dummy_pyhf.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_fit.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_infer.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_metrics.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_ops.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_package.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 relaxed-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 relaxed-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 relaxed-0.3.0/README.md
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 relaxed-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7615 2020-02-02 00:00:00.000000 relaxed-0.3.0/PKG-INFO
```

### Comparing `relaxed-0.2.2/LICENSE` & `relaxed-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Nathan Simpson.
+Copyright (c) 2023, Nathan Simpson.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `relaxed-0.2.2/PKG-INFO` & `relaxed-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,53 @@
 Metadata-Version: 2.1
 Name: relaxed
-Version: 0.2.2
-Summary: Differentiable versions of common operations in high-energy physics.
-Home-page: https://github.com/gradhep/relaxed
-Author: Nathan Simpson
-Author-email: n.s@cern.ch
-Maintainer: Nathan Simpson
-Maintainer-email: n.s@cern.ch
-License: BSD-3-Clause
-Project-URL: Documentation, https://relaxed.readthedocs.io/
+Version: 0.3.0
+Summary: Differentiable versions of common HEP operations.
+Project-URL: Homepage, https://github.com/gradhep/relaxed
 Project-URL: Bug Tracker, https://github.com/gradhep/relaxed/issues
 Project-URL: Discussions, https://github.com/gradhep/relaxed/discussions
 Project-URL: Changelog, https://github.com/gradhep/relaxed/releases
-Platform: Any
+Author-email: Nathan Simpson <nsimpson@turing.ac.uk>
+License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Requires-Dist: equinox
+Requires-Dist: jaxopt>=0.7
+Requires-Dist: optax>=0.1.2
+Requires-Dist: typing-extensions>=4.6; python_version < '3.11'
 Provides-Extra: dev
+Requires-Dist: pytest-cov>=3; extra == 'dev'
+Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: myst-parser>=0.13; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
+Requires-Dist: sphinx-book-theme>=0.1.0; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx>=4.0; extra == 'docs'
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: iminuit; extra == 'test'
+Requires-Dist: pyhf[jax]>=0.7.0; extra == 'test'
+Requires-Dist: pytest-cov>=3; extra == 'test'
+Requires-Dist: pytest>=6; extra == 'test'
+Description-Content-Type: text/markdown
 
 <p align="center">
   <img width="40%" alt="relaxed logo" src=relaxed-logo.png><br>
   <br>
   <a href="https://github.com/gradhep/relaxed/actions">
     <img alt="GitHub Workflow Status" src="https://github.com/gradhep/relaxed/workflows/CI/badge.svg">
   </a>
@@ -45,83 +61,108 @@
     <img alt="Zenodo DOI" src="https://zenodo.org/badge/264991846.svg">
   </a>
   <a href="https://mybinder.org/v2/gh/gradhep/relaxed/main?labpath=examples%2Fcuts.ipynb">
     <img alt="Binder" src="https://mybinder.org/badge_logo.svg">
   </a>
 </p>
 
-
-[actions-badge]:            https://github.com/gradhep/relaxed/workflows/CI/badge.svg
-[actions-link]:             https://github.com/gradhep/relaxed/actions
-[black-badge]:              https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]:               https://github.com/psf/black
-[conda-badge]:              https://img.shields.io/conda/vn/conda-forge/relaxed
-[conda-link]:               https://github.com/conda-forge/relaxed-feedstock
-[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
-[github-discussions-link]:  https://github.com/gradhep/relaxed/discussions
-[gitter-badge]:             https://badges.gitter.im/https://github.com/gradhep/relaxed/community.svg
-[gitter-link]:              https://gitter.im/https://github.com/gradhep/relaxed/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-[pypi-link]:                https://pypi.org/project/relaxed/
-[pypi-platforms]:           https://img.shields.io/pypi/pyversions/relaxed
-[pypi-version]:             https://badge.fury.io/py/relaxed.svg
-[rtd-badge]:                https://readthedocs.org/projects/relaxed/badge/?version=latest
-[rtd-link]:                 https://relaxed.readthedocs.io/en/latest/?badge=latest
-[sk-badge]:                 https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
-
+[actions-badge]: https://github.com/gradhep/relaxed/workflows/CI/badge.svg
+[actions-link]: https://github.com/gradhep/relaxed/actions
+[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black-link]: https://github.com/psf/black
+[conda-badge]: https://img.shields.io/conda/vn/conda-forge/relaxed
+[conda-link]: https://github.com/conda-forge/relaxed-feedstock
+[github-discussions-badge]:
+  https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
+[github-discussions-link]: https://github.com/gradhep/relaxed/discussions
+[gitter-badge]: https://badges.gitter.im/https://github.com/gradhep/relaxed/community.svg
+[gitter-link]:
+  https://gitter.im/https://github.com/gradhep/relaxed/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
+[pypi-link]: https://pypi.org/project/relaxed/
+[pypi-platforms]: https://img.shields.io/pypi/pyversions/relaxed
+[pypi-version]: https://badge.fury.io/py/relaxed.svg
+[rtd-badge]: https://readthedocs.org/projects/relaxed/badge/?version=latest
+[rtd-link]: https://relaxed.readthedocs.io/en/latest/?badge=latest
+[sk-badge]: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
 
 Provides differentiable ("relaxed") versions of common operations in high-energy physics.
 
-Based on [`jax`](http://github.com/google/jax). Where possible, function APIs try to mimic their commonly used counterparts, e.g. fitting and hypothesis testing in [`pyhf`](http://github.com/scikit-hep/pyhf).
+Based on [`jax`](http://github.com/google/jax). Where possible, function APIs try to mimic their
+commonly used counterparts, e.g. fitting and hypothesis testing in
+[`pyhf`](http://github.com/scikit-hep/pyhf).
 
 ## Currently implemented:
+
 - **[basic operations](src/relaxed/ops.py)**:
   - `relaxed.hist`: histograms via kernel density estimation (tunable bandwidth).
   - `relaxed.cut`: approximates a hard cut with a sigmoid function (tunable slope).
 - **[fitting routines](src/relaxed/mle.py)**:
   - `relaxed.mle.fit`: global MLE fit.
   - `relaxed.mle.fixed_poi_fit`: constrained fit given a value of a parameter of interest.
 - **[inference](src/relaxed/infer.py)**:
-  - `relaxed.infer.hypotest`: hypothesis test based on the profile likelihood. Supports test statistics for both limit setting (`q`) and discovery (`q_0`).
+  - `relaxed.infer.hypotest`: hypothesis test based on the profile likelihood. Supports test
+    statistics for both limit setting (`q`) and discovery (`q_0`).
   - `relaxed.fisher_info`: the fisher information matrix (of a `pyhf`-type model).
-  - `relaxed.cramer_rao_uncert`: inverts the fisher information matrix to provide uncertainties valid through the [Cramér-Rao bound](https://en.wikipedia.org/wiki/Cram%C3%A9r%E2%80%93Rao_bound).
+  - `relaxed.cramer_rao_uncert`: inverts the fisher information matrix to provide uncertainties
+    valid through the
+    [Cramér-Rao bound](https://en.wikipedia.org/wiki/Cram%C3%A9r%E2%80%93Rao_bound).
 - **[metrics](src/relaxed/metrics.py)**:
-  - `relaxed.metrics.gaussianity`: an experimental metric that quantifies the mean-squared difference of a likelihood function with respect to its gaussian approximation (covariance calculated using the Cramér-Rao bound above).
-  - `relaxed.metrics.asimov_sig`: easy access to the (single- and multi-bin) stat-only expected significance.
-
-We're maintaining a list of desired differentiable operations in [`list_of_operations.md`](list_of_operations.md) (thanks to [@cranmer](http://github.com/cranmer)) -- feel free to take inspiration or contribute with a PR if there's one you can handle :)
+  - `relaxed.metrics.gaussianity`: an experimental metric that quantifies the mean-squared
+    difference of a likelihood function with respect to its gaussian approximation (covariance
+    calculated using the Cramér-Rao bound above).
+  - `relaxed.metrics.asimov_sig`: easy access to the (single- and multi-bin) stat-only expected
+    significance.
+
+We're maintaining a list of desired differentiable operations in
+[`list_of_operations.md`](list_of_operations.md) (thanks to [@cranmer](http://github.com/cranmer))
+-- feel free to take inspiration or contribute with a PR if there's one you can handle :)
 
 ## Install
+
 In your virtual environment:
+
 ```
 python3 -m pip install relaxed
 ```
 
 ## Examples
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gradhep/relaxed/main?labpath=examples%2Fcuts.ipynb) <- Click here to start playing with our examples straight away (thanks to Binder)!
 
-If you'd rather run the example notebooks locally from `examples/`, you can clone the repository, then:
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gradhep/relaxed/main?labpath=examples%2Fcuts.ipynb)
+<- Click here to start playing with our examples straight away (thanks to Binder)!
+
+If you'd rather run the example notebooks locally from `examples/`, you can clone the repository,
+then:
 
 ```
 python3 -m venv venv  # or virtualenv
 source venv/bin/activate
 pip install --upgrade pip setuptools wheel
 pip install relaxed
 cd examples
 pip install -r requirements.txt
 ```
 
-Then launch jupyter through your preferred medium (vscode, jupyterlab, etc.), making sure to use this virtual env as your kernel (e.g. you can `pip` install and run jupyter lab in this env).
+Then launch jupyter through your preferred medium (vscode, jupyterlab, etc.), making sure to use
+this virtual env as your kernel (e.g. you can `pip` install and run jupyter lab in this env).
 
 ## Sharp bits
-For serious use with `pyhf`, e.g. in a [`neos`](http://github.com/gradhep/neos)-type workflow, it is temporarily recommended to install `pyhf` using a specific branch that is designed to be differentiable with respect to model construction:
+
+For serious use with `pyhf`, e.g. in a [`neos`](http://github.com/gradhep/neos)-type workflow, it is
+temporarily recommended to install `pyhf` using a specific branch that is designed to be
+differentiable with respect to model construction:
 
 ```
 python3 -m pip install git+http://github.com/scikit-hep/pyhf.git@make_difffable_model_ctor
 ```
+
 We plan to merge this into `pyhf` when it's stable, and will then drop this instruction :)
 
 ## Cite
-If you use `relaxed`, please cite us! You should be able to do that from the github UI (top-right, under 'cite this repository'), but if not, see our [Zenodo DOI](https://zenodo.org/badge/latestdoi/264991846) or our [`CITATION.cff`](CITATION.cff).
+
+If you use `relaxed`, please cite us! You should be able to do that from the github UI (top-right,
+under 'cite this repository'), but if not, see our
+[Zenodo DOI](https://zenodo.org/badge/latestdoi/264991846) or our [`CITATION.cff`](CITATION.cff).
 
 ## Acknowledgments
-Big thanks to all the developers of the main packages we use (`jax`, `pyhf`, `jaxopt`).
-Thanks also to [@dfm](github.com/user/dfm) for the README header inspiration ;)
+
+Big thanks to all the developers of the main packages we use (`jax`, `pyhf`, `jaxopt`). Thanks also
+to [@dfm](github.com/user/dfm) for the README header inspiration ;)
```

#### html2text {}

```diff
@@ -1,23 +1,34 @@
-Metadata-Version: 2.1 Name: relaxed Version: 0.2.2 Summary: Differentiable
-versions of common operations in high-energy physics. Home-page: https://
-github.com/gradhep/relaxed Author: Nathan Simpson Author-email: n.s@cern.ch
-Maintainer: Nathan Simpson Maintainer-email: n.s@cern.ch License: BSD-3-Clause
-Project-URL: Documentation, https://relaxed.readthedocs.io/ Project-URL: Bug
-Tracker, https://github.com/gradhep/relaxed/issues Project-URL: Discussions,
-https://github.com/gradhep/relaxed/discussions Project-URL: Changelog, https://
-github.com/gradhep/relaxed/releases Platform: Any Classifier: Development
-Status :: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
-BSD License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
-Scientific/Engineering Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: test License-
-File: LICENSE
+Metadata-Version: 2.1 Name: relaxed Version: 0.3.0 Summary: Differentiable
+versions of common HEP operations. Project-URL: Homepage, https://github.com/
+gradhep/relaxed Project-URL: Bug Tracker, https://github.com/gradhep/relaxed/
+issues Project-URL: Discussions, https://github.com/gradhep/relaxed/discussions
+Project-URL: Changelog, https://github.com/gradhep/relaxed/releases Author-
+email: Nathan Simpson
+turing.ac.uk> License-File: LICENSE Classifier: Development Status :: 1 -
+Planning Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Scientific/Engineering Classifier: Typing :: Typed Requires-Python:
+>=3.8 Requires-Dist: equinox Requires-Dist: jaxopt>=0.7 Requires-Dist:
+optax>=0.1.2 Requires-Dist: typing-extensions>=4.6; python_version < '3.11'
+Provides-Extra: dev Requires-Dist: pytest-cov>=3; extra == 'dev' Requires-Dist:
+pytest>=6; extra == 'dev' Provides-Extra: docs Requires-Dist: furo; extra ==
+'docs' Requires-Dist: myst-parser>=0.13; extra == 'docs' Requires-Dist: sphinx-
+autodoc-typehints; extra == 'docs' Requires-Dist: sphinx-book-theme>=0.1.0;
+extra == 'docs' Requires-Dist: sphinx-copybutton; extra == 'docs' Requires-
+Dist: sphinx>=4.0; extra == 'docs' Provides-Extra: test Requires-Dist: iminuit;
+extra == 'test' Requires-Dist: pyhf[jax]>=0.7.0; extra == 'test' Requires-Dist:
+pytest-cov>=3; extra == 'test' Requires-Dist: pytest>=6; extra == 'test'
+Description-Content-Type: text/markdown
                                 [relaxed logo]
 
 [GitHub_Workflow_Status] [Read_the_Docs] [Read_the_Docs] [Zenodo_DOI] [Binder]
 [actions-badge]: https://github.com/gradhep/relaxed/workflows/CI/badge.svg
 [actions-link]: https://github.com/gradhep/relaxed/actions [black-badge]:
 https://img.shields.io/badge/code%20style-black-000000.svg [black-link]: https:
 //github.com/psf/black [conda-badge]: https://img.shields.io/conda/vn/conda-
```

### Comparing `relaxed-0.2.2/README.md` & `relaxed-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,83 +14,108 @@
     <img alt="Zenodo DOI" src="https://zenodo.org/badge/264991846.svg">
   </a>
   <a href="https://mybinder.org/v2/gh/gradhep/relaxed/main?labpath=examples%2Fcuts.ipynb">
     <img alt="Binder" src="https://mybinder.org/badge_logo.svg">
   </a>
 </p>
 
-
-[actions-badge]:            https://github.com/gradhep/relaxed/workflows/CI/badge.svg
-[actions-link]:             https://github.com/gradhep/relaxed/actions
-[black-badge]:              https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]:               https://github.com/psf/black
-[conda-badge]:              https://img.shields.io/conda/vn/conda-forge/relaxed
-[conda-link]:               https://github.com/conda-forge/relaxed-feedstock
-[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
-[github-discussions-link]:  https://github.com/gradhep/relaxed/discussions
-[gitter-badge]:             https://badges.gitter.im/https://github.com/gradhep/relaxed/community.svg
-[gitter-link]:              https://gitter.im/https://github.com/gradhep/relaxed/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-[pypi-link]:                https://pypi.org/project/relaxed/
-[pypi-platforms]:           https://img.shields.io/pypi/pyversions/relaxed
-[pypi-version]:             https://badge.fury.io/py/relaxed.svg
-[rtd-badge]:                https://readthedocs.org/projects/relaxed/badge/?version=latest
-[rtd-link]:                 https://relaxed.readthedocs.io/en/latest/?badge=latest
-[sk-badge]:                 https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
-
+[actions-badge]: https://github.com/gradhep/relaxed/workflows/CI/badge.svg
+[actions-link]: https://github.com/gradhep/relaxed/actions
+[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black-link]: https://github.com/psf/black
+[conda-badge]: https://img.shields.io/conda/vn/conda-forge/relaxed
+[conda-link]: https://github.com/conda-forge/relaxed-feedstock
+[github-discussions-badge]:
+  https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
+[github-discussions-link]: https://github.com/gradhep/relaxed/discussions
+[gitter-badge]: https://badges.gitter.im/https://github.com/gradhep/relaxed/community.svg
+[gitter-link]:
+  https://gitter.im/https://github.com/gradhep/relaxed/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
+[pypi-link]: https://pypi.org/project/relaxed/
+[pypi-platforms]: https://img.shields.io/pypi/pyversions/relaxed
+[pypi-version]: https://badge.fury.io/py/relaxed.svg
+[rtd-badge]: https://readthedocs.org/projects/relaxed/badge/?version=latest
+[rtd-link]: https://relaxed.readthedocs.io/en/latest/?badge=latest
+[sk-badge]: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
 
 Provides differentiable ("relaxed") versions of common operations in high-energy physics.
 
-Based on [`jax`](http://github.com/google/jax). Where possible, function APIs try to mimic their commonly used counterparts, e.g. fitting and hypothesis testing in [`pyhf`](http://github.com/scikit-hep/pyhf).
+Based on [`jax`](http://github.com/google/jax). Where possible, function APIs try to mimic their
+commonly used counterparts, e.g. fitting and hypothesis testing in
+[`pyhf`](http://github.com/scikit-hep/pyhf).
 
 ## Currently implemented:
+
 - **[basic operations](src/relaxed/ops.py)**:
   - `relaxed.hist`: histograms via kernel density estimation (tunable bandwidth).
   - `relaxed.cut`: approximates a hard cut with a sigmoid function (tunable slope).
 - **[fitting routines](src/relaxed/mle.py)**:
   - `relaxed.mle.fit`: global MLE fit.
   - `relaxed.mle.fixed_poi_fit`: constrained fit given a value of a parameter of interest.
 - **[inference](src/relaxed/infer.py)**:
-  - `relaxed.infer.hypotest`: hypothesis test based on the profile likelihood. Supports test statistics for both limit setting (`q`) and discovery (`q_0`).
+  - `relaxed.infer.hypotest`: hypothesis test based on the profile likelihood. Supports test
+    statistics for both limit setting (`q`) and discovery (`q_0`).
   - `relaxed.fisher_info`: the fisher information matrix (of a `pyhf`-type model).
-  - `relaxed.cramer_rao_uncert`: inverts the fisher information matrix to provide uncertainties valid through the [Cramér-Rao bound](https://en.wikipedia.org/wiki/Cram%C3%A9r%E2%80%93Rao_bound).
+  - `relaxed.cramer_rao_uncert`: inverts the fisher information matrix to provide uncertainties
+    valid through the
+    [Cramér-Rao bound](https://en.wikipedia.org/wiki/Cram%C3%A9r%E2%80%93Rao_bound).
 - **[metrics](src/relaxed/metrics.py)**:
-  - `relaxed.metrics.gaussianity`: an experimental metric that quantifies the mean-squared difference of a likelihood function with respect to its gaussian approximation (covariance calculated using the Cramér-Rao bound above).
-  - `relaxed.metrics.asimov_sig`: easy access to the (single- and multi-bin) stat-only expected significance.
-
-We're maintaining a list of desired differentiable operations in [`list_of_operations.md`](list_of_operations.md) (thanks to [@cranmer](http://github.com/cranmer)) -- feel free to take inspiration or contribute with a PR if there's one you can handle :)
+  - `relaxed.metrics.gaussianity`: an experimental metric that quantifies the mean-squared
+    difference of a likelihood function with respect to its gaussian approximation (covariance
+    calculated using the Cramér-Rao bound above).
+  - `relaxed.metrics.asimov_sig`: easy access to the (single- and multi-bin) stat-only expected
+    significance.
+
+We're maintaining a list of desired differentiable operations in
+[`list_of_operations.md`](list_of_operations.md) (thanks to [@cranmer](http://github.com/cranmer))
+-- feel free to take inspiration or contribute with a PR if there's one you can handle :)
 
 ## Install
+
 In your virtual environment:
+
 ```
 python3 -m pip install relaxed
 ```
 
 ## Examples
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gradhep/relaxed/main?labpath=examples%2Fcuts.ipynb) <- Click here to start playing with our examples straight away (thanks to Binder)!
 
-If you'd rather run the example notebooks locally from `examples/`, you can clone the repository, then:
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gradhep/relaxed/main?labpath=examples%2Fcuts.ipynb)
+<- Click here to start playing with our examples straight away (thanks to Binder)!
+
+If you'd rather run the example notebooks locally from `examples/`, you can clone the repository,
+then:
 
 ```
 python3 -m venv venv  # or virtualenv
 source venv/bin/activate
 pip install --upgrade pip setuptools wheel
 pip install relaxed
 cd examples
 pip install -r requirements.txt
 ```
 
-Then launch jupyter through your preferred medium (vscode, jupyterlab, etc.), making sure to use this virtual env as your kernel (e.g. you can `pip` install and run jupyter lab in this env).
+Then launch jupyter through your preferred medium (vscode, jupyterlab, etc.), making sure to use
+this virtual env as your kernel (e.g. you can `pip` install and run jupyter lab in this env).
 
 ## Sharp bits
-For serious use with `pyhf`, e.g. in a [`neos`](http://github.com/gradhep/neos)-type workflow, it is temporarily recommended to install `pyhf` using a specific branch that is designed to be differentiable with respect to model construction:
+
+For serious use with `pyhf`, e.g. in a [`neos`](http://github.com/gradhep/neos)-type workflow, it is
+temporarily recommended to install `pyhf` using a specific branch that is designed to be
+differentiable with respect to model construction:
 
 ```
 python3 -m pip install git+http://github.com/scikit-hep/pyhf.git@make_difffable_model_ctor
 ```
+
 We plan to merge this into `pyhf` when it's stable, and will then drop this instruction :)
 
 ## Cite
-If you use `relaxed`, please cite us! You should be able to do that from the github UI (top-right, under 'cite this repository'), but if not, see our [Zenodo DOI](https://zenodo.org/badge/latestdoi/264991846) or our [`CITATION.cff`](CITATION.cff).
+
+If you use `relaxed`, please cite us! You should be able to do that from the github UI (top-right,
+under 'cite this repository'), but if not, see our
+[Zenodo DOI](https://zenodo.org/badge/latestdoi/264991846) or our [`CITATION.cff`](CITATION.cff).
 
 ## Acknowledgments
-Big thanks to all the developers of the main packages we use (`jax`, `pyhf`, `jaxopt`).
-Thanks also to [@dfm](github.com/user/dfm) for the README header inspiration ;)
+
+Big thanks to all the developers of the main packages we use (`jax`, `pyhf`, `jaxopt`). Thanks also
+to [@dfm](github.com/user/dfm) for the README header inspiration ;)
```

### Comparing `relaxed-0.2.2/list_of_operations.md` & `relaxed-0.3.0/list_of_operations.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,104 @@
 # List of differentiable operations
 
-
 ## Definitely useful with known solution
 
-* **Classification (binning)**:
-Assigning an event to a bin in a histogram or classifying it as a particular class label is a non-differentiable operation. Multi-class classification is a classic example in machine learning and statistics, and is typically relaxed with a sigmoid or a softmax.
-  * This was used in INFERNO and neos
-  * Alternatively, one could calculate smooth probability assignments using Kernel Density Estimation or some other kernel based approach
-
-* **Differentiable ranking and sorting**:
-Sorting is a fundamental operation. For instance, we typically sort particles by $p_T$.
-
-  * Differentiable Ranks and Sorting using Optimal Transport [https://arxiv.org/abs/1905.11885](https://arxiv.org/abs/1905.11885)
-  *  O(nlogn) time and O(n) space complexity [https://arxiv.org/abs/2002.08871](https://arxiv.org/abs/2002.08871) and [great slides](https://raw.githubusercontent.com/mblondel/mblondel.github.io/9e103aad534d3e2d51a357c72b2485309131e719/talks/mblondel-CIRM-2020-03.pdf)
-
-
-* **Differentiable clustering (partitions)**
-We have a set of objects and we would like to cluster or partition them. We can think of this in terms of graph where the nodes are the objects and edges indicate two objects are in the same cluster. We want all objects in the same cluster to be connected and no objects in different clusters to be connected.
-
-  * This can be imposed if the adjacency matrix is restricted to be of the form $u u^T$, where $u$ is a softmax output. This was used in [Set2Graph: Learning Graphs From Sets](https://arxiv.org/abs/2002.08772) for vertexing and is also described in slide 27 of [this talk](https://indico.cern.ch/event/809820/contributions/3632659/attachments/1971659/3280030/GNN_NYU_3_Jan_2020.pdf).
-  * note: one might think of using something like this for clustering calorimeter cells to calorimeter clusters.
-
-* **Barlow-Beeston for Monte Carlo Statistical Uncertainty:**
-The statistical uncertainty on template histograms from limited statistical uncertainty can be dealth with in a clean way by jointly modelling the statistical fluctuations in the data and the statistical fluctuations in the Monte Carlo samples. This was treated in [Fitting using finite Monte Carlo samples](https://doi.org/10.1016/0010-4655(93)90005-W) (pdf from [at FermiLab](https://lss.fnal.gov/archive/other/man-hep-93-1.pdf)). In a simple one-bin example one would model as $P(n,m|\mu,\lambda) = Pois(n|\mu+\lambda)Pois(m|\tau\lambda)$ where $n$ is count in data in a signal region, $\mu$ is the unknown exepected signal rate, $\lambda$ is the unknown expected background rate (a nuisance parameter), $\tau$ is the ratio of the Monte Carlo luminosity to data luminosity, and $m$ is the count in the Monte Carlo sample. This can easily be extended to multiple bins and multiple background sources per bin, but it introduces a nuisance parameter for each component of each bin. Note in this setup the observed Monte Carlo are treated as data (since it fluctuates and is on the left of the "|"). In HistFactory language, the Monte Carlo observation $m$ would be the `Data` of a new `Channel` and the unknown background $\tau\lambda$ would be modeled with a `ShapeFactor` that would be shared with the `Channel` that has the real observed data $n$. This is typically very heavy and leads to a proliferation of nuisance parameters, which cause problems for Minuit. Thus, typically an approximate approach is used where the different background contributions are combined. In HistFactory this is what is done when using `StatErrorConfig`. This treatment is usually fine, but has corner cases when $m=0$. One interesting aspect of the Barlow-Beeston approach is that optimization on the nuisance parameter $\lambda$ decouples from optimization on $\mu$. In fact, there is a closed form solution for $\hat{\lambda}(n,m,\mu)$ (eq. 14), so optimizing the full likelihood can be thought of as a nested optimization with $\lambda$ in the inner loop. Moreover, it can be thought of as the implicit minimization used for the profile likelihood fit in neos. Several years ago George Lewis wrote a wrapper for the log-likeihood created in HistFactory so that $\lambda$ was solved exactly and only the profiled likelihood with $\mu$ was exposed to Minuit. While elegant conceptually, the implementation in RooFit did not lead to significant performance gains for the number of nuisance parameters in the models at that time. However, it would be interesting to revisit this in the context of pyhf and grad-hep. References:
-
-  * [RooBarlowBeestonLL.cxx](https://root.cern/doc/master/RooBarlowBeestonLL_8cxx_source.html) [RooBarlowBeestonLL.h](https://root.cern/doc/master/RooBarlowBeestonLL_8h_source.html)
-  * [A RooFit example](https://root.cern/doc/master/rf709__BarlowBeeston_8C.html)
-
-* **ROC AUC:**
-While the area under ROC curve (ROC AUC) is not usually our ultimate physics goal, it may be useful or motivated in some cases. The ROC curve is non-differentiable, but can be relaxed into a rank statistic. This was used for example in [Backdrop: Stochastic Backpropagation](https://arxiv.org/abs/1806.01337)
- * Herschtal, A. and Raskutti, B. (2004). Optimising area under the roc curve using gradient descent. In Proceedings of the Twenty-first International Conference on Machine Learning, ICML ’04, pages 49–, New York, NY, USA. ACM. [doi/10.1145/1015330.1015366](https://dl.acm.org/doi/10.1145/1015330.1015366)
+- **Classification (binning)**: Assigning an event to a bin in a histogram or classifying it as a
+  particular class label is a non-differentiable operation. Multi-class classification is a classic
+  example in machine learning and statistics, and is typically relaxed with a sigmoid or a softmax.
+
+  - This was used in INFERNO and neos
+  - Alternatively, one could calculate smooth probability assignments using Kernel Density
+    Estimation or some other kernel based approach
+
+- **Differentiable ranking and sorting**: Sorting is a fundamental operation. For instance, we
+  typically sort particles by $p_T$.
+
+  - Differentiable Ranks and Sorting using Optimal Transport
+    [https://arxiv.org/abs/1905.11885](https://arxiv.org/abs/1905.11885)
+  - O(nlogn) time and O(n) space complexity
+    [https://arxiv.org/abs/2002.08871](https://arxiv.org/abs/2002.08871) and
+    [great slides](https://raw.githubusercontent.com/mblondel/mblondel.github.io/9e103aad534d3e2d51a357c72b2485309131e719/talks/mblondel-CIRM-2020-03.pdf)
+
+- **Differentiable clustering (partitions)** We have a set of objects and we would like to cluster
+  or partition them. We can think of this in terms of graph where the nodes are the objects and
+  edges indicate two objects are in the same cluster. We want all objects in the same cluster to be
+  connected and no objects in different clusters to be connected.
+
+  - This can be imposed if the adjacency matrix is restricted to be of the form $u u^T$, where $u$
+    is a softmax output. This was used in
+    [Set2Graph: Learning Graphs From Sets](https://arxiv.org/abs/2002.08772) for vertexing and is
+    also described in slide 27 of
+    [this talk](https://indico.cern.ch/event/809820/contributions/3632659/attachments/1971659/3280030/GNN_NYU_3_Jan_2020.pdf).
+  - note: one might think of using something like this for clustering calorimeter cells to
+    calorimeter clusters.
+
+- **Barlow-Beeston for Monte Carlo Statistical Uncertainty:** The statistical uncertainty on
+  template histograms from limited statistical uncertainty can be dealth with in a clean way by
+  jointly modelling the statistical fluctuations in the data and the statistical fluctuations in the
+  Monte Carlo samples. This was treated in
+  [Fitting using finite Monte Carlo samples](<https://doi.org/10.1016/0010-4655(93)90005-W>) (pdf
+  from [at FermiLab](https://lss.fnal.gov/archive/other/man-hep-93-1.pdf)). In a simple one-bin
+  example one would model as $P(n,m|\mu,\lambda) = Pois(n|\mu+\lambda)Pois(m|\tau\lambda)$ where $n$
+  is count in data in a signal region, $\mu$ is the unknown exepected signal rate, $\lambda$ is the
+  unknown expected background rate (a nuisance parameter), $\tau$ is the ratio of the Monte Carlo
+  luminosity to data luminosity, and $m$ is the count in the Monte Carlo sample. This can easily be
+  extended to multiple bins and multiple background sources per bin, but it introduces a nuisance
+  parameter for each component of each bin. Note in this setup the observed Monte Carlo are treated
+  as data (since it fluctuates and is on the left of the "|"). In HistFactory language, the Monte
+  Carlo observation $m$ would be the `Data` of a new `Channel` and the unknown background
+  $\tau\lambda$ would be modeled with a `ShapeFactor` that would be shared with the `Channel` that
+  has the real observed data $n$. This is typically very heavy and leads to a proliferation of
+  nuisance parameters, which cause problems for Minuit. Thus, typically an approximate approach is
+  used where the different background contributions are combined. In HistFactory this is what is
+  done when using `StatErrorConfig`. This treatment is usually fine, but has corner cases when
+  $m=0$. One interesting aspect of the Barlow-Beeston approach is that optimization on the nuisance
+  parameter $\lambda$ decouples from optimization on $\mu$. In fact, there is a closed form solution
+  for $\hat{\lambda}(n,m,\mu)$ (eq. 14), so optimizing the full likelihood can be thought of as a
+  nested optimization with $\lambda$ in the inner loop. Moreover, it can be thought of as the
+  implicit minimization used for the profile likelihood fit in neos. Several years ago George Lewis
+  wrote a wrapper for the log-likeihood created in HistFactory so that $\lambda$ was solved exactly
+  and only the profiled likelihood with $\mu$ was exposed to Minuit. While elegant conceptually, the
+  implementation in RooFit did not lead to significant performance gains for the number of nuisance
+  parameters in the models at that time. However, it would be interesting to revisit this in the
+  context of pyhf and grad-hep. References:
+
+  - [RooBarlowBeestonLL.cxx](https://root.cern/doc/master/RooBarlowBeestonLL_8cxx_source.html)
+    [RooBarlowBeestonLL.h](https://root.cern/doc/master/RooBarlowBeestonLL_8h_source.html)
+  - [A RooFit example](https://root.cern/doc/master/rf709__BarlowBeeston_8C.html)
+
+- **ROC AUC:** While the area under ROC curve (ROC AUC) is not usually our ultimate physics goal, it
+  may be useful or motivated in some cases. The ROC curve is non-differentiable, but can be relaxed
+  into a rank statistic. This was used for example in
+  [Backdrop: Stochastic Backpropagation](https://arxiv.org/abs/1806.01337)
+- Herschtal, A. and Raskutti, B. (2004). Optimising area under the roc curve using gradient descent.
+  In Proceedings of the Twenty-first International Conference on Machine Learning, ICML ’04, pages
+  49–, New York, NY, USA. ACM.
+  [doi/10.1145/1015330.1015366](https://dl.acm.org/doi/10.1145/1015330.1015366)
 
 ## Definitely useful seeking solution
 
-* **Differentiable legend placement in plots:**
-They are so annoying aren't they?
+- **Differentiable legend placement in plots:** They are so annoying aren't they?
 
-* **Differentiable peer review:**
-accept/reject is so non-diffable
+- **Differentiable peer review:** accept/reject is so non-diffable
 
 ## Potentially useful
 
-* **Differentiable Feature Selection by Discrete Relaxation**
- See [paper](https://www.microsoft.com/en-us/research/publication/differentiable-feature-selection-by-discrete-relaxation/)
-
-* **Gumbel Max Trick & Gumbel Machinery:**
-The Gumbel-Max Trick is a method to sample from a categorical distribution $Cat(\alpha_1, \dots, \alpha_K)$, where category $k$ has $\alpha_k$
-probability to be sampled among $K$ categories, and relies on the Gumbel distribution defined by the Cumulative Distribution Function.
-
-  * [Gumbel Max Trick](https://laurent-dinh.github.io/2016/11/22/gumbel-max.html)
-  * [Gumbel Machinery](https://cmaddis.github.io/gumbel-machinery)
-
- * **Sparse Structured Prediction:**
-  See paper [Differentiable Relaxed Optimization for Sparse Structured Prediction](https://arxiv.org/abs/2001.04437)
+- **Differentiable Feature Selection by Discrete Relaxation** See
+  [paper](https://www.microsoft.com/en-us/research/publication/differentiable-feature-selection-by-discrete-relaxation/)
 
-*  **Coreference resolution**:
-"Coreference resolution is the task of identifying all mentions which refer to the same entity in a document." "Coreference resolution can be regarded as a clustering problem: each cluster corresponds to a single entity and consists of all its mentions in a given text." From Optimizing Differentiable Relaxations of Coreference Evaluation Metrics [https://arxiv.org/abs/1704.04451](https://arxiv.org/abs/1704.04451)
+- **Gumbel Max Trick & Gumbel Machinery:** The Gumbel-Max Trick is a method to sample from a
+  categorical distribution $Cat(\alpha_1, \dots, \alpha_K)$, where category $k$ has $\alpha_k$
+  probability to be sampled among $K$ categories, and relies on the Gumbel distribution defined by
+  the Cumulative Distribution Function.
+
+  - [Gumbel Max Trick](https://laurent-dinh.github.io/2016/11/22/gumbel-max.html)
+  - [Gumbel Machinery](https://cmaddis.github.io/gumbel-machinery)
+
+- **Sparse Structured Prediction:** See paper
+  [Differentiable Relaxed Optimization for Sparse Structured Prediction](https://arxiv.org/abs/2001.04437)
+
+- **Coreference resolution**: "Coreference resolution is the task of identifying all mentions which
+  refer to the same entity in a document." "Coreference resolution can be regarded as a clustering
+  problem: each cluster corresponds to a single entity and consists of all its mentions in a given
+  text." From Optimizing Differentiable Relaxations of Coreference Evaluation Metrics
+  [https://arxiv.org/abs/1704.04451](https://arxiv.org/abs/1704.04451)
```

### Comparing `relaxed-0.2.2/relaxed-logo.png` & `relaxed-0.3.0/relaxed-logo.png`

 * *Files identical despite different names*

### Comparing `relaxed-0.2.2/src/relaxed/dummy_pyhf.py` & `relaxed-0.3.0/tests/dummy_pyhf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 from __future__ import annotations
 
 __all__ = ("example_model", "uncorrelated_background")
 
 from typing import Any, Iterable
 
+import jax
 import jax.numpy as jnp
 import pyhf
+from equinox import Module as PyTree
 
 
-# class-based
-class _Config:
-    def __init__(self) -> None:
+class _Config(PyTree):
+    poi_index: int
+    npars: int
+    auxdata: jax.Array
+
+    def __init__(self, aux) -> None:
         self.poi_index = 0
         self.npars = 2
+        self.auxdata = aux
 
-    def suggested_init(self) -> jnp.ndarray:
+    def suggested_init(self) -> jax.Array:
         return jnp.asarray([1.0, 1.0])
 
+    def suggested_bounds(self) -> tuple[jax.Array, jax.Array]:
+        return jnp.asarray([[0.0, 0.0], [10.0, 10.0]])
+
 
-class Model:
+class Model(PyTree):
     """Dummy class to mimic the functionality of `pyhf.Model`."""
 
+    sig: jax.Array
+    nominal: jax.Array
+    uncert: jax.Array
+    factor: jax.Array
+    config: _Config
+
     def __init__(self, spec: Iterable[Any]) -> None:
-        pyhf.set_backend("jax")
         self.sig, self.nominal, self.uncert = spec
         self.factor = (self.nominal / self.uncert) ** 2
-        self.aux = 1.0 * self.factor
-        self.config = _Config()
+        self.config = _Config(1.0 * self.factor)
 
-    def expected_data(self, pars: jnp.ndarray) -> jnp.ndarray:
+    def expected_data(self, pars: jax.Array) -> jax.Array:
         mu, gamma = pars
         expected_main = jnp.asarray([gamma * self.nominal + mu * self.sig])
-        aux_data = jnp.asarray([self.aux])
-        return jnp.concatenate([expected_main, aux_data])
+        return jnp.concatenate([expected_main, jnp.array([self.config.auxdata])])
 
-    def logpdf(self, pars: jnp.ndarray, data: jnp.ndarray) -> jnp.ndarray:
+    # logpdf as the call method
+    def logpdf(self, pars: jax.Array, data: jax.Array) -> jax.Array:
         maindata, auxdata = data
         main, _ = self.expected_data(pars)
         _, gamma = pars
         main = pyhf.probability.Poisson(main).log_prob(maindata)
         constraint = pyhf.probability.Poisson(gamma * self.factor).log_prob(auxdata)
         # sum log probs over bins
         return [jnp.sum(jnp.asarray([main + constraint]), axis=None)]
 
 
-def uncorrelated_background(s: jnp.ndarray, b: jnp.ndarray, db: jnp.ndarray) -> Model:
+def uncorrelated_background(s: jax.Array, b: jax.Array, db: jax.Array) -> Model:
     """Dummy class to mimic the functionality of `pyhf.simplemodels.hepdata_like`."""
     return Model([s, b, db])
 
 
 def _calc_yields(x: jnp.ndarray) -> tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]:
     s = 15 + x
     b = 45 - 2 * x
@@ -63,9 +76,8 @@
 
     model = uncorrelated_background(
         jnp.asarray([s]), jnp.asarray([b]), jnp.asarray([db])
     )
 
     if return_yields:
         return model, yields
-    else:
-        return model
+    return model
```

### Comparing `relaxed-0.2.2/src/relaxed/infer.py` & `relaxed-0.3.0/src/relaxed/infer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Calculate expected CLs values with hypothesis tests."""
 from __future__ import annotations
 
 __all__ = ("hypotest",)
 
 import logging
-from functools import partial
+from typing import Any
 
 import jax.numpy as jnp
 import pyhf
-from jax import jit
+from equinox import filter_jit
+from jax import Array
 
-from relaxed._types import Array
 from relaxed.mle import fit, fixed_poi_fit
 
+PyTree = Any
 
+
+@filter_jit
 def hypotest(
     test_poi: float,
     data: Array,
-    model: pyhf.Model,
-    lr: float,
+    model: PyTree,
     return_mle_pars: bool = False,
     test_stat: str = "q",
     expected_pars: Array | None = None,
     cls_method: bool = True,
 ) -> tuple[Array, Array] | Array:
     """Calculate expected CLs/p-values via hypothesis tests.
 
@@ -51,46 +53,44 @@
     Array
         The expected CLs/p-value.
     Array
         The MLE parameters, if `return_mle_pars` is True.
     """
     if test_stat == "q":
         return qmu_test(
-            test_poi, data, model, lr, return_mle_pars, expected_pars, cls_method
+            test_poi, data, model, return_mle_pars, expected_pars, cls_method
         )
-    elif test_stat == "q0":
+    if test_stat == "q0":
         logging.info(
             "test_poi automatically set to 0 for q0 test (bkg-only null hypothesis)"
         )
-        return q0_test(0.0, data, model, lr, return_mle_pars, expected_pars)
-    else:
-        raise ValueError(f"Unknown test statistic: {test_stat}")
+        return q0_test(0.0, data, model, return_mle_pars, expected_pars)
+
+    msg = f"Unknown test statistic: {test_stat}"
+    raise ValueError(msg)
 
 
-@partial(
-    jit, static_argnames=["model", "return_mle_pars", "cls_method"]
-)  # can remove model eventually
+@filter_jit
 def qmu_test(
     test_poi: float,
     data: Array,
-    model: pyhf.Model,
-    lr: float,
+    model: PyTree,
     return_mle_pars: bool = False,
     expected_pars: Array | None = None,
     cls_method: bool = True,
 ) -> tuple[Array, Array] | Array:
     # hard-code 1 as inits for now
     # TODO: need to parse different inits for constrained and global fits
     # because init_pars[0] is not necessarily the poi init
     init_pars = jnp.asarray(model.config.suggested_init())
     conditional_pars = fixed_poi_fit(
-        data, model, poi_condition=test_poi, init_pars=init_pars[:-1], lr=lr
+        data, model, poi_condition=test_poi, init_pars=init_pars[:-1]
     )
     if expected_pars is None:
-        mle_pars = fit(data, model, init_pars=init_pars, lr=lr)
+        mle_pars = fit(data, model, init_pars=init_pars)
     else:
         mle_pars = expected_pars
     profile_likelihood = -2 * (
         model.logpdf(conditional_pars, data)[0] - model.logpdf(mle_pars, data)[0]
     )
 
     poi_hat = mle_pars[model.config.poi_index]
@@ -102,34 +102,34 @@
         CLb = 1 - pyhf.tensorlib.normal_cdf(altval)
         CLs = CLsb / CLb
     else:
         CLs = CLsb
     return (CLs, mle_pars) if return_mle_pars else CLs
 
 
-@partial(
-    jit, static_argnames=["model", "return_mle_pars"]
-)  # can remove model eventually
+@filter_jit
 def q0_test(
     test_poi: float,
     data: Array,
-    model: pyhf.Model,
-    lr: float,
+    model: PyTree,
     return_mle_pars: bool = False,
     expected_pars: Array | None = None,
 ) -> tuple[Array, Array] | Array:
     # hard-code 1 as inits for now
     # TODO: need to parse different inits for constrained and global fits
     # because init_pars[0] is not necessarily the poi init
     init_pars = jnp.asarray(model.config.suggested_init())
     conditional_pars = fixed_poi_fit(
-        data, model, poi_condition=test_poi, init_pars=init_pars[:-1], lr=lr
+        data,
+        model,
+        poi_condition=test_poi,
+        init_pars=init_pars[:-1],
     )
     if expected_pars is None:
-        mle_pars = fit(data, model, init_pars=init_pars, lr=lr)
+        mle_pars = fit(data, model, init_pars=init_pars)
     else:
         mle_pars = expected_pars
     profile_likelihood = -2 * (
         model.logpdf(conditional_pars, data)[0] - model.logpdf(mle_pars, data)[0]
     )
 
     poi_hat = mle_pars[model.config.poi_index]
```

### Comparing `relaxed-0.2.2/src/relaxed/metrics.py` & `relaxed-0.3.0/src/relaxed/metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 __all__ = ("asimov_sig", "gaussianity")
 
 from functools import partial
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING, Any, cast
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
-from jax.random import PRNGKey, multivariate_normal
+from jax import Array
+from jax.random import multivariate_normal
 
-from relaxed._types import Array
 from relaxed.ops import fisher_info
 
 if TYPE_CHECKING:
-    import pyhf
+    PyTree = Any
 
 
 @jax.jit
 def asimov_sig(s: Array, b: Array) -> float:
     """Median expected significance for a counting experiment, valid in the asymptotic regime.
     Also valid for the multi-bin case.
 
@@ -39,25 +39,32 @@
 
 
 def _gaussian_logpdf(
     bestfit_pars: Array,
     data: Array,
     cov: Array,
 ) -> Array:
-    return jsp.stats.multivariate_normal.logpdf(data, bestfit_pars, cov).reshape(
+    return cast(
+        Array, jsp.stats.multivariate_normal.logpdf(data, bestfit_pars, cov)
+    ).reshape(
         1,
     )
 
 
-@partial(jax.jit, static_argnames=["model", "n_samples"])
+@partial(
+    jax.jit,
+    static_argnames=[
+        "n_samples",
+    ],
+)
 def gaussianity(
-    model: pyhf.Model,
+    model: PyTree,
     bestfit_pars: Array,
     data: Array,
-    rng_key: PRNGKey,
+    rng_key: Any,
     n_samples: int = 1000,
 ) -> Array:
     # - compare the likelihood of the fitted model with a gaussian approximation
     # that has the same MLE (fitted_pars)
     # - do this across a number of points in parspace (sampled from the gaussian approx)
     # and take the mean squared diff
     # - centre the values wrt the best-fit vals to scale the differences
```

### Comparing `relaxed-0.2.2/src/relaxed/ops.py` & `relaxed-0.3.0/src/relaxed/ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 from functools import partial
 from typing import Any
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
-
-from relaxed._types import Array
+from jax import Array
 
 
 @partial(jax.jit, static_argnames=["keep"])
 def cut(data: Array, cut_val: float, slope: float = 1.0, keep: str = "above") -> Array:
     """Use a sigmoid function as an approximate cut. Same as a hard cut in the limit of infinite slope.
     Note: this function returns weights, not indices.
 
@@ -33,18 +32,18 @@
     Returns
     -------
     Array
         Weighted yields of the data after the cut.
     """
     if keep == "above":
         return 1 / (1 + jnp.exp(-slope * (data - cut_val)))
-    elif keep == "below":
+    if keep == "below":
         return 1 / (1 + jnp.exp(slope * (data - cut_val)))
-    else:
-        raise ValueError(f"keep must be one of 'above' or 'below', not {keep}")
+    msg = f"keep must be one of 'above' or 'below', not {keep}"
+    raise ValueError(msg)
 
 
 @partial(jax.jit, static_argnames=["density", "reflect_infinities"])
 def hist(
     data: Array,
     bins: Array,
     bandwidth: float,  # | None = None,
@@ -90,15 +89,15 @@
             + jnp.array([counts[0]] + [0] * (len(counts) - 3))
             + jnp.array([0] * (len(counts) - 3) + [counts[-1]])
         )
 
     return counts
 
 
-@partial(jax.jit, static_argnames=["model"])
+@jax.jit
 def fisher_info(model: Any, pars: Array, data: Array) -> Array:
     """Fisher information matrix for a model with a logpdf method.
 
     Parameters
     ----------
     model : Any
         The model to compute the Fisher information matrix for.
@@ -112,15 +111,15 @@
     -------
     Array
         Fisher information matrix.
     """
     return jnp.linalg.inv(-jax.hessian(lambda p, d: model.logpdf(p, d)[0])(pars, data))
 
 
-@partial(jax.jit, static_argnames=["model"])
+@jax.jit
 def cramer_rao_uncert(model: Any, pars: Array, data: Array) -> Array:
     """Approximate uncertainties on MLE parameters for a model with a logpdf method.
     Defined as the square root of the diagonal of the Fisher information matrix, valid
     via the Cramer-Rao lower bound.
 
     Parameters
     ----------
```

### Comparing `relaxed-0.2.2/tests/test_fit.py` & `relaxed-0.3.0/tests/test_fit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,86 @@
+from __future__ import annotations
+
 import jax.numpy as jnp
 import numpy as np
 import pyhf
 import pytest
+from dummy_pyhf import example_model, uncorrelated_background
 from jax import jacrev
 
 import relaxed
-from relaxed.dummy_pyhf import example_model, uncorrelated_background
 
 
 @pytest.mark.parametrize("phi", np.linspace(0.0, 10.0, 5))
 def test_fit(phi):
+    pyhf.set_backend("jax")
     analytic_pars = jnp.array([0.0, 1.0])
     model = example_model(phi)
     mle_pars = relaxed.mle.fit(
         model=model,
         data=model.expected_data(analytic_pars),
         init_pars=model.config.suggested_init(),
-        lr=1e-3,
+        bounds=model.config.suggested_bounds(),
     )
     assert np.allclose(mle_pars, analytic_pars, atol=0.05)
 
 
 def test_fit_grad():
+    pyhf.set_backend("jax")
+
     def pipeline(x):
-        model = uncorrelated_background(x * 5.0, x * 20, x * 2)
-        mle_pars = relaxed.mle.fit(
+        analytic_pars = jnp.array([0.0, 1.0])
+        model = example_model(x)
+        return relaxed.mle.fit(
             model=model,
-            data=model.expected_data(jnp.array([0.0, 1.0])),
+            data=model.expected_data(analytic_pars),
             init_pars=model.config.suggested_init(),
-            lr=1e-2,
+            bounds=model.config.suggested_bounds(),
         )
-        return mle_pars
 
     jacrev(pipeline)(jnp.asarray(0.5))
 
 
 @pytest.mark.parametrize("phi", np.linspace(0.0, 10.0, 5))
 def test_fixed_poi_fit(phi):
     pyhf.set_backend("jax")
     analytic_pars = jnp.array([0.0, 1.0])
 
     model, yields = example_model(phi, return_yields=True)
     init = np.asarray(model.config.suggested_init())
     init = jnp.asarray(np.delete(init, model.config.poi_index))
+    lower, upper = model.config.suggested_bounds()
     relaxed_mle = relaxed.mle.fixed_poi_fit(
         model=model,
         data=model.expected_data(analytic_pars),
         init_pars=init,
-        lr=1e-2,
         poi_condition=1.0,
+        bounds=(lower[1:], upper[1:]),
     )
 
     m = pyhf.simplemodels.uncorrelated_background(*yields)
 
     pyhf_mle = pyhf.infer.mle.fixed_poi_fit(
         1.0,
         m.expected_data(analytic_pars),
         m,
     )
 
     assert np.allclose(relaxed_mle, pyhf_mle, atol=0.05)
 
 
 def test_fixed_poi_fit_grad():
+    pyhf.set_backend("jax")
+
     def pipeline(x):
         model = uncorrelated_background(x * 5.0, x * 20, x * 2)
-        mle_pars = relaxed.mle.fixed_poi_fit(
+        lower, upper = model.config.suggested_bounds()
+
+        return relaxed.mle.fixed_poi_fit(
             model=model,
             data=model.expected_data(jnp.array([0.0, 1.0])),
             init_pars=model.config.suggested_init()[1:],
-            lr=1e-2,
             poi_condition=1.0,
+            bounds=(lower[1:], upper[1:]),
         )
-        return mle_pars
 
     jacrev(pipeline)(jnp.asarray(0.5))
```

### Comparing `relaxed-0.2.2/tests/test_infer.py` & `relaxed-0.3.0/tests/test_infer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,122 +1,115 @@
+from __future__ import annotations
+
+import jax
 import jax.numpy as jnp
 import numpy as np
 import pyhf
 import pytest
+from dummy_pyhf import example_model, uncorrelated_background
 from jax import jacrev
 
 import relaxed
-from relaxed.dummy_pyhf import example_model, uncorrelated_background
+
+jax.config.update("jax_enable_x64", True)
 
 
 @pytest.mark.parametrize("test_stat", ["q", "q0"])
 @pytest.mark.parametrize("phi", np.linspace(0.0, 10.0, 5))
 def test_hypotest_validity(phi, test_stat):
     pyhf.set_backend("jax")
     if test_stat == "q":
         analytic_pars = jnp.array([0.0, 1.0])  # bkg-only hypothesis
     elif test_stat == "q0":
         analytic_pars = jnp.array([1.0, 1.0])  # nominal sig+bkg hypothesis
     else:
-        raise ValueError(f"Unknown test statistic: {test_stat}")
+        msg = f"Unknown test statistic: {test_stat}"
+        raise ValueError(msg)
     model, yields = example_model(phi, return_yields=True)
     relaxed_cls = relaxed.infer.hypotest(
-        1, model.expected_data(analytic_pars), model, lr=1e-3, test_stat=test_stat
+        1, model.expected_data(analytic_pars), model, test_stat=test_stat
     )
     m = pyhf.simplemodels.uncorrelated_background(*yields)
     pyhf_cls = pyhf.infer.hypotest(
         1, m.expected_data(analytic_pars), m, test_stat=test_stat
     )
     assert np.allclose(
         relaxed_cls,
         pyhf_cls,
-        atol=0.001,
     )  # tested working without dummy_pyhf on a pyhf fork, but not main yet
 
 
 @pytest.mark.parametrize("test_stat", ["q", "q0"])
 def test_hypotest_expected(test_stat):
     pyhf.set_backend("jax")
     if test_stat == "q":
         analytic_pars = jnp.array([0.0, 1.0])  # bkg-only hypothesis
     elif test_stat == "q0":
         analytic_pars = jnp.array([1.0, 1.0])  # nominal sig+bkg hypothesis
     else:
-        raise ValueError(f"Unknown test statistic: {test_stat}")
+        msg = f"Unknown test statistic: {test_stat}"
+        raise ValueError(msg)
     model, yields = example_model(5.0, return_yields=True)
     relaxed_cls = relaxed.infer.hypotest(
         1,
         model.expected_data(analytic_pars),
         model,
-        lr=1e-3,
         test_stat=test_stat,
         expected_pars=analytic_pars,
     )
     m = pyhf.simplemodels.uncorrelated_background(*yields)
     pyhf_cls = pyhf.infer.hypotest(
         1, m.expected_data(analytic_pars), m, test_stat=test_stat
     )
     assert np.allclose(
         relaxed_cls,
         pyhf_cls,
-        atol=0.001,
     )  # tested working without dummy_pyhf on a pyhf fork, but not main yet
 
 
 @pytest.mark.parametrize("test_stat", ["q", "q0"])
 @pytest.mark.parametrize("expected_pars", [True, False])
 def test_hypotest_grad(test_stat, expected_pars):
     pars = jnp.array([0.0, 1.0])
-    if expected_pars:
-        expars = pars
-    else:
-        expars = None
+    expars = pars if expected_pars else None
 
     def pipeline(x):
         model = uncorrelated_background(x * 5.0, x * 20, x * 2)
-        expected_cls = relaxed.infer.hypotest(
+        return relaxed.infer.hypotest(
             1.0,
             model=model,
             data=model.expected_data(pars),
-            lr=1e-2,
             test_stat=test_stat,
             expected_pars=expars,
         )
-        return expected_cls
 
     jacrev(pipeline)(jnp.asarray(0.5))
 
 
 @pytest.mark.parametrize("expected_pars", [True, False])
 def test_hypotest_grad_noCLs(expected_pars):
     pars = jnp.array([0.0, 1.0])
-    if expected_pars:
-        expars = pars
-    else:
-        expars = None
+    expars = pars if expected_pars else None
 
     def pipeline(x):
         model = uncorrelated_background(x * 5.0, x * 20, x * 2)
-        expected_cls = relaxed.infer.hypotest(
+        return relaxed.infer.hypotest(
             1.0,
             model=model,
             data=model.expected_data(pars),
-            lr=1e-2,
             test_stat="q",
             expected_pars=expars,
             cls_method=False,
         )
-        return expected_cls
 
     jacrev(pipeline)(jnp.asarray(0.5))
 
 
 def test_wrong_test_stat():
-    with pytest.raises(ValueError):
-        model = example_model(0.0)
+    model = example_model(0.0)
+    with pytest.raises(ValueError, match="Unknown test statistic: q1"):
         relaxed.infer.hypotest(
             1,
             model.expected_data(jnp.array([0.0, 1.0])),
             model,
-            lr=1e-2,
             test_stat="q1",
         )
```

### Comparing `relaxed-0.2.2/tests/test_metrics.py` & `relaxed-0.3.0/tests/test_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+from __future__ import annotations
+
 import jax.numpy as jnp
 import numpy as np
 import pyhf
 import pytest
+from dummy_pyhf import example_model, uncorrelated_background
 from jax import jacrev
 from jax.random import PRNGKey
 
 import relaxed
-from relaxed.dummy_pyhf import example_model
 
 
-@pytest.fixture
+@pytest.fixture()
 def data():
     nBg = 8000
     nSig = 300
     bins = np.linspace(0, 70, 10)
     background = np.histogram(np.random.normal(40, 10, nBg), bins=bins)[0]
     signal = np.histogram(np.random.normal(50, 5, nSig), bins=bins)[0]
     return signal, background
 
 
 def test_gaussianity():
     pyhf.set_backend("jax")
-    m = pyhf.simplemodels.uncorrelated_background([5, 5], [50, 50], [5, 5])
+    m = uncorrelated_background(
+        jnp.array([5.0, 5.0]),
+        jnp.array([10.0, 10.0]),
+        jnp.array([0.1, 0.1]),
+    )
     pars = jnp.asarray(m.config.suggested_init())
     data = jnp.asarray(m.expected_data(pars))
     relaxed.metrics.gaussianity(m, pars, data, PRNGKey(0))
 
 
 def test_gaussianity_grad():
     def pipeline(x):
@@ -57,13 +63,12 @@
         pars, bw, endpoints  # bin widths up to the last one (determined by endpoints)
     ):
         s, b = data
         start, end = endpoints
         bins = jnp.cumsum(jnp.array([start, *pars, (end - start) - jnp.sum(pars)]))
         sig_hist = relaxed.hist(s, bins=bins, bandwidth=bw)
         bg_hist = relaxed.hist(b, bins=bins, bandwidth=bw)
-        sig = relaxed.metrics.asimov_sig(sig_hist, bg_hist)
-        return sig
+        return relaxed.metrics.asimov_sig(sig_hist, bg_hist)
 
     jacrev(pipeline)(
         jnp.array([5.0, 10.0, 15.0]), 1e-3, (0, 70)
     )  # just check you can calc it w/o exception
```

### Comparing `relaxed-0.2.2/tests/test_ops.py` & `relaxed-0.3.0/tests/test_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+from __future__ import annotations
+
 from functools import partial
 
+import jax
 import jax.numpy as jnp
 import numpy as np
 import pyhf
 import pytest
+from dummy_pyhf import example_model, uncorrelated_background
 from jax import jacrev, vmap
 from jax.random import PRNGKey, normal
 
 import relaxed
-from relaxed.dummy_pyhf import example_model
+
+jax.config.update("jax_enable_x64", True)
 
 
-@pytest.fixture
+@pytest.fixture()
 def big_sample():
     return normal(PRNGKey(1), shape=(5000,))
 
 
-@pytest.fixture
+@pytest.fixture()
 def bins():
     return np.linspace(-5, 5, 6)
 
 
 def test_hist_validity(big_sample, bins):
     numpy_hist = np.histogram(big_sample, bins=bins)[0]
     relaxed_hist = relaxed.hist(big_sample, bins=bins, bandwidth=1e-6)
@@ -54,16 +59,15 @@
     assert np.allclose(numpy_hist, relaxed_hist, atol=0.01)
 
 
 def test_hist_grad_validity(bins):
     """Test the grads of the kde hist vs the analyitc grads of a normal dist wrt mu."""
 
     def gen_points(mu, jrng, nsamples):
-        points = normal(jrng, shape=(nsamples,)) + mu
-        return points
+        return normal(jrng, shape=(nsamples,)) + mu
 
     def bin_height(mu, jrng, bw, nsamples, bins):
         points = gen_points(mu, jrng, nsamples)
         return relaxed.hist(points, bins, bandwidth=bw)
 
     mus = jnp.linspace(-2, 2, 100)
 
@@ -95,58 +99,65 @@
 
     assert np.allclose(
         relaxed_grads, grads, atol=0.01, rtol=0.05
     )  # tols are a bit high because the grads are a little noisy/biased
 
 
 def test_fisher_info():
+    pyhf.set_backend("jax")
     model = example_model(5.0)
     pars = model.config.suggested_init()
     data = model.expected_data(pars)
     # just check that it doesn't crash
     relaxed.fisher_info(model, pars, data)
 
 
 def test_fisher_uncerts_validity():
     pyhf.set_backend("jax", pyhf.optimize.minuit_optimizer(verbose=1))
-
-    m = pyhf.simplemodels.uncorrelated_background([5, 5], [50, 50], [5, 5])
-
-    data = jnp.array([50.0, 50.0] + m.config.auxdata)
+    m = pyhf.simplemodels.uncorrelated_background([5], [50], [5])
+    data = jnp.array([50.0, *m.config.auxdata])
 
     fit_res = pyhf.infer.mle.fit(
         data,
         m,
         return_uncertainties=True,
         par_bounds=[
             [-1, 10],
             [-1, 10],
-            [-1, 10],
         ],  # fit @ boundary produces unstable uncerts
     )
 
     # minuit fit uncerts
     mle_pars, mle_uncerts = fit_res[:, 0], fit_res[:, 1]
 
     # uncertainties from autodiff hessian
-    relaxed_uncerts = relaxed.cramer_rao_uncert(m, mle_pars, data)
-    assert np.allclose(mle_uncerts, relaxed_uncerts, rtol=5e-2)
+    dummy_m = uncorrelated_background(
+        jnp.array([5]),
+        jnp.array([50]),
+        jnp.array([5]),
+    )
+    relaxed_uncerts = relaxed.cramer_rao_uncert(dummy_m, mle_pars, data)
+    assert np.allclose(mle_uncerts, relaxed_uncerts, rtol=0.05)
 
 
 def test_fisher_info_grad():
+    pyhf.set_backend("jax")
+
     def pipeline(x):
         model = example_model(5.0)
         pars = model.config.suggested_init()
         data = model.expected_data(pars)
         return relaxed.fisher_info(model, pars * x, data * x)
 
     jacrev(pipeline)(4.0)  # just check you can calc it w/o exception
 
 
 def test_fisher_uncert_grad():
+    pyhf.set_backend("jax")
+
     def pipeline(x):
         model = example_model(5.0)
         pars = model.config.suggested_init()
         data = model.expected_data(pars)
         return relaxed.cramer_rao_uncert(model, pars * x, data * x)
 
     jacrev(pipeline)(4.0)  # just check you can calc it w/o exception
@@ -172,9 +183,9 @@
         data = model.expected_data(pars)
         return relaxed.cut(data, x, keep=keep)
 
     jacrev(pipeline)(4.0)  # just check you can calc it w/o exception
 
 
 def test_invalid_cut_keep():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="keep must be one of"):
         relaxed.cut(jnp.array([1, 2, 3]), 0, keep="frogs")
```

