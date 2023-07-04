# Comparing `tmp/error-parity-0.1.4.tar.gz` & `tmp/error-parity-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-parity-0.1.4.tar", last modified: Mon Jun 26 14:21:21 2023, max compression
+gzip compressed data, was "error-parity-0.2.0.tar", last modified: Tue Jul  4 15:41:37 2023, max compression
```

## Comparing `error-parity-0.1.4.tar` & `error-parity-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 14:21:08.000000 error-parity-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 14:21:08.000000 error-parity-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-26 14:21:21.744439 error-parity-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-26 14:21:08.000000 error-parity-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/error_parity/
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/roc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/error_parity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 14:21:08.000000 error-parity-0.1.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 14:21:08.000000 error-parity-0.1.4/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 14:21:08.000000 error-parity-0.1.4/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:21:21.744439 error-parity-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-26 14:21:08.000000 error-parity-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:08.000000 error-parity-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-26 14:21:08.000000 error-parity-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-26 14:21:08.000000 error-parity-0.1.4/tests/test_cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-26 14:21:08.000000 error-parity-0.1.4/tests/test_equal_odds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:37.304294 error-parity-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 15:41:27.000000 error-parity-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-04 15:41:27.000000 error-parity-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-04 15:41:37.304294 error-parity-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-04 15:41:27.000000 error-parity-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:37.300294 error-parity-0.2.0/error_parity/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-07-04 15:41:27.000000 error-parity-0.2.0/error_parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-04 15:41:27.000000 error-parity-0.2.0/error_parity/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-07-04 15:41:27.000000 error-parity-0.2.0/error_parity/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-07-04 15:41:27.000000 error-parity-0.2.0/error_parity/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-04 15:41:27.000000 error-parity-0.2.0/error_parity/roc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18167 2023-07-04 15:41:27.000000 error-parity-0.2.0/error_parity/threshold_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:37.304294 error-parity-0.2.0/error_parity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-04 15:41:37.000000 error-parity-0.2.0/error_parity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-04 15:41:37.000000 error-parity-0.2.0/error_parity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:41:37.000000 error-parity-0.2.0/error_parity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-04 15:41:37.000000 error-parity-0.2.0/error_parity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:41:37.000000 error-parity-0.2.0/error_parity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:37.304294 error-parity-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 15:41:27.000000 error-parity-0.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-04 15:41:27.000000 error-parity-0.2.0/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 15:41:27.000000 error-parity-0.2.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:41:37.304294 error-parity-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-04 15:41:27.000000 error-parity-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:37.304294 error-parity-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:41:27.000000 error-parity-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-04 15:41:27.000000 error-parity-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-04 15:41:27.000000 error-parity-0.2.0/tests/test_cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-04 15:41:27.000000 error-parity-0.2.0/tests/test_equal_odds.py
```

### Comparing `error-parity-0.1.4/LICENSE` & `error-parity-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.4/PKG-INFO` & `error-parity-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.4
+Version: 0.2.0
 Summary: Achieve error-rate parity between protected groups for any predictor
-Home-page: https://github.com/AndreFCruz/error-parity
+Home-page: https://github.com/socialfoundations/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -21,16 +21,16 @@
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 # error-parity
 
-![Tests status](https://github.com/AndreFCruz/error-parity/actions/workflows/python-package.yml/badge.svg)
-![PyPI status](https://github.com/AndreFCruz/error-parity/actions/workflows/python-publish.yml/badge.svg)
+![Tests status](https://github.com/socialfoundations/error-parity/actions/workflows/python-package.yml/badge.svg)
+![PyPI status](https://github.com/socialfoundations/error-parity/actions/workflows/python-publish.yml/badge.svg)
 ![PyPI version](https://badgen.net/pypi/v/error-parity)
 ![OSI license](https://badgen.net/pypi/license/error-parity)
 ![Python compatibility](https://badgen.net/pypi/python/error-parity)
 <!-- ![PyPI version](https://img.shields.io/pypi/v/error-parity) -->
 <!-- ![OSI license](https://img.shields.io/pypi/l/error-parity) -->
 <!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/error-parity) -->
 
@@ -45,28 +45,31 @@
 Install package from [PyPI](https://pypi.org/project/error-parity/):
 ```
 pip install error-parity
 ```
 
 Or, for development, you can clone the repo and install from local sources:
 ```
-git clone https://github.com/AndreFCruz/error-parity.git
+git clone https://github.com/socialfoundations/error-parity.git
 pip install ./error-parity
 ```
 
 
 ## Getting started
 
+> See detailed example notebooks under the [**examples folder**](./examples/).
+
 ```py
-from error_parity import RelaxedEqualOdds
+from error_parity import RelaxedThresholdOptimizer
 
 # Given any trained model that outputs real-valued scores
-fair_clf = RelaxedEqualOdds(
+fair_clf = RelaxedThresholdOptimizer(
     predictor=lambda X: model.predict_proba(X)[:, -1],   # for sklearn API
     # predictor=model,  # use this for a callable model
+    constraint="equalized_odds",
     tolerance=0.05,     # fairness constraint tolerance
 )
 
 # Fit the fairness adjustment on some data
 # This will find the optimal _fair classifier_
 fair_clf.fit(X=X, y=y, group=group)
 
@@ -74,33 +77,38 @@
 # You have to provide group information to compute fair predictions
 y_pred_test = fair_clf(X=X_test, group=group_test)
 ```
 
 
 ## How it works
 
-Given a callable score-based predictor (i.e., `y_pred = predictor(X)`), and some `(X, Y, S)` data to fit, `RelaxedEqualOdds` will:
+Given a callable score-based predictor (i.e., `y_pred = predictor(X)`), and some `(X, Y, S)` data to fit, `RelaxedThresholdOptimizer` will:
 1. Compute group-specific ROC curves and their convex hulls;
 2. Compute the `r`-relaxed optimal solution for the chosen fairness criterion (using [cvxpy](https://www.cvxpy.org));
 3. Find the set of group-specific binary classifiers that match the optimal solution found.
     - each group-specific classifier is made up of (possibly randomized) group-specific thresholds over the given predictor;
     - if a group's ROC point is in the interior of its ROC curve, partial randomization of its predictions may be necessary.
 
 
-## Implementation road-map
+## Features and implementation road-map
 
 We welcome community contributions for [cvxpy](https://www.cvxpy.org) implementations of other fairness constraints.
 
 Currently implemented fairness constraints:
 - [x] equality of odds (Hardt et al., 2016);
   - i.e., equal group-specific TPR and FPR;
+  - use `constraint="equalized_odds"`;
+- [x] equal opportunity;
+  - i.e., equal group-specific TPR;
+  - use `constraint="true_positive_rate_parity"`;
+- [x] predictive equality;
+  - i.e., equal group-specific FPR;
+  - use `constraint="false_positive_rate_parity"`;
 
 Road-map:
-- [ ] equal opportunity;
-  - i.e., equal group-specific TPR;
 - [ ] demographic parity;
   - i.e., equal group-specific predicted prevalence;
 
 
 ## Citing
 
 This repository contains code and supplementary materials for the following preprint:
```

### Comparing `error-parity-0.1.4/README.md` & `error-parity-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # error-parity
 
-![Tests status](https://github.com/AndreFCruz/error-parity/actions/workflows/python-package.yml/badge.svg)
-![PyPI status](https://github.com/AndreFCruz/error-parity/actions/workflows/python-publish.yml/badge.svg)
+![Tests status](https://github.com/socialfoundations/error-parity/actions/workflows/python-package.yml/badge.svg)
+![PyPI status](https://github.com/socialfoundations/error-parity/actions/workflows/python-publish.yml/badge.svg)
 ![PyPI version](https://badgen.net/pypi/v/error-parity)
 ![OSI license](https://badgen.net/pypi/license/error-parity)
 ![Python compatibility](https://badgen.net/pypi/python/error-parity)
 <!-- ![PyPI version](https://img.shields.io/pypi/v/error-parity) -->
 <!-- ![OSI license](https://img.shields.io/pypi/l/error-parity) -->
 <!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/error-parity) -->
 
@@ -20,28 +20,31 @@
 Install package from [PyPI](https://pypi.org/project/error-parity/):
 ```
 pip install error-parity
 ```
 
 Or, for development, you can clone the repo and install from local sources:
 ```
-git clone https://github.com/AndreFCruz/error-parity.git
+git clone https://github.com/socialfoundations/error-parity.git
 pip install ./error-parity
 ```
 
 
 ## Getting started
 
+> See detailed example notebooks under the [**examples folder**](./examples/).
+
 ```py
-from error_parity import RelaxedEqualOdds
+from error_parity import RelaxedThresholdOptimizer
 
 # Given any trained model that outputs real-valued scores
-fair_clf = RelaxedEqualOdds(
+fair_clf = RelaxedThresholdOptimizer(
     predictor=lambda X: model.predict_proba(X)[:, -1],   # for sklearn API
     # predictor=model,  # use this for a callable model
+    constraint="equalized_odds",
     tolerance=0.05,     # fairness constraint tolerance
 )
 
 # Fit the fairness adjustment on some data
 # This will find the optimal _fair classifier_
 fair_clf.fit(X=X, y=y, group=group)
 
@@ -49,33 +52,38 @@
 # You have to provide group information to compute fair predictions
 y_pred_test = fair_clf(X=X_test, group=group_test)
 ```
 
 
 ## How it works
 
-Given a callable score-based predictor (i.e., `y_pred = predictor(X)`), and some `(X, Y, S)` data to fit, `RelaxedEqualOdds` will:
+Given a callable score-based predictor (i.e., `y_pred = predictor(X)`), and some `(X, Y, S)` data to fit, `RelaxedThresholdOptimizer` will:
 1. Compute group-specific ROC curves and their convex hulls;
 2. Compute the `r`-relaxed optimal solution for the chosen fairness criterion (using [cvxpy](https://www.cvxpy.org));
 3. Find the set of group-specific binary classifiers that match the optimal solution found.
     - each group-specific classifier is made up of (possibly randomized) group-specific thresholds over the given predictor;
     - if a group's ROC point is in the interior of its ROC curve, partial randomization of its predictions may be necessary.
 
 
-## Implementation road-map
+## Features and implementation road-map
 
 We welcome community contributions for [cvxpy](https://www.cvxpy.org) implementations of other fairness constraints.
 
 Currently implemented fairness constraints:
 - [x] equality of odds (Hardt et al., 2016);
   - i.e., equal group-specific TPR and FPR;
+  - use `constraint="equalized_odds"`;
+- [x] equal opportunity;
+  - i.e., equal group-specific TPR;
+  - use `constraint="true_positive_rate_parity"`;
+- [x] predictive equality;
+  - i.e., equal group-specific FPR;
+  - use `constraint="false_positive_rate_parity"`;
 
 Road-map:
-- [ ] equal opportunity;
-  - i.e., equal group-specific TPR;
 - [ ] demographic parity;
   - i.e., equal group-specific predicted prevalence;
 
 
 ## Citing
 
 This repository contains code and supplementary materials for the following preprint:
```

### Comparing `error-parity-0.1.4/error_parity/classifiers.py` & `error-parity-0.2.0/error_parity/classifiers.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.4/error_parity/cvxpy_utils.py` & `error-parity-0.2.0/error_parity/cvxpy_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,28 @@
 
 from .roc_utils import calc_cost_of_point, compute_global_roc_from_groupwise
 
 
 # Maximum distance from solution to feasibility or optimality
 SOLUTION_TOLERANCE = 1e-9
 
+# Set of all fairness constraints with a cvxpy LP implementation
+ALL_CONSTRAINTS = {
+    "equalized_odds",
+    "true_positive_rate_parity",
+    "false_positive_rate_parity",
+    "true_negative_rate_parity",
+    "false_negative_rate_parity",
+}
+
+NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE = (
+    "Currently only the following constraints are supported: {}.".format(
+        ", ".join(sorted(ALL_CONSTRAINTS))
+    )
+)
 
 def compute_line(p1: np.ndarray, p2: np.ndarray) -> tuple[float, float]:
     """Computes the slope and intercept of the line that passes
     through the two given points.
     
     The intercept is the value at x=0!
     (or NaN for vertical lines)
@@ -207,55 +221,72 @@
             polygon_vertices[i], polygon_vertices[(i+1) % len(polygon_vertices)],
             cvxpy_point,
         )
         for i in range(len(polygon_vertices))
     ]
 
 
-def compute_equal_odds_optimum(
+def compute_fair_optimum(
+        *,
+        fairness_constraint: str,
+        tolerance: float,
         groupwise_roc_hulls: dict[int, np.ndarray],
-        fairness_tolerance: float,
         group_sizes_label_pos: np.ndarray,
         group_sizes_label_neg: np.ndarray,
         global_prevalence: float,
         false_positive_cost: float = 1.,
         false_negative_cost: float = 1.,
     ) -> tuple[np.ndarray, np.ndarray]:
     """Computes the solution to finding the optimal fair (equal odds) classifier.
 
     Can relax the equal odds constraint by some given tolerance.
 
     Parameters
     ----------
+    fairness_constraint : str
+        The name of the fairness constraint under which the LP will be 
+        optimized. Possible inputs are:
+
+            'equalized_odds'
+                match true positive and false positive rates across groups
+
+    tolerance : float
+        A value for the tolerance when enforcing the fairness constraint.
+
     groupwise_roc_hulls : dict[int, np.ndarray]
         A dict mapping each group to the convex hull of the group's ROC curve.
         The convex hull is an np.array of shape (n_points, 2), containing the 
         points that form the convex hull of the ROC curve, sorted in COUNTER
         CLOCK-WISE order.
-    fairness_tolerance : float
-        A value for the tolerance when enforcing the equal odds fairness 
-        constraint, i.e., equality of TPR and FPR among groups.
+
     group_sizes_label_pos : np.ndarray
         The relative or absolute number of positive samples in each group.
+
     group_sizes_label_neg : np.ndarray
         The relative or absolute number of negative samples in each group.
+
     global_prevalence : float
         The global prevalence of positive samples.
+
     false_positive_cost : float, optional
         The cost of a FALSE POSITIVE error, by default 1.
+
     false_negative_cost : float, optional
         The cost of a FALSE NEGATIVE error, by default 1.
 
     Returns
     -------
     (groupwise_roc_points, global_roc_point) : tuple[np.ndarray, np.ndarray]
         A tuple pair, (<1>, <2>), containing:
         1: an array with the group-wise ROC points for the solution.
         2: an array with the single global ROC point for the solution.
     """
+    if fairness_constraint not in ALL_CONSTRAINTS:
+        raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
+
     n_groups = len(groupwise_roc_hulls)
     if n_groups != len(group_sizes_label_neg) or n_groups != len(group_sizes_label_pos):
         raise ValueError(
             f"Invalid arguments; all of the following should have the same "
             f"length: groupwise_roc_hulls, group_sizes_label_neg, group_sizes_label_pos;")
 
     # Group-wise ROC points
@@ -270,22 +301,48 @@
         # Global FPR is the average of group FPRs weighted by LNs in each group
         global_roc_point_var[0] == group_sizes_label_neg @ np.array([p[0] for p in groupwise_roc_points_vars]),
 
         # Global TPR is the average of group TPRs weighted by LPs in each group
         global_roc_point_var[1] == group_sizes_label_pos @ np.array([p[1] for p in groupwise_roc_points_vars]),
     ]
 
-    # Relaxed equal odds constraints
-    # 1st option - CONSTRAINT FOR: l-inf distance between any two group's ROCs being less than epsilon
-    constraints += [
-        cp.norm_inf(groupwise_roc_points_vars[i] - groupwise_roc_points_vars[j]) <= fairness_tolerance
-        for i, j in product(range(n_groups), range(n_groups))
-        if i < j
-        # if i != j
-    ]
+    ### APPLY FAIRNESS CONSTRAINTS
+    # If "equalized_odds"
+    # > i.e., constrain l-inf distance between any two groups' ROCs being less than `tolerance`
+    if fairness_constraint == "equalized_odds":
+        constraints += [
+            cp.norm_inf(groupwise_roc_points_vars[i] - groupwise_roc_points_vars[j]) <= tolerance
+            for i, j in product(range(n_groups), range(n_groups))
+            if i < j
+        ]
+
+    # If some rate parity, i.e., parity of one of {TPR, FPR, TNR, FNR}
+    # i.e., constrain absolute distance between any two groups' rate metric
+    elif fairness_constraint.endswith("rate_parity"):
+
+        roc_idx_of_interest: int
+        if fairness_constraint == "true_positive_rate_parity" or fairness_constraint == "false_negative_rate_parity":
+            roc_idx_of_interest = 1
+
+        elif fairness_constraint == "false_positive_rate_parity" or fairness_constraint == "false_negative_rate_parity":
+            roc_idx_of_interest = 0
+        
+        else:
+            # This point should never be reached as fairness constraint was previously validated
+            raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
+
+        constraints += [
+            cp.abs(groupwise_roc_points_vars[i][roc_idx_of_interest] - groupwise_roc_points_vars[j][roc_idx_of_interest]) <= tolerance
+            for i, j in product(range(n_groups), range(n_groups))
+            if i < j
+        ]
+
+    # TODO: implement other constraints here
+    else:
+        raise NotImplementedError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
 
     # Constraints for points in respective group-wise ROC curves
     for idx in range(n_groups):
         constraints += make_cvxpy_point_in_polygon_constraints(
             polygon_vertices=groupwise_roc_hulls[idx],
             cvxpy_point=groupwise_roc_points_vars[idx])
 
@@ -318,53 +375,35 @@
         # This line should never be reached (there are always trivial fair
         # solutions in the ROC diagonal)
         raise ValueError(f"cvxpy problem has no solution; status={prob.status}")
 
     groupwise_roc_points = np.vstack([p.value for p in groupwise_roc_points_vars])
     global_roc_point = global_roc_point_var.value
 
-    # Sanity check solution cost
+    # Validating solution cost
     solution_cost = calc_cost_of_point(
         fpr=global_roc_point[0],
         fnr=1-global_roc_point[1],
         prevalence=global_prevalence,
         false_pos_cost=false_positive_cost,
         false_neg_cost=false_negative_cost,
     )
 
     if not np.isclose(solution_cost, prob.value):
         logging.error(
-            f"Solution was found but cost did not pass sanity check! "
+            f"Solution was found but cost did not pass validation! "
             f"Found solution ROC point {global_roc_point} with theoretical cost "
             f"{prob.value}, but actual cost is {solution_cost};")
 
-    # Sanity check congruency between group-wise ROC points and global ROC point
+    # Validating congruency between group-wise ROC points and global ROC point
     global_roc_from_groupwise = compute_global_roc_from_groupwise(
         groupwise_roc_points=groupwise_roc_points,
         groupwise_label_pos_weight=group_sizes_label_pos,
         groupwise_label_neg_weight=group_sizes_label_neg,
     )
     if not all(np.isclose(global_roc_from_groupwise, global_roc_point)):
         logging.error(
             f"Solution: global ROC point ({global_roc_point}) does not seem to "
             f"match group-wise ROC points; global should be "
             f"({global_roc_from_groupwise}) to be consistent with group-wise;")
 
     return groupwise_roc_points, global_roc_point
-
-
-def _plot_polygons(polygons: list[np.ndarray]):
-    from matplotlib import pyplot as plt
-    fig = plt.figure(dpi=200, figsize=(5, 5))
-
-    for i, poly in enumerate(polygons):
-
-        # Plot ROC curve
-        plt.fill(
-            poly[:, 0], poly[:, 1],
-            alpha=0.2,
-            label=f"poly {i}",
-        )
-        
-        plt.legend(loc='lower right')
-    
-    plt.plot()
```

### Comparing `error-parity-0.1.4/error_parity/equal_odds.py` & `error-parity-0.2.0/error_parity/threshold_optimizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,67 @@
 """Solver for the relaxed equal odds problem.
 
 TODO
-- Add option for constraining only equality of FPR or TPR (currently it must be 
-both -> equal odds);
 - Add option for constraining equality of positive predictions (independence
 criterion, aka demographic parity);
 
 """
+from __future__ import annotations
+
 import logging
 from itertools import product
 from typing import Callable
 
 import numpy as np
 from sklearn.metrics import roc_curve
 
-from .cvxpy_utils import compute_equal_odds_optimum
+from .cvxpy_utils import (
+    compute_fair_optimum,
+    ALL_CONSTRAINTS,
+    NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE,
+)
 from .roc_utils import (
     roc_convex_hull,
     plot_polygon_edges,
     calc_cost_of_point,
 )
 from .classifiers import (
     Classifier,
     RandomizedClassifier,
     EnsembleGroupwiseClassifiers,
 )
 
 
-class RelaxedEqualOdds(Classifier):
+class RelaxedThresholdOptimizer(Classifier):
     """Class to encapsulate all the logic needed to compute the optimal equal
     odds classifier (with possibly relaxed constraints).
     """
 
     def __init__(
             self,
+            *,
             predictor: Callable[[np.ndarray], np.ndarray],
-            tolerance: float,
+            constraint: str = "equalized_odds",
+            tolerance: float = 0.0,
             false_pos_cost: float = 1.0,
             false_neg_cost: float = 1.0,
             max_roc_ticks: int = 1000,
             seed: int = 42,
             # distance: str = 'max',    # TODO: add option to use l1 or linf distances
         ):
         """Initializes the relaxed equal odds wrapper.
 
         Parameters
         ----------
         predictor : callable[(np.ndarray), float]
             A trained score predictor that takes in samples, X, in shape
             (num_samples, num_features), and outputs real-valued scores, R, in
             shape (num_samples,).
+        constraint : str
+            The fairness constraint to use. By default "equalized_odds".
         tolerance : float
             The absolute tolerance for the equal odds fairness constraint.
             Will allow for `tolerance` difference between group-wise ROC points.
         false_pos_cost : float, optional
             The cost of a FALSE POSITIVE error, by default 1.0.
         false_neg_cost : float, optional
             The cost of a FALSE NEGATIVE error, by default 1.0.
@@ -62,20 +70,25 @@
             computing the optimal fair classifier, by default 1000.
         seed : int
             A random seed used for reproducibility when producing randomized
             classifiers.
         """
         # Save arguments
         self.predictor = predictor
+        self.constraint = constraint
         self.tolerance = tolerance
         self.false_pos_cost = false_pos_cost
         self.false_neg_cost = false_neg_cost
         self.max_roc_ticks = max_roc_ticks
         self.seed = seed
 
+        # Validate constraint
+        if self.constraint not in ALL_CONSTRAINTS:
+            raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
+
         # Initialize instance variables
         self._all_roc_data: dict = None
         self._all_roc_hulls: dict = None
         self._groupwise_roc_points: np.ndarray = None
         self._global_roc_point: np.ndarray = None
         self._global_prevalence: float = None
         self._realized_classifier: EnsembleGroupwiseClassifiers = None
@@ -118,61 +131,124 @@
         return calc_cost_of_point(
             fpr=global_fpr,
             fnr=1 - global_tpr,
             prevalence=self._global_prevalence,
             false_pos_cost=false_pos_cost or self.false_pos_cost,
             false_neg_cost=false_neg_cost or self.false_neg_cost,
         )
-    
+
     def constraint_violation(self) -> float:
-        """This method should be part of a common interface between different
-        relaxed-constraint classes.
+        """Constraint violation of the LP solution found.
 
         Returns
         -------
         float
             The fairness constraint violation.
         """
-        return self.equal_odds_violation()
+        self._check_fit_status()
+
+        if self.constraint not in ALL_CONSTRAINTS:
+            raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
+
+        if self.constraint == "equalized_odds":
+            return self.equalized_odds_violation()
+
+        elif self.constraint.endswith("rate_parity"):
+            constraint_to_error_type = {
+                "true_positive_rate_parity": "fn",
+                "false_positive_rate_parity": "fp",
+                "true_negative_rate_parity": "fp",
+                "false_negative_rate_parity": "fn",
+            }
+
+            return self.error_rate_parity_constraint_violation(
+                error_type=constraint_to_error_type[self.constraint],
+            )
+
+        else:
+            raise NotImplementedError(
+                f"Standalone constraint violation not yet computed for "
+                f"constraint='{self.constraint}'."
+            )
+    
+    def error_rate_parity_constraint_violation(self, error_type: str) -> float:
+        """Computes the theoretical violation of an error-rate parity 
+        constraint.
+
+        Parameters
+        ----------
+        error_type : str
+            One of the following values:
+                "fp", for false positive errors (FPR or TNR parity);
+                "fn", for false negative errors (TPR or FNR parity).
 
-    def equal_odds_violation(self) -> float:
+        Returns
+        -------
+        float
+            The maximum constraint violation among all groups.
+        """
+        self._check_fit_status()
+        valid_error_types = ("fp", "fn")
+        if error_type not in valid_error_types:
+            raise ValueError(
+                f"Invalid error_type='{error_type}', must be one of "
+                f"{valid_error_types}.")
+
+        roc_idx_of_interest = 0 if error_type == "fp" else 1
+
+        return self._max_l_inf_between_points(
+            points=[
+                roc_point[roc_idx_of_interest]
+                for roc_point in self.groupwise_roc_points
+            ],
+        )
+    
+    def equalized_odds_violation(self) -> float:
         """Computes the theoretical violation of the equal odds constraint 
         (i.e., the maximum l-inf distance between the ROC point of any pair
         of groups).
 
         Returns
         -------
         float
             The equal-odds constraint violation.
         """
         self._check_fit_status()
 
-        n_groups = len(self.groupwise_roc_points)
+        # Compute l-inf distance between each pair of groups
+        return self._max_l_inf_between_points(
+            points=self.groupwise_roc_points,
+        )
+
+    @staticmethod
+    def _max_l_inf_between_points(points: list[float | np.ndarray]) -> float:
+
+        # Number of points (should correspond to the number of groups)
+        n_points = len(points)
 
         # Compute l-inf distance between each pair of groups
-        linf_constraint_violation = [
+        l_inf_constraint_violation = [
             (np.linalg.norm(
-                self.groupwise_roc_points[i] - self.groupwise_roc_points[j],
+                points[i] - points[j],
                 ord=np.inf), (i, j))
-            for i, j in product(range(n_groups), range(n_groups))
+            for i, j in product(range(n_points), range(n_points))
             if i < j
         ]
 
         # Return the maximum
-        max_violation, (groupA, groupB) = max(linf_constraint_violation)
+        max_violation, (groupA, groupB) = max(l_inf_constraint_violation)
         logging.info(
             f"Maximum fairness violation is between "
-            f"group={groupA} (p={self.groupwise_roc_points[groupA]}) and "
-            f"group={groupB} (p={self.groupwise_roc_points[groupB]});"
+            f"group={groupA} (p={points[groupA]}) and "
+            f"group={groupB} (p={points[groupB]});"
         )
 
         return max_violation
 
-
-    def fit(self, X: np.ndarray, y: np.ndarray, group: np.ndarray, y_scores: np.ndarray = None):
+    def fit(self, X: np.ndarray, y: np.ndarray, *, group: np.ndarray, y_scores: np.ndarray = None):
         """Fit this predictor to achieve the (possibly relaxed) equal odds 
         constraint on the provided data.
 
         Parameters
         ----------
         X : np.ndarray
             The input features.
@@ -248,17 +324,18 @@
 
             curr_roc_points = np.stack((group_fpr, group_tpr), axis=1)
             curr_roc_points = np.vstack((curr_roc_points, [1, 0]))  # Add point (1, 0) to ROC curve
 
             self._all_roc_hulls[g] = roc_convex_hull(curr_roc_points)
 
         # Find the group-wise optima that fulfill the fairness criteria
-        self._groupwise_roc_points, self._global_roc_point = compute_equal_odds_optimum(
+        self._groupwise_roc_points, self._global_roc_point = compute_fair_optimum(
+            fairness_constraint=self.constraint,
+            tolerance=self.tolerance,
             groupwise_roc_hulls=self._all_roc_hulls,
-            fairness_tolerance=self.tolerance,
             group_sizes_label_pos=group_sizes_label_pos,
             group_sizes_label_neg=group_sizes_label_neg,
             global_prevalence=self._global_prevalence,
             false_positive_cost=self.false_pos_cost,
             false_negative_cost=self.false_neg_cost,
         )
 
@@ -305,14 +382,15 @@
                 "There's nothing to plot: this classifier has not yet been "
                 "fitted to any data. Call clf.fit(...) before clf.plot().")
 
         return True
 
     def plot(
             self,
+            *,
             plot_roc_curves: bool = False,
             plot_roc_hulls: bool = True,
             plot_group_optima: bool = True,
             plot_group_triangulation: bool = True,
             plot_global_optimum: bool = True,
             plot_diagonal: bool = True,
             plot_relaxation: bool = False,
@@ -423,18 +501,20 @@
             plt.plot(
                 [0, 1], [0, 1],
                 ls='--', color="grey", alpha=0.5,
                 label="random clf.",
             )
 
         # Set axis settings
-        plt.title(f"Solution to {self.tolerance}-relaxed equal odds optimum")
+        plt.suptitle(f"Solution to {self.tolerance}-relaxed optimum", y=0.96)
+        plt.title(f"(fairness constraint: {self.constraint.replace('_', ' ')})", fontsize="small")
+
         plt.xlabel("False Positive Rate")
         plt.ylabel("True Positive Rate")
 
         plt.legend(loc="lower right", borderaxespad=2)
 
-    def __call__(self, X: np.ndarray, group: np.ndarray) -> int:
+    def __call__(self, X: np.ndarray, *, group: np.ndarray) -> int:
         return self._realized_classifier(X, group)
 
-    def predict(self, X: np.ndarray, group: np.ndarray) -> int:
-        return self(X, group)
+    def predict(self, X: np.ndarray, *, group: np.ndarray) -> int:
+        return self(X, group=group)
```

### Comparing `error-parity-0.1.4/error_parity/roc_utils.py` & `error-parity-0.2.0/error_parity/roc_utils.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.4/error_parity.egg-info/PKG-INFO` & `error-parity-0.2.0/error_parity.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.4
+Version: 0.2.0
 Summary: Achieve error-rate parity between protected groups for any predictor
-Home-page: https://github.com/AndreFCruz/error-parity
+Home-page: https://github.com/socialfoundations/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -21,16 +21,16 @@
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 # error-parity
 
-![Tests status](https://github.com/AndreFCruz/error-parity/actions/workflows/python-package.yml/badge.svg)
-![PyPI status](https://github.com/AndreFCruz/error-parity/actions/workflows/python-publish.yml/badge.svg)
+![Tests status](https://github.com/socialfoundations/error-parity/actions/workflows/python-package.yml/badge.svg)
+![PyPI status](https://github.com/socialfoundations/error-parity/actions/workflows/python-publish.yml/badge.svg)
 ![PyPI version](https://badgen.net/pypi/v/error-parity)
 ![OSI license](https://badgen.net/pypi/license/error-parity)
 ![Python compatibility](https://badgen.net/pypi/python/error-parity)
 <!-- ![PyPI version](https://img.shields.io/pypi/v/error-parity) -->
 <!-- ![OSI license](https://img.shields.io/pypi/l/error-parity) -->
 <!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/error-parity) -->
 
@@ -45,28 +45,31 @@
 Install package from [PyPI](https://pypi.org/project/error-parity/):
 ```
 pip install error-parity
 ```
 
 Or, for development, you can clone the repo and install from local sources:
 ```
-git clone https://github.com/AndreFCruz/error-parity.git
+git clone https://github.com/socialfoundations/error-parity.git
 pip install ./error-parity
 ```
 
 
 ## Getting started
 
+> See detailed example notebooks under the [**examples folder**](./examples/).
+
 ```py
-from error_parity import RelaxedEqualOdds
+from error_parity import RelaxedThresholdOptimizer
 
 # Given any trained model that outputs real-valued scores
-fair_clf = RelaxedEqualOdds(
+fair_clf = RelaxedThresholdOptimizer(
     predictor=lambda X: model.predict_proba(X)[:, -1],   # for sklearn API
     # predictor=model,  # use this for a callable model
+    constraint="equalized_odds",
     tolerance=0.05,     # fairness constraint tolerance
 )
 
 # Fit the fairness adjustment on some data
 # This will find the optimal _fair classifier_
 fair_clf.fit(X=X, y=y, group=group)
 
@@ -74,33 +77,38 @@
 # You have to provide group information to compute fair predictions
 y_pred_test = fair_clf(X=X_test, group=group_test)
 ```
 
 
 ## How it works
 
-Given a callable score-based predictor (i.e., `y_pred = predictor(X)`), and some `(X, Y, S)` data to fit, `RelaxedEqualOdds` will:
+Given a callable score-based predictor (i.e., `y_pred = predictor(X)`), and some `(X, Y, S)` data to fit, `RelaxedThresholdOptimizer` will:
 1. Compute group-specific ROC curves and their convex hulls;
 2. Compute the `r`-relaxed optimal solution for the chosen fairness criterion (using [cvxpy](https://www.cvxpy.org));
 3. Find the set of group-specific binary classifiers that match the optimal solution found.
     - each group-specific classifier is made up of (possibly randomized) group-specific thresholds over the given predictor;
     - if a group's ROC point is in the interior of its ROC curve, partial randomization of its predictions may be necessary.
 
 
-## Implementation road-map
+## Features and implementation road-map
 
 We welcome community contributions for [cvxpy](https://www.cvxpy.org) implementations of other fairness constraints.
 
 Currently implemented fairness constraints:
 - [x] equality of odds (Hardt et al., 2016);
   - i.e., equal group-specific TPR and FPR;
+  - use `constraint="equalized_odds"`;
+- [x] equal opportunity;
+  - i.e., equal group-specific TPR;
+  - use `constraint="true_positive_rate_parity"`;
+- [x] predictive equality;
+  - i.e., equal group-specific FPR;
+  - use `constraint="false_positive_rate_parity"`;
 
 Road-map:
-- [ ] equal opportunity;
-  - i.e., equal group-specific TPR;
 - [ ] demographic parity;
   - i.e., equal group-specific predicted prevalence;
 
 
 ## Citing
 
 This repository contains code and supplementary materials for the following preprint:
```

### Comparing `error-parity-0.1.4/error_parity.egg-info/SOURCES.txt` & `error-parity-0.2.0/error_parity.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 MANIFEST.in
 README.md
 setup.py
 error_parity/__init__.py
 error_parity/_version.py
 error_parity/classifiers.py
 error_parity/cvxpy_utils.py
-error_parity/equal_odds.py
 error_parity/roc_utils.py
+error_parity/threshold_optimizer.py
 error_parity.egg-info/PKG-INFO
 error_parity.egg-info/SOURCES.txt
 error_parity.egg-info/dependency_links.txt
 error_parity.egg-info/requires.txt
 error_parity.egg-info/top_level.txt
 requirements/dev.txt
 requirements/main.txt
```

### Comparing `error-parity-0.1.4/setup.py` & `error-parity-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     extras_require={
         "test": test_requirements,
         "dev": dev_requirements,
         "all": dev_requirements + test_requirements,
     },
 
     author='AndreFCruz',
-    url='https://github.com/AndreFCruz/error-parity',
+    url='https://github.com/socialfoundations/error-parity',
 
     license='MIT',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Science/Research',
```

### Comparing `error-parity-0.1.4/tests/conftest.py` & `error-parity-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.4/tests/test_cvxpy_utils.py` & `error-parity-0.2.0/tests/test_cvxpy_utils.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.4/tests/test_equal_odds.py` & `error-parity-0.2.0/tests/test_equal_odds.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 from itertools import product
 
 import pytest
 import numpy as np
 from sklearn.metrics import roc_auc_score
 
-from error_parity import RelaxedEqualOdds
+from error_parity import RelaxedThresholdOptimizer
 from error_parity.cvxpy_utils import SOLUTION_TOLERANCE, calc_cost_of_point
 from error_parity.roc_utils import compute_roc_point_from_predictions
 
 
 def test_synthetic_data_generation(
         y_true: np.ndarray,
         y_pred_scores: np.ndarray,
@@ -51,15 +51,23 @@
         atol=get_metric_abs_tolerance(group_size),
         rtol=0.01,
     ), (
         f"> '{metric_name}' mismatch; expected {theory_val:.3}; got {empirical_val:.3};"
     )
 
 
-def test_equal_odds_constraint_relaxation(
+def test_invalid_constraint_name():
+    with pytest.raises(ValueError) as excinfo:
+        clf = RelaxedThresholdOptimizer(
+            predictor=print,
+            constraint="random constraint name",
+        )
+
+
+def test_equalized_odds_constraint_relaxation(
         y_true: np.ndarray,
         y_pred_scores: np.ndarray,
         sensitive_attribute: np.ndarray,
         constraint_slack: float,
         random_seed: int,
     ):
     num_samples = len(y_true)
@@ -69,34 +77,35 @@
     # Predictor function
     # # > predicts the generated scores from the sample indices
     predictor = lambda idx: y_pred_scores[idx]
 
     # Hence, for this example, the features are the sample indices
     X_features = np.arange(num_samples)
 
-    clf = RelaxedEqualOdds(
+    clf = RelaxedThresholdOptimizer(
         predictor=predictor,
+        constraint="equalized_odds",
         tolerance=constraint_slack,
         false_pos_cost=1,
         false_neg_cost=1,
         seed=random_seed,
     )
 
     # Fit postprocessing to data
     clf.fit(X=X_features, y=y_true, group=sensitive_attribute)
 
     # Check that theoretical solution fulfills relaxed constraint
-    assert clf.equal_odds_violation() <= constraint_slack + SOLUTION_TOLERANCE, (
+    assert clf.equalized_odds_violation() <= constraint_slack + SOLUTION_TOLERANCE, (
         f"Solution fails to hit the target EO constraint; "
-        f"got: {clf.equal_odds_violation()}; "
+        f"got: {clf.equalized_odds_violation()}; "
         f"expected less than {constraint_slack};"
     )
 
     # Optimal binarized predictions
-    y_pred_binary = clf(X_features, sensitive_attribute)
+    y_pred_binary = clf(X_features, group=sensitive_attribute)
 
     # Check realized group-specific ROC points
     actual_group_roc_points = np.vstack([
         compute_roc_point_from_predictions(
             y_true=y_true[sensitive_attribute == g],
             y_pred_binary=y_pred_binary[sensitive_attribute == g],
         )
@@ -140,17 +149,17 @@
 
     # > empirical tolerance for constraint violation depends on the smallest group size
     smallest_denominator = min(
         np.sum(labels[sensitive_attribute == g])
         for g in unique_groups
         for labels in (y_true, 1-y_true)
     )
-    actual_equal_odds_violation = np.max(groupwise_differences)
+    actual_equalized_odds_violation = np.max(groupwise_differences)
     check_metric_tolerance(
-        empirical_val=max(actual_equal_odds_violation - constraint_slack, 0),
+        empirical_val=max(actual_equalized_odds_violation - constraint_slack, 0),
         theory_val=0.0,
         group_size=smallest_denominator,
         metric_name="EO violation above slack",
     )
 
     # Check realized global ROC point
     target_fpr, target_tpr = clf.global_roc_point
@@ -181,10 +190,20 @@
     check_metric_tolerance(
         theoretical_cost, actual_cost,
         group_size=num_samples,
         metric_name="classification loss",
     )
 
 
+def test_tpr_parity_constraint():
+    # TODO: test relaxation of TPR parity constraint
+    pass
+
+
+def test_fpr_parity_constraint():
+    # TODO: test relaxation of FPR parity constraint
+    pass
+
+
 def test_unprocessing():
     # TODO: test that unconstrained postprocessing strictly increases accuracy, whichever the input
     pass
```

