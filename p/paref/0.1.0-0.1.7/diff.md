# Comparing `tmp/paref-0.1.0.tar.gz` & `tmp/paref-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paref-0.1.0.tar", last modified: Fri Jun 30 17:42:56 2023, max compression
+gzip compressed data, was "paref-0.1.7.tar", last modified: Tue Jul  4 15:47:54 2023, max compression
```

## Comparing `paref-0.1.0.tar` & `paref-0.1.7.tar`

### file list

```diff
@@ -1,92 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.752595 paref-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 17:42:44.000000 paref-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-30 17:42:56.752595 paref-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-30 17:42:44.000000 paref-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.736595 paref-0.1.0/paref/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.736595 paref-0.1.0/paref/black_box_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/black_box_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.740595 paref-0.1.0/paref/black_box_functions/design_space/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/black_box_functions/design_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 17:42:44.000000 paref-0.1.0/paref/black_box_functions/design_space/bounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.740595 paref-0.1.0/paref/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.740595 paref-0.1.0/paref/interfaces/moo_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/moo_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/moo_algorithms/blackbox_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/moo_algorithms/paref_moo.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/moo_algorithms/stopping_criteria.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.740595 paref-0.1.0/paref/interfaces/pareto_reflections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/pareto_reflections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/pareto_reflections/pareto_reflection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.740595 paref-0.1.0/paref/interfaces/sequences_pareto_reflections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/sequences_pareto_reflections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-30 17:42:44.000000 paref-0.1.0/paref/interfaces/sequences_pareto_reflections/sequence_pareto_reflections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.740595 paref-0.1.0/paref/moo_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.740595 paref-0.1.0/paref/moo_algorithms/minimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/minimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/minimizer/bayesian_expected_improvement_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/minimizer/differential_evolution_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/minimizer/gpr_minimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.744595 paref-0.1.0/paref/moo_algorithms/minimizer/surrogates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/minimizer/surrogates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/minimizer/surrogates/gpr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.744595 paref-0.1.0/paref/moo_algorithms/multi_dimensional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/multi_dimensional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/multi_dimensional/find_1_pareto_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/multi_dimensional/find_all_pareto_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/multi_dimensional/find_edge_points.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.744595 paref-0.1.0/paref/moo_algorithms/stopping_criteria/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/stopping_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/stopping_criteria/convergence_reached.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/stopping_criteria/logical_or_stopping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/stopping_criteria/max_iterations_reached.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/stopping_criteria/no_pareto_point_was_found.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/stopping_criteria/time_limit_reached.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.744595 paref-0.1.0/paref/moo_algorithms/two_dimensional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/two_dimensional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/two_dimensional/expected_hypervolume_improvement_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/two_dimensional/fill_gaps_of_pareto_front_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-30 17:42:44.000000 paref-0.1.0/paref/moo_algorithms/two_dimensional/scan_evenly_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.744595 paref-0.1.0/paref/pareto_reflection_sequences/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.748595 paref-0.1.0/paref/pareto_reflection_sequences/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/generic/next_when_stopping_criteria_met.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/generic/repeating_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.748595 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/avoid_pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/fill_gap_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/find_1_pareto_points_for_all_components_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/find_all_pareto_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/find_edge_points_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/find_maximal_pareto_point_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/grid_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.748595 paref-0.1.0/paref/pareto_reflection_sequences/two_dimensional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/two_dimensional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflection_sequences/two_dimensional/fill_gaps_of_pareto_front_sequence_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.752595 paref-0.1.0/paref/pareto_reflections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/avoid_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/expected_hypervolume_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/fill_gap_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/find_1_pareto_points.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/find_2_pareto_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/find_edge_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/minimize_weighted_norm_to_utopia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.752595 paref-0.1.0/paref/pareto_reflections/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/operations/compose_reflections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/operations/compose_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-30 17:42:44.000000 paref-0.1.0/paref/pareto_reflections/restrict_by_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:42:56.736595 paref-0.1.0/paref.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-30 17:42:56.000000 paref-0.1.0/paref.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-30 17:42:56.000000 paref-0.1.0/paref.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:42:56.000000 paref-0.1.0/paref.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-30 17:42:56.000000 paref-0.1.0/paref.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 17:42:56.000000 paref-0.1.0/paref.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 17:42:44.000000 paref-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 17:42:56.752595 paref-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-30 17:42:44.000000 paref-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.574990 paref-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 15:47:42.000000 paref-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-04 15:47:54.574990 paref-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-04 15:47:42.000000 paref-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.566990 paref-0.1.7/paref/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.566990 paref-0.1.7/paref/black_box_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/black_box_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.566990 paref-0.1.7/paref/black_box_functions/design_space/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/black_box_functions/design_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-04 15:47:42.000000 paref-0.1.7/paref/black_box_functions/design_space/bounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.566990 paref-0.1.7/paref/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.566990 paref-0.1.7/paref/interfaces/moo_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/moo_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/moo_algorithms/blackbox_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/moo_algorithms/paref_moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/moo_algorithms/stopping_criteria.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/interfaces/pareto_reflections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/pareto_reflections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/pareto_reflections/pareto_reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/interfaces/sequences_pareto_reflections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/sequences_pareto_reflections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-04 15:47:42.000000 paref-0.1.7/paref/interfaces/sequences_pareto_reflections/sequence_pareto_reflections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/moo_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/moo_algorithms/minimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/minimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/minimizer/bayesian_expected_improvement_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/minimizer/differential_evolution_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/minimizer/gpr_minimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/moo_algorithms/minimizer/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/minimizer/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/minimizer/surrogates/gpr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/moo_algorithms/multi_dimensional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/multi_dimensional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/multi_dimensional/find_1_pareto_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/multi_dimensional/find_all_pareto_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/multi_dimensional/find_edge_points.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/moo_algorithms/stopping_criteria/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/stopping_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/stopping_criteria/convergence_reached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/stopping_criteria/logical_or_stopping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/stopping_criteria/max_iterations_reached.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/stopping_criteria/no_pareto_point_was_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/stopping_criteria/time_limit_reached.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/moo_algorithms/two_dimensional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/two_dimensional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/two_dimensional/fill_gaps_of_pareto_front_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-04 15:47:42.000000 paref-0.1.7/paref/moo_algorithms/two_dimensional/scan_evenly_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/pareto_reflection_sequences/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.570990 paref-0.1.7/paref/pareto_reflection_sequences/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/generic/next_when_stopping_criteria_met.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/generic/repeating_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.574990 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/avoid_pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/fill_gap_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/find_1_pareto_points_for_all_components_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/find_all_pareto_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/find_edge_points_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/find_maximal_pareto_point_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/grid_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.574990 paref-0.1.7/paref/pareto_reflection_sequences/two_dimensional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/two_dimensional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflection_sequences/two_dimensional/fill_gaps_of_pareto_front_sequence_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.574990 paref-0.1.7/paref/pareto_reflections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/avoid_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/fill_gap_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/find_1_pareto_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/find_2_pareto_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/find_edge_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/minimize_weighted_norm_to_utopia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.574990 paref-0.1.7/paref/pareto_reflections/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/operations/compose_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/operations/compose_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-04 15:47:42.000000 paref-0.1.7/paref/pareto_reflections/restrict_by_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:47:54.566990 paref-0.1.7/paref.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-04 15:47:54.000000 paref-0.1.7/paref.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-04 15:47:54.000000 paref-0.1.7/paref.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:47:54.000000 paref-0.1.7/paref.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 15:47:54.000000 paref-0.1.7/paref.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 15:47:54.000000 paref-0.1.7/paref.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-04 15:47:42.000000 paref-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 15:47:54.574990 paref-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-04 15:47:42.000000 paref-0.1.7/setup.py
```

### Comparing `paref-0.1.0/LICENSE.txt` & `paref-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/PKG-INFO` & `paref-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: paref
-Version: 0.1.0
+Version: 0.1.7
 Summary: Pareto reflection based multi-objective optimization
 Author: Nicolai Palm
 Author-email: nicolaipalm@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: examples_
+Provides-Extra: examples
 Provides-Extra: test
 License-File: LICENSE.txt
 
 [![Python Test & Lint](https://github.com/nicolaipalm/paref/actions/workflows/python-test.yml/badge.svg)](https://github.com/nicolaipalm/paref/actions/workflows/python-test.yml)
 [![Python Version](https://img.shields.io/badge/python-3.9+-blue.svg?style=plastic)](https://www.python.org/downloads/)
 
 
-[documentation]()//[notebooks]()
+[documentation](https://paref.readthedocs.io/en/latest/)//[notebooks](https://github.com/nicolaipalm/paref/tree/main/docs/notebooks)
 
 # Paref - using and building problem tailored MOO
 
 A multi-objective optimization (MOO) problem comes with an idea of what **[
 properties](#what-are-properties-of-pareto-points)** identified (Pareto) points must satisfy.
 The fact that these characteristics are fulfilled is what makes a MOO successful in the first place.
 Why not construct a MOO algorithm which searches exactly for those properties?
 With the language of PAreto REFlections this is now possible.
-This package contains
+This package contains...
 
-- a series of ready-to-use [MOO algorithms](table below) corresponding to frequently targeted properties
-- a framework for you to implement your problem specific MOO algorithm
-- generic and intuitive [interfaces]() for MOO algorithms, blackbox functions and more such that solving an MOO problem with Paref requires minimal effort
-- documentation including [how-to guides](), [examples](), [check sheets]() and Parefs' [architecture]() so that getting started with and using Paref becomes easy
+- a series of ready-to-use [MOO algorithms](https://github.com/nicolaipalm/paref/tree/main/paref/moo_algorithms) corresponding to frequently targeted properties
+- a framework for you to implement your problem tailored MOO algorithm
+- generic and intuitive [interfaces](https://github.com/nicolaipalm/paref/tree/main/paref/interfaces) for MOO algorithms, black-box functions and more, so solving a MOO problem with user-defined properties with Paref requires only minimal effort
 
-See the official [documentation](https://github.com/) for more information.
+See the official [documentation](https://paref.readthedocs.io/en/latest/) for more information.
 
 ## Content
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [What are properties of Pareto points?](#what-are-properties-of-pareto-points)
 
@@ -47,53 +47,37 @@
 
 The official release is available at PyPi:
 
 ```
 pip install paref
 ```
 
-You can clone this repository by running the following command:
-
-```
-git clone https://github.com/nicolaipalm/paref
-cd paref
-pip install
-```
-
-In your python terminal run (hello world where left side of w is pareto front)
-
-```python
-from paref.
-```
-
 ## Usage
 
-> 💡 See the [how-to guides]() for a more detailled description.
-
 Solving an MOO problem with Paref consists of the following steps
 
-0. [Define design and target space]()
-1. Define desired [properties](#what-are-properties-of-pareto-points) of Pareto points
-2. Initialize corresponding [MOO algorithm](link moo algos)
-3. [Implement and initialize bbf](link how to implement bbf)
-4. [Apply problem tailored MOO algorithm to blackbox function](link how to apply moo)
+0. Define design and target space
+1. Define desired properties of Pareto points
+2. Initialize corresponding MOO algorithm
+3. Implement and initialize bbf
+4. Apply problem tailored MOO algorithm to blackbox function
 
 This may look as follows:
 
 0. We use a mathematical test function with three input dimensions all between zero and one (i.e. design space is given by three-dimensional unit cube) and with two output dimensions (i.e. target space is the real plane)
 1. We want to have an idea of the "dimension" of the Pareto front (i.e. the Pareto points representing the minima in
    components) with minimum number of evaluations
-2. Accordingly, we choose the [FindEdgePoints]() algorithm:
+2. Accordingly, we choose the ``FindEdgePoints`` algorithm:
 
 ```python
 from paref.moo_algorithms.multi_dimensional.find_edge_points import FindEdgePoints
 moo = FindEdgePoints()
 ```
 
-3. We [implement](how-to-implement) and initialize the blackbox function in the Paref blackbox function interface
+3. We implement and initialize the blackbox function in the Paref blackbox function interface
 
 ```python
 import numpy as np
 from paref.black_box_functions.design_space.bounds import Bounds
 from paref.interfaces.moo_algorithms.blackbox_function import BlackboxFunction
 
 class TestFunction(BlackboxFunction):
@@ -131,13 +115,13 @@
 The fact that these characteristics are fulfilled is what makes a MOO successful in the first place.
 
 In mathematical terms, we understand properties of Pareto points as being element of a
 (mostly implicit defined) subset of the Pareto front.
 
 They include but are certainly not limited to the following:
 
-|              Property               |                                       Graphic                                        | Example | Algorithm(s) |Sequence|Pareto reflection|
-|:-----------------------------------:|:------------------------------------------------------------------------------------:|:------------:|:------------:|:-----:|:-----:|
-|         Being an edge point         |     ![Edge point](./docs/graphics/plots/reflections/FindEdgePointsSequence.svg)      |||||
-|            Filling a gap            |             ![Fill gap](./docs/graphics/plots/reflections/FillGap2D.svg)             |||||
-|      Being evenly distributed       | ![Edge point](./docs/graphics/plots/reflections/FillGapsOfParetoFrontSequence2D.svg) |||||
-| Being constrained to a defined area |        ![Fill gap](./docs/graphics/plots/reflections/RestrictByPoint.svg)         |||||
+|              Property               |                                       Graphic                                        | Example |                        Algorithm(s)                         |          Sequence           |  Pareto reflection   |
+|:-----------------------------------:|:------------------------------------------------------------------------------------:|:-------:|:-----------------------------------------------------------:|:---------------------------:|:--------------------:|
+|         Being an edge point         |     ![Edge point](./docs/graphics/plots/reflections/FindEdgePointsSequence.svg)      |         |                     ``FindEdgePoints``                      | ``FindEdgePointsSequence``  |                      |
+|            Filling a gap            |             ![Fill gap](./docs/graphics/plots/reflections/FillGap2D.svg)             |         |                                                             |                             |    ``FillGap2D``     |
+|      Being evenly distributed       | ![Edge point](./docs/graphics/plots/reflections/FillGapsOfParetoFrontSequence2D.svg) |         | ``FindEdgePoints`` followed by ``FillGapsOfParetoFront2D``  |                             |                      |
+| Being constrained to a defined area |          ![Fill gap](./docs/graphics/plots/reflections/RestrictByPoint.svg)          |         |                                                             |                             | ``RestrictByPoint``  |
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `paref-0.1.0/README.md` & `paref-0.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [![Python Test & Lint](https://github.com/nicolaipalm/paref/actions/workflows/python-test.yml/badge.svg)](https://github.com/nicolaipalm/paref/actions/workflows/python-test.yml)
 [![Python Version](https://img.shields.io/badge/python-3.9+-blue.svg?style=plastic)](https://www.python.org/downloads/)
 
 
-[documentation]()//[notebooks]()
+[documentation](https://paref.readthedocs.io/en/latest/)//[notebooks](https://github.com/nicolaipalm/paref/tree/main/docs/notebooks)
 
 # Paref - using and building problem tailored MOO
 
 A multi-objective optimization (MOO) problem comes with an idea of what **[
 properties](#what-are-properties-of-pareto-points)** identified (Pareto) points must satisfy.
 The fact that these characteristics are fulfilled is what makes a MOO successful in the first place.
 Why not construct a MOO algorithm which searches exactly for those properties?
 With the language of PAreto REFlections this is now possible.
-This package contains
+This package contains...
 
-- a series of ready-to-use [MOO algorithms](table below) corresponding to frequently targeted properties
-- a framework for you to implement your problem specific MOO algorithm
-- generic and intuitive [interfaces]() for MOO algorithms, blackbox functions and more such that solving an MOO problem with Paref requires minimal effort
-- documentation including [how-to guides](), [examples](), [check sheets]() and Parefs' [architecture]() so that getting started with and using Paref becomes easy
+- a series of ready-to-use [MOO algorithms](https://github.com/nicolaipalm/paref/tree/main/paref/moo_algorithms) corresponding to frequently targeted properties
+- a framework for you to implement your problem tailored MOO algorithm
+- generic and intuitive [interfaces](https://github.com/nicolaipalm/paref/tree/main/paref/interfaces) for MOO algorithms, black-box functions and more, so solving a MOO problem with user-defined properties with Paref requires only minimal effort
 
-See the official [documentation](https://github.com/) for more information.
+See the official [documentation](https://paref.readthedocs.io/en/latest/) for more information.
 
 ## Content
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [What are properties of Pareto points?](#what-are-properties-of-pareto-points)
 
@@ -30,53 +29,37 @@
 
 The official release is available at PyPi:
 
 ```
 pip install paref
 ```
 
-You can clone this repository by running the following command:
-
-```
-git clone https://github.com/nicolaipalm/paref
-cd paref
-pip install
-```
-
-In your python terminal run (hello world where left side of w is pareto front)
-
-```python
-from paref.
-```
-
 ## Usage
 
-> 💡 See the [how-to guides]() for a more detailled description.
-
 Solving an MOO problem with Paref consists of the following steps
 
-0. [Define design and target space]()
-1. Define desired [properties](#what-are-properties-of-pareto-points) of Pareto points
-2. Initialize corresponding [MOO algorithm](link moo algos)
-3. [Implement and initialize bbf](link how to implement bbf)
-4. [Apply problem tailored MOO algorithm to blackbox function](link how to apply moo)
+0. Define design and target space
+1. Define desired properties of Pareto points
+2. Initialize corresponding MOO algorithm
+3. Implement and initialize bbf
+4. Apply problem tailored MOO algorithm to blackbox function
 
 This may look as follows:
 
 0. We use a mathematical test function with three input dimensions all between zero and one (i.e. design space is given by three-dimensional unit cube) and with two output dimensions (i.e. target space is the real plane)
 1. We want to have an idea of the "dimension" of the Pareto front (i.e. the Pareto points representing the minima in
    components) with minimum number of evaluations
-2. Accordingly, we choose the [FindEdgePoints]() algorithm:
+2. Accordingly, we choose the ``FindEdgePoints`` algorithm:
 
 ```python
 from paref.moo_algorithms.multi_dimensional.find_edge_points import FindEdgePoints
 moo = FindEdgePoints()
 ```
 
-3. We [implement](how-to-implement) and initialize the blackbox function in the Paref blackbox function interface
+3. We implement and initialize the blackbox function in the Paref blackbox function interface
 
 ```python
 import numpy as np
 from paref.black_box_functions.design_space.bounds import Bounds
 from paref.interfaces.moo_algorithms.blackbox_function import BlackboxFunction
 
 class TestFunction(BlackboxFunction):
@@ -114,13 +97,13 @@
 The fact that these characteristics are fulfilled is what makes a MOO successful in the first place.
 
 In mathematical terms, we understand properties of Pareto points as being element of a
 (mostly implicit defined) subset of the Pareto front.
 
 They include but are certainly not limited to the following:
 
-|              Property               |                                       Graphic                                        | Example | Algorithm(s) |Sequence|Pareto reflection|
-|:-----------------------------------:|:------------------------------------------------------------------------------------:|:------------:|:------------:|:-----:|:-----:|
-|         Being an edge point         |     ![Edge point](./docs/graphics/plots/reflections/FindEdgePointsSequence.svg)      |||||
-|            Filling a gap            |             ![Fill gap](./docs/graphics/plots/reflections/FillGap2D.svg)             |||||
-|      Being evenly distributed       | ![Edge point](./docs/graphics/plots/reflections/FillGapsOfParetoFrontSequence2D.svg) |||||
-| Being constrained to a defined area |        ![Fill gap](./docs/graphics/plots/reflections/RestrictByPoint.svg)         |||||
+|              Property               |                                       Graphic                                        | Example |                        Algorithm(s)                         |          Sequence           |  Pareto reflection   |
+|:-----------------------------------:|:------------------------------------------------------------------------------------:|:-------:|:-----------------------------------------------------------:|:---------------------------:|:--------------------:|
+|         Being an edge point         |     ![Edge point](./docs/graphics/plots/reflections/FindEdgePointsSequence.svg)      |         |                     ``FindEdgePoints``                      | ``FindEdgePointsSequence``  |                      |
+|            Filling a gap            |             ![Fill gap](./docs/graphics/plots/reflections/FillGap2D.svg)             |         |                                                             |                             |    ``FillGap2D``     |
+|      Being evenly distributed       | ![Edge point](./docs/graphics/plots/reflections/FillGapsOfParetoFrontSequence2D.svg) |         | ``FindEdgePoints`` followed by ``FillGapsOfParetoFront2D``  |                             |                      |
+| Being constrained to a defined area |          ![Fill gap](./docs/graphics/plots/reflections/RestrictByPoint.svg)          |         |                                                             |                             | ``RestrictByPoint``  |
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `paref-0.1.0/paref/black_box_functions/design_space/bounds.py` & `paref-0.1.7/paref/black_box_functions/design_space/bounds.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/interfaces/moo_algorithms/blackbox_function.py` & `paref-0.1.7/paref/interfaces/moo_algorithms/blackbox_function.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/interfaces/moo_algorithms/paref_moo.py` & `paref-0.1.7/paref/interfaces/moo_algorithms/paref_moo.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
         This includes all the dimensions of the target space this MOO supports, i.e. to which this MOO can be applied.
         For example, if the MOO algorithm is a minimization algorithm, then, the only supported dimension is one, i.e.
         this property must return [2].
 
         .. warning::
 
-            If all dimensions are supported, then, this property must return None!
+            If all dimensions are supported, then, this property must return ``None``!
 
         Returns
         -------
         Optional[List[int]]
             list of supported dimensions or None if all dimensions are supported
 
         """
@@ -251,15 +251,15 @@
 
 class CompositionWithParetoReflection(BlackboxFunction):
     """Wrapper for composing a Pareto reflection with a blackbox function in order to obtain a new blackbox function
 
     This class constructs a new blackbox function :math:`p\\circ f` out of a blackbox function :math:`f` and a Pareto
     reflection :math:`p`.
     In particular, its design space is given by the design space of the underlying blackbox function and its target
-    space dimension is given by the dimension of the codomain of the Pareto reflection.
+    space dimension is given by the dimension of the codomain dimension of the Pareto reflection.
 
     .. note::
 
         Calling this blackbox function will call the underlying blackbox function. In particular, this means that
         the result is stored in the underlying blackbox function.
 
     """
```

### Comparing `paref-0.1.0/paref/interfaces/moo_algorithms/stopping_criteria.py` & `paref-0.1.7/paref/interfaces/moo_algorithms/stopping_criteria.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/interfaces/pareto_reflections/pareto_reflection.py` & `paref-0.1.7/paref/interfaces/pareto_reflections/pareto_reflection.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/interfaces/sequences_pareto_reflections/sequence_pareto_reflections.py` & `paref-0.1.7/paref/interfaces/sequences_pareto_reflections/sequence_pareto_reflections.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/moo_algorithms/minimizer/differential_evolution_minimizer.py` & `paref-0.1.7/paref/moo_algorithms/minimizer/differential_evolution_minimizer.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/moo_algorithms/minimizer/gpr_minimizer.py` & `paref-0.1.7/paref/moo_algorithms/minimizer/gpr_minimizer.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/moo_algorithms/minimizer/surrogates/gpr.py` & `paref-0.1.7/paref/moo_algorithms/minimizer/surrogates/gpr.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/moo_algorithms/multi_dimensional/find_1_pareto_points.py` & `paref-0.1.7/paref/moo_algorithms/multi_dimensional/find_1_pareto_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class Find1ParetoPoints(GPRMinimizer):
     """Find 1 Pareto points
 
 
 
-    ..note::
+    .. note::
 
         Use this algorithm if you want to find a 1 Pareto point (i.e. a minimum in some component)
         for each component, f.e. in order to estimate the dimension of the Pareto front.
 
 
     Examples
     --------
```

### Comparing `paref-0.1.0/paref/moo_algorithms/multi_dimensional/find_edge_points.py` & `paref-0.1.7/paref/moo_algorithms/multi_dimensional/find_edge_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class FindEdgePoints(GPRMinimizer):
     """Find edge points of Pareto front
 
 
 
-    ..note::
+    .. note::
 
         Use this algorithm if you want to find the edge points of the Pareto front, if they exist.
         *Notice:* In two dimensions, they always exist. However, in general they are likely to not exist.
         In order to test if the algorithm performed well, it is recommended to search for 1 Pareto points first
         (f.e. by
         :py:class:`this algorithm <paref.moo_algorithms.multi_dimensional.find_1_pareto_points.Find1ParetoPoints>`.)
         and then check if the found Pareto points are really minima in several components
```

### Comparing `paref-0.1.0/paref/moo_algorithms/stopping_criteria/convergence_reached.py` & `paref-0.1.7/paref/moo_algorithms/stopping_criteria/convergence_reached.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/moo_algorithms/stopping_criteria/logical_or_stopping_criteria.py` & `paref-0.1.7/paref/moo_algorithms/stopping_criteria/logical_or_stopping_criteria.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/moo_algorithms/stopping_criteria/max_iterations_reached.py` & `paref-0.1.7/paref/moo_algorithms/stopping_criteria/max_iterations_reached.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/moo_algorithms/two_dimensional/fill_gaps_of_pareto_front_2d.py` & `paref-0.1.7/paref/moo_algorithms/two_dimensional/fill_gaps_of_pareto_front_2d.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 from paref.pareto_reflection_sequences.two_dimensional.fill_gaps_of_pareto_front_sequence_2d import \
     FillGapsOfParetoFrontSequence2D
 
 
 class FillGapsOfParetoFront2D(GPRMinimizer):
     """Fill gaps of Pareto front in two dimensions
 
-
-
-    ..note::
+    .. note::
 
         Use this algorithm if you want to fill (by middle point) the gaps between the currently found Pareto front
         (Pareto front of the evaluations).
 
-    ..warning::
+
+    .. warning::
 
         The algorithm calculates an utopia point under the hood by setting it to the minimum of the components of the
         evaluations.
         If is, therefore, highly recommended to run the
         :py:class:`find edge points algorithm <paref.moo_algorithms.multi_dimensional.find_edge_points.FindEdgePoints>`
         before applying this algorithm.
```

### Comparing `paref-0.1.0/paref/moo_algorithms/two_dimensional/scan_evenly_2d.py` & `paref-0.1.7/paref/moo_algorithms/two_dimensional/scan_evenly_2d.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from paref.pareto_reflections.find_1_pareto_points import Find1ParetoPoints
 
 
 class ScanEvenly2D(GPRMinimizer):
     @property
     def sequence_of_pareto_reflections(self):  # -> SequenceParetoReflections:
         NextWhenStoppingCriteriaMet(stopping_criteria=ConvergenceReached(),
-                                    pareto_reflections=[Find1ParetoPoints(dimension_domain=2, dimension=0),
-                                                        Find1ParetoPoints(dimension_domain=2, dimension=1),
-
-                                                        ])
+                                    pareto_reflections=[
+                                        Find1ParetoPoints(dimension_domain=2, dimension=0),
+                                        Find1ParetoPoints(dimension_domain=2, dimension=1),
+                                        ])
         # TBA: grid search or one pareto points plus fill gaps
         raise NotImplementedError
 
     @property
     def supported_codomain_dimensions(self) -> int:
         # If None then all codomain dimensions are supported
         return 2
```

### Comparing `paref-0.1.0/paref/pareto_reflection_sequences/generic/next_when_stopping_criteria_met.py` & `paref-0.1.7/paref/pareto_reflection_sequences/generic/next_when_stopping_criteria_met.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/pareto_reflection_sequences/generic/repeating_sequence.py` & `paref-0.1.7/paref/pareto_reflection_sequences/generic/repeating_sequence.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/avoid_pareto_front.py` & `paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/avoid_pareto_front.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from paref.interfaces.sequences_pareto_reflections.sequence_pareto_reflections import SequenceParetoReflections
 from paref.pareto_reflections.avoid_points import AvoidPoints
 
 
 class AvoidParetoFront(SequenceParetoReflections):
     """Avoid the Pareto front of the evaluations plus some epsilon
 
-    ..warning::
+    .. warning::
 
         This sequence should only be used if the Pareto points found in each evaluation of the moo
         are too close together (since it
         may cause stability issues in the optimization).
         Then, this sequence is meant to be used as sequence of Pareto reflections parameter in the
         :py:meth:`apply to sequence method
         <paref.interfaces.moo_algorithms.paref_moo.ParefMOO.apply_to_sequence>`.
```

### Comparing `paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/find_1_pareto_points_for_all_components_sequence.py` & `paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/find_1_pareto_points_for_all_components_sequence.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/find_all_pareto_points.py` & `paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/find_all_pareto_points.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/pareto_reflection_sequences/multi_dimensional/find_edge_points_sequence.py` & `paref-0.1.7/paref/pareto_reflection_sequences/multi_dimensional/find_edge_points_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from paref.pareto_reflection_sequences.generic.next_when_stopping_criteria_met import NextWhenStoppingCriteriaMet
 from paref.pareto_reflections.find_edge_points import FindEdgePoints
 
 
 class FindEdgePointsSequence(SequenceParetoReflections):
     """Find all edge points of the Pareto front
 
-    ..warning::
+    .. warning::
 
         This Pareto reflection assumes that there exist edge points
 
     When to use
     -----------
     Use this sequence if you want to determine the edge points of your Pareto front, f.e. if you want
     to know the size of the Pareto front.
```

### Comparing `paref-0.1.0/paref/pareto_reflection_sequences/two_dimensional/fill_gaps_of_pareto_front_sequence_2d.py` & `paref-0.1.7/paref/pareto_reflection_sequences/two_dimensional/fill_gaps_of_pareto_front_sequence_2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     SequenceParetoReflections
 from paref.pareto_reflections.fill_gap_2d import FillGap2D
 
 
 class FillGapsOfParetoFrontSequence2D(SequenceParetoReflections):
     """Fill the gaps in the Pareto front already found
 
-    ..warning::
+    .. warning::
 
         If the approximate Pareto front is far away from the true Pareto front, then, this algorithm might
         tries to get closer to the true Pareto front in advance of filling the gaps.
         In order to prevent this, it is recommended to find the
         edge points of the true Pareto front in advance.
         To do so, you could use
         :py:class:`fill gap
@@ -80,15 +80,14 @@
         PF = PF[PF[:, 0].argsort()]
 
         # Calculate points with maximal distance
         max_norm_index = np.argmax(np.linalg.norm(PF[:-1] - PF[1:], axis=1))
 
         # If utopia point is not given, set it as lower edge of points where gap should be closed
         if self.utopia_point is None:
-            # self.utopia_point = np.min(blackbox_function.y, axis=0)
             utopia_point = np.min(np.array(PF[max_norm_index:max_norm_index + 2]), axis=0)
 
         else:
             utopia_point = self.utopia_point
 
         return FillGap2D(point_1=PF[max_norm_index + 1],
                          point_2=PF[max_norm_index],
```

### Comparing `paref-0.1.0/paref/pareto_reflections/avoid_points.py` & `paref-0.1.7/paref/pareto_reflections/avoid_points.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/pareto_reflections/fill_gap_2d.py` & `paref-0.1.7/paref/pareto_reflections/fill_gap_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         the gap, algorithms based on this Pareto reflection tend to be numerically unstable.
         It is recommended to choose an utopia point which is as close to the gap as possible.
 
     When to use
     -----------
     This Pareto reflection should be used if a Pareto point is desired which lies between two specified points
 
-    ..note::
+    .. note::
 
         This function works best if the two points are Pareto optimal.
 
 
     What it does
     ------------
     The Pareto points of this map are the ones which sit in the middle of the two given points (provided
@@ -32,15 +32,17 @@
         TBA
 
     Examples
     --------
     TBA: Add
     """
 
-    def __init__(self, point_1: np.ndarray, point_2: np.ndarray, utopia_point: np.ndarray, scalar: np.ndarray,
+    def __init__(self, point_1: np.ndarray,
+                 point_2: np.ndarray,
+                 utopia_point: np.ndarray,
                  potency: int = 6):
         """Specify the gap and some utopia point
 
         Parameters
         ----------
         point_1 : np.ndarray
             first point defining the gap
@@ -50,15 +52,14 @@
 
         utopia_point : np.ndarray
             utopia point
 
         potency : int default 6
             potency of underlying weighted norm
         """
-        super().__init__(utopia_point, potency, scalar)
         if point_1.shape != (self.dimension_domain,) or point_2.shape != (
                 self.dimension_domain,) or utopia_point.shape != (self.dimension_domain,):
             raise ValueError('Both points and utopia points must be 1 dimensional arrays of length 2! Shape of '
                              f'utopia_point: {utopia_point.shape}'
                              f'\n point_1: {point_1.shape} '
                              f'\n point_1: {point_2.shape}')
```

### Comparing `paref-0.1.0/paref/pareto_reflections/find_1_pareto_points.py` & `paref-0.1.7/paref/pareto_reflections/find_1_pareto_points.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from typing import Union
-
 import numpy as np
+
 from paref.pareto_reflections.minimize_weighted_norm_to_utopia import MinimizeWeightedNormToUtopia
 
 
 class Find1ParetoPoints(MinimizeWeightedNormToUtopia):
     """Find a Pareto point which is minimal in some specified component
 
     When to use
     -----------
     This Pareto reflection should be used if a Pareto point is desired which lie on the boundary of the Pareto front,
     i.e. are minimal in one component.
 
-    ..note::
+    .. note::
 
         In to dimensions, the edge points of the Pareto front are given by the boundary of the Pareto front.
         I.p. in two dimensions, this Pareto reflection searches for the edge points of the Pareto front.
 
     What it does
     ------------
     The Pareto points of this map are the ones which minimize the weighted sum where one component
@@ -31,19 +30,20 @@
     where :math:`j` is the component in which the minimum is searched.
 
     Examples
     --------
     # TBA: add
     """
 
-    def __init__(self, dimension_domain: int, dimension: int, utopia_point: np.ndarray,
-                 potency: Union[np.ndarray, float], scalar: np.ndarray, epsilon: float = 1e-3):
+    def __init__(self, dimension_domain: int,
+                 dimension: int,
+                 epsilon: float = 1e-3):
         """Specify the dimension of the input domain and the component in which the minimum is searched
 
-        ..warning::
+        .. warning::
 
             The smaller epsilon, the better. However, picking an epsilon too small may lead to an
             unstable optimization.
 
         Parameters
         ----------
         dimension_domain : int
@@ -51,15 +51,14 @@
 
         dimension : int
             component in which the minimum is searched
 
         epsilon : float default 1e-3
             weight on the other components
         """
-        super().__init__(utopia_point, potency, scalar)
         self.epsilon = epsilon
         self.dimension = dimension
         self._dimension_domain = dimension_domain
         self.potency = np.ones(dimension_domain)
         scalar = self.epsilon * np.ones(dimension_domain)
         scalar[self.dimension] = 1
         self.scalar = scalar
```

### Comparing `paref-0.1.0/paref/pareto_reflections/find_edge_points.py` & `paref-0.1.7/paref/pareto_reflections/find_edge_points.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import Union
-
 import numpy as np
 
 from paref.pareto_reflections.minimize_weighted_norm_to_utopia import MinimizeWeightedNormToUtopia
 
 
 class FindEdgePoints(MinimizeWeightedNormToUtopia):
     """Find the edge points of the Pareto front
 
-    ..warning::
+    .. warning::
 
         This Pareto reflection assumes that there exist edge points
 
     When to use
     -----------
     This Pareto reflection should be used if the edge points of the Pareto front are searched.
 
-    ..note::
+    .. note::
 
         In to dimensions, the edge points of the Pareto front always exist.
 
     What it does
     ------------
-    The Pareto points of this map are the ones which minimize the the weighted sum where one component
+    The Pareto points of this map are the ones which minimize the weighted sum where one component
     is given much smaller weight than the others.
 
     Mathematical formula
     --------------------
 
     .. math::
         p(x) = \sum_{i=1,...,n,i\\neq j}\\epsilon x_{i}+ x_j
@@ -34,19 +32,18 @@
     where :math:`j` is the component in which the minimum is searched.
 
     Examples
     --------
     # TBA: add
     """
 
-    def __init__(self, dimension_domain: int, dimension: int, utopia_point: np.ndarray,
-                 potency: Union[np.ndarray, float], scalar: np.ndarray, epsilon: float = 1e-3):
+    def __init__(self, dimension_domain: int, dimension: int, epsilon: float = 1e-3):
         """Specify the dimension of the input domain and the component of which the edge point is searched
 
-        ..warning::
+        .. warning::
 
             The smaller epsilon, the better. However, picking an epsilon too small may lead to an
             unstable optimization.
 
         Parameters
         ----------
         dimension_domain : int
@@ -54,15 +51,14 @@
 
         dimension : int
             component of which the edge point is searched
 
         epsilon : float default 1e-3
             weight on the component
         """
-        super().__init__(utopia_point, potency, scalar)
         self.epsilon = epsilon
         self.dimension = dimension
         self._dimension_domain = dimension_domain
         self.potency = np.ones(dimension_domain)
         scalar = np.ones(dimension_domain)
         scalar[self.dimension] = epsilon
         self.scalar = scalar
```

### Comparing `paref-0.1.0/paref/pareto_reflections/minimize_weighted_norm_to_utopia.py` & `paref-0.1.7/paref/pareto_reflections/minimize_weighted_norm_to_utopia.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from paref.interfaces.pareto_reflections.pareto_reflection import ParetoReflection
 
 
 class MinimizeWeightedNormToUtopia(ParetoReflection):
     """Find the Pareto point closest to some utopia point
     # TBA: not a norm in general rather a polynomial
 
-    ..note::
+    .. note::
 
         # TBA: add
         This Pareto reflection is highly flexible. TBA (used for finding lots of properties, for application: if
         utopia point represents only point which we are looking for...)
 
     When to use
     -----------
```

### Comparing `paref-0.1.0/paref/pareto_reflections/operations/compose_reflections.py` & `paref-0.1.7/paref/pareto_reflections/operations/compose_reflections.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/pareto_reflections/operations/compose_sequences.py` & `paref-0.1.7/paref/pareto_reflections/operations/compose_sequences.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref/pareto_reflections/restrict_by_point.py` & `paref-0.1.7/paref/pareto_reflections/restrict_by_point.py`

 * *Files identical despite different names*

### Comparing `paref-0.1.0/paref.egg-info/PKG-INFO` & `paref-0.1.7/paref.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: paref
-Version: 0.1.0
+Version: 0.1.7
 Summary: Pareto reflection based multi-objective optimization
 Author: Nicolai Palm
 Author-email: nicolaipalm@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: examples_
+Provides-Extra: examples
 Provides-Extra: test
 License-File: LICENSE.txt
 
 [![Python Test & Lint](https://github.com/nicolaipalm/paref/actions/workflows/python-test.yml/badge.svg)](https://github.com/nicolaipalm/paref/actions/workflows/python-test.yml)
 [![Python Version](https://img.shields.io/badge/python-3.9+-blue.svg?style=plastic)](https://www.python.org/downloads/)
 
 
-[documentation]()//[notebooks]()
+[documentation](https://paref.readthedocs.io/en/latest/)//[notebooks](https://github.com/nicolaipalm/paref/tree/main/docs/notebooks)
 
 # Paref - using and building problem tailored MOO
 
 A multi-objective optimization (MOO) problem comes with an idea of what **[
 properties](#what-are-properties-of-pareto-points)** identified (Pareto) points must satisfy.
 The fact that these characteristics are fulfilled is what makes a MOO successful in the first place.
 Why not construct a MOO algorithm which searches exactly for those properties?
 With the language of PAreto REFlections this is now possible.
-This package contains
+This package contains...
 
-- a series of ready-to-use [MOO algorithms](table below) corresponding to frequently targeted properties
-- a framework for you to implement your problem specific MOO algorithm
-- generic and intuitive [interfaces]() for MOO algorithms, blackbox functions and more such that solving an MOO problem with Paref requires minimal effort
-- documentation including [how-to guides](), [examples](), [check sheets]() and Parefs' [architecture]() so that getting started with and using Paref becomes easy
+- a series of ready-to-use [MOO algorithms](https://github.com/nicolaipalm/paref/tree/main/paref/moo_algorithms) corresponding to frequently targeted properties
+- a framework for you to implement your problem tailored MOO algorithm
+- generic and intuitive [interfaces](https://github.com/nicolaipalm/paref/tree/main/paref/interfaces) for MOO algorithms, black-box functions and more, so solving a MOO problem with user-defined properties with Paref requires only minimal effort
 
-See the official [documentation](https://github.com/) for more information.
+See the official [documentation](https://paref.readthedocs.io/en/latest/) for more information.
 
 ## Content
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [What are properties of Pareto points?](#what-are-properties-of-pareto-points)
 
@@ -47,53 +47,37 @@
 
 The official release is available at PyPi:
 
 ```
 pip install paref
 ```
 
-You can clone this repository by running the following command:
-
-```
-git clone https://github.com/nicolaipalm/paref
-cd paref
-pip install
-```
-
-In your python terminal run (hello world where left side of w is pareto front)
-
-```python
-from paref.
-```
-
 ## Usage
 
-> 💡 See the [how-to guides]() for a more detailled description.
-
 Solving an MOO problem with Paref consists of the following steps
 
-0. [Define design and target space]()
-1. Define desired [properties](#what-are-properties-of-pareto-points) of Pareto points
-2. Initialize corresponding [MOO algorithm](link moo algos)
-3. [Implement and initialize bbf](link how to implement bbf)
-4. [Apply problem tailored MOO algorithm to blackbox function](link how to apply moo)
+0. Define design and target space
+1. Define desired properties of Pareto points
+2. Initialize corresponding MOO algorithm
+3. Implement and initialize bbf
+4. Apply problem tailored MOO algorithm to blackbox function
 
 This may look as follows:
 
 0. We use a mathematical test function with three input dimensions all between zero and one (i.e. design space is given by three-dimensional unit cube) and with two output dimensions (i.e. target space is the real plane)
 1. We want to have an idea of the "dimension" of the Pareto front (i.e. the Pareto points representing the minima in
    components) with minimum number of evaluations
-2. Accordingly, we choose the [FindEdgePoints]() algorithm:
+2. Accordingly, we choose the ``FindEdgePoints`` algorithm:
 
 ```python
 from paref.moo_algorithms.multi_dimensional.find_edge_points import FindEdgePoints
 moo = FindEdgePoints()
 ```
 
-3. We [implement](how-to-implement) and initialize the blackbox function in the Paref blackbox function interface
+3. We implement and initialize the blackbox function in the Paref blackbox function interface
 
 ```python
 import numpy as np
 from paref.black_box_functions.design_space.bounds import Bounds
 from paref.interfaces.moo_algorithms.blackbox_function import BlackboxFunction
 
 class TestFunction(BlackboxFunction):
@@ -131,13 +115,13 @@
 The fact that these characteristics are fulfilled is what makes a MOO successful in the first place.
 
 In mathematical terms, we understand properties of Pareto points as being element of a
 (mostly implicit defined) subset of the Pareto front.
 
 They include but are certainly not limited to the following:
 
-|              Property               |                                       Graphic                                        | Example | Algorithm(s) |Sequence|Pareto reflection|
-|:-----------------------------------:|:------------------------------------------------------------------------------------:|:------------:|:------------:|:-----:|:-----:|
-|         Being an edge point         |     ![Edge point](./docs/graphics/plots/reflections/FindEdgePointsSequence.svg)      |||||
-|            Filling a gap            |             ![Fill gap](./docs/graphics/plots/reflections/FillGap2D.svg)             |||||
-|      Being evenly distributed       | ![Edge point](./docs/graphics/plots/reflections/FillGapsOfParetoFrontSequence2D.svg) |||||
-| Being constrained to a defined area |        ![Fill gap](./docs/graphics/plots/reflections/RestrictByPoint.svg)         |||||
+|              Property               |                                       Graphic                                        | Example |                        Algorithm(s)                         |          Sequence           |  Pareto reflection   |
+|:-----------------------------------:|:------------------------------------------------------------------------------------:|:-------:|:-----------------------------------------------------------:|:---------------------------:|:--------------------:|
+|         Being an edge point         |     ![Edge point](./docs/graphics/plots/reflections/FindEdgePointsSequence.svg)      |         |                     ``FindEdgePoints``                      | ``FindEdgePointsSequence``  |                      |
+|            Filling a gap            |             ![Fill gap](./docs/graphics/plots/reflections/FillGap2D.svg)             |         |                                                             |                             |    ``FillGap2D``     |
+|      Being evenly distributed       | ![Edge point](./docs/graphics/plots/reflections/FillGapsOfParetoFrontSequence2D.svg) |         | ``FindEdgePoints`` followed by ``FillGapsOfParetoFront2D``  |                             |                      |
+| Being constrained to a defined area |          ![Fill gap](./docs/graphics/plots/reflections/RestrictByPoint.svg)          |         |                                                             |                             | ``RestrictByPoint``  |
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `paref-0.1.0/paref.egg-info/SOURCES.txt` & `paref-0.1.7/paref.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 paref/moo_algorithms/stopping_criteria/__init__.py
 paref/moo_algorithms/stopping_criteria/convergence_reached.py
 paref/moo_algorithms/stopping_criteria/logical_or_stopping_criteria.py
 paref/moo_algorithms/stopping_criteria/max_iterations_reached.py
 paref/moo_algorithms/stopping_criteria/no_pareto_point_was_found.py
 paref/moo_algorithms/stopping_criteria/time_limit_reached.py
 paref/moo_algorithms/two_dimensional/__init__.py
-paref/moo_algorithms/two_dimensional/expected_hypervolume_improvement_2d.py
 paref/moo_algorithms/two_dimensional/fill_gaps_of_pareto_front_2d.py
 paref/moo_algorithms/two_dimensional/scan_evenly_2d.py
 paref/pareto_reflection_sequences/__init__.py
 paref/pareto_reflection_sequences/generic/__init__.py
 paref/pareto_reflection_sequences/generic/next_when_stopping_criteria_met.py
 paref/pareto_reflection_sequences/generic/repeating_sequence.py
 paref/pareto_reflection_sequences/multi_dimensional/__init__.py
@@ -54,15 +53,14 @@
 paref/pareto_reflection_sequences/multi_dimensional/find_edge_points_sequence.py
 paref/pareto_reflection_sequences/multi_dimensional/find_maximal_pareto_point_sequence.py
 paref/pareto_reflection_sequences/multi_dimensional/grid_search.py
 paref/pareto_reflection_sequences/two_dimensional/__init__.py
 paref/pareto_reflection_sequences/two_dimensional/fill_gaps_of_pareto_front_sequence_2d.py
 paref/pareto_reflections/__init__.py
 paref/pareto_reflections/avoid_points.py
-paref/pareto_reflections/expected_hypervolume_2d.py
 paref/pareto_reflections/fill_gap_2d.py
 paref/pareto_reflections/find_1_pareto_points.py
 paref/pareto_reflections/find_2_pareto_points.py
 paref/pareto_reflections/find_edge_points.py
 paref/pareto_reflections/minimize_weighted_norm_to_utopia.py
 paref/pareto_reflections/restrict_by_point.py
 paref/pareto_reflections/operations/__init__.py
```

### Comparing `paref-0.1.0/setup.py` & `paref-0.1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,36 +4,37 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='paref',
-    version='0.1.0',
+    version='0.1.7',
     license='MIT',
     description='Pareto reflection based multi-objective optimization',
     long_description=readme(),
     long_description_content_type='text/markdown',
     author='Nicolai Palm',
     author_email='nicolaipalm@googlemail.com',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
+        'Development Status :: 3 - Alpha'
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.9',
     install_requires=[
         'numpy',
         'scipy',
         'plotly',
         'gpytorch',
         'torch',
         'matplotlib',
         'tqdm',
     ],
     extras_require={
         'dev': ['pre-commit', 'flake8', 'flake8-print'],
-        'examples_': ['ipython', 'jupyter', 'pymoo'],
-        'test': ['pytest', 'pytest-cov'],  # "nbval"],
+        'examples': ['ipython', 'jupyter', 'pymoo'],
+        'test': ['pytest', 'pytest-cov'],
     },
     test_suite='tests',
 )
```

