# Comparing `tmp/pyvrp-0.3.0.tar.gz` & `tmp/pyvrp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvrp-0.3.0.tar", max compression
+gzip compressed data, was "pyvrp-0.4.1.tar", max compression
```

## Comparing `pyvrp-0.3.0.tar` & `pyvrp-0.4.1.tar`

### file list

```diff
@@ -1,160 +1,167 @@
--rw-r--r--   0        0        0     1082 2023-05-20 09:32:34.248392 pyvrp-0.3.0/LICENSE
--rw-r--r--   0        0        0     2102 2023-05-20 09:32:34.248392 pyvrp-0.3.0/README.md
--rw-r--r--   0        0        0     3248 2023-05-20 09:32:34.248392 pyvrp-0.3.0/build_extensions.py
--rw-r--r--   0        0        0     4855 2023-05-20 09:32:34.272393 pyvrp-0.3.0/meson.build
--rw-r--r--   0        0        0      150 2023-05-20 09:32:34.272393 pyvrp-0.3.0/meson_options.txt
--rw-r--r--   0        0        0     3503 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7123 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/GeneticAlgorithm.py
--rw-r--r--   0        0        0     8810 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/PenaltyManager.py
--rw-r--r--   0        0        0     6686 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/Population.py
--rw-r--r--   0        0        0     2928 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/Result.py
--rw-r--r--   0        0        0     6197 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/Statistics.py
--rw-r--r--   0        0        0     1391 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_CostEvaluator.pyi
--rw-r--r--   0        0        0     6101 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_Individual.pyi
--rw-r--r--   0        0        0      465 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_Matrix.pyi
--rw-r--r--   0        0        0     5128 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_ProblemData.pyi
--rw-r--r--   0        0        0     4086 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_SubPopulation.pyi
--rw-r--r--   0        0        0     1885 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_TimeWindowSegment.pyi
--rw-r--r--   0        0        0      267 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_XorShift128.pyi
--rw-r--r--   0        0        0      520 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/__init__.py
--rw-r--r--   0        0        0     8916 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cli.py
--rw-r--r--   0        0        0      834 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/CostEvaluator.cpp
--rw-r--r--   0        0        0     2201 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/CostEvaluator.h
--rw-r--r--   0        0        0      711 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/CostEvaluator_bindings.cpp
--rw-r--r--   0        0        0     8608 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Individual.cpp
--rw-r--r--   0        0        0     6297 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Individual.h
--rw-r--r--   0        0        0     4312 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Individual_bindings.cpp
--rw-r--r--   0        0        0     2484 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Matrix.h
--rw-r--r--   0        0        0      909 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Matrix_bindings.cpp
--rw-r--r--   0        0        0     1907 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/ProblemData.cpp
--rw-r--r--   0        0        0     3828 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/ProblemData.h
--rw-r--r--   0        0        0     2459 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/ProblemData_bindings.cpp
--rw-r--r--   0        0        0      574 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/README.md
--rw-r--r--   0        0        0     4784 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/SubPopulation.cpp
--rw-r--r--   0        0        0     3115 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/SubPopulation.h
--rw-r--r--   0        0        0     2750 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/SubPopulation_bindings.cpp
--rw-r--r--   0        0        0     3349 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/TimeWindowSegment.h
--rw-r--r--   0        0        0     1215 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/TimeWindowSegment_bindings.cpp
--rw-r--r--   0        0        0      581 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/XorShift128.cpp
--rw-r--r--   0        0        0     2017 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/XorShift128.h
--rw-r--r--   0        0        0      467 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/XorShift128_bindings.cpp
--rw-r--r--   0        0        0     2822 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/crossover/crossover.cpp
--rw-r--r--   0        0        0     1925 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/crossover/crossover.h
--rw-r--r--   0        0        0     8599 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/crossover/selective_route_exchange.cpp
--rw-r--r--   0        0        0      375 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/crossover/selective_route_exchange_bindings.cpp
--rw-r--r--   0        0        0     1007 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/diversity/broken_pairs_distance.cpp
--rw-r--r--   0        0        0      254 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/diversity/broken_pairs_distance_bindings.cpp
--rw-r--r--   0        0        0      659 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/diversity/diversity.h
--rw-r--r--   0        0        0     3011 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/CircleSector.h
--rw-r--r--   0        0        0    11368 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Exchange.h
--rw-r--r--   0        0        0     2173 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Exchange_bindings.cpp
--rw-r--r--   0        0        0    13068 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch.cpp
--rw-r--r--   0        0        0     3613 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch.h
--rw-r--r--   0        0        0     2513 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearchOperator.h
--rw-r--r--   0        0        0     1420 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch_bindings.cpp
--rw-r--r--   0        0        0     3688 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/MoveTwoClientsReversed.cpp
--rw-r--r--   0        0        0      481 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/MoveTwoClientsReversed.h
--rw-r--r--   0        0        0      482 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/MoveTwoClientsReversed_bindings.cpp
--rw-r--r--   0        0        0      970 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Node.cpp
--rw-r--r--   0        0        0     1617 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Node.h
--rw-r--r--   0        0        0     1112 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar.cpp
--rw-r--r--   0        0        0      735 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar.h
--rw-r--r--   0        0        0      436 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar_bindings.cpp
--rw-r--r--   0        0        0     3651 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Route.cpp
--rw-r--r--   0        0        0     4933 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Route.h
--rw-r--r--   0        0        0    10591 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar.cpp
--rw-r--r--   0        0        0     3186 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar.h
--rw-r--r--   0        0        0      420 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar_bindings.cpp
--rw-r--r--   0        0        0     4113 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt.cpp
--rw-r--r--   0        0        0      895 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt.h
--rw-r--r--   0        0        0      409 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt_bindings.cpp
--rw-r--r--   0        0        0       63 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/crossover/__init__.py
--rw-r--r--   0        0        0      374 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/crossover/_selective_route_exchange.pyi
--rw-r--r--   0        0        0     1961 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/crossover/selective_route_exchange.py
--rw-r--r--   0        0        0     8585 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/crossover/tests/test_selective_route_exchange.py
--rw-r--r--   0        0        0       58 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/diversity/__init__.py
--rw-r--r--   0        0        0     1462 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/diversity/_broken_pairs_distance.pyi
--rw-r--r--   0        0        0     1305 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/diversity/tests/test_broken_pairs_distance.py
--rw-r--r--   0        0        0     6601 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/LocalSearch.py
--rw-r--r--   0        0        0      896 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_Exchange.pyi
--rw-r--r--   0        0        0      880 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_LocalSearch.pyi
--rw-r--r--   0        0        0      204 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_MoveTwoClientsReversed.pyi
--rw-r--r--   0        0        0      196 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_RelocateStar.pyi
--rw-r--r--   0        0        0      192 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_SwapStar.pyi
--rw-r--r--   0        0        0      188 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_TwoOpt.pyi
--rw-r--r--   0        0        0      708 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/__init__.py
--rw-r--r--   0        0        0     5149 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/neighbourhood.py
--rw-r--r--   0        0        0        0 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/__init__.py
--rw-r--r--   0        0        0     9154 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_Exchange.py
--rw-r--r--   0        0        0     6376 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_LocalSearch.py
--rw-r--r--   0        0        0     2735 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_MoveTwoClientsReversed.py
--rw-r--r--   0        0        0     3145 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_RelocateStar.py
--rw-r--r--   0        0        0     3027 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_SwapStar.py
--rw-r--r--   0        0        0     2166 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_TwoOpt.py
--rw-r--r--   0        0        0     6092 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_neighbourhood.py
--rw-r--r--   0        0        0      392 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/exceptions.py
--rw-r--r--   0        0        0      436 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/__init__.py
--rw-r--r--   0        0        0     1106 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_coordinates.py
--rw-r--r--   0        0        0     1046 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_demands.py
--rw-r--r--   0        0        0     1199 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_diversity.py
--rw-r--r--   0        0        0     1129 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_instance.py
--rw-r--r--   0        0        0     2344 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_objectives.py
--rw-r--r--   0        0        0     1608 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_result.py
--rw-r--r--   0        0        0     4729 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_route_schedule.py
--rw-r--r--   0        0        0     1136 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_runtimes.py
--rw-r--r--   0        0        0     1844 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_solution.py
--rw-r--r--   0        0        0     1226 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_time_windows.py
--rw-r--r--   0        0        0        0 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/__init__.py
--rw-r--r--   0        0        0    47981 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
--rw-r--r--   0        0        0   141297 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
--rw-r--r--   0        0        0    35194 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
--rw-r--r--   0        0        0    25609 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
--rw-r--r--   0        0        0    43058 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
--rw-r--r--   0        0        0     3108 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/plotting/tests/test_plotting.py
--rw-r--r--   0        0        0     6047 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/read.py
--rw-r--r--   0        0        0     1048 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/show_versions.py
--rw-r--r--   0        0        0      444 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/MaxIterations.py
--rw-r--r--   0        0        0      589 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/MaxRuntime.py
--rw-r--r--   0        0        0      819 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/NoImprovement.py
--rw-r--r--   0        0        0      573 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      575 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/TimedNoImprovement.py
--rw-r--r--   0        0        0      217 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/__init__.py
--rw-r--r--   0        0        0      839 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/test_MaxIterations.py
--rw-r--r--   0        0        0     1031 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/test_MaxRuntime.py
--rw-r--r--   0        0        0     1777 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/test_NoImprovement.py
--rw-r--r--   0        0        0     1292 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/test_TimedNoImprovement.py
--rw-r--r--   0        0        0        0 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/__init__.py
--rw-r--r--   0        0        0      189 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/DepotNotOne.txt
--rw-r--r--   0        0        0      607 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/E-n22-k4.txt
--rw-r--r--   0        0        0      671 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
--rw-r--r--   0        0        0      668 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
--rw-r--r--   0        0        0      389 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/FileWithUnknownSection.txt
--rw-r--r--   0        0        0      191 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/MoreThanOneDepot.txt
--rw-r--r--   0        0        0      371 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/NonZeroDepotDemand.txt
--rw-r--r--   0        0        0      371 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
--rw-r--r--   0        0        0      371 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
--rw-r--r--   0        0        0      675 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/OkSmall.txt
--rw-r--r--   0        0        0      697 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/OkSmallGreedyRepair.txt
--rw-r--r--   0        0        0      754 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/OkSmallPrizes.txt
--rw-r--r--   0        0        0      347 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/RC208.sol
--rw-r--r--   0        0        0     7524 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/RC208.txt
--rw-r--r--   0        0        0      369 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
--rw-r--r--   0        0        0      187 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
--rw-r--r--   0        0        0      154 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/UnknownEdgeWeightType.txt
--rw-r--r--   0        0        0     2005 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/p06-2-50.vrp
--rw-r--r--   0        0        0     1256 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/helpers.py
--rw-r--r--   0        0        0     4538 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_CostEvaluator.py
--rw-r--r--   0        0        0     7641 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_GeneticAlgorithm.py
--rw-r--r--   0        0        0    12058 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Individual.py
--rw-r--r--   0        0        0     1190 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Matrix.py
--rw-r--r--   0        0        0     9864 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_PenaltyManager.py
--rw-r--r--   0        0        0    12857 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Population.py
--rw-r--r--   0        0        0     3222 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_ProblemData.py
--rw-r--r--   0        0        0     2743 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Result.py
--rw-r--r--   0        0        0     1148 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Statistics.py
--rw-r--r--   0        0        0     5918 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_SubPopulation.py
--rw-r--r--   0        0        0     1913 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_TimeWindowSegment.py
--rw-r--r--   0        0        0     1101 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_XorShift128.py
--rw-r--r--   0        0        0     6306 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_read.py
--rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 pyvrp-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1175 2023-07-04 09:33:31.369422 pyvrp-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2963 2023-07-04 09:33:31.369422 pyvrp-0.4.1/README.md
+-rw-r--r--   0        0        0     3563 2023-07-04 09:33:31.369422 pyvrp-0.4.1/build_extensions.py
+-rw-r--r--   0        0        0     3747 2023-07-04 09:33:31.397423 pyvrp-0.4.1/meson.build
+-rw-r--r--   0        0        0      302 2023-07-04 09:33:31.397423 pyvrp-0.4.1/meson_options.txt
+-rw-r--r--   0        0        0     3505 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6822 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/GeneticAlgorithm.py
+-rw-r--r--   0        0        0     8577 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/Model.py
+-rw-r--r--   0        0        0     8807 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/PenaltyManager.py
+-rw-r--r--   0        0        0     6608 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/Population.py
+-rw-r--r--   0        0        0     2922 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/Result.py
+-rw-r--r--   0        0        0     6191 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/Statistics.py
+-rw-r--r--   0        0        0     1375 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_CostEvaluator.pyi
+-rw-r--r--   0        0        0      563 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_Matrix.pyi
+-rw-r--r--   0        0        0     5791 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_ProblemData.pyi
+-rw-r--r--   0        0        0     6397 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_Solution.pyi
+-rw-r--r--   0        0        0     4089 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_SubPopulation.pyi
+-rw-r--r--   0        0        0     1664 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_TimeWindowSegment.pyi
+-rw-r--r--   0        0        0      267 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_XorShift128.pyi
+-rw-r--r--   0        0        0      554 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/__init__.py
+-rw-r--r--   0        0        0     8947 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cli.py
+-rw-r--r--   0        0        0       45 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/constants.py
+-rw-r--r--   0        0        0      854 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/CostEvaluator.cpp
+-rw-r--r--   0        0        0     2039 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/CostEvaluator.h
+-rw-r--r--   0        0        0     1354 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/CostEvaluator_bindings.cpp
+-rw-r--r--   0        0        0     2751 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Matrix.h
+-rw-r--r--   0        0        0     1041 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Matrix_bindings.cpp
+-rw-r--r--   0        0        0     5569 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Measure.h
+-rw-r--r--   0        0        0     2466 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/ProblemData.cpp
+-rw-r--r--   0        0        0     4789 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/ProblemData.h
+-rw-r--r--   0        0        0     5227 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/ProblemData_bindings.cpp
+-rw-r--r--   0        0        0      745 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/README.md
+-rw-r--r--   0        0        0    11014 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Solution.cpp
+-rw-r--r--   0        0        0     6952 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Solution.h
+-rw-r--r--   0        0        0     5857 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Solution_bindings.cpp
+-rw-r--r--   0        0        0     4670 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/SubPopulation.cpp
+-rw-r--r--   0        0        0     3036 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/SubPopulation.h
+-rw-r--r--   0        0        0     2744 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/SubPopulation_bindings.cpp
+-rw-r--r--   0        0        0     3725 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/TimeWindowSegment.h
+-rw-r--r--   0        0        0     1603 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/TimeWindowSegment_bindings.cpp
+-rw-r--r--   0        0        0      581 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/XorShift128.cpp
+-rw-r--r--   0        0        0     2109 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/XorShift128.h
+-rw-r--r--   0        0        0      467 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/XorShift128_bindings.cpp
+-rw-r--r--   0        0        0     5340 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/crossover/crossover.cpp
+-rw-r--r--   0        0        0     2010 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/crossover/crossover.h
+-rw-r--r--   0        0        0     8610 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/crossover/selective_route_exchange.cpp
+-rw-r--r--   0        0        0      375 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/crossover/selective_route_exchange_bindings.cpp
+-rw-r--r--   0        0        0     1003 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/diversity/broken_pairs_distance.cpp
+-rw-r--r--   0        0        0      254 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/diversity/broken_pairs_distance_bindings.cpp
+-rw-r--r--   0        0        0      636 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/diversity/diversity.h
+-rw-r--r--   0        0        0     3048 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/CircleSector.h
+-rw-r--r--   0        0        0    11425 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/Exchange.h
+-rw-r--r--   0        0        0     2173 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/Exchange_bindings.cpp
+-rw-r--r--   0        0        0    14552 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch.cpp
+-rw-r--r--   0        0        0     3734 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch.h
+-rw-r--r--   0        0        0     2647 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/LocalSearchOperator.h
+-rw-r--r--   0        0        0     1329 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch_bindings.cpp
+-rw-r--r--   0        0        0     3733 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/MoveTwoClientsReversed.cpp
+-rw-r--r--   0        0        0      504 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/MoveTwoClientsReversed.h
+-rw-r--r--   0        0        0      482 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/MoveTwoClientsReversed_bindings.cpp
+-rw-r--r--   0        0        0      970 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/Node.cpp
+-rw-r--r--   0        0        0     1616 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/Node.h
+-rw-r--r--   0        0        0     1175 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar.cpp
+-rw-r--r--   0        0        0      755 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar.h
+-rw-r--r--   0        0        0      436 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar_bindings.cpp
+-rw-r--r--   0        0        0     3952 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/Route.cpp
+-rw-r--r--   0        0        0     5350 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/Route.h
+-rw-r--r--   0        0        0    10975 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/SwapStar.cpp
+-rw-r--r--   0        0        0     3399 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/SwapStar.h
+-rw-r--r--   0        0        0      420 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/SwapStar_bindings.cpp
+-rw-r--r--   0        0        0     4352 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt.cpp
+-rw-r--r--   0        0        0      922 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt.h
+-rw-r--r--   0        0        0      409 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt_bindings.cpp
+-rw-r--r--   0        0        0       63 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/crossover/__init__.py
+-rw-r--r--   0        0        0      364 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/crossover/_selective_route_exchange.pyi
+-rw-r--r--   0        0        0     1949 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/crossover/selective_route_exchange.py
+-rw-r--r--   0        0        0    12528 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/crossover/tests/test_selective_route_exchange.py
+-rw-r--r--   0        0        0       58 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/diversity/__init__.py
+-rw-r--r--   0        0        0     1444 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/diversity/_broken_pairs_distance.pyi
+-rw-r--r--   0        0        0     1171 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/diversity/tests/test_broken_pairs_distance.py
+-rw-r--r--   0        0        0      580 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/exceptions.py
+-rw-r--r--   0        0        0      436 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_coordinates.py
+-rw-r--r--   0        0        0     1358 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_demands.py
+-rw-r--r--   0        0        0     1199 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_diversity.py
+-rw-r--r--   0        0        0     1129 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_instance.py
+-rw-r--r--   0        0        0     2344 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_objectives.py
+-rw-r--r--   0        0        0     1608 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_result.py
+-rw-r--r--   0        0        0     4690 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_route_schedule.py
+-rw-r--r--   0        0        0     1136 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_runtimes.py
+-rw-r--r--   0        0        0     1782 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_solution.py
+-rw-r--r--   0        0        0     1226 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_time_windows.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/__init__.py
+-rw-r--r--   0        0        0    47981 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
+-rw-r--r--   0        0        0   141297 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
+-rw-r--r--   0        0        0    35194 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
+-rw-r--r--   0        0        0    25609 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
+-rw-r--r--   0        0        0    43058 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
+-rw-r--r--   0        0        0     3079 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/plotting/tests/test_plotting.py
+-rw-r--r--   0        0        0     6782 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/read.py
+-rw-r--r--   0        0        0     6559 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/LocalSearch.py
+-rw-r--r--   0        0        0      896 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_Exchange.pyi
+-rw-r--r--   0        0        0      891 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_LocalSearch.pyi
+-rw-r--r--   0        0        0      204 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_MoveTwoClientsReversed.pyi
+-rw-r--r--   0        0        0      196 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_RelocateStar.pyi
+-rw-r--r--   0        0        0      192 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_SwapStar.pyi
+-rw-r--r--   0        0        0      188 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_TwoOpt.pyi
+-rw-r--r--   0        0        0      708 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/__init__.py
+-rw-r--r--   0        0        0     5149 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/neighbourhood.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/__init__.py
+-rw-r--r--   0        0        0    10470 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_Exchange.py
+-rw-r--r--   0        0        0     8638 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_LocalSearch.py
+-rw-r--r--   0        0        0     2633 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_MoveTwoClientsReversed.py
+-rw-r--r--   0        0        0     3029 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_RelocateStar.py
+-rw-r--r--   0        0        0     2918 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_SwapStar.py
+-rw-r--r--   0        0        0     3970 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_TwoOpt.py
+-rw-r--r--   0        0        0     6091 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_neighbourhood.py
+-rw-r--r--   0        0        0     1048 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/show_versions.py
+-rw-r--r--   0        0        0      444 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/MaxIterations.py
+-rw-r--r--   0        0        0      589 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/MaxRuntime.py
+-rw-r--r--   0        0        0      819 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/NoImprovement.py
+-rw-r--r--   0        0        0      573 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      575 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/TimedNoImprovement.py
+-rw-r--r--   0        0        0      217 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/__init__.py
+-rw-r--r--   0        0        0      839 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/test_MaxIterations.py
+-rw-r--r--   0        0        0     1031 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/test_MaxRuntime.py
+-rw-r--r--   0        0        0     1777 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/test_NoImprovement.py
+-rw-r--r--   0        0        0     1292 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/test_TimedNoImprovement.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/__init__.py
+-rw-r--r--   0        0        0      189 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/DepotNotOne.txt
+-rw-r--r--   0        0        0      607 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/E-n22-k4.txt
+-rw-r--r--   0        0        0      671 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
+-rw-r--r--   0        0        0      668 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
+-rw-r--r--   0        0        0      389 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/FileWithUnknownSection.txt
+-rw-r--r--   0        0        0      191 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/MoreThanOneDepot.txt
+-rw-r--r--   0        0        0      371 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/NonZeroDepotDemand.txt
+-rw-r--r--   0        0        0      371 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
+-rw-r--r--   0        0        0      371 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/NonZeroDepotReleaseTime.txt
+-rw-r--r--   0        0        0      371 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
+-rw-r--r--   0        0        0      675 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/OkSmall.txt
+-rw-r--r--   0        0        0      697 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/OkSmallGreedyRepair.txt
+-rw-r--r--   0        0        0      754 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/OkSmallPrizes.txt
+-rw-r--r--   0        0        0      744 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/OkSmallReleaseTimes.txt
+-rw-r--r--   0        0        0      347 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/RC208.sol
+-rw-r--r--   0        0        0     7524 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/RC208.txt
+-rw-r--r--   0        0        0      681 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/ReallyLargeDistance.txt
+-rw-r--r--   0        0        0      369 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
+-rw-r--r--   0        0        0      187 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
+-rw-r--r--   0        0        0      154 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/UnknownEdgeWeightType.txt
+-rw-r--r--   0        0        0     2005 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/p06-2-50.vrp
+-rw-r--r--   0        0        0     1985 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/helpers.py
+-rw-r--r--   0        0        0     4674 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_CostEvaluator.py
+-rw-r--r--   0        0        0     7586 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_GeneticAlgorithm.py
+-rw-r--r--   0        0        0     1348 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Matrix.py
+-rw-r--r--   0        0        0     8491 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Model.py
+-rw-r--r--   0        0        0     9864 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_PenaltyManager.py
+-rw-r--r--   0        0        0    12503 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Population.py
+-rw-r--r--   0        0        0     3570 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_ProblemData.py
+-rw-r--r--   0        0        0     2645 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Result.py
+-rw-r--r--   0        0        0    19074 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Solution.py
+-rw-r--r--   0        0        0     1134 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Statistics.py
+-rw-r--r--   0        0        0     5882 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_SubPopulation.py
+-rw-r--r--   0        0        0     2240 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_TimeWindowSegment.py
+-rw-r--r--   0        0        0     1101 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_XorShift128.py
+-rw-r--r--   0        0        0     7153 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_read.py
+-rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pyvrp-0.4.1/PKG-INFO
```

### Comparing `pyvrp-0.3.0/LICENSE` & `pyvrp-0.4.1/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 MIT License
 
+Copyright (c) 2020, Thibaut Vidal (HGS-CVRP)
+Copyright (c) 2022, ORTEC and TU/e (HGS-DIMACS)
 Copyright (c) since 2022, PyVRP contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `pyvrp-0.3.0/build_extensions.py` & `pyvrp-0.4.1/build_extensions.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,20 @@
     parser.add_argument(
         "--problem",
         default="vrptw",
         choices=["cvrp", "vrptw"],
         help="Which type of solver to compile. Defaults to 'vrptw'.",
     )
     parser.add_argument(
+        "--precision",
+        default="integer",
+        choices=["integer", "double"],
+        help="Double is more precise, integer faster. Defaults to 'integer'.",
+    )
+    parser.add_argument(
         "--clean",
         action="store_true",
         help="Clean build and installation directories before building.",
     )
     parser.add_argument(
         "--regenerate_type_stubs",
         action="store_true",
@@ -55,43 +61,45 @@
         extension.unlink()
 
     for extension in install_dir.rglob("*.pyd"):
         extension.unlink()
 
 
 def regenerate_stubs(install_dir: pathlib.Path):
-    def _regen(extension):
+    def regen(extension):
         ext_dir = extension.parent
         ext_name, _ = extension.name.split(".", maxsplit=1)
 
         check_call(
             ["stubgen", "--parse-only", "-o", ".", "-m", ext_name],
             cwd=ext_dir,
         )
 
     for extension in install_dir.rglob("*.so"):
-        _regen(extension)
+        regen(extension)
 
     for extension in install_dir.rglob("*.pyd"):
-        _regen(extension)
+        regen(extension)
 
 
 def build(
     build_dir: pathlib.Path,
     build_type: str,
     problem: str,
+    precision: str,
     additional: List[str],
 ):
     cwd = pathlib.Path.cwd()
     args = [
         # fmt: off
         "--buildtype", build_type,
         f"-Dpython.platlibdir={cwd.absolute()}",
         f"-Dproblem={problem}",
         f"-Dstrip={'true' if build_type == 'release' else 'false'}",
+        f"-Dprecision={precision}",
         *additional,
         # fmt: on
     ]
 
     cmd = "configure" if build_dir.exists() else "setup"
     check_call(["meson", cmd, build_dir, *args])
     check_call(["meson", "compile", "-C", build_dir])
@@ -105,15 +113,21 @@
     install_dir = cwd / "pyvrp"
 
     if args.clean or os.environ.get("CIBUILDWHEEL", "0") == "1":
         # Always start from an entirely clean build when building wheels in
         # the CI. Else only do so when expressly asked.
         clean(build_dir, install_dir)
 
-    build(build_dir, args.build_type, args.problem, args.additional)
+    build(
+        build_dir,
+        args.build_type,
+        args.problem,
+        args.precision,
+        args.additional,
+    )
 
     if args.regenerate_type_stubs:
         regenerate_stubs(install_dir)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyvrp-0.3.0/meson.build` & `pyvrp-0.4.1/meson.build`

 * *Files 27% similar despite different names*

```diff
@@ -20,30 +20,22 @@
         add_project_arguments('-fprofile-abs-path', language: 'cpp')
     endif
 
     add_project_arguments('--coverage', language: 'cpp')
     add_project_link_arguments('--coverage', language: 'cpp')
 endif
 
-if compiler.has_argument('-Wno-unused-parameter')
-    # Ignore unused parameters, because not all operator implementations use 
-    # every argument they are given (and that's OK).
-    add_project_arguments('-Wno-unused-parameter', language: 'cpp')
-endif
-
 if get_option('problem') == 'cvrp'
     # CVRP does not have time windows, so we set a flag that compiles time 
     # window stuff out of the extension modules.
-    add_project_arguments('-DVRP_NO_TIME_WINDOWS', language: 'cpp')
+    add_project_arguments('-DPYVRP_NO_TIME_WINDOWS', language: 'cpp')
+endif
 
-    if compiler.has_argument('-Wno-unused-private-field')
-        # Ignore unused fields, since a number of time window related fields
-        # are unused by the CVRP.
-        add_project_arguments('-Wno-unused-private-field', language: 'cpp')
-    endif
+if get_option('precision') == 'double'  # default is integer
+    add_project_arguments('-DPYVRP_DOUBLE_PRECISION', language: 'cpp')
 endif
 
 # We first compile a common library that contains all regular, C++ code. This
 # is then linked against by the extension modules. We also define source and
 # installation directories here, as a shorthand.
 INST_DIR = 'pyvrp'
 SRC_DIR = 'pyvrp' / 'cpp'
@@ -51,69 +43,54 @@
 
 libcommon = static_library(
     'common',
     [
         SRC_DIR / 'CostEvaluator.cpp',
         SRC_DIR / 'ProblemData.cpp',
         SRC_DIR / 'XorShift128.cpp',
-        SRC_DIR / 'Individual.cpp',
+        SRC_DIR / 'Solution.cpp',
         SRC_DIR / 'SubPopulation.cpp',
         SRC_DIR / 'crossover' / 'selective_route_exchange.cpp',
         SRC_DIR / 'crossover' / 'crossover.cpp',
         SRC_DIR / 'diversity' / 'broken_pairs_distance.cpp',
-        SRC_DIR / 'educate' / 'LocalSearch.cpp',
-        SRC_DIR / 'educate' / 'Route.cpp',
-        SRC_DIR / 'educate' / 'Node.cpp',
-        SRC_DIR / 'educate' / 'MoveTwoClientsReversed.cpp',
-        SRC_DIR / 'educate' / 'TwoOpt.cpp',
-        SRC_DIR / 'educate' / 'RelocateStar.cpp',
-        SRC_DIR / 'educate' / 'SwapStar.cpp',
+        SRC_DIR / 'search' / 'LocalSearch.cpp',
+        SRC_DIR / 'search' / 'Route.cpp',
+        SRC_DIR / 'search' / 'Node.cpp',
+        SRC_DIR / 'search' / 'MoveTwoClientsReversed.cpp',
+        SRC_DIR / 'search' / 'TwoOpt.cpp',
+        SRC_DIR / 'search' / 'RelocateStar.cpp',
+        SRC_DIR / 'search' / 'SwapStar.cpp',
     ],
     include_directories: INCLUDES,
 )
 
-# Next we get the extension dependencies. These are pretty simple: we only
-# depend on Python (duh!) and pybind11.
+# Next we get the extension dependencies.
 py = import('python').find_installation()
-pybind11 = dependency('pybind11', required: false)
-
-if not pybind11.found()
-    # Fallback: this looks for the pybind11 header files using pybind11-config.
-    # Getting pybind11 using Meson's dependency mechanism is nicer, but that
-    # sometimes fails even when pybind11 is actually available on the system.
-    message('Could not find pybind11 as a dependency: trying headers.')
-
-    pybind11 = find_program('pybind11-config')
-    pybind11 = run_command(pybind11, ['--includes'], check: true)
-    pybind11 = pybind11.stdout().split('-I')[-1].strip()
-    pybind11 = declare_dependency(include_directories: [pybind11])
-endif
-
-assert(pybind11.found(), 'Could not find pybind11!')
+pybind11 = dependency('pybind11')
 dependencies = [py.dependency(), pybind11]
 
 # Extension as [extension name, subdirectory]. Here 'extension name' names the
 # eventual module name and the bindings source file, and 'subdirectory' gives 
 # the source and installation directories (relative to SRC_DIR and INST_DIR).
 extensions = [
     ['Matrix', ''],
     ['CostEvaluator', ''],
     ['ProblemData', ''],
     ['SubPopulation', ''],
     ['TimeWindowSegment', ''],
     ['XorShift128', ''],
-    ['Individual', ''],
+    ['Solution', ''],
     ['selective_route_exchange', 'crossover'],
     ['broken_pairs_distance', 'diversity'],
-    ['LocalSearch', 'educate'],
-    ['Exchange', 'educate'],
-    ['MoveTwoClientsReversed', 'educate'],
-    ['TwoOpt', 'educate'],
-    ['RelocateStar', 'educate'],
-    ['SwapStar', 'educate'],
+    ['LocalSearch', 'search'],
+    ['Exchange', 'search'],
+    ['MoveTwoClientsReversed', 'search'],
+    ['TwoOpt', 'search'],
+    ['RelocateStar', 'search'],
+    ['SwapStar', 'search'],
 ]
 
 foreach extension : extensions  # extension[0] = name, extension[1] = subdir
     message('Going to build ' + extension[0])
 
     source_dir = '/'.join([SRC_DIR, extension[1]])
     install_dir = '/'.join([INST_DIR, extension[1]])
```

### Comparing `pyvrp-0.3.0/pyproject.toml` & `pyvrp-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvrp"
-version = "0.3.0"
+version = "0.4.1"
 description = "A state-of-the-art vehicle routing problem solver."
 authors = [
     "Niels Wouda <nielswouda@gmail.com>",
     "Leon Lan <leon.lanyidong@gmail.com>",
     "Wouter Kool <wouter.kool@ortec.com>",
 ]
 license = "MIT"
@@ -74,19 +74,18 @@
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 pytest = ">=6.0.0"
 pytest-cov = ">=2.6.1"
 codecov = "*"
 
-# These are used in the build script: for compiling the library (meson, ninja,
-# and pybind11) and for generating type stubs (mypy).
+# These are used in the build script: for compiling the library (meson, ninja)
+# and for generating type stubs (mypy).
 meson = "^1.0.0"
 ninja = "^1.11.1"
-pybind11 = {extras = ["global"], version = "^2.10.3"}
 mypy = "^0.991"
 
 
 [tool.poetry.scripts]
 pyvrp = "pyvrp.cli:main"
 
 
@@ -119,29 +118,30 @@
     "docs/*",
 ]
 
 
 [tool.coverage.report]
 exclude_lines = [
     # This excludes all abstract methods from code coverage checks as they are
-    # never instantiated directly anyway
+    # never instantiated directly anyway.
     "pragma: no cover",
     "@abstract",
 ]
 
 
 [tool.cibuildwheel]
 # We do not support old Python versions (<3.8) and somewhat uncommon platforms.
-skip = "cp36-* cp37-* pp* *_ppc64le *_i686 *_s390x *-win32"
+# For musllinux-based builds we assume users can compile the thing themselves.
+skip = "cp36-* cp37-* pp* *_ppc64le *_i686 *_s390x *-win32 *-musllinux*"
 build-verbosity = "3"
 build-frontend = "build"
 
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "build_extensions.py"
 
 
 [build-system]
-# pybind11, meson, and ninja are needed to build the C++ extensions.
-requires = ["poetry-core", "pybind11", "meson", "ninja"]
+# meson and ninja are needed to build the C++ extensions.
+requires = ["poetry-core", "meson", "ninja"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyvrp-0.3.0/pyvrp/GeneticAlgorithm.py` & `pyvrp-0.4.1/pyvrp/GeneticAlgorithm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import time
 from dataclasses import dataclass
 from typing import Callable, Collection, Tuple
 
-from pyvrp.educate.LocalSearch import LocalSearch
+from pyvrp.search.LocalSearch import LocalSearch
 from pyvrp.stop import StoppingCriterion
 
 from .PenaltyManager import PenaltyManager
 from .Population import Population
 from .Result import Result
 from .Statistics import Statistics
 from ._CostEvaluator import CostEvaluator
-from ._Individual import Individual
 from ._ProblemData import ProblemData
+from ._Solution import Solution
 from ._XorShift128 import XorShift128
 
-_Parents = Tuple[Individual, Individual]
+_Parents = Tuple[Solution, Solution]
 CrossoverOperator = Callable[
-    [_Parents, ProblemData, CostEvaluator, XorShift128], Individual
+    [_Parents, ProblemData, CostEvaluator, XorShift128], Solution
 ]
 
 
 @dataclass
 class GeneticAlgorithmParams:
     repair_probability: float = 0.80
     collect_statistics: bool = False
@@ -72,15 +72,15 @@
         self,
         data: ProblemData,
         penalty_manager: PenaltyManager,
         rng: XorShift128,
         population: Population,
         local_search: LocalSearch,
         crossover_op: CrossoverOperator,
-        initial_solutions: Collection[Individual],
+        initial_solutions: Collection[Solution],
         params: GeneticAlgorithmParams = GeneticAlgorithmParams(),
     ):
         if len(initial_solutions) == 0:
             raise ValueError("Expected at least one initial solution.")
 
         self._data = data
         self._pm = penalty_manager
@@ -115,105 +115,98 @@
             A Result object, containing statistics and the best found solution.
         """
         start = time.perf_counter()
         stats = Statistics()
         iters = 0
         iters_no_improvement = 1
 
-        for individual in self._initial_solutions:
-            self._pop.add(individual, self._cost_evaluator)
+        for sol in self._initial_solutions:
+            self._pop.add(sol, self._cost_evaluator)
 
         while not stop(self._cost_evaluator.cost(self._best)):
             iters += 1
 
             if iters_no_improvement == self._params.nb_iter_no_improvement:
                 iters_no_improvement = 1
                 self._pop.clear()
 
-                for individual in self._initial_solutions:
-                    self._pop.add(individual, self._cost_evaluator)
+                for sol in self._initial_solutions:
+                    self._pop.add(sol, self._cost_evaluator)
 
             curr_best = self._cost_evaluator.cost(self._best)
 
             parents = self._pop.select(self._rng, self._cost_evaluator)
             offspring = self._op(
                 parents, self._data, self._cost_evaluator, self._rng
             )
-            self._educate(offspring)
+            self._search(offspring)
 
             new_best = self._cost_evaluator.cost(self._best)
 
             if new_best < curr_best:
                 iters_no_improvement = 1
             else:
                 iters_no_improvement += 1
 
             if self._params.collect_statistics:
                 stats.collect_from(self._pop, self._cost_evaluator)
 
         end = time.perf_counter() - start
         return Result(self._best, stats, iters, end)
 
-    def _educate(self, individual: Individual):
-        def is_new_best(indiv):
-            cost = self._cost_evaluator.cost(indiv)
+    def _search(self, sol: Solution):
+        def is_new_best(sol):
+            cost = self._cost_evaluator.cost(sol)
             best_cost = self._cost_evaluator.cost(self._best)
             return cost < best_cost
 
-        def add_and_register(indiv):
-            self._pop.add(indiv, self._cost_evaluator)
-            self._pm.register_load_feasible(not indiv.has_excess_load())
-            self._pm.register_time_feasible(not indiv.has_time_warp())
+        def add_and_register(sol):
+            self._pop.add(sol, self._cost_evaluator)
+            self._pm.register_load_feasible(not sol.has_excess_load())
+            self._pm.register_time_feasible(not sol.has_time_warp())
 
         intensify_prob = self._params.intensify_probability
         should_intensify = self._rng.rand() < intensify_prob
 
-        individual = self._ls.run(
-            individual, self._cost_evaluator, should_intensify
-        )
+        sol = self._ls.run(sol, self._cost_evaluator, should_intensify)
 
-        if is_new_best(individual):
-            self._best = individual
+        if is_new_best(sol):
+            self._best = sol
 
             # Only intensify feasible, new best solutions. See also the repair
             # step below. TODO Refactor to on_best callback (see issue #111)
             if self._params.intensify_on_best:
-                individual = self._ls.intensify(
-                    individual,
-                    self._cost_evaluator,
-                    overlap_tolerance_degrees=360,
+                sol = self._ls.intensify(
+                    sol, self._cost_evaluator, overlap_tolerance_degrees=360
                 )
 
-                if is_new_best(individual):
-                    self._best = individual
+                if is_new_best(sol):
+                    self._best = sol
 
-        add_and_register(individual)
+        add_and_register(sol)
 
         # Possibly repair if current solution is infeasible. In that case, we
         # penalise infeasibility more using a penalty booster.
         if (
-            not individual.is_feasible()
+            not sol.is_feasible()
             and self._rng.rand() < self._params.repair_probability
         ):
-
             should_intensify = self._rng.rand() < intensify_prob
-            individual = self._ls.run(
-                individual,
-                self._pm.get_booster_cost_evaluator(),
-                should_intensify,
+            sol = self._ls.run(
+                sol, self._pm.get_booster_cost_evaluator(), should_intensify
             )
 
-            if is_new_best(individual):
-                self._best = individual
+            if is_new_best(sol):
+                self._best = sol
 
                 if self._params.intensify_on_best:
-                    individual = self._ls.intensify(
-                        individual,
+                    sol = self._ls.intensify(
+                        sol,
                         self._pm.get_booster_cost_evaluator(),
                         overlap_tolerance_degrees=360,
                     )
 
-                    if is_new_best(individual):
-                        self._best = individual
+                    if is_new_best(sol):
+                        self._best = sol
 
-            if individual.is_feasible():
-                add_and_register(individual)
+            if sol.is_feasible():
+                add_and_register(sol)
```

### Comparing `pyvrp-0.3.0/pyvrp/PenaltyManager.py` & `pyvrp-0.4.1/pyvrp/PenaltyManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         """
         Registers another capacity feasibility result. The current load penalty
         is updated once sufficiently many results have been gathered.
 
         Parameters
         ----------
         is_load_feasible
-            Boolean indicating whether the last individual was feasible w.r.t
+            Boolean indicating whether the last solution was feasible w.r.t.
             the capacity constraint.
         """
         self._load_feas.append(is_load_feasible)
         if (
             len(self._load_feas)
             == self._params.num_registrations_between_penalty_updates
         ):
@@ -184,16 +184,16 @@
         """
         Registers another time feasibility result. The current time warp
         penalty is updated once sufficiently many results have been gathered.
 
         Parameters
         ----------
         is_time_feasible
-            Boolean indicating whether the last individual was feasible w.r.t
-             the time constraint.
+            Boolean indicating whether the last solution was feasible w.r.t.
+            the time constraint.
         """
         self._time_feas.append(is_time_feasible)
         if (
             len(self._time_feas)
             == self._params.num_registrations_between_penalty_updates
         ):
             avg = fmean(self._time_feas)
```

### Comparing `pyvrp-0.3.0/pyvrp/Population.py` & `pyvrp-0.4.1/pyvrp/Population.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Callable, Generator, Tuple
 from warnings import warn
 
 from ._CostEvaluator import CostEvaluator
-from ._Individual import Individual
+from ._Solution import Solution
 from ._SubPopulation import PopulationParams, SubPopulation
 from ._XorShift128 import XorShift128
 from .exceptions import EmptySolutionWarning
 
 
 class Population:
     """
@@ -21,37 +21,37 @@
         a look at :mod:`pyvrp.diversity` for available operators.
     params, optional
         Population parameters. If not provided, a default will be used.
     """
 
     def __init__(
         self,
-        diversity_op: Callable[[Individual, Individual], float],
+        diversity_op: Callable[[Solution, Solution], float],
         params: PopulationParams = PopulationParams(),
     ):
         self._op = diversity_op
         self._params = params
 
         self._feas = SubPopulation(diversity_op, params)
         self._infeas = SubPopulation(diversity_op, params)
 
-    def __iter__(self) -> Generator[Individual, None, None]:
+    def __iter__(self) -> Generator[Solution, None, None]:
         """
-        Iterates over the individuals contained in this population.
+        Iterates over the solutions contained in this population.
 
         Yields
         ------
         iterable
-            An iterable object of individuals.
+            An iterable object of solutions.
         """
         for item in self._feas:
-            yield item.individual
+            yield item.solution
 
         for item in self._infeas:
-            yield item.individual
+            yield item.solution
 
     def __len__(self) -> int:
         """
         Returns the current population size.
 
         Returns
         -------
@@ -70,98 +70,98 @@
             CostEvaluator to use for computing the fitness.
         """
         self._feas.update_fitness(cost_evaluator)
         self._infeas.update_fitness(cost_evaluator)
 
     def num_feasible(self) -> int:
         """
-        Returns the number of feasible individuals in the population.
+        Returns the number of feasible solutions in the population.
 
         Returns
         -------
         int
-            Number of feasible individuals.
+            Number of feasible solutions.
         """
         return len(self._feas)
 
     def num_infeasible(self) -> int:
         """
-        Returns the number of infeasible individuals in the population.
+        Returns the number of infeasible solutions in the population.
 
         Returns
         -------
         int
-            Number of infeasible individuals.
+            Number of infeasible solutions.
         """
         return len(self._infeas)
 
-    def add(self, individual: Individual, cost_evaluator: CostEvaluator):
+    def add(self, solution: Solution, cost_evaluator: CostEvaluator):
         """
-        Adds the given individual to the population. Survivor selection is
+        Adds the given solution to the population. Survivor selection is
         automatically triggered when the population reaches its maximum size.
 
         Parameters
         ----------
-        individual
-            Individual to add to the population.
+        solution
+            Solution to add to the population.
         cost_evaluator
             CostEvaluator to use to compute the cost.
         """
-        if individual.num_clients() == 0:
+        if solution.num_clients() == 0:
             msg = """
             An empty solution is being added to the population. This typically
             indicates that there is a significant difference between the values
             of the prizes and the other objective terms, which hints at a data
             problem. Note that not every part of PyVRP can work gracefully with
             empty solutions.
             """
             warn(msg, EmptySolutionWarning)
 
-        # Note: the CostEvaluator is required here since adding an individual
+        # Note: the CostEvaluator is required here since adding a solution
         # may trigger a purge which needs to compute the biased fitness which
         # requires computing the cost.
-        if individual.is_feasible():
+        if solution.is_feasible():
             # Note: the feasible subpopulation actually doet not depend
             # on the penalty values but we use the same implementation.
-            self._feas.add(individual, cost_evaluator)
+            self._feas.add(solution, cost_evaluator)
         else:
-            self._infeas.add(individual, cost_evaluator)
+            self._infeas.add(solution, cost_evaluator)
 
     def clear(self):
         """
-        Clears the population by removing all individuals currently in the
+        Clears the population by removing all solutions currently in the
         population.
         """
         self._feas = SubPopulation(self._op, self._params)
         self._infeas = SubPopulation(self._op, self._params)
 
     def select(
         self,
         rng: XorShift128,
         cost_evaluator: CostEvaluator,
         k: int = 2,
-    ) -> Tuple[Individual, Individual]:
+    ) -> Tuple[Solution, Solution]:
         """
         Selects two (if possible non-identical) parents by tournament, subject
         to a diversity restriction.
 
         Parameters
         ----------
         rng
             Random number generator.
         cost_evaluator
             Cost evaluator to use when computing the fitness.
         k
-            The number of individuals to draw for the tournament. Defaults to
+            The number of solutions to draw for the tournament. Defaults to
             two, which results in a binary tournament.
 
         Returns
         -------
         tuple
-            A pair of individuals (parents).
+            A solution pair (parents).
         """
         self._update_fitness(cost_evaluator)
 
         first = self._get_tournament(rng, k)
         second = self._get_tournament(rng, k)
 
         diversity = self._op(first, second)
@@ -174,46 +174,46 @@
             second = self._get_tournament(rng, k)
             diversity = self._op(first, second)
 
         return first, second
 
     def get_tournament(
         self, rng: XorShift128, cost_evaluator: CostEvaluator, k: int = 2
-    ) -> Individual:
+    ) -> Solution:
         """
-        Selects an individual from this population by k-ary tournament, based
-        on the (internal) fitness values of the selected individuals.
+        Selects a solution from this population by k-ary tournament, based
+        on the (internal) fitness values of the selected solutions.
 
         Parameters
         ----------
         rng
             Random number generator.
         cost_evaluator
             Cost evaluator to use when computing the fitness.
         k
-            The number of individuals to draw for the tournament. Defaults to
+            The number of solutions to draw for the tournament. Defaults to
             two, which results in a binary tournament.
 
         Returns
         -------
-        Individual
-            The selected individual.
+        Solution
+            The selected solution.
         """
         self._update_fitness(cost_evaluator)
         return self._get_tournament(rng, k)
 
-    def _get_tournament(self, rng: XorShift128, k: int) -> Individual:
+    def _get_tournament(self, rng: XorShift128, k: int) -> Solution:
         if k <= 0:
             raise ValueError(f"Expected k > 0; got k = {k}.")
 
         def select():
             num_feas = len(self._feas)
             idx = rng.randint(len(self))
 
             if idx < num_feas:
                 return self._feas[idx]
 
             return self._infeas[idx - num_feas]
 
         items = [select() for _ in range(k)]
         fittest = min(items, key=lambda item: item.fitness)
-        return fittest.individual
+        return fittest.solution
```

### Comparing `pyvrp-0.3.0/pyvrp/Result.py` & `pyvrp-0.4.1/pyvrp/Result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 from dataclasses import dataclass
 
 from .Statistics import Statistics
 from ._CostEvaluator import CostEvaluator
-from ._Individual import Individual
+from ._Solution import Solution
 
 
 @dataclass
 class Result:
     """
     Stores the outcomes of a single run. An instance of this class is returned
     once the GeneticAlgorithm completes.
@@ -26,15 +26,15 @@
 
     Raises
     ------
     ValueError
         When the number of iterations or runtime are negative.
     """
 
-    best: Individual
+    best: Solution
     stats: Statistics
     num_iterations: int
     runtime: float
 
     def __post_init__(self):
         if self.num_iterations < 0:
             raise ValueError("Negative number of iterations not understood.")
```

### Comparing `pyvrp-0.3.0/pyvrp/Statistics.py` & `pyvrp-0.4.1/pyvrp/Statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Collects statistics from the given population object.
 
         Parameters
         ----------
         population
             Population instance to collect statistics from.
         cost_evaluator
-            CostEvaluator used to compute costs for individuals.
+            CostEvaluator used to compute costs for solutions.
         """
         start = self._clock
         self._clock = perf_counter()
 
         self.runtimes.append(self._clock - start)
         self.num_iterations += 1
 
@@ -82,17 +82,17 @@
                 best_cost=nan,
                 avg_cost=nan,
                 avg_num_routes=nan,
             )
 
         size = len(subpop)
         costs = [
-            cost_evaluator.penalised_cost(item.individual) for item in subpop
+            cost_evaluator.penalised_cost(item.solution) for item in subpop
         ]
-        num_routes = [item.individual.num_routes() for item in subpop]
+        num_routes = [item.solution.num_routes() for item in subpop]
         diversities = [item.avg_distance_closest() for item in subpop]
 
         return _Datum(
             size=size,
             avg_diversity=fmean(diversities),
             best_cost=min(costs),
             avg_cost=fmean(costs),
```

### Comparing `pyvrp-0.3.0/pyvrp/_CostEvaluator.pyi` & `pyvrp-0.4.1/pyvrp/_CostEvaluator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import overload
 
-from pyvrp._Individual import Individual
+from pyvrp._Solution import Solution
 
 class CostEvaluator:
     """
     Creates a CostEvaluator instance.
 
     This class contains time warp and load penalties, and can compute penalties
     for a given time warp and load.
@@ -18,21 +18,21 @@
     """
 
     def __init__(
         self, capacity_penalty: int = 0, tw_penalty: int = 0
     ) -> None: ...
     def load_penalty(self, load: int, vehicle_capacity: int) -> int: ...
     def tw_penalty(self, time_warp: int) -> int: ...
-    def penalised_cost(self, individual: Individual) -> int: ...
-    def cost(self, individual: Individual) -> int:
+    def penalised_cost(self, solution: Solution) -> int: ...
+    def cost(self, solution: Solution) -> int:
         """
-        Evaluates and returns the cost/objective of the given individual.
+        Evaluates and returns the cost/objective of the given solution.
         Hand-waving some details, let :math:`x_{ij} \\in \\{ 0, 1 \\}` indicate
         if edge :math:`(i, j)` is used in the solution encoded by the given
-        individual, and :math:`y_i \\in \\{ 0, 1 \\}` indicate if client
+        solution, and :math:`y_i \\in \\{ 0, 1 \\}` indicate if client
         :math:`i` is visited. The objective is then given by
 
         .. math::
 
            \\sum_{(i, j)} d_{ij} x_{ij} + \\sum_{i} p_i (1 - y_i),
 
         where the first part lists the distance costs, and the second part the
```

### Comparing `pyvrp-0.3.0/pyvrp/_Individual.pyi` & `pyvrp-0.4.1/pyvrp/_Solution.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Any, Dict, Iterator, List, Tuple
+from typing import Any, Dict, Iterator, List, Tuple, Union
 
 from ._ProblemData import ProblemData
 from ._XorShift128 import XorShift128
 
 class Route:
     """
     A simple class that stores the route plan and some statistics.
     """
 
-    def __init__(self, data: ProblemData, visits: List[int]) -> None: ...
+    def __init__(
+        self, data: ProblemData, visits: List[int], vehicle_type: int
+    ) -> None: ...
     def __getitem__(self, idx: int) -> int: ...
     def __iter__(self) -> Iterator[int]: ...
     def __len__(self) -> int: ...
     def is_feasible(self) -> bool: ...
     def has_excess_load(self) -> bool: ...
     def has_time_warp(self) -> bool: ...
     def demand(self) -> int:
@@ -43,110 +45,118 @@
         """
         Any time warp incurred along the route.
         """
     def wait_duration(self) -> int:
         """
         Total waiting duration on this route.
         """
+    def release_time(self) -> int:
+        """
+        Release time of visits on this route.
+        """
     def prizes(self) -> int:
         """
         Total prize value collected on this route.
         """
+    def centroid(self) -> Tuple[float, float]:
+        """
+        Center point of the client locations on this route.
+        """
+    def vehicle_type(self) -> int:
+        """
+        Index of the type of vehicle used on this route.
+        """
 
-class Individual:
+class Solution:
     """
-    The Individual class encodes VRP solutions.
+    Encodes VRP solutions.
 
     Parameters
     ----------
     data
         Data instance.
     routes
-        Route list to use.
+        Route list to use. Should be a list of Route objects, or list of list
+        of ints representing clients.
 
     Raises
     ------
     RuntimeError
         When the number of routes in the ``routes`` argument exceeds
-        :py:attr:`~pyvrp._ProblemData.ProblemData.num_vehicles`.
+        :py:attr:`~pyvrp._ProblemData.ProblemData.num_vehicles`, or when an
+        empty route has been passed as part of ``routes``.
     """
 
     def __init__(
         self,
         data: ProblemData,
-        routes: List[List[int]],
+        routes: List[Union[Route, List[int]]],
     ) -> None: ...
     @classmethod
-    def make_random(
-        cls,
-        data: ProblemData,
-        rng: XorShift128,
-    ) -> Individual:
+    def make_random(cls, data: ProblemData, rng: XorShift128) -> Solution:
         """
-        Creates a randomly generated Individual.
+        Creates a randomly generated solution.
 
         Parameters
         ----------
         data
             Data instance.
         rng
             Random number generator to use.
 
         Returns
         -------
-        Individual
-            The randomly generated Individual.
+        Solution
+            The randomly generated solution.
         """
     def get_neighbours(self) -> List[Tuple[int, int]]:
         """
         Returns a list of neighbours for each client, by index. Also includes
         the depot at index 0, which only neighbours itself.
 
         Returns
         -------
         list
             A list of ``(pred, succ)`` tuples that encode for each client their
-            predecessor and successors in this individual's routes.
+            predecessor and successors in this solutions's routes.
         """
     def get_routes(self) -> List[Route]:
         """
-        The solution this individual encodes, as a list of routes.
+        The solution's routing decisions.
 
         .. note::
 
-           This list is of length
-           :py:attr:`~pyvrp._ProblemData.ProblemData.num_vehicles`, but there
-           could be a number of empty routes. These empty routes are all in the
-           higher indices (guarantee). Use :meth:`~num_routes` to determine
-           which of the lower indices contain non-empty routes.
+           The length of this list is equal to the number of non-empty routes,
+           which is at most equal to
+           :py:attr:`~pyvrp._ProblemData.ProblemData.num_vehicles`.
 
         Returns
         -------
         list
-            A list of routes. Each :class:`~pyvrp._Individual.Route` starts and
+            A list of routes. Each :class:`~pyvrp._Solution.Route` starts and
             ends at the depot (0), but that is implicit: the depot is not part
             of the returned routes.
         """
     def has_excess_load(self) -> bool:
         """
-        Returns whether this individual violates capacity constraints.
+        Returns whether this solution violates capacity constraints.
 
         Returns
         -------
         bool
-            True if the individual is not capacity feasible, False otherwise.
+            True if the solution is not capacity feasible, False otherwise.
         """
     def has_time_warp(self) -> bool:
         """
-        Returns whether this individual violates time window constraints.
+        Returns whether this solution violates time window constraints.
 
         Returns
         -------
         bool
-            True if the individual is not time window feasible, False
+            True if the solution is not time window feasible, False
             otherwise.
         """
     def distance(self) -> int:
         """
         Returns the total distance over all routes.
 
         Returns
@@ -188,40 +198,40 @@
         Returns
         -------
         int
             Value of uncollected prizes.
         """
     def is_feasible(self) -> bool:
         """
-        Whether this individual is feasible. This is a shorthand for checking
-        :meth:`~has_excess_load` and :meth:`~has_time_warp` both return
+        Whether this solution is feasible. This is a shorthand for checking
+        that :meth:`~has_excess_load` and :meth:`~has_time_warp` both return
         false.
 
         Returns
         -------
         bool
-            Whether the solution of this individual is feasible with respect to
+            Whether the solution of this solution is feasible with respect to
             capacity and time window constraints.
         """
     def num_routes(self) -> int:
         """
-        Number of non-empty routes in this solution.
+        Number of routes in this solution.
 
         Returns
         -------
         int
-            Number of non-empty routes.
+            Number of routes.
         """
     def num_clients(self) -> int:
         """
         Number of clients in this solution.
 
         Returns
         -------
         int
             Number of clients in this solution.
         """
-    def __copy__(self) -> Individual: ...
-    def __deepcopy__(self, memo: Dict) -> Individual: ...
+    def __copy__(self) -> Solution: ...
+    def __deepcopy__(self, memo: Dict) -> Solution: ...
     def __hash__(self) -> int: ...
     def __eq__(self, other: Any) -> bool: ...
     def __str__(self) -> str: ...
```

### Comparing `pyvrp-0.3.0/pyvrp/_ProblemData.pyi` & `pyvrp-0.4.1/pyvrp/_ProblemData.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from typing import List
-
-from pyvrp._Matrix import Matrix
+from typing import List, Tuple
 
 class Client:
     """
     Simple data object storing all client data as (read-only) properties.
 
     Parameters
     ----------
@@ -21,66 +19,84 @@
         visit the client for. Service should start (but not necessarily end)
         within the [:py:attr:`~tw_early`, :py:attr:`~tw_late`] interval.
         Default 0.
     tw_early
         Earliest time at which we can visit this client. Default 0.
     tw_late
         Latest time at which we can visit this client. Default 0.
+    release_time
+        Earliest time at which this client is released, that is, the earliest
+        time at which a vehicle may leave the depot to visit this client.
+        Default 0.
     prize
         Prize collected by visiting this client. Default 0.
     required
         Whether this client must be part of a feasible solution. Default True.
     """
 
     x: int
     y: int
     demand: int
     service_duration: int
     tw_early: int
     tw_late: int
+    release_time: int
     prize: int
     required: bool
-
     def __init__(
         self,
         x: int,
         y: int,
         demand: int = 0,
         service_duration: int = 0,
         tw_early: int = 0,
         tw_late: int = 0,
+        release_time: int = 0,
         prize: int = 0,
         required: bool = True,
     ) -> None: ...
 
+class VehicleType:
+    """
+    Simple data object storing all vehicle type data as properties.
+
+    Attributes
+    ----------
+    capacity
+        Capacity (maximum total demand) of this vehicle type.
+    num_available
+        Number of vehicles of this type that are available.
+    """
+
+    capacity: int
+    num_available: int
+    def __init__(self, capacity: int, num_available: int) -> None: ...
+
 class ProblemData:
     """
     Creates a problem data instance. This instance contains all information
     needed to solve the vehicle routing problem.
 
     Parameters
     ----------
     clients
         List of clients. The first client (at index 0) is assumed to be the
         depot. The time window for the depot is assumed to describe the overall
         time horizon. The depot should have 0 demand and 0 service duration.
-    nb_vehicles
-        The number of vehicles in this problem instance.
-    vehicle_cap
-        Homogenous vehicle capacity for all vehicles in the problem instance.
+    vehicle_types
+        List of vehicle types in the problem instance.
     duration_matrix
         A matrix that gives the travel times between clients (and the depot at
         index 0).
     """
 
     def __init__(
         self,
         clients: List[Client],
-        nb_vehicles: int,
-        vehicle_cap: int,
+        vehicle_types: List[VehicleType],
         distance_matrix: List[List[int]],
         duration_matrix: List[List[int]],
     ): ...
     def client(self, client: int) -> Client:
         """
         Returns client data for the given client.
 
@@ -100,14 +116,37 @@
         as the client with number `0`.
 
         Returns
         -------
         Client
             A simple data object containing the depot's information.
         """
+    def centroid(self) -> Tuple[float, float]:
+        """
+        Center point of all client locations (excluding the depot).
+
+        Returns
+        -------
+        tuple
+            Centroid of all client locations.
+        """
+    def vehicle_type(self, vehicle_type: int) -> VehicleType:
+        """
+        Returns vehicle type data for the given vehicle type.
+
+        Parameters
+        ----------
+        vehicle_type
+            Vehicle type number whose information to retrieve.
+
+        Returns
+        -------
+        VehicleType
+            A simple data object containing the vehicle type information.
+        """
     def dist(self, first: int, second: int) -> int:
         """
         Returns the travel distance between the first and second argument,
         according to this instance's travel distance matrix.
 
         Parameters
         ----------
@@ -134,32 +173,14 @@
             Client or depot number.
 
         Returns
         -------
         int
             Travel duration between the given clients.
         """
-    def distance_matrix(self) -> Matrix:
-        """
-        Returns the travel distance matrix used for distance computations.
-
-        Returns
-        -------
-        Matrix
-            Travel distance matrix.
-        """
-    def duration_matrix(self) -> Matrix:
-        """
-        Returns the travel duration matrix used for duration computations.
-
-        Returns
-        -------
-        Matrix
-            Travel duration matrix.
-        """
     @property
     def num_clients(self) -> int:
         """
         Number of clients in this problem instance.
 
         Returns
         -------
@@ -170,20 +191,19 @@
     def num_vehicles(self) -> int:
         """
         Number of vehicles in this problem instance.
 
         Returns
         -------
         int
-            Number of vehicles in the instance.
+            Number of vehicles in this problem instance.
         """
     @property
-    def vehicle_capacity(self) -> int:
+    def num_vehicle_types(self) -> int:
         """
-        Returns the homogenous vehicle capacities of all vehicles in this
-        problem data instance.
+        Number of vehicle types in this problem instance.
 
         Returns
         -------
         int
-            Capacity of each vehicle in the instance.
+            Number of vehicle types in this problem instance.
         """
```

### Comparing `pyvrp-0.3.0/pyvrp/_TimeWindowSegment.pyi` & `pyvrp-0.4.1/pyvrp/_TimeWindowSegment.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -7,32 +7,35 @@
         self,
         idx_first: int,
         idx_last: int,
         duration: int,
         time_warp: int,
         tw_early: int,
         tw_late: int,
+        release_time: int,
     ) -> None:
         """
         Creates a time window segment.
 
         Parameters
         ----------
         idx_first
-            Index of the first customer in the route segment.
+            Index of the first client in the route segment.
         idx_last
-            Index of the last customer in the route segment.
+            Index of the last client in the route segment.
         duration
             Total duration, including waiting time.
         time_warp
             Total time warp on the route segment.
         tw_early
             Earliest visit moment of the first client.
         tw_late
-            Latest visit moment of the last client.
+            Latest visit moment of the first client.
+        release_time
+            Earliest moment to start the route segment.
         """
     @overload
     @staticmethod
     def merge(
         duration_matrix: Matrix,
         first: TimeWindowSegment,
         second: TimeWindowSegment,
@@ -47,26 +50,14 @@
         first: TimeWindowSegment,
         second: TimeWindowSegment,
         third: TimeWindowSegment,
     ) -> TimeWindowSegment:
         """
         Merges three time window segments, in order.
         """
-    @overload
-    @staticmethod
-    def merge(
-        duration_matrix: Matrix,
-        first: TimeWindowSegment,
-        second: TimeWindowSegment,
-        third: TimeWindowSegment,
-        fourth: TimeWindowSegment,
-    ) -> TimeWindowSegment:
-        """
-        Merges four time window segments, in order.
-        """
     def total_time_warp(self) -> int:
         """
         Returns the total time warp on this route segment.
 
         Returns
         -------
         int
```

### Comparing `pyvrp-0.3.0/pyvrp/__init__.py` & `pyvrp-0.4.1/pyvrp/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .GeneticAlgorithm import GeneticAlgorithm, GeneticAlgorithmParams
+from .Model import Model
 from .PenaltyManager import PenaltyManager, PenaltyParams
 from .Population import Population, PopulationParams
 from .Result import Result
 from .Statistics import Statistics
 from ._CostEvaluator import CostEvaluator
-from ._Individual import Individual, Route
 from ._Matrix import Matrix
-from ._ProblemData import Client, ProblemData
+from ._ProblemData import Client, ProblemData, VehicleType
+from ._Solution import Route, Solution
 from ._XorShift128 import XorShift128
 from .read import read, read_solution
 from .show_versions import show_versions
```

### Comparing `pyvrp-0.3.0/pyvrp/cli.py` & `pyvrp-0.4.1/pyvrp/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 try:
     import tomli
     from tqdm.contrib.concurrent import process_map
 except ModuleNotFoundError:
     msg = "Install 'tqdm' and 'tomli' to use the command line program."
     raise ModuleNotFoundError(msg)
 
-import pyvrp.educate
+import pyvrp.search
 from pyvrp import (
     GeneticAlgorithm,
     GeneticAlgorithmParams,
-    Individual,
     PenaltyManager,
     PenaltyParams,
     Population,
     PopulationParams,
     Result,
+    Solution,
     XorShift128,
 )
 from pyvrp.crossover import selective_route_exchange as srex
 from pyvrp.diversity import broken_pairs_distance as bpd
-from pyvrp.educate import (
+from pyvrp.read import INSTANCE_FORMATS, ROUND_FUNCS, read
+from pyvrp.search import (
     NODE_OPERATORS,
     ROUTE_OPERATORS,
     LocalSearch,
     NeighbourhoodParams,
     compute_neighbours,
 )
-from pyvrp.read import INSTANCE_FORMATS, ROUND_FUNCS, read
 from pyvrp.stop import MaxIterations, MaxRuntime
 
 
 def tabulate(headers: List[str], rows: np.ndarray) -> str:
     """
     Creates a simple table from the given header and row data.
     """
@@ -132,29 +132,28 @@
     pop = Population(bpd, params=pop_params)
 
     neighbours = compute_neighbours(data, nb_params)
     ls = LocalSearch(data, rng, neighbours)
 
     node_ops = NODE_OPERATORS
     if "node_ops" in config:
-        node_ops = [getattr(pyvrp.educate, op) for op in config["node_ops"]]
+        node_ops = [getattr(pyvrp.search, op) for op in config["node_ops"]]
 
     for op in node_ops:
         ls.add_node_operator(op(data))
 
     route_ops = ROUTE_OPERATORS
     if "route_ops" in config:
-        route_ops = [getattr(pyvrp.educate, op) for op in config["route_ops"]]
+        route_ops = [getattr(pyvrp.search, op) for op in config["route_ops"]]
 
     for op in route_ops:
         ls.add_route_operator(op(data))
 
     init = [
-        Individual.make_random(data, rng)
-        for _ in range(pop_params.min_pop_size)
+        Solution.make_random(data, rng) for _ in range(pop_params.min_pop_size)
     ]
     algo = GeneticAlgorithm(
         data, pen_manager, rng, pop, ls, srex, init, gen_params
     )
 
     if max_runtime is not None:
         stop = MaxRuntime(max_runtime)
@@ -171,23 +170,24 @@
 
     if sol_dir:
         instance_name = Path(data_loc).stem
         where = Path(sol_dir) / (instance_name + ".sol")
 
         with open(where, "w") as fh:
             fh.write(str(result.best))
+            fh.write(f"Cost: {result.cost()}\n")
 
     return result
 
 
 def benchmark_solve(instance: str, **kwargs):
     """
     Small wrapper script around ``solve()`` that translates result objects into
     a few key statistics, and returns those. This is needed because the result
-    solution (of type ``Individual``) cannot be pickled.
+    solution (of type ``Solution``) cannot be pickled.
     """
     res = solve(instance, **kwargs)
     instance_name = Path(instance).stem
 
     return (
         instance_name,
         "Y" if res.is_feasible() else "N",
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/Individual.cpp` & `pyvrp-0.4.1/pyvrp/cpp/Solution.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,133 +1,182 @@
-#include "Individual.h"
+#include "Solution.h"
 #include "ProblemData.h"
 
 #include <fstream>
 #include <numeric>
-#include <sstream>
+#include <unordered_map>
 
 using Client = int;
 using Visits = std::vector<Client>;
-using Routes = std::vector<Individual::Route>;
+using Routes = std::vector<Solution::Route>;
 
-void Individual::evaluate(ProblemData const &data)
+void Solution::evaluate(ProblemData const &data)
 {
-    size_t allPrizes = 0;
+    Cost allPrizes = 0;
     for (size_t client = 1; client <= data.numClients(); ++client)
         allPrizes += data.client(client).prize;
 
     for (auto const &route : routes_)
     {
-        if (route.empty())  // First empty route. All subsequent routes are
-            break;          // empty as well.
-
         // Whole solution statistics.
-        numRoutes_++;
         numClients_ += route.size();
         prizes_ += route.prizes();
         distance_ += route.distance();
         timeWarp_ += route.timeWarp();
         excessLoad_ += route.excessLoad();
     }
 
     uncollectedPrizes_ = allPrizes - prizes_;
 }
 
-size_t Individual::numRoutes() const { return numRoutes_; }
+size_t Solution::numRoutes() const { return routes_.size(); }
 
-size_t Individual::numClients() const { return numClients_; }
+size_t Solution::numClients() const { return numClients_; }
 
-Routes const &Individual::getRoutes() const { return routes_; }
+Routes const &Solution::getRoutes() const { return routes_; }
 
-std::vector<std::pair<Client, Client>> const &Individual::getNeighbours() const
+std::vector<std::pair<Client, Client>> const &Solution::getNeighbours() const
 {
     return neighbours;
 }
 
-bool Individual::isFeasible() const
-{
-    return !hasExcessLoad() && !hasTimeWarp();
-}
+bool Solution::isFeasible() const { return !hasExcessLoad() && !hasTimeWarp(); }
 
-bool Individual::hasExcessLoad() const { return excessLoad_ > 0; }
+bool Solution::hasExcessLoad() const { return excessLoad_ > 0; }
 
-bool Individual::hasTimeWarp() const { return timeWarp_ > 0; }
+bool Solution::hasTimeWarp() const { return timeWarp_ > 0; }
 
-size_t Individual::distance() const { return distance_; }
+Distance Solution::distance() const { return distance_; }
 
-size_t Individual::excessLoad() const { return excessLoad_; }
+Load Solution::excessLoad() const { return excessLoad_; }
 
-size_t Individual::prizes() const { return prizes_; }
+Cost Solution::prizes() const { return prizes_; }
 
-size_t Individual::uncollectedPrizes() const { return uncollectedPrizes_; }
+Cost Solution::uncollectedPrizes() const { return uncollectedPrizes_; }
 
-size_t Individual::timeWarp() const { return timeWarp_; }
+Duration Solution::timeWarp() const { return timeWarp_; }
 
-void Individual::makeNeighbours()
+void Solution::makeNeighbours()
 {
     for (auto const &route : routes_)
         for (size_t idx = 0; idx != route.size(); ++idx)
             neighbours[route[idx]]
                 = {idx == 0 ? 0 : route[idx - 1],                  // pred
                    idx == route.size() - 1 ? 0 : route[idx + 1]};  // succ
 }
 
-bool Individual::operator==(Individual const &other) const
+bool Solution::operator==(Solution const &other) const
 {
-    // First compare simple attributes, since that's a quick and cheap check.
-    // Only when these are the same we test if the neighbours are all equal.
-    // clang-format off
-    return distance_ == other.distance_
-        && excessLoad_ == other.excessLoad_
-        && timeWarp_ == other.timeWarp_
-        && numRoutes_ == other.numRoutes_
-        && neighbours == other.neighbours;
-    // clang-format on
+    // First compare simple attributes, since that's quick and cheap.
+    bool const simpleChecks = distance_ == other.distance_
+                              && excessLoad_ == other.excessLoad_
+                              && timeWarp_ == other.timeWarp_
+                              && routes_.size() == other.routes_.size();
+
+    if (!simpleChecks)
+        return false;
+
+    // Now test if the neighbours are all equal. If that's the case we have
+    // the same visit structure across routes.
+    if (neighbours != other.neighbours)
+        return false;
+
+    // The visits are the same for both solutions, but the vehicle assignments
+    // need not be. We check this via a mapping from the first client in each
+    // route to the vehicle type of that route. We need to base this on the
+    // visits since the routes need not be in the same order between solutions.
+    std::unordered_map<Client, VehicleType> client2vehType;
+    for (auto const &route : routes_)
+        client2vehType[route.visits()[0]] = route.vehicleType();
+
+    for (auto const &route : other.routes_)
+        if (client2vehType[route.visits()[0]] != route.vehicleType())
+            return false;
+
+    return true;
 }
 
-Individual::Individual(ProblemData const &data, XorShift128 &rng)
-    : routes_(data.numVehicles()), neighbours(data.numClients() + 1, {0, 0})
+Solution::Solution(ProblemData const &data, XorShift128 &rng)
+    : neighbours(data.numClients() + 1, {0, 0})
 {
     // Shuffle clients (to create random routes)
     auto clients = std::vector<int>(data.numClients());
     std::iota(clients.begin(), clients.end(), 1);
     std::shuffle(clients.begin(), clients.end(), rng);
 
     // Distribute clients evenly over the routes: the total number of clients
     // per vehicle, with an adjustment in case the division is not perfect.
     auto const numVehicles = data.numVehicles();
     auto const numClients = data.numClients();
-    auto const perVehicle = std::max(numClients / numVehicles, size_t(1));
+    auto const perVehicle = std::max<size_t>(numClients / numVehicles, 1);
     auto const perRoute = perVehicle + (numClients % numVehicles != 0);
+    auto const numRoutes = (numClients + perRoute - 1) / perRoute;
 
-    std::vector<std::vector<Client>> routes(data.numVehicles());
+    std::vector<std::vector<Client>> routes(numRoutes);
     for (size_t idx = 0; idx != numClients; ++idx)
         routes[idx / perRoute].push_back(clients[idx]);
 
-    for (size_t idx = 0; idx != routes.size(); ++idx)
-        routes_[idx] = Route(data, routes[idx]);
+    routes_.reserve(numRoutes);
+    size_t count = 0;
+    for (size_t vehType = 0; vehType != data.numVehicleTypes(); ++vehType)
+    {
+        auto const numAvailable = data.vehicleType(vehType).numAvailable;
+        for (size_t i = 0; i != numAvailable; ++i)
+            if (count < routes.size())
+                routes_.emplace_back(data, routes[count++], vehType);
+    }
 
     makeNeighbours();
     evaluate(data);
 }
 
-Individual::Individual(ProblemData const &data,
-                       std::vector<std::vector<Client>> const &routes)
-    : routes_(data.numVehicles()), neighbours(data.numClients() + 1, {0, 0})
+Solution::Solution(ProblemData const &data,
+                   std::vector<std::vector<Client>> const &routes)
+{
+    Routes transformedRoutes;
+    transformedRoutes.reserve(routes.size());
+    for (auto const &visits : routes)
+        transformedRoutes.emplace_back(data, visits, 0);
+
+    *this = Solution(data, transformedRoutes);
+}
+
+Solution::Solution(ProblemData const &data, std::vector<Route> const &routes)
+    : routes_(routes), neighbours(data.numClients() + 1, {0, 0})
 {
     if (routes.size() > data.numVehicles())
     {
         auto const msg = "Number of routes must not exceed number of vehicles.";
         throw std::runtime_error(msg);
     }
 
     std::vector<size_t> visits(data.numClients() + 1, 0);
+    std::vector<size_t> usedVehicles(data.numVehicleTypes(), 0);
     for (auto const &route : routes)
+    {
+        if (route.empty())
+        {
+            auto const msg = "Solution should not contain empty routes.";
+            throw std::runtime_error(msg);
+        }
+
+        usedVehicles[route.vehicleType()]++;
         for (auto const client : route)
             visits[client]++;
+    }
+
+    for (size_t vehType = 0; vehType != data.numVehicleTypes(); vehType++)
+        if (usedVehicles[vehType] > data.vehicleType(vehType).numAvailable)
+        {
+            std::ostringstream msg;
+            auto const numAvailable = data.vehicleType(vehType).numAvailable;
+            msg << "Used more than " << numAvailable << " vehicles of type "
+                << vehType << '.';
+            throw std::runtime_error(msg.str());
+        }
 
     for (size_t client = 1; client <= data.numClients(); ++client)
     {
         if (data.client(client).required && visits[client] == 0)
         {
             std::ostringstream msg;
             msg << "Client " << client << " is required but not present.";
@@ -138,46 +187,45 @@
         {
             std::ostringstream msg;
             msg << "Client " << client << " is visited more than once.";
             throw std::runtime_error(msg.str());
         }
     }
 
-    for (size_t idx = 0; idx != routes.size(); ++idx)
-        routes_[idx] = Route(data, routes[idx]);
-
-    // a precedes b only when a is not empty and b is. Combined with a stable
-    // sort, this ensures we keep the original sorting as much as possible, but
-    // also make sure all empty routes are at the end of routes_.
-    auto comp = [](auto &a, auto &b) { return !a.empty() && b.empty(); };
-    std::stable_sort(routes_.begin(), routes_.end(), comp);
-
     makeNeighbours();
     evaluate(data);
 }
 
-Individual::Route::Route(ProblemData const &data, Visits const visits)
-    : visits_(std::move(visits))
+Solution::Route::Route(ProblemData const &data,
+                       Visits const visits,
+                       size_t const vehicleType)
+    : visits_(std::move(visits)), centroid_({0, 0}), vehicleType_(vehicleType)
 {
     if (visits_.empty())
         return;
 
-    int time = data.depot().twEarly;
+    for (size_t idx = 0; idx != size(); ++idx)
+        release_ = std::max(release_, data.client(visits_[idx]).releaseTime);
+
+    Duration time = std::max(release_, data.depot().twEarly);
     int prevClient = 0;
 
     for (size_t idx = 0; idx != size(); ++idx)
     {
         auto const &clientData = data.client(visits_[idx]);
 
         distance_ += data.dist(prevClient, visits_[idx]);
         duration_ += data.duration(prevClient, visits_[idx]);
         demand_ += clientData.demand;
         service_ += clientData.serviceDuration;
         prizes_ += clientData.prize;
 
+        centroid_.first += static_cast<double>(clientData.x) / size();
+        centroid_.second += static_cast<double>(clientData.y) / size();
+
         time += data.client(prevClient).serviceDuration
                 + data.duration(prevClient, visits_[idx]);
 
         if (time < clientData.twEarly)  // add wait duration
         {
             wait_ += clientData.twEarly - time;
             time = clientData.twEarly;
@@ -191,82 +239,101 @@
 
         prevClient = visits_[idx];
     }
 
     Client const last = visits_.back();  // last client has depot as successor
     distance_ += data.dist(last, 0);
     duration_ += data.duration(last, 0);
+
     time += data.client(last).serviceDuration + data.duration(last, 0);
-    timeWarp_ += std::max(time - data.depot().twLate, 0);  // depot closing tw
-    excessLoad_ = data.vehicleCapacity() < demand_
-                      ? demand_ - data.vehicleCapacity()
-                      : 0;
+    timeWarp_ += std::max<Duration>(time - data.depot().twLate, 0);
+
+    auto const capacity = data.vehicleType(vehicleType).capacity;
+    excessLoad_ = capacity < demand_ ? demand_ - capacity : 0;
 }
 
-bool Individual::Route::empty() const { return visits_.empty(); }
+bool Solution::Route::empty() const { return visits_.empty(); }
 
-size_t Individual::Route::size() const { return visits_.size(); }
+size_t Solution::Route::size() const { return visits_.size(); }
 
-Client Individual::Route::operator[](size_t idx) const { return visits_[idx]; }
+Client Solution::Route::operator[](size_t idx) const { return visits_[idx]; }
 
-Visits::const_iterator Individual::Route::begin() const
+Visits::const_iterator Solution::Route::begin() const
 {
     return visits_.cbegin();
 }
 
-Visits::const_iterator Individual::Route::end() const { return visits_.cend(); }
+Visits::const_iterator Solution::Route::end() const { return visits_.cend(); }
 
-Visits::const_iterator Individual::Route::cbegin() const
+Visits::const_iterator Solution::Route::cbegin() const
 {
     return visits_.cbegin();
 }
 
-Visits::const_iterator Individual::Route::cend() const
-{
-    return visits_.cend();
-}
+Visits::const_iterator Solution::Route::cend() const { return visits_.cend(); }
+
+Visits const &Solution::Route::visits() const { return visits_; }
 
-Visits const &Individual::Route::visits() const { return visits_; }
+Distance Solution::Route::distance() const { return distance_; }
 
-size_t Individual::Route::distance() const { return distance_; }
+Load Solution::Route::demand() const { return demand_; }
 
-size_t Individual::Route::demand() const { return demand_; }
+Load Solution::Route::excessLoad() const { return excessLoad_; }
 
-size_t Individual::Route::excessLoad() const { return excessLoad_; }
+Duration Solution::Route::duration() const { return duration_; }
 
-size_t Individual::Route::duration() const { return duration_; }
+Duration Solution::Route::serviceDuration() const { return service_; }
 
-size_t Individual::Route::serviceDuration() const { return service_; }
+Duration Solution::Route::timeWarp() const { return timeWarp_; }
 
-size_t Individual::Route::timeWarp() const { return timeWarp_; }
+Duration Solution::Route::waitDuration() const { return wait_; }
 
-size_t Individual::Route::waitDuration() const { return wait_; }
+Duration Solution::Route::releaseTime() const { return release_; }
 
-size_t Individual::Route::prizes() const { return prizes_; }
+Cost Solution::Route::prizes() const { return prizes_; }
 
-bool Individual::Route::isFeasible() const
+std::pair<double, double> const &Solution::Route::centroid() const
+{
+    return centroid_;
+}
+
+size_t Solution::Route::vehicleType() const { return vehicleType_; }
+
+bool Solution::Route::isFeasible() const
 {
     return !hasExcessLoad() && !hasTimeWarp();
 }
 
-bool Individual::Route::hasExcessLoad() const { return excessLoad_ > 0; }
+bool Solution::Route::hasExcessLoad() const { return excessLoad_ > 0; }
 
-bool Individual::Route::hasTimeWarp() const { return timeWarp_ > 0; }
+bool Solution::Route::hasTimeWarp() const { return timeWarp_ > 0; }
 
-std::ostream &operator<<(std::ostream &out, Individual const &indiv)
+bool Solution::Route::operator==(Solution::Route const &other) const
 {
-    auto const &routes = indiv.getRoutes();
+    // First compare simple attributes, since that's a quick and cheap check.
+    // Only when these are the same we test if the visits are all equal.
 
-    for (size_t idx = 0; idx != indiv.numRoutes(); ++idx)
+    // clang-format off
+    return distance_ == other.distance_
+        && demand_ == other.demand_
+        && timeWarp_ == other.timeWarp_
+        && vehicleType_ == other.vehicleType_
+        && visits_ == other.visits_;
+    // clang-format on
+}
+
+std::ostream &operator<<(std::ostream &out, Solution const &sol)
+{
+    auto const &routes = sol.getRoutes();
+
+    for (size_t idx = 0; idx != routes.size(); ++idx)
         out << "Route #" << idx + 1 << ": " << routes[idx] << '\n';
 
-    out << "Distance: " << indiv.distance() << '\n';
-    out << "Prizes: " << indiv.prizes() << '\n';
     return out;
 }
 
-std::ostream &operator<<(std::ostream &out, Individual::Route const &route)
+std::ostream &operator<<(std::ostream &out, Solution::Route const &route)
 {
     for (Client const client : route)
         out << client << ' ';
     return out;
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/Individual.h` & `pyvrp-0.4.1/pyvrp/cpp/Solution.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,127 @@
-#ifndef INDIVIDUAL_H
-#define INDIVIDUAL_H
+#ifndef PYVRP_SOLUTION_H
+#define PYVRP_SOLUTION_H
 
+#include "Measure.h"
 #include "ProblemData.h"
 #include "XorShift128.h"
 
+#include <functional>
 #include <iosfwd>
 #include <vector>
 
-class Individual
+class Solution
 {
-    friend struct std::hash<Individual>;  // friend struct to enable hashing
+    friend struct std::hash<Solution>;  // friend struct to enable hashing
 
     using Client = int;
+    using VehicleType = size_t;
 
 public:
     /**
      * A simple Route class that contains the route plan and some statistics.
      */
     class Route
     {
         using Visits = std::vector<Client>;
 
         Visits visits_ = {};     // Client visits on this route
-        size_t distance_ = 0;    // Total travel distance on this route
-        size_t demand_ = 0;      // Total demand served on this route
-        size_t excessLoad_ = 0;  // Demand in excess of the vehicle's capacity
-        size_t duration_ = 0;    // Total travel duration on this route
-        size_t service_ = 0;     // Total service duration on this route
-        size_t timeWarp_ = 0;    // Total time warp on this route
-        size_t wait_ = 0;        // Total waiting duration on this route
-        size_t prizes_ = 0;      // Total prize value collected on this route
+        Distance distance_ = 0;  // Total travel distance on this route
+        Load demand_ = 0;        // Total demand served on this route
+        Load excessLoad_ = 0;    // Excess demand (wrt vehicle capacity)
+        Duration duration_ = 0;  // Total travel duration on this route
+        Duration service_ = 0;   // Total service duration on this route
+        Duration timeWarp_ = 0;  // Total time warp on this route
+        Duration wait_ = 0;      // Total waiting duration on this route
+        Duration release_ = 0;   // Release time of this route
+        Cost prizes_ = 0;        // Total value of prizes on this route
+
+        std::pair<double, double> centroid_;  // center of the route
+        VehicleType vehicleType_ = 0;         // Type of vehicle of this route
 
     public:
         [[nodiscard]] bool empty() const;
         [[nodiscard]] size_t size() const;
         [[nodiscard]] Client operator[](size_t idx) const;
 
         Visits::const_iterator begin() const;
         Visits::const_iterator end() const;
         Visits::const_iterator cbegin() const;
         Visits::const_iterator cend() const;
 
         [[nodiscard]] Visits const &visits() const;
-        [[nodiscard]] size_t distance() const;
-        [[nodiscard]] size_t demand() const;
-        [[nodiscard]] size_t excessLoad() const;
-        [[nodiscard]] size_t duration() const;
-        [[nodiscard]] size_t serviceDuration() const;
-        [[nodiscard]] size_t timeWarp() const;
-        [[nodiscard]] size_t waitDuration() const;
-        [[nodiscard]] size_t prizes() const;
+        [[nodiscard]] Distance distance() const;
+        [[nodiscard]] Load demand() const;
+        [[nodiscard]] Load excessLoad() const;
+        [[nodiscard]] Duration duration() const;
+        [[nodiscard]] Duration serviceDuration() const;
+        [[nodiscard]] Duration timeWarp() const;
+        [[nodiscard]] Duration waitDuration() const;
+        [[nodiscard]] Duration releaseTime() const;
+        [[nodiscard]] Cost prizes() const;
+
+        [[nodiscard]] std::pair<double, double> const &centroid() const;
+        [[nodiscard]] VehicleType vehicleType() const;
 
         [[nodiscard]] bool isFeasible() const;
         [[nodiscard]] bool hasExcessLoad() const;
         [[nodiscard]] bool hasTimeWarp() const;
 
+        bool operator==(Route const &other) const;
+
         Route() = default;  // default is empty
-        Route(ProblemData const &data, Visits const visits);
+        Route(ProblemData const &data,
+              Visits const visits,
+              VehicleType const vehicleType);
     };
 
 private:
     using Routes = std::vector<Route>;
 
-    size_t numRoutes_ = 0;          // Number of routes
-    size_t numClients_ = 0;         // Number of clients in the solution
-    size_t distance_ = 0;           // Total distance
-    size_t excessLoad_ = 0;         // Total excess load over all routes
-    size_t prizes_ = 0;             // Total collected prize value
-    size_t uncollectedPrizes_ = 0;  // Total uncollected prize value
-    size_t timeWarp_ = 0;           // Total time warp over all routes
+    size_t numClients_ = 0;       // Number of clients in the solution
+    Distance distance_ = 0;       // Total distance
+    Load excessLoad_ = 0;         // Total excess load over all routes
+    Cost prizes_ = 0;             // Total collected prize value
+    Cost uncollectedPrizes_ = 0;  // Total uncollected prize value
+    Duration timeWarp_ = 0;       // Total time warp over all routes
 
-    Routes routes_;  // Routes - only the first numRoutes_ are non-empty
+    Routes routes_;
     std::vector<std::pair<Client, Client>> neighbours;  // pairs of [pred, succ]
 
     // Determines the [pred, succ] pairs for each client.
     void makeNeighbours();
 
     // Evaluates this solution's characteristics.
     void evaluate(ProblemData const &data);
 
+    // These are only available within a solution; from the outside a solution
+    // is immutable.
+    Solution &operator=(Solution const &other) = default;
+    Solution &operator=(Solution &&other) = default;
+
 public:
     /**
-     * Returns the number of non-empty routes in this individual's solution.
-     * Such non-empty routes are guaranteed to be in the lower indices of the
-     * routes returned by ``getRoutes``.
+     * Returns the number of routes in this solution. Equal to the length of
+     * the vector of routes returned by ``getRoutes``.
      */
     [[nodiscard]] size_t numRoutes() const;
 
     /**
      * Number of clients in the solution.
      */
     [[nodiscard]] size_t numClients() const;
 
     /**
-     * Returns this individual's routing decisions.
+     * Returns the routing decisions.
      */
     [[nodiscard]] Routes const &getRoutes() const;
 
     /**
      * Returns a vector of [pred, succ] clients for each client (index) in this
-     * individual's routes. Includes the depot at index 0.
+     * solutions's routes. Includes the depot at index 0.
      */
     [[nodiscard]] std::vector<std::pair<Client, Client>> const &
     getNeighbours() const;
 
     /**
      * @return True when this solution is feasible; false otherwise.
      */
@@ -118,78 +136,82 @@
      * @return True if the solution violates time window constraints.
      */
     [[nodiscard]] bool hasTimeWarp() const;
 
     /**
      * @return Total distance over all routes.
      */
-    [[nodiscard]] size_t distance() const;
+    [[nodiscard]] Distance distance() const;
 
     /**
      * @return Total excess load over all routes.
      */
-    [[nodiscard]] size_t excessLoad() const;
+    [[nodiscard]] Load excessLoad() const;
 
     /**
      * @return Total collected prize value over all routes.
      */
-    [[nodiscard]] size_t prizes() const;
+    [[nodiscard]] Cost prizes() const;
 
     /**
      * @return Total prize value of all unvisited clients.
      */
-    [[nodiscard]] size_t uncollectedPrizes() const;
+    [[nodiscard]] Cost uncollectedPrizes() const;
 
     /**
      * @return Total time warp over all routes.
      */
-    [[nodiscard]] size_t timeWarp() const;
+    [[nodiscard]] Duration timeWarp() const;
 
-    bool operator==(Individual const &other) const;
+    bool operator==(Solution const &other) const;
 
-    Individual &operator=(Individual const &other) = delete;  // is immutable
-    Individual &operator=(Individual &&other) = delete;       // is immutable
+    Solution(Solution const &other) = default;
+    Solution(Solution &&other) = default;
 
-    Individual(Individual const &other) = default;
-    Individual(Individual &&other) = default;
+    /**
+     * Constructs a random solution using the given random number generator.
+     *
+     * @param data Data instance describing the problem that's being solved.
+     * @param rng  Random number generator.
+     */
+    Solution(ProblemData const &data, XorShift128 &rng);
 
     /**
-     * Constructs a random individual using the given random number generator.
+     * Constructs a solution using routes given as lists of client indices.
+     * This constructor assumes all routes use vehicles having vehicle type 0.
      *
-     * @param data           Data instance describing the problem that's being
-     *                       solved.
-     * @param rng            Random number generator.
+     * @param data   Data instance describing the problem that's being solved.
+     * @param routes Solution's route list.
      */
-    Individual(ProblemData const &data, XorShift128 &rng);
+    Solution(ProblemData const &data,
+             std::vector<std::vector<Client>> const &routes);
 
     /**
-     * Constructs an individual having the given routes as its solution.
+     * Constructs a solution from the given list of Routes.
      *
-     * @param data           Data instance describing the problem that's being
-     *                       solved.
-     * @param routes         Solution's route list.
+     * @param data   Data instance describing the problem that's being solved.
+     * @param routes Solution's route list.
      */
-    Individual(ProblemData const &data,
-               std::vector<std::vector<Client>> const &routes);
+    Solution(ProblemData const &data, std::vector<Route> const &routes);
 };
 
-std::ostream &operator<<(std::ostream &out, Individual const &indiv);
-std::ostream &operator<<(std::ostream &out, Individual::Route const &route);
+std::ostream &operator<<(std::ostream &out, Solution const &sol);
+std::ostream &operator<<(std::ostream &out, Solution::Route const &route);
 
 namespace std
 {
-template <> struct hash<Individual>
+template <> struct hash<Solution>
 {
-    std::size_t operator()(Individual const &individual) const
+    size_t operator()(Solution const &sol) const
     {
         size_t res = 17;
-        res = res * 31 + std::hash<size_t>()(individual.numRoutes_);
-        res = res * 31 + std::hash<size_t>()(individual.distance_);
-        res = res * 31 + std::hash<size_t>()(individual.excessLoad_);
-        res = res * 31 + std::hash<size_t>()(individual.timeWarp_);
+        res = res * 31 + std::hash<size_t>()(sol.routes_.size());
+        res = res * 31 + std::hash<Distance>()(sol.distance_);
+        res = res * 31 + std::hash<Load>()(sol.excessLoad_);
+        res = res * 31 + std::hash<Duration>()(sol.timeWarp_);
 
         return res;
     }
 };
 }  // namespace std
 
-#endif
+#endif  // PYVRP_SOLUTION_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/Matrix.h` & `pyvrp-0.4.1/pyvrp/cpp/Matrix.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef MATRIX_H
-#define MATRIX_H
+#ifndef PYVRP_MATRIX_H
+#define PYVRP_MATRIX_H
 
 #include <algorithm>
 #include <sstream>
 #include <stdexcept>
 #include <vector>
 
 template <typename T> class Matrix
@@ -36,14 +36,18 @@
      */
     explicit Matrix(std::vector<std::vector<T>> const &data);
 
     [[nodiscard]] decltype(auto) operator()(size_t row, size_t col);
 
     [[nodiscard]] decltype(auto) operator()(size_t row, size_t col) const;
 
+    [[nodiscard]] size_t numCols() const;
+
+    [[nodiscard]] size_t numRows() const;
+
     /**
      * @return Maximum element in the matrix.
      */
     [[nodiscard]] T max() const;
 
     /**
      * @return Matrix size.
@@ -91,15 +95,19 @@
 
 template <typename T>
 decltype(auto) Matrix<T>::operator()(size_t row, size_t col) const
 {
     return data_[cols_ * row + col];
 }
 
+template <typename T> size_t Matrix<T>::numCols() const { return cols_; }
+
+template <typename T> size_t Matrix<T>::numRows() const { return rows_; }
+
 template <typename T> T Matrix<T>::max() const
 {
     return *std::max_element(data_.begin(), data_.end());
 }
 
 template <typename T> size_t Matrix<T>::size() const { return data_.size(); }
 
-#endif
+#endif  // PYVRP_MATRIX_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/Matrix_bindings.cpp` & `pyvrp-0.4.1/pyvrp/cpp/Matrix_bindings.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 PYBIND11_MODULE(_Matrix, m)
 {
     py::class_<Matrix<int>>(m, "Matrix")
         .def(py::init<size_t>(), py::arg("dimension"))
         .def(py::init<size_t, size_t>(), py::arg("n_rows"), py::arg("n_cols"))
         .def(py::init<std::vector<std::vector<int>>>(), py::arg("data"))
+        .def_property_readonly("num_cols", &Matrix<int>::numCols)
+        .def_property_readonly("num_rows", &Matrix<int>::numRows)
         .def(
             "__getitem__",
             [](Matrix<int> &m, std::pair<size_t, size_t> idx) -> int {
                 return m(idx.first, idx.second);
             },
             py::arg("idx"))
         .def(
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/ProblemData.cpp` & `pyvrp-0.4.1/pyvrp/cpp/ProblemData.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 #include <cmath>
 #include <fstream>
 #include <sstream>
 #include <string>
 #include <vector>
 
-ProblemData::Client::Client(int x,
-                            int y,
-                            int demand,
-                            int serviceDuration,
-                            int twEarly,
-                            int twLate,
-                            int prize,
+ProblemData::Client::Client(Coordinate x,
+                            Coordinate y,
+                            Load demand,
+                            Duration serviceDuration,
+                            Duration twEarly,
+                            Duration twLate,
+                            Duration releaseTime,
+                            Cost prize,
                             bool required)
     : x(x),
       y(y),
       demand(demand),
       serviceDuration(serviceDuration),
       twEarly(twEarly),
       twLate(twLate),
+      releaseTime(releaseTime),
       prize(prize),
       required(required)
 {
     if (demand < 0)
         throw std::invalid_argument("demand must be >= 0");
 
     if (serviceDuration < 0)
@@ -34,30 +36,44 @@
 
     if (prize < 0)
         throw std::invalid_argument("prize must be >= 0");
 }
 
 ProblemData::Client const &ProblemData::depot() const { return client(0); }
 
-Matrix<int> const &ProblemData::distanceMatrix() const { return dist_; }
+std::pair<double, double> const &ProblemData::centroid() const
+{
+    return centroid_;
+}
+
+Matrix<Distance> const &ProblemData::distanceMatrix() const { return dist_; }
 
-Matrix<int> const &ProblemData::durationMatrix() const { return dur_; }
+Matrix<Duration> const &ProblemData::durationMatrix() const { return dur_; }
 
 size_t ProblemData::numClients() const { return numClients_; }
 
-size_t ProblemData::numVehicles() const { return numVehicles_; }
+size_t ProblemData::numVehicleTypes() const { return numVehicleTypes_; }
 
-size_t ProblemData::vehicleCapacity() const { return vehicleCapacity_; }
+size_t ProblemData::numVehicles() const { return numVehicles_; }
 
 ProblemData::ProblemData(std::vector<Client> const &clients,
-                         size_t numVehicles,
-                         size_t vehicleCap,
-                         std::vector<std::vector<int>> const &distMat,
-                         std::vector<std::vector<int>> const &durMat)
-    : dist_(distMat),
-      dur_(durMat),
+                         std::vector<VehicleType> const &vehicleTypes,
+                         Matrix<Distance> const distMat,
+                         Matrix<Duration> const durMat)
+    : centroid_({0, 0}),
+      dist_(std::move(distMat)),
+      dur_(std::move(durMat)),
       clients_(clients),
-      numClients_(std::max(clients.size(), static_cast<size_t>(1)) - 1),
-      numVehicles_(numVehicles),
-      vehicleCapacity_(vehicleCap)
+      vehicleTypes_(vehicleTypes),
+      numClients_(std::max<size_t>(clients.size(), 1) - 1),
+      numVehicleTypes_(vehicleTypes.size()),
+      numVehicles_(0)
 {
+    for (auto const &vehicleType : vehicleTypes)
+        numVehicles_ += vehicleType.numAvailable;
+
+    for (size_t idx = 1; idx <= numClients(); ++idx)
+    {
+        centroid_.first += static_cast<double>(clients[idx].x) / numClients();
+        centroid_.second += static_cast<double>(clients[idx].y) / numClients();
+    }
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/ProblemData.h` & `pyvrp-0.4.1/pyvrp/cpp/ProblemData.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,131 +1,158 @@
-#ifndef HGS_PROBLEMDATA_H
-#define HGS_PROBLEMDATA_H
+#ifndef PYVRP_PROBLEMDATA_H
+#define PYVRP_PROBLEMDATA_H
 
 #include "Matrix.h"
+#include "Measure.h"
 #include "XorShift128.h"
 
 #include <iosfwd>
 #include <vector>
 
 class ProblemData
 {
 public:
     struct Client
     {
-        int x;                 // Coordinate X
-        int y;                 // Coordinate Y
-        int demand;            // Demand
-        int serviceDuration;   // Service duration
-        int twEarly;           // Earliest arrival (when using time windows)
-        int twLate;            // Latest arrival (when using time windows)
-        int prize = 0;         // Prize collected when visiting this client
-        bool required = true;  // Must this client be part of a solution?
-
-        Client(int x,
-               int y,
-               int demand = 0,
-               int serviceDuration = 0,
-               int twEarly = 0,
-               int twLate = 0,
-               int prize = 0,
+        Coordinate const x;
+        Coordinate const y;
+        Load const demand;
+        Duration const serviceDuration;
+        Duration const twEarly;      // Earliest possible start of service
+        Duration const twLate;       // Latest possible start of service
+        Duration const releaseTime;  // Earliest possible time to leave depot
+        Cost const prize = 0;        // Prize for visiting this client
+        bool const required = true;  // Must client be in solution?
+
+        Client(Coordinate x,
+               Coordinate y,
+               Load demand = 0,
+               Duration serviceDuration = 0,
+               Duration twEarly = 0,
+               Duration twLate = 0,
+               Duration releaseTime = 0,
+               Cost prize = 0,
                bool required = true);
     };
 
+    struct VehicleType
+    {
+        Load capacity;        // Capacity (max total demand) of the vehicle
+        size_t numAvailable;  // Number of available vehicles of this type
+    };
+
 private:
-    Matrix<int> const dist_;       // Distance matrix (+depot)
-    Matrix<int> const dur_;        // Duration matrix (+depot)
-    std::vector<Client> clients_;  // Client (+depot) information
+    std::pair<double, double> centroid_;     // Centroid of client locations
+    Matrix<Distance> const dist_;            // Distance matrix (+depot)
+    Matrix<Duration> const dur_;             // Duration matrix (+depot)
+    std::vector<Client> clients_;            // Client (+depot) information
+    std::vector<VehicleType> vehicleTypes_;  // Vehicle type information
 
     size_t const numClients_;
-    size_t const numVehicles_;
-    size_t const vehicleCapacity_;
+    size_t const numVehicleTypes_;
+    size_t numVehicles_;  // Number of vehicles - derived from vehicle types
 
 public:
     /**
      * @param client Client whose data to return.
      * @return A struct containing the indicated client's information.
      */
     [[nodiscard]] inline Client const &client(size_t client) const;
 
     /**
      * @return A struct containing the depot's information.
      */
     [[nodiscard]] Client const &depot() const;
 
     /**
+     * @return Centroid of client locations.
+     */
+    [[nodiscard]] std::pair<double, double> const &centroid() const;
+
+    /**
+     * @param vehicleType Vehicle type whose data to return.
+     * @return A struct containing the vehicle type's information.
+     */
+    [[nodiscard]] inline VehicleType const &
+    vehicleType(size_t vehicleType) const;
+
+    /**
      * Returns the distance between the indicated two clients.
      *
      * @param first  First client.
      * @param second Second client.
      * @return distance from the first to the second client.
      */
-    [[nodiscard]] inline int dist(size_t first, size_t second) const;
+    [[nodiscard]] inline Distance dist(size_t first, size_t second) const;
 
     /**
      * Returns the travel duration between the indicated two clients.
      *
      * @param first  First client.
      * @param second Second client.
      * @return Travel duration from the first to the second client.
      */
-    [[nodiscard]] inline int duration(size_t first, size_t second) const;
+    [[nodiscard]] inline Duration duration(size_t first, size_t second) const;
 
     /**
      * @return The full travel distance matrix.
      */
-    [[nodiscard]] Matrix<int> const &distanceMatrix() const;
+    [[nodiscard]] Matrix<Distance> const &distanceMatrix() const;
 
     /**
      * @return The full travel duration matrix.
      */
-    [[nodiscard]] Matrix<int> const &durationMatrix() const;
+    [[nodiscard]] Matrix<Duration> const &durationMatrix() const;
 
     /**
      * @return Total number of clients in this instance.
      */
     [[nodiscard]] size_t numClients() const;
 
     /**
-     * @return Total number of vehicles available in this instance.
+     * @return Total number of vehicle types in this instance.
      */
-    [[nodiscard]] size_t numVehicles() const;
+    [[nodiscard]] size_t numVehicleTypes() const;
 
     /**
-     * @return Capacity of each vehicle in this instance.
+     * @return Total number of vehicles available in this instance.
      */
-    [[nodiscard]] size_t vehicleCapacity() const;
+    [[nodiscard]] size_t numVehicles() const;
 
     /**
      * Constructs a ProblemData object with the given data. Assumes the list of
      * clients contains the depot, such that each vector is one longer than the
      * number of clients.
      *
      * @param clients      List of clients (including depot at index 0).
-     * @param numVehicles  Number of vehicles.
-     * @param vehicleCap   Vehicle capacity.
+     * @param vehicleTypes List of vehicle types.
      * @param distMat      Distance matrix.
      * @param durMat       Duration matrix.
      */
     ProblemData(std::vector<Client> const &clients,
-                size_t numVehicles,
-                size_t vehicleCap,
-                std::vector<std::vector<int>> const &distMat,
-                std::vector<std::vector<int>> const &durMat);
+                std::vector<VehicleType> const &vehicleTypes,
+                Matrix<Distance> const distMat,
+                Matrix<Duration> const durMat);
 };
 
 ProblemData::Client const &ProblemData::client(size_t client) const
 {
     return clients_[client];
 }
 
-int ProblemData::dist(size_t first, size_t second) const
+ProblemData::VehicleType const &
+ProblemData::vehicleType(size_t vehicleType) const
+{
+    return vehicleTypes_[vehicleType];
+}
+
+Distance ProblemData::dist(size_t first, size_t second) const
 {
     return dist_(first, second);
 }
 
-int ProblemData::duration(size_t first, size_t second) const
+Duration ProblemData::duration(size_t first, size_t second) const
 {
     return dur_(first, second);
 }
 
-#endif  // HGS_PROBLEMDATA_H
+#endif  // PYVRP_PROBLEMDATA_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/README.md` & `pyvrp-0.4.1/pyvrp/cpp/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # CPP
 
 This folder contains all C++ extension classes and functions. These extensions
 are ordered in the way they will appear in the `pyvrp` package: everything in
 this top-level folder will be made available in the top-level `pyvrp` package,
-whereas for example everything in `cpp/educate` will be present in 
-`pyvrp.educate` after installation (and so on for the other folders).
+whereas for example everything in `cpp/search` will be present in 
+`pyvrp.search` after installation (and so on for the other folders).
+
+When building on our implementation, please refrain from defining symbols 
+starting with the `PYVRP_` prefix. PyVRP reserves any such global declarations
+for internal use.
 
 We use `pybind11` to generate the Python bindings for the C++ codebase. These
 bindings are generated in the `X_bindings.cpp` source files of each object `X`
 that we want to expose to Python.
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/SubPopulation.cpp` & `pyvrp-0.4.1/pyvrp/cpp/SubPopulation.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,123 @@
 #include "SubPopulation.h"
 
 #include <numeric>
 
+using const_iter = std::vector<SubPopulation::Item>::const_iterator;
+using iter = std::vector<SubPopulation::Item>::iterator;
+
 SubPopulation::SubPopulation(DiversityMeasure divOp,
                              PopulationParams const &params)
     : divOp(divOp), params(params)
 {
 }
 
 SubPopulation::~SubPopulation()
 {
     for (auto &item : items)
-        delete item.individual;
+        delete item.solution;
 }
 
-void SubPopulation::add(Individual const *individual,
+void SubPopulation::add(Solution const *solution,
                         CostEvaluator const &costEvaluator)
 {
-    // Copy the given individual into a new memory location, and use that from
+    // Copy the given solution into a new memory location, and use that from
     // now on.
-    individual = new Individual(*individual);
-    Item item = {&params, individual, 0.0, {}};
+    solution = new Solution(*solution);
+    Item item = {&params, solution, 0.0, {}};
 
-    for (auto &other : items)  // update distance to other individuals
+    for (auto &other : items)  // update distance to other solutions
     {
-        auto const div = divOp(*individual, *other.individual);
+        auto const div = divOp(*solution, *other.solution);
         auto cmp = [](auto &elem, auto &value) { return elem.first < value; };
 
         auto &oProx = other.proximity;
         auto place = std::lower_bound(oProx.begin(), oProx.end(), div, cmp);
-        oProx.emplace(place, div, individual);
+        oProx.emplace(place, div, solution);
 
         auto &iProx = item.proximity;
         place = std::lower_bound(iProx.begin(), iProx.end(), div, cmp);
-        iProx.emplace(place, div, other.individual);
+        iProx.emplace(place, div, other.solution);
     }
 
-    items.push_back(item);  // add individual
+    items.push_back(item);  // add solution
 
     if (size() > params.maxPopSize())
         purge(costEvaluator);
 }
 
 size_t SubPopulation::size() const { return items.size(); }
 
 SubPopulation::Item const &SubPopulation::operator[](size_t idx) const
 {
     return items[idx];
 }
 
-std::vector<SubPopulation::Item>::const_iterator SubPopulation::cbegin() const
-{
-    return items.cbegin();
-}
+const_iter SubPopulation::cbegin() const { return items.cbegin(); }
 
-std::vector<SubPopulation::Item>::const_iterator SubPopulation::cend() const
-{
-    return items.cend();
-}
+const_iter SubPopulation::cend() const { return items.cend(); }
 
-void SubPopulation::remove(
-    std::vector<SubPopulation::Item>::iterator const &iterator,
-    CostEvaluator const &costEvaluator)
+void SubPopulation::remove(iter const &iterator)
 {
-    for (auto &[params, individual, fitness, proximity] : items)
-        // Remove individual from other proximities.
+    for (auto &[params, solution, fitness, proximity] : items)
+        // Remove solution from other proximities.
         for (size_t idx = 0; idx != proximity.size(); ++idx)
-            if (proximity[idx].second == iterator->individual)
+            if (proximity[idx].second == iterator->solution)
             {
                 proximity.erase(proximity.begin() + idx);
                 break;
             }
 
-    delete iterator->individual;  // dispose of manually allocated memory
-    items.erase(iterator);        // before the item is removed.
+    delete iterator->solution;  // dispose of manually allocated memory
+    items.erase(iterator);      // before the item is removed.
 }
 
 void SubPopulation::purge(CostEvaluator const &costEvaluator)
 {
     // First we remove duplicates. This does not rely on the fitness values.
     while (size() > params.minPopSize)
     {
         // Remove duplicates from the subpopulation (if they exist)
         auto const pred = [&](auto &iterator) {
             return !iterator.proximity.empty()
-                   && *iterator.proximity[0].second == *iterator.individual;
+                   && *iterator.proximity[0].second == *iterator.solution;
         };
 
         auto const duplicate = std::find_if(items.begin(), items.end(), pred);
 
         if (duplicate == items.end())  // there are no more duplicates
             break;
 
-        remove(duplicate, costEvaluator);
+        remove(duplicate);
     }
 
     while (size() > params.minPopSize)
     {
         // Before using fitness, we must update fitness
         updateFitness(costEvaluator);
         auto const worstFitness = std::max_element(
             items.begin(), items.end(), [](auto const &a, auto const &b) {
                 return a.fitness < b.fitness;
             });
 
-        remove(worstFitness, costEvaluator);
+        remove(worstFitness);
     }
 }
 
 void SubPopulation::updateFitness(CostEvaluator const &costEvaluator)
 {
     if (items.empty())
         return;
 
     std::vector<size_t> byCost(size());
     std::iota(byCost.begin(), byCost.end(), 0);
 
     std::stable_sort(byCost.begin(), byCost.end(), [&](size_t a, size_t b) {
-        return costEvaluator.penalisedCost(*items[a].individual)
-               < costEvaluator.penalisedCost(*items[b].individual);
+        return costEvaluator.penalisedCost(*items[a].solution)
+               < costEvaluator.penalisedCost(*items[b].solution);
     });
 
     std::vector<std::pair<double, size_t>> diversity;
     for (size_t costRank = 0; costRank != size(); costRank++)
     {
         auto const dist = items[byCost[costRank]].avgDistanceClosest();
         diversity.emplace_back(-dist, costRank);  // higher is better
@@ -146,9 +141,9 @@
 {
     auto const maxSize = std::min(proximity.size(), params->nbClose);
     auto result = 0.0;
 
     for (size_t idx = 0; idx != maxSize; ++idx)
         result += proximity[idx].first;
 
-    return result / std::max(maxSize, size_t(1));
+    return result / std::max<size_t>(maxSize, 1);
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/SubPopulation.h` & `pyvrp-0.4.1/pyvrp/cpp/SubPopulation.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-#ifndef SUBPOPULATION_H
-#define SUBPOPULATION_H
+#ifndef PYVRP_SUBPOPULATION_H
+#define PYVRP_SUBPOPULATION_H
 
 #include "CostEvaluator.h"
-#include "Individual.h"
+#include "Solution.h"
 #include "diversity/diversity.h"
 
 #include <functional>
 #include <iosfwd>
 #include <stdexcept>
 #include <vector>
 
@@ -52,55 +52,54 @@
 {
     DiversityMeasure divOp;
     PopulationParams const &params;  // owned by Population, on the Python side
 
 public:
     struct Item
     {
-        using Proximity = std::vector<std::pair<double, Individual const *>>;
+        using Proximity = std::vector<std::pair<double, Solution const *>>;
 
         PopulationParams const *params;
 
         // Note that this pointer is not owned by the Item - it is merely a
         // reference to memory owned and allocated by the SubPopulation this
         // item is part of. The SubPopulation remains responsible for managing
         // that memory.
-        Individual const *individual;
+        Solution const *solution;
+
         // Fitness should be used carefully: only directly after updateFitness
         // was called. At any other moment, it will be outdated.
         double fitness;
         Proximity proximity;
 
         double avgDistanceClosest() const;
     };
 
 private:
     std::vector<Item> items;
 
     // Removes the element at the given iterator location from the items.
-    void remove(std::vector<Item>::iterator const &iterator,
-                CostEvaluator const &costEvaluator);
+    void remove(std::vector<Item>::iterator const &iterator);
 
 public:
     SubPopulation(DiversityMeasure divOp, PopulationParams const &params);
 
     ~SubPopulation();
 
-    void add(Individual const *individual, CostEvaluator const &costEvaluator);
+    void add(Solution const *solution, CostEvaluator const &costEvaluator);
 
     std::vector<Item>::const_iterator cbegin() const;
 
     std::vector<Item>::const_iterator cend() const;
 
     size_t size() const;
 
     Item const &operator[](size_t idx) const;
 
     void purge(CostEvaluator const &costEvaluator);
 
-    // Recomputes the fitness of all individuals maintained by this population.
-    // This is called whenever an individual is added to, or removed from, the
-    // population.
+    // Recomputes the fitness of all solutions maintained by this subpopulation.
+    // This is called whenever a solution is added or removed.
     void updateFitness(CostEvaluator const &costEvaluator);
 };
 
-#endif  // SUBPOPULATION_H
+#endif  // PYVRP_SUBPOPULATION_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/SubPopulation_bindings.cpp` & `pyvrp-0.4.1/pyvrp/cpp/SubPopulation_bindings.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -21,28 +21,28 @@
         .def_property_readonly("max_pop_size", &PopulationParams::maxPopSize)
         .def_readwrite("nb_elite", &PopulationParams::nbElite)
         .def_readwrite("nb_close", &PopulationParams::nbClose)
         .def_readwrite("lb_diversity", &PopulationParams::lbDiversity)
         .def_readwrite("ub_diversity", &PopulationParams::ubDiversity);
 
     py::class_<SubPopulation::Item>(m, "SubPopulationItem")
-        .def_readonly("individual",
-                      &SubPopulation::Item::individual,
+        .def_readonly("solution",
+                      &SubPopulation::Item::solution,
                       py::return_value_policy::reference_internal)
         .def_readonly("fitness", &SubPopulation::Item::fitness)
         .def("avg_distance_closest", &SubPopulation::Item::avgDistanceClosest);
 
     py::class_<SubPopulation>(m, "SubPopulation")
         .def(py::init<DiversityMeasure, PopulationParams const &>(),
              py::arg("diversity_op"),
              py::arg("params"),
              py::keep_alive<1, 3>())  // keep params alive
         .def("add",
              &SubPopulation::add,
-             py::arg("individual"),
+             py::arg("solution"),
              py::arg("cost_evaluator"))
         .def("__len__", &SubPopulation::size)
         .def(
             "__getitem__",
             [](SubPopulation const &subPop, int idx) {
                 // int so we also support negative offsets from the end.
                 idx = idx < 0 ? subPop.size() + idx : idx;
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/TimeWindowSegment.h` & `pyvrp-0.4.1/pyvrp/cpp/TimeWindowSegment.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,110 @@
-#ifndef TIMEWINDOWDATA_H
-#define TIMEWINDOWDATA_H
+#ifndef PYVRP_TIMEWINDOWSEGMENT_H
+#define PYVRP_TIMEWINDOWSEGMENT_H
 
 #include "Matrix.h"
+#include "Measure.h"
 
 class TimeWindowSegment
 {
     using TWS = TimeWindowSegment;
 
-    int idxFirst = 0;  // Index of the first client in the segment
-    int idxLast = 0;   // Index of the last client in the segment
-    int duration = 0;  // Total duration, incl. waiting and servicing
-    int timeWarp = 0;  // Cumulative time warp
-    int twEarly = 0;   // Earliest visit moment of first client
-    int twLate = 0;    // Latest visit moment of last client
+    int idxFirst = 0;          // Index of the first client in the segment
+    int idxLast = 0;           // Index of the last client in the segment
+    Duration duration = 0;     // Total duration, incl. waiting and servicing
+    Duration timeWarp = 0;     // Cumulative time warp
+    Duration twEarly = 0;      // Earliest visit moment of first client
+    Duration twLate = 0;       // Latest visit moment of first client
+    Duration releaseTime = 0;  // Earliest allowed moment to leave the depot
 
-    [[nodiscard]] inline TWS merge(Matrix<int> const &durationMatrix,
+    [[nodiscard]] inline TWS merge(Matrix<Duration> const &durationMatrix,
                                    TWS const &other) const;
 
 public:
     template <typename... Args>
-    [[nodiscard]] inline static TWS merge(Matrix<int> const &durationMatrix,
-                                          TWS const &first,
-                                          TWS const &second,
-                                          Args... args);
+    [[nodiscard]] inline static TWS
+    merge(Matrix<Duration> const &durationMatrix,
+          TWS const &first,
+          TWS const &second,
+          Args... args);
 
     /**
      * Total time warp, that is, the time warp along the the segment, and
      * potential time warp due to too late a release time.
      */
-    [[nodiscard]] inline int totalTimeWarp() const;
+    [[nodiscard]] inline Duration totalTimeWarp() const;
 
-    TimeWindowSegment() = default;
+    TimeWindowSegment() = default;  // TODO at least require client index
 
     inline TimeWindowSegment(int idxFirst,
                              int idxLast,
-                             int duration,
-                             int timeWarp,
-                             int twEarly,
-                             int twLate);
+                             Duration duration,
+                             Duration timeWarp,
+                             Duration twEarly,
+                             Duration twLate,
+                             Duration releaseTime);
 };
 
-TimeWindowSegment TimeWindowSegment::merge(Matrix<int> const &durationMatrix,
-                                           TimeWindowSegment const &other) const
+TimeWindowSegment TimeWindowSegment::merge(
+    [[maybe_unused]] Matrix<Duration> const &durationMatrix,
+    [[maybe_unused]] TimeWindowSegment const &other) const
 {
-#ifdef VRP_NO_TIME_WINDOWS
+#ifdef PYVRP_NO_TIME_WINDOWS
     return {};
 #else
     auto const arcDuration = durationMatrix(idxLast, other.idxFirst);
-    auto const delta = duration - timeWarp + arcDuration;
-    auto const deltaWaitTime = std::max(other.twEarly - delta - twLate, 0);
-    auto const deltaTimeWarp = std::max(twEarly + delta - other.twLate, 0);
+    auto const diff = duration - timeWarp + arcDuration;
+    auto const diffWait = std::max<Duration>(other.twEarly - diff - twLate, 0);
+    auto const diffTw = std::max<Duration>(twEarly + diff - other.twLate, 0);
 
     return {idxFirst,
             other.idxLast,
-            duration + other.duration + arcDuration + deltaWaitTime,
-            timeWarp + other.timeWarp + deltaTimeWarp,
-            std::max(other.twEarly - delta, twEarly) - deltaWaitTime,
-            std::min(other.twLate - delta, twLate) + deltaTimeWarp};
+            duration + other.duration + arcDuration + diffWait,
+            timeWarp + other.timeWarp + diffTw,
+            std::max(other.twEarly - diff, twEarly) - diffWait,
+            std::min(other.twLate - diff, twLate) + diffTw,
+            std::max(releaseTime, other.releaseTime)};
 #endif
 }
 
 template <typename... Args>
-TimeWindowSegment TimeWindowSegment::merge(Matrix<int> const &durationMatrix,
-                                           TimeWindowSegment const &first,
-                                           TimeWindowSegment const &second,
-                                           Args... args)
+TimeWindowSegment TimeWindowSegment::merge(
+    [[maybe_unused]] Matrix<Duration> const &durationMatrix,
+    [[maybe_unused]] TimeWindowSegment const &first,
+    [[maybe_unused]] TimeWindowSegment const &second,
+    [[maybe_unused]] Args... args)
 {
-#ifdef VRP_NO_TIME_WINDOWS
+#ifdef PYVRP_NO_TIME_WINDOWS
     return {};
 #else
     auto const res = first.merge(durationMatrix, second);
 
     if constexpr (sizeof...(args) == 0)
         return res;
     else
         return merge(durationMatrix, res, args...);
 #endif
 }
 
-int TimeWindowSegment::totalTimeWarp() const { return timeWarp; }
+Duration TimeWindowSegment::totalTimeWarp() const
+{
+    return timeWarp + std::max<Duration>(releaseTime - twLate, 0);
+}
 
 TimeWindowSegment::TimeWindowSegment(int idxFirst,
                                      int idxLast,
-                                     int duration,
-                                     int timeWarp,
-                                     int twEarly,
-                                     int twLate)
+                                     Duration duration,
+                                     Duration timeWarp,
+                                     Duration twEarly,
+                                     Duration twLate,
+                                     Duration releaseTime)
     : idxFirst(idxFirst),
       idxLast(idxLast),
       duration(duration),
       timeWarp(timeWarp),
       twEarly(twEarly),
-      twLate(twLate)
+      twLate(twLate),
+      releaseTime(releaseTime)
 {
 }
 
-#endif  // TIMEWINDOWDATA_H
+#endif  // PYVRP_TIMEWINDOWSEGMENT_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/XorShift128.cpp` & `pyvrp-0.4.1/pyvrp/cpp/XorShift128.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/cpp/XorShift128.h` & `pyvrp-0.4.1/pyvrp/cpp/XorShift128.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-#ifndef XORSHIFT128_H
-#define XORSHIFT128_H
+#ifndef PYVRP_XORSHIFT128_H
+#define PYVRP_XORSHIFT128_H
 
-#include <climits>
 #include <cstddef>
 #include <cstdint>
+#include <limits>
 #include <type_traits>
 
 /**
  * This class implements a XOR-shift pseudo-random number generator. It
  * generates the next number of a sequence by repeatedly taking the 'exclusive
  * or' (the ^ operator) of a number with a bit-shifted version of itself. See
  * also here for more details: https://en.wikipedia.org/wiki/Xorshift.
@@ -56,24 +56,30 @@
      *
      * @param high Upper bound on the integer to generate.
      * @return A pseudo-random integer.
      */
     template <typename T> result_type randint(T high);
 };
 
-constexpr size_t XorShift128::min() { return 0; }
+constexpr size_t XorShift128::min()
+{
+    return std::numeric_limits<result_type>::min();
+}
 
-constexpr size_t XorShift128::max() { return UINT32_MAX; }
+constexpr size_t XorShift128::max()
+{
+    return std::numeric_limits<result_type>::max();
+}
 
 template <typename T> T XorShift128::rand()
 {
     static_assert(std::is_floating_point<T>::value);
     return operator()() / static_cast<T>(max());
 }
 
 template <typename T> XorShift128::result_type XorShift128::randint(T high)
 {
     static_assert(std::is_integral<T>::value);
     return operator()() % high;
 }
 
-#endif  // XORSHIFT128_H
+#endif  // PYVRP_XORSHIFT128_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/crossover/crossover.h` & `pyvrp-0.4.1/pyvrp/cpp/crossover/crossover.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-#ifndef CROSSOVER_H
-#define CROSSOVER_H
+#ifndef PYVRP_CROSSOVER_H
+#define PYVRP_CROSSOVER_H
 
 #include "CostEvaluator.h"
-#include "Individual.h"
 #include "ProblemData.h"
+#include "Solution.h"
 #include "XorShift128.h"
 
 #include <functional>
 #include <vector>
 
 namespace crossover
 {
 /**
- * Greedily inserts the unplanned clients into non-empty routes.
+ * Greedily inserts each unplanned client into the route that's nearest to the
+ * client.
  */
 void greedyRepair(std::vector<std::vector<int>> &routes,
                   std::vector<int> const &unplanned,
-                  ProblemData const &data);
+                  ProblemData const &data,
+                  CostEvaluator const &costEvaluator);
 }  // namespace crossover
 
 /**
  * Performs two SREX crossovers of the given parents. SREX is a method that
  * selects a set of routes for each parent and replaces the selected routes of
  * the first parent with those of the second parent. The routes are selected by
  * minimizing the overlap between the two sets of routes. This is achieved
  * through a heuristic that iteratively shifts adjacent routes until no further
  * improvement in minimizing the overlap is observed. Then, two offspring are
  * generated by replacing the selected routes in two distinct ways, and the
  * offspring with the lowest cost is returned.
  *
- * @param parents          The parent individuals.
+ * @param parents          The parent solutions.
  * @param data             The problem data.
  * @param costEvaluator    The cost evaluator.
- * @param startIndices     Start indices of routes in parent individuals.
+ * @param startIndices     Start indices of routes in parent solutions.
  * @param numMovedRoutes   Number of routes to move.
  * @return A new offspring.
  *
  * <br />
  * Yuichi Nagata and Shigenobu Kobayashi. "A memetic algorithm for
  * the pickup and delivery problem with time windows using selective route
  * exchange crossover". In: International Conference on Parallel Problem Solving
  * from Nature. Springer. 2010, pp. 536–545.
  */
-Individual selectiveRouteExchange(
-    std::pair<Individual const *, Individual const *> const &parents,
+Solution selectiveRouteExchange(
+    std::pair<Solution const *, Solution const *> const &parents,
     ProblemData const &data,
     CostEvaluator const &costEvaluator,
     std::pair<size_t, size_t> const startIndices,
     size_t const numMovedRoutes);
 
-#endif  // CROSSOVER_H
+#endif  // PYVRP_CROSSOVER_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/crossover/selective_route_exchange.cpp` & `pyvrp-0.4.1/pyvrp/cpp/crossover/selective_route_exchange.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,47 @@
 #include "crossover.h"
 
+#include <cassert>
 #include <cmath>
 #include <unordered_set>
 
 using Client = int;
 using Clients = std::vector<Client>;
 using ClientSet = std::unordered_set<Client>;
-using Route = Individual::Route;
+using Route = Solution::Route;
 using Routes = std::vector<Route>;
 
 namespace
 {
+// Angle of the given route w.r.t. the centroid of all client locations.
 double routeAngle(ProblemData const &data, Route const &route)
 {
-    // Computes the route angle center. Assumes that the route is non-empty.
-    int cumulatedX = 0;
-    int cumulatedY = 0;
-
-    for (int node : route)
-    {
-        cumulatedX += data.client(node).x;
-        cumulatedY += data.client(node).y;
-    }
-
     // This computes a pseudo-angle that sorts roughly equivalently to the atan2
     // angle, but is much faster to compute. See the following post for details:
     // https://stackoverflow.com/a/16561333/4316405.
-    auto const routeSize = static_cast<double>(route.size());
-    auto const dy = cumulatedY / routeSize - data.depot().y;
-    auto const dx = cumulatedX / routeSize - data.depot().x;
+    auto const [dataX, dataY] = data.centroid();
+    auto const [routeX, routeY] = route.centroid();
+    auto const dx = routeX - dataX;
+    auto const dy = routeY - dataY;
     return std::copysign(1. - dx / (std::fabs(dx) + std::fabs(dy)), dy);
 }
 
-Routes getNonEmptyRoutesByAscendingAngle(ProblemData const &data, Routes routes)
+Routes sortByAscAngle(ProblemData const &data, Routes routes)
 {
     auto cmp = [&data](Route a, Route b) {
-        return (a.empty() || b.empty())
-                   ? !a.empty() && b.empty()
-                   : routeAngle(data, a) < routeAngle(data, b);
+        return routeAngle(data, a) < routeAngle(data, b);
     };
 
     std::sort(routes.begin(), routes.end(), cmp);
-
-    size_t empty = 0;
-    for (; empty != routes.size(); ++empty)
-        if (routes[empty].empty())
-            break;
-
-    routes.resize(empty);
     return routes;
 }
 }  // namespace
 
-Individual selectiveRouteExchange(
-    std::pair<Individual const *, Individual const *> const &parents,
+Solution selectiveRouteExchange(
+    std::pair<Solution const *, Solution const *> const &parents,
     ProblemData const &data,
     CostEvaluator const &costEvaluator,
     std::pair<size_t, size_t> const startIndices,
     size_t const numMovedRoutes)
 {
     // We create two candidate offsprings, both based on parent A:
     // Let A and B denote the set of customers selected from parents A and B
@@ -74,46 +58,46 @@
     // Offspring 2:
     // A^B and Ac, remainder A\B unplanned
     // (note A^B v Ac v A\B = (A^B v A\B) v Ac = A v Ac = all)
 
     auto startA = startIndices.first;
     auto startB = startIndices.second;
 
-    // Sort routes according to center angle for both parents
-    auto const routesA
-        = getNonEmptyRoutesByAscendingAngle(data, parents.first->getRoutes());
-    auto const routesB
-        = getNonEmptyRoutesByAscendingAngle(data, parents.second->getRoutes());
-
-    size_t nRoutesA = routesA.size();
-    size_t nRoutesB = routesB.size();
+    size_t nRoutesA = parents.first->numRoutes();
+    size_t nRoutesB = parents.second->numRoutes();
 
     if (startA >= nRoutesA)
         throw std::invalid_argument("Expected startA < nRoutesA.");
 
     if (startB >= nRoutesB)
         throw std::invalid_argument("Expected startB < nRoutesB.");
 
     if (numMovedRoutes < 1 || numMovedRoutes > std::min(nRoutesA, nRoutesB))
-        throw std::invalid_argument(
-            "Expected numMovedRoutes in [1, min(nRoutesA, nRoutesB)]");
+    {
+        auto msg = "Expected numMovedRoutes in [1, min(nRoutesA, nRoutesB)]";
+        throw std::invalid_argument(msg);
+    }
+
+    // Sort parents' routes by (ascending) polar angle.
+    auto const routesA = sortByAscAngle(data, parents.first->getRoutes());
+    auto const routesB = sortByAscAngle(data, parents.second->getRoutes());
 
     ClientSet selectedA;
     ClientSet selectedB;
 
     // Routes are sorted on polar angle, so selecting adjacent routes in both
     // parents should result in a large overlap when the start indices are
     // close to each other.
     for (size_t r = 0; r < numMovedRoutes; r++)
     {
-        selectedA.insert(routesA[(startA + r) % nRoutesA].begin(),
-                         routesA[(startA + r) % nRoutesA].end());
+        auto const &routeA = routesA[(startA + r) % nRoutesA];
+        selectedA.insert(routeA.begin(), routeA.end());
 
-        selectedB.insert(routesB[(startB + r) % nRoutesB].begin(),
-                         routesB[(startB + r) % nRoutesB].end());
+        auto const &routeB = routesB[(startB + r) % nRoutesB];
+        selectedB.insert(routeB.begin(), routeB.end());
     }
 
     // For the selection, we want to minimize |A\B| as these need replanning
     while (true)
     {
         // Difference for moving 'left' in parent A
         int differenceALeft = 0;
@@ -198,56 +182,70 @@
 
     // Identify differences between route sets
     ClientSet clientsInSelectedBNotA;
     for (Client c : selectedB)
         if (!selectedA.contains(c))
             clientsInSelectedBNotA.insert(c);
 
-    std::vector<std::vector<Client>> routes1(data.numVehicles());
-    std::vector<std::vector<Client>> routes2(data.numVehicles());
+    std::vector<std::vector<Client>> visits1(nRoutesA);
+    std::vector<std::vector<Client>> visits2(nRoutesA);
 
     // Replace selected routes from parent A with routes from parent B
     for (size_t r = 0; r < numMovedRoutes; r++)
     {
         size_t indexA = (startA + r) % nRoutesA;
         size_t indexB = (startB + r) % nRoutesB;
 
         for (Client c : routesB[indexB])
         {
-            routes1[indexA].push_back(c);  // c in B
+            visits1[indexA].push_back(c);  // c in B
 
             if (!clientsInSelectedBNotA.contains(c))
-                routes2[indexA].push_back(c);  // c in A^B
+                visits2[indexA].push_back(c);  // c in A^B
         }
     }
 
     // Move routes from parent A that are kept
     for (size_t r = numMovedRoutes; r < nRoutesA; r++)
     {
         size_t indexA = (startA + r) % nRoutesA;
 
         for (Client c : routesA[indexA])
         {
             if (!clientsInSelectedBNotA.contains(c))
-                routes1[indexA].push_back(c);  // c in Ac\B
+                visits1[indexA].push_back(c);  // c in Ac\B
 
-            routes2[indexA].push_back(c);  // c in Ac
+            visits2[indexA].push_back(c);  // c in Ac
         }
     }
 
     // Insert unplanned clients (those that were in the removed routes of A, but
     // not the inserted routes of B).
     Clients unplanned;
     for (Client c : selectedA)
         if (!selectedB.contains(c))
             unplanned.push_back(c);
 
-    crossover::greedyRepair(routes1, unplanned, data);
-    crossover::greedyRepair(routes2, unplanned, data);
+    crossover::greedyRepair(visits1, unplanned, data, costEvaluator);
+    crossover::greedyRepair(visits2, unplanned, data, costEvaluator);
+
+    // Assign correct types to routes (from parents) and filter empty
+    std::vector<Solution::Route> routes1;
+    routes1.reserve(nRoutesA);
+    std::vector<Solution::Route> routes2;
+    routes2.reserve(nRoutesA);
+
+    for (size_t r = 0; r < nRoutesA; r++)
+    {
+        if (!visits1[r].empty())
+            routes1.emplace_back(data, visits1[r], routesA[r].vehicleType());
+        if (!visits2[r].empty())
+            routes2.emplace_back(data, visits2[r], routesA[r].vehicleType());
+    }
 
-    Individual indiv1{data, routes1};
-    Individual indiv2{data, routes2};
+    Solution sol1{data, routes1};
+    Solution sol2{data, routes2};
 
-    auto const cost1 = costEvaluator.penalisedCost(indiv1);
-    auto const cost2 = costEvaluator.penalisedCost(indiv2);
-    return cost1 < cost2 ? indiv1 : indiv2;
+    auto const cost1 = costEvaluator.penalisedCost(sol1);
+    auto const cost2 = costEvaluator.penalisedCost(sol2);
+    return cost1 < cost2 ? sol1 : sol2;
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/diversity/broken_pairs_distance.cpp` & `pyvrp-0.4.1/pyvrp/cpp/diversity/broken_pairs_distance.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "diversity.h"
 
-double brokenPairsDistance(Individual const &first, Individual const &second)
+double brokenPairsDistance(Solution const &first, Solution const &second)
 {
     auto const &fNeighbours = first.getNeighbours();
     auto const &sNeighbours = second.getNeighbours();
 
     // The neighbours vector contains the depot, so its size is always at least
     // one. Thus numClients >= 0.
     size_t const numClients = fNeighbours.size() - 1;
@@ -19,9 +19,9 @@
         // broken if it is not in the second solution.
         numBrokenPairs += fSucc != sSucc;
         numBrokenPairs += fPred != sPred;
     }
 
     // numBrokenPairs is at most 2n since we can count at most two broken edges
     // for each client. Here, we normalise the distance to [0, 1].
-    return numBrokenPairs / (2. * std::max(numClients, size_t(1)));
+    return numBrokenPairs / (2. * std::max<size_t>(numClients, 1));
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/CircleSector.h` & `pyvrp-0.4.1/pyvrp/cpp/search/CircleSector.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef CIRCLESECTOR_H
-#define CIRCLESECTOR_H
+#ifndef PYVRP_CIRCLESECTOR_H
+#define PYVRP_CIRCLESECTOR_H
 
 // Data structure to represent circle sectors
 // Angles are measured in [0,65535] instead of [0,359], in such a way that
 // modulo operations are much faster (since 2^16 = 65536) Credit to Fabian
 // Giesen at "https://web.archive.org/web/20200912191950" and
 // "https://fgiesen.wordpress.com/2015/09/24/intervals-in-modular-arithmetic/"
 // for useful implementation tips regarding interval overlaps in modular
@@ -75,8 +75,8 @@
                 end = point;
             else
                 start = point;
         }
     }
 };
 
-#endif
+#endif  // PYVRP_CIRCLESECTOR_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/Exchange.h` & `pyvrp-0.4.1/pyvrp/cpp/search/Exchange.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef EXCHANGE_H
-#define EXCHANGE_H
+#ifndef PYVRP_EXCHANGE_H
+#define PYVRP_EXCHANGE_H
 
 #include "LocalSearchOperator.h"
 #include "TimeWindowSegment.h"
 
 #include <cassert>
 
 using TWS = TimeWindowSegment;
@@ -25,24 +25,25 @@
     // Tests if the segments of U and V overlap in the same route
     inline bool overlap(Node *U, Node *V) const;
 
     // Tests if the segments of U and V are adjacent in the same route
     inline bool adjacent(Node *U, Node *V) const;
 
     // Special case that's applied when M == 0
-    int evalRelocateMove(Node *U,
-                         Node *V,
-                         CostEvaluator const &costEvaluator) const;
+    Cost evalRelocateMove(Node *U,
+                          Node *V,
+                          CostEvaluator const &costEvaluator) const;
 
     // Applied when M != 0
-    int
+    Cost
     evalSwapMove(Node *U, Node *V, CostEvaluator const &costEvaluator) const;
 
 public:
-    int evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator) override;
+    Cost
+    evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator) override;
 
     void apply(Node *U, Node *V) const override;
 };
 
 template <size_t N, size_t M>
 bool Exchange<N, M>::containsDepot(Node *node, size_t segLength) const
 {
@@ -54,52 +55,50 @@
     // also moving the node *at* position) is larger than size().
     return node->position + segLength - 1 > node->route->size();
 }
 
 template <size_t N, size_t M>
 bool Exchange<N, M>::overlap(Node *U, Node *V) const
 {
-    // clang-format off
     return U->route == V->route
-        // We need max(M, 1) here because when V is the depot and M == 0, this
-        // would turn negative and wrap around to a large number.
-        && U->position <= V->position + std::max(M, size_t(1)) - 1
-        && V->position <= U->position + N - 1;
-    // clang-format on
+           // We need max(M, 1) here because when V is the depot and M == 0,
+           // this would turn negative and wrap around to a large number.
+           && U->position <= V->position + std::max<size_t>(M, 1) - 1
+           && V->position <= U->position + N - 1;
 }
 
 template <size_t N, size_t M>
 bool Exchange<N, M>::adjacent(Node *U, Node *V) const
 {
     if (U->route != V->route)
         return false;
 
     return U->position + N == V->position || V->position + M == U->position;
 }
 
 template <size_t N, size_t M>
-int Exchange<N, M>::evalRelocateMove(Node *U,
-                                     Node *V,
-                                     CostEvaluator const &costEvaluator) const
+Cost Exchange<N, M>::evalRelocateMove(Node *U,
+                                      Node *V,
+                                      CostEvaluator const &costEvaluator) const
 {
     auto const posU = U->position;
     auto const posV = V->position;
 
     assert(posU > 0);
     auto *endU = N == 1 ? U : (*U->route)[posU + N - 1];
 
-    int const current = U->route->distBetween(posU - 1, posU + N)
-                        + data.dist(V->client, n(V)->client);
+    Distance const current = U->route->distBetween(posU - 1, posU + N)
+                             + data.dist(V->client, n(V)->client);
 
-    int const proposed = data.dist(V->client, U->client)
-                         + U->route->distBetween(posU, posU + N - 1)
-                         + data.dist(endU->client, n(V)->client)
-                         + data.dist(p(U)->client, n(endU)->client);
+    Distance const proposed = data.dist(V->client, U->client)
+                              + U->route->distBetween(posU, posU + N - 1)
+                              + data.dist(endU->client, n(V)->client)
+                              + data.dist(p(U)->client, n(endU)->client);
 
-    int deltaCost = proposed - current;
+    Cost deltaCost = static_cast<Cost>(proposed - current);
 
     if (U->route != V->route)
     {
         if (U->route->isFeasible() && deltaCost >= 0)
             return deltaCost;
 
         auto uTWS = TWS::merge(
@@ -107,25 +106,25 @@
 
         deltaCost += costEvaluator.twPenalty(uTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
         auto const loadDiff = U->route->loadBetween(posU, posU + N - 1);
 
         deltaCost += costEvaluator.loadPenalty(U->route->load() - loadDiff,
-                                               data.vehicleCapacity());
+                                               U->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(U->route->load(),
-                                               data.vehicleCapacity());
+                                               U->route->capacity());
 
         if (deltaCost >= 0)    // if delta cost of just U's route is not enough
             return deltaCost;  // even without V, the move will never be good.
 
         deltaCost += costEvaluator.loadPenalty(V->route->load() + loadDiff,
-                                               data.vehicleCapacity());
+                                               V->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(V->route->load(),
-                                               data.vehicleCapacity());
+                                               V->route->capacity());
 
         auto vTWS = TWS::merge(data.durationMatrix(),
                                V->twBefore,
                                U->route->twBetween(posU, posU + N - 1),
                                n(V)->twAfter);
 
         deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
@@ -162,41 +161,41 @@
         deltaCost -= costEvaluator.twPenalty(route->timeWarp());
     }
 
     return deltaCost;
 }
 
 template <size_t N, size_t M>
-int Exchange<N, M>::evalSwapMove(Node *U,
-                                 Node *V,
-                                 CostEvaluator const &costEvaluator) const
+Cost Exchange<N, M>::evalSwapMove(Node *U,
+                                  Node *V,
+                                  CostEvaluator const &costEvaluator) const
 {
     auto const posU = U->position;
     auto const posV = V->position;
 
     assert(posU > 0 && posV > 0);
     auto *endU = N == 1 ? U : (*U->route)[posU + N - 1];
     auto *endV = M == 1 ? V : (*V->route)[posV + M - 1];
 
     assert(U->route && V->route);
 
-    int const current = U->route->distBetween(posU - 1, posU + N)
-                        + V->route->distBetween(posV - 1, posV + M);
+    Distance const current = U->route->distBetween(posU - 1, posU + N)
+                             + V->route->distBetween(posV - 1, posV + M);
 
-    int const proposed
+    Distance const proposed
         //   p(U) -> V -> ... -> endV -> n(endU)
         // + p(V) -> U -> ... -> endU -> n(endV)
         = data.dist(p(U)->client, V->client)
           + V->route->distBetween(posV, posV + M - 1)
           + data.dist(endV->client, n(endU)->client)
           + data.dist(p(V)->client, U->client)
           + U->route->distBetween(posU, posU + N - 1)
           + data.dist(endU->client, n(endV)->client);
 
-    int deltaCost = proposed - current;
+    Cost deltaCost = static_cast<Cost>(proposed - current);
 
     if (U->route != V->route)
     {
         if (U->route->isFeasible() && V->route->isFeasible() && deltaCost >= 0)
             return deltaCost;
 
         auto uTWS = TWS::merge(data.durationMatrix(),
@@ -208,30 +207,30 @@
         deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
         auto const loadU = U->route->loadBetween(posU, posU + N - 1);
         auto const loadV = V->route->loadBetween(posV, posV + M - 1);
         auto const loadDiff = loadU - loadV;
 
         deltaCost += costEvaluator.loadPenalty(U->route->load() - loadDiff,
-                                               data.vehicleCapacity());
+                                               U->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(U->route->load(),
-                                               data.vehicleCapacity());
+                                               U->route->capacity());
 
         auto vTWS = TWS::merge(data.durationMatrix(),
                                p(V)->twBefore,
                                U->route->twBetween(posU, posU + N - 1),
                                n(endV)->twAfter);
 
         deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
 
         deltaCost += costEvaluator.loadPenalty(V->route->load() + loadDiff,
-                                               data.vehicleCapacity());
+                                               V->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(V->route->load(),
-                                               data.vehicleCapacity());
+                                               V->route->capacity());
     }
     else  // within same route
     {
         auto const *route = U->route;
 
         if (!route->hasTimeWarp() && deltaCost >= 0)
             return deltaCost;
@@ -262,17 +261,17 @@
         deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
     }
 
     return deltaCost;
 }
 
 template <size_t N, size_t M>
-int Exchange<N, M>::evaluate(Node *U,
-                             Node *V,
-                             CostEvaluator const &costEvaluator)
+Cost Exchange<N, M>::evaluate(Node *U,
+                              Node *V,
+                              CostEvaluator const &costEvaluator)
 {
     if (containsDepot(U, N) || overlap(U, V))
         return 0;
 
     if constexpr (M > 0)
         if (containsDepot(V, M))
             return 0;
@@ -307,16 +306,16 @@
     {
         auto *prev = p(uToInsert);
         uToInsert->insertAfter(insertUAfter);
         uToInsert = prev;
     }
 
     // ...and swap the overlapping nodes!
-    for (size_t count = 0; count != std::min(N, M); ++count)
+    for (size_t count = 0; count != M; ++count)
     {
         U->swapWith(V);
         U = n(U);
         V = n(V);
     }
 }
 
-#endif  // EXCHANGE_H
+#endif  // PYVRP_EXCHANGE_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/Exchange_bindings.cpp` & `pyvrp-0.4.1/pyvrp/cpp/search/Exchange_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch.cpp` & `pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #include "LocalSearch.h"
+#include "Measure.h"
 #include "TimeWindowSegment.h"
 
 #include <algorithm>
 #include <cassert>
 #include <numeric>
 #include <set>
 #include <stdexcept>
 #include <vector>
 
 using TWS = TimeWindowSegment;
 
-Individual LocalSearch::search(Individual &individual,
-                               CostEvaluator const &costEvaluator)
+Solution LocalSearch::search(Solution &solution,
+                             CostEvaluator const &costEvaluator)
 {
-    loadIndividual(individual);
-
-    // Shuffling the order beforehand adds diversity to the search
-    std::shuffle(orderNodes.begin(), orderNodes.end(), rng);
-    std::shuffle(nodeOps.begin(), nodeOps.end(), rng);
+    loadSolution(solution);
 
     if (nodeOps.empty())
         throw std::runtime_error("No known node operators.");
 
     // Caches the last time nodes were tested for modification (uses numMoves to
     // track this). The lastModified field, in contrast, track when a route was
     // last *actually* modified.
@@ -67,43 +64,47 @@
                     if (p(V)->isDepot() && applyNodeOps(U, p(V), costEvaluator))
                         continue;
                 }
             }
 
             if (step > 0)  // empty moves are not tested initially to avoid
             {              // using too many routes.
-                auto pred = [](auto const &route) { return route.empty(); };
-                auto empty = std::find_if(routes.begin(), routes.end(), pred);
+                auto begin = routes.begin();
+                for (size_t t = 0; t != data.numVehicleTypes(); t++)
+                {
+                    // Check move involving empty route of each vehicle type
+                    // (if such a route exists).
+                    auto const end = begin + data.vehicleType(t).numAvailable;
+                    auto pred = [](auto const &route) { return route.empty(); };
+                    auto empty = std::find_if(begin, end, pred);
+                    begin = end;
 
-                if (empty == routes.end())
-                    continue;
+                    if (empty == end)
+                        continue;
 
-                if (U->route)  // try inserting U into the empty route.
-                    applyNodeOps(U, empty->depot, costEvaluator);
-                else  // U is not in the solution, so again try inserting.
-                    maybeInsert(U, empty->depot, costEvaluator);
+                    if (U->route)  // try inserting U into the empty route.
+                        applyNodeOps(U, empty->depot, costEvaluator);
+                    else  // U is not in the solution, so again try inserting.
+                        maybeInsert(U, empty->depot, costEvaluator);
+                }
             }
         }
     }
 
-    return exportIndividual();
+    return exportSolution();
 }
 
-Individual LocalSearch::intensify(Individual &individual,
-                                  CostEvaluator const &costEvaluator,
-                                  int overlapToleranceDegrees)
+Solution LocalSearch::intensify(Solution &solution,
+                                CostEvaluator const &costEvaluator,
+                                int overlapToleranceDegrees)
 {
-    loadIndividual(individual);
+    loadSolution(solution);
 
     auto const overlapTolerance = overlapToleranceDegrees * 65536;
 
-    // Shuffling the order beforehand adds diversity to the search
-    std::shuffle(orderRoutes.begin(), orderRoutes.end(), rng);
-    std::shuffle(routeOps.begin(), routeOps.end(), rng);
-
     if (routeOps.empty())
         throw std::runtime_error("No known route operators.");
 
     std::vector<int> lastTestedRoutes(data.numVehicles(), -1);
     lastModified = std::vector<int>(data.numVehicles(), 0);
 
     searchCompleted = false;
@@ -121,15 +122,15 @@
                 continue;
 
             auto const lastTested = lastTestedRoutes[U.idx];
             lastTestedRoutes[U.idx] = numMoves;
 
             // Shuffling in this loop should not matter much as we are
             // already randomizing the routes U.
-            for (int rV = 0; rV != U.idx; ++rV)
+            for (size_t rV = 0; rV != U.idx; ++rV)
             {
                 auto &V = routes[rV];
 
                 if (V.empty() || !U.overlapsWith(V, overlapTolerance))
                     continue;
 
                 auto const lastModifiedRoute
@@ -138,15 +139,24 @@
                 if (lastModifiedRoute > lastTested
                     && applyRouteOps(&U, &V, costEvaluator))
                     continue;
             }
         }
     }
 
-    return exportIndividual();
+    return exportSolution();
+}
+
+void LocalSearch::shuffle(XorShift128 &rng)
+{
+    std::shuffle(orderNodes.begin(), orderNodes.end(), rng);
+    std::shuffle(nodeOps.begin(), nodeOps.end(), rng);
+
+    std::shuffle(orderRoutes.begin(), orderRoutes.end(), rng);
+    std::shuffle(routeOps.begin(), routeOps.end(), rng);
 }
 
 bool LocalSearch::applyNodeOps(Node *U,
                                Node *V,
                                CostEvaluator const &costEvaluator)
 {
     for (auto *nodeOp : nodeOps)
@@ -188,31 +198,32 @@
 
 void LocalSearch::maybeInsert(Node *U,
                               Node *V,
                               CostEvaluator const &costEvaluator)
 {
     assert(!U->route && V->route);
 
-    auto const &uClient = data.client(U->client);
-
-    int const current = data.dist(V->client, n(V)->client);
-    int const proposed = data.dist(V->client, U->client)
-                         + data.dist(U->client, n(V)->client) - uClient.prize;
+    Distance const deltaDist = data.dist(V->client, U->client)
+                               + data.dist(U->client, n(V)->client)
+                               - data.dist(V->client, n(V)->client);
 
-    int deltaCost = proposed - current;
+    auto const &uClient = data.client(U->client);
+    Cost deltaCost = static_cast<Cost>(deltaDist) - uClient.prize;
 
     deltaCost += costEvaluator.loadPenalty(V->route->load() + uClient.demand,
-                                           data.vehicleCapacity());
+                                           V->route->capacity());
     deltaCost
-        -= costEvaluator.loadPenalty(V->route->load(), data.vehicleCapacity());
+        -= costEvaluator.loadPenalty(V->route->load(), V->route->capacity());
 
-    if (deltaCost >= V->route->timeWarp())  // adding U will likely not lower
-        return;                             // time warp, so we can stop here.
+    // If this is true, adding U cannot decrease time warp in V's route enough
+    // to offset the deltaCost.
+    if (deltaCost >= costEvaluator.twPenalty(V->route->timeWarp()))
+        return;
 
-    auto vTWS
+    auto const vTWS
         = TWS::merge(data.durationMatrix(), V->twBefore, U->tw, n(V)->twAfter);
 
     deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
     deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
 
     if (deltaCost < 0)
     {
@@ -221,27 +232,25 @@
     }
 }
 
 void LocalSearch::maybeRemove(Node *U, CostEvaluator const &costEvaluator)
 {
     assert(U->route);
 
-    auto const &uClient = data.client(U->client);
-
-    int const current = data.dist(p(U)->client, U->client)
-                        + data.dist(U->client, n(U)->client) - uClient.prize;
-
-    int const proposed = data.dist(p(U)->client, n(U)->client);
+    Distance const deltaDist = data.dist(p(U)->client, n(U)->client)
+                               - data.dist(p(U)->client, U->client)
+                               - data.dist(U->client, n(U)->client);
 
-    int deltaCost = proposed - current;
+    auto const &uClient = data.client(U->client);
+    Cost deltaCost = static_cast<Cost>(deltaDist) + uClient.prize;
 
     deltaCost += costEvaluator.loadPenalty(U->route->load() - uClient.demand,
-                                           data.vehicleCapacity());
+                                           U->route->capacity());
     deltaCost
-        -= costEvaluator.loadPenalty(U->route->load(), data.vehicleCapacity());
+        -= costEvaluator.loadPenalty(U->route->load(), U->route->capacity());
 
     auto uTWS
         = TWS::merge(data.durationMatrix(), p(U)->twBefore, n(U)->twAfter);
 
     deltaCost += costEvaluator.twPenalty(uTWS.totalTimeWarp());
     deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
@@ -264,30 +273,30 @@
     if (U != V)
     {
         V->update();
         lastModified[V->idx] = numMoves;
     }
 }
 
-void LocalSearch::loadIndividual(Individual const &individual)
+void LocalSearch::loadSolution(Solution const &solution)
 {
     for (size_t client = 0; client <= data.numClients(); client++)
     {
         clients[client].tw = {static_cast<int>(client),  // TODO cast
                               static_cast<int>(client),  // TODO cast
                               data.client(client).serviceDuration,
                               0,
                               data.client(client).twEarly,
-                              data.client(client).twLate};
+                              data.client(client).twLate,
+                              data.client(client).releaseTime};
 
         clients[client].route = nullptr;  // nullptr implies "not in solution"
     }
 
-    auto const &routesIndiv = individual.getRoutes();
-
+    // First empty all routes
     for (size_t r = 0; r != data.numVehicles(); r++)
     {
         Node *startDepot = &startDepots[r];
         Node *endDepot = &endDepots[r];
 
         startDepot->prev = endDepot;
         startDepot->next = endDepot;
@@ -296,63 +305,86 @@
         endDepot->next = startDepot;
 
         startDepot->tw = clients[0].tw;
         startDepot->twBefore = clients[0].tw;
 
         endDepot->tw = clients[0].tw;
         endDepot->twAfter = clients[0].tw;
+    }
 
-        Route *route = &routes[r];
+    // Determine offsets for vehicle types.
+    std::vector<size_t> vehicleOffset(data.numVehicleTypes(), 0);
+    for (size_t vehType = 1; vehType < data.numVehicleTypes(); vehType++)
+    {
+        auto const available = data.vehicleType(vehType).numAvailable;
+        vehicleOffset[vehType] = vehicleOffset[vehType - 1] + available;
+    }
 
-        if (!routesIndiv[r].empty())
-        {
-            Node *client = &clients[routesIndiv[r][0]];
-            client->route = route;
+    // Load routes from solution.
+    for (auto const &solRoute : solution.getRoutes())
+    {
+        // Determine index of next route of this type to load, where we rely
+        // on solution to be valid to not exceed the number of vehicles per
+        // vehicle type.
+        auto const r = vehicleOffset[solRoute.vehicleType()]++;
+        Route *route = &routes[r];
+        Node *startDepot = &startDepots[r];
+        Node *endDepot = &endDepots[r];
 
-            client->prev = startDepot;
-            startDepot->next = client;
+        Node *client = &clients[solRoute[0]];
+        client->route = route;
 
-            for (size_t idx = 1; idx < routesIndiv[r].size(); idx++)
-            {
-                Node *prev = client;
+        client->prev = startDepot;
+        startDepot->next = client;
 
-                client = &clients[routesIndiv[r][idx]];
-                client->route = route;
+        for (size_t idx = 1; idx < solRoute.size(); idx++)
+        {
+            Node *prev = client;
 
-                client->prev = prev;
-                prev->next = client;
-            }
+            client = &clients[solRoute[idx]];
+            client->route = route;
 
-            client->next = endDepot;
-            endDepot->prev = client;
+            client->prev = prev;
+            prev->next = client;
         }
 
-        route->update();
+        client->next = endDepot;
+        endDepot->prev = client;
     }
 
+    for (auto &route : routes)
+        route.update();
+
     for (auto *routeOp : routeOps)
-        routeOp->init(individual);
+        routeOp->init(solution);
 }
 
-Individual LocalSearch::exportIndividual()
+Solution LocalSearch::exportSolution() const
 {
-    std::vector<std::vector<int>> indivRoutes(data.numVehicles());
+    std::vector<Solution::Route> solRoutes;
+    solRoutes.reserve(data.numVehicles());
 
     for (size_t r = 0; r < data.numVehicles(); r++)
     {
+        if (routes[r].empty())
+            continue;
+
+        std::vector<int> visits;
         Node *node = startDepots[r].next;
 
         while (!node->isDepot())
         {
-            indivRoutes[r].push_back(node->client);
+            visits.push_back(node->client);
             node = node->next;
         }
+
+        solRoutes.emplace_back(data, visits, routes[r].vehicleType());
     }
 
-    return {data, indivRoutes};
+    return {data, solRoutes};
 }
 
 void LocalSearch::addNodeOperator(NodeOp &op) { nodeOps.emplace_back(&op); }
 
 void LocalSearch::addRouteOperator(RouteOp &op) { routeOps.emplace_back(&op); }
 
 void LocalSearch::setNeighbours(Neighbours neighbours)
@@ -379,43 +411,50 @@
     auto isEmpty = [](auto const &neighbours) { return neighbours.empty(); };
     if (std::all_of(neighbours.begin(), neighbours.end(), isEmpty))
         throw std::runtime_error("Neighbourhood is empty.");
 
     this->neighbours = neighbours;
 }
 
-LocalSearch::Neighbours LocalSearch::getNeighbours() { return neighbours; }
+LocalSearch::Neighbours const &LocalSearch::getNeighbours() const
+{
+    return neighbours;
+}
 
-LocalSearch::LocalSearch(ProblemData &data,
-                         XorShift128 &rng,
-                         Neighbours neighbours)
+LocalSearch::LocalSearch(ProblemData const &data, Neighbours neighbours)
     : data(data),
-      rng(rng),
       neighbours(data.numClients() + 1),
       orderNodes(data.numClients()),
       orderRoutes(data.numVehicles()),
       lastModified(data.numVehicles(), -1),
       clients(data.numClients() + 1),
-      routes(data.numVehicles(), data),
       startDepots(data.numVehicles()),
       endDepots(data.numVehicles())
 {
     setNeighbours(neighbours);
 
     std::iota(orderNodes.begin(), orderNodes.end(), 1);
     std::iota(orderRoutes.begin(), orderRoutes.end(), 0);
 
     for (size_t i = 0; i <= data.numClients(); i++)
         clients[i].client = i;
 
-    for (size_t i = 0; i < data.numVehicles(); i++)
+    routes.reserve(data.numVehicles());
+    size_t rIdx = 0;
+    for (size_t vehType = 0; vehType != data.numVehicleTypes(); ++vehType)
     {
-        routes[i].idx = i;
-        routes[i].depot = &startDepots[i];
+        auto const numAvailable = data.vehicleType(vehType).numAvailable;
+        for (size_t i = 0; i != numAvailable; ++i)
+        {
+            routes.emplace_back(data, rIdx, vehType);
+            routes[rIdx].depot = &startDepots[rIdx];
+
+            startDepots[rIdx].client = 0;
+            startDepots[rIdx].route = &routes[rIdx];
 
-        startDepots[i].client = 0;
-        startDepots[i].route = &routes[i];
+            endDepots[rIdx].client = 0;
+            endDepots[rIdx].route = &routes[rIdx];
 
-        endDepots[i].client = 0;
-        endDepots[i].route = &routes[i];
+            rIdx++;
+        }
     }
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch.h` & `pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-#ifndef LOCALSEARCH_H
-#define LOCALSEARCH_H
+#ifndef PYVRP_LOCALSEARCH_H
+#define PYVRP_LOCALSEARCH_H
 
 #include "CostEvaluator.h"
-#include "Individual.h"
 #include "LocalSearchOperator.h"
 #include "Node.h"
 #include "ProblemData.h"
 #include "Route.h"
+#include "Solution.h"
 #include "XorShift128.h"
 
 #include <functional>
 #include <stdexcept>
 #include <vector>
 
 class LocalSearch
 {
     using NodeOp = LocalSearchOperator<Node>;
     using RouteOp = LocalSearchOperator<Route>;
     using Neighbours = std::vector<std::vector<int>>;
 
-    ProblemData &data;
-    XorShift128 &rng;
+    ProblemData const &data;
 
-    // Neighborhood restrictions: For each client, list of nearby clients (size
-    // nbClients + 1, but nothing stored for the depot!)
+    // Neighborhood restrictions: list of nearby clients for each client (size
+    // numClients + 1, but nothing stored for the depot!)
     Neighbours neighbours;
 
-    std::vector<int> orderNodes;   // random node order used in RI operators
-    std::vector<int> orderRoutes;  // random route order used in SWAP* operators
+    std::vector<int> orderNodes;   // node order used by LocalSearch::search
+    std::vector<int> orderRoutes;  // route order used by LocalSearch::intensify
 
     std::vector<int> lastModified;  // tracks when routes were last modified
 
     std::vector<Node> clients;  // Note that clients[0] is a sentinel value
     std::vector<Route> routes;
+
     std::vector<Node> startDepots;  // These mark the start of routes
     std::vector<Node> endDepots;    // These mark the end of routes
 
     std::vector<NodeOp *> nodeOps;
     std::vector<RouteOp *> routeOps;
 
     int numMoves = 0;              // Operator counter
     bool searchCompleted = false;  // No further improving move found?
 
-    // Load an initial solution that we will attempt to improve
-    void loadIndividual(Individual const &individual);
+    // Load an initial solution that we will attempt to improve.
+    void loadSolution(Solution const &solution);
 
-    // Export the LS solution back into an individual
-    Individual exportIndividual();
+    // Export the LS solution back into a solution.
+    Solution exportSolution() const;
 
     // Tests the node pair (U, V).
     bool applyNodeOps(Node *U, Node *V, CostEvaluator const &costEvaluator);
 
     // Tests the route pair (U, V).
     bool applyRouteOps(Route *U, Route *V, CostEvaluator const &costEvaluator);
 
@@ -81,29 +81,33 @@
      * no nearby client.
      */
     void setNeighbours(Neighbours neighbours);
 
     /**
      * @return The neighbourhood structure currently in use.
      */
-    Neighbours getNeighbours();
+    Neighbours const &getNeighbours() const;
+
+    /**
+     * Performs regular (node-based) local search around the given solution,
+     * and returns a new, hopefully improved solution.
+     */
+    Solution search(Solution &solution, CostEvaluator const &costEvaluator);
 
     /**
-     * Performs regular (node-based) local search around the given individual,
-     * and returns a new, hopefully improved individual.
+     * Performs a more intensive route-based local search around the given
+     * solution, and returns a new, hopefully improved solution.
      */
-    Individual search(Individual &individual,
-                      CostEvaluator const &costEvaluator);
+    Solution intensify(Solution &solution,
+                       CostEvaluator const &costEvaluator,
+                       int overlapToleranceDegrees = 0);
 
     /**
-     * Performs a more intensive local search around the given individual,
-     * using route-based operators and subpath enumeration. Returns a new,
-     * hopefully improved individual.
+     * Shuffles the order in which the node and route pairs are evaluated, and
+     * the order in which node and route operators are applied.
      */
-    Individual intensify(Individual &individual,
-                         CostEvaluator const &costEvaluator,
-                         int overlapToleranceDegrees = 0);
+    void shuffle(XorShift128 &rng);
 
-    LocalSearch(ProblemData &data, XorShift128 &rng, Neighbours neighbours);
+    LocalSearch(ProblemData const &data, Neighbours neighbours);
 };
 
-#endif
+#endif  // PYVRP_LOCALSEARCH_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearchOperator.h` & `pyvrp-0.4.1/pyvrp/cpp/search/LocalSearchOperator.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-#ifndef LOCALSEARCHOPERATOR_H
-#define LOCALSEARCHOPERATOR_H
+#ifndef PYVRP_LOCALSEARCHOPERATOR_H
+#define PYVRP_LOCALSEARCHOPERATOR_H
 
 #include "CostEvaluator.h"
-#include "Individual.h"
+#include "Measure.h"
 #include "Node.h"
 #include "ProblemData.h"
 #include "Route.h"
+#include "Solution.h"
 
 template <typename Arg> class LocalSearchOperatorBase
 {
     // Can only be specialised into either a Node or Route operator; there
     // are no other types that are expected to work.
     static_assert(std::is_same<Arg, Node>::value
                   || std::is_same<Arg, Route>::value);
@@ -25,24 +26,23 @@
      * The contract is as follows: if the cost delta is negative, that is the
      * true cost delta of this move. As such, improving moves are fully
      * evaluated. The operator, however, is free to return early if it knows
      * the move will never be good: that is, when it determines the cost delta
      * cannot become negative at all. In that case, the returned (non-negative)
      * cost delta does not constitute a full evaluation.
      */
-    virtual int evaluate(Arg *U, Arg *V, CostEvaluator const &costEvaluator)
-    {
-        return 0;
-    }
+    virtual Cost evaluate(Arg *U, Arg *V, CostEvaluator const &costEvaluator)
+        = 0;
 
     /**
      * Applies this operator to the given arguments. For improvements, should
      * only be called if <code>evaluate()</code> returns a negative delta cost.
      */
-    virtual void apply(Arg *U, Arg *V) const {};
+    // TODO remove arguments - always applies to most recently evaluated pair.
+    virtual void apply(Arg *U, Arg *V) const = 0;
 
     LocalSearchOperatorBase(ProblemData const &data) : data(data){};
     virtual ~LocalSearchOperatorBase() = default;
 };
 
 template <typename Arg>
 class LocalSearchOperator : public LocalSearchOperatorBase<Arg>
@@ -58,21 +58,21 @@
 template <>  // specialisation for route operators
 class LocalSearchOperator<Route> : public LocalSearchOperatorBase<Route>
 {
     using LocalSearchOperatorBase::LocalSearchOperatorBase;
 
 public:
     /**
-     * Called once after loading in the individual to improve. This can be used
+     * Called once after loading in the solution to improve. This can be used
      * to e.g. update local operator state.
      */
-    virtual void init(Individual const &indiv){};
+    virtual void init([[maybe_unused]] Solution const &solution){};
 
     /**
      * Called when a route has been changed. Can be used to update caches, but
      * the implementation should be fast: this is called every time something
      * changes!
      */
-    virtual void update(Route *U){};
+    virtual void update([[maybe_unused]] Route *U){};
 };
 
-#endif  // LOCALSEARCHOPERATOR_H
+#endif  // PYVRP_LOCALSEARCHOPERATOR_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch_bindings.cpp` & `pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch_bindings.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -5,22 +5,18 @@
 #include <pybind11/stl.h>
 
 namespace py = pybind11;
 
 PYBIND11_MODULE(_LocalSearch, m)
 {
     py::class_<LocalSearch>(m, "LocalSearch")
-        .def(py::init<ProblemData &,
-                      XorShift128 &,
-                      std::vector<std::vector<int>>>(),
+        .def(py::init<ProblemData const &, std::vector<std::vector<int>>>(),
              py::arg("data"),
-             py::arg("rng"),
              py::arg("neighbours"),
-             py::keep_alive<1, 2>(),  // keep data and rng alive at least until
-             py::keep_alive<1, 3>())  // local search is freed
+             py::keep_alive<1, 2>())  // keep data alive until LS is freed
         .def("add_node_operator",
              &LocalSearch::addNodeOperator,
              py::arg("op"),
              py::keep_alive<1, 2>())
         .def("add_route_operator",
              &LocalSearch::addRouteOperator,
              py::arg("op"),
@@ -29,15 +25,16 @@
              &LocalSearch::setNeighbours,
              py::arg("neighbours"))
         .def("get_neighbours",
              &LocalSearch::getNeighbours,
              py::return_value_policy::reference_internal)
         .def("search",
              &LocalSearch::search,
-             py::arg("individual"),
+             py::arg("solution"),
              py::arg("cost_evaluator"))
         .def("intensify",
              &LocalSearch::intensify,
-             py::arg("individual"),
+             py::arg("solution"),
              py::arg("cost_evaluator"),
-             py::arg("overlap_tolerance_degrees") = 0);
+             py::arg("overlap_tolerance_degrees") = 0)
+        .def("shuffle", &LocalSearch::shuffle, py::arg("rng"));
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/MoveTwoClientsReversed.cpp` & `pyvrp-0.4.1/pyvrp/cpp/search/MoveTwoClientsReversed.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 #include "Route.h"
 #include "TimeWindowSegment.h"
 
 #include <cassert>
 
 using TWS = TimeWindowSegment;
 
-int MoveTwoClientsReversed::evaluate(Node *U,
-                                     Node *V,
-                                     CostEvaluator const &costEvaluator)
+Cost MoveTwoClientsReversed::evaluate(Node *U,
+                                      Node *V,
+                                      CostEvaluator const &costEvaluator)
 {
     if (U == n(V) || n(U) == V || n(U)->isDepot())
         return 0;
 
     auto const posU = U->position;
     auto const posV = V->position;
 
     assert(U->route && V->route);
 
-    int const current = U->route->distBetween(posU - 1, posU + 2)
-                        + data.dist(V->client, n(V)->client);
-    int const proposed = data.dist(p(U)->client, n(n(U))->client)
-                         + data.dist(V->client, n(U)->client)
-                         + data.dist(n(U)->client, U->client)
-                         + data.dist(U->client, n(V)->client);
+    Distance const current = U->route->distBetween(posU - 1, posU + 2)
+                             + data.dist(V->client, n(V)->client);
+    Distance const proposed = data.dist(p(U)->client, n(n(U))->client)
+                              + data.dist(V->client, n(U)->client)
+                              + data.dist(n(U)->client, U->client)
+                              + data.dist(U->client, n(V)->client);
 
-    int deltaCost = proposed - current;
+    Cost deltaCost = static_cast<Cost>(proposed - current);
 
     if (U->route != V->route)
     {
         if (U->route->isFeasible() && deltaCost >= 0)
             return deltaCost;
 
         auto uTWS = TWS::merge(
@@ -37,25 +37,25 @@
 
         deltaCost += costEvaluator.twPenalty(uTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
         auto const loadDiff = U->route->loadBetween(posU, posU + 1);
 
         deltaCost += costEvaluator.loadPenalty(U->route->load() - loadDiff,
-                                               data.vehicleCapacity());
+                                               U->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(U->route->load(),
-                                               data.vehicleCapacity());
+                                               U->route->capacity());
 
         if (deltaCost >= 0)    // if delta cost of just U's route is not enough
             return deltaCost;  // even without V, the move will never be good
 
         deltaCost += costEvaluator.loadPenalty(V->route->load() + loadDiff,
-                                               data.vehicleCapacity());
+                                               V->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(V->route->load(),
-                                               data.vehicleCapacity());
+                                               V->route->capacity());
 
         auto vTWS = TWS::merge(
             data.durationMatrix(), V->twBefore, n(U)->tw, U->tw, n(V)->twAfter);
 
         deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
     }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/Node.cpp` & `pyvrp-0.4.1/pyvrp/cpp/search/Node.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/Node.h` & `pyvrp-0.4.1/pyvrp/cpp/search/Node.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#ifndef NODE_H
-#define NODE_H
+#ifndef PYVRP_NODE_H
+#define PYVRP_NODE_H
 
-#include "ProblemData.h"
+#include "Measure.h"
 #include "TimeWindowSegment.h"
 
 class Route;
 
 struct Node
 {
     int client;       // Client represented with this node
     size_t position;  // Position in the route
     Node *next;       // Next node in the route order
     Node *prev;       // Previous node in the route order
     Route *route;     // Pointer towards the associated route
 
     // TODO can these data fields be moved to Route?
-    int cumulatedLoad;              // Load from depot to client (inclusive)
-    int cumulatedDistance;          // Distance from depot to client (inclusive)
-    int cumulatedReversalDistance;  // Distance if (0 .. client) is reversed
+    Load cumulatedLoad;                  // Load depot -> client (incl)
+    Distance cumulatedDistance;          // Dist depot -> client (incl)
+    Distance cumulatedReversalDistance;  // Dist if (0..client) is reversed
 
     TimeWindowSegment tw;        // TWS for individual node (client)
     TimeWindowSegment twBefore;  // TWS for (0...client) including self
     TimeWindowSegment twAfter;   // TWS for (client...0) including self
 
     [[nodiscard]] inline bool isDepot() const;
 
@@ -49,8 +49,8 @@
 inline Node *p(Node *node) { return node->prev; }
 
 /**
  * Convenience method accessing the node directly after the argument.
  */
 inline Node *n(Node *node) { return node->next; }
 
-#endif  // NODE_H
+#endif  // PYVRP_NODE_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar.h` & `pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-#ifndef RELOCATESTAR_H
-#define RELOCATESTAR_H
+#ifndef PYVRP_RELOCATESTAR_H
+#define PYVRP_RELOCATESTAR_H
 
 #include "Exchange.h"
 #include "LocalSearchOperator.h"
 
 /**
  * Performs the best (1, 0)-exchange move between routes U and V. Tests both
  * ways: from U to V, and from V to U.
  */
 class RelocateStar : public LocalSearchOperator<Route>
 {
     struct Move
     {
-        int deltaCost = 0;
+        Cost deltaCost = 0;
         Node *from = nullptr;
         Node *to = nullptr;
     };
 
     Exchange<1, 0> relocate;
     Move move;
 
 public:
-    int
+    Cost
     evaluate(Route *U, Route *V, CostEvaluator const &costEvaluator) override;
 
     void apply(Route *U, Route *V) const override;
 
     RelocateStar(ProblemData const &data)
         : LocalSearchOperator<Route>(data), relocate(data)
     {
     }
 };
 
-#endif  // RELOCATESTAR_H
+#endif  // PYVRP_RELOCATESTAR_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/Route.cpp` & `pyvrp-0.4.1/pyvrp/cpp/search/Route.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 #include "Route.h"
 
 #include <cmath>
 #include <ostream>
 
 using TWS = TimeWindowSegment;
 
-Route::Route(ProblemData const &data) : data(data) {}
+Route::Route(ProblemData const &data, size_t const idx, size_t const vehType)
+    : data(data), vehicleType_(vehType), idx(idx)
+{
+}
 
 void Route::setupNodes()
 {
     nodes.clear();
     auto *node = depot;
 
     do
@@ -23,32 +26,35 @@
 }
 
 void Route::setupSector()
 {
     if (empty())  // Note: sector has no meaning for empty routes, don't use
         return;
 
-    auto const depotData = data.client(0);
-    auto const clientData = data.client(n(depot)->client);
-    auto const angle = CircleSector::positive_mod(static_cast<int>(
-        32768. * atan2(clientData.y - depotData.y, clientData.x - depotData.x)
-        / M_PI));
+    auto const &depotData = data.client(0);
+    auto const &clientData = data.client(n(depot)->client);
+
+    auto const diffX = static_cast<double>(clientData.x - depotData.x);
+    auto const diffY = static_cast<double>(clientData.y - depotData.y);
+    auto const angle = CircleSector::positive_mod(
+        static_cast<int>(32768. * atan2(diffY, diffX) / M_PI));
 
     sector.initialize(angle);
 
     for (auto it = nodes.begin(); it != nodes.end() - 1; ++it)
     {
         auto const *node = *it;
         assert(!node->isDepot());
 
-        auto const clientData = data.client(node->client);
-        auto const angle = CircleSector::positive_mod(static_cast<int>(
-            32768.
-            * atan2(clientData.y - depotData.y, clientData.x - depotData.x)
-            / M_PI));
+        auto const &clientData = data.client(node->client);
+
+        auto const diffX = static_cast<double>(clientData.x - depotData.x);
+        auto const diffY = static_cast<double>(clientData.y - depotData.y);
+        auto const angle = CircleSector::positive_mod(
+            static_cast<int>(32768. * atan2(diffY, diffX) / M_PI));
 
         sector.extend(angle);
     }
 }
 
 void Route::setupRouteTimeWindows()
 {
@@ -59,27 +65,29 @@
         auto *prev = p(node);
         prev->twAfter
             = TWS::merge(data.durationMatrix(), prev->tw, node->twAfter);
         node = prev;
     } while (!node->isDepot());
 }
 
+size_t Route::vehicleType() const { return vehicleType_; }
+
 bool Route::overlapsWith(Route const &other, int const tolerance) const
 {
     return CircleSector::overlap(sector, other.sector, tolerance);
 }
 
 void Route::update()
 {
     auto const oldNodes = nodes;
     setupNodes();
 
-    int load = 0;
-    int distance = 0;
-    int reverseDistance = 0;
+    Load load = 0;
+    Distance distance = 0;
+    Distance reverseDistance = 0;
     bool foundChange = false;
 
     for (size_t pos = 0; pos != nodes.size(); ++pos)
     {
         auto *node = nodes[pos];
 
         if (!foundChange && (pos >= oldNodes.size() || node != oldNodes[pos]))
@@ -111,15 +119,15 @@
             = TWS::merge(data.durationMatrix(), p(node)->twBefore, node->tw);
     }
 
     setupSector();
     setupRouteTimeWindows();
 
     load_ = nodes.back()->cumulatedLoad;
-    isLoadFeasible_ = static_cast<size_t>(load_) <= data.vehicleCapacity();
+    isLoadFeasible_ = load_ <= capacity();
 
     timeWarp_ = nodes.back()->twBefore.totalTimeWarp();
     isTimeWarpFeasible_ = timeWarp_ == 0;
 }
 
 std::ostream &operator<<(std::ostream &out, Route const &route)
 {
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/Route.h` & `pyvrp-0.4.1/pyvrp/cpp/search/Route.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-#ifndef HGS_VRPTW_ROUTE_H
-#define HGS_VRPTW_ROUTE_H
+#ifndef PYVRP_ROUTE_H
+#define PYVRP_ROUTE_H
 
 #include "CircleSector.h"
 #include "Node.h"
+#include "ProblemData.h"
 #include "TimeWindowSegment.h"
 
 #include <array>
 #include <bit>
 #include <cassert>
 #include <iosfwd>
 
 class Route
 {
     ProblemData const &data;
+    size_t const vehicleType_;
 
     std::vector<Node *> nodes;  // List of nodes (in order) in this solution.
     CircleSector sector;        // Circle sector of the route's clients
 
-    int load_;             // Current route load.
+    Load load_;            // Current route load.
     bool isLoadFeasible_;  // Whether current load is feasible.
 
-    int timeWarp_;             // Current route time warp.
+    Duration timeWarp_;        // Current route time warp.
     bool isTimeWarpFeasible_;  // Whether current time warp is feasible.
 
     // Populates the nodes vector.
     void setupNodes();
 
     // Sets the sector data.
     void setupSector();
 
     // Sets forward node time windows.
     void setupRouteTimeWindows();
 
-public:           // TODO make fields private
-    int idx;      // Route index
-    Node *depot;  // Pointer to the associated depot
+public:                // TODO make fields private
+    size_t const idx;  // Route index
+    Node *depot;       // Pointer to the associated depot
 
     /**
      * @return The client or depot node at the given position.
      */
     [[nodiscard]] inline Node *operator[](size_t position) const;
 
     /**
@@ -47,102 +49,114 @@
      * @return true if the route is feasible, false otherwise.
      */
     [[nodiscard]] inline bool isFeasible() const;
 
     /**
      * Determines whether this route is load-feasible.
      *
-     * @return true if the route exceeds the vehicle capacity, false otherwise.
+     * @return true if the route exceeds the capacity, false otherwise.
      */
     [[nodiscard]] inline bool hasExcessLoad() const;
 
     /**
      * Determines whether this route is time-feasible.
      *
      * @return true if the route has time warp, false otherwise.
      */
     [[nodiscard]] inline bool hasTimeWarp() const;
 
     /**
      * @return Total load on this route.
      */
-    [[nodiscard]] inline int load() const;
+    [[nodiscard]] inline Load load() const;
 
     /**
      * @return Total time warp on this route.
      */
-    [[nodiscard]] inline int timeWarp() const;
+    [[nodiscard]] inline Duration timeWarp() const;
 
     /**
      * @return true if this route is empty, false otherwise.
      */
     [[nodiscard]] inline bool empty() const;
 
     /**
+     * @return The load capacity of this route.
+     */
+    [[nodiscard]] inline Load capacity() const;
+
+    /**
      * @return Number of clients in this route.
      */
     [[nodiscard]] inline size_t size() const;
 
     /**
      * Calculates time window data for segment [start, end].
      */
     [[nodiscard]] inline TimeWindowSegment twBetween(size_t start,
                                                      size_t end) const;
 
     /**
      * Calculates the distance for segment [start, end].
      */
-    [[nodiscard]] inline int distBetween(size_t start, size_t end) const;
+    [[nodiscard]] inline Distance distBetween(size_t start, size_t end) const;
 
     /**
      * Calculates the load for segment [start, end].
      */
-    [[nodiscard]] inline int loadBetween(size_t start, size_t end) const;
+    [[nodiscard]] inline Load loadBetween(size_t start, size_t end) const;
+
+    /**
+     * @return This route's vehicle type.
+     */
+    [[nodiscard]] size_t vehicleType() const;
 
     /**
      * Tests if this route overlaps with the other route, that is, whether
      * their circle sectors overlap with a given tolerance.
      */
     [[nodiscard]] bool overlapsWith(Route const &other,
                                     int const tolerance) const;
 
     /**
      * Updates this route. To be called after swapping nodes/changing the
      * solution.
      */
     void update();
 
-    Route(ProblemData const &data);
+    Route(ProblemData const &data, size_t const idx, size_t const vehType);
 };
 
 bool Route::isFeasible() const { return !hasExcessLoad() && !hasTimeWarp(); }
 
 bool Route::hasExcessLoad() const { return !isLoadFeasible_; }
 
 bool Route::hasTimeWarp() const
 {
-#ifdef VRP_NO_TIME_WINDOWS
+#ifdef PYVRP_NO_TIME_WINDOWS
     return false;
 #else
     return !isTimeWarpFeasible_;
 #endif
 }
 
 Node *Route::operator[](size_t position) const
 {
     assert(position > 0);
     return nodes[position - 1];
 }
 
-int Route::load() const { return load_; }
+Load Route::load() const { return load_; }
 
-int Route::timeWarp() const { return timeWarp_; }
+Duration Route::timeWarp() const { return timeWarp_; }
 
 bool Route::empty() const { return size() == 0; }
 
+Load Route::capacity() const { return data.vehicleType(vehicleType_).capacity; }
+
 size_t Route::size() const
 {
     return nodes.size() - 1;  // exclude end depot
 }
 
 TimeWindowSegment Route::twBetween(size_t start, size_t end) const
 {
@@ -153,27 +167,27 @@
     for (size_t step = start; step != end; ++step)
         tws = TimeWindowSegment::merge(
             data.durationMatrix(), tws, nodes[step]->tw);
 
     return tws;
 }
 
-int Route::distBetween(size_t start, size_t end) const
+Distance Route::distBetween(size_t start, size_t end) const
 {
     assert(start <= end && end <= nodes.size());
 
     auto const startDist = start == 0 ? 0 : nodes[start - 1]->cumulatedDistance;
     auto const endDist = nodes[end - 1]->cumulatedDistance;
 
     assert(startDist <= endDist);
 
     return endDist - startDist;
 }
 
-int Route::loadBetween(size_t start, size_t end) const
+Load Route::loadBetween(size_t start, size_t end) const
 {
     assert(start <= end && end <= nodes.size());
 
     auto const *startNode = start == 0 ? depot : nodes[start - 1];
     auto const atStart = data.client(startNode->client).demand;
     auto const startLoad = startNode->cumulatedLoad;
     auto const endLoad = nodes[end - 1]->cumulatedLoad;
@@ -182,8 +196,8 @@
 
     return endLoad - startLoad + atStart;
 }
 
 // Outputs a route into a given ostream in CVRPLib format
 std::ostream &operator<<(std::ostream &out, Route const &route);
 
-#endif  // HGS_VRPTW_ROUTE_H
+#endif  // PYVRP_ROUTE_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar.cpp` & `pyvrp-0.4.1/pyvrp/cpp/search/SwapStar.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #include "SwapStar.h"
 
 using TWS = TimeWindowSegment;
 
 void SwapStar::updateRemovalCosts(Route *R1, CostEvaluator const &costEvaluator)
 {
-    auto const currTimeWarp = costEvaluator.twPenalty(R1->timeWarp());
-
     for (Node *U = n(R1->depot); !U->isDepot(); U = n(U))
     {
         auto twData
             = TWS::merge(data.durationMatrix(), p(U)->twBefore, n(U)->twAfter);
+
+        Distance const deltaDist = data.dist(p(U)->client, n(U)->client)
+                                   - data.dist(p(U)->client, U->client)
+                                   - data.dist(U->client, n(U)->client);
+
         removalCosts(R1->idx, U->client)
-            = data.dist(p(U)->client, n(U)->client)
-              - data.dist(p(U)->client, U->client)
-              - data.dist(U->client, n(U)->client)
-              + costEvaluator.twPenalty(twData.totalTimeWarp()) - currTimeWarp;
+            = static_cast<Cost>(deltaDist)
+              + costEvaluator.twPenalty(twData.totalTimeWarp())
+              - costEvaluator.twPenalty(R1->timeWarp());
     }
 }
 
 void SwapStar::updateInsertionCost(Route *R,
                                    Node *U,
                                    CostEvaluator const &costEvaluator)
 {
@@ -26,70 +28,78 @@
 
     insertPositions = {};
     insertPositions.shouldUpdate = false;
 
     // Insert cost of U just after the depot (0 -> U -> ...)
     auto twData = TWS::merge(
         data.durationMatrix(), R->depot->twBefore, U->tw, n(R->depot)->twAfter);
-    int cost = data.dist(0, U->client)
-               + data.dist(U->client, n(R->depot)->client)
-               - data.dist(0, n(R->depot)->client)
-               + costEvaluator.twPenalty(twData.totalTimeWarp())
-               - costEvaluator.twPenalty(R->timeWarp());
 
-    insertPositions.maybeAdd(cost, R->depot);
+    Distance deltaDist = data.dist(0, U->client)
+                         + data.dist(U->client, n(R->depot)->client)
+                         - data.dist(0, n(R->depot)->client);
+
+    Cost deltaCost = static_cast<Cost>(deltaDist)
+                     + costEvaluator.twPenalty(twData.totalTimeWarp())
+                     - costEvaluator.twPenalty(R->timeWarp());
+
+    insertPositions.maybeAdd(deltaCost, R->depot);
 
     for (Node *V = n(R->depot); !V->isDepot(); V = n(V))
     {
         // Insert cost of U just after V (V -> U -> ...)
         twData = TWS::merge(
             data.durationMatrix(), V->twBefore, U->tw, n(V)->twAfter);
-        int deltaCost = data.dist(V->client, U->client)
-                        + data.dist(U->client, n(V)->client)
-                        - data.dist(V->client, n(V)->client)
-                        + costEvaluator.twPenalty(twData.totalTimeWarp())
-                        - costEvaluator.twPenalty(R->timeWarp());
+
+        deltaDist = data.dist(V->client, U->client)
+                    + data.dist(U->client, n(V)->client)
+                    - data.dist(V->client, n(V)->client);
+
+        deltaCost = static_cast<Cost>(deltaDist)
+                    + costEvaluator.twPenalty(twData.totalTimeWarp())
+                    - costEvaluator.twPenalty(R->timeWarp());
 
         insertPositions.maybeAdd(deltaCost, V);
     }
 }
 
-std::pair<int, Node *> SwapStar::getBestInsertPoint(
+std::pair<Cost, Node *> SwapStar::getBestInsertPoint(
     Node *U, Node *V, CostEvaluator const &costEvaluator)
 {
     auto &best_ = cache(V->route->idx, U->client);
 
     if (best_.shouldUpdate)  // then we first update the insert positions
         updateInsertionCost(V->route, U, costEvaluator);
 
     for (size_t idx = 0; idx != 3; ++idx)  // only OK if V is not adjacent
         if (best_.locs[idx] && best_.locs[idx] != V && n(best_.locs[idx]) != V)
             return std::make_pair(best_.costs[idx], best_.locs[idx]);
 
     // As a fallback option, we consider inserting in the place of V
     auto const twData = TWS::merge(
         data.durationMatrix(), p(V)->twBefore, U->tw, n(V)->twAfter);
-    int deltaCost = data.dist(p(V)->client, U->client)
-                    + data.dist(U->client, n(V)->client)
-                    - data.dist(p(V)->client, n(V)->client)
-                    + costEvaluator.twPenalty(twData.totalTimeWarp())
-                    - costEvaluator.twPenalty(V->route->timeWarp());
+
+    Distance const deltaDist = data.dist(p(V)->client, U->client)
+                               + data.dist(U->client, n(V)->client)
+                               - data.dist(p(V)->client, n(V)->client);
+    Cost const deltaCost = static_cast<Cost>(deltaDist)
+                           + costEvaluator.twPenalty(twData.totalTimeWarp())
+                           - costEvaluator.twPenalty(V->route->timeWarp());
 
     return std::make_pair(deltaCost, p(V));
 }
 
-void SwapStar::init(Individual const &indiv)
+void SwapStar::init(Solution const &solution)
 {
-    LocalSearchOperator<Route>::init(indiv);
+    LocalSearchOperator<Route>::init(solution);
     std::fill(updated.begin(), updated.end(), true);
 }
 
-int SwapStar::evaluate(Route *routeU,
-                       Route *routeV,
-                       CostEvaluator const &costEvaluator)
+Cost SwapStar::evaluate(Route *routeU,
+                        Route *routeV,
+                        CostEvaluator const &costEvaluator)
 {
     best = {};
 
     if (updated[routeV->idx])
     {
         updateRemovalCosts(routeV, costEvaluator);
         updated[routeV->idx] = false;
@@ -106,29 +116,29 @@
         for (size_t idx = 1; idx != data.numClients() + 1; ++idx)
             cache(routeU->idx, idx).shouldUpdate = true;
     }
 
     for (Node *U = n(routeU->depot); !U->isDepot(); U = n(U))
         for (Node *V = n(routeV->depot); !V->isDepot(); V = n(V))
         {
-            int deltaCost = 0;
+            Cost deltaCost = 0;
 
-            int const uDemand = data.client(U->client).demand;
-            int const vDemand = data.client(V->client).demand;
-            int const loadDiff = uDemand - vDemand;
+            auto const uDemand = data.client(U->client).demand;
+            auto const vDemand = data.client(V->client).demand;
+            auto const loadDiff = uDemand - vDemand;
 
             deltaCost += costEvaluator.loadPenalty(routeU->load() - loadDiff,
-                                                   data.vehicleCapacity());
+                                                   U->route->capacity());
             deltaCost -= costEvaluator.loadPenalty(routeU->load(),
-                                                   data.vehicleCapacity());
+                                                   U->route->capacity());
 
             deltaCost += costEvaluator.loadPenalty(routeV->load() + loadDiff,
-                                                   data.vehicleCapacity());
+                                                   V->route->capacity());
             deltaCost -= costEvaluator.loadPenalty(routeV->load(),
-                                                   data.vehicleCapacity());
+                                                   V->route->capacity());
 
             deltaCost += removalCosts(routeU->idx, U->client);
             deltaCost += removalCosts(routeV->idx, V->client);
 
             if (deltaCost >= 0)  // an early filter on many moves, before doing
                 continue;        // costly work determining insertion points
 
@@ -157,44 +167,42 @@
     // complete evaluation. But in practice that almost never happens, and is
     // not worth spending time on.
     if (best.cost >= 0)
         return best.cost;
 
     // Now do a full evaluation of the proposed swap move. This includes
     // possible time warp penalties.
-    int const current = data.dist(p(best.U)->client, best.U->client)
-                        + data.dist(best.U->client, n(best.U)->client)
-                        + data.dist(p(best.V)->client, best.V->client)
-                        + data.dist(best.V->client, n(best.V)->client);
+    Distance const current = data.dist(p(best.U)->client, best.U->client)
+                             + data.dist(best.U->client, n(best.U)->client)
+                             + data.dist(p(best.V)->client, best.V->client)
+                             + data.dist(best.V->client, n(best.V)->client);
 
-    int const proposed = data.dist(best.VAfter->client, best.V->client)
-                         + data.dist(best.UAfter->client, best.U->client);
+    Distance const proposed = data.dist(best.VAfter->client, best.V->client)
+                              + data.dist(best.UAfter->client, best.U->client);
 
-    int deltaCost = proposed - current;
+    Distance deltaDist = proposed - current;
 
     if (best.VAfter == p(best.U))
-    {
         // Insert in place of U
-        deltaCost += data.dist(best.V->client, n(best.U)->client);
-    }
+        deltaDist += data.dist(best.V->client, n(best.U)->client);
     else
-    {
-        deltaCost += data.dist(best.V->client, n(best.VAfter)->client)
+        deltaDist += data.dist(best.V->client, n(best.VAfter)->client)
                      + data.dist(p(best.U)->client, n(best.U)->client)
                      - data.dist(best.VAfter->client, n(best.VAfter)->client);
-    }
 
     if (best.UAfter == p(best.V))
         // Insert in place of V
-        deltaCost += data.dist(best.U->client, n(best.V)->client);
+        deltaDist += data.dist(best.U->client, n(best.V)->client);
     else
-        deltaCost += data.dist(best.U->client, n(best.UAfter)->client)
+        deltaDist += data.dist(best.U->client, n(best.UAfter)->client)
                      + data.dist(p(best.V)->client, n(best.V)->client)
                      - data.dist(best.UAfter->client, n(best.UAfter)->client);
 
+    Cost deltaCost = static_cast<Cost>(deltaDist);
+
     // It is not possible to have UAfter == V or VAfter == U, so the positions
     // are always strictly different
     if (best.VAfter->position + 1 == best.U->position)
     {
         // Special case
         auto uTWS = TWS::merge(data.durationMatrix(),
                                best.VAfter->twBefore,
@@ -262,27 +270,25 @@
     deltaCost -= costEvaluator.twPenalty(routeU->timeWarp());
     deltaCost -= costEvaluator.twPenalty(routeV->timeWarp());
 
     auto const uDemand = data.client(best.U->client).demand;
     auto const vDemand = data.client(best.V->client).demand;
 
     deltaCost += costEvaluator.loadPenalty(routeU->load() - uDemand + vDemand,
-                                           data.vehicleCapacity());
-    deltaCost
-        -= costEvaluator.loadPenalty(routeU->load(), data.vehicleCapacity());
+                                           routeU->capacity());
+    deltaCost -= costEvaluator.loadPenalty(routeU->load(), routeU->capacity());
 
     deltaCost += costEvaluator.loadPenalty(routeV->load() + uDemand - vDemand,
-                                           data.vehicleCapacity());
-    deltaCost
-        -= costEvaluator.loadPenalty(routeV->load(), data.vehicleCapacity());
+                                           routeV->capacity());
+    deltaCost -= costEvaluator.loadPenalty(routeV->load(), routeV->capacity());
 
     return deltaCost;
 }
 
-void SwapStar::apply(Route *U, Route *V) const
+void SwapStar::apply([[maybe_unused]] Route *U, [[maybe_unused]] Route *V) const
 {
     if (best.U && best.UAfter && best.V && best.VAfter)
     {
         best.U->insertAfter(best.UAfter);
         best.V->insertAfter(best.VAfter);
     }
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar.h` & `pyvrp-0.4.1/pyvrp/cpp/search/SwapStar.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-#ifndef SWAPSTAR_H
-#define SWAPSTAR_H
+#ifndef PYVRP_SWAPSTAR_H
+#define PYVRP_SWAPSTAR_H
 
 #include "LocalSearchOperator.h"
 #include "Matrix.h"
+#include "Measure.h"
 
 #include <array>
+#include <limits>
 #include <vector>
 
 /**
  * Explores the SWAP* neighbourhood of [1]. The SWAP* neighbourhood explores
  * free form re-insertions of nodes U and V in the given routes (so the nodes
  * are exchanged between routes, but they are not necessarily inserted in
  * the same place as the other exchanged node). Our implementation of the
@@ -19,18 +21,20 @@
  * https://doi.org/10.1016/j.cor.2021.105643
  */
 class SwapStar : public LocalSearchOperator<Route>
 {
     struct ThreeBest  // stores three best SWAP* insertion points
     {
         bool shouldUpdate = true;
-        std::array<int, 3> costs = {INT_MAX, INT_MAX, INT_MAX};
+        std::array<Cost, 3> costs = {std::numeric_limits<Cost>::max(),
+                                     std::numeric_limits<Cost>::max(),
+                                     std::numeric_limits<Cost>::max()};
         std::array<Node *, 3> locs = {nullptr, nullptr, nullptr};
 
-        void maybeAdd(int costInsert, Node *placeInsert)
+        void maybeAdd(Cost costInsert, Node *placeInsert)
         {
             if (costInsert >= costs[2])
                 return;
 
             if (costInsert >= costs[1])
             {
                 costs[2] = costInsert;
@@ -53,15 +57,15 @@
                 locs[0] = placeInsert;
             }
         }
     };
 
     struct BestMove  // tracks the best SWAP* move
     {
-        int cost = 0;
+        Cost cost = 0;
 
         Node *U = nullptr;
         Node *UAfter = nullptr;
 
         Node *V = nullptr;
         Node *VAfter = nullptr;
     };
@@ -72,27 +76,27 @@
     // Updates the cache storing the three best positions in the given route for
     // the passed-in node (client).
     void
     updateInsertionCost(Route *R, Node *U, CostEvaluator const &costEvaluator);
 
     // Gets the delta cost and reinsert point for U in the route of V, assuming
     // V is removed.
-    inline std::pair<int, Node *>
+    inline std::pair<Cost, Node *>
     getBestInsertPoint(Node *U, Node *V, CostEvaluator const &costEvaluator);
 
     Matrix<ThreeBest> cache;
-    Matrix<int> removalCosts;
+    Matrix<Cost> removalCosts;
     std::vector<bool> updated;
 
     BestMove best;
 
 public:
-    void init(Individual const &indiv) override;
+    void init(Solution const &solution) override;
 
-    int
+    Cost
     evaluate(Route *U, Route *V, CostEvaluator const &costEvaluator) override;
 
     void apply(Route *U, Route *V) const override;
 
     void update(Route *U) override;
 
     explicit SwapStar(ProblemData const &data)
@@ -100,8 +104,8 @@
           cache(data.numVehicles(), data.numClients() + 1),
           removalCosts(data.numVehicles(), data.numClients() + 1),
           updated(data.numVehicles(), true)
     {
     }
 };
 
-#endif  // SWAPSTAR_H
+#endif  // PYVRP_SWAPSTAR_H
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt.cpp` & `pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #include "TwoOpt.h"
 
 #include "Route.h"
 #include "TimeWindowSegment.h"
 
 using TWS = TimeWindowSegment;
 
-int TwoOpt::evalWithinRoute(Node *U,
-                            Node *V,
-                            CostEvaluator const &costEvaluator) const
+Cost TwoOpt::evalWithinRoute(Node *U,
+                             Node *V,
+                             CostEvaluator const &costEvaluator) const
 {
     if (U->position + 1 >= V->position)
         return 0;
 
-    int deltaCost = data.dist(U->client, V->client)
-                    + data.dist(n(U)->client, n(V)->client)
-                    + V->cumulatedReversalDistance
-                    - data.dist(U->client, n(U)->client)
-                    - data.dist(V->client, n(V)->client)
-                    - n(U)->cumulatedReversalDistance;
+    Distance const deltaDist = data.dist(U->client, V->client)
+                               + data.dist(n(U)->client, n(V)->client)
+                               + V->cumulatedReversalDistance
+                               - data.dist(U->client, n(U)->client)
+                               - data.dist(V->client, n(V)->client)
+                               - n(U)->cumulatedReversalDistance;
+
+    Cost deltaCost = static_cast<Cost>(deltaDist);
 
     if (!U->route->hasTimeWarp() && deltaCost >= 0)
         return deltaCost;
 
     auto tws = U->twBefore;
     auto *itRoute = V;
     while (itRoute != U)
@@ -34,24 +36,24 @@
 
     deltaCost += costEvaluator.twPenalty(tws.totalTimeWarp());
     deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
     return deltaCost;
 }
 
-int TwoOpt::evalBetweenRoutes(Node *U,
-                              Node *V,
-                              CostEvaluator const &costEvaluator) const
+Cost TwoOpt::evalBetweenRoutes(Node *U,
+                               Node *V,
+                               CostEvaluator const &costEvaluator) const
 {
-    int const current = data.dist(U->client, n(U)->client)
-                        + data.dist(V->client, n(V)->client);
-    int const proposed = data.dist(U->client, n(V)->client)
-                         + data.dist(V->client, n(U)->client);
+    Distance const current = data.dist(U->client, n(U)->client)
+                             + data.dist(V->client, n(V)->client);
+    Distance const proposed = data.dist(U->client, n(V)->client)
+                              + data.dist(V->client, n(U)->client);
 
-    int deltaCost = proposed - current;
+    Cost deltaCost = static_cast<Cost>(proposed - current);
 
     if (U->route->isFeasible() && V->route->isFeasible() && deltaCost >= 0)
         return deltaCost;
 
     auto const uTWS
         = TWS::merge(data.durationMatrix(), U->twBefore, n(V)->twAfter);
 
@@ -60,25 +62,25 @@
 
     auto const vTWS
         = TWS::merge(data.durationMatrix(), V->twBefore, n(U)->twAfter);
 
     deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
     deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
 
-    int const deltaLoad = U->cumulatedLoad - V->cumulatedLoad;
-
-    deltaCost += costEvaluator.loadPenalty(U->route->load() - deltaLoad,
-                                           data.vehicleCapacity());
+    deltaCost += costEvaluator.loadPenalty(U->cumulatedLoad + V->route->load()
+                                               - V->cumulatedLoad,
+                                           U->route->capacity());
     deltaCost
-        -= costEvaluator.loadPenalty(U->route->load(), data.vehicleCapacity());
+        -= costEvaluator.loadPenalty(U->route->load(), U->route->capacity());
 
-    deltaCost += costEvaluator.loadPenalty(V->route->load() + deltaLoad,
-                                           data.vehicleCapacity());
+    deltaCost += costEvaluator.loadPenalty(V->cumulatedLoad + U->route->load()
+                                               - U->cumulatedLoad,
+                                           V->route->capacity());
     deltaCost
-        -= costEvaluator.loadPenalty(V->route->load(), data.vehicleCapacity());
+        -= costEvaluator.loadPenalty(V->route->load(), V->route->capacity());
 
     return deltaCost;
 }
 
 void TwoOpt::applyWithinRoute(Node *U, Node *V) const
 {
     auto *itRoute = V;
@@ -114,15 +116,15 @@
         auto *node = itRouteU;
         itRouteU = n(itRouteU);
         node->insertAfter(insertLocation);
         insertLocation = node;
     }
 }
 
-int TwoOpt::evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator)
+Cost TwoOpt::evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator)
 {
     if (U->route->idx > V->route->idx)  // will be tackled in a later iteration
         return 0;                       // - no need to process here already
 
     return U->route == V->route ? evalWithinRoute(U, V, costEvaluator)
                                 : evalBetweenRoutes(U, V, costEvaluator);
 }
```

### Comparing `pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt.h` & `pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-#ifndef TWOOPT_H
-#define TWOOPT_H
+#ifndef PYVRP_TWOOPT_H
+#define PYVRP_TWOOPT_H
 
 #include "LocalSearchOperator.h"
 
 /**
  * 2-OPT moves.
  *
  * Between routes: replaces U -> X and V -> Y by U -> Y and V -> X, if that is
  * an improving move. Within route: replaces U -> X and V -> Y by U -> V and
  * X -> Y, if that is an improving move.
  */
 class TwoOpt : public LocalSearchOperator<Node>
 {
     using LocalSearchOperator::LocalSearchOperator;
 
-    int
+    Cost
     evalWithinRoute(Node *U, Node *V, CostEvaluator const &costEvaluator) const;
 
-    int evalBetweenRoutes(Node *U,
-                          Node *V,
-                          CostEvaluator const &costEvaluator) const;
+    Cost evalBetweenRoutes(Node *U,
+                           Node *V,
+                           CostEvaluator const &costEvaluator) const;
 
     void applyWithinRoute(Node *U, Node *V) const;
 
     void applyBetweenRoutes(Node *U, Node *V) const;
 
 public:
-    int evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator) override;
+    Cost
+    evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator) override;
 
     void apply(Node *U, Node *V) const override;
 };
 
-#endif  // TWOOPT_H
+#endif  // PYVRP_TWOOPT_H
```

### Comparing `pyvrp-0.3.0/pyvrp/crossover/selective_route_exchange.py` & `pyvrp-0.4.1/pyvrp/crossover/selective_route_exchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Tuple
 
 from pyvrp._CostEvaluator import CostEvaluator
-from pyvrp._Individual import Individual
 from pyvrp._ProblemData import ProblemData
+from pyvrp._Solution import Solution
 from pyvrp._XorShift128 import XorShift128
 
 from ._selective_route_exchange import selective_route_exchange as _srex
 
 
 def selective_route_exchange(
-    parents: Tuple[Individual, Individual],
+    parents: Tuple[Solution, Solution],
     data: ProblemData,
     cost_evaluator: CostEvaluator,
     rng: XorShift128,
-) -> Individual:
+) -> Solution:
     """
     This crossover operator due to Nagata and Kobayashi (2010) combines routes
     from both parents to generate a new offspring solution. It does this by
     carefully selecting routes from the second parent that could be exchanged
     with routes from the first parent. After exchanging these routes, the
     resulting offspring solution is repaired using a greedy repair strategy.
 
@@ -30,15 +30,15 @@
     cost_evaluator
         The cost evaluator to be used during the greedy repair step.
     rng
         The random number generator to use.
 
     Returns
     -------
-    Individual
+    Solution
         A new offspring.
 
     References
     ----------
     .. [1] Nagata, Y., & Kobayashi, S. (2010). A Memetic Algorithm for the
            Pickup and Delivery Problem with Time Windows Using Selective Route
            Exchange Crossover. *Parallel Problem Solving from Nature*, PPSN XI,
```

### Comparing `pyvrp-0.3.0/pyvrp/educate/_Exchange.pyi` & `pyvrp-0.4.1/pyvrp/search/_Exchange.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/educate/__init__.py` & `pyvrp-0.4.1/pyvrp/search/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/educate/neighbourhood.py` & `pyvrp-0.4.1/pyvrp/search/neighbourhood.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/educate/tests/test_Exchange.py` & `pyvrp-0.4.1/pyvrp/search/tests/test_Exchange.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
-from pyvrp import Client, CostEvaluator, Individual, ProblemData, XorShift128
-from pyvrp.educate import LocalSearch, NeighbourhoodParams, compute_neighbours
-from pyvrp.educate._Exchange import (
+from pyvrp import (
+    Client,
+    CostEvaluator,
+    ProblemData,
+    Route,
+    Solution,
+    VehicleType,
+    XorShift128,
+)
+from pyvrp.search import LocalSearch, NeighbourhoodParams, compute_neighbours
+from pyvrp.search._Exchange import (
     Exchange10,
     Exchange11,
     Exchange20,
     Exchange21,
     Exchange22,
     Exchange30,
     Exchange31,
     Exchange32,
     Exchange33,
 )
-from pyvrp.tests.helpers import read
+from pyvrp.tests.helpers import make_heterogeneous, read
 
 
 @mark.parametrize(
     "operator",
     [
         Exchange11,
         Exchange21,
@@ -39,21 +47,21 @@
     rng = XorShift128(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(operator(data))
 
     single_route = list(range(1, data.num_clients + 1))
-    individual = Individual(data, [single_route])
-    improved_individual = ls.search(individual, cost_evaluator)
+    sol = Solution(data, [single_route])
+    improved_sol = ls.search(sol, cost_evaluator)
 
     # The new solution should strictly improve on our original solution.
-    assert_equal(improved_individual.num_routes(), 1)
-    current_cost = cost_evaluator.penalised_cost(individual)
-    improved_cost = cost_evaluator.penalised_cost(improved_individual)
+    assert_equal(improved_sol.num_routes(), 1)
+    current_cost = cost_evaluator.penalised_cost(sol)
+    improved_cost = cost_evaluator.penalised_cost(improved_sol)
     assert_(improved_cost < current_cost)
 
 
 @mark.parametrize(
     "operator",
     [
         Exchange10,
@@ -71,22 +79,22 @@
     rng = XorShift128(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(operator(data))
 
     single_route = list(range(1, data.num_clients + 1))
-    individual = Individual(data, [single_route])
-    improved_individual = ls.search(individual, cost_evaluator)
+    sol = Solution(data, [single_route])
+    improved_sol = ls.search(sol, cost_evaluator)
 
     # The new solution should strictly improve on our original solution, and
     # should use more routes.
-    assert_(improved_individual.num_routes() > 1)
-    current_cost = cost_evaluator.penalised_cost(individual)
-    improved_cost = cost_evaluator.penalised_cost(improved_individual)
+    assert_(improved_sol.num_routes() > 1)
+    current_cost = cost_evaluator.penalised_cost(sol)
+    improved_cost = cost_evaluator.penalised_cost(improved_sol)
     assert_(improved_cost < current_cost)
 
 
 @mark.parametrize(
     "operator",
     [
         Exchange22,
@@ -107,18 +115,18 @@
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(operator(data))
 
-    individual = Individual(data, [[1, 2], [3], [4]])
-    new_individual = ls.search(individual, cost_evaluator)
+    sol = Solution(data, [[1, 2], [3], [4]])
+    new_sol = ls.search(sol, cost_evaluator)
 
-    assert_equal(new_individual, individual)
+    assert_equal(new_sol, sol)
 
 
 @mark.parametrize("operator", [Exchange32, Exchange33])
 def test_cannot_exchange_when_segments_overlap(operator):
     """
     (3, 2)- and (3, 3)-exchange cannot exchange anything on a length-four
     single route solution: there's always overlap between the segments.
@@ -127,18 +135,18 @@
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(operator(data))
 
-    individual = Individual(data, [[1, 2, 3, 4]])
-    new_individual = ls.search(individual, cost_evaluator)
+    sol = Solution(data, [[1, 2, 3, 4]])
+    new_sol = ls.search(sol, cost_evaluator)
 
-    assert_equal(new_individual, individual)
+    assert_equal(new_sol, sol)
 
 
 def test_cannot_swap_adjacent_segments():
     """
     (2, 2)-exchange on a single route cannot swap adjacent segments, since
     that's already covered by (2, 0)-exchange.
     """
@@ -149,18 +157,18 @@
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(Exchange22(data))
 
     # An adjacent swap by (2, 2)-exchange could have created the single-route
     # solution [3, 4, 1, 2], which has a much lower cost. But that's not
     # allowed because adjacent swaps are not allowed.
-    individual = Individual(data, [[1, 2, 3, 4]])
-    new_individual = ls.search(individual, cost_evaluator)
+    sol = Solution(data, [[1, 2, 3, 4]])
+    new_sol = ls.search(sol, cost_evaluator)
 
-    assert_equal(new_individual, individual)
+    assert_equal(new_sol, sol)
 
 
 def test_swap_between_routes_OkSmall():
     """
     On the OkSmall example, (2, 1)-exchange should be able to swap parts of a
     two route solution, resulting in something better.
     """
@@ -168,21 +176,21 @@
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(Exchange21(data))
 
-    individual = Individual(data, [[1, 2], [3, 4]])
-    improved_individual = ls.search(individual, cost_evaluator)
-    expected = Individual(data, [[3, 4, 2], [1]])
-    assert_equal(improved_individual, expected)
+    sol = Solution(data, [[1, 2], [3, 4]])
+    improved_sol = ls.search(sol, cost_evaluator)
+    expected = Solution(data, [[3, 4, 2], [1]])
+    assert_equal(improved_sol, expected)
 
-    current_cost = cost_evaluator.penalised_cost(individual)
-    improved_cost = cost_evaluator.penalised_cost(improved_individual)
+    current_cost = cost_evaluator.penalised_cost(sol)
+    improved_cost = cost_evaluator.penalised_cost(improved_sol)
     assert_(improved_cost < current_cost)
 
 
 def test_relocate_after_depot_should_work():
     """
     This test exercises the bug identified in issue #142, involving a relocate
     action that should insert directly after the depot.
@@ -197,20 +205,20 @@
     # moving clients behind the depot of a route.
     neighbours = [[] for _ in range(data.num_clients + 1)]
     neighbours[2].append(1)
 
     ls = LocalSearch(data, rng, neighbours)
     ls.add_node_operator(Exchange10(data))
 
-    # This individual can be improved by moving 3 into its own route, that is,
+    # This solution can be improved by moving 3 into its own route, that is,
     # inserting it after the depot of an empty route. Before the bug was fixed,
     # (1, 0)-exchange never performed this move.
-    individual = Individual(data, [[1, 2, 3], [4]])
-    expected = Individual(data, [[1, 2], [3], [4]])
-    assert_equal(ls.search(individual, cost_evaluator), expected)
+    sol = Solution(data, [[1, 2, 3], [4]])
+    expected = Solution(data, [[1, 2], [3], [4]])
+    assert_equal(ls.search(sol, cost_evaluator), expected)
 
 
 def test_relocate_only_happens_when_distance_and_duration_allow_it():
     """
     Tests that (1, 0)-exchange checks the duration matrix for time-window
     feasibility before applying a move that improves the traveled distance.
     """
@@ -218,16 +226,15 @@
         Client(x=0, y=0, demand=0, service_duration=0, tw_early=0, tw_late=10),
         Client(x=1, y=0, demand=0, service_duration=0, tw_early=0, tw_late=5),
         Client(x=2, y=0, demand=0, service_duration=0, tw_early=0, tw_late=5),
     ]
 
     data = ProblemData(
         clients=clients,
-        nb_vehicles=1,
-        vehicle_cap=0,
+        vehicle_types=[VehicleType(0, 1)],
         distance_matrix=[  # distance-wise, the best route is 0 -> 1 -> 2 -> 0.
             [0, 1, 5],
             [5, 0, 1],
             [1, 5, 0],
         ],
         duration_matrix=[  # duration-wise, the best route is 0 -> 2 -> 1 -> 0.
             [0, 100, 2],
@@ -237,20 +244,53 @@
     )
 
     # We consider two solutions. The first is duration optimal, and overall the
     # only feasible solution. This solution can thus not be improved further.
     # We also consider a distance-optimal solution that is not feasible. Since
     # we have non-zero time warp penalty, this solution should be improved into
     # the duration optimal solution.
-    duration_optimal = Individual(data, [[2, 1]])
-    distance_optimal = Individual(data, [[1, 2]])
+    duration_optimal = Solution(data, [[2, 1]])
+    distance_optimal = Solution(data, [[1, 2]])
 
     assert_(distance_optimal.distance() < duration_optimal.distance())
     assert_(duration_optimal.time_warp() < distance_optimal.time_warp())
 
     cost_evaluator = CostEvaluator(1, 1)
     rng = XorShift128(seed=42)
     ls = LocalSearch(data, rng, compute_neighbours(data))
     ls.add_node_operator(Exchange10(data))
 
     assert_equal(ls.search(duration_optimal, cost_evaluator), duration_optimal)
     assert_equal(ls.search(distance_optimal, cost_evaluator), duration_optimal)
+
+
+def test_relocate_to_heterogeneous_empty_route():
+    """
+    This test asserts that a customer will be relocated to a non-empty route
+    with a different capacity even if there is another empty route in between.
+    """
+    vehicle_types = [VehicleType(cap, 1) for cap in [12, 5, 1, 3]]
+    data = make_heterogeneous(read("data/OkSmall.txt"), vehicle_types)
+    # Use a huge cost for load penalties to make other aspects irrelevant
+    cost_evaluator = CostEvaluator(100_000, 6)
+    rng = XorShift128(seed=42)
+
+    # This is a non-empty neighbourhood (so LS does not complain), but the only
+    # client moves allowed by it will not improve the initial solution created
+    # below. So the only improvements (1, 0)-exchange can make must come from
+    # moving clients behind the depot of a route.
+    neighbours = [[] for _ in range(data.num_clients + 1)]
+    neighbours[2].append(1)
+
+    ls = LocalSearch(data, rng, neighbours)
+    ls.add_node_operator(Exchange10(data))
+
+    # The initial solution has routes with loads [13, 5, 0, 0]
+    # with excess [1, 0, 0, 0]. Moving node 3 to route 4 will resolve all
+    # load penalties, but other moves would increase load penalties.
+    # Therefore, this requires moving to an empty route which is not the first.
+    sol = Solution(data, [Route(data, [1, 2, 3], 0), Route(data, [4], 1)])
+    expected = Solution(
+        data,
+        [Route(data, [1, 2], 0), Route(data, [4], 1), Route(data, [3], 3)],
+    )
+    assert_equal(ls.search(sol, cost_evaluator), expected)
```

### Comparing `pyvrp-0.3.0/pyvrp/educate/tests/test_LocalSearch.py` & `pyvrp-0.4.1/pyvrp/search/tests/test_LocalSearch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from numpy.testing import assert_, assert_equal, assert_raises
 from pytest import mark
 
-from pyvrp import CostEvaluator, Individual, XorShift128
-from pyvrp.educate import (
+from pyvrp import CostEvaluator, Route, Solution, VehicleType, XorShift128
+from pyvrp.search import (
     Exchange10,
     Exchange11,
     LocalSearch,
     NeighbourhoodParams,
     Neighbours,
     compute_neighbours,
 )
-from pyvrp.tests.helpers import read
+from pyvrp.search._LocalSearch import LocalSearch as cpp_LocalSearch
+from pyvrp.tests.helpers import make_heterogeneous, read
 
 
 def test_local_search_raises_when_there_are_no_operators():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
 
     ls = LocalSearch(data, rng, compute_neighbours(data))
-    individual = Individual.make_random(data, rng)
+    sol = Solution.make_random(data, rng)
 
     with assert_raises(RuntimeError):
-        ls.search(individual, cost_evaluator)
+        ls.search(sol, cost_evaluator)
 
     with assert_raises(RuntimeError):
-        ls.intensify(individual, cost_evaluator)
+        ls.intensify(sol, cost_evaluator)
 
 
 def test_local_search_raises_when_neighbourhood_structure_is_empty():
     data = read("data/OkSmall.txt")
     rng = XorShift128(seed=42)
 
     # Is completely empty neighbourhood, so there's nothing to do for the
@@ -90,17 +91,15 @@
     weight_wait_time: int,
     weight_time_warp: int,
     nb_granular: int,
     symmetric_proximity: bool,
     symmetric_neighbours: bool,
 ):
     data = read("data/RC208.txt", "solomon", round_func="trunc")
-
-    seed = 42
-    rng = XorShift128(seed=seed)
+    rng = XorShift128(seed=42)
 
     params = NeighbourhoodParams(nb_granular=1)
     prev_neighbours = compute_neighbours(data, params)
     ls = LocalSearch(data, rng, prev_neighbours)
 
     params = NeighbourhoodParams(
         weight_wait_time,
@@ -126,65 +125,124 @@
     assert_equal(ls.get_neighbours(), neighbours)
     neighbours[1] = []
     assert_(ls.get_neighbours() != neighbours)
 
 
 def test_reoptimize_changed_objective_timewarp_OkSmall():
     """
-    This test reproduces a bug where loadIndividual in LocalSearch.cpp would
+    This test reproduces a bug where loadSolution in LocalSearch.cpp would
     reset the timewarp for a route to 0 if the route was not changed. This
     would cause improving moves with a smaller timewarp not to be considered
     because the current cost doesn't count the current time warp.
     """
     data = read("data/OkSmall.txt")
     rng = XorShift128(seed=42)
 
-    individual = Individual(data, [[1, 2, 3, 4]])
+    sol = Solution(data, [[1, 2, 3, 4]])
 
     # We make neighbours only contain 1 -> 2, so the only feasible move
     # is changing [1, 2, 3, 4] into [2, 1, 3, 4] or moving one of the nodes
     # into its own route. Since those solutions have larger distance but
     # smaller time warp, they are considered improving moves with a
     # sufficiently large time warp penalty.
     neighbours: Neighbours = [[], [2], [], [], []]  # 1 -> 2 only
     ls = LocalSearch(data, rng, neighbours)
     ls.add_node_operator(Exchange10(data))
 
-    # With 0 timewarp penalty, the individual should not change since
+    # With 0 timewarp penalty, the solution should not change since
     # the solution [2, 1, 3, 4] has larger distance
-    improved_indiv = ls.search(individual, CostEvaluator(0, 0))
-    assert_equal(individual, improved_indiv)
+    improved_sol = ls.search(sol, CostEvaluator(0, 0))
+    assert_equal(sol, improved_sol)
 
     # Now doing it again with a large TW penalty, we must find the alternative
     # solution
     # (previously this was not the case since due to caching the current TW was
     # computed as being zero, causing the move to be evaluated as worse)
     cost_evaluator_tw = CostEvaluator(0, 1000)
-    improved_indiv = ls.search(individual, cost_evaluator_tw)
-    improved_cost = cost_evaluator_tw.penalised_cost(improved_indiv)
-    assert_(improved_cost < cost_evaluator_tw.penalised_cost(individual))
+    improved_sol = ls.search(sol, cost_evaluator_tw)
+    improved_cost = cost_evaluator_tw.penalised_cost(improved_sol)
+    assert_(improved_cost < cost_evaluator_tw.penalised_cost(sol))
 
 
 def test_prize_collecting():
     """
     Tests that local search works on a small prize-collecting instance.
     """
     data = read("data/p06-2-50.vrp", round_func="dimacs")
     rng = XorShift128(seed=42)
     cost_evaluator = CostEvaluator(1, 1)
 
-    individual = Individual.make_random(data, rng)
-    individual_cost = cost_evaluator.penalised_cost(individual)
+    sol = Solution.make_random(data, rng)
+    sol_cost = cost_evaluator.penalised_cost(sol)
 
     # Random solutions are complete...
-    assert_equal(individual.num_clients(), data.num_clients)
+    assert_equal(sol.num_clients(), data.num_clients)
 
     ls = LocalSearch(data, rng, compute_neighbours(data))
     ls.add_node_operator(Exchange10(data))  # relocate
     ls.add_node_operator(Exchange11(data))  # swap
 
-    improved = ls.search(individual, cost_evaluator)
+    improved = ls.search(sol, cost_evaluator)
     improved_cost = cost_evaluator.penalised_cost(improved)
 
     # ...but an optimised prize-collecting solution is likely not complete.
-    assert_(improved.num_clients() < individual.num_clients())
-    assert_(improved_cost < individual_cost)
+    assert_(improved.num_clients() < sol.num_clients())
+    assert_(improved_cost < sol_cost)
+
+
+def test_cpp_shuffle_results_in_different_solution():
+    data = read("data/RC208.txt", "solomon", round_func="trunc")
+    rng = XorShift128(seed=42)
+
+    ls = cpp_LocalSearch(data, compute_neighbours(data))
+    ls.add_node_operator(Exchange10(data))
+    ls.add_node_operator(Exchange11(data))
+
+    cost_evaluator = CostEvaluator(1, 1)
+    sol = Solution.make_random(data, rng)
+
+    # LocalSearch::search is deterministic, so two calls with the same base
+    # solution should result in the same improved solution.
+    improved1 = ls.search(sol, cost_evaluator)
+    improved2 = ls.search(sol, cost_evaluator)
+    assert_(improved1 == improved2)
+
+    # But the shuffle method changes the order in which moves are evaluated,
+    # which should result in a very different search trajectory.
+    ls.shuffle(rng)
+    improved3 = ls.search(sol, cost_evaluator)
+    assert_(improved3 != improved1)
+
+
+def test_route_vehicle_types_are_preserved_for_locally_optimal_solutions():
+    # This test tests that we will preserve vehicle types
+    data = read("data/RC208.txt", "solomon", round_func="trunc")
+    rng = XorShift128(seed=42)
+
+    neighbours = compute_neighbours(data)
+    ls = cpp_LocalSearch(data, neighbours)
+    ls.add_node_operator(Exchange10(data))
+    ls.add_node_operator(Exchange11(data))
+
+    cost_evaluator = CostEvaluator(1, 1)
+    sol = Solution.make_random(data, rng)
+
+    # LocalSearch::search is deterministic, so two calls with the same base
+    # solution should result in the same improved solution.
+    improved = ls.search(sol, cost_evaluator)
+
+    # Now make the instance heterogeneous and update the local search
+    data = make_heterogeneous(
+        data, [VehicleType(1000, 25), VehicleType(1000, 25)]
+    )
+    ls = cpp_LocalSearch(data, neighbours)
+    ls.add_node_operator(Exchange10(data))
+    ls.add_node_operator(Exchange11(data))
+
+    # Update the improved (locally optimal) solution with vehicles of type 1
+    routes = [Route(data, r.visits(), 1) for r in improved.get_routes()]
+    improved = Solution(data, routes)
+
+    # Doing the search should not find any further improvements thus not change
+    # the solution, especially not change the vehicle types
+    further_improved = ls.search(improved, cost_evaluator)
+    assert_equal(further_improved, improved)
```

### Comparing `pyvrp-0.3.0/pyvrp/educate/tests/test_MoveTwoClientsReversed.py` & `pyvrp-0.4.1/pyvrp/search/tests/test_MoveTwoClientsReversed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, Individual, XorShift128
-from pyvrp.educate import (
+from pyvrp import CostEvaluator, Solution, XorShift128
+from pyvrp.search import (
     LocalSearch,
     MoveTwoClientsReversed,
     NeighbourhoodParams,
     compute_neighbours,
 )
 from pyvrp.tests.helpers import read
 
@@ -20,34 +20,34 @@
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(MoveTwoClientsReversed(data))
 
-    individual = Individual(data, [[1, 4, 2, 3]])
-    improved_individual = ls.search(individual, cost_evaluator)
+    sol = Solution(data, [[1, 4, 2, 3]])
+    improved_sol = ls.search(sol, cost_evaluator)
 
     # The new solution should strictly improve on our original solution.
-    assert_equal(improved_individual.num_routes(), 1)
-    current_cost = cost_evaluator.penalised_cost(individual)
-    improved_cost = cost_evaluator.penalised_cost(improved_individual)
+    assert_equal(improved_sol.num_routes(), 1)
+    current_cost = cost_evaluator.penalised_cost(sol)
+    improved_cost = cost_evaluator.penalised_cost(improved_sol)
     assert_(improved_cost < current_cost)
 
     # (2, 3) was inserted after 1 as 1 -> 3 -> 2 -> 4. Then (1, 3) got inserted
     # after 4 as 2 -> 4 -> 3 -> 1.
-    expected = Individual(data, [[2, 4, 3, 1]])
-    assert_equal(improved_individual, expected)
+    expected = Solution(data, [[2, 4, 3, 1]])
+    assert_equal(improved_sol, expected)
 
     # These two-route solutions can all be created by MoveTwoClientsReversed
     # from the returned solution. So they must have a cost that's at best equal
     # to the returned solution's cost.
     for routes in ([[3, 1], [4, 2]], [[2, 1], [3, 4]], [[2, 4], [1, 3]]):
-        other = Individual(data, routes)
-        improved_cost = cost_evaluator.penalised_cost(improved_individual)
+        other = Solution(data, routes)
+        improved_cost = cost_evaluator.penalised_cost(improved_sol)
         other_cost = cost_evaluator.penalised_cost(other)
         assert_(improved_cost <= other_cost)
 
 
 @mark.parametrize("seed", [2643, 2742, 2941, 3457, 4299, 4497, 6178, 6434])
 def test_RC208_instance(seed: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
@@ -55,14 +55,14 @@
     rng = XorShift128(seed=seed)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(MoveTwoClientsReversed(data))
 
     single_route = list(range(1, data.num_clients + 1))
-    individual = Individual(data, [single_route])
-    improved_individual = ls.search(individual, cost_evaluator)
+    sol = Solution(data, [single_route])
+    improved_sol = ls.search(sol, cost_evaluator)
 
     # The new solution should strictly improve on our original solution.
-    current_cost = cost_evaluator.penalised_cost(individual)
-    improved_cost = cost_evaluator.penalised_cost(improved_individual)
+    current_cost = cost_evaluator.penalised_cost(sol)
+    improved_cost = cost_evaluator.penalised_cost(improved_sol)
     assert_(improved_cost < current_cost)
```

### Comparing `pyvrp-0.3.0/pyvrp/educate/tests/test_RelocateStar.py` & `pyvrp-0.4.1/pyvrp/search/tests/test_RelocateStar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, Individual, XorShift128
-from pyvrp.educate import (
+from pyvrp import CostEvaluator, Solution, XorShift128
+from pyvrp.search import (
     Exchange10,
     LocalSearch,
     NeighbourhoodParams,
     RelocateStar,
     compute_neighbours,
 )
 from pyvrp.tests.helpers import read
@@ -25,26 +25,26 @@
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
 
     ls.add_node_operator(Exchange10(data))
     ls.add_route_operator(RelocateStar(data))
 
     for _ in range(10):  # repeat a few times to really make sure
-        individual = Individual.make_random(data, rng)
-        exchange_individual = ls.search(individual, cost_evaluator)
-        relocate_individual = ls.intensify(
-            exchange_individual, cost_evaluator, overlap_tolerance_degrees=360
+        sol = Solution.make_random(data, rng)
+        exchange_sol = ls.search(sol, cost_evaluator)
+        relocate_sol = ls.intensify(
+            exchange_sol, cost_evaluator, overlap_tolerance_degrees=360
         )
 
         # RELOCATE* applies the best (1, 0)-exchange moves between routes. But
         # when the granular neighbourhood covers the entire client space, that
         # best move has already been evaluated and applied by regular (1,0)
-        # exchange. Thus, at this point the individual cannot be improved
+        # exchange. Thus, at this point the solution cannot be improved
         # further by RELOCATE*.
-        assert_equal(relocate_individual, exchange_individual)
+        assert_equal(relocate_sol, exchange_sol)
 
 
 @mark.parametrize("size", [2, 5, 10])
 def test_exchange10_and_relocate_star_differ_small_neighbourhoods(size: int):
     """
     This test restricts the sizes of the granular neighbourhoods, so now
     (1, 0)-Exchange and RELOCATE* should start to differ.
@@ -55,23 +55,23 @@
 
     nb_params = NeighbourhoodParams(nb_granular=size)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
 
     ls.add_node_operator(Exchange10(data))
     ls.add_route_operator(RelocateStar(data))
 
-    individual = Individual.make_random(data, rng)
-    exchange_individual = ls.search(individual, cost_evaluator)
-    relocate_individual = ls.intensify(
-        exchange_individual, cost_evaluator, overlap_tolerance_degrees=360
+    sol = Solution.make_random(data, rng)
+    exchange_sol = ls.search(sol, cost_evaluator)
+    relocate_sol = ls.intensify(
+        exchange_sol, cost_evaluator, overlap_tolerance_degrees=360
     )
 
-    # The original individual was not that great, so after (1, 0)-Exchange it
+    # The original solution was not that great, so after (1, 0)-Exchange it
     # should have improved. But that operator is restricted by the size of the
     # granular neighbourhood, which limits the number of operators. RELOCATE*
     # overcomes some of that, and as a result, should be able to improve the
     # solution further.
-    current_cost = cost_evaluator.penalised_cost(individual)
-    exchange_cost = cost_evaluator.penalised_cost(exchange_individual)
-    relocate_cost = cost_evaluator.penalised_cost(relocate_individual)
+    current_cost = cost_evaluator.penalised_cost(sol)
+    exchange_cost = cost_evaluator.penalised_cost(exchange_sol)
+    relocate_cost = cost_evaluator.penalised_cost(relocate_sol)
     assert_(current_cost > exchange_cost)
     assert_(exchange_cost > relocate_cost)
```

### Comparing `pyvrp-0.3.0/pyvrp/educate/tests/test_SwapStar.py` & `pyvrp-0.4.1/pyvrp/search/tests/test_SwapStar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, Individual, XorShift128
-from pyvrp.educate import (
+from pyvrp import CostEvaluator, Solution, XorShift128
+from pyvrp.search import (
     Exchange11,
     LocalSearch,
     NeighbourhoodParams,
     SwapStar,
     compute_neighbours,
 )
 from pyvrp.tests.helpers import read
@@ -28,27 +28,27 @@
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
 
     ls.add_node_operator(Exchange11(data))
     ls.add_route_operator(SwapStar(data))
 
     for _ in range(10):  # repeat a few times to really make sure
-        individual = Individual.make_random(data, rng)
+        sol = Solution.make_random(data, rng)
 
-        swap_individual = ls.search(individual, cost_evaluator)
-        swap_star_individual = ls.intensify(
-            swap_individual, cost_evaluator, overlap_tolerance_degrees=360
+        swap_sol = ls.search(sol, cost_evaluator)
+        swap_star_sol = ls.intensify(
+            swap_sol, cost_evaluator, overlap_tolerance_degrees=360
         )
 
         # The regular swap operator should have been able to improve the random
-        # individual. After swap gets stuck, SWAP* should still be able to
-        # further improve the individual.
-        current_cost = cost_evaluator.penalised_cost(individual)
-        swap_cost = cost_evaluator.penalised_cost(swap_individual)
-        swap_star_cost = cost_evaluator.penalised_cost(swap_star_individual)
+        # solution. After swap gets stuck, SWAP* should still be able to
+        # further improve the solution.
+        current_cost = cost_evaluator.penalised_cost(sol)
+        swap_cost = cost_evaluator.penalised_cost(swap_sol)
+        swap_star_cost = cost_evaluator.penalised_cost(swap_star_sol)
         assert_(swap_cost < current_cost)
         assert_(swap_star_cost < swap_cost)
 
 
 @mark.parametrize("seed", [2643, 2742, 2941, 3457, 4299, 4497, 6178, 6434])
 def test_swap_star_on_RC208_instance(seed: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
@@ -58,18 +58,18 @@
     ls = LocalSearch(data, rng, compute_neighbours(data))
     ls.add_route_operator(SwapStar(data))
 
     # Make an initial solution that consists of two routes, by randomly
     # splitting the single-route solution.
     route = list(range(1, data.num_clients + 1))
     split = rng.randint(data.num_clients)
-    individual = Individual(data, [route[:split], route[split:]])
-    improved_individual = ls.intensify(
-        individual, cost_evaluator, overlap_tolerance_degrees=360
+    sol = Solution(data, [route[:split], route[split:]])
+    improved_sol = ls.intensify(
+        sol, cost_evaluator, overlap_tolerance_degrees=360
     )
 
     # The new solution should strictly improve on our original solution, but
     # cannot use more routes since SWAP* does not create routes.
-    assert_equal(improved_individual.num_routes(), 2)
-    current_cost = cost_evaluator.penalised_cost(individual)
-    improved_cost = cost_evaluator.penalised_cost(improved_individual)
+    assert_equal(improved_sol.num_routes(), 2)
+    current_cost = cost_evaluator.penalised_cost(sol)
+    improved_cost = cost_evaluator.penalised_cost(improved_sol)
     assert_(improved_cost < current_cost)
```

### Comparing `pyvrp-0.3.0/pyvrp/educate/tests/test_neighbourhood.py` & `pyvrp-0.4.1/pyvrp/search/tests/test_neighbourhood.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Set
 
 import numpy as np
 from numpy.testing import assert_, assert_equal, assert_raises
 from pytest import mark
 
-from pyvrp.educate import NeighbourhoodParams, compute_neighbours
+from pyvrp.search import NeighbourhoodParams, compute_neighbours
 from pyvrp.tests.helpers import read
 
 
 @mark.parametrize(
     "weight_wait_time,"
     "weight_time_warp,"
     "nb_granular,"
```

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_coordinates.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_diversity.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_diversity.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_instance.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_instance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_objectives.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_objectives.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_result.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_result.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_route_schedule.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_route_schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,20 @@
         Title to add to the plot.
     ax, optional
         Axes object to draw the plot on. One will be created if not provided.
     """
     if not ax:
         _, ax = plt.subplots()
 
+    vehicle_type = data.vehicle_type(route.vehicle_type())
     depot = data.client(0)  # For readability, define variable
     horizon = depot.tw_late - depot.tw_early
 
     # Initialise tracking variables
-    t = 0
-    wait_time = 0
-    time_warp = 0
+    t = route.release_time()
     drive_time = 0
     serv_time = 0
     dist = 0
     load = sum([data.client(idx).demand for idx in route])
     slack = horizon
 
     # Traces and objects used for plotting
@@ -84,20 +83,18 @@
         t += delta_time
         drive_time += delta_time
         dist += delta_dist
 
         add_traces(dist, t, drive_time, serv_time, load)
 
         if t < stop.tw_early:
-            wait_time += stop.tw_early - t
             t = stop.tw_early
 
         slack = min(slack, stop.tw_late - t)
         if t > stop.tw_late:
-            time_warp += t - stop.tw_late
             timewarp_lines.append(((dist, t), (dist, stop.tw_late)))
             t = stop.tw_late
 
         load -= stop.demand
 
         add_traces(dist, t, drive_time, serv_time, load)
 
@@ -147,20 +144,20 @@
     )
 
     # Plot remaining load on second axis
     twin1 = ax.twinx()
     twin1.fill_between(
         *zip(*trace_load), color="black", alpha=0.1, label="Load in vehicle"
     )
-    twin1.set_ylim([0, data.vehicle_capacity])
+    twin1.set_ylim([0, vehicle_type.capacity])
 
     # Set labels, legends and title
     ax.set_xlabel("Distance")
     ax.set_ylabel("Time")
-    twin1.set_ylabel(f"Load (capacity = {data.vehicle_capacity})")
+    twin1.set_ylabel(f"Load (capacity = {vehicle_type.capacity:.0f})")
 
     if legend:
         twin1.legend(loc="upper right")
         ax.legend(loc="upper left")
 
     if title:
         ax.set_title(title)
```

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_runtimes.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_runtimes.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_solution.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_solution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from pyvrp import Individual, ProblemData
+from pyvrp import ProblemData, Solution
 
 
 def plot_solution(
-    solution: Individual,
+    solution: Solution,
     data: ProblemData,
     plot_customers: bool = False,
     ax: Optional[plt.Axes] = None,
 ):
     """
     Plots the given solution.
 
@@ -35,26 +35,25 @@
     y_coords = np.array([data.client(client).y for client in range(dim)])
 
     # This is the depot
     kwargs = dict(c="tab:red", marker="*", zorder=3, s=500)
     ax.scatter(x_coords[0], y_coords[0], label="Depot", **kwargs)
 
     for idx, route in enumerate(solution.get_routes(), 1):
-        if route:
-            x = x_coords[route]
-            y = y_coords[route]
-
-            # Coordinates of customers served by this route.
-            if len(route) == 1 or plot_customers:
-                ax.scatter(x, y, label=f"Route {idx}", zorder=3, s=75)
-            ax.plot(x, y)
-
-            # Edges from and to the depot, very thinly dashed.
-            kwargs = dict(ls=(0, (5, 15)), linewidth=0.25, color="grey")
-            ax.plot([x_coords[0], x[0]], [y_coords[0], y[0]], **kwargs)
-            ax.plot([x[-1], x_coords[0]], [y[-1], y_coords[0]], **kwargs)
+        x = x_coords[route]
+        y = y_coords[route]
+
+        # Coordinates of customers served by this route.
+        if len(route) == 1 or plot_customers:
+            ax.scatter(x, y, label=f"Route {idx}", zorder=3, s=75)
+        ax.plot(x, y)
+
+        # Edges from and to the depot, very thinly dashed.
+        kwargs = dict(ls=(0, (5, 15)), linewidth=0.25, color="grey")
+        ax.plot([x_coords[0], x[0]], [y_coords[0], y[0]], **kwargs)
+        ax.plot([x[-1], x_coords[0]], [y[-1], y_coords[0]], **kwargs)
 
     ax.grid(color="grey", linestyle="solid", linewidth=0.2)
 
     ax.set_title("Solution")
     ax.set_aspect("equal", "datalim")
     ax.legend(frameon=False, ncol=2)
```

### Comparing `pyvrp-0.3.0/pyvrp/plotting/plot_time_windows.py` & `pyvrp-0.4.1/pyvrp/plotting/plot_time_windows.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png` & `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png` & `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png` & `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png` & `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png` & `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/plotting/tests/test_plotting.py` & `pyvrp-0.4.1/pyvrp/plotting/tests/test_plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from matplotlib.testing.decorators import image_comparison as img_comp
 from numpy.testing import assert_, assert_raises
 
 from pyvrp import (
     CostEvaluator,
-    Individual,
     Population,
     PopulationParams,
+    Solution,
     XorShift128,
     plotting,
 )
 from pyvrp.Result import Result
 from pyvrp.Statistics import Statistics
 from pyvrp.diversity import broken_pairs_distance
 from pyvrp.exceptions import StatisticsNotCollectedError
 from pyvrp.tests.helpers import make_random_solutions, read, read_solution
 
 IMG_KWARGS = dict(remove_text=True, tol=2, extensions=["png"], style="mpl20")
 
 
 def test_plotting_methods_raise_when_no_stats_available():
     data = read("data/OkSmall.txt")
-    individual = Individual(data, [[1, 2, 3, 4]])
-    res = Result(individual, Statistics(), 0, 0.0)
+    sol = Solution(data, [[1, 2, 3, 4]])
+    res = Result(sol, Statistics(), 0, 0.0)
 
     assert_(not res.has_statistics())
 
     with assert_raises(StatisticsNotCollectedError):
         plotting.plot_diversity(res)
 
     with assert_raises(StatisticsNotCollectedError):
@@ -41,58 +41,59 @@
 
 
 @img_comp(["plot_solution", "plot_solution_with_customers"], **IMG_KWARGS)
 def test_plot_solution():
     data = read("data/RC208.txt", "solomon", round_func="trunc")
     bks = read_solution("data/RC208.sol")
 
-    individual = Individual(data, bks)
+    sol = Solution(data, bks)
 
-    plotting.plot_solution(individual, data)
-    plotting.plot_solution(individual, data, plot_customers=True)
+    plotting.plot_solution(sol, data)
+    plotting.plot_solution(sol, data, plot_customers=True)
 
 
 @img_comp(["plot_result"], **IMG_KWARGS)
 def test_plot_result():
     num_iterations = 100
 
     data = read("data/RC208.txt", "solomon", round_func="trunc")
     bks = read_solution("data/RC208.sol")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
 
     params = PopulationParams()
     pop = Population(broken_pairs_distance, params=params)
 
-    for indiv in make_random_solutions(params.min_pop_size, data, rng):
-        pop.add(indiv, cost_evaluator)
+    for sol in make_random_solutions(params.min_pop_size, data, rng):
+        pop.add(sol, cost_evaluator)
 
     stats = Statistics()
 
     for i in range(num_iterations):
         if i == num_iterations // 2:
             # Make sure we insert a feasible solution
-            individual = Individual(data, bks)
+            sol = Solution(data, bks)
         else:
-            individual = Individual.make_random(data, rng)
+            sol = Solution.make_random(data, rng)
 
-        pop.add(individual, cost_evaluator)
+        pop.add(sol, cost_evaluator)
         stats.collect_from(pop, cost_evaluator)
 
         # Hacky to produce deterministic result
         stats.runtimes[-1] = i % 3
 
-    res = Result(Individual(data, bks), stats, num_iterations, 0.0)
+    res = Result(Solution(data, bks), stats, num_iterations, 0.0)
     plotting.plot_result(res, data)
 
 
 @img_comp(["plot_instance"], **IMG_KWARGS)
 def test_plot_instance():
     data = read("data/RC208.txt", "solomon", round_func="trunc")
     plotting.plot_instance(data)
 
 
 @img_comp(["plot_route_schedule"], **IMG_KWARGS)
 def test_plot_route_schedule():
     data = read("data/RC208.txt", "solomon", round_func="trunc")
     bks = read_solution("data/RC208.sol")
-    plotting.plot_route_schedule(data, bks[0])
+    sol = Solution(data, bks)
+    plotting.plot_route_schedule(data, sol.get_routes()[0])
```

### Comparing `pyvrp-0.3.0/pyvrp/read.py` & `pyvrp-0.4.1/pyvrp/read.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import functools
 import pathlib
 from numbers import Number
 from typing import Callable, Dict, List, Union
+from warnings import warn
 
 import numpy as np
 import vrplib
 
-from ._ProblemData import Client, ProblemData
+from pyvrp.constants import MAX_USER_VALUE
+from pyvrp.exceptions import ScalingWarning
+
+from ._ProblemData import Client, ProblemData, VehicleType
 
 _Routes = List[List[int]]
 _RoundingFunc = Callable[[np.ndarray], np.ndarray]
 
 _INT_MAX = np.iinfo(np.int32).max
 
 
@@ -126,14 +130,19 @@
     else:
         # No time window data. So the time window component is not relevant,
         # and we set all time-related fields to zero.
         durations = np.zeros_like(distances)
         service_times = np.zeros(dimension, dtype=int)
         time_windows = np.zeros((dimension, 2), dtype=int)
 
+    if "release_time" in instance:
+        release_times: np.ndarray = round_func(instance["release_time"])
+    else:
+        release_times = np.zeros(dimension, dtype=int)
+
     prizes = round_func(instance.get("prize", np.zeros(dimension, dtype=int)))
 
     # Checks
     if len(depots) != 1 or depots[0] != 0:
         raise ValueError(
             "Source file should contain single depot with index 1 "
             + "(depot index should be 0 after subtracting offset 1)"
@@ -144,35 +153,46 @@
 
     if time_windows[0, 0] != 0:
         raise ValueError("Depot start of time window must be 0")
 
     if service_times[0] != 0:
         raise ValueError("Depot service duration must be 0")
 
+    if release_times[0] != 0:
+        raise ValueError("Depot release time must be 0")
+
     if (time_windows[:, 0] > time_windows[:, 1]).any():
         raise ValueError("Time window cannot start after end")
 
     clients = [
         Client(
             coords[idx][0],  # x
             coords[idx][1],  # y
             demands[idx],
             service_times[idx],
             time_windows[idx][0],  # TW early
             time_windows[idx][1],  # TW late
+            release_times[idx],
             prizes[idx],
             np.isclose(prizes[idx], 0),  # required only when prize is zero
         )
         for idx in range(dimension)
     ]
+    vehicle_types = [VehicleType(capacity, num_vehicles)]
+
+    if max(distances.max(), durations.max()) > MAX_USER_VALUE:
+        msg = """
+        The maximum distance or duration value is very large. This might
+        impact numerical stability. Consider rescaling your input data.
+        """
+        warn(msg, ScalingWarning)
 
     return ProblemData(
         clients,
-        num_vehicles,
-        capacity,
+        vehicle_types,
         distances,
         durations,
     )
 
 
 def read_solution(where: Union[str, pathlib.Path]) -> _Routes:
     """
```

### Comparing `pyvrp-0.3.0/pyvrp/show_versions.py` & `pyvrp-0.4.1/pyvrp/show_versions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/stop/MaxRuntime.py` & `pyvrp-0.4.1/pyvrp/stop/MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/stop/NoImprovement.py` & `pyvrp-0.4.1/pyvrp/stop/NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/stop/StoppingCriterion.py` & `pyvrp-0.4.1/pyvrp/stop/StoppingCriterion.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/stop/TimedNoImprovement.py` & `pyvrp-0.4.1/pyvrp/stop/TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/stop/tests/test_MaxIterations.py` & `pyvrp-0.4.1/pyvrp/stop/tests/test_MaxIterations.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/stop/tests/test_MaxRuntime.py` & `pyvrp-0.4.1/pyvrp/stop/tests/test_MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/stop/tests/test_NoImprovement.py` & `pyvrp-0.4.1/pyvrp/stop/tests/test_NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/stop/tests/test_TimedNoImprovement.py` & `pyvrp-0.4.1/pyvrp/stop/tests/test_TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/data/E-n22-k4.txt` & `pyvrp-0.4.1/pyvrp/tests/data/E-n22-k4.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/data/EdgeWeightsNoExplicit.txt` & `pyvrp-0.4.1/pyvrp/tests/data/EdgeWeightsNoExplicit.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt` & `pyvrp-0.4.1/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/data/OkSmall.txt` & `pyvrp-0.4.1/pyvrp/tests/data/OkSmall.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/data/OkSmallGreedyRepair.txt` & `pyvrp-0.4.1/pyvrp/tests/data/OkSmallGreedyRepair.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/data/OkSmallPrizes.txt` & `pyvrp-0.4.1/pyvrp/tests/data/OkSmallPrizes.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/data/RC208.txt` & `pyvrp-0.4.1/pyvrp/tests/data/RC208.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/data/p06-2-50.vrp` & `pyvrp-0.4.1/pyvrp/tests/data/p06-2-50.vrp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_CostEvaluator.py` & `pyvrp-0.4.1/pyvrp/tests/test_CostEvaluator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,135 @@
 import numpy as np
-from numpy.testing import assert_, assert_allclose, assert_equal
+from numpy.testing import assert_, assert_allclose
 from pytest import mark
 
-from pyvrp import CostEvaluator, Individual
+from pyvrp import CostEvaluator, Solution
 from pyvrp.tests.helpers import read
 
 
 def test_load_penalty():
     cost_evaluator = CostEvaluator(2, 1)
 
-    assert_equal(cost_evaluator.load_penalty(0, 1), 0)  # below capacity
-    assert_equal(cost_evaluator.load_penalty(1, 1), 0)  # at capacity
+    assert_allclose(cost_evaluator.load_penalty(0, 1), 0)  # below capacity
+    assert_allclose(cost_evaluator.load_penalty(1, 1), 0)  # at capacity
 
     # Penalty per unit excess capacity is 2
     # 1 unit above capacity
-    assert_equal(cost_evaluator.load_penalty(2, 1), 2)
+    assert_allclose(cost_evaluator.load_penalty(2, 1), 2)
     # 2 units above capacity
-    assert_equal(cost_evaluator.load_penalty(3, 1), 4)
+    assert_allclose(cost_evaluator.load_penalty(3, 1), 4)
 
     # Penalty per unit excess capacity is 4
     cost_evaluator = CostEvaluator(4, 1)
 
     # 1 unit above capacity
-    assert_equal(cost_evaluator.load_penalty(2, 1), 4)
+    assert_allclose(cost_evaluator.load_penalty(2, 1), 4)
     # 2 units above capacity
-    assert_equal(cost_evaluator.load_penalty(3, 1), 8)
+    assert_allclose(cost_evaluator.load_penalty(3, 1), 8)
 
 
 @mark.parametrize("capacity", [5, 15, 29, 51, 103])
 def test_load_penalty_always_zero_when_below_capacity(capacity: int):
     load_penalty = 2
     cost_evaluator = CostEvaluator(load_penalty, 1)
 
     for load in range(capacity):  # all below capacity
-        assert_equal(cost_evaluator.load_penalty(load, capacity), 0)
+        assert_allclose(cost_evaluator.load_penalty(load, capacity), 0)
 
     # at capacity
-    assert_equal(cost_evaluator.load_penalty(capacity, capacity), 0)
+    assert_allclose(cost_evaluator.load_penalty(capacity, capacity), 0)
     # above capacity
-    assert_equal(
+    assert_allclose(
         cost_evaluator.load_penalty(capacity + 1, capacity), load_penalty
     )
-    assert_equal(
+    assert_allclose(
         cost_evaluator.load_penalty(capacity + 2, capacity), 2 * load_penalty
     )
 
 
 def test_tw_penalty():
     cost_evaluator = CostEvaluator(1, 2)
 
     # Penalty per unit time warp is 2
-    assert_equal(cost_evaluator.tw_penalty(0), 0)
-    assert_equal(cost_evaluator.tw_penalty(1), 2)
-    assert_equal(cost_evaluator.tw_penalty(2), 4)
+    assert_allclose(cost_evaluator.tw_penalty(0), 0)
+    assert_allclose(cost_evaluator.tw_penalty(1), 2)
+    assert_allclose(cost_evaluator.tw_penalty(2), 4)
 
     cost_evaluator = CostEvaluator(1, 4)
 
     # Penalty per unit excess capacity is now 4
-    assert_equal(cost_evaluator.tw_penalty(0), 0)
-    assert_equal(cost_evaluator.tw_penalty(1), 4)
-    assert_equal(cost_evaluator.tw_penalty(2), 8)
+    assert_allclose(cost_evaluator.tw_penalty(0), 0)
+    assert_allclose(cost_evaluator.tw_penalty(1), 4)
+    assert_allclose(cost_evaluator.tw_penalty(2), 8)
 
 
 def test_cost():
     data = read("data/OkSmall.txt")
     default_cost_evaluator = CostEvaluator()
     cost_evaluator = CostEvaluator(20, 6)
 
-    # Feasible individual
-    feas_indiv = Individual(data, [[1, 2], [3], [4]])
-    distance = feas_indiv.distance()
-
-    assert_equal(cost_evaluator.cost(feas_indiv), distance)
-    assert_equal(default_cost_evaluator.cost(feas_indiv), distance)
-
-    # Infeasible individual
-    infeas_indiv = Individual(data, [[1, 2, 3, 4]])
-
-    # C++ code represents infinity as UINT_MAX
-    INFEAS_COST = np.iinfo(np.uint32).max
-    assert_equal(cost_evaluator.cost(infeas_indiv), INFEAS_COST)
-    assert_equal(default_cost_evaluator.cost(infeas_indiv), INFEAS_COST)
+    feas_sol = Solution(data, [[1, 2], [3], [4]])  # feasible solution
+    distance = feas_sol.distance()
+
+    assert_allclose(cost_evaluator.cost(feas_sol), distance)
+    assert_allclose(default_cost_evaluator.cost(feas_sol), distance)
+
+    infeas_sol = Solution(data, [[1, 2, 3, 4]])  # infeasible solution
+    assert_(not infeas_sol.is_feasible())
+
+    # The C++ code represents infinity using a relevant maximal value, which
+    # depends on the precision type (double or integer).
+    if isinstance(distance, int):
+        INFEAS_COST = np.iinfo(np.int32).max
+    else:
+        INFEAS_COST = np.finfo(np.float64).max
+
+    assert_allclose(cost_evaluator.cost(infeas_sol), INFEAS_COST)
+    assert_allclose(default_cost_evaluator.cost(infeas_sol), INFEAS_COST)
 
 
 def test_cost_with_prizes():
     data = read("data/p06-2-50.vrp", round_func="dimacs")
     cost_evaluator = CostEvaluator(1, 1)
 
-    indiv = Individual(data, [[1, 2], [3, 4, 5]])
-    cost = cost_evaluator.cost(indiv)
-    assert_(indiv.is_feasible())
+    sol = Solution(data, [[1, 2], [3, 4, 5]])
+    cost = cost_evaluator.cost(sol)
+    assert_(sol.is_feasible())
 
     prizes = [data.client(idx).prize for idx in range(data.num_clients + 1)]
     collected = sum(prizes[:6])
     uncollected = sum(prizes) - collected
 
     assert_allclose(prizes[0], 0)
-    assert_allclose(indiv.prizes(), collected)
-    assert_allclose(indiv.uncollected_prizes(), uncollected)
-    assert_allclose(indiv.distance() + indiv.uncollected_prizes(), cost)
+    assert_allclose(sol.prizes(), collected)
+    assert_allclose(sol.uncollected_prizes(), uncollected)
+    assert_allclose(sol.distance() + sol.uncollected_prizes(), cost)
 
 
 def test_penalised_cost():
     data = read("data/OkSmall.txt")
     penalty_capacity = 20
     penalty_tw = 6
-    default_cost_evaluator = CostEvaluator()
+    default_evaluator = CostEvaluator()
     cost_evaluator = CostEvaluator(penalty_capacity, penalty_tw)
 
-    # Feasible individual
-    feas_indiv = Individual(data, [[1, 2], [3], [4]])
-    feas_dist = feas_indiv.distance()
-
-    # For feasible individual, cost and penalised_cost should equal distance
-    assert_equal(cost_evaluator.penalised_cost(feas_indiv), feas_dist)
-    assert_equal(default_cost_evaluator.penalised_cost(feas_indiv), feas_dist)
-
-    # Infeasible individual
-    infeas_indiv = Individual(data, [[1, 2, 3, 4]])
-
-    # Compute cost associated to violated constraints
-    load_penalty_cost = penalty_capacity * infeas_indiv.excess_load()
-    tw_penalty_cost = penalty_tw * infeas_indiv.time_warp()
-    infeas_dist = infeas_indiv.distance()
+    feas = Solution(data, [[1, 2], [3], [4]])
+    assert_(feas.is_feasible())
+
+    # For a feasible solution, cost and penalised_cost equal distance.
+    assert_allclose(cost_evaluator.penalised_cost(feas), feas.distance())
+    assert_allclose(default_evaluator.penalised_cost(feas), feas.distance())
+
+    infeas = Solution(data, [[1, 2, 3, 4]])
+    assert_(not infeas.is_feasible())
+
+    # Compute cost associated with violated constraints.
+    load_penalty_cost = penalty_capacity * infeas.excess_load()
+    tw_penalty_cost = penalty_tw * infeas.time_warp()
+    infeas_dist = infeas.distance()
 
     # Test penalised cost
     expected_cost = infeas_dist + load_penalty_cost + tw_penalty_cost
-    assert_equal(cost_evaluator.penalised_cost(infeas_indiv), expected_cost)
+    assert_allclose(cost_evaluator.penalised_cost(infeas), expected_cost)
 
     # Default cost evaluator has 0 weights and only computes distance as cost
-    assert_equal(
-        default_cost_evaluator.penalised_cost(infeas_indiv), infeas_dist
-    )
+    assert_allclose(default_evaluator.penalised_cost(infeas), infeas_dist)
```

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_GeneticAlgorithm.py` & `pyvrp-0.4.1/pyvrp/tests/test_GeneticAlgorithm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from numpy.testing import assert_, assert_allclose, assert_equal, assert_raises
 from pytest import mark
 
 from pyvrp import (
     GeneticAlgorithm,
     GeneticAlgorithmParams,
-    Individual,
     PenaltyManager,
     Population,
     PopulationParams,
+    Solution,
     XorShift128,
 )
 from pyvrp.crossover import selective_route_exchange as srex
 from pyvrp.diversity import broken_pairs_distance as bpd
-from pyvrp.educate import Exchange10, LocalSearch, compute_neighbours
+from pyvrp.search import Exchange10, LocalSearch, compute_neighbours
 from pyvrp.stop import MaxIterations
 from pyvrp.tests.helpers import make_random_solutions, read, read_solution
 
 
 @mark.parametrize(
     "repair_probability,"
     "collect_statistics,"
@@ -104,18 +104,17 @@
     pop = Population(bpd)
     assert_equal(len(pop), 0)
 
     with assert_raises(ValueError):
         # No initial solutions should raise.
         GeneticAlgorithm(data, pen_manager, rng, pop, ls, srex, [])
 
-    individual = Individual.make_random(data, rng)
-
     # One initial solution, so this should be OK.
-    GeneticAlgorithm(data, pen_manager, rng, pop, ls, srex, [individual])
+    sol = Solution.make_random(data, rng)
+    GeneticAlgorithm(data, pen_manager, rng, pop, ls, srex, [sol])
 
 
 def test_initial_solutions_added_when_running():
     """
     Tests that GeneticAlgorithm adds initial solutions to the population
     when running the algorithm.
     """
@@ -127,15 +126,15 @@
     init = set(make_random_solutions(25, data, rng))
     algo = GeneticAlgorithm(data, pm, rng, pop, ls, srex, init)
 
     algo.run(MaxIterations(0))
 
     # Since we ran the algorithm for zero iterations, the population should
     # contain only the initial solutions.
-    current = {individual for individual in pop}
+    current = {sol for sol in pop}
     assert_equal(len(current & init), 25)
     assert_equal(len(pop), 25)
 
 
 def test_initial_solutions_added_when_restarting():
     """
     Tests that GeneticAlgorithm clears the population and adds the initial
@@ -147,15 +146,15 @@
     pop = Population(bpd)
 
     ls = LocalSearch(data, rng, compute_neighbours(data))
     ls.add_node_operator(Exchange10(data))
 
     # We use the best known solution as one of the initial solutions so that
     # there are no improving iterations.
-    init = {Individual(data, read_solution("data/RC208.sol"))}
+    init = {Solution(data, read_solution("data/RC208.sol"))}
     init.update(make_random_solutions(24, data, rng))
 
     params = GeneticAlgorithmParams(
         repair_probability=0,
         intensify_probability=0,
         intensify_on_best=False,
         nb_iter_no_improvement=100,
@@ -163,18 +162,18 @@
     algo = GeneticAlgorithm(data, pm, rng, pop, ls, srex, init, params=params)
 
     algo.run(MaxIterations(100))
 
     # There are precisely enough non-improving iterations to trigger the
     # restarting mechanism. GA should have cleared and re-initialised the
     # population with the initial solutions.
-    current = {individual for individual in pop}
+    current = {sol for sol in pop}
     assert_equal(len(current & init), 25)
 
-    # The population contains one more individual because of the educate step.
+    # The population contains one more solution because of the search step.
     assert_equal(len(pop), 26)
 
 
 def test_best_solution_improves_with_more_iterations():
     data = read("data/RC208.txt", "solomon", "dimacs")
     rng = XorShift128(seed=42)
     pm = PenaltyManager()
@@ -208,15 +207,15 @@
     the best found solution.
     """
     data = read("data/RC208.txt", "solomon", "dimacs")
     rng = XorShift128(seed=42)
     pm = PenaltyManager()
     pop = Population(bpd)
 
-    bks = Individual(data, read_solution("data/RC208.sol"))
+    bks = Solution(data, read_solution("data/RC208.sol"))
     init = [bks] + make_random_solutions(24, data, rng)
 
     ls = LocalSearch(data, rng, compute_neighbours(data))
     algo = GeneticAlgorithm(data, pm, rng, pop, ls, srex, init)
 
     result = algo.run(MaxIterations(0))
```

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_Matrix.py` & `pyvrp-0.4.1/pyvrp/tests/test_Matrix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from numpy.testing import assert_equal, assert_raises
 
 from pyvrp._Matrix import Matrix
 
 
 def test_dimension_constructor():
     square = Matrix(10)
+    assert_equal(square.num_rows, 10)
+    assert_equal(square.num_cols, 10)
     assert_equal(square.size(), 10 * 10)
     assert_equal(square.max(), 0)  # matrix initialises all zero
 
     rectangle = Matrix(10, 20)
+    assert_equal(rectangle.num_rows, 10)
+    assert_equal(rectangle.num_cols, 20)
     assert_equal(rectangle.size(), 10 * 20)
     assert_equal(rectangle.max(), 0)  # matrix initialises all zero
 
 
 def test_data_constructor():
     empty = Matrix([[], []])
     assert_equal(empty.size(), 0)
```

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_PenaltyManager.py` & `pyvrp-0.4.1/pyvrp/tests/test_PenaltyManager.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_Population.py` & `pyvrp-0.4.1/pyvrp/tests/test_Population.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     assert_raises,
     assert_warns,
 )
 from pytest import mark
 
 from pyvrp import (
     CostEvaluator,
-    Individual,
     Population,
     PopulationParams,
+    Solution,
     XorShift128,
 )
 from pyvrp.diversity import broken_pairs_distance as bpd
 from pyvrp.exceptions import EmptySolutionWarning
 from pyvrp.tests.helpers import make_random_solutions, read
 
 
@@ -107,72 +107,72 @@
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
 
     params = PopulationParams()
     pop = Population(bpd, params=params)
 
-    for indiv in make_random_solutions(params.min_pop_size, data, rng):
-        pop.add(indiv, cost_evaluator)
+    for sol in make_random_solutions(params.min_pop_size, data, rng):
+        pop.add(sol, cost_evaluator)
 
-    # Population should initialise at least min_pop_size individuals
+    # Population should initialise at least min_pop_size solutions
     assert_(len(pop) >= params.min_pop_size)
     assert_equal(len(pop), pop.num_feasible() + pop.num_infeasible())
 
     num_feas = pop.num_feasible()
     num_infeas = pop.num_infeasible()
 
-    while True:  # keep adding feasible individuals until we are about to purge
-        individual = Individual.make_random(data, rng)
+    while True:  # keep adding feasible solutions until we are about to purge
+        sol = Solution.make_random(data, rng)
 
-        if individual.is_feasible():
-            pop.add(individual, cost_evaluator)
+        if sol.is_feasible():
+            pop.add(sol, cost_evaluator)
             num_feas += 1
 
             assert_equal(len(pop), num_feas + num_infeas)
             assert_equal(pop.num_feasible(), num_feas)
 
         if num_feas == params.max_pop_size:  # next add() triggers purge
             break
 
-    # RNG is fixed, and this next individual is feasible. Since we now have a
-    # feasible population that is of maximal size, adding this individual
-    # should trigger survivor selection (purge). Survivor selection reduces the
+    # RNG is fixed, and this next solution is feasible. Since we now have a
+    # feasible population that is of maximal size, adding this solution should
+    # trigger survivor selection (purge). Survivor selection reduces the
     # feasible subpopulation to min_pop_size, so the overal population is then
     # just num_infeas + min_pop_size.
-    individual = Individual.make_random(data, rng)
-    assert_(individual.is_feasible())
+    sol = Solution.make_random(data, rng)
+    assert_(sol.is_feasible())
 
-    pop.add(individual, cost_evaluator)
+    pop.add(sol, cost_evaluator)
     assert_equal(pop.num_feasible(), params.min_pop_size)
     assert_equal(len(pop), num_infeas + params.min_pop_size)
 
 
 def test_select_returns_same_parents_if_no_other_option():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=2_147_483_647)
 
     params = PopulationParams(min_pop_size=0)
     pop = Population(bpd, params=params)
 
     assert_equal(len(pop), 0)
 
-    pop.add(Individual(data, [[3, 2], [1, 4]]), cost_evaluator)
+    pop.add(Solution(data, [[3, 2], [1, 4]]), cost_evaluator)
     assert_equal(len(pop), 1)
 
-    # We added a single individual, so we should now get the same parent twice.
+    # We added a single solution, so we should now get the same parent twice.
     parents = pop.select(rng, cost_evaluator)
     assert_(parents[0] == parents[1])
 
-    # Now we add another, different individual.
-    pop.add(Individual(data, [[3, 2], [1], [4]]), cost_evaluator)
+    # Now we add another, different solution.
+    pop.add(Solution(data, [[3, 2], [1], [4]]), cost_evaluator)
     assert_equal(len(pop), 2)
 
-    # We should now get two different individuals as parents, at least most of
+    # We should now get two different solutions as parents, at least most of
     # the time. The actual probability of getting the same parents is very
     # small, but not zero. So let's do an experiment where we do 1000 selects,
     # and collect the number of times the parents are different.
     different_parents = 0
     for _ in range(1_000):
         parents = pop.select(rng, cost_evaluator)
         different_parents += parents[0] != parents[1]
@@ -195,89 +195,82 @@
     params = PopulationParams(min_pop_size=0, generation_size=0)
     pop = Population(bpd, params=params)
 
     assert_equal(len(pop), 0)
 
     for _ in range(10):
         # With zero min_pop_size and zero generation_size, every additional
-        # individual triggers a purge. So the population size can never grow
+        # solution triggers a purge. So the population size can never grow
         # beyond zero.
-        pop.add(Individual.make_random(data, rng), cost_evaluator)
+        pop.add(Solution.make_random(data, rng), cost_evaluator)
         assert_equal(len(pop), 0)
 
 
 @mark.parametrize("nb_elite", [5, 25])
-def test_elite_individuals_are_not_purged(nb_elite: int):
+def test_elite_solutions_are_not_purged(nb_elite: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     params = PopulationParams(nb_elite=nb_elite)
     rng = XorShift128(seed=42)
 
     pop = Population(bpd, params=params)
 
-    # Keep adding individuals until the infeasible subpopulation is of maximum
+    # Keep adding solutions until the infeasible subpopulation is of maximum
     # size.
     while pop.num_infeasible() != params.max_pop_size:
-        pop.add(Individual.make_random(data, rng), cost_evaluator)
+        pop.add(Solution.make_random(data, rng), cost_evaluator)
 
     assert_equal(pop.num_infeasible(), params.max_pop_size)
 
-    # These are the nb_elite best solutions in the current solution pool. These
+    # These are the elite best solutions in the current solution pool. These
     # should never be purged.
-    curr_individuals = [
-        individual for individual in pop if not individual.is_feasible()
-    ]
-
-    best_individuals = sorted(
-        curr_individuals, key=cost_evaluator.penalised_cost
-    )
-    elite_individuals = best_individuals[:nb_elite]
+    curr_sols = [sol for sol in pop if not sol.is_feasible()]
+    best_sols = sorted(curr_sols, key=cost_evaluator.penalised_cost)
+    elite_sols = best_sols[:nb_elite]
 
     # Add a solution that is certainly not feasible, thus causing a purge.
     single_route = [client for client in range(1, data.num_clients + 1)]
-    pop.add(Individual(data, [single_route]), cost_evaluator)
+    pop.add(Solution(data, [single_route]), cost_evaluator)
 
     # After the purge, there should remain min_pop_size infeasible solutions.
     assert_equal(pop.num_infeasible(), params.min_pop_size)
 
-    # In the infeasible subpopulation, nb_elite solutions from before the purge
-    # should also still be present. We test that by selecting the nb_elite best
-    # individuals from before the purge. We test by id/memory location because
-    # these individuals should still be present, unmodified.
-    new_individuals = [id(individual) for individual in pop]
-    for elite_individual in elite_individuals:
-        assert_(id(elite_individual) in new_individuals)
+    # Elite solutions from before the purge should also still be present. We
+    # test by id/memory location that these solutions are still present.
+    new_sols = [id(sol) for sol in pop]
+    for elite_sol in elite_sols:
+        assert_(id(elite_sol) in new_sols)
 
 
 @mark.parametrize("k", [2, 3])
 def test_tournament_ranks_by_fitness(k: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
     pop = Population(bpd)
 
-    for individual in make_random_solutions(50, data, rng):
-        if not individual.is_feasible():
-            pop.add(individual, cost_evaluator)
+    for sol in make_random_solutions(50, data, rng):
+        if not sol.is_feasible():
+            pop.add(sol, cost_evaluator)
 
     assert_equal(pop.num_feasible(), 0)
 
-    # Since this test requires the fitness values of the individuals, we have
+    # Since this test requires the fitness values of the solutions, we have
     # to access the underlying infeasible subpopulation directly.
     infeas_pop = pop._infeas
     infeas_pop.update_fitness(cost_evaluator)
 
     items = [item for item in pop._infeas]
     by_fitness = sorted(items, key=lambda item: item.fitness)
-    indiv2idx = {item.individual: idx for idx, item in enumerate(by_fitness)}
+    sol2idx = {item.solution: idx for idx, item in enumerate(by_fitness)}
     infeas_count = np.zeros(len(infeas_pop))
 
     for _ in range(10_000):
-        indiv = pop.get_tournament(rng, cost_evaluator, k=k)
-        infeas_count[indiv2idx[indiv]] += 1
+        sol = pop.get_tournament(rng, cost_evaluator, k=k)
+        infeas_count[sol2idx[sol]] += 1
 
     # Now we compare the observed ranking from the tournament selection with
     # what we expect from the actual fitness ranking. We compute the percentage
     # of times we're incorrect, and test that that number is not too high.
     actual_rank = 1 + np.argsort(-infeas_count)  # higher is better
     expected_rank = 1 + np.arange(len(infeas_pop))
     pct_off = np.abs((actual_rank - expected_rank) / len(infeas_pop)).mean()
@@ -296,78 +289,76 @@
 @mark.parametrize("k", [-100, -1, 0])  # k must be strictly positive
 def test_tournament_raises_for_invalid_k(k: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
     pop = Population(bpd)
 
-    for individual in make_random_solutions(5, data, rng):
-        pop.add(individual, cost_evaluator)
+    for sol in make_random_solutions(5, data, rng):
+        pop.add(sol, cost_evaluator)
 
     with assert_raises(ValueError):
         pop.get_tournament(rng, cost_evaluator, k=k)
 
 
 def test_purge_removes_duplicates():
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     params = PopulationParams(min_pop_size=20, generation_size=5)
     rng = XorShift128(seed=42)
 
     pop = Population(bpd, params=params)
 
-    for indiv in make_random_solutions(params.min_pop_size, data, rng):
-        pop.add(indiv, cost_evaluator)
+    for sol in make_random_solutions(params.min_pop_size, data, rng):
+        pop.add(sol, cost_evaluator)
 
     assert_equal(len(pop), params.min_pop_size)
 
-    # This is the individual we are going to add a few times. That should make
+    # This is the solution we are going to add a few times. That should make
     # sure the relevant subpopulation definitely contains duplicates.
-    individual = Individual.make_random(data, rng)
-    assert_(not individual.is_feasible())
+    sol = Solution.make_random(data, rng)
+    assert_(not sol.is_feasible())
 
     for _ in range(params.generation_size):
-        pop.add(individual, cost_evaluator)
+        pop.add(sol, cost_evaluator)
 
     # Make sure we have not yet purged, and increase the minimum population
     # size by one to make sure we're definitely not removing *all* of the
-    # duplicate individuals.
+    # duplicate solutions.
     assert_(pop.num_infeasible() != params.min_pop_size)
     params.min_pop_size += 1
 
-    # Keep adding individuals until we have had a purge, and returned to the
-    # minimum population size.
+    # Keep adding the solution until we have had a purge, and returned to the
+    # minimum population size. Note that the purge is done after adding the
+    # solution, so we must add the same solution in order to have at most
+    # min_pop_size - 1 other solutions than the duplicated solution.
     while pop.num_infeasible() != params.min_pop_size:
-        pop.add(Individual.make_random(data, rng), cost_evaluator)
+        pop.add(sol, cost_evaluator)
 
     # Since duplicates are purged first, there should now be only one of them
     # in the subpopulation. There cannot be zero, because we made sure of that.
-    duplicates = 0
-    for other in pop:
-        if other == individual:
-            duplicates += 1
-
+    duplicates = sum(other == sol for other in pop)
     assert_equal(duplicates, 1)
 
 
 def test_clear():
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
     pop = Population(bpd)
 
-    for individual in make_random_solutions(10, data, rng):
-        pop.add(individual, cost_evaluator)
+    for sol in make_random_solutions(10, data, rng):
+        pop.add(sol, cost_evaluator)
 
     assert_equal(len(pop), 10)
 
     pop.clear()
     assert_equal(len(pop), 0)
 
 
 def test_add_emits_warning_when_solution_is_empty():
     data = read("data/p06-2-50.vrp", round_func="dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     pop = Population(bpd)
 
     with assert_warns(EmptySolutionWarning):
-        pop.add(Individual(data, []), cost_evaluator)
+        pop.add(Solution(data, []), cost_evaluator)
```

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_ProblemData.py` & `pyvrp-0.4.1/pyvrp/tests/test_ProblemData.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,121 @@
+import numpy as np
 from numpy.random import default_rng
 from numpy.testing import assert_, assert_allclose, assert_raises
 from pytest import mark
 
-from pyvrp import Client, ProblemData
+from pyvrp import Client, ProblemData, VehicleType
+from pyvrp.tests.helpers import read
 
 
 @mark.parametrize(
-    "x,y,demand,service_duration,tw_early,tw_late,prize",
+    "x,y,demand,service_duration,tw_early,tw_late,release_time,prize",
     [
-        (1, 1, 1, 1, 0, 1, 0),  # normal
-        (1, 1, 1, 0, 0, 1, 0),  # zero duration
-        (1, 1, 0, 1, 0, 1, 0),  # zero demand
-        (1, 1, 1, 1, 0, 0, 0),  # zero length time interval
-        (-1, -1, 1, 1, 0, 1, 0),  # negative coordinates
-        (0, 0, 1, 1, 0, 1, 1),  # positive prize
+        (1, 1, 1, 1, 0, 1, 0, 0),  # normal
+        (1, 1, 1, 0, 0, 1, 0, 0),  # zero duration
+        (1, 1, 0, 1, 0, 1, 0, 0),  # zero demand
+        (1, 1, 1, 1, 0, 0, 0, 0),  # zero length time interval
+        (-1, -1, 1, 1, 0, 1, 0, 0),  # negative coordinates
+        (1, 1, 1, 1, 0, 1, 1, 0),  # positive release time
+        (0, 0, 1, 1, 0, 1, 0, 1),  # positive prize
     ],
 )
 def test_client_constructor_initialises_data_fields_correctly(
     x: int,
     y: int,
     demand: int,
     service_duration: int,
     tw_early: int,
     tw_late: int,
+    release_time: int,
     prize: int,
 ):
-    client = Client(x, y, demand, service_duration, tw_early, tw_late, prize)
+    client = Client(
+        x, y, demand, service_duration, tw_early, tw_late, release_time, prize
+    )
     assert_allclose(client.x, x)
     assert_allclose(client.y, y)
     assert_allclose(client.demand, demand)
     assert_allclose(client.service_duration, service_duration)
     assert_allclose(client.tw_early, tw_early)
     assert_allclose(client.tw_late, tw_late)
+    assert_allclose(client.release_time, release_time)
     assert_allclose(client.prize, prize)
 
 
 @mark.parametrize(
-    "x,y,demand,service_duration,tw_early,tw_late,prize",
+    "x,y,demand,service,tw_early,tw_late,release_time,prize",
     [
-        (1, 1, 1, 1, 1, 0, 0),  # late < early
-        (1, 1, 1, -1, 0, 1, 0),  # negative duration
-        (1, 1, -1, 1, 0, 1, 0),  # negative demand
-        (1, 1, 1, 1, 0, 1, -1),  # negative prize
+        (1, 1, 1, 1, 1, 0, 0, 0),  # late < early
+        (1, 1, 1, -1, 0, 1, 0, 0),  # negative service duration
+        (1, 1, -1, 1, 0, 1, 0, 0),  # negative demand
+        (1, 1, 1, 1, 0, 1, 0, -1),  # negative prize
     ],
 )
 def test_raises_for_invalid_client_data(
     x: int,
     y: int,
     demand: int,
-    service_duration: int,
+    service: int,
     tw_early: int,
     tw_late: int,
+    release_time: int,
     prize: int,
 ):
     with assert_raises(ValueError):
-        Client(x, y, demand, service_duration, tw_early, tw_late, prize)
+        Client(x, y, demand, service, tw_early, tw_late, release_time, prize)
 
 
 def test_depot_is_first_client():
     """
     The ``depot()`` helper should return the first client, that is,
     ``client(0)``.
     """
     mat = [[0, 1], [1, 0]]
 
     data = ProblemData(
         clients=[Client(x=0, y=0), Client(x=0, y=1)],
-        nb_vehicles=1,
-        vehicle_cap=1,
+        vehicle_types=[VehicleType(1, 2)],
         distance_matrix=mat,
         duration_matrix=mat,
     )
 
     assert_(data.depot() is data.client(0))
 
 
+def test_centroid():
+    data = read("data/OkSmall.txt")
+
+    centroid = data.centroid()
+    x = [data.client(idx).x for idx in range(1, data.num_clients + 1)]
+    y = [data.client(idx).y for idx in range(1, data.num_clients + 1)]
+
+    assert_allclose(centroid[0], np.mean(x))
+    assert_allclose(centroid[1], np.mean(y))
+
+
 def test_matrix_access():
     """
-    Tests that the ``duration()``, ``duration_matrix()``, ``dist()``, and
-    ``distance_matrix()`` methods correctly index the underlying duration
-    and distance matrices.
+    Tests that the ``duration()`` and ``dist()`` methods correctly index the
+    underlying duration and distance matrices.
     """
     gen = default_rng(seed=42)
     size = 6
 
     dist_mat = gen.integers(500, size=(size, size))
     dur_mat = gen.integers(500, size=(size, size))
     clients = [
         Client(x=0, y=0, demand=0, service_duration=0, tw_early=0, tw_late=10)
         for _ in range(size)
     ]
 
     data = ProblemData(
         clients=clients,
-        nb_vehicles=1,
-        vehicle_cap=1,
+        vehicle_types=[VehicleType(1, 2)],
         distance_matrix=dist_mat,  # type: ignore
         duration_matrix=dur_mat,  # type: ignore
     )
 
-    dist_mat_data = data.distance_matrix()
-    dur_mat_data = data.duration_matrix()
-
     for frm in range(size):
         for to in range(size):
             assert_allclose(dur_mat[frm, to], data.duration(frm, to))
             assert_allclose(dist_mat[frm, to], data.dist(frm, to))
-
-            assert_allclose(dur_mat_data[frm, to], dur_mat[frm, to])
-            assert_allclose(dist_mat_data[frm, to], dist_mat[frm, to])
```

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_Result.py` & `pyvrp-0.4.1/pyvrp/tests/test_Result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 import math
 
 from numpy.testing import assert_, assert_allclose, assert_equal, assert_raises
 from pytest import mark
 
-from pyvrp import CostEvaluator, Individual, Population, XorShift128
+from pyvrp import CostEvaluator, Population, Solution, XorShift128
 from pyvrp.Result import Result
 from pyvrp.Statistics import Statistics
 from pyvrp.diversity import broken_pairs_distance
 from pyvrp.tests.helpers import read
 
 
 @mark.parametrize(
     "routes, num_iterations, runtime",
     [([[1, 2], [3], [4]], 1, 1.5), ([[1, 2, 3, 4]], 100, 54.2)],
 )
 def test_fields_are_correctly_set(routes, num_iterations, runtime):
     data = read("data/OkSmall.txt")
-    indiv = Individual(data, routes)
+    sol = Solution(data, routes)
 
-    res = Result(indiv, Statistics(), num_iterations, runtime)
+    res = Result(sol, Statistics(), num_iterations, runtime)
 
-    assert_equal(res.is_feasible(), indiv.is_feasible())
+    assert_equal(res.is_feasible(), sol.is_feasible())
     assert_equal(res.num_iterations, num_iterations)
-    if indiv.is_feasible():
-        assert_allclose(res.cost(), CostEvaluator().cost(indiv))
+    assert_allclose(res.runtime, runtime)
+
+    if sol.is_feasible():
+        assert_allclose(res.cost(), CostEvaluator().cost(sol))
     else:
         assert_equal(res.cost(), math.inf)
-    assert_allclose(res.runtime, runtime)
 
 
 @mark.parametrize(
     "num_iterations, runtime",
     [
         (-1, 0.0),  # num_iterations < 0
         (0, -1.0),  # runtime < 0
     ],
 )
 def test_init_raises_invalid_arguments(num_iterations, runtime):
     data = read("data/OkSmall.txt")
-    indiv = Individual(data, [[1, 2, 3, 4], [], []])
+    sol = Solution(data, [[1, 2, 3, 4]])
 
     with assert_raises(ValueError):
-        Result(indiv, Statistics(), num_iterations, runtime)
+        Result(sol, Statistics(), num_iterations, runtime)
 
 
 @mark.parametrize(
     "num_iterations, has_statistics", [(0, False), (1, True), (10, True)]
 )
 def test_has_statistics(num_iterations: int, has_statistics: bool):
     data = read("data/OkSmall.txt")
@@ -53,35 +54,34 @@
     rng = XorShift128(seed=42)
     pop = Population(broken_pairs_distance)
     stats = Statistics()
 
     for _ in range(num_iterations):
         stats.collect_from(pop, cost_evaluator)
 
-    best = Individual.make_random(data, rng)
+    best = Solution.make_random(data, rng)
     res = Result(best, stats, num_iterations, 0.0)
     assert_equal(res.has_statistics(), has_statistics)
     assert_equal(res.num_iterations, num_iterations)
 
 
 @mark.parametrize(
     "routes",
     [[[1, 2], [3], [4]], [[1, 2, 3, 4]]],
 )
 def test_str_contains_essential_information(routes):
     data = read("data/OkSmall.txt")
 
-    individual = Individual(data, routes)
-    res = Result(individual, Statistics(), 0, 0.0)
+    sol = Solution(data, routes)
+    res = Result(sol, Statistics(), 0, 0.0)
     str_representation = str(res)
 
     # Test that feasibility status and solution cost are presented.
-    if individual.is_feasible():
-        cost = CostEvaluator().cost(individual)
+    if sol.is_feasible():
+        cost = CostEvaluator().cost(sol)
         assert_(str(cost) in str_representation)
     else:
         assert_("INFEASIBLE" in str_representation)
 
-    # And make sure that all non-empty routes are printed as well.
-    for route in individual.get_routes():
-        if route:
-            assert_(str(route) in str_representation)
+    # And make sure that all routes are printed as well.
+    for route in sol.get_routes():
+        assert_(str(route) in str_representation)
```

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_Statistics.py` & `pyvrp-0.4.1/pyvrp/tests/test_Statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 def test_csv_serialises_correctly(tmp_path):
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
     pop = Population(broken_pairs_distance)
 
-    for individual in make_random_solutions(10, data, rng):
-        pop.add(individual, cost_evaluator)
+    for sol in make_random_solutions(10, data, rng):
+        pop.add(sol, cost_evaluator)
 
     collected_stats = Statistics()
 
     for _ in range(10):  # populate the statistics object
         collected_stats.collect_from(pop, cost_evaluator)
 
     csv_path = tmp_path / "test.csv"
```

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_TimeWindowSegment.py` & `pyvrp-0.4.1/pyvrp/tests/test_TimeWindowSegment.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,47 +3,54 @@
 
 from pyvrp._Matrix import Matrix
 from pyvrp._TimeWindowSegment import TimeWindowSegment
 
 
 @mark.parametrize("existing_time_warp", [2, 5, 10])
 def test_total_time_warp(existing_time_warp):
-    tws1 = TimeWindowSegment(0, 0, 0, existing_time_warp, 0, 0)
+    tws1 = TimeWindowSegment(0, 0, 0, existing_time_warp, 0, 0, 0)
     assert_equal(tws1.total_time_warp(), existing_time_warp)
 
 
 def test_merge_two():
-    tws1 = TimeWindowSegment(0, 0, 5, 0, 0, 5)
-    tws2 = TimeWindowSegment(1, 1, 0, 5, 3, 6)
+    tws1 = TimeWindowSegment(0, 0, 5, 0, 0, 5, 0)
+    tws2 = TimeWindowSegment(1, 1, 0, 5, 3, 6, 0)
 
     mat = Matrix([[1, 4], [1, 2]])
     merged = TimeWindowSegment.merge(mat, tws1, tws2)
 
     # There is no release time, so segment time warp and total time warp should
     # be equal. The first stop (tws1) takes already has five duration, and
     # starts at time 0. Then, we have to drive for 4 units (mat(0, 1) = 4) to
     # get to the second stop (tws2). This second segment has 5 time warp, and
     # we arrive there at time 5 + 4 = 9, which is 9 - 6 = 3 after its closing
     # time window. So we get a final time warp of 5 + 3 = 8.
     assert_equal(merged.total_time_warp(), 8)
 
+    # Now, let's add a bit of release time (3), so that the total time warp
+    # should become 8 + 3 = 11.
+    tws2 = TimeWindowSegment(1, 1, 0, 5, 3, 6, 3)
+    merged = TimeWindowSegment.merge(mat, tws1, tws2)
+    assert_equal(merged.total_time_warp(), 11)
+
 
 def test_merge_multiple():
-    tws1 = TimeWindowSegment(0, 0, 5, 0, 0, 5)
-    tws2 = TimeWindowSegment(1, 1, 0, 0, 3, 6)
-    tws3 = TimeWindowSegment(2, 2, 0, 0, 2, 3)
+    tws1 = TimeWindowSegment(0, 0, 5, 0, 0, 5, 0)
+    tws2 = TimeWindowSegment(1, 1, 0, 0, 3, 6, 0)
+    tws3 = TimeWindowSegment(2, 2, 0, 0, 2, 3, 2)
 
     mat = Matrix([[1, 4, 1], [1, 2, 4], [1, 1, 1]])
     merged1 = TimeWindowSegment.merge(mat, tws1, tws2)
     merged2 = TimeWindowSegment.merge(mat, merged1, tws3)
     merged3 = TimeWindowSegment.merge(mat, tws1, tws2, tws3)
 
     # Merge all together should be the same as merging in several steps.
     assert_equal(merged3.total_time_warp(), merged2.total_time_warp())
 
     # After also merging in tws3, we should have 3 time warp from 0 -> 1, and 7
-    # time warp from 1 -> 2, for 10 total time warp.
-    assert_equal(merged3.total_time_warp(), 10)
+    # time warp from 1 -> 2. Since there's also a release time of 2, the total
+    # time warp is 12.
+    assert_equal(merged3.total_time_warp(), 12)
 
 
 # TODO test two previously merged segments, e.g. merge(merge(1, 2),
 #  merge(3, 4)), each with time warp
```

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_XorShift128.py` & `pyvrp-0.4.1/pyvrp/tests/test_XorShift128.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.3.0/pyvrp/tests/test_read.py` & `pyvrp-0.4.1/pyvrp/tests/test_read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from numpy.testing import assert_equal, assert_raises
+from numpy.testing import assert_equal, assert_raises, assert_warns
 from pytest import mark
 
+from pyvrp.exceptions import ScalingWarning
 from pyvrp.tests.helpers import read
 
 
 @mark.parametrize(
     "where, exception",
     [
         ("data/UnknownEdgeWeightFmt.txt", ValueError),
         ("data/UnknownEdgeWeightType.txt", ValueError),
         ("somewhere that does not exist", FileNotFoundError),
         ("data/FileWithUnknownSection.txt", ValueError),
         ("data/DepotNotOne.txt", ValueError),
         ("data/MoreThanOneDepot.txt", ValueError),
         ("data/NonZeroDepotServiceDuration.txt", ValueError),
         ("data/NonZeroDepotOpenTimeWindow.txt", ValueError),
+        ("data/NonZeroDepotReleaseTime.txt", ValueError),
         ("data/NonZeroDepotDemand.txt", ValueError),
         ("data/TimeWindowOpenLargerThanClose.txt", ValueError),
         ("data/EdgeWeightsNoExplicit.txt", ValueError),
         ("data/EdgeWeightsNotFullMatrix.txt", ValueError),
     ],
 )
 def test_raises_invalid_file(where: str, exception: Exception):
@@ -37,15 +39,16 @@
 
 def test_reading_OkSmall_instance():
     data = read("data/OkSmall.txt")
 
     # From the DIMENSION, VEHICLES, and CAPACITY fields in the file.
     assert_equal(data.num_clients, 4)
     assert_equal(data.num_vehicles, 3)
-    assert_equal(data.vehicle_capacity, 10)
+    assert_equal(data.num_vehicle_types, 1)
+    assert_equal(data.vehicle_type(0).capacity, 10)
 
     # From the NODE_COORD_SECTION in the file
     expected = [
         (2334, 726),
         (226, 1297),
         (590, 530),
         (435, 718),
@@ -61,26 +64,20 @@
         [0, 1544, 1944, 1931, 1476],
         [1726, 0, 1992, 1427, 1593],
         [1965, 1975, 0, 621, 1090],
         [2063, 1433, 647, 0, 818],
         [1475, 1594, 1090, 828, 0],
     ]
 
-    # For instances read through VRPLIB/read(), distance is duration. So these
-    # matrices should be the same as the expected edge weights above.
-    dist_mat = data.distance_matrix()
-    dur_mat = data.duration_matrix()
-
+    # For instances read through VRPLIB/read(), distance is duration. So the
+    # dist/durs should be the same as the expected edge weights above.
     for frm in range(data.num_clients + 1):  # incl. depot
         for to in range(data.num_clients + 1):  # incl. depot
             assert_equal(data.dist(frm, to), expected[frm][to])
-            assert_equal(dist_mat[frm, to], expected[frm][to])
-
             assert_equal(data.duration(frm, to), expected[frm][to])
-            assert_equal(dur_mat[frm, to], expected[frm][to])
 
     # From the DEMAND_SECTION in the file
     expected = [0, 5, 5, 3, 5]
 
     for client in range(data.num_clients + 1):  # incl. depot
         assert_equal(data.client(client).demand, expected[client])
 
@@ -104,15 +101,15 @@
         assert_equal(data.client(client).service_duration, expected[client])
 
 
 def test_reading_En22k4_instance():  # instance from CVRPLIB
     data = read("data/E-n22-k4.txt", round_func="trunc1")
 
     assert_equal(data.num_clients, 21)
-    assert_equal(data.vehicle_capacity, 6_000)
+    assert_equal(data.vehicle_type(0).capacity, 6_000)
 
     # Coordinates are scaled by 10 to align with 1 decimal distance precision
     assert_equal(data.depot().x, 1450)  # depot [x, y] location
     assert_equal(data.depot().y, 2150)
 
     assert_equal(data.client(1).x, 1510)  # first customer [x, y] location
     assert_equal(data.client(1).y, 2640)
@@ -124,28 +121,31 @@
     #      dX = 151 - 145 = 6
     #      dY = 264 - 215 = 49
     #      dist = sqrt(dX^2 + dY^2) = 49.37
     #      int(10 * dist) = 493
     assert_equal(data.dist(0, 1), 493)
     assert_equal(data.dist(1, 0), 493)
 
-    # This is a CVRP instance, so time window data should all be zeroed out.
+    # This is a CVRP instance, so all other fields should have default values.
     for client in range(data.num_clients + 1):  # incl. depot
         assert_equal(data.client(client).service_duration, 0)
         assert_equal(data.client(client).tw_early, 0)
         assert_equal(data.client(client).tw_late, 0)
+        assert_equal(data.client(client).release_time, 0)
+        assert_equal(data.client(client).prize, 0)
+        assert_equal(data.client(client).required, True)
 
 
 def test_reading_RC208_instance():  # Solomon style instance
     data = read(
         "data/RC208.txt", instance_format="solomon", round_func="trunc1"
     )
 
     assert_equal(data.num_clients, 100)  # Excl. depot
-    assert_equal(data.vehicle_capacity, 1_000)
+    assert_equal(data.vehicle_type(0).capacity, 1_000)
 
     # Coordinates and times are scaled by 10 for 1 decimal distance precision
     assert_equal(data.depot().x, 400)  # depot [x, y] location
     assert_equal(data.depot().y, 500)
     assert_equal(data.depot().tw_early, 0)
     assert_equal(data.depot().tw_late, 9600)
 
@@ -167,9 +167,24 @@
     #      int(10 * dist) = 380
     assert_equal(data.dist(0, 1), 380)
     assert_equal(data.dist(1, 0), 380)
 
     for client in range(1, data.num_clients + 1):  # excl. depot
         assert_equal(data.client(client).service_duration, 100)
 
+    # This is a VRPTW instance, so all other fields should have default values.
+    for client in range(data.num_clients + 1):  # incl. depot
+        assert_equal(data.client(client).release_time, 0)
+        assert_equal(data.client(client).prize, 0)
+        assert_equal(data.client(client).required, True)
+
+
+def test_warns_about_scaling_issues(recwarn):
+    # But 100 million is too large. That's really close to INT_MAX, and might
+    # result in issues. So now a warning should be issued.
+    with assert_warns(ScalingWarning):
+        # The arc from the depot to client 4 is really large (one billion), so
+        # that should trigger a warning.
+        read("data/ReallyLargeDistance.txt")
+
 
 # TODO test round funcs
```

