# Comparing `tmp/regain-0.3.8.tar.gz` & `tmp/regain-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regain-0.3.8.tar", last modified: Wed Apr 19 10:38:40 2023, max compression
+gzip compressed data, was "regain-0.3.9.tar", last modified: Tue Jul  4 09:26:27 2023, max compression
```

## Comparing `regain-0.3.8.tar` & `regain-0.3.9.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.615666 regain-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-19 10:38:27.000000 regain-0.3.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-19 10:38:27.000000 regain-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-19 10:38:27.000000 regain-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-19 10:38:40.615666 regain-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-19 10:38:27.000000 regain-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.595665 regain-0.3.8/regain/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-19 10:38:27.000000 regain-0.3.8/regain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.599665 regain-0.3.8/regain/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3427 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/_laplace_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/gaussian_process_.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15577 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/gwishart_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8907 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/wishart_distribution_.py
--rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-04-19 10:38:27.000000 regain-0.3.8/regain/bayesian/wishart_process_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-19 10:38:27.000000 regain-0.3.8/regain/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.603665 regain-0.3.8/regain/covariance/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/graphical_lasso_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/infimal_convolution_.py
--rw-r--r--   0 runner    (1001) docker     (123)    30869 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/kernel_latent_time_graphical_lasso_.py
--rw-r--r--   0 runner    (1001) docker     (123)    28021 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/kernel_time_graphical_lasso_.py
--rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/latent_graphical_lasso_.py
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/latent_time_graphical_lasso_.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/latent_time_matrix_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/missing_graphical_lasso_.py
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-04-19 10:38:27.000000 regain-0.3.8/regain/covariance/time_graphical_lasso_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.603665 regain-0.3.8/regain/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 10:38:27.000000 regain-0.3.8/regain/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-19 10:38:27.000000 regain-0.3.8/regain/data/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.607665 regain-0.3.8/regain/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23461 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/ising.py
--rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/multi_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-04-19 10:38:27.000000 regain-0.3.8/regain/datasets/poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-19 10:38:27.000000 regain-0.3.8/regain/discriminant_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.607665 regain-0.3.8/regain/forward_backward/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-19 10:38:27.000000 regain-0.3.8/regain/forward_backward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-19 10:38:27.000000 regain-0.3.8/regain/forward_backward/forward_backward.py
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-04-19 10:38:27.000000 regain-0.3.8/regain/forward_backward/time_graphical_lasso_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.611665 regain-0.3.8/regain/generalized_linear_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_ising.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_time_ising.py
--rw-r--r--   0 runner    (1001) docker     (123)    26895 2023-04-19 10:38:27.000000 regain-0.3.8/regain/generalized_linear_model/glm_time_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.611665 regain-0.3.8/regain/linear_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/_group_lasso_overlap_old_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/group_lasso_.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/group_lasso_overlap_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-19 10:38:27.000000 regain-0.3.8/regain/linear_model/lasso_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.611665 regain-0.3.8/regain/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 10:38:27.000000 regain-0.3.8/regain/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-04-19 10:38:27.000000 regain-0.3.8/regain/model_selection/_bayesian_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    27777 2023-04-19 10:38:27.000000 regain-0.3.8/regain/model_selection/stability_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-19 10:38:27.000000 regain-0.3.8/regain/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.615666 regain-0.3.8/regain/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/plotly.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-19 10:38:27.000000 regain-0.3.8/regain/plotting/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-04-19 10:38:27.000000 regain-0.3.8/regain/prox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-19 10:38:27.000000 regain-0.3.8/regain/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-19 10:38:27.000000 regain-0.3.8/regain/update_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-04-19 10:38:27.000000 regain-0.3.8/regain/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-19 10:38:27.000000 regain-0.3.8/regain/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.615666 regain-0.3.8/regain/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-19 10:38:27.000000 regain-0.3.8/regain/wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.615666 regain-0.3.8/regain/wrapper/paspal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:27.000000 regain-0.3.8/regain/wrapper/paspal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-19 10:38:27.000000 regain-0.3.8/regain/wrapper/paspal/glopridu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:38:40.599665 regain-0.3.8/regain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-19 10:38:40.000000 regain-0.3.8/regain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-19 10:38:40.000000 regain-0.3.8/regain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:38:40.000000 regain-0.3.8/regain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 10:38:40.000000 regain-0.3.8/regain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-19 10:38:40.615666 regain-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 10:38:27.000000 regain-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.469467 regain-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 09:26:17.000000 regain-0.3.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 09:26:17.000000 regain-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 09:26:17.000000 regain-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-04 09:26:27.469467 regain-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-04 09:26:17.000000 regain-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.461467 regain-0.3.9/regain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-04 09:26:17.000000 regain-0.3.9/regain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.461467 regain-0.3.9/regain/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-04 09:26:17.000000 regain-0.3.9/regain/bayesian/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3427 2023-07-04 09:26:17.000000 regain-0.3.9/regain/bayesian/_laplace_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-04 09:26:17.000000 regain-0.3.9/regain/bayesian/gaussian_process_.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15902 2023-07-04 09:26:17.000000 regain-0.3.9/regain/bayesian/gwishart_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-07-04 09:26:17.000000 regain-0.3.9/regain/bayesian/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-04 09:26:17.000000 regain-0.3.9/regain/bayesian/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8907 2023-07-04 09:26:17.000000 regain-0.3.9/regain/bayesian/wishart_distribution_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-04 09:26:17.000000 regain-0.3.9/regain/bayesian/wishart_process_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-04 09:26:17.000000 regain-0.3.9/regain/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.465467 regain-0.3.9/regain/covariance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/infimal_convolution_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30722 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/kernel_latent_time_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27854 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/kernel_time_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/latent_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/latent_time_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/latent_time_matrix_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/missing_graphical_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-07-04 09:26:17.000000 regain-0.3.9/regain/covariance/time_graphical_lasso_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.465467 regain-0.3.9/regain/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-04 09:26:17.000000 regain-0.3.9/regain/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-04 09:26:17.000000 regain-0.3.9/regain/data/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.465467 regain-0.3.9/regain/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-04 09:26:17.000000 regain-0.3.9/regain/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-07-04 09:26:17.000000 regain-0.3.9/regain/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23461 2023-07-04 09:26:17.000000 regain-0.3.9/regain/datasets/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-04 09:26:17.000000 regain-0.3.9/regain/datasets/ising.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-07-04 09:26:17.000000 regain-0.3.9/regain/datasets/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-07-04 09:26:17.000000 regain-0.3.9/regain/datasets/multi_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-04 09:26:17.000000 regain-0.3.9/regain/datasets/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-04 09:26:17.000000 regain-0.3.9/regain/discriminant_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.465467 regain-0.3.9/regain/forward_backward/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-04 09:26:17.000000 regain-0.3.9/regain/forward_backward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-07-04 09:26:17.000000 regain-0.3.9/regain/forward_backward/forward_backward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-04 09:26:17.000000 regain-0.3.9/regain/forward_backward/time_graphical_lasso_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.465467 regain-0.3.9/regain/generalized_linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:17.000000 regain-0.3.9/regain/generalized_linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-04 09:26:17.000000 regain-0.3.9/regain/generalized_linear_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-04 09:26:17.000000 regain-0.3.9/regain/generalized_linear_model/glm_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-04 09:26:17.000000 regain-0.3.9/regain/generalized_linear_model/glm_ising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-07-04 09:26:17.000000 regain-0.3.9/regain/generalized_linear_model/glm_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-07-04 09:26:17.000000 regain-0.3.9/regain/generalized_linear_model/glm_time_ising.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26767 2023-07-04 09:26:17.000000 regain-0.3.9/regain/generalized_linear_model/glm_time_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.465467 regain-0.3.9/regain/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-04 09:26:17.000000 regain-0.3.9/regain/linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-04 09:26:17.000000 regain-0.3.9/regain/linear_model/_group_lasso_overlap_old_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-04 09:26:17.000000 regain-0.3.9/regain/linear_model/group_lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-07-04 09:26:17.000000 regain-0.3.9/regain/linear_model/group_lasso_overlap_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-04 09:26:17.000000 regain-0.3.9/regain/linear_model/lasso_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-04 09:26:17.000000 regain-0.3.9/regain/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.469467 regain-0.3.9/regain/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-04 09:26:17.000000 regain-0.3.9/regain/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-07-04 09:26:17.000000 regain-0.3.9/regain/model_selection/_bayesian_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27777 2023-07-04 09:26:17.000000 regain-0.3.9/regain/model_selection/stability_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-04 09:26:17.000000 regain-0.3.9/regain/norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.469467 regain-0.3.9/regain/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-04 09:26:17.000000 regain-0.3.9/regain/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-04 09:26:17.000000 regain-0.3.9/regain/plotting/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-04 09:26:17.000000 regain-0.3.9/regain/plotting/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-04 09:26:17.000000 regain-0.3.9/regain/plotting/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-07-04 09:26:17.000000 regain-0.3.9/regain/plotting/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-04 09:26:17.000000 regain-0.3.9/regain/prox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-04 09:26:17.000000 regain-0.3.9/regain/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-04 09:26:17.000000 regain-0.3.9/regain/update_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-07-04 09:26:17.000000 regain-0.3.9/regain/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-04 09:26:17.000000 regain-0.3.9/regain/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.469467 regain-0.3.9/regain/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-04 09:26:17.000000 regain-0.3.9/regain/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.469467 regain-0.3.9/regain/wrapper/paspal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:17.000000 regain-0.3.9/regain/wrapper/paspal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-04 09:26:17.000000 regain-0.3.9/regain/wrapper/paspal/glopridu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:26:27.461467 regain-0.3.9/regain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-04 09:26:27.000000 regain-0.3.9/regain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-04 09:26:27.000000 regain-0.3.9/regain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:26:27.000000 regain-0.3.9/regain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 09:26:27.000000 regain-0.3.9/regain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-04 09:26:27.469467 regain-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-04 09:26:17.000000 regain-0.3.9/setup.py
```

### Comparing `regain-0.3.8/LICENSE` & `regain-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/PKG-INFO` & `regain-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: regain
-Version: 0.3.8
+Version: 0.3.9
 Summary: REGAIN (Regularised Graph Inference)
 Home-page: https://github.com/fdtomasi/regain
-Download-URL: https://github.com/fdtomasi/regain/archive/v0.3.8.tar.gz
+Download-URL: https://github.com/fdtomasi/regain/archive/v0.3.9.tar.gz
 Author: Federico Tomasi
 Author-email: fdtomasi@gmail.com
 Maintainer: Federico Tomasi
 Maintainer-email: fdtomasi@gmail.com
 License: FreeBSD
 Keywords: graph inference,latent variables
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,16 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
 
-[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
+![build](https://github.com/fdtomasi/regain/actions/workflows/python-package.yml/badge.svg)
+[![codecov](https://codecov.io/gh/fdtomasi/regain/branch/master/graph/badge.svg?token=1eLrec0OsI)](https://codecov.io/gh/fdtomasi/regain) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
 
 # regain
 Regularised graph inference across multiple time stamps, considering the influence of latent variables.
 It inherits functionalities from the [scikit-learn](https://github.com/scikit-learn/scikit-learn) package.
 
 ## Getting started
 ### Dependencies
```

### Comparing `regain-0.3.8/README.md` & `regain-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
+![build](https://github.com/fdtomasi/regain/actions/workflows/python-package.yml/badge.svg)
+[![codecov](https://codecov.io/gh/fdtomasi/regain/branch/master/graph/badge.svg?token=1eLrec0OsI)](https://codecov.io/gh/fdtomasi/regain) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
 
 # regain
 Regularised graph inference across multiple time stamps, considering the influence of latent variables.
 It inherits functionalities from the [scikit-learn](https://github.com/scikit-learn/scikit-learn) package.
 
 ## Getting started
 ### Dependencies
```

### Comparing `regain-0.3.8/regain/__init__.py` & `regain-0.3.9/regain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `regain-0.3.8/regain/bayesian/__init__.py` & `regain-0.3.9/regain/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/bayesian/_laplace_approximation.py` & `regain-0.3.9/regain/bayesian/_laplace_approximation.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/bayesian/gaussian_process_.py` & `regain-0.3.9/regain/bayesian/gaussian_process_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/bayesian/gwishart_inference.py` & `regain-0.3.9/regain/bayesian/gwishart_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,30 @@
 from functools import partial
 
 import numpy as np
 from numpy import binary_repr
 from scipy import linalg
 from scipy.optimize import minimize
 from scipy.special import comb
-from sklearn.covariance import empirical_covariance
-from sklearn.covariance.empirical_covariance_ import log_likelihood
+from sklearn.covariance import empirical_covariance, log_likelihood
 from sklearn.linear_model import LassoLars
 from sklearn.utils import Bunch, check_array
 from sklearn.utils.extmath import fast_logdet
 
 from regain.covariance.graphical_lasso_ import GraphicalLasso, graphical_lasso
 
 
 def mk_all_ugs(n_dim):
     """Utility for generating all possible graphs."""
     nedges = int(comb(n_dim, 2))
-    m = 2 ** nedges
+    m = 2**nedges
 
-    ind = np.array([list(binary_repr(x, width=len(binary_repr(m - 1)))) for x in range(m)]).astype(int)
+    ind = np.array(
+        [list(binary_repr(x, width=len(binary_repr(m - 1)))) for x in range(m)]
+    ).astype(int)
     ord = np.argsort(ind.sum(axis=1))
     ind = ind[ord]
 
     ut = np.triu(np.ones((n_dim, n_dim)), 1) > 0
 
     Gs = []
     for i in range(m):
@@ -94,26 +95,36 @@
         scores = []
         for j, mb in enumerate(mb_i):
             X_mb = X[:, mb]
             if X_mb.shape[1] < 1:
                 X_mb = np.zeros((X.shape[0], 1))
 
             y_mb = X[:, i]
-            score = np.sum([LassoLars(alpha=alpha).fit(X_mb, y_mb).score(X_mb, y_mb) for alpha in alphas])
+            score = np.sum(
+                [
+                    LassoLars(alpha=alpha).fit(X_mb, y_mb).score(X_mb, y_mb)
+                    for alpha in alphas
+                ]
+            )
 
             scores.append(score)
         scores_all.append(scores)
 
     ss = np.exp(np.array(scores_all))
     normalized_scores = ss / np.repeat(ss.sum(axis=1)[:, None], ss.shape[1], axis=1)
     return normalized_scores
 
 
 def _get_graphs(blankets, scores, n_dim, n_resampling=200):
-    idx = np.array([np.random.choice(scores.shape[1], p=scores[i], size=n_resampling) for i in range(n_dim)])
+    idx = np.array(
+        [
+            np.random.choice(scores.shape[1], p=scores[i], size=n_resampling)
+            for i in range(n_dim)
+        ]
+    )
 
     graphs_ = np.array([blankets[i][idx[i]] for i in range(n_dim)]).transpose(1, 0, 2)
     # symmetrise with AND operator -> product
     graphs = np.array([g * g.T for g in graphs_])
     return graphs
 
 
@@ -264,15 +275,19 @@
             tmp2 = A[0, :].dot(B[:, 0]) + A[1, :].dot(B[:, 1])
 
             diagH[e1] = -(dn - 2) * tmp2 / 2
             # diagH(e1) = -(dn-2) * trace(M1(nz2,nz1)*M2(nz1,nz2))/2;
 
         logdetHdiag = sum(np.log(-diagH))
         lognormconst = dof * np.log(2 * np.pi) / 2 + logh - logdetHdiag / 2.0
-        score = lognormconst - GWprior.lognormconst - n_samples * n_dim * np.log(2 * np.pi) / 2
+        score = (
+            lognormconst
+            - GWprior.lognormconst
+            - n_samples * n_dim * np.log(2 * np.pi) / 2
+        )
         GWpost.lognormconst = lognormconst
 
     elif score_method == "laplace":
         # Full laplace approximation
         H = np.empty((dof, dof))
         for e1 in range(dof):
             # nz1 = [Vi[e1], Vj[e1]]
@@ -290,15 +305,19 @@
                 # tmp2 = np.trace(A.dot(B))
                 tmp2 = (A * B.T).sum()
                 H[e2, e1] = H[e1, e2] = -(dn - 2) * tmp2 / 2.0
 
         # neg Hessian will be posdef
         logdetH = 2 * sum(np.log(np.diag(linalg.cholesky(-H))))
         lognormconst = dof * np.log(2 * np.pi) / 2 + logh - logdetH / 2.0
-        score = lognormconst - GWprior.lognormconst - n_samples * n_dim * np.log(2 * np.pi) / 2
+        score = (
+            lognormconst
+            - GWprior.lognormconst
+            - n_samples * n_dim * np.log(2 * np.pi) / 2
+        )
         GWpost.lognormconst = lognormconst
 
     GWpost.score = score
     return GWpost
 
 
 def GWishartScore(X, G, d0=3, S0=None, score_method="bic", mode="covsel"):
@@ -311,15 +330,17 @@
     GWprior = Bunch(d0=d0, S0=S0, lognormconst=0, lognormconstDiag=0)
 
     # %If method is laplace, compute laplace approximation to denominator
     if score_method in ["laplace", "diaglaplace"]:
         noData = np.zeros((0, n_dim))
 
         P0, S_noData = GWishartFit(noData, G, GWprior)
-        GWtemp = compute_score(noData, G, P0, S_noData, GWprior=GWprior, score_method=score_method)
+        GWtemp = compute_score(
+            noData, G, P0, S_noData, GWprior=GWprior, score_method=score_method
+        )
         GWprior.lognormconst = GWtemp.lognormconst
 
     # Compute the map precision matrix P
     P, S = GWishartFit(X, G, GWprior, mode=mode)
 
     # Compute the score
     GWpost = compute_score(X, G, P, S, GWprior, score_method)
@@ -340,32 +361,39 @@
     """Bayesian graphical lasso."""
     n_samples, n_dim = X.shape
 
     if alphas is None:
         alphas = np.logspace(-2, 0, 20)
 
     # get a series of Markov blankets for vaiours alphas
-    mdl = GraphicalLasso(assume_centered=assume_centered, tol=tol, max_iter=max_iter, verbose=False)
+    mdl = GraphicalLasso(
+        assume_centered=assume_centered, tol=tol, max_iter=max_iter, verbose=False
+    )
     precisions = [mdl.set_params(alpha=a).fit(X).precision_ for a in alphas]
     mblankets = markov_blankets(precisions, tol=tol, unique=True)
 
     normalized_scores = score_blankets(mblankets, X=X, alphas=[0.01, 0.5, 1])
 
-    graphs = _get_graphs(mblankets, normalized_scores, n_dim=n_dim, n_resampling=n_resampling)
+    graphs = _get_graphs(
+        mblankets, normalized_scores, n_dim=n_dim, n_resampling=n_resampling
+    )
 
     nonzeros_all = [np.triu(g, 1) + np.eye(n_dim, dtype=bool) for g in graphs]
 
     # Roverato'02: convert from HIW to G-Wishart (delta + |V| - 1)
     d0 = 3 + n_dim - 1
     S0 = np.eye(n_dim)  # same as Roverato'02
 
     # Find non-zero elements of upper triangle of G
     # make sure diagonal is non-zero
     # G = nonzeros_all[1] # probably can discard if all zeros?
-    res = [GWishartScore(X, G, d0=d0, S0=S0, mode=mode, score_method=scoring) for G in nonzeros_all]
+    res = [
+        GWishartScore(X, G, d0=d0, S0=S0, mode=mode, score_method=scoring)
+        for G in nonzeros_all
+    ]
 
     top_n = [x.P for x in sorted(res, key=lambda x: x.score)[::-1][:top_n]]
     return np.mean(top_n, axis=0)
 
 
 class BayesianGraphicalLasso(GraphicalLasso):
     """Sparse inverse covariance estimation with an l1-penalized estimator.
@@ -435,15 +463,20 @@
         verbose=False,
         assume_centered=False,
         mode="gl",
         scoring="diaglaplace",
         top_n=1,
     ):
         super(GraphicalLasso, self).__init__(
-            alpha=alpha, tol=tol, max_iter=max_iter, verbose=verbose, assume_centered=assume_centered, mode=mode
+            alpha=alpha,
+            tol=tol,
+            max_iter=max_iter,
+            verbose=verbose,
+            assume_centered=assume_centered,
+            mode=mode,
         )
         self.alphas = alphas
         self.n_resampling = n_resampling
         self.scoring = scoring
         self.top_n = top_n
 
     def fit(self, X, y=None):
```

### Comparing `regain-0.3.8/regain/bayesian/sampling.py` & `regain-0.3.9/regain/bayesian/sampling.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/bayesian/stats.py` & `regain-0.3.9/regain/bayesian/stats.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/bayesian/wishart_distribution_.py` & `regain-0.3.9/regain/bayesian/wishart_distribution_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/bayesian/wishart_process_.py` & `regain-0.3.9/regain/bayesian/wishart_process_.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,27 @@
 from __future__ import print_function
 
 from functools import partial
 
 import numpy as np
 from scipy import linalg, stats
 from sklearn.covariance import empirical_covariance
-from sklearn.datasets.base import Bunch
 from sklearn.gaussian_process import kernels
 from sklearn.metrics.pairwise import rbf_kernel
+from sklearn.utils import Bunch
 from sklearn.utils.validation import check_X_y
 from tqdm import trange
 
 from regain.bayesian.gaussian_process_ import sample as sample_gp
-from regain.bayesian.sampling import GWP_construct, elliptical_slice, sample_ell, sample_hyper_kernel
+from regain.bayesian.sampling import (
+    GWP_construct,
+    elliptical_slice,
+    sample_ell,
+    sample_hyper_kernel,
+)
 from regain.bayesian.stats import lognstat, t_mvn_logpdf
 from regain.covariance.time_graphical_lasso_ import TimeGraphicalLasso
 
 
 def fit(
     theta,
     var_prop,
@@ -105,37 +110,51 @@
         # We first do ESS to obtain a new sample for u
         pbar.set_description("loss: {:.3e}".format(current_state.log_likelihood))
 
         current_state = elliptical_slice(current_state, umat, likelihood=likelihood)
 
         # We now do MH for sampling the hyperparameter of the kernel
         theta, accept = sample_hyper_kernel(
-            theta, var_prop, np.vstack(current_state.xx), kern, prior_distr=prior_theta_kernel
+            theta,
+            var_prop,
+            np.vstack(current_state.xx),
+            kern,
+            prior_distr=prior_theta_kernel,
         )
 
         if accept:
             # new kernel parameter, recompute
             K = kern(inverse_width=theta)
             while True:
                 try:
                     umat = sample_gp(K, nu=nu, p=p)
                     break
                 except Exception:
                     K += 1e-8 * np.eye(K.shape[0])
 
             current_state["xx"] = umat
-            current_state["log_likelihood"] = likelihood(GWP_construct(umat, current_state["L"]))
+            current_state["log_likelihood"] = likelihood(
+                GWP_construct(umat, current_state["L"])
+            )
 
         # We now do MH for sampling the elements in the matrix L
         # spherical normal prior, element uncorrelated
         if learn_ell:
-            Ltau = sample_ell(Ltau, var_Lprop, current_state.xx, prior_distr=prior_ell, likelihood=likelihood)
+            Ltau = sample_ell(
+                Ltau,
+                var_Lprop,
+                current_state.xx,
+                prior_distr=prior_ell,
+                likelihood=likelihood,
+            )
             L__[np.tril_indices_from(L__)] = Ltau
             current_state["L"] = L__
-            current_state["log_likelihood"] = likelihood(GWP_construct(current_state["xx"], current_state["L"]))
+            current_state["log_likelihood"] = likelihood(
+                GWP_construct(current_state["xx"], current_state["L"])
+            )
 
         samples_u.append(current_state.xx)
         loglikes[i] = current_state.log_likelihood
         lps[i] = theta
         if learn_ell:
             Ls.append(L__)
     return_list = [samples_u, loglikes, lps]
@@ -233,42 +252,54 @@
         self.var_Lprop = var_Lprop
         # self.mu_Lprior = mu_Lprior
         # self.var_Lprior = var_Lprior
         self.kernel = kernel
         self.learn_ell = learn_ell
 
         mu_prior, sigma_prior = lognstat(mu_prior, var_prior)
-        self.prior_theta_kernel = stats.lognorm(loc=0, s=sigma_prior, scale=np.exp(mu_prior))
+        self.prior_theta_kernel = stats.lognorm(
+            loc=0, s=sigma_prior, scale=np.exp(mu_prior)
+        )
         self.prior_ell = stats.norm(loc=mu_Lprior, scale=np.sqrt(var_Lprior))
 
     def fit(self, X, y):
         """Fit the WishartProcess model to X.
 
         Parameters
         ----------
         X : ndarray, shape = (n_samples * n_times, n_dimensions)
             Data matrix.
         y : ndarray, shape = (n_times,)
             Indicate the temporal belonging of each matrix.
         """
         # Covariance does not make sense for a single feature
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         n_dimensions = X.shape[1]
         self.classes_, n_samples = np.unique(y, return_counts=True)
         n_times = self.classes_.size
 
         # n_samples = np.array([x.shape[0] for x in X])
         if self.assume_centered:
             self.location_ = np.zeros((n_times, n_dimensions))
         else:
             self.location_ = np.array([X[y == cl].mean(0) for cl in self.classes_])
 
         # X = (X - self.location_).transpose(1, 2, 0)  # put time last
-        X_center = [X[y == cl] - self.location_[i] for i, cl in enumerate(self.classes_)]
+        X_center = [
+            X[y == cl] - self.location_[i] for i, cl in enumerate(self.classes_)
+        ]
         if self.kernel is None or self.kernel.lower() == "rbf":
             kern = partial(_rbf_kernel, var=1)
         else:
             kern = _periodic_kernel
 
         self.likelihood = partial(t_mvn_logpdf, X_center)
         self.nu_ = 1
@@ -298,25 +329,25 @@
 
         if self.learn_ell:
             samples_u, loglikes, lps, Ls = out
         else:
             samples_u, loglikes, lps = out
 
         # Burn in
-        self.lps_after_burnin = lps[self.burn_in :]
-        self.samples_u_after_burnin = samples_u[self.burn_in :]
-        self.loglikes_after_burnin = loglikes[self.burn_in :]
+        self.lps_after_burnin = lps[self.burn_in:]
+        self.samples_u_after_burnin = samples_u[self.burn_in:]
+        self.loglikes_after_burnin = loglikes[self.burn_in:]
 
         # % Select the best hyperparameters based on the loglikes_after_burnin
         pos = np.argmax(self.loglikes_after_burnin)
         self.lmap = self.lps_after_burnin[pos]
         self.u_map = self.samples_u_after_burnin[pos]
 
         if self.learn_ell:
-            self.Ls_after_burnin = Ls[self.burn_in :]
+            self.Ls_after_burnin = Ls[self.burn_in:]
             self.Lmap = self.Ls_after_burnin[pos]
         else:
             self.Lmap = L
 
         self.D_map = GWP_construct(self.u_map, self.Lmap)
 
         # compatibility with sklearn
@@ -342,12 +373,22 @@
         -------
         res : float
             The likelihood of the data set with `self.covariance_` as an
             estimator of its covariance matrix.
 
         """
         # Covariance does not make sense for a single feature
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
-        X_center = np.array([X[y == cl] - self.location_[i] for i, cl in enumerate(self.classes_)])
+        X_center = np.array(
+            [X[y == cl] - self.location_[i] for i, cl in enumerate(self.classes_)]
+        )
         logp = t_mvn_logpdf(X_center, self.D_map)
         return logp
```

### Comparing `regain-0.3.8/regain/clustering.py` & `regain-0.3.9/regain/clustering.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/covariance/__init__.py` & `regain-0.3.9/regain/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/covariance/graphical_lasso_.py` & `regain-0.3.9/regain/covariance/graphical_lasso_.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,31 +28,27 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Sparse inverse covariance selection via ADMM.
 
 More information can be found in the paper linked at:
 http://www.stanford.edu/~boyd/papers/distr_opt_stat_learning_admm.html
 """
-from __future__ import division
-
 import warnings
 
 import numpy as np
 from scipy import linalg
 from six.moves import range
-from sklearn.covariance import GraphicalLasso as GraphLasso
-from sklearn.covariance import empirical_covariance
+from sklearn.covariance import GraphicalLasso as GraphLasso, empirical_covariance
 from sklearn.utils.extmath import fast_logdet
 from sklearn.utils.validation import check_array
 
 from regain.norm import l1_od_norm
-from regain.prox import prox_logdet, soft_thresholding_od
+from regain.prox import prox_logdet, soft_thresholding_off_diagonal
 from regain.update_rules import update_rho
-from regain.utils import convergence
-
+from regain.utils import Convergence
 
 
 def logl(emp_cov, precision):
     """Gaussian log-likelihood without constant term."""
     return fast_logdet(precision) - np.sum(emp_cov * precision)
 
 
@@ -160,40 +156,43 @@
         A = Z - U
         A += A.T
         A /= 2.0
         K = prox_logdet(emp_cov - rho * A, lamda=1.0 / rho)
 
         # z-update with relaxation
         K_hat = over_relax * K - (1 - over_relax) * Z
-        Z = soft_thresholding_od(K_hat + U, lamda=alpha / rho)
+        Z = soft_thresholding_off_diagonal(K_hat + U, lamda=alpha / rho)
 
         # update residuals
         U += K_hat - Z
 
         # diagnostics, reporting, termination checks
         obj = objective(emp_cov, K, Z, alpha) if compute_objective else np.nan
         rnorm = np.linalg.norm(K - Z, "fro")
         snorm = rho * np.linalg.norm(Z - Z_old, "fro")
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
-            e_pri=np.sqrt(K.size) * tol + rtol * max(np.linalg.norm(K, "fro"), np.linalg.norm(Z, "fro")),
+            e_pri=np.sqrt(K.size) * tol
+            + rtol * max(np.linalg.norm(K, "fro"), np.linalg.norm(Z, "fro")),
             e_dual=np.sqrt(K.size) * tol + rtol * rho * np.linalg.norm(U),
         )
 
         Z_old = Z.copy()
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(check)
 
         checks.append(check)
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         U *= rho / rho_new
         rho = rho_new
     else:
         warnings.warn("Objective did not converge.")
 
     return_list = [Z, emp_cov]
@@ -274,15 +273,20 @@
         verbose=False,
         assume_centered=False,
         update_rho_options=None,
         compute_objective=True,
         init="empirical",
     ):
         super(GraphicalLasso, self).__init__(
-            alpha=alpha, tol=tol, max_iter=max_iter, verbose=verbose, assume_centered=assume_centered, mode=mode
+            alpha=alpha,
+            tol=tol,
+            max_iter=max_iter,
+            verbose=verbose,
+            assume_centered=assume_centered,
+            mode=mode,
         )
         self.rho = rho
         self.rtol = rtol
         self.over_relax = over_relax
         self.update_rho_options = update_rho_options
         self.compute_objective = compute_objective
         self.init = init
```

### Comparing `regain-0.3.8/regain/covariance/infimal_convolution_.py` & `regain-0.3.9/regain/covariance/infimal_convolution_.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from scipy import linalg
 from six.moves import range
 from sklearn.utils.extmath import squared_norm
 
 from regain.norm import l1_od_norm
 from regain.prox import prox_laplacian, prox_trace_indicator, soft_thresholding
 from regain.update_rules import update_rho
-from regain.utils import convergence
+from regain.utils import Convergence
 
 
 def objective(S, R, K, L, alpha, tau):
     """Objective function for latent graphical lasso."""
     obj = 0.5 * squared_norm(S - R)
     obj += alpha * l1_od_norm(K)
     obj += tau * np.linalg.norm(L, ord="nuc")
@@ -132,32 +132,35 @@
         # update residuals
         U += R - K + L
 
         # diagnostics, reporting, termination checks
         obj = objective(S, R, K, L, alpha, tau) if compute_objective else np.nan
         rnorm = np.linalg.norm(R - K + L)
         snorm = rho * np.linalg.norm(R - R_old)
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
-            e_pri=np.sqrt(R.size) * tol + rtol * max(np.linalg.norm(R), np.linalg.norm(K - L)),
+            e_pri=np.sqrt(R.size) * tol
+            + rtol * max(np.linalg.norm(R), np.linalg.norm(K - L)),
             e_dual=np.sqrt(R.size) * tol + rtol * rho * np.linalg.norm(U),
         )
         R_old = R.copy()
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(check)
 
         checks.append(check)
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
         if check.obj == np.inf:
             break
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         U *= rho / rho_new
         rho = rho_new
     else:
         warnings.warn("Objective did not converge.")
 
     covariance_ = linalg.pinvh(K)
```

### Comparing `regain-0.3.8/regain/covariance/kernel_latent_time_graphical_lasso_.py` & `regain-0.3.9/regain/covariance/kernel_latent_time_graphical_lasso_.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,48 +28,45 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Graphical latent variable models selection over time via ADMM.
 
 This adds the possibility to specify a temporal constraint with a kernel
 function.
 """
-from __future__ import division
-
 import warnings
-from functools import partial
 
 import numpy as np
 from scipy import linalg
-from six.moves import map, range, zip
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.gaussian_process import kernels
 from sklearn.utils.extmath import squared_norm
 from sklearn.utils.validation import check_is_fitted
 
 from regain.covariance.kernel_time_graphical_lasso_ import (
     KernelTimeGraphicalLasso,
     init_precision,
     objective as obj_ktgl,
     precision_similarity,
 )
 from regain.prox import prox_logdet, prox_trace_indicator, soft_thresholding
 from regain.update_rules import update_rho
-from regain.utils import convergence
+from regain.utils import Convergence
 from regain.validation import check_norm_prox
 
 
 def objective(
     S, n_samples, R, Z_0, Z_M, W_0, W_M, alpha, tau, kernel_psi, kernel_phi, psi, phi
 ):
     """Objective function for latent variable time-varying graphical lasso."""
     obj = obj_ktgl(n_samples, S, R, Z_0, Z_M, alpha, kernel_psi, psi)
+
     if isinstance(tau, np.ndarray):
-        obj += sum(np.linalg.norm(t * w, ord="nuc") for t, w in zip(tau, W_0))
+        obj += np.sum(np.linalg.norm(tau * W_0, ord="nuc", axis=(-2, -1)))
     else:
-        obj += tau * sum(map(partial(np.linalg.norm, ord="nuc"), W_0))
+        obj += tau * np.sum(np.linalg.norm(W_0, ord="nuc", axis=(-2, -1)))
 
     for m in range(1, W_0.shape[0]):
         # all possible markovians jumps
         W_L, W_R = W_M[m]
         obj += np.sum(np.array(list(map(phi, W_R - W_L))) * np.diag(kernel_phi, m))
 
     return obj
@@ -187,15 +184,16 @@
         A = Z_0 - W_0 - X_0
         A += A.transpose(0, 2, 1)
         A /= 2.0
         A *= -rho / n_samples[:, None, None]
         A += emp_cov
         # A = emp_cov / rho - A
 
-        R = np.array([prox_logdet(a, lamda=ni / rho) for a, ni in zip(A, n_samples)])
+        lamda = np.expand_dims(n_samples / rho, -1)
+        R = prox_logdet(A, lamda=lamda)
 
         # update Z_0
         A = R + W_0 + X_0
         for m in range(1, n_times):
             A[:-m] += Z_M[m][0] - Y_M[m][0]
             A[m:] += Z_M[m][1] - Y_M[m][1]
 
@@ -309,15 +307,15 @@
                 psi,
                 phi,
             )
             if compute_objective
             else np.nan
         )
 
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=n_features * np.sqrt(n_times * (2 * n_times - 1)) * tol
             + rtol
             * max(
                 np.sqrt(
@@ -358,18 +356,15 @@
 
         R_old = R.copy()
         for m in range(1, n_times):
             Z_M_old[m] = (Z_M[m][0].copy(), Z_M[m][1].copy())
             W_M_old[m] = (W_M[m][0].copy(), W_M[m][1].copy())
 
         if verbose:
-            print(
-                "obj: %.4f, rnorm: %.4f, snorm: %.4f,"
-                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
-            )
+            print(check)
 
         checks.append(check)
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
         rho_new = update_rho(
             rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
@@ -534,15 +529,15 @@
             except TypeError:
                 # maybe it's a ConstantKernel
                 kernel_phi = self.kernel_phi(constant_value=self.ker_phi_param)(
                     self.classes_[:, None]
                 )
 
         else:
-            kernel_phi = self.kernel_phi
+            kernel_phi = self.kernel_phi or np.identity(self.classes_.size)
             if kernel_phi.shape[0] != self.classes_.size:
                 raise ValueError(
                     "kernel_phi size does not match classes of samples, "
                     "got {} classes and kernel_phi has shape {}".format(
                         self.classes_.size, kernel_phi.shape[0]
                     )
                 )
@@ -554,15 +549,15 @@
                 )
             except TypeError:
                 # maybe it's a ConstantKernel
                 kernel_psi = self.kernel_psi(constant_value=self.ker_psi_param)(
                     self.classes_[:, None]
                 )
         else:
-            kernel_psi = self.kernel_psi
+            kernel_psi = self.kernel_psi or np.identity(self.classes_.size)
             if kernel_psi.shape[0] != self.classes_.size:
                 raise ValueError(
                     "kernel_psi size does not match classes of samples, "
                     "got {} classes and kernel_psi has shape {}".format(
                         self.classes_.size, kernel_psi.shape[0]
                     )
                 )
```

### Comparing `regain-0.3.8/regain/covariance/kernel_time_graphical_lasso_.py` & `regain-0.3.9/regain/covariance/kernel_time_graphical_lasso_.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,47 +28,47 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Sparse inverse covariance selection over time via ADMM.
 
 This adds the possibility to specify a temporal constraint with a kernel
 function.
 """
-from __future__ import division
-
 import warnings
 
 import numpy as np
 from scipy import linalg
-from six.moves import map, range, zip
+from six.moves import map, range
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.gaussian_process import kernels
 from sklearn.utils.extmath import squared_norm
 from sklearn.utils.validation import check_is_fitted
 
 from regain.covariance.time_graphical_lasso_ import (
     TimeGraphicalLasso,
     init_precision,
     loss,
 )
 from regain.norm import l1_od_norm
 from regain.prox import prox_logdet, soft_thresholding
 from regain.update_rules import update_rho
-from regain.utils import convergence
+from regain.utils import Convergence
 from regain.validation import check_norm_prox
 
+
 # from regain.clustering import graph_k_means
 
 
 def objective(n_samples, S, K, Z_0, Z_M, alpha, kernel, psi):
     """Objective function for time-varying graphical lasso."""
     obj = loss(S, K, n_samples=n_samples)
+
     if isinstance(alpha, np.ndarray):
-        obj += sum(l1_od_norm(a * z) for a, z in zip(alpha, Z_0))
+        obj += np.sum(l1_od_norm(alpha * Z_0))
     else:
-        obj += alpha * sum(map(l1_od_norm, Z_0))
+        obj += alpha * np.sum(l1_od_norm(Z_0))
 
     for m in range(1, Z_0.shape[0]):
         # all possible markovians jumps
         Z_L, Z_R = Z_M[m]
         obj += np.sum(np.array(list(map(psi, Z_R - Z_L))) * np.diag(kernel, m))
 
     return obj
@@ -159,15 +159,15 @@
         Z_R_old = np.zeros_like(Z_R)
         Z_M_old[m] = (Z_L_old, Z_R_old)
 
     if n_samples is None:
         n_samples = np.ones(n_times)
 
     checks = [
-        convergence(
+        Convergence(
             obj=objective(n_samples, emp_cov, Z_0, Z_0, Z_M, alpha, kernel, psi)
         )
     ]
     for iteration_ in range(max_iter):
         # update K
         A = Z_0 - U_0
         for m in range(1, n_times):
@@ -179,17 +179,16 @@
         # K = np.array(map(soft_thresholding_, A))
         A += A.transpose(0, 2, 1)
         A /= 2.0
 
         A *= -rho * n_times / n_samples[:, None, None]
         A += emp_cov
 
-        K = np.array(
-            [prox_logdet(a, lamda=ni / (rho * n_times)) for a, ni in zip(A, n_samples)]
-        )
+        lamda = np.expand_dims(n_samples / (rho * n_times), -1)
+        K = prox_logdet(A, lamda)
 
         # update Z_0
         A = K + U_0
         A += A.transpose(0, 2, 1)
         A /= 2.0
         Z_0 = soft_thresholding(A, lamda=alpha / rho)
 
@@ -242,15 +241,15 @@
 
         obj = (
             objective(n_samples, emp_cov, Z_0, K, Z_M, alpha, kernel, psi)
             if compute_objective
             else np.nan
         )
 
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=n_features * n_times * tol
             + rtol
             * max(
                 np.sqrt(
@@ -280,18 +279,15 @@
             ),
         )
         Z_0_old = Z_0.copy()
         for m in range(1, n_times):
             Z_M_old[m] = (Z_M[m][0].copy(), Z_M[m][1].copy())
 
         if verbose:
-            print(
-                "obj: %.4f, rnorm: %.4f, snorm: %.4f,"
-                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
-            )
+            print(check)
 
         checks.append(check)
         if stop_at is not None:
             if abs(check.obj - stop_at) / abs(stop_at) < stop_when:
                 break
 
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
@@ -544,15 +540,15 @@
                     )
                 except TypeError:
                     # maybe it's a ConstantKernel
                     kernel = self.kernel(constant_value=self.ker_param)(
                         self.classes_[:, None]
                     )
             else:
-                kernel = self.kernel
+                kernel = self.kernel or np.identity(self.classes_.size)
                 if kernel.shape[0] != self.classes_.size:
                     raise ValueError(
                         "Kernel size does not match classes of samples, "
                         "got {} classes and kernel has shape {}".format(
                             self.classes_.size, kernel.shape[0]
                         )
                     )
```

### Comparing `regain-0.3.8/regain/covariance/latent_graphical_lasso_.py` & `regain-0.3.9/regain/covariance/latent_graphical_lasso_.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 """Graphical latent variable model selection via ADMM."""
 from __future__ import division
 
 import warnings
 
 import numpy as np
 from scipy import linalg
-from six.moves import range
 
-from regain.covariance.graphical_lasso_ import GraphicalLasso, init_precision
-from regain.covariance.graphical_lasso_ import objective as obj_gl
+from regain.covariance.graphical_lasso_ import (
+    GraphicalLasso,
+    init_precision,
+    objective as obj_gl,
+)
 from regain.prox import prox_logdet, prox_trace_indicator, soft_thresholding
 from regain.update_rules import update_rho
-from regain.utils import convergence
+from regain.utils import Convergence
 
 
 def objective(emp_cov, R, K, L, alpha, tau):
     """Objective function for latent graphical lasso."""
     obj = obj_gl(emp_cov, R, K, alpha=alpha)
     obj += tau * np.linalg.norm(L, ord="nuc")
     return obj
@@ -140,32 +142,35 @@
         # update residuals
         U += R - K + L
 
         # diagnostics, reporting, termination checks
         obj = objective(emp_cov, R, K, L, alpha, tau) if compute_objective else np.nan
         rnorm = np.linalg.norm(R - K + L)
         snorm = rho * np.linalg.norm(R - R_old)
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
-            e_pri=np.sqrt(R.size) * tol + rtol * max(np.linalg.norm(R), np.linalg.norm(K - L)),
+            e_pri=np.sqrt(R.size) * tol
+            + rtol * max(np.linalg.norm(R), np.linalg.norm(K - L)),
             e_dual=np.sqrt(R.size) * tol + rtol * rho * np.linalg.norm(U),
         )
         R_old = R.copy()
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(check)
 
         checks.append(check)
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
         if check.obj == np.inf:
             break
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         U *= rho / rho_new
         rho = rho_new
     else:
         warnings.warn("Objective did not converge.")
 
     covariance_ = linalg.pinvh(K)
@@ -289,15 +294,20 @@
 
         Parameters
         ----------
         emp_cov : ndarray, shape (n_features, n_features)
             Empirical covariance of data.
 
         """
-        self.precision_, self.latent_, self.covariance_, self.n_iter_ = latent_graphical_lasso(
+        (
+            self.precision_,
+            self.latent_,
+            self.covariance_,
+            self.n_iter_,
+        ) = latent_graphical_lasso(
             emp_cov,
             alpha=self.alpha,
             tau=self.tau,
             rho=self.rho,
             tol=self.tol,
             rtol=self.rtol,
             max_iter=self.max_iter,
```

### Comparing `regain-0.3.8/regain/covariance/latent_time_graphical_lasso_.py` & `regain-0.3.9/regain/covariance/latent_time_graphical_lasso_.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,41 +24,41 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Graphical latent variable models selection over time via ADMM."""
-from __future__ import division
-
 import warnings
-from functools import partial
 
 import numpy as np
 from scipy import linalg
-from six.moves import map, range, zip
 from sklearn.utils.extmath import squared_norm
 
-from regain.covariance.time_graphical_lasso_ import TimeGraphicalLasso, init_precision
-from regain.covariance.time_graphical_lasso_ import objective as obj_tgl
+from regain.covariance.time_graphical_lasso_ import (
+    TimeGraphicalLasso,
+    init_precision,
+    objective as obj_tgl,
+)
 from regain.prox import prox_logdet, prox_trace_indicator, soft_thresholding
 from regain.update_rules import update_rho
-from regain.utils import convergence
+from regain.utils import Convergence
 from regain.validation import check_norm_prox
 
 
-def objective(S, n_samples, R, Z_0, Z_1, Z_2, W_0, W_1, W_2, alpha, tau, beta, eta, psi, phi):
+def objective(
+    emp_cov, n_samples, R, Z_0, Z_1, Z_2, W_0, W_1, W_2, alpha, tau, beta, eta, psi, phi
+):
     """Objective function for latent variable time-varying graphical lasso."""
-    # obj = sum(- n * logl(s, r) for s, r, n in zip(S, R, n_samples))
-    obj = obj_tgl(n_samples, S, R, Z_0, Z_1, Z_2, alpha, beta, psi)
+    obj = obj_tgl(n_samples, emp_cov, R, Z_0, Z_1, Z_2, alpha, beta, psi)
 
     if isinstance(tau, np.ndarray):
-        obj += sum(np.linalg.norm(t * w, ord="nuc") for t, w in zip(tau, W_0))
+        obj += np.sum(np.linalg.norm(tau * W_0, ord="nuc", axis=(-2, -1)))
     else:
-        obj += tau * sum(map(partial(np.linalg.norm, ord="nuc"), W_0))
+        obj += tau * np.sum(np.linalg.norm(W_0, ord="nuc", axis=(-2, -1)))
 
     if isinstance(eta, np.ndarray):
         obj += sum(b[0][0] * m for b, m in zip(eta, map(phi, W_2 - W_1)))
     else:
         obj += eta * sum(map(phi, W_2 - W_1))
     return obj
 
@@ -172,23 +172,22 @@
         A = Z_0 - W_0 - X_0
         A += A.transpose(0, 2, 1)
         A /= 2.0
         A *= -rho / n_samples[:, None, None]
         A += emp_cov
         # A = emp_cov / rho - A
 
-        R = np.array([prox_logdet(a, lamda=ni / rho) for a, ni in zip(A, n_samples)])
+        lamda = np.expand_dims(n_samples / rho, -1)
+        R = prox_logdet(A, lamda=lamda)
 
         # update Z_0
         A = R + W_0 + X_0
         A[:-1] += Z_1 - X_1
         A[1:] += Z_2 - X_2
         A /= divisor[:, None, None]
-        # soft_thresholding_ = partial(soft_thresholding, lamda=alpha / rho)
-        # Z_0 = np.array(map(soft_thresholding_, A))
         Z_0 = soft_thresholding(A, lamda=alpha / (rho * divisor[:, None, None]))
 
         # update Z_1, Z_2
         A_1 = Z_0[:-1] + X_1
         A_2 = Z_0[1:] + X_2
         if not psi_node_penalty:
             prox_e = prox_psi(A_2 - A_1, lamda=2.0 * beta / rho)
@@ -208,15 +207,16 @@
         A = Z_0 - R - X_0
         A[:-1] += W_1 - U_1
         A[1:] += W_2 - U_2
         A /= divisor[:, None, None]
         A += A.transpose(0, 2, 1)
         A /= 2.0
 
-        W_0 = np.array([prox_trace_indicator(a, lamda=tau / (rho * div)) for a, div in zip(A, divisor)])
+        lamda = np.expand_dims(tau / (rho * divisor), -1)
+        W_0 = prox_trace_indicator(A, lamda)
 
         # update W_1, W_2
         A_1 = W_0[:-1] + U_1
         A_2 = W_0[1:] + U_2
         if not phi_node_penalty:
             prox_e = prox_phi(A_2 - A_1, lamda=2.0 * eta / rho)
             W_1 = 0.5 * (A_1 + A_2 - prox_e)
@@ -252,61 +252,87 @@
             + squared_norm(Z_1 - Z_1_old)
             + squared_norm(Z_2 - Z_2_old)
             + squared_norm(W_1 - W_1_old)
             + squared_norm(W_2 - W_2_old)
         )
 
         obj = (
-            objective(emp_cov, n_samples, R, Z_0, Z_1, Z_2, W_0, W_1, W_2, alpha, tau, beta, eta, psi, phi)
+            objective(
+                emp_cov,
+                n_samples,
+                R,
+                Z_0,
+                Z_1,
+                Z_2,
+                W_0,
+                W_1,
+                W_2,
+                alpha,
+                tau,
+                beta,
+                eta,
+                psi,
+                phi,
+            )
             if compute_objective
             else np.nan
         )
 
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=np.sqrt(R.size + 4 * Z_1.size) * tol
             + rtol
             * max(
                 np.sqrt(
-                    squared_norm(R) + squared_norm(Z_1) + squared_norm(Z_2) + squared_norm(W_1) + squared_norm(W_2)
+                    squared_norm(R)
+                    + squared_norm(Z_1)
+                    + squared_norm(Z_2)
+                    + squared_norm(W_1)
+                    + squared_norm(W_2)
                 ),
                 np.sqrt(
                     squared_norm(Z_0 - W_0)
                     + squared_norm(Z_0[:-1])
                     + squared_norm(Z_0[1:])
                     + squared_norm(W_0[:-1])
                     + squared_norm(W_0[1:])
                 ),
             ),
             e_dual=np.sqrt(R.size + 4 * Z_1.size) * tol
             + rtol
             * rho
             * (
                 np.sqrt(
-                    squared_norm(X_0) + squared_norm(X_1) + squared_norm(X_2) + squared_norm(U_1) + squared_norm(U_2)
+                    squared_norm(X_0)
+                    + squared_norm(X_1)
+                    + squared_norm(X_2)
+                    + squared_norm(U_1)
+                    + squared_norm(U_2)
                 )
             ),
         )
 
         R_old = R.copy()
         Z_1_old = Z_1.copy()
         Z_2_old = Z_2.copy()
         W_1_old = W_1.copy()
         W_2_old = W_2.copy()
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(check)
 
         checks.append(check)
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         X_0 *= rho / rho_new
         X_1 *= rho / rho_new
         X_2 *= rho / rho_new
         U_1 *= rho / rho_new
         U_2 *= rho / rho_new
         rho = rho_new
@@ -459,15 +485,20 @@
 
         Parameters
         ----------
         emp_cov : ndarray, shape (n_features, n_features)
             Empirical covariance of data.
 
         """
-        self.precision_, self.latent_, self.covariance_, self.n_iter_ = latent_time_graphical_lasso(
+        (
+            self.precision_,
+            self.latent_,
+            self.covariance_,
+            self.n_iter_,
+        ) = latent_time_graphical_lasso(
             emp_cov,
             n_samples=n_samples,
             alpha=self.alpha,
             tau=self.tau,
             rho=self.rho,
             beta=self.beta,
             eta=self.eta,
```

### Comparing `regain-0.3.8/regain/covariance/latent_time_matrix_decomposition.py` & `regain-0.3.9/regain/covariance/latent_time_matrix_decomposition.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,33 +27,32 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Latent variable time-varying matrix decomposition using ADMM."""
 from __future__ import division
 
 import warnings
-from functools import partial
 
 import numpy as np
 from six.moves import map, range, zip
 from sklearn.utils.extmath import squared_norm
 
 from regain.covariance.latent_time_graphical_lasso_ import LatentTimeGraphicalLasso
 from regain.norm import l1_od_norm
 from regain.prox import prox_trace_indicator, soft_thresholding
 from regain.update_rules import update_rho
-from regain.utils import convergence
+from regain.utils import Convergence
 from regain.validation import check_input, check_norm_prox
 
 
 def objective(S, R, Z_0, Z_1, Z_2, W_0, W_1, W_2, alpha, tau, beta, eta, psi, phi):
     """Objective for latent variable time-varying matrix decomposition."""
     obj = squared_norm(S - R)
-    obj += alpha * sum(map(l1_od_norm, Z_0))
-    obj += tau * sum(map(partial(np.linalg.norm, ord="nuc"), W_0))
+    obj += alpha * np.sum(l1_od_norm(Z_0))
+    obj += tau * np.sum(np.linalg.norm(W_0, ord="nuc", axis=(-2, -1)))
     obj += beta * sum(map(psi, Z_2 - Z_1))
     obj += eta * sum(map(phi, W_2 - W_1))
     return obj
 
 
 def latent_time_matrix_decomposition(
     emp_cov,
@@ -175,15 +174,20 @@
         A = Z_0 - R - X_0
         A[:-1] += W_1 - U_1
         A[1:] += W_2 - U_2
         A /= divisor[:, None, None]
         A += A.transpose(0, 2, 1)
         A /= 2.0
 
-        W_0 = np.array([prox_trace_indicator(a, lamda=tau / (rho * div)) for a, div in zip(A, divisor)])
+        W_0 = np.array(
+            [
+                prox_trace_indicator(a, lamda=tau / (rho * div))
+                for a, div in zip(A, divisor)
+            ]
+        )
 
         # update W_1, W_2
         A_1 = W_0[:-1] + U_1
         A_2 = W_0[1:] + U_2
         if not phi_node_penalty:
             prox_e = prox_phi(A_2 - A_1, lamda=2.0 * eta / rho)
             W_1 = 0.5 * (A_1 + A_2 - prox_e)
@@ -219,61 +223,86 @@
             + squared_norm(Z_1 - Z_1_old)
             + squared_norm(Z_2 - Z_2_old)
             + squared_norm(W_1 - W_1_old)
             + squared_norm(W_2 - W_2_old)
         )
 
         obj = (
-            objective(emp_cov, R, Z_0, Z_1, Z_2, W_0, W_1, W_2, alpha, tau, beta, eta, psi, phi)
+            objective(
+                emp_cov,
+                R,
+                Z_0,
+                Z_1,
+                Z_2,
+                W_0,
+                W_1,
+                W_2,
+                alpha,
+                tau,
+                beta,
+                eta,
+                psi,
+                phi,
+            )
             if compute_objective
             else np.nan
         )
 
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=np.sqrt(R.size + 4 * Z_1.size) * tol
             + rtol
             * max(
                 np.sqrt(
-                    squared_norm(R) + squared_norm(Z_1) + squared_norm(Z_2) + squared_norm(W_1) + squared_norm(W_2)
+                    squared_norm(R)
+                    + squared_norm(Z_1)
+                    + squared_norm(Z_2)
+                    + squared_norm(W_1)
+                    + squared_norm(W_2)
                 ),
                 np.sqrt(
                     squared_norm(Z_0 - W_0)
                     + squared_norm(Z_0[:-1])
                     + squared_norm(Z_0[1:])
                     + squared_norm(W_0[:-1])
                     + squared_norm(W_0[1:])
                 ),
             ),
             e_dual=np.sqrt(R.size + 4 * Z_1.size) * tol
             + rtol
             * rho
             * (
                 np.sqrt(
-                    squared_norm(X_0) + squared_norm(X_1) + squared_norm(X_2) + squared_norm(U_1) + squared_norm(U_2)
+                    squared_norm(X_0)
+                    + squared_norm(X_1)
+                    + squared_norm(X_2)
+                    + squared_norm(U_1)
+                    + squared_norm(U_2)
                 )
             ),
         )
 
         R_old = R.copy()
         Z_1_old = Z_1.copy()
         Z_2_old = Z_2.copy()
         W_1_old = W_1.copy()
         W_2_old = W_2.copy()
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check)
+            print(check)
 
         checks.append(check)
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         X_0 *= rho / rho_new
         X_1 *= rho / rho_new
         X_2 *= rho / rho_new
         U_1 *= rho / rho_new
         U_2 *= rho / rho_new
         rho = rho_new
```

### Comparing `regain-0.3.8/regain/covariance/missing_graphical_lasso_.py` & `regain-0.3.9/regain/covariance/missing_graphical_lasso_.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,30 +33,31 @@
 http://www.stanford.edu/~boyd/papers/distr_opt_stat_learning_admm.html
 """
 from __future__ import division
 
 import warnings
 
 import numpy as np
-from six.moves import range
 
 from regain.covariance.graphical_lasso_ import GraphicalLasso, graphical_lasso, logl
 
 
 def compute_empirical_covariance(X, K, cs):
     emp_cov = np.zeros((X.shape[0], K.shape[0], K.shape[0]))
     aux = np.nan_to_num(np.copy(X))
     aux += cs
     for i in range(X.shape[0]):
         for v in range(emp_cov.shape[1]):
             for s in range(emp_cov.shape[1]):
                 if np.isnan(X[i, v]) and np.isnan(X[i, s]):
                     nans = np.where(np.isnan(X[i, :]))[0]
                     xxm, yym = np.meshgrid(nans, nans)
-                    inv = np.linalg.pinv(K[xxm, yym])[np.where(nans == v)[0][0], np.where(nans == s)[0][0]]
+                    inv = np.linalg.pinv(K[xxm, yym])[
+                        np.where(nans == v)[0][0], np.where(nans == s)[0][0]
+                    ]
                     emp_cov[i, v, s] = inv + cs[i, v] * cs[i, s]
                 else:
                     emp_cov[i, v, s] = aux[i, v] * aux[i, s]
     emp_cov = np.sum(emp_cov, axis=0)
     return emp_cov / np.max(emp_cov)
 
 
@@ -172,15 +173,17 @@
             compute_objective=compute_objective,
             init=K,
         )
         loglik = logl(emp_cov, K)
         diff = old_logl - loglik
         checks.append(dict(iteration=iter_, log_likelihood=logl, difference=diff))
         if verbose:
-            print("Iter %d: log-likelihood %.4f, difference: %.4f" % (iter_, loglik, diff))
+            print(
+                "Iter %d: log-likelihood %.4f, difference: %.4f" % (iter_, loglik, diff)
+            )
         if np.abs(diff) < tol:
             break
     else:
         warnings.warn("The Missing Graphical Lasso algorithm did not converge")
     aux = np.nan_to_num(np.copy(X))
     aux += cs
     return_list = [K, emp_cov, aux]
@@ -292,15 +295,20 @@
         y : (ignored)
 
         """
         # Covariance does not make sense for a single feature
         # X = check_array(
         #     X, ensure_min_features=2, ensure_min_samples=2, estimator=self)
 
-        self.precision_, self.covariance_, self.complete_data_matrix_, self.n_iter_ = missing_graphical_lasso(
+        (
+            self.precision_,
+            self.covariance_,
+            self.complete_data_matrix_,
+            self.n_iter_,
+        ) = missing_graphical_lasso(
             X,
             alpha=self.alpha,
             tol=self.tol,
             rtol=self.rtol,
             max_iter=self.max_iter,
             over_relax=self.over_relax,
             rho=self.rho,
```

### Comparing `regain-0.3.8/regain/covariance/time_graphical_lasso_.py` & `regain-0.3.9/regain/covariance/time_graphical_lasso_.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,42 +34,50 @@
 """
 from __future__ import division
 
 import warnings
 
 import numpy as np
 from scipy import linalg
-from six.moves import map, range, zip
 from sklearn.covariance import empirical_covariance, log_likelihood
 from sklearn.utils.extmath import squared_norm
 from sklearn.utils.validation import check_X_y
 
-from regain.covariance.graphical_lasso_ import GraphicalLasso, init_precision, logl
+from regain.covariance.graphical_lasso_ import GraphicalLasso, init_precision
+from regain.math import batch_logdet
 from regain.norm import l1_od_norm
 from regain.prox import prox_logdet, soft_thresholding
 from regain.update_rules import update_rho
-from regain.utils import convergence, error_norm_time
+from regain.utils import Convergence, error_norm_time
 from regain.validation import check_norm_prox
 
 
-def loss(S, K, n_samples=None):
+def batch_log_likelihood(emp_cov, precision):
+    """Gaussian log-likelihood without constant term."""
+    return batch_logdet(precision) - np.sum(emp_cov * precision, axis=(-1, -2))
+
+
+def loss(emp_cov, precision, n_samples: np.ndarray = None) -> float:
     """Loss function for time-varying graphical lasso."""
     if n_samples is None:
-        n_samples = np.ones(S.shape[0])
-    return sum(-ni * logl(emp_cov, precision) for emp_cov, precision, ni in zip(S, K, n_samples))
+        # 1 sample for each batch, ie, do not scale.
+        batch_dim = emp_cov.shape[0]
+        n_samples = np.ones(batch_dim)
 
+    return np.sum(-n_samples * batch_log_likelihood(emp_cov, precision))
 
-def objective(n_samples, S, K, Z_0, Z_1, Z_2, alpha, beta, psi):
+
+def objective(n_samples, emp_cov, K, Z_0, Z_1, Z_2, alpha, beta, psi) -> float:
     """Objective function for time-varying graphical lasso."""
-    obj = loss(S, K, n_samples=n_samples)
+    obj: float = loss(emp_cov, K, n_samples=n_samples)
 
     if isinstance(alpha, np.ndarray):
-        obj += sum(l1_od_norm(a * z) for a, z in zip(alpha, Z_0))
+        obj += np.sum(l1_od_norm(alpha * Z_0))
     else:
-        obj += alpha * sum(map(l1_od_norm, Z_0))
+        obj += alpha * np.sum(l1_od_norm(Z_0))
 
     if isinstance(beta, np.ndarray):
         obj += sum(b[0][0] * m for b, m in zip(beta, map(psi, Z_2 - Z_1)))
     else:
         obj += beta * sum(map(psi, Z_2 - Z_1))
 
     return obj
@@ -163,30 +171,35 @@
     divisor = np.full(emp_cov.shape[0], 3, dtype=float)
     divisor[0] -= 1
     divisor[-1] -= 1
 
     if n_samples is None:
         n_samples = np.ones(emp_cov.shape[0])
 
-    checks = [convergence(obj=objective(n_samples, emp_cov, Z_0, Z_0, Z_1, Z_2, alpha, beta, psi))]
+    checks = [
+        Convergence(
+            obj=objective(n_samples, emp_cov, Z_0, Z_0, Z_1, Z_2, alpha, beta, psi)
+        )
+    ]
     for iteration_ in range(max_iter):
         # update K
         A = Z_0 - U_0
         A[:-1] += Z_1 - U_1
         A[1:] += Z_2 - U_2
         A /= divisor[:, None, None]
         # soft_thresholding_ = partial(soft_thresholding, lamda=alpha / rho)
         # K = np.array(map(soft_thresholding_, A))
         A += A.transpose(0, 2, 1)
         A /= 2.0
 
         A *= -rho * divisor[:, None, None] / n_samples[:, None, None]
         A += emp_cov
 
-        K = np.array([prox_logdet(a, lamda=ni / (rho * div)) for a, div, ni in zip(A, divisor, n_samples)])
+        lamda = np.expand_dims(n_samples / (rho * divisor), -1)
+        K = prox_logdet(A, lamda)
 
         # update Z_0
         A = K + U_0
         A += A.transpose(0, 2, 1)
         A /= 2.0
         Z_0 = soft_thresholding(A, lamda=alpha / rho)
 
@@ -209,54 +222,70 @@
 
         # update residuals
         U_0 += K - Z_0
         U_1 += K[:-1] - Z_1
         U_2 += K[1:] - Z_2
 
         # diagnostics, reporting, termination checks
-        rnorm = np.sqrt(squared_norm(K - Z_0) + squared_norm(K[:-1] - Z_1) + squared_norm(K[1:] - Z_2))
+        rnorm = np.sqrt(
+            squared_norm(K - Z_0)
+            + squared_norm(K[:-1] - Z_1)
+            + squared_norm(K[1:] - Z_2)
+        )
 
-        snorm = rho * np.sqrt(squared_norm(Z_0 - Z_0_old) + squared_norm(Z_1 - Z_1_old) + squared_norm(Z_2 - Z_2_old))
+        snorm = rho * np.sqrt(
+            squared_norm(Z_0 - Z_0_old)
+            + squared_norm(Z_1 - Z_1_old)
+            + squared_norm(Z_2 - Z_2_old)
+        )
 
-        obj = objective(n_samples, emp_cov, Z_0, K, Z_1, Z_2, alpha, beta, psi) if compute_objective else np.nan
+        obj = (
+            objective(n_samples, emp_cov, Z_0, K, Z_1, Z_2, alpha, beta, psi)
+            if compute_objective
+            else np.nan
+        )
 
         # if np.isinf(obj):
         #     Z_0 = Z_0_old
         #     break
 
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=np.sqrt(K.size + 2 * Z_1.size) * tol
             + rtol
             * max(
                 np.sqrt(squared_norm(Z_0) + squared_norm(Z_1) + squared_norm(Z_2)),
                 np.sqrt(squared_norm(K) + squared_norm(K[:-1]) + squared_norm(K[1:])),
             ),
             e_dual=np.sqrt(K.size + 2 * Z_1.size) * tol
-            + rtol * rho * np.sqrt(squared_norm(U_0) + squared_norm(U_1) + squared_norm(U_2)),
+            + rtol
+            * rho
+            * np.sqrt(squared_norm(U_0) + squared_norm(U_1) + squared_norm(U_2)),
             # precision=Z_0.copy()
         )
         Z_0_old = Z_0.copy()
         Z_1_old = Z_1.copy()
         Z_2_old = Z_2.copy()
 
         if verbose:
-            print("obj: %.4f, rnorm: %.4f, snorm: %.4f," "eps_pri: %.4f, eps_dual: %.4f" % check[:5])
+            print(check)
 
         checks.append(check)
         if stop_at is not None:
             if abs(check.obj - stop_at) / abs(stop_at) < stop_when:
                 break
 
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
             break
 
-        rho_new = update_rho(rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {}))
+        rho_new = update_rho(
+            rho, rnorm, snorm, iteration=iteration_, **(update_rho_options or {})
+        )
         # scaled dual variables should be also rescaled
         U_0 *= rho / rho_new
         U_1 *= rho / rho_new
         U_2 *= rho / rho_new
         rho = rho_new
 
         # assert is_pos_def(Z_0)
@@ -437,28 +466,39 @@
         X : ndarray, shape = (n_samples * n_times, n_dimensions)
             Data matrix.
         y : ndarray, shape = (n_times,)
             Indicate the temporal belonging of each sample.
 
         """
         # Covariance does not make sense for a single feature
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         n_dimensions = X.shape[1]
         self.classes_, n_samples = np.unique(y, return_counts=True)
         n_times = self.classes_.size
 
         # n_samples = np.array([x.shape[0] for x in X])
         if self.assume_centered:
             self.location_ = np.zeros((n_times, n_dimensions))
         else:
             self.location_ = np.array([X[y == cl].mean(0) for cl in self.classes_])
 
         emp_cov = np.array(
-            [empirical_covariance(X[y == cl], assume_centered=self.assume_centered) for cl in self.classes_]
+            [
+                empirical_covariance(X[y == cl], assume_centered=self.assume_centered)
+                for cl in self.classes_
+            ]
         )
 
         return self._fit(emp_cov, n_samples)
 
     def score(self, X, y):
         """Computes the log-likelihood of a Gaussian data set with
         `self.covariance_` as an estimator of its covariance matrix.
@@ -478,20 +518,30 @@
         -------
         res : float
             The likelihood of the data set with `self.covariance_` as an
             estimator of its covariance matrix.
 
         """
         # Covariance does not make sense for a single feature
-        X, y = check_X_y(X, y, accept_sparse=False, dtype=np.float64, order="C", ensure_min_features=2, estimator=self)
+        X, y = check_X_y(
+            X,
+            y,
+            accept_sparse=False,
+            dtype=np.float64,
+            order="C",
+            ensure_min_features=2,
+            estimator=self,
+        )
 
         # compute empirical covariance of the test set
         test_cov = np.array(
             [
-                empirical_covariance(X[y == cl] - self.location_[i], assume_centered=True)
+                empirical_covariance(
+                    X[y == cl] - self.location_[i], assume_centered=True
+                )
                 for i, cl in enumerate(self.classes_)
             ]
         )
 
         res = sum(
             X[y == cl].shape[0] * log_likelihood(S, K)
             for S, K, cl in zip(test_cov, self.get_observed_precision(), self.classes_)
@@ -525,8 +575,10 @@
 
         Returns
         -------
         The Mean Squared Error (in the sense of the Frobenius norm) between
         `self` and `comp_cov` covariance estimators.
 
         """
-        return error_norm_time(self.covariance_, comp_cov, norm=norm, scaling=scaling, squared=squared)
+        return error_norm_time(
+            self.covariance_, comp_cov, norm=norm, scaling=scaling, squared=squared
+        )
```

### Comparing `regain-0.3.8/regain/data/__init__.py` & `regain-0.3.9/regain/data/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/data/base.py` & `regain-0.3.9/regain/data/base.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/datasets/__init__.py` & `regain-0.3.9/regain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/datasets/base.py` & `regain-0.3.9/regain/datasets/base.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/datasets/gaussian.py` & `regain-0.3.9/regain/datasets/gaussian.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/datasets/ising.py` & `regain-0.3.9/regain/datasets/ising.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/datasets/kernels.py` & `regain-0.3.9/regain/datasets/kernels.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/datasets/multi_class.py` & `regain-0.3.9/regain/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/datasets/poisson.py` & `regain-0.3.9/regain/datasets/poisson.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 def poisson_theta_generator(
     n_dim_obs=10,
     T=10,
     mode="l1",
     random_graph="erdos-renyi",
-    probability=0.2,
+    probability=0.5,
     degree=3,
     n_to_change=3,
     **kwargs
 ):
     """Generates adjacency matix for Ising graphical model.
 
     Parameters
@@ -174,17 +174,20 @@
         Matrix of shape (n, n_dim_obs)
     """
     n_dim_obs = theta.shape[0]
     if _type == "LPGM":
         A = _adjacency_to_A(theta, typ="scale-free")
         sigma = _lambda * theta
         ltri_sigma = sigma[np.tril_indices(sigma.shape[0], k=-1)]
-        nonzero_sigma = ltri_sigma[np.where(ltri_sigma != 0)]
-        aux = [_lambda] * theta.shape[0]
-        Y_lambda = np.array(aux + nonzero_sigma.ravel().tolist()[0])
+        nonzero_sigma = np.array(ltri_sigma[np.where(ltri_sigma != 0)])
+
+        # aux = [_lambda] * theta.shape[0]
+        lambda_list = np.full(n_dim_obs, fill_value=_lambda)
+        Y_lambda = np.concatenate([lambda_list, nonzero_sigma.reshape(-1)], axis=0)
+        assert Y_lambda.shape[0] == n_dim_obs + nonzero_sigma.size
 
         Y = np.array([np.random.poisson(l, n_samples) for l in Y_lambda]).T
         X = Y.dot(A.T)
 
         # add noise
         X = X + np.random.poisson(_lambda_noise, size=(n_samples, n_dim_obs))
```

### Comparing `regain-0.3.8/regain/discriminant_analysis.py` & `regain-0.3.9/regain/discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/forward_backward/__init__.py` & `regain-0.3.9/regain/forward_backward/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/forward_backward/forward_backward.py` & `regain-0.3.9/regain/forward_backward/forward_backward.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import numpy as np
-from regain.prox import soft_thresholding_od, prox_FL
+
+from regain.prox import prox_FL, soft_thresholding_off_diagonal
 from regain.utils import positive_definite
 
 
 def _scalar_product(x, y):
     return (x * y).sum()
     # return x.ravel().dot(y.ravel())
 
@@ -72,17 +73,19 @@
     ----------
     Salzo S. (2017). https://doi.org/10.1137/16M1073741
 
     """
     fx = function_f(K=x)
     for i in range(max_iter):
         if laplacian_penalty:
-            prox = soft_thresholding_od(x - gamma * grad, alpha * gamma)
+            prox = soft_thresholding_off_diagonal(x - gamma * grad, alpha * gamma)
         else:
-            prox = prox_FL(x - gamma * grad, beta * gamma, alpha * gamma, p=p, symmetric=True)
+            prox = prox_FL(
+                x - gamma * grad, beta * gamma, alpha * gamma, p=p, symmetric=True
+            )
         if positive_definite(prox) and choose != "gamma":
             break
 
         if choose == "gamma":
             y_minus_x = prox - x
             loss_diff = function_f(K=x + lamda * y_minus_x) - fx
```

### Comparing `regain-0.3.8/regain/forward_backward/time_graphical_lasso_.py` & `regain-0.3.9/regain/forward_backward/time_graphical_lasso_.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,34 +24,31 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Time graph lasso via forward_backward (for now only in case of l1 norm)."""
-from __future__ import division, print_function
-
 import warnings
 from functools import partial
 
 import numpy as np
 from scipy import linalg
-from six.moves import map, range, zip
 from sklearn.covariance._graph_lasso import alpha_max  # noqa
 from sklearn.utils.extmath import squared_norm
 
 from regain.covariance.time_graphical_lasso_ import (
     TimeGraphicalLasso,
     init_precision,
     loss as loss_tgl,
 )
 from regain.norm import l1_od_norm, vector_p_norm
-from regain.prox import prox_FL, soft_thresholding_od
-from regain.utils import convergence
+from regain.prox import prox_FL, soft_thresholding_off_diagonal
 from .forward_backward import _scalar_product, choose_gamma, choose_lamda, upper_diag_3d
+from ..utils import Convergence
 
 
 def loss(S, K, n_samples=None, vareps=0):
     """Loss function for time-varying graphical lasso."""
     loss_ = loss_tgl(S, K, n_samples=n_samples)
     loss_ += vareps / 2.0 * _scalar_product(K, K)
     return loss_
@@ -69,17 +66,17 @@
 
     return grad
 
 
 def penalty(precision, alpha, beta, psi):
     """Penalty for time-varying graphical lasso."""
     if isinstance(alpha, np.ndarray):
-        obj = sum(a[0][0] * m for a, m in zip(alpha, map(l1_od_norm, precision)))
+        obj = sum(a[0][0] * m for a, m in zip(alpha, l1_od_norm(precision)))
     else:
-        obj = alpha * sum(map(l1_od_norm, precision))
+        obj = alpha * np.sum(l1_od_norm(precision))
     if isinstance(beta, np.ndarray):
         obj += sum(
             b[0][0] * m for b, m in zip(beta, map(psi, precision[1:] - precision[:-1]))
         )
     else:
         obj += beta * psi(precision[1:] - precision[:-1])
     return obj
@@ -268,15 +265,15 @@
         gradient_f = partial(
             grad_loss, emp_cov=emp_cov, n_samples=n_samples, vareps=vareps
         )
         function_g = partial(penalty, alpha=alpha, beta=beta, psi=psi)
 
     max_residual = -np.inf
     n_linesearch = 0
-    checks = [convergence(obj=obj_partial(precision=K))]
+    checks = [Convergence(obj=obj_partial(precision=K))]
     for iteration_ in range(max_iter):
         k_previous = K.copy()
         x_inv = np.array([linalg.pinvh(x) for x in K])
         grad = gradient_f(K, x_inv=x_inv)
 
         if choose in ["gamma", "both"]:
             gamma, y = choose_gamma(
@@ -295,15 +292,15 @@
                 choose=choose,
                 laplacian_penalty=laplacian_penalty,
             )
 
         x_hat = K - gamma * grad
         if choose not in ["gamma", "both"]:
             if laplacian_penalty:
-                y = soft_thresholding_od(x_hat, alpha * gamma)
+                y = soft_thresholding_off_diagonal(x_hat, alpha * gamma)
             else:
                 y = prox_FL(
                     x_hat, beta * gamma, alpha * gamma, p=time_norm, symmetric=True
                 )
 
         if choose in ("lamda", "both"):
             lamda, n_ls = choose_lamda(
@@ -324,15 +321,15 @@
                 vareps=vareps,
             )
             n_linesearch += n_ls
 
         K = K + min(max(lamda, 0), 1) * (y - K)
         # K, t = fista_step(Y, Y - Y_old, t)
 
-        check = convergence(
+        check = Convergence(
             obj=obj_partial(precision=K),
             rnorm=np.linalg.norm(upper_diag_3d(K) - upper_diag_3d(k_previous)),
             snorm=np.linalg.norm(
                 obj_partial(precision=K) - obj_partial(precision=k_previous)
             ),
             e_pri=np.sqrt(upper_diag_3d(K).size) * tol
             + tol
@@ -340,18 +337,15 @@
                 np.linalg.norm(upper_diag_3d(K)),
                 np.linalg.norm(upper_diag_3d(k_previous)),
             ),
             e_dual=tol,
         )
 
         if verbose and iteration_ % (50 if verbose < 2 else 1) == 0:
-            print(
-                "obj: %.4f, rnorm: %.7f, snorm: %.4f,"
-                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
-            )
+            print(check)
 
         if return_history:
             checks.append(check)
 
         if np.isnan(check.rnorm) or np.isnan(check.snorm):
             warnings.warn("precision is not positive definite.")
```

### Comparing `regain-0.3.8/regain/generalized_linear_model/base.py` & `regain-0.3.9/regain/generalized_linear_model/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-import numpy as np
-
 from abc import ABC, abstractmethod
+from dataclasses import dataclass
 
+import numpy as np
 from sklearn.base import BaseEstimator
-from regain.utils import namedtuple_with_defaults
 
-convergence = namedtuple_with_defaults("convergence", "iter obj iter_norm iter_r_norm")
+
+@dataclass
+class Convergence:
+    iter: float = 0
+    obj: float = 0
+    iter_norm: float = 0
+    iter_r_norm: float = 0
+
+    def __str__(self):
+        return f"Iter: {self.iter}, objective: {self.obj:.4f}, iter_norm {self.iter_norm:.4f}, iter_norm_normalized: {self.iter_r_norm:.4f}"
 
 
 def build_adjacency_matrix(neighbours, how="union"):
     out = np.eye(len(neighbours))
     if how.lower() == "union":
         for i, arr in enumerate(neighbours):
             where = [j for j in range(len(neighbours)) if j != i]
```

### Comparing `regain-0.3.8/regain/generalized_linear_model/glm_gaussian.py` & `regain-0.3.9/regain/generalized_linear_model/glm_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
 from sklearn.utils import check_array
 
 from regain.generalized_linear_model.base import (
+    Convergence,
     GLM_GM,
     build_adjacency_matrix,
-    convergence,
 )
 from regain.prox import soft_thresholding
 
 
 def objective(X, theta, n, r, selector, alpha):
     XXT = X[:, r].T.dot(X[:, selector]).dot(theta)
     TXXT = theta.T.dot(X[:, selector].T).dot(X[:, selector]).dot(theta)
@@ -70,31 +70,28 @@
     thetas = [theta]
     checks = []
     for iter_ in range(max_iter):
         theta_new = theta - gamma * gradient(X, theta, ix, selector, n)
         theta = soft_thresholding(theta_new, alpha * gamma)
         thetas.append(theta)
 
-        check = convergence(
+        check = Convergence(
             iter=iter_,
             obj=objective(X, theta, n, ix, selector, alpha),
             iter_norm=np.linalg.norm(thetas[-2] - thetas[-1]),
             iter_r_norm=(
                 np.linalg.norm(thetas[-2] - thetas[-1]) / np.linalg.norm(thetas[-1])
             ),
         )
         checks.append(check)
         # if adjust_gamma: # TODO multiply or divide
         if verbose:
-            print(
-                "Iter: %d, objective: %.4f, iter_norm %.4f"
-                % (check[0], check[1], check[2])
-            )
+            print(check)
 
-        if check[-2] < tol:
+        if check.iter_norm < tol:
             break
 
     return_list = [thetas[-1]]
     if return_history:
         return_list.append(thetas)
         return_list.append(checks)
     if return_n_iter:
```

### Comparing `regain-0.3.8/regain/generalized_linear_model/glm_ising.py` & `regain-0.3.9/regain/generalized_linear_model/glm_ising.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import warnings
 
 import numpy as np
-
-from sklearn.utils import check_array
 from sklearn.base import BaseEstimator
 from sklearn.linear_model import LogisticRegression
+from sklearn.utils import check_array
 
-from regain.generalized_linear_model.base import GLM_GM, convergence
-from regain.generalized_linear_model.base import build_adjacency_matrix
-from regain.prox import soft_thresholding_od
+from regain.generalized_linear_model.base import (
+    Convergence,
+    GLM_GM,
+    build_adjacency_matrix,
+)
 from regain.norm import l1_od_norm
+from regain.prox import soft_thresholding_off_diagonal
 
 
 def loss(X, theta):
     n, d = X.shape
     objective = 0
     if not np.all(theta == theta.T):
         return np.float("inf")
@@ -114,53 +116,55 @@
     checks = []
     for iter_ in range(max_iter):
         theta_old = thetas[-1]
         if not line_search:
             grad = _gradient_ising(X, theta, n, A, rho, T)
             theta_new = theta - gamma * grad
             theta = (theta_new + theta_new.T) / 2
-            theta = soft_thresholding_od(theta, alpha * gamma)
+            theta = soft_thresholding_off_diagonal(theta, alpha * gamma)
         else:
             while True:
                 grad = _gradient_ising(X, theta, n, A, rho, T)
                 theta_new = theta - gamma * grad
                 theta = (theta_new + theta_new.T) / 2
-                theta = soft_thresholding_od(theta, alpha * gamma)
+                theta = soft_thresholding_off_diagonal(theta, alpha * gamma)
                 print(theta)
                 loss_new = loss(X, theta)
                 loss_old = loss(X, theta_old)
                 # Line search
                 diff_theta2 = np.linalg.norm(theta_old - theta) ** 2
                 grad_diff = np.trace(grad.dot(theta_old - theta))
                 diff = loss_old - grad_diff + (diff_theta2 / (2 * gamma))
 
                 if loss_new > diff or np.isinf(loss_new) or np.isnan(loss_new):
                     gamma = update_gamma * gamma
                     theta = theta_old - gamma * grad
-                    theta = soft_thresholding_od(theta, alpha * gamma)
+                    theta = soft_thresholding_off_diagonal(theta, alpha * gamma)
                     loss_new = loss(X, theta)
                     diff = loss_old - grad_diff + (diff_theta2 / (2 * gamma))
                 else:
                     break
         thetas.append(theta)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            check = convergence(
+            check = Convergence(
                 iter=iter_,
                 obj=objective(X, theta, alpha),
                 iter_norm=np.linalg.norm(thetas[-2] - thetas[-1]),
-                iter_r_norm=(np.linalg.norm(thetas[-2] - thetas[-1]) / np.linalg.norm(thetas[-1])),
+                iter_r_norm=(
+                    np.linalg.norm(thetas[-2] - thetas[-1]) / np.linalg.norm(thetas[-1])
+                ),
             )
         checks.append(check)
         # if adjust_gamma: # TODO multiply or divide
         if verbose:
-            print("Iter: %d, objective: %.4f, iter_norm %.4f" % (check[0], check[1], check[2]))
+            print(check)
 
-        if np.abs(check[2]) < tol:
+        if np.abs(check.iter_norm) < tol:
             break
 
     return_list = [thetas[-1]]
     if return_history:
         return_list.append(thetas)
         return_list.append(checks)
     if return_n_iter:
@@ -235,15 +239,22 @@
         verbose=False,
         return_history=True,
         return_n_iter=False,
         compute_objective=True,
         gamma=1,
     ):
         super(IsingGraphicalModel, self).__init__(
-            alpha, tol, rtol, max_iter, verbose, return_history, return_n_iter, compute_objective
+            alpha,
+            tol,
+            rtol,
+            max_iter,
+            verbose,
+            return_history,
+            return_n_iter,
+            compute_objective,
         )
         self.reconstruction = reconstruction
         self.mode = mode
         self.rho = rho
         self.gamma = gamma
 
     def get_precision(self):
@@ -255,15 +266,22 @@
             Data matrix.
         y : added for compatiblity
         gamma: float,
             Step size of the proximal gradient descent.
         """
         X = check_array(X)
         if self.mode.lower() == "symmetric_fbs":
-            res = _fit(X, self.alpha, tol=self.tol, gamma=self.gamma, max_iter=self.max_iter, verbose=self.verbose)
+            res = _fit(
+                X,
+                self.alpha,
+                tol=self.tol,
+                gamma=self.gamma,
+                max_iter=self.max_iter,
+                verbose=self.verbose,
+            )
             self.precision_ = res[0]
             self.history = res[1:]
         elif self.mode.lower() == "coordinate_descent":
             raise ValueError("Not implemented")
             # thetas_pred = []
             # historys = []
             # for ix in range(X.shape[1]):
@@ -279,23 +297,31 @@
             thetas_pred = []
             for ix in range(X.shape[1]):
                 verbose = min(0, self.verbose - 1)
                 selector = np.array([i for i in range(X.shape[1]) if i != ix])
                 print("pd")
                 res = (
                     LogisticRegression(
-                        C=1 / self.alpha, penalty="l1", solver="liblinear", verbose=verbose, random_state=0
+                        C=1 / self.alpha,
+                        penalty="l1",
+                        solver="liblinear",
+                        verbose=verbose,
+                        random_state=0,
                     )
                     .fit(X[:, selector], X[:, ix])
                     .coef_
                 )
                 thetas_pred.append(res)
-            self.precision_ = build_adjacency_matrix(thetas_pred, how=self.reconstruction)
+            self.precision_ = build_adjacency_matrix(
+                thetas_pred, how=self.reconstruction
+            )
         else:
             raise ValueError(
-                "Unknown optimization mode. Found " + self.mode + ". Options are 'coordiante_descent', "
+                "Unknown optimization mode. Found "
+                + self.mode
+                + ". Options are 'coordiante_descent', "
                 "'symmetric_fbs'"
             )
         return self
 
     def score(self, X, y=None):
         return 0
```

### Comparing `regain-0.3.8/regain/generalized_linear_model/glm_poisson.py` & `regain-0.3.9/regain/generalized_linear_model/glm_poisson.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,24 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
-from sklearn.utils import check_array
 from sklearn.base import BaseEstimator
+from sklearn.utils import check_array
 
-from regain.generalized_linear_model.base import GLM_GM, convergence
-from regain.generalized_linear_model.base import build_adjacency_matrix
-from regain.prox import soft_thresholding
+from regain.generalized_linear_model.base import (
+    Convergence,
+    GLM_GM,
+    build_adjacency_matrix,
+)
 from regain.norm import l1_od_norm
+from regain.prox import soft_thresholding
 
 
 def loss_single_variable(X, theta, n, r, selector):
     objective = 0
     for i in range(n):
         XXT = X[i, r] * X[i, selector].dot(theta)
         expXT = np.exp(X[i, selector].dot(theta))
@@ -117,29 +120,28 @@
                 theta = soft_thresholding(theta, alpha * gamma)
                 loss_new = loss_single_variable(X, theta, n, ix, selector)
                 diff = loss_old - grad_diff + (diff_theta2 / (2 * gamma))
             else:
                 break
         thetas.append(theta)
         if iter_ > 0:
-            check = convergence(
+            check = Convergence(
                 iter=iter_,
                 obj=objective_single_variable(X, theta, n, ix, selector, alpha),
                 iter_norm=np.linalg.norm(thetas[-2] - thetas[-1]),
-                iter_r_norm=(np.linalg.norm(thetas[-2] - thetas[-1]) / np.linalg.norm(thetas[-2])),
+                iter_r_norm=(
+                    np.linalg.norm(thetas[-2] - thetas[-1]) / np.linalg.norm(thetas[-2])
+                ),
             )
             checks.append(check)
             # if adjust_gamma: # TODO multiply or divide
             if verbose:
-                print(
-                    "Iter: %d, objective: %.4f, iter_norm %.4f,"
-                    " iter_norm_normalized: %.4f" % (check[0], check[1], check[2], check[3])
-                )
+                print(check)
 
-            if np.abs(check[2]) < tol:
+            if np.abs(check.iter_norm) < tol:
                 break
 
     return_list = [thetas[-1]]
     if return_history:
         return_list.append(thetas)
         return_list.append(checks)
     if return_n_iter:
@@ -224,15 +226,22 @@
         intercept=False,
         verbose=False,
         return_history=True,
         return_n_iter=False,
         compute_objective=True,
     ):
         super(PoissonGraphicalModel, self).__init__(
-            alpha, tol, rtol, max_iter, verbose, return_history, return_n_iter, compute_objective
+            alpha,
+            tol,
+            rtol,
+            max_iter,
+            verbose,
+            return_history,
+            return_n_iter,
+            compute_objective,
         )
         self.reconstruction = reconstruction
         self.mode = mode
         self.gamma = gamma
         self.intercept = intercept
 
     def get_precision(self):
@@ -247,28 +256,33 @@
             Step size of the proximal gradient descent.
         """
         X = check_array(X)
         if self.mode.lower() == "symmetric_fbs":
             raise ValueError("Not implemented.")
 
         elif self.mode.lower() == "coordinate_descent":
-            print("sono qui")
             thetas_pred = []
             historys = []
             if self.intercept:
                 X = np.hstack((X, np.ones((X.shape[0], 1))))
             for ix in range(X.shape[1]):
                 verbose = max(0, self.verbose - 1)
-                res = fit_each_variable(X, ix, self.alpha, tol=self.tol, verbose=verbose)
+                res = fit_each_variable(
+                    X, ix, self.alpha, tol=self.tol, verbose=verbose
+                )
                 thetas_pred.append(res[0])
                 historys.append(res[1:])
-            self.precision_ = build_adjacency_matrix(thetas_pred, how=self.reconstruction)
+            self.precision_ = build_adjacency_matrix(
+                thetas_pred, how=self.reconstruction
+            )
             self.history = historys
         else:
             raise ValueError(
-                "Unknown optimization mode. Found " + self.mode + ". Options are 'coordiante_descent', "
+                "Unknown optimization mode. Found "
+                + self.mode
+                + ". Options are 'coordiante_descent', "
                 "'symmetric_fbs'"
             )
         return self
 
     def score(self, X, y=None):
         return 0
```

### Comparing `regain-0.3.8/regain/generalized_linear_model/glm_time_ising.py` & `regain-0.3.9/regain/generalized_linear_model/glm_time_ising.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,45 +27,43 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import warnings
 
 import numpy as np
-
-from six.moves import map, range, zip
-
 from sklearn.base import BaseEstimator
-from sklearn.utils.extmath import squared_norm
-from sklearn.utils.validation import check_X_y
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.gaussian_process import kernels
-
-from sklearn.utils.validation import check_is_fitted
+from sklearn.utils.extmath import squared_norm
+from sklearn.utils.validation import check_X_y, check_is_fitted
 
 from regain.covariance.time_graphical_lasso_ import init_precision
 from regain.generalized_linear_model.glm_ising import _fit, loss
 from regain.norm import l1_od_norm
-from regain.utils import convergence
 from regain.update_rules import update_rho
+from regain.utils import Convergence
 from regain.validation import check_norm_prox
 
 
-def loss_ising(X, K, n_samples=None):
+def loss_ising(X, precision, n_samples=None):
     """Loss function for time-varying ising model."""
     if n_samples is None:
-        n_samples = np.ones(X.shape[0])
-    return sum(-ni * loss(x, k) for x, k, ni in zip(X, K, n_samples))
+        # 1 sample for each batch, ie, do not scale.
+        batch_dim = X.shape[0]
+        n_samples = np.ones(batch_dim)
+
+    return sum(-ni * loss(x, k) for x, k, ni in zip(X, precision, n_samples))
 
 
 def objective(X, K, Z_M, alpha, kernel, psi):
     """Objective function for time-varying ising model."""
 
     obj = loss_ising(X, K)
-    obj += alpha * sum(map(l1_od_norm, K))
+    obj += alpha * np.sum(l1_od_norm(K))
 
     for m in range(1, K.shape[0]):
         # all possible non markovians jumps
         Z_L, Z_R = Z_M[m]
         obj += np.sum(np.array(list(map(psi, Z_R - Z_L))) * np.diag(kernel, m))
 
     return obj
@@ -154,30 +152,28 @@
         U_R = np.zeros_like(Z_R)
         U_M[m] = (U_L, U_R)
 
         Z_L_old = np.zeros_like(Z_L)
         Z_R_old = np.zeros_like(Z_R)
         Z_M_old[m] = (Z_L_old, Z_R_old)
 
-    checks = [convergence(obj=objective(X, K, Z_M, alpha, kernel, psi))]
+    checks = [Convergence(obj=objective(X, K, Z_M, alpha, kernel, psi))]
     for iteration_ in range(max_iter):
         # update K
 
         A = np.zeros_like(K)
         for m in range(1, n_times):
             A[:-m] += Z_M[m][0] - U_M[m][0]
             A[m:] += Z_M[m][1] - U_M[m][1]
 
         A /= n_times
         A += A.transpose(0, 2, 1)
         A /= 2.0
         # K_new = np.zeros_like(K)
 
-        print(K.shape)
-
         for t in range(n_times):
             K[t, :, :] = _fit(
                 X=X[t, :, :],
                 A=A[t, :, :],
                 alpha=alpha,
                 gamma=gamma,
                 tol=tol,
@@ -231,15 +227,15 @@
                 + squared_norm(Z_M[m][1] - Z_M_old[m][1])
                 for m in range(1, n_times)
             )
         )
 
         obj = objective(X, K, Z_M, alpha, kernel, psi) if compute_objective else np.nan
 
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=n_features * n_times * tol
             + rtol
             * max(
                 np.sqrt(
@@ -266,18 +262,15 @@
                 )
             ),
         )
         for m in range(1, n_times):
             Z_M_old[m] = (Z_M[m][0].copy(), Z_M[m][1].copy())
 
         if verbose:
-            print(
-                "obj: %.4f, rnorm: %.4f, snorm: %.4f,"
-                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
-            )
+            print(check)
 
         checks.append(check)
         if stop_at is not None:
             if abs(check.obj - stop_at) / abs(stop_at) < stop_when:
                 break
 
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
@@ -505,15 +498,15 @@
                     )
                 except TypeError:
                     # maybe it's a ConstantKernel
                     kernel = self.kernel(constant_value=self.ker_param)(
                         self.classes_[:, None]
                     )
             else:
-                kernel = self.kernel
+                kernel = self.kernel or np.identity(self.classes_.size)
                 if kernel.shape[0] != self.classes_.size:
                     raise ValueError(
                         "Kernel size does not match classes of samples, "
                         "got {} classes and kernel has shape {}".format(
                             self.classes_.size, kernel.shape[0]
                         )
                     )
@@ -575,15 +568,14 @@
     from regain.norm import l1_od_norm
     from scipy.spatial.distance import squareform
     from itertools import combinations
 
     distances = squareform(
         [l1_od_norm(t1 - t2) for t1, t2 in combinations(precision, 2)]
     )
-    print(distances)
     distances /= np.max(distances)
     return 1 - distances
 
 
 class SimilarityTemporalIsingModel(TemporalIsingModel):
     """Learn how to relate different adjacencies matrices across times.
 
@@ -746,15 +738,14 @@
                     and np.linalg.norm(labels_pred - labels_pred_old) / labels_pred.size
                     < self.eps
                 ):
                     break
                 kernel = kernels.RBF(0.0001)(labels_pred[:, None]) + kernels.RBF(
                     self.beta
                 )(np.arange(n_times)[:, None])
-                print(kernel)
                 labels_pred_old = labels_pred
 
             else:
                 warnings.warn("theta did not converge.")
             self.similarity_matrix_ = kernel
 
         else:
```

### Comparing `regain-0.3.8/regain/generalized_linear_model/glm_time_poisson.py` & `regain-0.3.9/regain/generalized_linear_model/glm_time_poisson.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,42 +27,41 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import warnings
 
 import numpy as np
-from six.moves import map, range, zip
 from sklearn.base import BaseEstimator
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.gaussian_process import kernels
 from sklearn.utils.extmath import squared_norm
 from sklearn.utils.validation import check_X_y, check_is_fitted
 
 from regain.covariance.kernel_time_graphical_lasso_ import precision_similarity
 from regain.generalized_linear_model.base import build_adjacency_matrix
 from regain.generalized_linear_model.glm_poisson import fit_each_variable, loss
 from regain.norm import l1_od_norm
 from regain.update_rules import update_rho
-from regain.utils import convergence
+from regain.utils import Convergence
 from regain.validation import check_norm_prox
 
 
 def loss_poisson(X, K, n_samples=None):
     """Loss function for time-varying poisson model."""
     if n_samples is None:
         n_samples = np.ones(X.shape[0])
     return sum(-ni * loss(x, k) for x, k, ni in zip(X, K, n_samples))
 
 
 def objective(X, K, Z_M, alpha, kernel, psi):
     """Objective function for time-varying poisson model."""
 
     obj = loss_poisson(X, K)
-    obj += alpha * sum(map(l1_od_norm, K))
+    obj += alpha * np.sum(l1_od_norm(K))
 
     for m in range(1, K.shape[0]):
         # all possible non markovians jumps
         Z_L, Z_R = Z_M[m]
         obj += np.sum(np.array(list(map(psi, Z_R - Z_L))) * np.diag(kernel, m))
 
     return obj
@@ -149,15 +148,15 @@
         U_R = np.zeros_like(Z_R)
         U_M[m] = (U_L, U_R)
 
         Z_L_old = np.zeros_like(Z_L)
         Z_R_old = np.zeros_like(Z_R)
         Z_M_old[m] = (Z_L_old, Z_R_old)
 
-    checks = [convergence(obj=objective(X, K, Z_M, alpha, kernel, psi))]
+    checks = [Convergence(obj=objective(X, K, Z_M, alpha, kernel, psi))]
     for iteration_ in range(max_iter):
         # update K
         A = np.zeros_like(K)
         for m in range(1, n_times):
             A[:-m] += Z_M[m][0] - U_M[m][0]
             A[m:] += Z_M[m][1] - U_M[m][1]
 
@@ -224,15 +223,15 @@
                 + squared_norm(Z_M[m][1] - Z_M_old[m][1])
                 for m in range(1, n_times)
             )
         )
 
         obj = objective(X, K, Z_M, alpha, kernel, psi) if compute_objective else np.nan
 
-        check = convergence(
+        check = Convergence(
             obj=obj,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=n_features * n_times * tol
             + rtol
             * max(
                 np.sqrt(
@@ -259,18 +258,15 @@
                 )
             ),
         )
         for m in range(1, n_times):
             Z_M_old[m] = (Z_M[m][0].copy(), Z_M[m][1].copy())
 
         if verbose:
-            print(
-                "obj: %.4f, rnorm: %.4f, snorm: %.4f,"
-                "eps_pri: %.4f, eps_dual: %.4f" % check[:5]
-            )
+            print(check)
 
         checks.append(check)
         if stop_at is not None:
             if abs(check.obj - stop_at) / abs(stop_at) < stop_when:
                 break
 
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
@@ -497,15 +493,15 @@
                     )
                 except TypeError:
                     # maybe it's a ConstantKernel
                     kernel = self.kernel(constant_value=self.ker_param)(
                         self.classes_[:, None]
                     )
             else:
-                kernel = self.kernel
+                kernel = self.kernel or np.identity(self.classes_.size)
                 if kernel.shape[0] != self.classes_.size:
                     raise ValueError(
                         "Kernel size does not match classes of samples, "
                         "got {} classes and kernel has shape {}".format(
                             self.classes_.size, kernel.shape[0]
                         )
                     )
```

### Comparing `regain-0.3.8/regain/linear_model/__init__.py` & `regain-0.3.9/regain/linear_model/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/linear_model/_group_lasso_overlap_old_.py` & `regain-0.3.9/regain/linear_model/_group_lasso_overlap_old_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/linear_model/group_lasso_.py` & `regain-0.3.9/regain/linear_model/group_lasso_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/linear_model/group_lasso_overlap_.py` & `regain-0.3.9/regain/linear_model/group_lasso_overlap_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/linear_model/lasso_.py` & `regain-0.3.9/regain/linear_model/lasso_.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/model_selection/__init__.py` & `regain-0.3.9/regain/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/model_selection/_bayesian_optimization.py` & `regain-0.3.9/regain/model_selection/_bayesian_optimization.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/model_selection/stability_optimization.py` & `regain-0.3.9/regain/model_selection/stability_optimization.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/norm.py` & `regain-0.3.9/regain/norm.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,37 +32,47 @@
 import numpy as np
 from scipy.optimize import minimize
 
 
 def vector_p_norm(a, p=1):
     """Sum of norms for each vector."""
     b = np.array([b.flatten() for b in a]).T
-    return np.linalg.norm(b, axis=1, ord=1).sum()
+    return np.linalg.norm(b, axis=1, ord=p).sum()
 
 
 def l1_norm(precision):
     """L1 norm."""
     return np.abs(precision).sum()
 
 
+def matrix_l1_norm(matrix):
+    """Sum components over the last 2 dimensions."""
+    return np.sum(np.abs(matrix), (-1, -2))
+
+
 def l1_od_norm(precision):
     """L1 norm off-diagonal."""
-    return l1_norm(precision) - np.abs(np.diag(precision)).sum()
+    diagonal_sum = np.abs(np.diagonal(precision, axis1=-2, axis2=-1)).sum(-1)
+    return matrix_l1_norm(precision) - diagonal_sum
 
 
 def node_penalty(X):
     """Node penalty. See Hallac for details."""
     cons = (
         {
             "type": "eq",
-            "fun": lambda x: np.array((x.reshape(X.shape) + x.reshape(X.shape).T - X).sum()),
+            "fun": lambda x: np.array(
+                (x.reshape(X.shape) + x.reshape(X.shape).T - X).sum()
+            ),
             "jac": lambda x: np.full(X.size, 2),
         },
     )
     try:
         res = minimize(
-            lambda x: np.sum(np.linalg.norm(x.reshape(X.shape), axis=0)), np.random.randn(X.size), constraints=cons
+            lambda x: np.sum(np.linalg.norm(x.reshape(X.shape), axis=0)),
+            np.random.randn(X.size),
+            constraints=cons,
         ).fun
     except ValueError:
         res = np.nan
 
     return res
```

### Comparing `regain-0.3.8/regain/plotting/__init__.py` & `regain-0.3.9/regain/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/plotting/covariance.py` & `regain-0.3.9/regain/plotting/covariance.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/plotting/graph.py` & `regain-0.3.9/regain/plotting/graph.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/plotting/plotly.py` & `regain-0.3.9/regain/plotting/plotly.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/plotting/results.py` & `regain-0.3.9/regain/plotting/results.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/prox.py` & `regain-0.3.9/regain/prox.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,169 +28,139 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Proximal functions."""
 import warnings
 from functools import partial
 
-import collections
-
 import numpy as np
-from six.moves import range, zip
 from sklearn.utils.extmath import squared_norm
 
+from regain.math import create_from_diagonal, fill_diagonal, get_diagonal
 from regain.update_rules import update_rho
-from regain.utils import convergence
+from regain.utils import Convergence
 
 try:
     from prox_tv import tv1_1d, tvp_1d, tvgen, tvp_2d
-except:
+except ImportError:
     # fused lasso prox cannot be used
     pass
 
 
 def soft_thresholding(a, lamda):
     """Soft-thresholding."""
     return np.sign(a) * np.maximum(np.abs(a) - lamda, 0)
 
 
-def _soft_thresholding_od_2d(a, lamda):
-    # this assumes array is 2-dimensional
-    # no check is performed for optimisation
+def soft_thresholding_off_diagonal(a, lamda):
+    """Soft-thresholding."""
     soft = soft_thresholding(a, lamda)
-    np.fill_diagonal(soft, np.diag(a))
+    fill_diagonal(soft, get_diagonal(a))
     return soft
 
 
-def soft_thresholding_od(a, lamda):
-    """Off-diagonal soft-thresholding."""
-    if a.ndim > 2:
-        out = np.empty_like(a)
-        if not isinstance(lamda, collections.Iterable):
-            lamda = np.repeat(lamda, a.shape[0])
-        else:
-            assert lamda.shape[0] == a.shape[0]
-
-        for t in range(a.shape[0]):
-            out[t] = _soft_thresholding_od_2d(a[t], lamda[t])
-    else:
-        out = _soft_thresholding_od_2d(a, lamda)
-    return out
-
-
 def soft_thresholding_vector(a, lamda):
     """Soft-thresholding for vectors."""
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        return np.maximum(1 - lamda / np.linalg.norm(a), 0) * a
-
-
-def _blockwise_soft_thresholding_2d(a, lamda):
-    """Proximal operator for l2 norm, a is two-dimensional."""
-    return np.array([soft_thresholding_vector(aa, lamda) for aa in a.T]).T
+    return np.maximum(1 - lamda / np.linalg.norm(a, axis=-1, keepdims=True), 0) * a
 
 
 def blockwise_soft_thresholding(a, lamda):
-    """Proximal operator for l2 norm."""
-    if a.ndim > 2:
-        out = np.empty_like(a, dtype=float)
-        if not isinstance(lamda, collections.Iterable):
-            lamda = np.repeat(lamda, a.shape[0])
-        else:
-            lamda = lamda.ravel()
-            assert lamda.shape[0] == a.shape[0]
-
-        for t in range(a.shape[0]):
-            out[t] = _blockwise_soft_thresholding_2d(a[t], lamda[t])
-    else:
-        out = _blockwise_soft_thresholding_2d(a, lamda)
+    """Proximal operator for l2 norm column-wise."""
+    out = soft_thresholding_vector(a.swapaxes(-1, -2), lamda).swapaxes(-1, -2)
     return out
 
 
 def blockwise_soft_thresholding_symmetric(a, lamda):
     """Proximal operator for l2 norm, for symmetric matrices (last 2 axes)."""
-    col_norms = np.linalg.norm(a, axis=1)
-    ones_vect = np.ones(a.shape[1])
-
-    if a.ndim > 2:
-        out = np.empty_like(a, dtype=float)
-        if not isinstance(lamda, collections.Iterable):
-            lamda = np.repeat(lamda, a.shape[0])
-        else:
-            lamda = lamda.ravel()
-            assert lamda.shape[0] == a.shape[0]
-
-        out = np.empty_like(a, dtype=float)
-        for t, (x, c_norm) in enumerate(zip(a, col_norms)):
-            out[t] = np.dot(x, np.diag((ones_vect - lamda[t] / c_norm) * (c_norm > lamda[t])))
-
-    else:
-        out = np.dot(a, np.diag((ones_vect - lamda / col_norms) * (col_norms > lamda)))
-
+    col_norms = np.linalg.norm(a, axis=-2)
+    out = np.matmul(
+        a, create_from_diagonal((1 - lamda / col_norms) * (col_norms > lamda))
+    )
     return out
 
 
-# %% Perform prox operator:   min_x (1/2t)||x-w||^2 subject to |x|<=radius
-# function [ z ] = project_1ball( z,radius )
-# %  By Moreau's identity, projection onto 1-norm ball can be computed
-# %  using the proximal of the conjugate problem, which is L-infinity
-# %  minimization.
-#   z = z -  prox_infinityNorm(z,radius);
-# end
-# %% Perform prox operator:   min ||x||_inf + (1/2t)||x-w||^2
-# function [ xk ] = prox_infinityNorm( w,t )
-#     N = length(w);
-#     wabs = abs(w);
-#     ws = (cumsum(sort(wabs,'descend'))- t)./(1:N)';
-#     alphaopt = max(ws);
-#     if alphaopt>0
-#       xk = min(wabs,alphaopt).*sign(w); % truncation step
-#     else
-#       xk = zeros(size(w)); % if t is big, then solution is zero
-#     end
-# end
 def prox_linf_1d(a, lamda):
-    """Proximal operator for the l-inf norm.
+    """Proximal operator for the l-inf norm, defined as:
+
+    min ||x||_inf + (1/2t)||x-w||^2
 
     Since there is no closed-form, we can minimize it with scipy.
+
+    Matlab reference
+    ------
+    %% Perform prox operator:   min_x (1/2t)||x-w||^2 subject to |x|<=radius
+    function [ z ] = project_1ball( z,radius )
+    %  By Moreau's identity, projection onto 1-norm ball can be computed
+    %  using the proximal of the conjugate problem, which is L-infinity
+    %  minimization.
+      z = z -  prox_infinityNorm(z,radius);
+    end
+
+    %% Perform prox operator:   min ||x||_inf + (1/2t)||x-w||^2
+    function [ xk ] = prox_infinityNorm( w,t )
+        N = length(w);
+        wabs = abs(w);
+        ws = (cumsum(sort(wabs,'descend'))- t)./(1:N)';
+        alphaopt = max(ws);
+        if alphaopt>0
+          xk = min(wabs,alphaopt).*sign(w); % truncation step
+        else
+          xk = zeros(size(w)); % if t is big, then solution is zero
+        end
+    end
     """
     from scipy.optimize import minimize
 
-    def _f(x):
-        return lamda * np.linalg.norm(x, np.inf) + 0.5 * np.power(np.linalg.norm(a - x), 2)
+    def f(x):
+        return lamda * np.linalg.norm(x, np.inf) + 0.5 * squared_norm(a - x)
 
-    return minimize(_f, a).x
+    return minimize(f, a).x
 
 
 def prox_linf(a, lamda):
     """Proximal operator for l-inf norm."""
     x = np.zeros_like(a)
     for t in range(a.shape[0]):
         x[t] = np.array([prox_linf_1d(a[t, :, j], lamda) for j in range(a.shape[1])]).T
     return x
 
 
 def prox_logdet(a, lamda):
     """Time-varying latent variable graphical lasso prox."""
     es, Q = np.linalg.eigh(a)
     xi = (-es + np.sqrt(np.square(es) + 4.0 / lamda)) * lamda / 2.0
-    return np.linalg.multi_dot((Q, np.diag(xi), Q.T))
+    # return np.linalg.multi_dot((Q, np.diag(xi), Q.T))
+
+    # support ndim > 2
+    Xi = create_from_diagonal(xi)
+    QXiQt = np.matmul(np.matmul(Q, Xi), np.swapaxes(Q, -1, -2))
+    return QXiQt
 
 
 def prox_logdet_ala_ma(a, lamda):
     es, Q = np.linalg.eigh(a)
     xi = (-es + np.sqrt(np.square(es) + 4.0 * lamda)) / 2.0
-    return np.linalg.multi_dot((Q, np.diag(xi), Q.T))
+    # return np.linalg.multi_dot((Q, np.diag(xi), Q.T))
+
+    # support ndim > 2
+    Xi = create_from_diagonal(xi)
+    QXiQt = np.matmul(np.matmul(Q, Xi), np.swapaxes(Q, -1, -2))
+    return QXiQt
 
 
 def prox_trace_indicator(a, lamda):
     """Time-varying latent variable graphical lasso prox."""
     es, Q = np.linalg.eigh(a)
     xi = np.maximum(es - lamda, 0)
-    return np.linalg.multi_dot((Q, np.diag(xi), Q.T))
+    # return np.linalg.multi_dot((Q, np.diag(xi), Q.T))
+
+    # support ndim > 2
+    Xi = create_from_diagonal(xi)
+    QXiQt = np.matmul(np.matmul(Q, Xi), np.swapaxes(Q, -1, -2))
+    return QXiQt
 
 
 def prox_laplacian(a, lamda):
     """Prox for l_2 square norm, Laplacian regularisation."""
     return a / (1 + 2.0 * lamda)
 
 
@@ -211,15 +181,17 @@
 
     V = np.zeros_like(U_1)
     W = np.zeros_like(U_1)
     V_old = np.zeros_like(U_1)
     W_old = np.zeros_like(U_1)
 
     for iteration_ in range(max_iter):
-        A = (Y_1 - Y_2 - W - U_1 + (W.transpose(0, 2, 1) - U_2).transpose(0, 2, 1)) / 2.0
+        A = (
+            Y_1 - Y_2 - W - U_1 + (W.transpose(0, 2, 1) - U_2).transpose(0, 2, 1)
+        ) / 2.0
         V = blockwise_soft_thresholding_symmetric(A, lamda=lamda)
 
         A = np.concatenate(((V + U_2).transpose(0, 2, 1), A_12), axis=1)
         D = V + U_1
         # Z = np.linalg.solve(C.T*C + eta*np.identity(3*n), - C.T*D + eta* A)
         Z = np.empty_like(A)
         for i, (A_i, D_i) in enumerate(zip(A, D)):
@@ -230,23 +202,29 @@
         delta_U_1 = V + W - (Y_1 - Y_2)
         delta_U_2 = V - W.transpose(0, 2, 1)
         U_1 += delta_U_1
         U_2 += delta_U_2
 
         # diagnostics
         rnorm = np.sqrt(squared_norm(delta_U_1) + squared_norm(delta_U_2))
-        snorm = rho * np.sqrt(squared_norm(W - W_old) + squared_norm(V + W - V_old - W_old))
-        check = convergence(
+        snorm = rho * np.sqrt(
+            squared_norm(W - W_old) + squared_norm(V + W - V_old - W_old)
+        )
+        check = Convergence(
             obj=np.nan,
             rnorm=rnorm,
             snorm=snorm,
             e_pri=np.sqrt(2 * V.size) * tol
             + rtol
-            * max(np.sqrt(squared_norm(W) + squared_norm(V + W)), np.sqrt(squared_norm(V) + squared_norm(Y_1 - Y_2))),
-            e_dual=np.sqrt(2 * V.size) * tol + rtol * rho * np.sqrt(squared_norm(U_1) + squared_norm(U_2)),
+            * max(
+                np.sqrt(squared_norm(W) + squared_norm(V + W)),
+                np.sqrt(squared_norm(V) + squared_norm(Y_1 - Y_2)),
+            ),
+            e_dual=np.sqrt(2 * V.size) * tol
+            + rtol * rho * np.sqrt(squared_norm(U_1) + squared_norm(U_2)),
         )
         W_old = W.copy()
         V_old = V.copy()
 
         # if np.linalg.norm(delta_U_1, 'fro') < tol and \
         #         np.linalg.norm(delta_U_2, 'fro') < tol:
         if check.rnorm <= check.e_pri and check.snorm <= check.e_dual:
@@ -286,15 +264,17 @@
             x, y = np.triu_indices_from(a[0])
             b = np.vstack(a.transpose(1, 2, 0))
             upper_ind = x * a.shape[1] + y
             Z = np.zeros_like(b)
             Z[upper_ind] = [func(row, beta) for row in b[upper_ind]]
 
             e = np.array(np.split(Z, a.shape[1], axis=0)).transpose(2, 0, 1)
-            Y = (e + e.transpose(0, 2, 1)) / (np.array([np.eye(a.shape[1]) for i in range(a.shape[0])]) + 1)
+            Y = (e + e.transpose(0, 2, 1)) / (
+                np.array([np.eye(a.shape[1]) for i in range(a.shape[0])]) + 1
+            )
         else:
             for i in range(np.power(a.shape[1], 2)):
                 solution = func(a.flat[i :: np.power(a.shape[1], 2)], beta)
                 Y.flat[i :: np.power(a.shape[1], 2)] = solution
 
     # fused-lasso (soft-thresholding on the solution)
     Y_soft = soft_thresholding(Y, lamda)
```

### Comparing `regain-0.3.8/regain/scores.py` & `regain-0.3.9/regain/scores.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,85 +25,98 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
-from sklearn.utils.extmath import fast_logdet
+
+from regain.math import batch_logdet
 
 
 def log_likelihood(emp_cov, precision):
     """Gaussian log-likelihood without constant term."""
-    return fast_logdet(precision) - np.sum(emp_cov * precision)
+    return batch_logdet(precision) - np.sum(emp_cov * precision, axis=(-1, -2))
+
+
+def log_likelihood_t(emp_cov, precision):
+    """Gaussian log-likelihood without constant term for batch of matrices."""
+    return log_likelihood(emp_cov, precision).sum()
 
 
 def BIC(emp_cov, precision):
     """Bayesian Information Criterion for Gaussian models"""
-    return log_likelihood(emp_cov, precision) - (np.sum(precision != 0) - precision.shape[0])
+    return log_likelihood(emp_cov, precision) - (
+        np.sum(precision != 0) - precision.shape[0]
+    )
 
 
 def EBIC(emp_cov, precision, n=100, epsilon=0.5):
     """E - Bayesian Information Criterion for Gaussian models.
 
-    It penalizes more then BIC by multplying the degrees of freedom also based
+    It penalizes more than BIC by multplying the degrees of freedom also based
     on sample size.
     """
 
     likelihood = log_likelihood(emp_cov, precision)
     of_nonzero = np.sum(precision != 0) - precision.shape[0]
-    penalty = np.log(n) / n * of_nonzero + 4 * epsilon * np.log(precision.shape[0]) / n * of_nonzero
+    penalty = (
+        np.log(n) / n * of_nonzero
+        + 4 * epsilon * np.log(precision.shape[0]) / n * of_nonzero
+    )
     return likelihood - penalty
 
 
 def EBIC_m(emp_cov, precision, n=100, epsilon=0.5):
     """E - Bayesian Information Criterion for Gaussian models.
 
-    It penalizes more then BIC and E-BIC by multplying the degrees of freedom
+    It penalizes more than BIC and E-BIC by multplying the degrees of freedom
     based on sample size and the number of variables.
     """
     likelihood = log_likelihood(emp_cov, precision)
     of_nonzero = np.sum(precision != 0) - precision.shape[0]
     p = precision.shape[0]
-    penalty = np.log(n) / n * of_nonzero + 4 * epsilon * np.log(p * (p - 1) / 2) / n * of_nonzero
+    penalty = (
+        np.log(n) / n * of_nonzero
+        + 4 * epsilon * np.log(p * (p - 1) / 2) / n * of_nonzero
+    )
     return likelihood - penalty
 
 
-def log_likelihood_t(emp_cov, precision):
-    """Gaussian log-likelihood without constant term in time"""
-    score = 0
-    for e, p in zip(emp_cov, precision):
-        score += fast_logdet(p) - np.sum(e * p)
-    return score
-
-
 def BIC_t(emp_cov, precision):
     """Bayesian Information Criterion for Gaussian models in time."""
 
     precision = np.array(precision)
-    return log_likelihood_t(emp_cov, precision) - (np.sum(precision != 0) - precision.shape[1] * precision.shape[0])
+    return log_likelihood_t(emp_cov, precision) - (
+        np.sum(precision != 0) - precision.shape[1] * precision.shape[0]
+    )
 
 
 def EBIC_t(emp_cov, precision, n=100, epsilon=0.5):
     """E - Bayesian Information Criterion for Gaussian models in time.
 
-    It penalizes more then BIC by multplying the degrees of freedom also based
-    on sample size.
+    It penalizes more than BIC by multiplying the degrees of freedom
+    also based on sample size.
     """
     likelihood = log_likelihood_t(emp_cov, precision)
     n_variables = precision.shape[1] * precision.shape[0]
     of_nonzero = np.sum(precision != 0) - n_variables
-    penalty = np.log(n) / n * of_nonzero + 4 * epsilon * np.log(n_variables) / n * of_nonzero
+    penalty = (
+        np.log(n) / n * of_nonzero + 4 * epsilon * np.log(n_variables) / n * of_nonzero
+    )
     return likelihood - penalty
 
 
 def EBIC_m_t(emp_cov, precision, n=100, epsilon=0.5):
     """E - Bayesian Information Criterion for Gaussian models in time.
 
-    It penalizes more then BIC and E-BIC by multplying the degrees of freedom
+    It penalizes more than BIC and E-BIC by multiplying the degrees of freedom
     based on sample size and the number of variables.
     """
     likelihood = log_likelihood_t(emp_cov, precision)
     n_variables = precision.shape[1] * precision.shape[0]
     of_nonzero = np.sum(precision != 0) - n_variables
-    penalty = np.log(n) / n * of_nonzero + 4 * epsilon * np.log(n_variables * (n_variables - 1) / 2) / n * of_nonzero
+    penalty = (
+        np.log(n) / n * of_nonzero
+        + 4 * epsilon * np.log(n_variables * (n_variables - 1) / 2) / n * of_nonzero
+    )
     return likelihood - penalty
```

### Comparing `regain-0.3.8/regain/update_rules.py` & `regain-0.3.9/regain/update_rules.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/utils.py` & `regain-0.3.9/regain/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,51 +27,60 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Utils for REGAIN package."""
 from __future__ import division
 
-import collections
 import functools
 import logging
 import os
 import sys
 import warnings
 from contextlib import contextmanager
+from dataclasses import dataclass
 
 import numpy as np
 import six
 from numpy.linalg.linalg import LinAlgError
 from scipy import stats
 from scipy.spatial.distance import squareform
 from six.moves import cPickle as pkl
 from sklearn.metrics import average_precision_score, matthews_corrcoef
 
 
-def display_topics(H, W, feature_names, documents, n_top_words, n_top_documents, print_docs=True):
+def display_topics(
+    H, W, feature_names, documents, n_top_words, n_top_documents, print_docs=True
+):
     """Display topics of LDA."""
     topics = []
     for topic_idx, topic in enumerate(H):
         topics.append(
-            " ".join([feature_names[i] + " (%.3f)" % topic[i] for i in topic.argsort()[: -n_top_words - 1 : -1]])
+            " ".join(
+                [
+                    feature_names[i] + " (%.3f)" % topic[i]
+                    for i in topic.argsort()[: -n_top_words - 1 : -1]
+                ]
+            )
         )
 
         print("Topic %d: %s" % (topic_idx, topics[-1]))
         top_doc_indices = np.argsort(W[:, topic_idx])[::-1][:n_top_documents]
         if print_docs:
             for i, doc_index in enumerate(top_doc_indices):
                 print("doc %d: %s" % (doc_index, documents[doc_index]))
     return topics
 
 
 def logentropy_normalize(X):
     """Log-entropy normalisation."""
     P = X / X.values.sum(axis=0, keepdims=True)
-    E = 1 + (P * np.log(P)).fillna(0).values.sum(axis=0, keepdims=True) / np.log1p(X.shape[0])
+    E = 1 + (P * np.log(P)).fillna(0).values.sum(axis=0, keepdims=True) / np.log1p(
+        X.shape[0]
+    )
     return E * np.log1p(X)
 
 
 def top_n_indexes(arr, n):
     import bottleneck as bn
 
     idx = bn.argpartition(arr, arr.size - n, axis=None)[-n:]
@@ -83,26 +92,28 @@
     """Discard low values in a matrix."""
     mask_array = np.zeros_like(arr)
     for idx in top_n_indexes(np.abs(arr), n):
         mask_array[idx] = arr[idx]
     return mask_array
 
 
-def namedtuple_with_defaults(typename, field_names, default_values=()):
-    T = collections.namedtuple(typename, field_names)
-    T.__new__.__defaults__ = (None,) * len(T._fields)
-    if isinstance(default_values, collections.Mapping):
-        prototype = T(**default_values)
-    else:
-        prototype = T(*default_values)
-    T.__new__.__defaults__ = tuple(prototype)
-    return T
-
-
-convergence = namedtuple_with_defaults("convergence", "obj rnorm snorm e_pri e_dual precision")
+@dataclass
+class Convergence:
+    obj: float = 0
+    rnorm: float = 0
+    snorm: float = 0
+    e_pri: float = 0
+    e_dual: float = 0
+    precision: float = 0
+
+    def __str__(self):
+        return (
+            f"obj: {self.obj:.4f}, rnorm: {self.rnorm:.4f}, snorm: {self.snorm:.4f},"
+            f"eps_pri: {self.e_pri:.4f}, eps_dual: {self.e_dual:.4f}"
+        )
 
 
 @contextmanager
 def suppress_stdout():
     """Suppress function output.
 
     Usage
@@ -119,15 +130,19 @@
             sys.stdout = old_stdout
 
 
 def _ensure_filename_ending(filename, possible_extensions=".txt"):
     if isinstance(possible_extensions, six.string_types):
         possible_extensions = [possible_extensions]
 
-    return filename + ("" if any(filename.endswith(end) for end in possible_extensions) else possible_extensions[0])
+    return filename + (
+        ""
+        if any(filename.endswith(end) for end in possible_extensions)
+        else possible_extensions[0]
+    )
 
 
 def init_logger(filename, verbose=True):
     """Initialise logger."""
     logfile = _ensure_filename_ending(filename, [".log", ".txt"])
     logging.shutdown()
     root_logger = logging.getLogger()
@@ -137,19 +152,24 @@
         _.close()
     for _ in list(root_logger.filters):
         root_logger.removeFilter(_)
         _.flush()
         _.close()
 
     logging.basicConfig(
-        filename=logfile, level=logging.INFO, filemode="w", format="%(levelname)s (%(asctime)-15s): %(message)s"
+        filename=logfile,
+        level=logging.INFO,
+        filemode="w",
+        format="%(levelname)s (%(asctime)-15s): %(message)s",
     )
     stream_handler = logging.StreamHandler()
     stream_handler.setLevel(logging.INFO if verbose else logging.ERROR)
-    stream_handler.setFormatter(logging.Formatter("%(levelname)s (%(asctime)-15s): %(message)s"))
+    stream_handler.setFormatter(
+        logging.Formatter("%(levelname)s (%(asctime)-15s): %(message)s")
+    )
 
     root_logger.addHandler(stream_handler)
     return logfile
 
 
 def save_pickle(obj, filename):
     """Save pickle utility."""
@@ -166,15 +186,17 @@
 
 
 def write_network(dataframe, filename):
     """Write a network as a list of interactions."""
     dataframe.stack().to_csv(filename)
 
 
-def read_network(filename, threshold=1.0, full_network=True, fill_diagonal=True, delimiter="auto"):
+def read_network(
+    filename, threshold=1.0, full_network=True, fill_diagonal=True, delimiter="auto"
+):
     """Read a network from a list of interactions.
 
     Parameters
     ----------
     filename : str
         Filename to read from.
     threshold : float, optional
@@ -225,15 +247,19 @@
     if fill_diagonal:
         np.fill_diagonal(net_julia.values, net_julia.sum(axis=1).values)
     return net_julia
 
 
 def flatten(lst):
     """Flatten a list."""
-    return [y for l in lst for y in flatten(l)] if isinstance(lst, (list, np.ndarray)) else [lst]
+    return (
+        [y for l in lst for y in flatten(l)]
+        if isinstance(lst, (list, np.ndarray))
+        else [lst]
+    )
 
 
 def upper_to_full(a):
     """Convert the upper part to a full symmetric matrix."""
     n = int((np.sqrt(1 + 8 * a.shape[0]) - 1) / 2)
     A = np.zeros((n, n))
     idx = np.triu_indices(n)
@@ -254,15 +280,19 @@
     """Utility to help move to the new API.
 
     Data are 3 dimensional with the first dimension representing classes or
     time. The first dimension is compressed, and the belongin of the samples
     to the class is encoded in y.
     """
     X = np.vstack(data)
-    y = np.array([np.ones(x.shape[0]) * i for i, x in enumerate(data)]).flatten().astype(int)
+    y = (
+        np.array([np.ones(x.shape[0]) * i for i, x in enumerate(data)])
+        .flatten()
+        .astype(int)
+    )
     return X, y
 
 
 def error_rank(ells_true, ells_pred):
     """Compute the mean absolute error in rank between two matrices.
 
     Parameters
@@ -281,15 +311,22 @@
     d = np.diag(x).reshape(1, x.shape[0])
     d = 1.0 / np.sqrt(d)
     x *= d
     x *= d.T
 
 
 def error_norm(
-    cov, comp_cov, norm="frobenius", scaling=True, squared=True, upper_triangular=False, nonzero=False, n=False
+    cov,
+    comp_cov,
+    norm="frobenius",
+    scaling=True,
+    squared=True,
+    upper_triangular=False,
+    nonzero=False,
+    n=False,
 ):
     """Mean Squared Error between two covariance estimators.
 
     Parameters
     ----------
     cov, comp_cov : array-like, shape = [n_features, n_features]
         The covariance to compare with.
@@ -330,25 +367,28 @@
     if nonzero:
         comp_cov = comp_cov[np.where(cov == 0)]
         cov = cov[np.where(cov == 0)]
 
     error = comp_cov - cov
     # compute the error norm
     if norm == "frobenius":
-        squared_norm = np.sum(error ** 2)
+        squared_norm = np.sum(error**2)
     elif norm == "spectral":
         squared_norm = np.amax(np.linalg.svdvals(np.dot(error.T, error)))
     else:
         raise NotImplementedError("Only spectral and frobenius norms are implemented")
     # optionally scale the error norm
     if scaling:
         scaling_factor = (
             error.shape[0]
             if len(error.shape) < 3
-            else (np.prod(error.shape[:2]) * ((error.shape[1] - 1) / 2.0 if upper_triangular else error.shape[1]))
+            else (
+                np.prod(error.shape[:2])
+                * ((error.shape[1] - 1) / 2.0 if upper_triangular else error.shape[1])
+            )
         )
         squared_norm = squared_norm / scaling_factor
     # finally get either the squared norm or the norm
     if squared:
         result = squared_norm
     else:
         result = np.sqrt(squared_norm)
@@ -380,15 +420,20 @@
 
     Returns
     -------
     The Mean Squared Error (in the sense of the Frobenius norm) between
     `self` and `comp_cov` covariance estimators.
 
     """
-    return np.mean([error_norm(x, y, norm=norm, scaling=scaling, squared=squared) for x, y in zip(cov, comp_cov)])
+    return np.mean(
+        [
+            error_norm(x, y, norm=norm, scaling=scaling, squared=squared)
+            for x, y in zip(cov, comp_cov)
+        ]
+    )
 
 
 def structure_error(true, pred, thresholding=False, eps=1e-2, no_diagonal=False):
     """Error in structure between a precision matrix and predicted.
 
     Parameters
     ----------
@@ -453,20 +498,24 @@
 
     fall_out = FP / (FP + TN) if (FP + TN) > 0 else 1
     specificity = TN / (FP + TN) if (FP + TN) > 0 else 1.0 - fall_out
 
     balanced_accuracy = 0.5 * (recall + specificity)
     false_discovery_rate = FP / (TP + FP) if TP + FP > 0 else 1 - precision
     false_omission_rate = FN / (FN + TN) if FN + TN > 0 else 0
-    negative_predicted_value = TN / (FN + TN) if FN + TN > 0 else 1 - false_omission_rate
+    negative_predicted_value = (
+        TN / (FN + TN) if FN + TN > 0 else 1 - false_omission_rate
+    )
 
     positive_likelihood_ratio = recall / fall_out if fall_out > 0 else 0
     negative_likelihood_ratio = miss_rate / specificity if specificity > 0 else 0
     diagnostic_odds_ratio = (
-        positive_likelihood_ratio / negative_likelihood_ratio if negative_likelihood_ratio > 0 else 0
+        positive_likelihood_ratio / negative_likelihood_ratio
+        if negative_likelihood_ratio > 0
+        else 0
     )
 
     dictionary = dict(
         tp=TP,
         tn=TN,
         fp=FP,
         fn=FN,
```

### Comparing `regain-0.3.8/regain/validation.py` & `regain-0.3.9/regain/validation.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/wrapper/__init__.py` & `regain-0.3.9/regain/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain/wrapper/paspal/glopridu.py` & `regain-0.3.9/regain/wrapper/paspal/glopridu.py`

 * *Files identical despite different names*

### Comparing `regain-0.3.8/regain.egg-info/PKG-INFO` & `regain-0.3.9/regain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: regain
-Version: 0.3.8
+Version: 0.3.9
 Summary: REGAIN (Regularised Graph Inference)
 Home-page: https://github.com/fdtomasi/regain
-Download-URL: https://github.com/fdtomasi/regain/archive/v0.3.8.tar.gz
+Download-URL: https://github.com/fdtomasi/regain/archive/v0.3.9.tar.gz
 Author: Federico Tomasi
 Author-email: fdtomasi@gmail.com
 Maintainer: Federico Tomasi
 Maintainer-email: fdtomasi@gmail.com
 License: FreeBSD
 Keywords: graph inference,latent variables
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,16 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
 
-[![develstat](https://travis-ci.com/fdtomasi/regain.svg?branch=master)](https://travis-ci.org/fdtomasi/regain) [![covdevel](http://codecov.io/github/fdtomasi/regain/coverage.svg?branch=master)](http://codecov.io/github/fdtomasi/regain?branch=master) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
+![build](https://github.com/fdtomasi/regain/actions/workflows/python-package.yml/badge.svg)
+[![codecov](https://codecov.io/gh/fdtomasi/regain/branch/master/graph/badge.svg?token=1eLrec0OsI)](https://codecov.io/gh/fdtomasi/regain) [![licence](https://img.shields.io/badge/licence-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause) [![PyPI](https://img.shields.io/pypi/v/regain.svg)](https://pypi.python.org/pypi/regain) [![Conda](https://img.shields.io/conda/v/fdtomasi/regain.svg)](https://anaconda.org/fdtomasi/regain)
 
 # regain
 Regularised graph inference across multiple time stamps, considering the influence of latent variables.
 It inherits functionalities from the [scikit-learn](https://github.com/scikit-learn/scikit-learn) package.
 
 ## Getting started
 ### Dependencies
```

### Comparing `regain-0.3.8/regain.egg-info/SOURCES.txt` & `regain-0.3.9/regain.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 regain/__init__.py
 regain/clustering.py
 regain/discriminant_analysis.py
+regain/math.py
 regain/norm.py
 regain/prox.py
 regain/scores.py
 regain/update_rules.py
 regain/utils.py
 regain/validation.py
 regain.egg-info/PKG-INFO
```

### Comparing `regain-0.3.8/setup.py` & `regain-0.3.9/setup.py`

 * *Files identical despite different names*

