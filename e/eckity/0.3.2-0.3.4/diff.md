# Comparing `tmp/eckity-0.3.2.tar.gz` & `tmp/eckity-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eckity-0.3.2.tar", last modified: Tue Jul  4 16:07:32 2023, max compression
+gzip compressed data, was "eckity-0.3.4.tar", last modified: Mon Apr 24 14:24:01 2023, max compression
```

## Comparing `eckity-0.3.2.tar` & `eckity-0.3.4.tar`

### file list

```diff
@@ -1,177 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.706473 eckity-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-04 16:07:20.000000 eckity-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-04 16:07:32.706473 eckity-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-04 16:07:20.000000 eckity-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.674473 eckity-0.3.2/eckity/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.678473 eckity-0.3.2/eckity/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/algorithms/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/algorithms/simple_evolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.678473 eckity-0.3.2/eckity/base/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/before_after_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.678473 eckity-0.3.2/eckity/breeders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/breeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/breeders/breeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/breeders/simple_breeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.678473 eckity-0.3.2/eckity/creators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.682473 eckity-0.3.2/eckity/creators/ga_creators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/ga_creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/ga_creators/bit_string_vector_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/ga_creators/float_vector_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/ga_creators/int_vector_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/ga_creators/simple_vector_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.682473 eckity-0.3.2/eckity/creators/gp_creators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/gp_creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/gp_creators/full.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/gp_creators/grow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/gp_creators/ramped_hh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/creators/gp_creators/tree_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.682473 eckity-0.3.2/eckity/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/evaluators/individual_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/evaluators/population_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/evaluators/simple_individual_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/evaluators/simple_population_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/event_based_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.682473 eckity-0.3.2/eckity/fitness/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/fitness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/fitness/fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/fitness/gp_fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/fitness/simple_fitness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.682473 eckity-0.3.2/eckity/genetic_encodings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.686473 eckity-0.3.2/eckity/genetic_encodings/ga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/bit_string_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/float_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/int_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.686473 eckity-0.3.2/eckity/genetic_encodings/ga/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/tests/test_bit_string_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/tests/test_float_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/tests/test_int_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/ga/vector_individual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.686473 eckity-0.3.2/eckity/genetic_encodings/gp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/gp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.686473 eckity-0.3.2/eckity/genetic_encodings/gp/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/gp/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/gp/tree/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/gp/tree/tree_individual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_encodings/gp/tree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.686473 eckity-0.3.2/eckity/genetic_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.686473 eckity-0.3.2/eckity/genetic_operators/crossovers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/crossovers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/crossovers/subtree_crossover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/crossovers/vector_k_point_crossover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/failable_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/genetic_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.690473 eckity-0.3.2/eckity/genetic_operators/mutations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/mutations/erc_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/mutations/identity_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/mutations/subtree_mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.690473 eckity-0.3.2/eckity/genetic_operators/mutations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/mutations/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/mutations/tests/test_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/mutations/vector_n_point_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/mutations/vector_random_mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.690473 eckity-0.3.2/eckity/genetic_operators/selections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/selections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/selections/elitism_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/selections/selection_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/genetic_operators/selections/tournament_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/individual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.690473 eckity-0.3.2/eckity/multi_objective_evolution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/multi_objective_evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/multi_objective_evolution/crowding_termination_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/multi_objective_evolution/nsga2_breeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/multi_objective_evolution/nsga2_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/multi_objective_evolution/nsga2_fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/multi_objective_evolution/nsga2_front_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/multi_objective_evolution/nsga2_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/population.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.694473 eckity-0.3.2/eckity/sklearn_compatible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/sklearn_compatible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/sklearn_compatible/classification_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/sklearn_compatible/regression_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/sklearn_compatible/sk_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/sklearn_compatible/sk_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/sklearn_compatible/sklearn_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.694473 eckity-0.3.2/eckity/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/statistics/best_average_worst_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/statistics/best_avg_worst_size_tree_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/statistics/minimal_print_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/statistics/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/subpopulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.694473 eckity-0.3.2/eckity/termination_checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/termination_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/termination_checkers/termination_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-04 16:07:20.000000 eckity-0.3.2/eckity/termination_checkers/threshold_from_target_termination_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.678473 eckity-0.3.2/eckity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-04 16:07:32.000000 eckity-0.3.2/eckity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-04 16:07:32.000000 eckity-0.3.2/eckity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:07:32.000000 eckity-0.3.2/eckity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 16:07:32.000000 eckity-0.3.2/eckity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 16:07:32.000000 eckity-0.3.2/eckity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.694473 eckity-0.3.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.694473 eckity-0.3.2/examples/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.694473 eckity-0.3.2/examples/multi_objective/moe_base_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/multi_objective/moe_base_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/multi_objective/moe_base_test/nsga2_basic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.694473 eckity-0.3.2/examples/multi_objective/zdt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/multi_objective/zdt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/multi_objective/zdt/nsga2zdt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/multi_objective/zdt/nsga2zdt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/multi_objective/zdt/nsga2zdt3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.694473 eckity-0.3.2/examples/treegp/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.698473 eckity-0.3.2/examples/treegp/non_sklearn_mode/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/non_sklearn_mode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.698473 eckity-0.3.2/examples/treegp/non_sklearn_mode/multiplexer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/non_sklearn_mode/multiplexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/non_sklearn_mode/multiplexer/mux_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/non_sklearn_mode/multiplexer/mux_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.698473 eckity-0.3.2/examples/treegp/non_sklearn_mode/symbolic_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/non_sklearn_mode/symbolic_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.698473 eckity-0.3.2/examples/treegp/sklearn_mode/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/sklearn_mode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.698473 eckity-0.3.2/examples/treegp/sklearn_mode/breast_cancer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/sklearn_mode/breast_cancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/sklearn_mode/breast_cancer/breast_cancer_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/sklearn_mode/breast_cancer/classification_gridsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.702473 eckity-0.3.2/examples/treegp/sklearn_mode/symbolic_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/sklearn_mode/symbolic_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/sklearn_mode/symbolic_regression/regression_gridsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.702473 eckity-0.3.2/examples/vectorga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/vectorga/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.702473 eckity-0.3.2/examples/vectorga/knapsack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/vectorga/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/vectorga/knapsack/knapsack_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/vectorga/knapsack/knapsack_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.702473 eckity-0.3.2/examples/vectorga/one_max/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/vectorga/one_max/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/vectorga/one_max/one_max_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/vectorga/one_max/one_max_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-04 16:07:20.000000 eckity-0.3.2/examples/vectorga/one_max/one_max_problem_float.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 16:07:32.706473 eckity-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-04 16:07:20.000000 eckity-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.702473 eckity-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:32.706473 eckity-0.3.2/tests/moe_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:07:20.000000 eckity-0.3.2/tests/moe_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-04 16:07:20.000000 eckity-0.3.2/tests/moe_test/test_moe_base_test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-04 16:07:20.000000 eckity-0.3.2/tests/moe_test/test_moe_front_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-04 16:07:20.000000 eckity-0.3.2/tests/test_sklearn_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.621170 eckity-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-24 14:23:50.000000 eckity-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-24 14:24:01.621170 eckity-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-24 14:23:50.000000 eckity-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/algorithms/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/algorithms/simple_evolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/before_after_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity/breeders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/breeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/breeders/breeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/breeders/simple_breeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/creators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/creators/ga_creators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/bit_string_vector_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/float_vector_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/int_vector_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/ga_creators/simple_vector_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/creators/gp_creators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/grow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/ramped_hh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/creators/gp_creators/tree_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/individual_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/population_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/simple_individual_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/evaluators/simple_population_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/event_based_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/fitness/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/fitness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/fitness/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/fitness/gp_fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/fitness/simple_fitness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/genetic_encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.605169 eckity-0.3.4/eckity/genetic_encodings/ga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/bit_string_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/float_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/int_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/ga/vector_individual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_encodings/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_encodings/gp/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/tree/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/tree/tree_individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_encodings/gp/tree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_operators/crossovers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/crossovers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/crossovers/subtree_crossover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/crossovers/vector_k_point_crossover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/failable_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/genetic_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_operators/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/erc_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/identity_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/subtree_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/vector_n_point_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/mutations/vector_random_mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.609169 eckity-0.3.4/eckity/genetic_operators/selections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/selections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/selections/elitism_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/selections/selection_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/genetic_operators/selections/tournament_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/individual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.613170 eckity-0.3.4/eckity/multi_objective_evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/crowding_termination_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_breeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_front_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/multi_objective_evolution/nsga2_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.613170 eckity-0.3.4/eckity/sklearn_compatible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/classification_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/regression_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/sk_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/sk_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/sklearn_compatible/sklearn_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.613170 eckity-0.3.4/eckity/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/best_average_worst_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/best_avg_worst_size_tree_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/minimal_print_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/statistics/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/subpopulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/eckity/termination_checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/termination_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/termination_checkers/termination_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-24 14:23:50.000000 eckity-0.3.4/eckity/termination_checkers/threshold_from_target_termination_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.601169 eckity-0.3.4/eckity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 14:24:01.000000 eckity-0.3.4/eckity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/multi_objective/moe_base_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/moe_base_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/moe_base_test/nsga2_basic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/multi_objective/zdt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/zdt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/non_sklearn_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/mux_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/mux_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/sklearn_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/breast_cancer_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/classification_gridsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/regression_gridsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/vectorga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/vectorga/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/knapsack/knapsack_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/knapsack/knapsack_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.617169 eckity-0.3.4/examples/vectorga/one_max/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/one_max/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/one_max/one_max_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-24 14:23:50.000000 eckity-0.3.4/examples/vectorga/one_max/one_max_problem_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:24:01.621170 eckity-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 14:23:50.000000 eckity-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.621170 eckity-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:24:01.621170 eckity-0.3.4/tests/moe_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/moe_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/moe_test/test_moe_base_test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/moe_test/test_moe_front_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/test_sklearn_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-24 14:23:50.000000 eckity-0.3.4/tests/test_vector.py
```

### Comparing `eckity-0.3.2/LICENSE` & `eckity-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/PKG-INFO` & `eckity-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eckity
-Version: 0.3.2
+Version: 0.3.4
 Summary: EC-KitY: Evolutionary Computation Tool Kit in Python.
 Home-page: https://www.eckity.org
 Author: Moshe Sipper, Achiya Elyasaf, Itai Tzruia, Tomer Halperin
 Author-email: sipper@gmail.com, achiya@bgu.ac.il, itaitz@post.bgu.ac.il, tomerhal@post.bgu.ac.il
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/EC-KitY/EC-KitY/issues
 Description-Content-Type: text/markdown
@@ -23,18 +23,17 @@
 - Written in Python
 - Can work with or without scikit-learn, i.e., supports both sklearn and non-sklearn modes
 - Designed with modern software engineering in mind
 - Designed to support all popular EC paradigms (GA, GP, ES, coevolution, multi-objective, etc').
 
 ### Dependencies
 For the basic evolution mode, EC-KitY requires:
-- Python (>=3.6)
-- Numpy (>=1.14.6)
-- Pandas (>=0.25.0)
-- Overrides (>= 6.1.0)
+- numpy (>=1.14.6)
+- pandas (>=0.25.0)
+- overrides (>= 6.1.0)
 
 For sklearn mode, EC-KitY additionally requires:
 - scikit-learn (>=0.24.2)
 
 ### User installation
 
 `pip install eckity`
```

### Comparing `eckity-0.3.2/README.md` & `eckity-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 - Written in Python
 - Can work with or without scikit-learn, i.e., supports both sklearn and non-sklearn modes
 - Designed with modern software engineering in mind
 - Designed to support all popular EC paradigms (GA, GP, ES, coevolution, multi-objective, etc').
 
 ### Dependencies
 For the basic evolution mode, EC-KitY requires:
-- Python (>=3.6)
-- Numpy (>=1.14.6)
-- Pandas (>=0.25.0)
-- Overrides (>= 6.1.0)
+- numpy (>=1.14.6)
+- pandas (>=0.25.0)
+- overrides (>= 6.1.0)
 
 For sklearn mode, EC-KitY additionally requires:
 - scikit-learn (>=0.24.2)
 
 ### User installation
 
 `pip install eckity`
```

### Comparing `eckity-0.3.2/eckity/algorithms/algorithm.py` & `eckity-0.3.4/eckity/algorithms/algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,24 +42,22 @@
         Responsible for evaluating each individual's fitness concurrently and returns the best
          individual of each subpopulation (returns a single individual in simple case).
 
 	max_generation: int, default=1000
 		Maximal number of generations to run the evolutionary process.
 		Note the evolution could end before reaching max_generation,
 		depends on the termination checker.
-		Note that there are max_generation + 1 (at max) fitness calculations,
-		but only max_generation (at max) of selection
 
 	events: dict(str, dict(object, function)), default=None
 		Dictionary of events, where each event holds a dictionary of (subscriber, callback method).
 
 	event_names: list of strings, default=None
 		Names of events to publish during the evolution.
 
-    termination_checker: TerminationChecker or a list of TerminationCheckers, default=ThresholdFromTargetTerminationChecker()
+    termination_checker: TerminationChecker, default=ThresholdFromTargetTerminationChecker()
         Responsible for checking if the algorithm should finish before reaching max_generation.
 
 	max_workers: int, default=None
 		Maximal number of worker nodes for the Executor object
 		that evaluates the fitness of the individuals.
 
 	random_generator: module, default=random
@@ -179,17 +177,17 @@
 	def evolve(self):
 		"""
 		Performs the evolutionary run by initializing the random seed, creating the population,
 		performing the evolutionary loop and finally finishing the evolution process
 		"""
 		self.initialize()
 
-		if self.should_terminate(self.population,
-                                 self.best_of_run_,
-                                 self.generation_num):
+		if self.termination_checker.should_terminate(self.population,
+													 self.best_of_run_,
+													 self.generation_num):
 			self.final_generation_ = 0
 			self.publish('after_generation')
 		else:
 			self.evolve_main_loop()
 
 		self.finish()
 		self.publish('evolution_finished')
@@ -232,35 +230,29 @@
 		self.best_of_run_ = self.population_evaluator.act(self.population)
 		self.publish('init')
 
 	def evolve_main_loop(self):
 		"""
 		Performs the evolutionary main loop
 		"""
-		# there was already "preprocessing" generation created - gen #0
-		# now create another self.max_generation generations (at maximum), starting for gen #1
-		for gen in range(1, self.max_generation + 1):
+		for gen in range(self.max_generation):
 			self.generation_num = gen
-			self.update_gen(self.population, gen)
 
 			self.set_generation_seed(self.next_seed())
 			self.generation_iteration(gen)
-			if self.should_terminate(self.population, self.best_of_run_, gen):
+			if self.termination_checker.should_terminate(self.population,
+														 self.best_of_run_,
+														 self.generation_num):
 				self.final_generation_ = gen
 				self.publish('after_generation')
 				break
 			self.publish('after_generation')
 
 		self.executor.shutdown()
 
-	def update_gen(self, population, gen):
-		for subpopulation in population.sub_populations:
-			for ind in subpopulation.individuals:
-				ind.gen = gen
-
 	@abstractmethod
 	def generation_iteration(self, gen):
 		"""
 		Performs an iteration of the evolutionary main loop
 
 		Parameters
 		----------
@@ -353,21 +345,15 @@
 		Returns
 		----------
 		int
 			random seed number
 		"""
 		return self.random_generator.randint(SEED_MIN_VALUE, SEED_MAX_VALUE)
 
-	def should_terminate(self, population, best_of_run_, generation_num):
-		if isinstance(self.termination_checker, list):
-			return any([t.should_terminate(population, best_of_run_, generation_num) for t in self.termination_checker])
-		else:
-			return self.termination_checker.should_terminate(population, best_of_run_, generation_num)
-
-    # Necessary for valid pickling, since SimpleQueue object cannot be pickled
+	# Necessary for valid pickling, since SimpleQueue object cannot be pickled
 	def __getstate__(self):
 		state = self.__dict__.copy()
 		del state['executor']
 		del state['random_generator']
 
 		return state
```

### Comparing `eckity-0.3.2/eckity/algorithms/simple_evolution.py` & `eckity-0.3.4/eckity/algorithms/simple_evolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,14 @@
 		-------
 		object
 			Output as computed by the best individual of the evolutionary run.
 
 		"""
 		return self.best_of_run_.execute(**kwargs)
 
-
 	def finish(self):
 		"""
 		Finish the evolutionary run by showing the best individual and printing the best fitness
 		"""
 		# todo should move to finisher
 		self.best_of_run_.show()
 
@@ -189,16 +188,15 @@
 			return {
 				"population": self.population,
 				"statistics": self.statistics,
 				"breeder": self.breeder,
 				"termination_checker": self.termination_checker,
 				"max_generation": self.max_generation,
 				"events": self.events,
-				"max_workers": self.max_workers,
-				"generation_num": self.generation_num,
+				"max_workers": self.max_workers
 			}
 
 		# default case
 		return {
 			"population": self.population,
 			"best_of_run_": self.best_of_run_,
 			"best_of_gen": self.best_of_gen,
```

### Comparing `eckity-0.3.2/eckity/before_after_publisher.py` & `eckity-0.3.4/eckity/before_after_publisher.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/breeders/breeder.py` & `eckity-0.3.4/eckity/breeders/breeder.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/breeders/simple_breeder.py` & `eckity-0.3.4/eckity/breeders/simple_breeder.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/creators/creator.py` & `eckity-0.3.4/eckity/creators/creator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/creators/ga_creators/simple_vector_creator.py` & `eckity-0.3.4/eckity/creators/ga_creators/simple_vector_creator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/creators/gp_creators/full.py` & `eckity-0.3.4/eckity/creators/gp_creators/full.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/creators/gp_creators/grow.py` & `eckity-0.3.4/eckity/creators/gp_creators/grow.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/creators/gp_creators/ramped_hh.py` & `eckity-0.3.4/eckity/creators/gp_creators/ramped_hh.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 		Parameters
 		----------
 		grow_creator: GrowCreator
 			a tree creator that creates trees using the grow method
 
 		full_creator: FullCreator
-			a tree creator that creates trees using the full method
+			a tree creator that creates trees using the grow method
 
 		init_depth : (int, int)
 		Min and max depths of initial random trees. The default is None.
 
 		function_set : list
 			List of functions used as internal nodes in the GP tree. The default is None.
```

### Comparing `eckity-0.3.2/eckity/creators/gp_creators/tree_creator.py` & `eckity-0.3.4/eckity/creators/gp_creators/tree_creator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/evaluators/individual_evaluator.py` & `eckity-0.3.4/eckity/evaluators/individual_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/evaluators/population_evaluator.py` & `eckity-0.3.4/eckity/evaluators/population_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/evaluators/simple_individual_evaluator.py` & `eckity-0.3.4/eckity/evaluators/simple_individual_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/evaluators/simple_population_evaluator.py` & `eckity-0.3.4/eckity/evaluators/simple_population_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/event_based_operator.py` & `eckity-0.3.4/eckity/event_based_operator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/fitness/fitness.py` & `eckity-0.3.4/eckity/fitness/fitness.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         i.e., if it should be minimized or maximized
     """
     def __init__(self,
                  context=None,
                  trials=None,
                  is_evaluated=False,
                  is_relative_fitness=False,
-                 should_cache_between_gens=True,
+                 should_cache_between_gens=False,
                  higher_is_better=False):
         self.context = context
         self.trials = trials
         self._is_evaluated = is_evaluated
         self.is_relative_fitness = is_relative_fitness
         self.should_cache_between_gens = False if is_relative_fitness else should_cache_between_gens
         self.higher_is_better = higher_is_better
@@ -114,14 +114,16 @@
         """
         raise ValueError("better_than is an abstract method in class Fitness")
 
     def set_not_evaluated(self):
         """
         Set this fitness score status to be not evaluated
         """
+        if not self.is_fitness_evaluated():
+            raise ValueError('Fitness already not evaluated')
         self._is_evaluated = False
 
     def is_fitness_evaluated(self):
         """
         Check this fitness score status (if the fitness score is updated)
 
         Returns
```

### Comparing `eckity-0.3.2/eckity/fitness/gp_fitness.py` & `eckity-0.3.4/eckity/fitness/gp_fitness.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/fitness/simple_fitness.py` & `eckity-0.3.4/eckity/fitness/simple_fitness.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         Updates the fitness score to `fitness`
 
         Parameters
         ----------
         fitness: float
             the fitness score to be updated
         """
+        if self._is_evaluated:
+            raise AttributeError('fitness already evaluated and set to', self.fitness)
         self.fitness = fitness
         self._is_evaluated = True
 
     @overrides
     def get_pure_fitness(self):
         """
         Returns the pure fitness score of the individual (before applying balancing methods like bloat control)
```

### Comparing `eckity-0.3.2/eckity/genetic_encodings/ga/bit_string_vector.py` & `eckity-0.3.4/eckity/genetic_encodings/ga/bit_string_vector.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,53 +11,56 @@
     """
     A Bit Vector individual representation for Genetic Algorithms operations.
     It is represented by a list of ones and zeros.
 
     Parameters
     ----------
     fitness : Fitness
-        Fitness handler class.
-        Responsible of keeping the fitness value of the individual.
+        Fitness handler class, responsible of keeping the fitness value of the individual.
 
     length : int
         Vector length - the number of cells in the vector.
 
     bounds : tuple or list of tuples
-        Min/Max values for each vector cell (if of length n),
-        or the minimum and maximum (if of length 1).
+        Min/Max values for each vector cell (if of length n), or the minimum and maximum (if of length 1).
     """
 
     def __init__(self,
                  fitness,
                  length,
-                 bounds=(0, 1),
-                 vector=None):
-        super().__init__(fitness=fitness,
-                         length=length,
-                         bounds=bounds,
-                         vector=vector)
+                 bounds=(0, 1)):
+        super().__init__(fitness=fitness, length=length, bounds=bounds)
 
     def get_random_number_in_bounds(self, index):
         """
-        Return a random number of available cell values (0 or 1),
-        with equal probability.
+        Return a random number of available cell values - 0 or 1, with equal probability.
 
         Parameters
         ----------
         index : int
             cell index
 
         Returns
         -------
         int
             random value according to bounds field
         """
+        # todo check if need to check bounds - is it tuple always?
         return randint(self.bounds[0], self.bounds[1])
 
     def bit_flip(self, index):
         """
-        Flip the bit in the given index.
+        Return a random number of available cell values - 0 or 1, with equal probability.
+
+        Parameters
+        ----------
+        index : int
+            cell index
+
+        Returns
+        -------
+        int
+            random value according to bounds field
         """
-        return self.bounds[1] \
-            if self.cell_value(index) == self.bounds[0] else self.bounds[0]
+        return self.bounds[1] if self.cell_value(index) == self.bounds[0] else self.bounds[0]
 
 # end class bit string vector
```

### Comparing `eckity-0.3.2/eckity/genetic_encodings/ga/float_vector.py` & `eckity-0.3.4/eckity/genetic_encodings/ga/float_vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,18 +21,17 @@
         Vector length - the number of cells in the vector.
 
     bounds : tuple or list of tuples
         Min/Max values for each vector cell (if of length n), or the minimum and maximum (if of length 1).
     """
     def __init__(self,
                  fitness,
-                 length,
-                 bounds=(0.0, 1.0),
-                 vector=None):
-        super().__init__(fitness=fitness, length=length, bounds=bounds, vector=vector)
+                 length=1,
+                 bounds=(0.0, 1.0)):
+        super().__init__(fitness=fitness, length=length, bounds=bounds)
 
     def get_random_number_in_bounds(self, index):
         """
         Return a random number from possible cell values.
 
         Parameters
         ----------
```

### Comparing `eckity-0.3.2/eckity/genetic_encodings/ga/int_vector.py` & `eckity-0.3.4/eckity/genetic_encodings/ga/int_vector.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,17 +25,16 @@
 
     bounds : tuple or list of tuples
         Min/Max values for each vector cell (if of length n), or the minimum and maximum (if of length 1).
     """
     def __init__(self,
                  fitness,
                  length,
-                 bounds=(MIN_BOUND, MAX_BOUND),
-                 vector=None):
-        super().__init__(fitness, length=length, bounds=bounds, vector=vector)
+                 bounds=(MIN_BOUND, MAX_BOUND)):
+        super().__init__(fitness, length=length, bounds=bounds)
 
     def get_random_number_in_bounds(self, index):
         """
         Return a random number from possible cell values, according to bounds.
 
         Parameters
         ----------
```

### Comparing `eckity-0.3.2/eckity/genetic_encodings/ga/vector_individual.py` & `eckity-0.3.4/eckity/genetic_encodings/ga/vector_individual.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,34 +23,24 @@
     bounds : list of tuples
         Min/Max values for each vector cell (if of length n), or the minimum and maximum (if of length 1).
     """
 
     def __init__(self,
                  fitness,
                  bounds,
-                 length,
-                 vector=None):
+                 length=1):
         super().__init__(fitness)
 
         if (type(bounds) == tuple and len(bounds) != 2) \
                 or (type(bounds) == list and len(bounds) != length):
             raise ValueError(f'Bounds must be either a tuple of size 2 or a list of {length} tuples')
 
         self.bounds = bounds
         self.length = length
-        
-        if vector is None:
-            self.vector = []
-        
-        else:
-            if not isinstance(vector, list):
-                raise ValueError(f'Expected vector argument in Vector constructor to be a list, got {type(vector)}')
-            if len(vector) != length:
-                raise ValueError(f'Expected vector argument in Vector constructor to be of length {length}, got {len(vector)}')
-            self.vector = vector
+        self.vector = []
 
     def size(self):
         """
         Compute size of vector.
 
         Returns
         -------
```

### Comparing `eckity-0.3.2/eckity/genetic_encodings/gp/tree/functions.py` & `eckity-0.3.4/eckity/genetic_encodings/gp/tree/functions.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_encodings/gp/tree/tree_individual.py` & `eckity-0.3.4/eckity/genetic_encodings/gp/tree/tree_individual.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_encodings/gp/tree/utils.py` & `eckity-0.3.4/eckity/genetic_encodings/gp/tree/utils.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_operators/crossovers/subtree_crossover.py` & `eckity-0.3.4/eckity/genetic_operators/crossovers/subtree_crossover.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_operators/crossovers/vector_k_point_crossover.py` & `eckity-0.3.4/eckity/genetic_operators/crossovers/vector_k_point_crossover.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_operators/failable_operator.py` & `eckity-0.3.4/eckity/genetic_operators/failable_operator.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,16 +39,14 @@
 
         Parameters
         -------
         payload: object
             relevant data for the applied operator (usually a list of individuals)
         """
         for i in range(self.attempts):
-            print('attempt', i)
-            print(payload[0].applied_operators)
             # attempt to execute the operator
             succeeded, result = self.attempt_operator(payload, i)
 
             # return if succeeded
             if succeeded:
                 return result
         # after all attempts failed, execute the `on_fail` mechanism
```

### Comparing `eckity-0.3.2/eckity/genetic_operators/mutations/erc_mutation.py` & `eckity-0.3.4/eckity/genetic_operators/mutations/erc_mutation.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_operators/mutations/subtree_mutation.py` & `eckity-0.3.4/eckity/genetic_operators/mutations/subtree_mutation.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_operators/mutations/vector_n_point_mutation.py` & `eckity-0.3.4/eckity/genetic_operators/mutations/vector_n_point_mutation.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_operators/mutations/vector_random_mutation.py` & `eckity-0.3.4/eckity/genetic_operators/mutations/vector_random_mutation.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,15 @@
                          events=events,
                          attempts=attempts)
 
     def on_fail(self, payload):
         """
         Handle gauss mutation failure by returning a callable uniform mutation
         """
-        print('reached on fail')
-        print(payload[0].applied_operators)
-        mut = FloatVectorUniformOnePointMutation(self.probability, self.arity, self.events)
+        mut = FloatVectorUniformNPointMutation(1, self.probability, self.arity, self.events)
         return mut.apply_operator(payload)
 
 
 class FloatVectorGaussNPointMutation(VectorNPointMutation):
     """
     Gaussian N Point Float Mutation
     """
```

### Comparing `eckity-0.3.2/eckity/genetic_operators/selections/elitism_selection.py` & `eckity-0.3.4/eckity/genetic_operators/selections/elitism_selection.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,12 @@
         self.higher_is_better = higher_is_better
 
     def select(self, source_inds, dest_inds):
         elites = sorted(source_inds,
                         key=lambda ind: ind.get_augmented_fitness(),
                         reverse=self.higher_is_better)[:self.num_elites]
         for elite in elites:
-            cloned = elite.clone()
-            cloned.selected_by.append(type(self).__name__)
-            dest_inds.append(cloned)
+            dest_inds.append(elite.clone())
         self.selected_individuals = dest_inds
         # TODO shouldn't it be after_operator? why is this needed?
         # self.publish("after_selection")
         return dest_inds
```

### Comparing `eckity-0.3.2/eckity/genetic_operators/selections/selection_method.py` & `eckity-0.3.4/eckity/genetic_operators/selections/selection_method.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/genetic_operators/selections/tournament_selection.py` & `eckity-0.3.4/eckity/genetic_operators/selections/tournament_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,12 +26,10 @@
         # self.publish("after_selection")   # TODO this already publishes 'after_operator' event
 
         return dest_inds
 
     def _pick_tournament_winner(self, tournament):
         winner = tournament[0]
         for participant in tournament[1:]:
-            if participant.better_than(winner):
+            if participant.fitness.better_than(participant, winner.fitness, winner):
                 winner = participant
-        result = winner.clone()
-        result.selected_by.append(type(self).__name__)
-        return result
+        return winner.clone()
```

### Comparing `eckity-0.3.2/eckity/multi_objective_evolution/crowding_termination_checker.py` & `eckity-0.3.4/eckity/multi_objective_evolution/crowding_termination_checker.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/multi_objective_evolution/nsga2_breeder.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_breeder.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/multi_objective_evolution/nsga2_evolution.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_evolution.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/multi_objective_evolution/nsga2_fitness.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_fitness.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/multi_objective_evolution/nsga2_front_sorting.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_front_sorting.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/multi_objective_evolution/nsga2_plot.py` & `eckity-0.3.4/eckity/multi_objective_evolution/nsga2_plot.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/population.py` & `eckity-0.3.4/eckity/population.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/sklearn_compatible/classification_evaluator.py` & `eckity-0.3.4/eckity/sklearn_compatible/classification_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/sklearn_compatible/regression_evaluator.py` & `eckity-0.3.4/eckity/sklearn_compatible/regression_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/sklearn_compatible/sk_classifier.py` & `eckity-0.3.4/eckity/sklearn_compatible/sk_classifier.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/sklearn_compatible/sklearn_wrapper.py` & `eckity-0.3.4/eckity/sklearn_compatible/sklearn_wrapper.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/statistics/best_average_worst_statistics.py` & `eckity-0.3.4/eckity/statistics/best_average_worst_statistics.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/statistics/best_avg_worst_size_tree_statistics.py` & `eckity-0.3.4/eckity/statistics/best_avg_worst_size_tree_statistics.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/statistics/minimal_print_statistics.py` & `eckity-0.3.4/eckity/statistics/minimal_print_statistics.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/statistics/statistics.py` & `eckity-0.3.4/eckity/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/subpopulation.py` & `eckity-0.3.4/eckity/subpopulation.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/termination_checkers/termination_checker.py` & `eckity-0.3.4/eckity/termination_checkers/termination_checker.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity/termination_checkers/threshold_from_target_termination_checker.py` & `eckity-0.3.4/eckity/termination_checkers/threshold_from_target_termination_checker.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/eckity.egg-info/PKG-INFO` & `eckity-0.3.4/eckity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eckity
-Version: 0.3.2
+Version: 0.3.4
 Summary: EC-KitY: Evolutionary Computation Tool Kit in Python.
 Home-page: https://www.eckity.org
 Author: Moshe Sipper, Achiya Elyasaf, Itai Tzruia, Tomer Halperin
 Author-email: sipper@gmail.com, achiya@bgu.ac.il, itaitz@post.bgu.ac.il, tomerhal@post.bgu.ac.il
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/EC-KitY/EC-KitY/issues
 Description-Content-Type: text/markdown
@@ -23,18 +23,17 @@
 - Written in Python
 - Can work with or without scikit-learn, i.e., supports both sklearn and non-sklearn modes
 - Designed with modern software engineering in mind
 - Designed to support all popular EC paradigms (GA, GP, ES, coevolution, multi-objective, etc').
 
 ### Dependencies
 For the basic evolution mode, EC-KitY requires:
-- Python (>=3.6)
-- Numpy (>=1.14.6)
-- Pandas (>=0.25.0)
-- Overrides (>= 6.1.0)
+- numpy (>=1.14.6)
+- pandas (>=0.25.0)
+- overrides (>= 6.1.0)
 
 For sklearn mode, EC-KitY additionally requires:
 - scikit-learn (>=0.24.2)
 
 ### User installation
 
 `pip install eckity`
```

### Comparing `eckity-0.3.2/eckity.egg-info/SOURCES.txt` & `eckity-0.3.4/eckity.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,14 @@
 eckity/fitness/simple_fitness.py
 eckity/genetic_encodings/__init__.py
 eckity/genetic_encodings/ga/__init__.py
 eckity/genetic_encodings/ga/bit_string_vector.py
 eckity/genetic_encodings/ga/float_vector.py
 eckity/genetic_encodings/ga/int_vector.py
 eckity/genetic_encodings/ga/vector_individual.py
-eckity/genetic_encodings/ga/tests/__init__.py
-eckity/genetic_encodings/ga/tests/test_bit_string_vector.py
-eckity/genetic_encodings/ga/tests/test_float_vector.py
-eckity/genetic_encodings/ga/tests/test_int_vector.py
 eckity/genetic_encodings/gp/__init__.py
 eckity/genetic_encodings/gp/tree/__init__.py
 eckity/genetic_encodings/gp/tree/functions.py
 eckity/genetic_encodings/gp/tree/tree_individual.py
 eckity/genetic_encodings/gp/tree/utils.py
 eckity/genetic_operators/__init__.py
 eckity/genetic_operators/failable_operator.py
@@ -64,16 +60,14 @@
 eckity/genetic_operators/crossovers/vector_k_point_crossover.py
 eckity/genetic_operators/mutations/__init__.py
 eckity/genetic_operators/mutations/erc_mutation.py
 eckity/genetic_operators/mutations/identity_transformation.py
 eckity/genetic_operators/mutations/subtree_mutation.py
 eckity/genetic_operators/mutations/vector_n_point_mutation.py
 eckity/genetic_operators/mutations/vector_random_mutation.py
-eckity/genetic_operators/mutations/tests/__init__.py
-eckity/genetic_operators/mutations/tests/test_mutations.py
 eckity/genetic_operators/selections/__init__.py
 eckity/genetic_operators/selections/elitism_selection.py
 eckity/genetic_operators/selections/selection_method.py
 eckity/genetic_operators/selections/tournament_selection.py
 eckity/multi_objective_evolution/__init__.py
 eckity/multi_objective_evolution/crowding_termination_checker.py
 eckity/multi_objective_evolution/nsga2_breeder.py
@@ -120,15 +114,15 @@
 examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py
 examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py
 examples/vectorga/__init__.py
 examples/vectorga/knapsack/__init__.py
 examples/vectorga/knapsack/knapsack_evaluator.py
 examples/vectorga/knapsack/knapsack_main.py
 examples/vectorga/one_max/__init__.py
-examples/vectorga/one_max/one_max_evaluator.py
 examples/vectorga/one_max/one_max_problem.py
 examples/vectorga/one_max/one_max_problem_float.py
 tests/__init__.py
 tests/test_sklearn_compatibility.py
+tests/test_vector.py
 tests/moe_test/__init__.py
 tests/moe_test/test_moe_base_test_eval.py
 tests/moe_test/test_moe_front_selection.py
```

### Comparing `eckity-0.3.2/examples/multi_objective/moe_base_test/nsga2_basic_test.py` & `eckity-0.3.4/examples/multi_objective/moe_base_test/nsga2_basic_test.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/multi_objective/zdt/nsga2zdt1.py` & `eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt1.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/multi_objective/zdt/nsga2zdt2.py` & `eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt2.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/multi_objective/zdt/nsga2zdt3.py` & `eckity-0.3.4/examples/multi_objective/zdt/nsga2zdt3.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/non_sklearn_mode/multiplexer/mux_evaluator.py` & `eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/mux_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/non_sklearn_mode/multiplexer/mux_main.py` & `eckity-0.3.4/examples/treegp/non_sklearn_mode/multiplexer/mux_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_evaluator.py` & `eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_main.py` & `eckity-0.3.4/examples/treegp/non_sklearn_mode/symbolic_regression/sym_reg_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/sklearn_mode/breast_cancer/breast_cancer_main.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/breast_cancer_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/sklearn_mode/breast_cancer/classification_gridsearch.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/breast_cancer/classification_gridsearch.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/sklearn_mode/symbolic_regression/regression_gridsearch.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/regression_gridsearch.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py` & `eckity-0.3.4/examples/treegp/sklearn_mode/symbolic_regression/sklearn_sym_reg_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/vectorga/knapsack/knapsack_evaluator.py` & `eckity-0.3.4/examples/vectorga/knapsack/knapsack_evaluator.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/vectorga/knapsack/knapsack_main.py` & `eckity-0.3.4/examples/vectorga/knapsack/knapsack_main.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/examples/vectorga/one_max/one_max_problem.py` & `eckity-0.3.4/examples/vectorga/one_max/one_max_problem.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,31 @@
 from eckity.genetic_operators.mutations.vector_random_mutation import BitStringVectorFlipMutation, \
     BitStringVectorNFlipMutation
 from eckity.genetic_operators.selections.tournament_selection import TournamentSelection
 from eckity.statistics.best_average_worst_statistics import BestAverageWorstStatistics
 from eckity.subpopulation import Subpopulation
 from eckity.termination_checkers.threshold_from_target_termination_checker import ThresholdFromTargetTerminationChecker
 
-from one_max_evaluator import OneMaxEvaluator
+
+class OneMaxEvaluator(SimpleIndividualEvaluator):
+    def evaluate_individual(self, individual):
+        """
+            Compute the fitness value of a given individual.
+
+            Parameters
+            ----------
+            individual: Vector
+                The individual to compute the fitness value for.
+
+            Returns
+            -------
+            float
+                The evaluated fitness value of the given individual.
+        """
+        return sum(individual.vector)
 
 
 def main():
     # Initialize the evolutionary algorithm
     algo = SimpleEvolution(
         Subpopulation(creators=GABitStringVectorCreator(length=100),
                       population_size=300,
@@ -30,15 +46,15 @@
                       ],
                       selection_methods=[
                           # (selection method, selection probability) tuple
                           (TournamentSelection(tournament_size=3, higher_is_better=True), 1)
                       ]
                       ),
         breeder=SimpleBreeder(),
-        max_workers=1,
+        max_workers=4,
         max_generation=500,
 
         termination_checker=ThresholdFromTargetTerminationChecker(optimal=100, threshold=0.0),
         statistics=BestAverageWorstStatistics()
     )
 
     # evolve the generated initial population
```

### Comparing `eckity-0.3.2/setup.py` & `eckity-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/tests/moe_test/test_moe_base_test_eval.py` & `eckity-0.3.4/tests/moe_test/test_moe_base_test_eval.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/tests/moe_test/test_moe_front_selection.py` & `eckity-0.3.4/tests/moe_test/test_moe_front_selection.py`

 * *Files identical despite different names*

### Comparing `eckity-0.3.2/tests/test_sklearn_compatibility.py` & `eckity-0.3.4/tests/test_sklearn_compatibility.py`

 * *Files identical despite different names*

