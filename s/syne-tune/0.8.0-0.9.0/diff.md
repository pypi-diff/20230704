# Comparing `tmp/syne_tune-0.8.0.tar.gz` & `tmp/syne_tune-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syne_tune-0.8.0.tar", last modified: Tue Jun 20 15:04:45 2023, max compression
+gzip compressed data, was "syne_tune-0.9.0.tar", last modified: Tue Jul  4 10:02:50 2023, max compression
```

## Comparing `syne_tune-0.8.0.tar` & `syne_tune-0.9.0.tar`

### file list

```diff
@@ -1,309 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-20 15:04:35.000000 syne_tune-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 15:04:35.000000 syne_tune-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 15:04:35.000000 syne_tune-0.8.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-06-20 15:04:45.744142 syne_tune-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18904 2023-06-20 15:04:35.000000 syne_tune-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 15:04:45.748142 syne_tune-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-20 15:04:35.000000 syne_tune-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/local_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/backend/python_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/python_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/python_backend/python_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/python_backend/python_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/custom_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/backend/simulator_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/simulator_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/simulator_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/trial_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/trial_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/blackbox_repository/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/tensorboard_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    43893 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/config_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/aggregate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/experiment_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/multiobjective.py
--rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/plot_per_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    36758 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/results_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/num_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40558 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_rush.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multi_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
--rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/pbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/random_seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/ray_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18409 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    42227 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    34595 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/remote_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/remote_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/remote_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/results_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/tuner_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/tuning_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/utils/config_as_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/utils/parse_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15789 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.236537 syne_tune-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-04 10:02:41.000000 syne_tune-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 10:02:41.000000 syne_tune-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 10:02:41.000000 syne_tune-0.9.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-04 10:02:50.236537 syne_tune-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-07-04 10:02:41.000000 syne_tune-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-04 10:02:50.236537 syne_tune-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-04 10:02:41.000000 syne_tune-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/local_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/backend/python_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/python_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/python_backend/python_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/python_backend/python_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/custom_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/backend/simulator_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/simulator_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/simulator_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/trial_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/trial_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/blackbox_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/tensorboard_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43893 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/config_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/baselines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/lcbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/nas201.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/yahpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/default_baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/experiment_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/experiments/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/experiments/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/aggregate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/plot_per_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36795 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17334 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/results_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/num_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45677 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multi_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/pbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/random_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/ray_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18469 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42228 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34595 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31125 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.236537 syne_tune-0.9.0/syne_tune/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/remote_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/remote_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/remote_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/results_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/tuner_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/tuning_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.236537 syne_tune-0.9.0/syne_tune/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/utils/config_as_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/utils/parse_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/top_level.txt
```

### Comparing `syne_tune-0.8.0/LICENSE` & `syne_tune-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/PKG-INFO` & `syne_tune-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne_tune
-Version: 0.8.0
+Version: 0.9.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -135,35 +135,47 @@
     n_workers=4,  # how many trials are evaluated in parallel
 )
 tuner.run()
 ```
 
 The above example runs ASHA with 4 asynchronous workers on a local machine.
 
+## Experimentation with Syne Tune
+
+If you plan to use advanced features of Syne Tune, such as different execution
+backends or running experiments remotely, writing launcher scripts like
+`examples/launch_height_simple.py` can become tedious. Syne Tune provides an
+advanced experimentation framework, which you can learn about in
+[this tutorial](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html)
+or also in
+[this one](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html).
+
 ## Supported HPO methods
 
 The following hyperparameter optimization (HPO) methods are available in Syne Tune:
 
 Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer? 
 :--- | :---: | :---: | :---: | :---: | :---: 
 Grid Search |  | deterministic | yes | no | no 
 Random Search | Bergstra, et al. (2011) | random | yes | no | no 
 Bayesian Optimization | Snoek, et al. (2012) | model-based | yes | no | no 
 BORE | Tiao, et al. (2021) | model-based | yes | no | no 
+CQR | Salinas, et al. (2023) | model-based | yes | no | no 
 MedianStoppingRule | Golovin, et al. (2017) | any | yes | yes | no 
 SyncHyperband | Li, et al. (2018) | random | no | yes | no 
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
 HyperTune | Li, et al. (2022) | model-based | yes | yes | no
 DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
-ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no 
+ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no
+ASHACQR | Salinas, et al. (2023) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
 RUSH | Zappella, et al. (2021)| random | yes | yes | yes 
@@ -223,14 +235,20 @@
   launches HPO locally to tune a gluon-ts time series forecasting algorithm
 * [launch_rl_tuning.py](examples/launch_rl_tuning.py):
   launches HPO locally to tune a RL algorithm on the cartpole environment
 * [launch_height_ray.py](examples/launch_height_ray.py):
   launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
   scheduler
 
+## Examples for Experimentation and Benchmarking
+
+You will find many examples for experimentation and benchmarking in
+[benchmarking/examples/](benchmarking/examples/) and in
+benchmarking/nusery/](benchmarking/nursery/).
+
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
 * [What are the different installations options supported?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-different-installations-options-supported)
@@ -267,18 +285,20 @@
 
 Do you want to know more? Here are a number of tutorials.
 * [Basics of Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)
 * [Choosing a Configuration Space](https://syne-tune.readthedocs.io/en/latest/search_space.html)
 * [Using the Built-in Schedulers](https://syne-tune.readthedocs.io/en/latest/schedulers.html)
 * [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
 * [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
+* [Visualization of Results](https://syne-tune.readthedocs.io/en/latest/tutorials/visualization/README.html)
+* [Rapid Experimentation with Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html)
 * [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
 * [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
 * [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
-
+* [Distributed Hyperparameter Tuning: Finding the Right Model can be Fast and Fun](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html)
 
 ## Blog Posts
 
 - [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
 - [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
 - [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
```

### Comparing `syne_tune-0.8.0/README.md` & `syne_tune-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,35 +106,47 @@
     n_workers=4,  # how many trials are evaluated in parallel
 )
 tuner.run()
 ```
 
 The above example runs ASHA with 4 asynchronous workers on a local machine.
 
+## Experimentation with Syne Tune
+
+If you plan to use advanced features of Syne Tune, such as different execution
+backends or running experiments remotely, writing launcher scripts like
+`examples/launch_height_simple.py` can become tedious. Syne Tune provides an
+advanced experimentation framework, which you can learn about in
+[this tutorial](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html)
+or also in
+[this one](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html).
+
 ## Supported HPO methods
 
 The following hyperparameter optimization (HPO) methods are available in Syne Tune:
 
 Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer? 
 :--- | :---: | :---: | :---: | :---: | :---: 
 Grid Search |  | deterministic | yes | no | no 
 Random Search | Bergstra, et al. (2011) | random | yes | no | no 
 Bayesian Optimization | Snoek, et al. (2012) | model-based | yes | no | no 
 BORE | Tiao, et al. (2021) | model-based | yes | no | no 
+CQR | Salinas, et al. (2023) | model-based | yes | no | no 
 MedianStoppingRule | Golovin, et al. (2017) | any | yes | yes | no 
 SyncHyperband | Li, et al. (2018) | random | no | yes | no 
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
 HyperTune | Li, et al. (2022) | model-based | yes | yes | no
 DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
-ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no 
+ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no
+ASHACQR | Salinas, et al. (2023) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
 RUSH | Zappella, et al. (2021)| random | yes | yes | yes 
@@ -194,14 +206,20 @@
   launches HPO locally to tune a gluon-ts time series forecasting algorithm
 * [launch_rl_tuning.py](examples/launch_rl_tuning.py):
   launches HPO locally to tune a RL algorithm on the cartpole environment
 * [launch_height_ray.py](examples/launch_height_ray.py):
   launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
   scheduler
 
+## Examples for Experimentation and Benchmarking
+
+You will find many examples for experimentation and benchmarking in
+[benchmarking/examples/](benchmarking/examples/) and in
+benchmarking/nusery/](benchmarking/nursery/).
+
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
 * [What are the different installations options supported?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-different-installations-options-supported)
@@ -238,18 +256,20 @@
 
 Do you want to know more? Here are a number of tutorials.
 * [Basics of Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)
 * [Choosing a Configuration Space](https://syne-tune.readthedocs.io/en/latest/search_space.html)
 * [Using the Built-in Schedulers](https://syne-tune.readthedocs.io/en/latest/schedulers.html)
 * [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
 * [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
+* [Visualization of Results](https://syne-tune.readthedocs.io/en/latest/tutorials/visualization/README.html)
+* [Rapid Experimentation with Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html)
 * [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
 * [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
 * [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
-
+* [Distributed Hyperparameter Tuning: Finding the Right Model can be Fast and Fun](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html)
 
 ## Blog Posts
 
 - [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
 - [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
 - [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
```

### Comparing `syne_tune-0.8.0/setup.py` & `syne_tune-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/__init__.py` & `syne_tune-0.9.0/syne_tune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/__init__.py` & `syne_tune-0.9.0/syne_tune/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/local_backend.py` & `syne_tune-0.9.0/syne_tune/backend/local_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/python_backend/__init__.py` & `syne_tune-0.9.0/syne_tune/backend/python_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/python_backend/python_backend.py` & `syne_tune-0.9.0/syne_tune/backend/python_backend/python_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/python_backend/python_entrypoint.py` & `syne_tune-0.9.0/syne_tune/backend/python_backend/python_entrypoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/__init__.py` & `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/custom_framework.py` & `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/custom_framework.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv` & `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/instance_info.py` & `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/instance_info.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py` & `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py` & `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/simulator_backend/__init__.py` & `syne_tune-0.9.0/syne_tune/backend/simulator_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/simulator_backend/events.py` & `syne_tune-0.9.0/syne_tune/backend/simulator_backend/events.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/simulator_backend/simulator_backend.py` & `syne_tune-0.9.0/syne_tune/backend/simulator_backend/simulator_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/simulator_backend/simulator_callback.py` & `syne_tune-0.9.0/syne_tune/backend/simulator_backend/simulator_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/simulator_backend/time_keeper.py` & `syne_tune-0.9.0/syne_tune/backend/simulator_backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/time_keeper.py` & `syne_tune-0.9.0/syne_tune/backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/trial_backend.py` & `syne_tune-0.9.0/syne_tune/backend/trial_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/backend/trial_status.py` & `syne_tune-0.9.0/syne_tune/backend/trial_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/__init__.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_offline.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_offline.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_surrogate.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_surrogate.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_tabular.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_tabular.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/utils.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/repository.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/repository.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/serialize.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/serialize.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/simulated_tabular_backend.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/simulated_tabular_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/blackbox_repository/utils.py` & `syne_tune-0.9.0/syne_tune/blackbox_repository/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/callbacks/__init__.py` & `syne_tune-0.9.0/syne_tune/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py` & `syne_tune-0.9.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py` & `syne_tune-0.9.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/callbacks/remove_checkpoints_callback.py` & `syne_tune-0.9.0/syne_tune/callbacks/remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/callbacks/tensorboard_callback.py` & `syne_tune-0.9.0/syne_tune/callbacks/tensorboard_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/config_space.py` & `syne_tune-0.9.0/syne_tune/config_space.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/constants.py` & `syne_tune-0.9.0/syne_tune/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/experiments/__init__.py` & `syne_tune-0.9.0/syne_tune/experiments/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,31 +13,35 @@
 from syne_tune.experiments.experiment_result import (
     ExperimentResult,
     load_experiment,
     get_metadata,
     list_experiments,
     load_experiments_df,
 )
-from syne_tune.experiments.plotting import (
+from syne_tune.experiments.visualization.plot_per_trial import (
+    TrialsOfExperimentResults,
+    MultiFidelityParameters,
+)
+from syne_tune.experiments.visualization.plotting import (
     ComparativeResults,
     PlotParameters,
     SubplotParameters,
     ShowTrialParameters,
 )
-from syne_tune.experiments.plot_per_trial import (
-    TrialsOfExperimentResults,
-    MultiFidelityParameters,
+from syne_tune.experiments.visualization.multiobjective import (
+    hypervolume_indicator_column_generator,
 )
 
 __all__ = [
     "ExperimentResult",
     "load_experiment",
     "get_metadata",
     "list_experiments",
     "load_experiments_df",
     "ComparativeResults",
     "PlotParameters",
     "SubplotParameters",
     "ShowTrialParameters",
     "TrialsOfExperimentResults",
     "MultiFidelityParameters",
+    "hypervolume_indicator_column_generator",
 ]
```

### Comparing `syne_tune-0.8.0/syne_tune/experiments/aggregate_results.py` & `syne_tune-0.9.0/syne_tune/experiments/visualization/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/experiments/experiment_result.py` & `syne_tune-0.9.0/syne_tune/experiments/experiment_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         if len(self.metric_names()) > 1 and verbose:
             logger.warning(
                 "Several metrics exists, this will "
                 f"use metric={metric_name} (index={metric}) out of {self.metric_names()}."
             )
 
         metric_mode = self.metric_mode()
-        if len(metric_mode) > 1:
+        if isinstance(metric_mode, list):
             metric_mode = metric_mode[metric]
 
         return metric, metric_name, metric_mode
 
 
 def download_single_experiment(
     tuner_name: str,
```

### Comparing `syne_tune-0.8.0/syne_tune/experiments/multiobjective.py` & `syne_tune-0.9.0/syne_tune/experiments/visualization/multiobjective.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/experiments/plot_per_trial.py` & `syne_tune-0.9.0/syne_tune/experiments/visualization/plot_per_trial.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 import numpy as np
 import pandas as pd
 
 from syne_tune.constants import (
     ST_TUNER_TIME,
 )
-from syne_tune.experiments.plotting import PlotParameters
-from syne_tune.experiments.results_utils import (
+from syne_tune.experiments.visualization.plotting import PlotParameters
+from syne_tune.experiments.visualization.results_utils import (
     MapMetadataToSetup,
     DateTimeBounds,
     create_index_for_result_files,
     load_results_dataframe_per_benchmark,
     download_result_files_from_s3,
     SINGLE_BENCHMARK_KEY,
 )
```

### Comparing `syne_tune-0.8.0/syne_tune/experiments/plotting.py` & `syne_tune-0.9.0/syne_tune/experiments/visualization/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 import logging
 import copy
 
 import numpy as np
 import pandas as pd
 
 from syne_tune.constants import ST_TUNER_TIME
-from syne_tune.experiments.aggregate_results import aggregate_and_errors_over_time
-from syne_tune.experiments.results_utils import (
+from syne_tune.experiments.visualization.aggregate_results import (
+    aggregate_and_errors_over_time,
+)
+from syne_tune.experiments.visualization.results_utils import (
     MapMetadataToSetup,
     MapMetadataToSubplot,
     DateTimeBounds,
     create_index_for_result_files,
     load_results_dataframe_per_benchmark,
     download_result_files_from_s3,
     _insert_into_nested_dict,
```

### Comparing `syne_tune-0.8.0/syne_tune/experiments/results_utils.py` & `syne_tune-0.9.0/syne_tune/experiments/visualization/results_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import pandas as pd
 
 from syne_tune.constants import (
     ST_DATETIME_FORMAT,
     ST_METADATA_FILENAME,
     ST_RESULTS_DATAFRAME_FILENAME,
 )
+from syne_tune.experiments.launchers.utils import sync_from_s3_command
 from syne_tune.util import experiment_path, s3_experiment_path
 
 logger = logging.getLogger(__name__)
 
 
 _MapMetadataToSetup = Callable[[Dict[str, Any]], Optional[str]]
 
@@ -365,26 +366,14 @@
     if not dfs:
         res_df = None
     else:
         res_df = pd.concat(dfs, ignore_index=True)
     return res_df
 
 
-def sync_from_s3_command(experiment_name: str, s3_bucket: Optional[str] = None) -> str:
-    s3_source_path = s3_experiment_path(
-        s3_bucket=s3_bucket, experiment_name=experiment_name
-    )
-    target_path = str(experiment_path() / experiment_name)
-    return (
-        f'aws s3 sync {s3_source_path} {target_path} --exclude "*" '
-        f'--include "*{ST_METADATA_FILENAME}" '
-        f'--include "*{ST_RESULTS_DATAFRAME_FILENAME}"'
-    )
-
-
 def download_result_files_from_s3(
     experiment_names: Tuple[str, ...],
     s3_bucket: Optional[str] = None,
 ):
     """
     Downloads result files from S3. This works only if the result objects on S3
     have prefixes ``f"{s3_experiment_path(s3_bucket)}{ename}/"``, where ``ename``
```

### Comparing `syne_tune-0.8.0/syne_tune/num_gpu.py` & `syne_tune-0.9.0/syne_tune/num_gpu.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/__init__.py` & `syne_tune-0.9.0/syne_tune/experiments/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/baselines.py` & `syne_tune-0.9.0/syne_tune/optimizer/baselines.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,40 +9,44 @@
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Dict, Optional, Any, List, Union
 import logging
 import copy
+from functools import partial
 
 from syne_tune.optimizer.schedulers import (
     FIFOScheduler,
     HyperbandScheduler,
     PopulationBasedTraining,
 )
-from syne_tune.optimizer.schedulers.multiobjective import MOASHA
+from syne_tune.optimizer.schedulers.multiobjective import (
+    MOASHA,
+    MultiObjectiveRegularizedEvolution,
+    NSGA2Searcher,
+    LinearScalarizedScheduler,
+)
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.estimator import Estimator
 from syne_tune.optimizer.schedulers.searchers.regularized_evolution import (
     RegularizedEvolution,
 )
-from syne_tune.optimizer.schedulers.multiobjective.multi_objective_regularized_evolution import (
-    MultiObjectiveRegularizedEvolution,
-)
-from syne_tune.optimizer.schedulers.multiobjective.nsga2_searcher import NSGA2Searcher
 from syne_tune.optimizer.schedulers.synchronous import (
     SynchronousGeometricHyperbandScheduler,
     GeometricDifferentialEvolutionHyperbandScheduler,
 )
 from syne_tune.optimizer.schedulers.transfer_learning import (
     TransferLearningTaskEvaluations,
 )
 from syne_tune.optimizer.schedulers.random_seeds import RandomSeedGenerator
 from syne_tune.try_import import (
     try_import_blackbox_repository_message,
     try_import_bore_message,
     try_import_botorch_message,
+    try_import_moo_message,
 )
 from syne_tune.util import dict_get
 
 logger = logging.getLogger(__name__)
 
 
 def _random_seed_from_generator(random_seed: int) -> int:
@@ -729,14 +733,159 @@
             metric=metric,
             searcher=RegularizedEvolution(**searcher_kwargs),
             random_seed=random_seed,
             **kwargs,
         )
 
 
+def create_gaussian_process_estimator(
+    config_space: Dict[str, Any],
+    metric: str,
+    mode: Optional[str] = None,
+    random_seed: Optional[int] = None,
+    search_options: Optional[Dict[str, Any]] = None,
+) -> Estimator:
+    scheduler = BayesianOptimization(
+        config_space=config_space,
+        metric=metric,
+        mode=mode,
+        random_seed=random_seed,
+        search_options=search_options,
+    )
+    searcher = scheduler.searcher  # GPFIFOSearcher
+    state_transformer = searcher.state_transformer  # ModelStateTransformer
+    estimator = state_transformer.estimator  # GaussProcEmpiricalBayesEstimator
+
+    # update the estimator properties
+    estimator.active_metric = metric
+    return estimator
+
+
+class MORandomScalarizationBayesOpt(FIFOScheduler):
+    """
+    Uses :class:`~syne_tune.optimizer.schedulers.multiobjective.MultiObjectiveMultiSurrogateSearcher`
+    with one standard GP surrogate model per metric (same as in
+    :class:`BayesianOptimization`, together with the
+    :class:`~syne_tune.optimizer.schedulers.multiobjective.MultiObjectiveLCBRandomLinearScalarization`
+    acquisition function.
+
+    If `estimators` is given, surrogate models are taken from there, and the
+    default is used otherwise. This is useful if you have a good low-variance
+    model for one of the objectives.
+
+    :param config_space: Configuration space for evaluation function
+    :param metric: Name of metrics to optimize
+    :param mode: Modes of optimization. Defaults to "min" for all
+    :param random_seed: Random seed, optional
+    :param estimators: Use these surrogate models instead of the default GP
+        one. Optional
+    :param kwargs: Additional arguments to
+        :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`. Here,
+        ``kwargs["search_options"]`` is used to create the searcher and its
+        GP surrogate models.
+    """
+
+    def __init__(
+        self,
+        config_space: Dict[str, Any],
+        metric: List[str],
+        mode: Union[List[str], str] = "min",
+        random_seed: Optional[int] = None,
+        estimators: Optional[Dict[str, Estimator]] = None,
+        **kwargs,
+    ):
+        try:
+            from syne_tune.optimizer.schedulers.multiobjective import (
+                MultiObjectiveMultiSurrogateSearcher,
+                MultiObjectiveLCBRandomLinearScalarization,
+            )
+        except ImportError:
+            logging.info(try_import_moo_message())
+            raise
+
+        searcher_kwargs = _create_searcher_kwargs(
+            config_space, metric, random_seed, kwargs
+        )
+        searcher_kwargs["mode"] = mode
+        if estimators is None:
+            estimators = dict()
+        else:
+            estimators = estimators.copy()
+        if isinstance(mode, str):
+            mode = [mode] * len(metric)
+        if "search_options" in kwargs:
+            search_options = kwargs["search_options"].copy()
+        else:
+            search_options = dict()
+        search_options["no_fantasizing"] = True
+        for _metric, _mode in zip(metric, mode):
+            if _metric not in estimators:
+                estimators[_metric] = create_gaussian_process_estimator(
+                    config_space=config_space,
+                    metric=_metric,
+                    mode=_mode,
+                    search_options=search_options,
+                )
+        searcher = MultiObjectiveMultiSurrogateSearcher(
+            config_space=config_space,
+            metric=metric,
+            mode=mode,
+            estimators=estimators,
+            scoring_class=partial(
+                MultiObjectiveLCBRandomLinearScalarization, random_seed=random_seed
+            ),
+            random_seed=random_seed,
+        )
+        super().__init__(
+            config_space=config_space,
+            metric=metric,
+            mode=mode,
+            searcher=searcher,
+            random_seed=random_seed,
+            **kwargs,
+        )
+
+
+class NSGA2(FIFOScheduler):
+    """
+    See :class:`~syne_tune.optimizer.schedulers.searchers.RandomSearcher`
+    for ``kwargs["search_options"]`` parameters.
+
+    :param config_space: Configuration space for evaluation function
+    :param metric: Name of metric to optimize
+    :param population_size: The size of the population for NSGA-2
+    :param random_seed: Random seed, optional
+    :param kwargs: Additional arguments to
+        :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`
+    """
+
+    def __init__(
+        self,
+        config_space: Dict[str, Any],
+        metric: List[str],
+        mode: Union[List[str], str] = "min",
+        population_size: int = 20,
+        random_seed: Optional[int] = None,
+        **kwargs,
+    ):
+        searcher_kwargs = _create_searcher_kwargs(
+            config_space, metric, random_seed, kwargs
+        )
+        searcher_kwargs["mode"] = mode
+        searcher_kwargs["population_size"] = population_size
+        super(NSGA2, self).__init__(
+            config_space=config_space,
+            metric=metric,
+            mode=mode,
+            searcher=NSGA2Searcher(**searcher_kwargs),
+            random_seed=random_seed,
+            **kwargs,
+        )
+
+
 class MOREA(FIFOScheduler):
     """
 
     See :class:`~syne_tune.optimizer.schedulers.searchers.RandomSearcher`
     for ``kwargs["search_options"]`` parameters.
 
     :param config_space: Configuration space for evaluation function
@@ -774,48 +923,44 @@
             mode=mode,
             searcher=MultiObjectiveRegularizedEvolution(**searcher_kwargs),
             random_seed=random_seed,
             **kwargs,
         )
 
 
-class NSGA2(FIFOScheduler):
+class MOLinearScalarizationBayesOpt(LinearScalarizedScheduler):
     """
+    Uses :class:`~syne_tune.optimizer.schedulers.multiobjective.LinearScalarizedScheduler`
+    together with a default GP surrogate model.
 
-    See :class:`~syne_tune.optimizer.schedulers.searchers.RandomSearcher`
+    See :class:`~syne_tune.optimizer.schedulers.searchers.GPFIFOSearcher`
     for ``kwargs["search_options"]`` parameters.
 
     :param config_space: Configuration space for evaluation function
     :param metric: Name of metric to optimize
-    :param population_size: The size of the population for NSGA-2
-    :param random_seed: Random seed, optional
+    :param scalarization_weights: Positive weight used for the scalarization.
+        Defaults to all 1
     :param kwargs: Additional arguments to
         :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`
     """
 
     def __init__(
         self,
         config_space: Dict[str, Any],
         metric: List[str],
-        mode: Union[List[str], str] = "min",
-        population_size: int = 20,
-        random_seed: Optional[int] = None,
+        scalarization_weights: Optional[List[float]] = None,
         **kwargs,
     ):
-        searcher_kwargs = _create_searcher_kwargs(
-            config_space, metric, random_seed, kwargs
-        )
-        searcher_kwargs["mode"] = mode
-        searcher_kwargs["population_size"] = population_size
-        super(NSGA2, self).__init__(
+        searcher_name = "bayesopt"
+        _assert_searcher_must_be(kwargs, searcher_name)
+        super().__init__(
             config_space=config_space,
             metric=metric,
-            mode=mode,
-            searcher=NSGA2Searcher(**searcher_kwargs),
-            random_seed=random_seed,
+            scalarization_weights=scalarization_weights,
+            searcher=searcher_name,
             **kwargs,
         )
 
 
 class ConstrainedBayesianOptimization(FIFOScheduler):
     """Constrained Bayesian Optimization.
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/scheduler.py` & `syne_tune-0.9.0/syne_tune/optimizer/scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/fifo.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/fifo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_pasha.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_pasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_promotion.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_rush.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_stopping.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_stopping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/median_stopping_rule.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/median_stopping_rule.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multi_fidelity.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 import logging
 from functools import partial
-from typing import Optional, List, Dict, Any
+from typing import Optional, List, Dict, Any, Union
 
 from syne_tune.optimizer.schedulers.multiobjective.random_scalarization import (
     MultiObjectiveLCBRandomLinearScalarization,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     TrialEvaluations,
 )
@@ -69,15 +69,15 @@
     """
 
     def __init__(
         self,
         config_space: Dict[str, Any],
         metric: List[str],
         estimators: Dict[str, Estimator],
-        mode: Optional[List[str]] = None,
+        mode: Union[List[str], str] = "min",
         points_to_evaluate: Optional[List[Dict[str, Any]]] = None,
         scoring_class: Optional[ScoringFunctionConstructor] = None,
         num_initial_candidates: int = DEFAULT_NUM_INITIAL_CANDIDATES,
         num_initial_random_choices: int = DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS,
         allow_duplicates: bool = False,
         restrict_configurations: Optional[List[Dict[str, Any]]] = None,
         clone_from_state: bool = False,
@@ -124,16 +124,17 @@
         metrics = {name: result[name] for name in self._metric}
 
         self.state_transformer.label_trial(
             TrialEvaluations(trial_id=trial_id, metrics=metrics), config=config
         )
         if self.debug_log is not None:
             _trial_id = self._trial_id_string(trial_id, result)
-            msg = f"Update for trial_id {_trial_id}: metric = {metrics:.3f}"
-            logger.info(msg)
+            part = ",".join(f"{k}:{v:.3f}" for k, v in metrics.items())
+            msg = f"Update for trial_id {_trial_id}: metrics = ["
+            logger.info(msg + part + "]")
 
     def clone_from_state(self, state):
         # Create clone with mutable state taken from 'state'
         init_state = decode_state(state["state"], self._hp_ranges_in_state())
         estimator = self.state_transformer.estimator
         # Call internal constructor
         new_searcher = MultiObjectiveMultiSurrogateSearcher(
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Dict, Optional, Iterable, List, Callable
 
 import numpy as np
-import scipy.stats
 from numpy.random import RandomState
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     Predictor,
     ScoringFunction,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
@@ -70,27 +69,28 @@
         self.weights_sampler = weights_sampler
 
     def score(
         self,
         candidates: Iterable[Configuration],
         predictor: Optional[Dict[str, Predictor]] = None,
     ) -> List[float]:
+        from scipy import stats
 
         if predictor is None:
             predictor = self.predictor
         weights = self.weights_sampler()
         scores = np.zeros(len(candidates))
         for metric, metric_predictor in predictor.items():
             predictions = metric_predictor.predict_candidates(candidates)
             predicted_mean = predictions[0]["mean"]
             predicted_std = predictions[0]["std"]
 
             metric_score = self._single_objective_score(predicted_mean, predicted_std)
             if self.normalize_acquisition:
-                metrics_score_normalized = scipy.stats.rankdata(metric_score)
+                metrics_score_normalized = stats.rankdata(metric_score)
                 metrics_score_normalized = (
                     metrics_score_normalized / metrics_score_normalized.max()
                 )
             scores += metrics_score_normalized * weights[metric]
         return list(scores)
 
     def _single_objective_score(self, mean: np.ndarray, std: np.ndarray) -> np.ndarray:
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/utils.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/networks.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/networks.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/pbt.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/pbt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/random_seeds.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/random_seeds.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/ray_scheduler.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/ray_scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/remove_checkpoints.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/remove_checkpoints.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/scheduler_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/scheduler_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,41 +26,41 @@
 from syne_tune.optimizer.schedulers.searchers.random_grid_searcher import (  # noqa: F401
     RandomSearcher,
     GridSearcher,
 )
 from syne_tune.optimizer.schedulers.searchers.searcher_factory import (  # noqa: F401
     searcher_factory,
 )
-from syne_tune.optimizer.schedulers.searchers.model_based_searcher import (  # noqa: F401
-    ModelBasedSearcher,
-    BayesianOptimizationSearcher,
-)
 
 __all__ = [
     "BaseSearcher",
     "impute_points_to_evaluate",
     "StochasticSearcher",
     "StochasticAndFilterDuplicatesSearcher",
     "extract_random_seed",
     "RandomSearcher",
     "GridSearcher",
     "searcher_factory",
-    "ModelBasedSearcher",
-    "BayesianOptimizationSearcher",
 ]
 
 try:
+    from syne_tune.optimizer.schedulers.searchers.model_based_searcher import (  # noqa: F401
+        ModelBasedSearcher,
+        BayesianOptimizationSearcher,
+    )
     from syne_tune.optimizer.schedulers.searchers.gp_fifo_searcher import (  # noqa: F401
         GPFIFOSearcher,
     )
     from syne_tune.optimizer.schedulers.searchers.gp_multifidelity_searcher import (  # noqa: F401
         GPMultiFidelitySearcher,
     )
 
     __all__.extend(
         [
+            "ModelBasedSearcher",
+            "BayesianOptimizationSearcher",
             "GPFIFOSearcher",
             "GPMultiFidelitySearcher",
         ]
     )
 except ImportError:
     logging.info(try_import_gpsearchers_message())
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py` & `syne_tune-0.9.0/syne_tune/experiments/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         ``update_params == True``. Otherwise, these parameters are not changed,
         but only the posterior state is computed.
         If your surrogate model is not Bayesian, or does not have hyperparameters,
         you can ignore the ``update_params`` argument.
 
         If ``self.state.pending_evaluations`` is not empty, we compute posterior for state without pending evals.
         This method can be overwritten for any other behaviour such as one found in
-        ``syne_tune.optimizer.schedulers.searchers.bayesopt.models.gp_model.GaussProcEstimator.fit_from_state``
+        :meth:`~syne_tune.optimizer.schedulers.searchers.bayesopt.models.gp_model.GaussProcEstimator.fit_from_state`.
 
         :param state: Current data model parameters are to be fit on, and the
             posterior state is to be computed from
         :param update_params: See above
         :return: Predictor, wrapping the posterior state
         """
         if state.pending_evaluations:
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/de.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/de.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 import logging
 import numpy as np
 
 from syne_tune.optimizer.schedulers.searchers import (
     BaseSearcher,
     GPMultiFidelitySearcher,
 )
+from syne_tune.optimizer.schedulers.searchers.dyhpo.hyperband_dyhpo import (
+    KEY_NEW_CONFIGURATION,
+)
 from syne_tune.optimizer.schedulers.searchers.model_based_searcher import (
     create_initial_candidates_scorer,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
@@ -42,17 +45,14 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.meanstd_acqfunc_impl import (
     EIAcquisitionFunction,
 )
 
 logger = logging.getLogger(__name__)
 
 
-KEY_NEW_CONFIGURATION = "new_configuration"
-
-
 INTERNAL_KEY = "RESERVED_KEY_31415927"
 
 
 # DEBUG:
 def _debug_print_info(
     resource: int, scores: List[float], acq_function: EIAcquisitionFunction
 ):
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 from numpy.random import RandomState
 import logging
 from collections import Counter
 
 from syne_tune.optimizer.schedulers.hyperband_promotion import (
     PromotionRungSystem,
 )
-from syne_tune.optimizer.schedulers.searchers.dyhpo.dyhpo_searcher import (
-    DynamicHPOSearcher,
-    KEY_NEW_CONFIGURATION,
-)
+from syne_tune.optimizer.schedulers.searchers import BaseSearcher
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_SH_PROBABILITY = 0.25
 
 
+KEY_NEW_CONFIGURATION = "new_configuration"
+
+
 class ScheduleDecision:
     PROMOTE_SH = 0
     PROMOTE_DYHPO = 1
     START_DYHPO = 2
 
 
 _SUMMARY_SCHEDULE_RECORDS = [
@@ -96,22 +96,19 @@
         self,
         rung_levels: List[int],
         promote_quantiles: List[float],
         metric: str,
         mode: str,
         resource_attr: str,
         max_t: int,
-        searcher: DynamicHPOSearcher,
+        searcher: BaseSearcher,
         probability_sh: bool,
         random_state: RandomState,
     ):
         assert len(rung_levels) > 0, "rung_levels must not be empty"
-        assert isinstance(
-            searcher, DynamicHPOSearcher
-        ), "searcher must be of type DynamicHPOSearcher. Use searcher='dyhpo'"
         assert (
             0 <= probability_sh < 1
         ), f"probability_sh = {probability_sh}, must be in [0, 1)"
         super().__init__(
             rung_levels, promote_quantiles, metric, mode, resource_attr, max_t
         )
         self._check_rung_levels(rung_levels)
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -893,15 +893,15 @@
         "opt_debug_writer": False,
         "num_fantasy_samples": 20,
         "scheduler": "fifo",
         "num_init_random": DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS,
         "num_init_candidates": DEFAULT_NUM_INITIAL_CANDIDATES,
         "initial_scoring": DEFAULT_INITIAL_SCORING,
         "skip_local_optimization": False,
-        "debug_log": True,
+        "debug_log": False,
         "cost_attr": "elapsed_time",
         "normalize_targets": True,
         "no_fantasizing": False,
         "allow_duplicates": False,
         "input_warping": False,
         "boxcox_transform": False,
         "max_size_top_fraction": 0.25,
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/common.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Tuple, Dict, List, Any, Optional, Union
 import numpy as np
-from autograd import numpy as anp
 
 from syne_tune.config_space import (
     Domain,
     FiniteRange,
     Categorical,
     Ordinal,
     OrdinalNearestNeighbor,
@@ -835,11 +834,11 @@
     :return: ``(features, resources)``
     """
     r_min, r_max = resource_attr_range
     features = features_ext[:, :-1]
     resources_encoded = features_ext[:, -1].reshape((-1,))
     lower = r_min - 0.5 + EPS
     width = r_max - r_min + 1 - 2 * EPS
-    resources = anp.clip(
-        anp.round(resources_encoded * width + lower), r_min, r_max
+    resources = np.clip(
+        np.round(resources_encoded * width + lower), r_min, r_max
     ).astype("int64")
     return features, resources
```

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/successive_halving.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/successive_halving.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/remote/__init__.py` & `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/remote/estimators.py` & `syne_tune-0.9.0/syne_tune/remote/estimators.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,43 +6,38 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
+from syne_tune.remote.constants import (
+    DEFAULT_CPU_INSTANCE,
+    PYTORCH_LATEST_FRAMEWORK,
+    PYTORCH_LATEST_PY_VERSION,
+    HUGGINGFACE_LATEST_FRAMEWORK_VERSION,
+    HUGGINGFACE_LATEST_PYTORCH_VERSION,
+    HUGGINGFACE_LATEST_TRANSFORMERS_VERSION,
+    HUGGINGFACE_LATEST_PY_VERSION,
+    MXNET_LATEST_PY_VERSION,
+    MXNET_LATEST_VERSION,
+)
 from syne_tune.try_import import try_import_aws_message
 
 try:
     from sagemaker.pytorch import PyTorch
     from sagemaker.huggingface import HuggingFace
     from sagemaker.mxnet import MXNet
     from sagemaker.tensorflow import TensorFlow
     from sagemaker.sklearn import SKLearn
     from sagemaker.chainer import Chainer
     from sagemaker.xgboost import XGBoost
 except ImportError:
     print(try_import_aws_message())
 
-DEFAULT_CPU_INSTANCE = "ml.c5.4xlarge"
-DEFAULT_CPU_INSTANCE_SMALL = "ml.m5.large"
-DEFAULT_GPU_INSTANCE_1GPU = "ml.g4dn.xlarge"
-DEFAULT_GPU_INSTANCE_4GPU = "ml.g4dn.12xlarge"
-
-PYTORCH_LATEST_FRAMEWORK = "1.12.1"
-PYTORCH_LATEST_PY_VERSION = "py38"
-
-HUGGINGFACE_LATEST_FRAMEWORK_VERSION = "4.4"
-HUGGINGFACE_LATEST_PYTORCH_VERSION = "1.7.1"
-HUGGINGFACE_LATEST_TRANSFORMERS_VERSION = "4.6.1"
-HUGGINGFACE_LATEST_PY_VERSION = "py36"
-
-MXNET_LATEST_PY_VERSION = "py38"
-MXNET_LATEST_VERSION = "1.9.0"
-
 
 def instance_sagemaker_estimator(**kwargs):
     """
     Returns SageMaker estimator to be used for simulator back-end experiments
     and for remote launching of SageMaker back-end experiments.
 
     :param kwargs: Extra arguments to SageMaker estimator
```

### Comparing `syne_tune-0.8.0/syne_tune/remote/remote_launcher.py` & `syne_tune-0.9.0/syne_tune/remote/remote_launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 import boto3
 
 import syne_tune
 from syne_tune import Tuner
 from syne_tune.remote.estimators import (
     instance_sagemaker_estimator,
-    DEFAULT_CPU_INSTANCE,
 )
+from syne_tune.remote.constants import DEFAULT_CPU_INSTANCE
 from syne_tune.remote.remote_metrics_callback import RemoteTuningMetricsCallback
 from syne_tune.backend.sagemaker_backend.sagemaker_utils import (
     add_syne_tune_dependency,
     get_execution_role,
 )
 from syne_tune.constants import ST_REMOTE_UPLOAD_DIR_NAME
 from syne_tune.util import s3_experiment_path
@@ -199,17 +199,19 @@
         )
         if endpoint_requirements.exists():
             logger.info(
                 f"copy endpoint script requirements to {self.remote_script_dir()}"
             )
             shutil.copy(endpoint_requirements, tgt_requirement)
 
-        # add tuner requirements, this will create the req file if it does not exist
+        # Add tuner requirements, this will create the req file if it does not exist
+        # The leading "\n" makes sure this works even if the file behind
+        # ``tgt_requirement`` does not end with "\n"
         with open(tgt_requirement, "a") as reqf:
-            reqf.write("syne-tune[extra]\n")
+            reqf.write("\nsyne-tune[extra]\n")
 
     def get_source_dir(self) -> Path:
         # note: this logic would be better moved to the backend.
         if self.is_source_dir_specified():
             return Path(self.tuner.trial_backend.source_dir)
         else:
             return Path(self.tuner.trial_backend.entrypoint_path()).parent
```

### Comparing `syne_tune-0.8.0/syne_tune/remote/remote_main.py` & `syne_tune-0.9.0/syne_tune/remote/remote_main.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/remote/remote_metrics_callback.py` & `syne_tune-0.9.0/syne_tune/remote/remote_metrics_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/remote/scheduling.py` & `syne_tune-0.9.0/syne_tune/remote/scheduling.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/report.py` & `syne_tune-0.9.0/syne_tune/report.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/results_callback.py` & `syne_tune-0.9.0/syne_tune/results_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/stopping_criterion.py` & `syne_tune-0.9.0/syne_tune/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/try_import.py` & `syne_tune-0.9.0/syne_tune/try_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/tuner.py` & `syne_tune-0.9.0/syne_tune/tuner.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/tuner_callback.py` & `syne_tune-0.9.0/syne_tune/tuner_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/tuning_status.py` & `syne_tune-0.9.0/syne_tune/tuning_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/util.py` & `syne_tune-0.9.0/syne_tune/util.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/utils/__init__.py` & `syne_tune-0.9.0/syne_tune/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/utils/checkpoint.py` & `syne_tune-0.9.0/syne_tune/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/utils/config_as_json.py` & `syne_tune-0.9.0/syne_tune/utils/config_as_json.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune/utils/parse_bool.py` & `syne_tune-0.9.0/syne_tune/utils/parse_bool.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.8.0/syne_tune.egg-info/PKG-INFO` & `syne_tune-0.9.0/syne_tune.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne-tune
-Version: 0.8.0
+Version: 0.9.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -135,35 +135,47 @@
     n_workers=4,  # how many trials are evaluated in parallel
 )
 tuner.run()
 ```
 
 The above example runs ASHA with 4 asynchronous workers on a local machine.
 
+## Experimentation with Syne Tune
+
+If you plan to use advanced features of Syne Tune, such as different execution
+backends or running experiments remotely, writing launcher scripts like
+`examples/launch_height_simple.py` can become tedious. Syne Tune provides an
+advanced experimentation framework, which you can learn about in
+[this tutorial](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html)
+or also in
+[this one](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html).
+
 ## Supported HPO methods
 
 The following hyperparameter optimization (HPO) methods are available in Syne Tune:
 
 Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer? 
 :--- | :---: | :---: | :---: | :---: | :---: 
 Grid Search |  | deterministic | yes | no | no 
 Random Search | Bergstra, et al. (2011) | random | yes | no | no 
 Bayesian Optimization | Snoek, et al. (2012) | model-based | yes | no | no 
 BORE | Tiao, et al. (2021) | model-based | yes | no | no 
+CQR | Salinas, et al. (2023) | model-based | yes | no | no 
 MedianStoppingRule | Golovin, et al. (2017) | any | yes | yes | no 
 SyncHyperband | Li, et al. (2018) | random | no | yes | no 
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
 HyperTune | Li, et al. (2022) | model-based | yes | yes | no
 DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
-ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no 
+ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no
+ASHACQR | Salinas, et al. (2023) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
 RUSH | Zappella, et al. (2021)| random | yes | yes | yes 
@@ -223,14 +235,20 @@
   launches HPO locally to tune a gluon-ts time series forecasting algorithm
 * [launch_rl_tuning.py](examples/launch_rl_tuning.py):
   launches HPO locally to tune a RL algorithm on the cartpole environment
 * [launch_height_ray.py](examples/launch_height_ray.py):
   launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
   scheduler
 
+## Examples for Experimentation and Benchmarking
+
+You will find many examples for experimentation and benchmarking in
+[benchmarking/examples/](benchmarking/examples/) and in
+benchmarking/nusery/](benchmarking/nursery/).
+
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
 * [What are the different installations options supported?](https://syne-tune.readthedocs.io/en/latest/faq.html#what-are-the-different-installations-options-supported)
@@ -267,18 +285,20 @@
 
 Do you want to know more? Here are a number of tutorials.
 * [Basics of Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)
 * [Choosing a Configuration Space](https://syne-tune.readthedocs.io/en/latest/search_space.html)
 * [Using the Built-in Schedulers](https://syne-tune.readthedocs.io/en/latest/schedulers.html)
 * [Multi-Fidelity Hyperparameter Optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html)
 * [Benchmarking in Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/benchmarking/README.html)
+* [Visualization of Results](https://syne-tune.readthedocs.io/en/latest/tutorials/visualization/README.html)
+* [Rapid Experimentation with Syne Tune](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html)
 * [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
 * [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
 * [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
-
+* [Distributed Hyperparameter Tuning: Finding the Right Model can be Fast and Fun](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html)
 
 ## Blog Posts
 
 - [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
 - [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
 - [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
```

### Comparing `syne_tune-0.8.0/syne_tune.egg-info/SOURCES.txt` & `syne_tune-0.9.0/syne_tune.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -65,20 +65,39 @@
 syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
 syne_tune/callbacks/__init__.py
 syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
 syne_tune/callbacks/hyperband_remove_checkpoints_score.py
 syne_tune/callbacks/remove_checkpoints_callback.py
 syne_tune/callbacks/tensorboard_callback.py
 syne_tune/experiments/__init__.py
-syne_tune/experiments/aggregate_results.py
+syne_tune/experiments/baselines.py
+syne_tune/experiments/default_baselines.py
 syne_tune/experiments/experiment_result.py
-syne_tune/experiments/multiobjective.py
-syne_tune/experiments/plot_per_trial.py
-syne_tune/experiments/plotting.py
-syne_tune/experiments/results_utils.py
+syne_tune/experiments/benchmark_definitions/__init__.py
+syne_tune/experiments/benchmark_definitions/common.py
+syne_tune/experiments/benchmark_definitions/fcnet.py
+syne_tune/experiments/benchmark_definitions/lcbench.py
+syne_tune/experiments/benchmark_definitions/nas201.py
+syne_tune/experiments/benchmark_definitions/yahpo.py
+syne_tune/experiments/launchers/__init__.py
+syne_tune/experiments/launchers/hpo_main_common.py
+syne_tune/experiments/launchers/hpo_main_local.py
+syne_tune/experiments/launchers/hpo_main_sagemaker.py
+syne_tune/experiments/launchers/hpo_main_simulator.py
+syne_tune/experiments/launchers/launch_remote_common.py
+syne_tune/experiments/launchers/launch_remote_local.py
+syne_tune/experiments/launchers/launch_remote_sagemaker.py
+syne_tune/experiments/launchers/launch_remote_simulator.py
+syne_tune/experiments/launchers/utils.py
+syne_tune/experiments/visualization/__init__.py
+syne_tune/experiments/visualization/aggregate_results.py
+syne_tune/experiments/visualization/multiobjective.py
+syne_tune/experiments/visualization/plot_per_trial.py
+syne_tune/experiments/visualization/plotting.py
+syne_tune/experiments/visualization/results_utils.py
 syne_tune/optimizer/__init__.py
 syne_tune/optimizer/baselines.py
 syne_tune/optimizer/scheduler.py
 syne_tune/optimizer/schedulers/__init__.py
 syne_tune/optimizer/schedulers/fifo.py
 syne_tune/optimizer/schedulers/hyperband.py
 syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
@@ -248,14 +267,15 @@
 syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
 syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
 syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
 syne_tune/optimizer/schedulers/utils/__init__.py
 syne_tune/optimizer/schedulers/utils/simple_profiler.py
 syne_tune/optimizer/schedulers/utils/successive_halving.py
 syne_tune/remote/__init__.py
+syne_tune/remote/constants.py
 syne_tune/remote/estimators.py
 syne_tune/remote/remote_launcher.py
 syne_tune/remote/remote_main.py
 syne_tune/remote/remote_metrics_callback.py
 syne_tune/remote/scheduling.py
 syne_tune/utils/__init__.py
 syne_tune/utils/checkpoint.py
```

### Comparing `syne_tune-0.8.0/syne_tune.egg-info/requires.txt` & `syne_tune-0.9.0/syne_tune.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
 s3fs
 
 [benchmarks]
-datasets==1.8.0
 tqdm
-torchvision
 torch
+torchvision
 filelock
+datasets==1.8.0
 transformers
 
 [blackbox-repository]
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet==0.8.1
 s3fs
@@ -76,36 +76,37 @@
 matplotlib
 scikit-learn
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet==0.8.1
 xgboost
 h5py
-datasets==1.8.0
 tqdm
-torchvision
 torch
+torchvision
 filelock
+datasets==1.8.0
 transformers
 onnxruntime>=1.10.0
-configspace
+configspace<=0.6.1
 yahpo-gym
 ray[tune]>=2.0.0
 scikit-optimize
 botorch>=0.7.2
 
 [gpsearchers]
 scipy>=1.3.3
 autograd>=1.3
 
 [kde]
 statsmodels
 
 [moo]
 pymoo>=0.6.0
+scipy>=1.3.3
 
 [raytune]
 ray[tune]>=2.0.0
 scikit-learn
 scikit-optimize
 
 [sklearn]
@@ -113,10 +114,10 @@
 
 [visual]
 matplotlib
 
 [yahpo]
 onnxruntime>=1.10.0
 pyyaml
-configspace
+configspace<=0.6.1
 pandas
 yahpo-gym
```

