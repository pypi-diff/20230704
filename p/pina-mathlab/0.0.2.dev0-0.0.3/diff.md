# Comparing `tmp/pina-mathlab-0.0.2.dev0.tar.gz` & `tmp/pina-mathlab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PINA/PINA/dist/.tmp-idoflel_/pina-mathlab-0.0.2.dev0.tar", last modified: Wed Apr 19 08:09:22 2023, max compression
+gzip compressed data, was "/home/runner/work/PINA/PINA/dist/.tmp-xxd368s9/pina-mathlab-0.0.3.tar", last modified: Tue Jul  4 11:39:51 2023, max compression
```

## Comparing `pina-mathlab-0.0.2.dev0.tar` & `pina-mathlab-0.0.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_cos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_sin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_softplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_square.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/chebyshev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/label_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/location.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/model/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/deeponet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/feed_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/convolution_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/integral.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/stride.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/utils_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/multi_feed_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/pinn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/problem/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/parametric_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/spatial_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/timedep_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/span.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_deeponet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_fnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_label_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_pinn.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/adaptive_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_cos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_sin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_softplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_square.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/label_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/deeponet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/feed_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/model/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/convolution_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/stride.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/utils_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/multi_feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/pinn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/parametric_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/spatial_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/timedep_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_deeponet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_fnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_label_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_pinn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_utils.py
```

### Comparing `pina-mathlab-0.0.2.dev0/LICENSE.rst` & `pina-mathlab-0.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/PKG-INFO` & `pina-mathlab-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pina-mathlab
-Version: 0.0.2.dev0
+Version: 0.0.3
 Summary: Physic Informed Neural networks for Advance modeling.
 Home-page: https://github.com/mathLab/PINA
 Author: Nicola Demo, Maria Strazzullo
 Author-email: demo.nicola@gmail.com, 
 License: MIT
 Keywords: physics-informed neural-network
 Classifier: Development Status :: 3 - Alpha
@@ -15,8 +15,8 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.rst
 
-PINA is a Python package providing an easy interface to deal with physics-informed neural networks (PINN) for the approximation of (differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a simple and intuitive way to formalize a specific problem and solve it using PINN.
+PINA is a Python package providing an easy interface to deal with physics-informed neural networks (PINN) for the approximation of (differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a simple and intuitive way to formalize a specific problem and solve it using PINN. The approximated solution of a differential equation can be implemented using PINA in a few lines of code thanks to the intuitive and user-friendly interface.
```

### Comparing `pina-mathlab-0.0.2.dev0/README.md` & `pina-mathlab-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 	<!-- * [Recent works with PyDMD](#recent-works-with-pydmd) -->
 * [Authors and contributors](#authors-and-contributors)
 * [How to contribute](#how-to-contribute)
 	* [Submitting a patch](#submitting-a-patch)
 * [License](#license)
 
 ## Description
-**PINA** is a Python package providing an easy interface to deal with *physics-informed neural networks* (PINN) for the approximation of (differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a simple and intuitive way to formalize a specific problem and solve it using PINN.
+**PINA** is a Python package providing an easy interface to deal with *physics-informed neural networks* (PINN) for the approximation of (differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a simple and intuitive way to formalize a specific problem and solve it using PINN. The approximated solution of a differential equation can be implemented using PINA in a few lines of code thanks to the intuitive and user-friendly interface.
+
+<p align="center">
+    <a href="http://mathlab.github.io/PINA/" target="_blank" >
+    <img alt="PINA interface for solving problems." src="readme/API_color.png" width="400" />
+    </a>
+</p>
+
 
 #### Physics-informed neural network
 PINN is a novel approach that involves neural networks to solve supervised learning tasks while respecting any given law of physics described by general nonlinear differential equations. Proposed in *"Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations"*, such framework aims to solve problems in a continuous and nonlinear settings.
 
 #### Problem definition
 First step is formalization of the problem in the PINA framework. We take as example here a simple Poisson problem, but PINA is already able to deal with **multi-dimensional**, **parametric**, **time-dependent** problems.
 Consider:
@@ -158,22 +165,21 @@
 * Raissi, Maziar, Paris Perdikaris, and George E. Karniadakis.
   *Physics-informed neural networks: A deep learning framework for solving
   forward and inverse problems involving nonlinear partial differential
   equations.* Journal of Computational Physics 378 (2019): 686-707.
 
 
 ## Authors and contributors
-**PINA** is currently developed and mantained at [SISSA mathLab](http://mathlab.sissa.it/) by
-* [Nicola Demo](mailto:demo.nicola@gmail.com)
-* [Maria Strazzullo](mailto:mstrazzu@gmail.com)
-
+We warmly thank all the contributors that have supported PINA!
 
-under the supervision of [Prof. Gianluigi Rozza](mailto:gianluigi.rozza@sissa.it).
+<a href="https://github.com/mathLab/PINA/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=mathLab/PINA" />
+</a>
 
-Contact us by email for further information or questions about **PINA**, or suggest pull requests. Contributions improving either the code or the documentation are welcome!
+Made with [contrib.rocks](https://contrib.rocks).
 
 
 ## How to contribute
 We'd love to accept your patches and contributions to this project. There are just a few small guidelines you need to follow.
 
 ### Submitting a patch
```

### Comparing `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_cos.py` & `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_cos.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_exp.py` & `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_exp.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_linear.py` & `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_linear.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_relu.py` & `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_relu.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_sin.py` & `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_sin.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_softplus.py` & `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_softplus.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_square.py` & `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_square.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_tanh.py` & `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_tanh.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/condition.py` & `pina-mathlab-0.0.3/pina/condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,18 @@
             raise TypeError('`input_points` must be a torch.Tensor.')
         if not self._dictvalue_isinstance(kwargs, 'output_points', LabelTensor):
             raise TypeError('`output_points` must be a torch.Tensor.')
         if not self._dictvalue_isinstance(kwargs, 'location', Location):
             raise TypeError('`location` must be a Location.')
 
         if 'function' in kwargs:
-            kwargs['function'] = [kwargs['function']]
+            if not isinstance(kwargs['function'], list):                        
+                kwargs['function'] = [kwargs['function']]
+
 
             for i, func in enumerate(kwargs['function']):
                 if not callable(func):
                     raise TypeError(
                         f'`function[{i}]` must be a callable function.')
 
         for key, value in kwargs.items():
-            setattr(self, key, value)
+            setattr(self, key, value)
```

### Comparing `pina-mathlab-0.0.2.dev0/pina/label_tensor.py` & `pina-mathlab-0.0.3/pina/label_tensor.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/deeponet.py` & `pina-mathlab-0.0.3/pina/model/deeponet.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/feed_forward.py` & `pina-mathlab-0.0.3/pina/model/feed_forward.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/layers/convolution.py` & `pina-mathlab-0.0.3/pina/model/layers/convolution.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/layers/convolution_2d.py` & `pina-mathlab-0.0.3/pina/model/layers/convolution_2d.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/layers/integral.py` & `pina-mathlab-0.0.3/pina/model/layers/integral.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/layers/stride.py` & `pina-mathlab-0.0.3/pina/model/layers/stride.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/layers/utils_convolution.py` & `pina-mathlab-0.0.3/pina/model/layers/utils_convolution.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/multi_feed_forward.py` & `pina-mathlab-0.0.3/pina/model/multi_feed_forward.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/model/network.py` & `pina-mathlab-0.0.3/pina/model/network.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/operators.py` & `pina-mathlab-0.0.3/pina/operators.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/pinn.py` & `pina-mathlab-0.0.3/pina/pinn.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/plotter.py` & `pina-mathlab-0.0.3/pina/plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,28 +182,41 @@
         if filename:
             plt.title('Output {} with parameter {}'.format(components,
                                                            fixed_variables))
             plt.savefig(filename)
         else:
             plt.show()
 
-    def plot_loss(self, pinn, label=None, log_scale=True):
+    def plot_loss(self, pinn, label=None, log_scale=True, filename=None):
         """
         Plot the loss function values during traininig.
 
         :param PINN pinn: the PINN object.
         :param str label: the label to use in the legend, defaults to None.
         :param bool log_scale: If True, the y axis is in log scale. Default is
             True.
+        :param str filename: the file name to save the plot. If None, the plot
+            is not saved. Default is None.
         """
 
         if not label:
             label = str(pinn)
 
         epochs = list(pinn.history_loss.keys())
         loss = np.array(list(pinn.history_loss.values()))
+
+        # if multiple outputs, sum the loss
         if loss.ndim != 1:
-            loss = loss[:, 0]
+            loss = np.sum(loss, axis=1)
 
+        # plot loss
         plt.plot(epochs, loss, label=label)
+        plt.legend()
         if log_scale:
             plt.yscale('log')
+        plt.title('Loss function')
+        plt.xlabel('Epochs')
+        plt.ylabel('Loss')
+
+        # save plot
+        if filename:
+            plt.savefig(filename)
```

### Comparing `pina-mathlab-0.0.2.dev0/pina/problem/abstract_problem.py` & `pina-mathlab-0.0.3/pina/problem/abstract_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/problem/parametric_problem.py` & `pina-mathlab-0.0.3/pina/problem/parametric_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         >>> from pina import Condition, Span
         >>> import torch
         >>>
         >>> class ParametricODE(SpatialProblem, ParametricProblem):
         >>>
         >>>     output_variables = ['u']
         >>>     spatial_domain = Span({'x': [0, 1]})
-        >>>     parameter_domain = Span({'alpha': {1, 10}})
+        >>>     parameter_domain = Span({'alpha': [1, 10]})
         >>>
         >>>     def ode_equation(input_, output_):
         >>>         u_x = grad(output_, input_, components=['u'], d=['x'])
         >>>         u = output_.extract(['u'])
         >>>         alpha = input_.extract(['alpha'])
         >>>         return alpha * u_x - u
         >>>
@@ -39,12 +39,18 @@
         >>>     conditions = {
         >>>         'x0': Condition(Span({'x': 0, 'alpha':[1, 10]}), initial_condition),
         >>>         'D': Condition(Span({'x': [0, 1], 'alpha':[1, 10]}), ode_equation)}
     """
 
     @abstractmethod
     def parameter_domain(self):
+        """
+        The parameters' domain of the problem.
+        """
         pass
 
     @property
     def parameters(self):
+        """
+        The parameters' variables of the problem.
+        """
         return self.parameter_domain.variables
```

### Comparing `pina-mathlab-0.0.2.dev0/pina/problem/spatial_problem.py` & `pina-mathlab-0.0.3/pina/problem/spatial_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/problem/timedep_problem.py` & `pina-mathlab-0.0.3/pina/problem/timedep_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/span.py` & `pina-mathlab-0.0.3/pina/span.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina/utils.py` & `pina-mathlab-0.0.3/pina/utils.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/PKG-INFO` & `pina-mathlab-0.0.3/pina_mathlab.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pina-mathlab
-Version: 0.0.2.dev0
+Version: 0.0.3
 Summary: Physic Informed Neural networks for Advance modeling.
 Home-page: https://github.com/mathLab/PINA
 Author: Nicola Demo, Maria Strazzullo
 Author-email: demo.nicola@gmail.com, 
 License: MIT
 Keywords: physics-informed neural-network
 Classifier: Development Status :: 3 - Alpha
@@ -15,8 +15,8 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.rst
 
-PINA is a Python package providing an easy interface to deal with physics-informed neural networks (PINN) for the approximation of (differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a simple and intuitive way to formalize a specific problem and solve it using PINN.
+PINA is a Python package providing an easy interface to deal with physics-informed neural networks (PINN) for the approximation of (differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a simple and intuitive way to formalize a specific problem and solve it using PINN. The approximated solution of a differential equation can be implemented using PINA in a few lines of code thanks to the intuitive and user-friendly interface.
```

### Comparing `pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/SOURCES.txt` & `pina-mathlab-0.0.3/pina_mathlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/setup.py` & `pina-mathlab-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 URL = 'https://github.com/mathLab/PINA'
 MAIL = meta['__mail__']
 AUTHOR = meta['__author__']
 VERSION = meta['__version__']
 KEYWORDS = 'physics-informed neural-network'
 
 REQUIRED = [
-    'future', 'numpy', 'matplotlib', 'torch'
+    'numpy', 'matplotlib', 'torch'
 ]
 
 EXTRAS = {
     'docs': ['sphinx', 'sphinx_rtd_theme'],
     'test': ['pytest', 'pytest-cov'],
 }
 
 LDESCRIPTION = (
     "PINA is a Python package providing an easy interface to deal with "
     "physics-informed neural networks (PINN) for the approximation of "
-    "(differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a "
-    "simple and intuitive way to formalize a specific problem and solve it "
-    "using PINN."
+    "(differential, nonlinear, ...) functions. Based on Pytorch, PINA "
+    "offers a simple and intuitive way to formalize a specific problem "
+    "and solve it using PINN. The approximated solution of a differential "
+    "equation can be implemented using PINA in a few lines of code thanks "
+    "to the intuitive and user-friendly interface."
 )
 
 setup(
     name=PIPNAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LDESCRIPTION,
```

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_condition.py` & `pina-mathlab-0.0.3/tests/test_condition.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_conv.py` & `pina-mathlab-0.0.3/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_deeponet.py` & `pina-mathlab-0.0.3/tests/test_deeponet.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_fnn.py` & `pina-mathlab-0.0.3/tests/test_fnn.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_label_tensor.py` & `pina-mathlab-0.0.3/tests/test_label_tensor.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_network.py` & `pina-mathlab-0.0.3/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_operators.py` & `pina-mathlab-0.0.3/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_pinn.py` & `pina-mathlab-0.0.3/tests/test_pinn.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.2.dev0/tests/test_utils.py` & `pina-mathlab-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

