# Comparing `tmp/robomimic-0.2.0.tar.gz` & `tmp/robomimic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robomimic-0.2.0.tar", last modified: Fri Dec 17 18:57:38 2021, max compression
+gzip compressed data, was "robomimic-0.3.0.tar", last modified: Tue Jul  4 00:50:50 2023, max compression
```

## Comparing `robomimic-0.2.0.tar` & `robomimic-0.3.0.tar`

### file list

```diff
@@ -1,108 +1,116 @@
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.146937 robomimic-0.2.0/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     1089 2021-07-20 20:45:12.000000 robomimic-0.2.0/LICENSE
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)      312 2021-07-20 20:46:16.000000 robomimic-0.2.0/MANIFEST.in
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6327 2021-12-17 18:57:38.146817 robomimic-0.2.0/PKG-INFO
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6364 2021-12-17 18:52:11.000000 robomimic-0.2.0/README.md
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.131765 robomimic-0.2.0/examples/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     9137 2021-12-17 18:52:11.000000 robomimic-0.2.0/examples/add_new_modality.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     1291 2021-07-20 23:18:54.000000 robomimic-0.2.0/examples/simple_config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     4599 2021-12-17 18:52:11.000000 robomimic-0.2.0/examples/simple_obs_nets.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6043 2021-12-17 18:52:11.000000 robomimic-0.2.0/examples/simple_train_loop.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    22884 2021-12-17 18:52:11.000000 robomimic-0.2.0/examples/train_bc_rnn.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.131997 robomimic-0.2.0/robomimic/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     7133 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/__init__.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.134203 robomimic-0.2.0/robomimic/algo/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)      612 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/algo/__init__.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    15951 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/algo/algo.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    23775 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/algo/bc.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    44533 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/algo/bcq.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    29777 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/algo/cql.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    28386 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/algo/gl.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    12936 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/algo/hbc.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6819 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/algo/iris.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    22248 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/algo/td3_bc.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.136154 robomimic-0.2.0/robomimic/config/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)      570 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/config/__init__.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    16265 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/config/base_config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5551 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/config/bc_config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5785 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/config/bcq_config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    11279 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/config/config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5618 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/config/cql_config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5131 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/config/gl_config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     4068 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/config/hbc_config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     4408 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/config/iris_config.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5755 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/config/td3_bc_config.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.136806 robomimic-0.2.0/robomimic/envs/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)        0 2021-07-20 20:47:32.000000 robomimic-0.2.0/robomimic/envs/__init__.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5868 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/envs/env_base.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     8277 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/envs/env_gym.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    14348 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/envs/env_ig_momart.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    13969 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/envs/env_robosuite.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.129877 robomimic-0.2.0/robomimic/exps/
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.138113 robomimic-0.2.0/robomimic/exps/templates/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     7843 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/exps/templates/bc.json
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     9082 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/exps/templates/bcq.json
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     7381 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/exps/templates/cql.json
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     7412 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/exps/templates/gl.json
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    14024 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/exps/templates/hbc.json
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    24446 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/exps/templates/iris.json
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6835 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/exps/templates/td3_bc.json
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.139728 robomimic-0.2.0/robomimic/models/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)       47 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/models/__init__.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    52131 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/models/base_nets.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     4673 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/models/distributions.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    34703 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/models/obs_nets.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    46080 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/models/policy_nets.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    58845 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/models/vae_nets.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    12072 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/models/value_nets.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.141927 robomimic-0.2.0/robomimic/scripts/
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.142398 robomimic-0.2.0/robomimic/scripts/conversion/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5362 2021-07-20 20:47:32.000000 robomimic-0.2.0/robomimic/scripts/conversion/convert_d4rl.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     2413 2021-07-20 20:47:32.000000 robomimic-0.2.0/robomimic/scripts/conversion/convert_robosuite.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6878 2021-07-22 22:50:53.000000 robomimic-0.2.0/robomimic/scripts/conversion/convert_roboturk_pilot.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    11185 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/scripts/dataset_states_to_obs.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     7108 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/scripts/download_datasets.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6766 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/scripts/download_momart_datasets.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5436 2021-07-23 01:46:55.000000 robomimic-0.2.0/robomimic/scripts/extract_obs_from_raw_datasets.sh
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)      871 2021-07-20 20:47:32.000000 robomimic-0.2.0/robomimic/scripts/generate_config_templates.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    62602 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/scripts/generate_paper_configs.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5188 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/scripts/get_dataset_info.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     4407 2021-07-20 20:47:32.000000 robomimic-0.2.0/robomimic/scripts/hyperparam_helper.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    13087 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/scripts/playback_dataset.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    13499 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/scripts/run_trained_agent.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     3566 2021-07-20 20:47:32.000000 robomimic-0.2.0/robomimic/scripts/split_train_val.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    15575 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/scripts/train.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.145232 robomimic-0.2.0/robomimic/utils/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)        0 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/utils/__init__.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    26037 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/utils/dataset.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     9136 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/utils/env_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    14099 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/utils/file_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    12644 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/utils/hyperparam_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     4321 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/utils/log_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     7576 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/utils/loss_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)      188 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/utils/macros.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    37689 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/utils/obs_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     2999 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/utils/python_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    30262 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/utils/tensor_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     8749 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/utils/test_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6153 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/utils/torch_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    21666 2021-12-17 18:52:11.000000 robomimic-0.2.0/robomimic/utils/train_utils.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     1603 2021-07-20 20:47:31.000000 robomimic-0.2.0/robomimic/utils/vis_utils.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.132669 robomimic-0.2.0/robomimic.egg-info/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6327 2021-12-17 18:57:38.000000 robomimic-0.2.0/robomimic.egg-info/PKG-INFO
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     2748 2021-12-17 18:57:38.000000 robomimic-0.2.0/robomimic.egg-info/SOURCES.txt
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)        1 2021-12-17 18:57:38.000000 robomimic-0.2.0/robomimic.egg-info/dependency_links.txt
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)        2 2021-12-17 18:57:38.000000 robomimic-0.2.0/robomimic.egg-info/eager_resources.txt
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)      124 2021-12-17 18:57:38.000000 robomimic-0.2.0/robomimic.egg-info/requires.txt
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)       10 2021-12-17 18:57:38.000000 robomimic-0.2.0/robomimic.egg-info/top_level.txt
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)       38 2021-12-17 18:57:38.146976 robomimic-0.2.0/setup.cfg
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     1284 2021-12-17 18:52:11.000000 robomimic-0.2.0/setup.py
-drwxr-xr-x   0 ajaymandlekar   (501) staff       (20)        0 2021-12-17 18:57:38.146561 robomimic-0.2.0/tests/
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)      388 2021-07-20 20:47:52.000000 robomimic-0.2.0/tests/test.sh
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     9817 2021-12-17 18:52:11.000000 robomimic-0.2.0/tests/test_bc.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    10574 2021-12-17 18:52:11.000000 robomimic-0.2.0/tests/test_bcq.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     5829 2021-12-17 18:52:11.000000 robomimic-0.2.0/tests/test_cql.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     2668 2021-07-20 20:47:52.000000 robomimic-0.2.0/tests/test_examples.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     6719 2021-12-17 18:52:11.000000 robomimic-0.2.0/tests/test_hbc.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)    13881 2021-12-17 18:52:11.000000 robomimic-0.2.0/tests/test_iris.py
--rw-r--r--   0 ajaymandlekar   (501) staff       (20)     7169 2021-12-17 18:52:11.000000 robomimic-0.2.0/tests/test_scripts.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.944761 robomimic-0.3.0/
+-rw-r--r--   0 amandlekar   (502) staff       (20)     1089 2022-09-02 00:20:41.000000 robomimic-0.3.0/LICENSE
+-rw-r--r--   0 amandlekar   (502) staff       (20)      312 2022-09-02 00:20:41.000000 robomimic-0.3.0/MANIFEST.in
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4570 2023-07-04 00:50:50.944584 robomimic-0.3.0/PKG-INFO
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4685 2023-07-04 00:42:13.000000 robomimic-0.3.0/README.md
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.912960 robomimic-0.3.0/examples/
+-rw-r--r--   0 amandlekar   (502) staff       (20)     9137 2022-09-02 00:20:41.000000 robomimic-0.3.0/examples/add_new_modality.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     1291 2022-09-02 00:20:41.000000 robomimic-0.3.0/examples/simple_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4636 2023-07-04 00:23:26.000000 robomimic-0.3.0/examples/simple_obs_nets.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     6149 2023-07-04 00:23:26.000000 robomimic-0.3.0/examples/simple_train_loop.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    24605 2023-07-04 00:23:26.000000 robomimic-0.3.0/examples/train_bc_rnn.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.913509 robomimic-0.3.0/robomimic/
+-rw-r--r--   0 amandlekar   (502) staff       (20)     7018 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/__init__.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.917678 robomimic-0.3.0/robomimic/algo/
+-rw-r--r--   0 amandlekar   (502) staff       (20)      647 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/__init__.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    17809 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/algo.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    32957 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/bc.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    44707 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/bcq.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    29951 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/cql.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    28734 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/gl.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    13110 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/hbc.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    15318 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/iql.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     6993 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/iris.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    22422 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/algo/td3_bc.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.920119 robomimic-0.3.0/robomimic/config/
+-rw-r--r--   0 amandlekar   (502) staff       (20)      620 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/config/__init__.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    16334 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/config/base_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     7739 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/config/bc_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5834 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/config/bcq_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    11279 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/config/config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5618 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/config/cql_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5131 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/config/gl_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4068 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/config/hbc_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4835 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/config/iql_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4408 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/config/iris_config.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5755 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/config/td3_bc_config.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.921208 robomimic-0.3.0/robomimic/envs/
+-rw-r--r--   0 amandlekar   (502) staff       (20)        0 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/envs/__init__.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     6072 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/envs/env_base.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     8277 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/envs/env_gym.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    14348 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/envs/env_ig_momart.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    14478 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/envs/env_robosuite.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     7818 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/envs/wrappers.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.909877 robomimic-0.3.0/robomimic/exps/
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.923086 robomimic-0.3.0/robomimic/exps/templates/
+-rw-r--r--   0 amandlekar   (502) staff       (20)     6064 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/exps/templates/bc.json
+-rw-r--r--   0 amandlekar   (502) staff       (20)     6750 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/exps/templates/bcq.json
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5049 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/exps/templates/cql.json
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5080 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/exps/templates/gl.json
+-rw-r--r--   0 amandlekar   (502) staff       (20)     9027 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/exps/templates/hbc.json
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5275 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/exps/templates/iql.json
+-rw-r--r--   0 amandlekar   (502) staff       (20)    15868 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/exps/templates/iris.json
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4502 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/exps/templates/td3_bc.json
+-rw-r--r--   0 amandlekar   (502) staff       (20)      852 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/macros.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.925948 robomimic-0.3.0/robomimic/models/
+-rw-r--r--   0 amandlekar   (502) staff       (20)       46 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/models/__init__.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    41616 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/models/base_nets.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4673 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/models/distributions.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    33955 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/models/obs_core.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    45780 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/models/obs_nets.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    61271 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/models/policy_nets.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    15788 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/models/transformers.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    58840 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/models/vae_nets.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    12072 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/models/value_nets.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.935803 robomimic-0.3.0/robomimic/scripts/
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.936753 robomimic-0.3.0/robomimic/scripts/conversion/
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5362 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/scripts/conversion/convert_d4rl.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     2472 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/scripts/conversion/convert_robosuite.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     6878 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/scripts/conversion/convert_roboturk_pilot.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    12393 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/scripts/dataset_states_to_obs.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     7634 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/scripts/download_datasets.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     6766 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/scripts/download_momart_datasets.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5716 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/scripts/extract_obs_from_raw_datasets.sh
+-rw-r--r--   0 amandlekar   (502) staff       (20)      871 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/scripts/generate_config_templates.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    64386 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/scripts/generate_paper_configs.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5188 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/scripts/get_dataset_info.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4407 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/scripts/hyperparam_helper.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    13087 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/scripts/playback_dataset.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    13499 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/scripts/run_trained_agent.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)      997 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/scripts/setup_macros.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     3566 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/scripts/split_train_val.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    16476 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/scripts/train.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.941994 robomimic-0.3.0/robomimic/utils/
+-rw-r--r--   0 amandlekar   (502) staff       (20)        0 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/utils/__init__.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    26246 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/dataset.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    10875 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/env_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    18509 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/file_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    14639 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/hyperparam_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     8292 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/log_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     7576 2022-09-02 00:20:41.000000 robomimic-0.3.0/robomimic/utils/loss_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    37676 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/obs_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     2993 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/python_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    30286 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/tensor_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     8904 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/test_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     7077 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/torch_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    22984 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/train_utils.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     3034 2023-07-04 00:23:26.000000 robomimic-0.3.0/robomimic/utils/vis_utils.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.914848 robomimic-0.3.0/robomimic.egg-info/
+-rw-r--r--   0 amandlekar   (502) staff       (20)     4570 2023-07-04 00:50:50.000000 robomimic-0.3.0/robomimic.egg-info/PKG-INFO
+-rw-r--r--   0 amandlekar   (502) staff       (20)     2970 2023-07-04 00:50:50.000000 robomimic-0.3.0/robomimic.egg-info/SOURCES.txt
+-rw-r--r--   0 amandlekar   (502) staff       (20)        1 2023-07-04 00:50:50.000000 robomimic-0.3.0/robomimic.egg-info/dependency_links.txt
+-rw-r--r--   0 amandlekar   (502) staff       (20)        2 2023-07-04 00:50:50.000000 robomimic-0.3.0/robomimic.egg-info/eager_resources.txt
+-rw-r--r--   0 amandlekar   (502) staff       (20)      135 2023-07-04 00:50:50.000000 robomimic-0.3.0/robomimic.egg-info/requires.txt
+-rw-r--r--   0 amandlekar   (502) staff       (20)       10 2023-07-04 00:50:50.000000 robomimic-0.3.0/robomimic.egg-info/top_level.txt
+-rw-r--r--   0 amandlekar   (502) staff       (20)       38 2023-07-04 00:50:50.944817 robomimic-0.3.0/setup.cfg
+-rw-r--r--   0 amandlekar   (502) staff       (20)     1323 2023-07-04 00:23:26.000000 robomimic-0.3.0/setup.py
+drwxr-xr-x   0 amandlekar   (502) staff       (20)        0 2023-07-04 00:50:50.944292 robomimic-0.3.0/tests/
+-rw-r--r--   0 amandlekar   (502) staff       (20)      388 2022-09-02 00:20:41.000000 robomimic-0.3.0/tests/test.sh
+-rw-r--r--   0 amandlekar   (502) staff       (20)    10256 2023-07-04 00:23:26.000000 robomimic-0.3.0/tests/test_bc.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    10574 2022-09-02 00:20:41.000000 robomimic-0.3.0/tests/test_bcq.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5829 2022-09-02 00:20:41.000000 robomimic-0.3.0/tests/test_cql.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     2668 2022-09-02 00:20:41.000000 robomimic-0.3.0/tests/test_examples.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     6719 2022-09-02 00:20:41.000000 robomimic-0.3.0/tests/test_hbc.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     5387 2023-07-04 00:23:26.000000 robomimic-0.3.0/tests/test_iql.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)    13881 2022-09-02 00:20:41.000000 robomimic-0.3.0/tests/test_iris.py
+-rw-r--r--   0 amandlekar   (502) staff       (20)     7169 2022-09-02 00:20:41.000000 robomimic-0.3.0/tests/test_scripts.py
```

### Comparing `robomimic-0.2.0/LICENSE` & `robomimic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/README.md` & `robomimic-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -7,57 +7,83 @@
   <img width="24.0%" src="docs/images/task_square.gif">
   <img width="24.0%" src="docs/images/task_lift_real.gif">
   <img width="24.0%" src="docs/images/task_can_real.gif">
   <img width="24.0%" src="docs/images/task_tool_hang_real.gif">
   <img width="24.0%" src="docs/images/task_transport.gif">
  </p>
 
-[**[Homepage]**](https://arise-initiative.github.io/robomimic-web/) &ensp; [**[Documentation]**](https://arise-initiative.github.io/robomimic-web/docs/introduction/overview.html) &ensp; [**[Study Paper]**](https://arxiv.org/abs/2108.03298) &ensp; [**[Study Website]**](https://arise-initiative.github.io/robomimic-web/study/) &ensp; [**[ARISE Initiative]**](https://github.com/ARISE-Initiative)
+[**[Homepage]**](https://robomimic.github.io/) &ensp; [**[Documentation]**](https://robomimic.github.io/docs/introduction/overview.html) &ensp; [**[Study Paper]**](https://arxiv.org/abs/2108.03298) &ensp; [**[Study Website]**](https://robomimic.github.io/study/) &ensp; [**[ARISE Initiative]**](https://github.com/ARISE-Initiative)
 
 -------
 ## Latest Updates
-- [12/16/2021] **v0.2.0**: Modular observation modalities and encoders :wrench:, support for [MOMART](https://sites.google.com/view/il-for-mm/home) datasets :open_file_folder:
+- [07/03/2023] **v0.3.0**: BC-Transformer and IQL :brain:, support for DeepMind MuJoCo bindings :robot:, pre-trained image reps :eye:, wandb logging :chart_with_upwards_trend:, and more
+- [05/23/2022] **v0.2.1**: Updated website and documentation to feature more tutorials :notebook_with_decorative_cover:
+- [12/16/2021] **v0.2.0**: Modular observation modalities and encoders :wrench:, support for [MOMART](https://sites.google.com/view/il-for-mm/home) datasets :open_file_folder: [[release notes]](https://github.com/ARISE-Initiative/robomimic/releases/tag/v0.2.0) [[documentation]](https://robomimic.github.io/docs/v0.2/introduction/overview.html)
 - [08/09/2021] **v0.1.0**: Initial code and paper release
 
 -------
 
-**robomimic** is a framework for robot learning from demonstration. It offers a broad set of demonstration datasets collected on robot manipulation domains, and learning algorithms to learn from these datasets. This project is part of the broader [Advancing Robot Intelligence through Simulated Environments (ARISE) Initiative](https://github.com/ARISE-Initiative), with the aim of lowering the barriers of entry for cutting-edge research at the intersection of AI and Robotics.
+## Colab quickstart
+Get started with a quick colab notebook demo of robomimic with installing anything locally.
 
-Imitating human demonstrations is a promising approach to endow robots with various manipulation capabilities. While recent advances have been made in imitation learning and batch (offline) reinforcement learning, a lack of open-source human datasets and reproducible learning methods make assessing the state of the field difficult. The overarching goal of **robomimic** is to provide researchers and practitioners with:
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1b62r_km9pP40fKF0cBdpdTO2P_2eIbC6?usp=sharing)
 
-- a **standardized set of large demonstration datasets** across several benchmarking tasks to facilitate fair comparisons, with a focus on learning from human-provided demonstrations
-- a **standardized set of large demonstration datasets** across several benchmarking tasks to facilitate fair comparisons, with a focus on learning from human-provided demonstrations (see [this link](https://arise-initiative.github.io/robomimic-web/docs/introduction/quickstart.html#supported-datasets) for a list of supported datasets)
-- **high-quality implementations of several learning algorithms** for training closed-loop policies from offline datasets to make reproducing results easy and lower the barrier to entry
-- a **modular design** that offers great flexibility in extending algorithms and designing new algorithms
-
-This release of **robomimic** contains seven offline learning [algorithms](https://arise-initiative.github.io/robomimic-web/docs/modules/algorithms.html) and standardized [datasets](https://arise-initiative.github.io/robomimic-web/docs/introduction/results.html) collected across five simulated and three real-world multi-stage manipulation tasks of varying complexity. We highlight some features below (for a more thorough list of features, see [this link](https://arise-initiative.github.io/robomimic-web/docs/introduction/quickstart.html#features-overview)):
-
-- **standardized datasets:** a set of datasets collected from different sources (single proficient human, multiple humans, and machine-generated) across several simulated and real-world tasks, along with a plug-and-play [Dataset class](https://arise-initiative.github.io/robomimic-web/docs/modules/datasets.html) to easily use the datasets outside of this project
-- **algorithm implementations:** several high-quality implementations of offline learning algorithms, including BC, BC-RNN, HBC, IRIS, BCQ, CQL, and TD3-BC
-- **multiple observation spaces:** support for learning both low-dimensional and visuomotor policies, with support for observation tensor dictionaries throughout the codebase, making it easy to specify different subsets of observations to train a policy. This includes a set of useful tensor utilities to work with nested dictionaries of torch Tensors and numpy arrays.
-- **visualization utilities:** utilities for visualizing demonstration data, playing back actions, visualizing trained policies, and collecting new datasets using trained policies
-- **train launching utilities:** utilities for easily running hyperparameter sweeps, enabled by a flexible [Config](https://arise-initiative.github.io/robomimic-web/docs/modules/configs.html) management system
 
-## Contributing to robomimic
+-------
 
-This framework originally began development in late 2018. Researchers in the [Stanford Vision and Learning Lab](http://svl.stanford.edu/) (SVL) used it as an internal tool for training policies from offline human demonstration datasets. Now it is actively maintained and used for robotics research projects across multiple labs. We welcome community contributions to this project. For details please check our [contributing guidelines](https://arise-initiative.github.io/robomimic-web/docs/miscellaneous/contributing.html).
+**robomimic** is a framework for robot learning from demonstration.
+It offers a broad set of demonstration datasets collected on robot manipulation domains and offline learning algorithms to learn from these datasets.
+**robomimic** aims to make robot learning broadly *accessible* and *reproducible*, allowing researchers and practitioners to benchmark tasks and algorithms fairly and to develop the next generation of robot learning algorithms.
 
-## Troubleshooting
+## Core Features
+
+<p align="center">
+  <img width="50.0%" src="docs/images/core_features.png">
+ </p>
+
+<!-- **Standardized Datasets**
+- Simulated and real-world tasks
+- Multiple environments and robots
+- Diverse human-collected and machine-generated datasets
+
+**Suite of Learning Algorithms**
+- Imitation Learning algorithms (BC, BC-RNN, HBC)
+- Offline RL algorithms (BCQ, CQL, IRIS, TD3-BC)
 
-Please see the [troubleshooting](https://arise-initiative.github.io/robomimic-web/docs/miscellaneous/troubleshooting.html) section for common fixes, or [submit an issue](https://github.com/ARISE-Initiative/robomimic/issues) on our github page.
+**Modular Design**
+- Low-dim + Visuomotor policies
+- Diverse network architectures
+- Support for external datasets
 
-## Reproducing study results
+**Flexible Workflow**
+- Hyperparameter sweep tools
+- Dataset visualization tools
+- Generating new datasets -->
 
-The **robomimic** framework also makes reproducing the results from this [study](https://arise-initiative.github.io/robomimic-web/study.) easy. See the [results documentation](https://arise-initiative.github.io/robomimic-web/docs/introduction/results.html) for more information.
 
-## Citations
+## Reproducing benchmarks
+
+The robomimic framework also makes reproducing the results from different benchmarks and datasets easy. See the [datasets page](https://robomimic.github.io/docs/datasets/overview.html) for more information on downloading datasets and reproducing experiments.
+
+## Troubleshooting
+
+Please see the [troubleshooting](https://robomimic.github.io/docs/miscellaneous/troubleshooting.html) section for common fixes, or [submit an issue](https://github.com/ARISE-Initiative/robomimic/issues) on our github page.
+
+## Contributing to robomimic
+This project is part of the broader [Advancing Robot Intelligence through Simulated Environments (ARISE) Initiative](https://github.com/ARISE-Initiative), with the aim of lowering the barriers of entry for cutting-edge research at the intersection of AI and Robotics.
+The project originally began development in late 2018 by researchers in the [Stanford Vision and Learning Lab](http://svl.stanford.edu/) (SVL).
+Now it is actively maintained and used for robotics research projects across multiple labs.
+We welcome community contributions to this project.
+For details please check our [contributing guidelines](https://robomimic.github.io/docs/miscellaneous/contributing.html).
+
+## Citation
 
 Please cite [this paper](https://arxiv.org/abs/2108.03298) if you use this framework in your work:
 
 ```bibtex
 @inproceedings{robomimic2021,
   title={What Matters in Learning from Offline Human Demonstrations for Robot Manipulation},
   author={Ajay Mandlekar and Danfei Xu and Josiah Wong and Soroush Nasiriany and Chen Wang and Rohun Kulkarni and Li Fei-Fei and Silvio Savarese and Yuke Zhu and Roberto Mart\'{i}n-Mart\'{i}n},
-  booktitle={arXiv preprint arXiv:2108.03298},
+  booktitle={Conference on Robot Learning (CoRL)},
   year={2021}
 }
-```
+```
```

### Comparing `robomimic-0.2.0/examples/add_new_modality.py` & `robomimic-0.3.0/examples/add_new_modality.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/examples/simple_config.py` & `robomimic-0.3.0/examples/simple_config.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/examples/simple_obs_nets.py` & `robomimic-0.3.0/examples/simple_obs_nets.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 This is purely for instructional purposes, in case others would like to make use of or extend the
 functionality.
 """
 
 from collections import OrderedDict
 
 import torch
-from robomimic.models.obs_nets import ObservationEncoder, MLP, ObservationDecoder
-from robomimic.models.base_nets import CropRandomizer
+from robomimic.models.base_nets import MLP
+from robomimic.models.obs_nets import ObservationEncoder, ObservationDecoder
+from robomimic.models.obs_core import CropRandomizer
 import robomimic.utils.tensor_utils as TensorUtils
 import robomimic.utils.obs_utils as ObsUtils
 
 
 def simple_obs_example():
     obs_encoder = ObservationEncoder(feature_activation=torch.nn.ReLU)
```

### Comparing `robomimic-0.2.0/examples/simple_train_loop.py` & `robomimic-0.3.0/examples/simple_train_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 
             if not has_printed_batch_info:
                 has_printed_batch_info = True
                 print_batch_info(batch)
 
             # process batch for training
             input_batch = model.process_batch_for_training(batch)
+            input_batch = model.postprocess_batch_for_training(input_batch, obs_normalization_stats=None)
 
             # forward and backward pass
             info = model.train_on_batch(batch=input_batch, epoch=epoch, validate=False)
 
             # record loss
             step_log = model.log_info(info)
             losses.append(step_log["Loss"])
```

### Comparing `robomimic-0.2.0/examples/train_bc_rnn.py` & `robomimic-0.3.0/examples/train_bc_rnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     python train_bc_rnn.py --dataset /path/to/dataset.hdf5 --output /path/to/output_dir
 """
 import argparse
 
 import robomimic
 import robomimic.utils.torch_utils as TorchUtils
 import robomimic.utils.test_utils as TestUtils
-import robomimic.utils.macros as Macros
+import robomimic.macros as Macros
 from robomimic.config import config_factory
 from robomimic.scripts.train import train
 
 
 def robosuite_hyperparameters(config):
     """
     Sets robosuite-specific hyperparameters.
@@ -58,15 +58,15 @@
     config.experiment.render_video = True                       # render evaluation rollouts to videos
     config.experiment.keep_all_videos = False                   # save all videos, instead of only saving those for saved model checkpoints
     config.experiment.video_skip = 5                            # render video frame every n environment steps during rollout
 
     ## evaluation rollout config ##
     config.experiment.rollout.enabled = True                    # enable evaluation rollouts
     config.experiment.rollout.n = 50                            # number of rollouts per evaluation
-    config.experiment.rollout.horizon = 400                     # maximum number of env steps per rollout
+    config.experiment.rollout.horizon = 400                     # set horizon based on length of demonstrations (can be obtained with scripts/get_dataset_info.py)
     config.experiment.rollout.rate = 50                         # do rollouts every @rate epochs
     config.experiment.rollout.warmstart = 0                     # number of epochs to wait before starting rollouts
     config.experiment.rollout.terminate_on_success = True       # end rollout early after task success
 
     ## dataset loader config ##
 
     # num workers for loading data - generally set to 0 for low-dim datasets, and 2 for image datasets
@@ -82,15 +82,16 @@
 
     # if true, normalize observations at train and test time, using the global mean and standard deviation
     # of each observation in each dimension, computed across the training set. See SequenceDataset.normalize_obs
     # in utils/dataset.py for more information.
     config.train.hdf5_normalize_obs = False                     # no obs normalization
 
     # if provided, demonstrations are filtered by the list of demo keys under "mask/@hdf5_filter_key"
-    config.train.hdf5_filter_key = None                         # by default, use no filter key
+    config.train.hdf5_filter_key = "train"                      # by default, use "train" and "valid" filter keys corresponding to train-valid split
+    config.train.hdf5_validation_filter_key = "valid"
 
     # fetch sequences of length 10 from dataset for RNN training
     config.train.seq_length = 10
 
     # keys from hdf5 to load per demonstration, besides "obs" and "next_obs"
     config.train.dataset_keys = (
         "actions",
@@ -128,14 +129,26 @@
     config.observation.encoder.rgb.core_kwargs.backbone_kwargs.input_coord_conv = False
     config.observation.encoder.rgb.core_kwargs.pool_class = "SpatialSoftmax"                # Alternate options are "SpatialMeanPool" or None (no pooling)
     config.observation.encoder.rgb.core_kwargs.pool_kwargs.num_kp = 32                      # Default arguments for "SpatialSoftmax"
     config.observation.encoder.rgb.core_kwargs.pool_kwargs.learnable_temperature = False    # Default arguments for "SpatialSoftmax"
     config.observation.encoder.rgb.core_kwargs.pool_kwargs.temperature = 1.0                # Default arguments for "SpatialSoftmax"
     config.observation.encoder.rgb.core_kwargs.pool_kwargs.noise_std = 0.0                  # Default arguments for "SpatialSoftmax"
 
+    # if you prefer to use pre-trained visual representations, uncomment the following lines
+    # R3M
+    # config.observation.encoder.rgb.core_kwargs.backbone_class = 'R3MConv'                         # R3M backbone for image observations (unused if no image observations)
+    # config.observation.encoder.rgb.core_kwargs.backbone_kwargs.r3m_model_class = 'resnet18'       # R3M model class (resnet18, resnet34, resnet50)
+    # config.observation.encoder.rgb.core_kwargs.backbone_kwargs.freeze = True                      # whether to freeze network during training or allow finetuning
+    # config.observation.encoder.rgb.core_kwargs.pool_class = None                                  # no pooling class for pretraining model
+    # MVP
+    # config.observation.encoder.rgb.core_kwargs.backbone_class = 'MVPConv'                                   # MVP backbone for image observations (unused if no image observations)
+    # config.observation.encoder.rgb.core_kwargs.backbone_kwargs.mvp_model_class = 'vitb-mae-egosoup'         # MVP model class (vits-mae-hoi, vits-mae-in, vits-sup-in, vitb-mae-egosoup, vitl-256-mae-egosoup)
+    # config.observation.encoder.rgb.core_kwargs.backbone_kwargs.freeze = True                                # whether to freeze network during training or allow finetuning
+    # config.observation.encoder.rgb.core_kwargs.pool_class = None                                            # no pooling class for pretraining model
+
     # observation randomizer class - set to None to use no randomization, or 'CropRandomizer' to use crop randomization
     config.observation.encoder.rgb.obs_randomizer_class = None
 
     # kwargs for observation randomizers (for the CropRandomizer, this is size and number of crops)
     config.observation.encoder.rgb.obs_randomizer_kwargs.crop_height = 76
     config.observation.encoder.rgb.obs_randomizer_kwargs.crop_width = 76
     config.observation.encoder.rgb.obs_randomizer_kwargs.num_crops = 1
@@ -232,15 +245,16 @@
 
     # if true, normalize observations at train and test time, using the global mean and standard deviation
     # of each observation in each dimension, computed across the training set. See SequenceDataset.normalize_obs
     # in utils/dataset.py for more information.
     config.train.hdf5_normalize_obs = False                     # no obs normalization
 
     # if provided, demonstrations are filtered by the list of demo keys under "mask/@hdf5_filter_key"
-    config.train.hdf5_filter_key = None                         # by default, use no filter key
+    config.train.hdf5_filter_key = "train"                      # by default, use "train" and "valid" filter keys corresponding to train-valid split
+    config.train.hdf5_validation_filter_key = "valid"
 
     # fetch sequences of length 10 from dataset for RNN training
     config.train.seq_length = 50
 
     # keys from hdf5 to load per demonstration, besides "obs" and "next_obs"
     config.train.dataset_keys = (
         "actions",
```

### Comparing `robomimic-0.2.0/robomimic/__init__.py` & `robomimic-0.3.0/robomimic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 
 # stores released dataset links and rollout horizons in global dictionary.
 # Structure is given below for each type of dataset:
 
 # robosuite / real
 # {
@@ -56,54 +56,57 @@
     """
 
     # all proficient human datasets
     ph_tasks = ["lift", "can", "square", "transport", "tool_hang", "lift_real", "can_real", "tool_hang_real"]
     ph_horizons = [400, 400, 400, 700, 700, 1000, 1000, 1000]
     for task, horizon in zip(ph_tasks, ph_horizons):
         register_dataset_link(task=task, dataset_type="ph", hdf5_type="raw", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/ph/demo.hdf5".format(task))
+            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/ph/demo{}.hdf5".format(
+                task, "" if "real" in task else "_v141"
+            )
+        )
         # real world datasets only have demo.hdf5 files which already contain all observation modalities
         # while sim datasets store raw low-dim mujoco states in the demo.hdf5
         if "real" not in task:
             register_dataset_link(task=task, dataset_type="ph", hdf5_type="low_dim", horizon=horizon,
-                link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/ph/low_dim.hdf5".format(task))
+                link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/ph/low_dim_v141.hdf5".format(task))
             register_dataset_link(task=task, dataset_type="ph", hdf5_type="image", horizon=horizon,
-                link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/ph/image.hdf5".format(task))
+                link=None)
 
     # all multi human datasets
     mh_tasks = ["lift", "can", "square", "transport"]
     mh_horizons = [500, 500, 500, 1100]
     for task, horizon in zip(mh_tasks, mh_horizons):
         register_dataset_link(task=task, dataset_type="mh", hdf5_type="raw", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mh/demo.hdf5".format(task))
+            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mh/demo_v141.hdf5".format(task))
         register_dataset_link(task=task, dataset_type="mh", hdf5_type="low_dim", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mh/low_dim.hdf5".format(task))
+            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mh/low_dim_v141.hdf5".format(task))
         register_dataset_link(task=task, dataset_type="mh", hdf5_type="image", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mh/image.hdf5".format(task))
+            link=None)
 
     # all machine generated datasets
     for task, horizon in zip(["lift", "can"], [400, 400]):
         register_dataset_link(task=task, dataset_type="mg", hdf5_type="raw", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/demo.hdf5".format(task))
+            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/demo_v141.hdf5".format(task))
         register_dataset_link(task=task, dataset_type="mg", hdf5_type="low_dim_sparse", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/low_dim_sparse.hdf5".format(task))
+            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/low_dim_sparse_v141.hdf5".format(task))
         register_dataset_link(task=task, dataset_type="mg", hdf5_type="image_sparse", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/image_sparse.hdf5".format(task))
+            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/image_sparse_v141.hdf5".format(task))
         register_dataset_link(task=task, dataset_type="mg", hdf5_type="low_dim_dense", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/low_dim_dense.hdf5".format(task))
+            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/low_dim_dense_v141.hdf5".format(task))
         register_dataset_link(task=task, dataset_type="mg", hdf5_type="image_dense", horizon=horizon,
-            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/image_dense.hdf5".format(task))
+            link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/{}/mg/image_dense_v141.hdf5".format(task))
 
     # can-paired dataset
     register_dataset_link(task="can", dataset_type="paired", hdf5_type="raw", horizon=400,
-        link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/can/paired/demo.hdf5")
+        link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/can/paired/demo_v141.hdf5")
     register_dataset_link(task="can", dataset_type="paired", hdf5_type="low_dim", horizon=400,
-        link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/can/paired/low_dim.hdf5")
+        link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/can/paired/low_dim_v141.hdf5")
     register_dataset_link(task="can", dataset_type="paired", hdf5_type="image", horizon=400,
-        link="http://downloads.cs.stanford.edu/downloads/rt_benchmark/can/paired/image.hdf5")
+        link=None)
 
 
 def register_momart_dataset_link(task, dataset_type, link, dataset_size):
     """
     Helper function to register dataset link in global dictionary.
     Also takes a @horizon parameter - this corresponds to the evaluation
     rollout horizon that should be used during training.
```

### Comparing `robomimic-0.2.0/robomimic/algo/__init__.py` & `robomimic-0.3.0/robomimic/algo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from robomimic.algo.algo import register_algo_factory_func, algo_name_to_factory_func, algo_factory, Algo, PolicyAlgo, ValueAlgo, PlannerAlgo, HierarchicalAlgo, RolloutPolicy
 
 # note: these imports are needed to register these classes in the global algo registry
 from robomimic.algo.bc import BC, BC_Gaussian, BC_GMM, BC_VAE, BC_RNN, BC_RNN_GMM
 from robomimic.algo.bcq import BCQ, BCQ_GMM, BCQ_Distributional
 from robomimic.algo.cql import CQL
+from robomimic.algo.iql import IQL
 from robomimic.algo.gl import GL, GL_VAE, ValuePlanner
 from robomimic.algo.hbc import HBC
 from robomimic.algo.iris import IRIS
 from robomimic.algo.td3_bc import TD3_BC
```

### Comparing `robomimic-0.2.0/robomimic/algo/algo.py` & `robomimic-0.3.0/robomimic/algo/algo.py`

 * *Files 8% similar despite different names*

```diff
@@ -197,14 +197,56 @@
 
         Returns:
             input_batch (dict): processed and filtered batch that
                 will be used for training 
         """
         return batch
 
+    def postprocess_batch_for_training(self, batch, obs_normalization_stats):
+        """
+        Does some operations (like channel swap, uint8 to float conversion, normalization)
+        after @process_batch_for_training is called, in order to ensure these operations
+        take place on GPU.
+
+        Args:
+            batch (dict): dictionary with torch.Tensors sampled
+                from a data loader. Assumed to be on the device where
+                training will occur (after @process_batch_for_training
+                is called)
+
+            obs_normalization_stats (dict or None): if provided, this should map observation 
+                keys to dicts with a "mean" and "std" of shape (1, ...) where ... is the 
+                default shape for the observation.
+
+        Returns:
+            batch (dict): postproceesed batch
+        """
+
+        # we will search the nested batch dictionary for the following special batch dict keys
+        # and apply the processing function to their values (which correspond to observations)
+        obs_keys = ["obs", "next_obs", "goal_obs"]
+
+        def recurse_helper(d):
+            """
+            Apply process_obs_dict to values in nested dictionary d that match a key in obs_keys.
+            """
+            for k in d:
+                if k in obs_keys:
+                    # found key - stop search and process observation
+                    if d[k] is not None:
+                        d[k] = ObsUtils.process_obs_dict(d[k])
+                        if obs_normalization_stats is not None:
+                            d[k] = ObsUtils.normalize_obs(d[k], obs_normalization_stats=obs_normalization_stats)
+                elif isinstance(d[k], dict):
+                    # search down into dictionary
+                    recurse_helper(d[k])
+
+        recurse_helper(batch)
+        return batch
+
     def train_on_batch(self, batch, epoch, validate=False):
         """
         Training on a single batch of data.
 
         Args:
             batch (dict): dictionary with torch.Tensors sampled
                 from a data loader and filtered by @process_batch_for_training
```

### Comparing `robomimic-0.2.0/robomimic/algo/bc.py` & `robomimic-0.3.0/robomimic/algo/bc.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Implementation of Behavioral Cloning (BC).
 """
 from collections import OrderedDict
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+import torch.distributions as D
 
 import robomimic.models.base_nets as BaseNets
 import robomimic.models.obs_nets as ObsNets
 import robomimic.models.policy_nets as PolicyNets
 import robomimic.models.vae_nets as VAENets
 import robomimic.utils.loss_utils as LossUtils
 import robomimic.utils.tensor_utils as TensorUtils
@@ -34,26 +35,47 @@
 
     # note: we need the check below because some configs import BCConfig and exclude
     # some of these options
     gaussian_enabled = ("gaussian" in algo_config and algo_config.gaussian.enabled)
     gmm_enabled = ("gmm" in algo_config and algo_config.gmm.enabled)
     vae_enabled = ("vae" in algo_config and algo_config.vae.enabled)
 
-    if algo_config.rnn.enabled:
-        if gmm_enabled:
-            return BC_RNN_GMM, {}
-        return BC_RNN, {}
-    assert sum([gaussian_enabled, gmm_enabled, vae_enabled]) <= 1
+    rnn_enabled = algo_config.rnn.enabled
+    transformer_enabled = algo_config.transformer.enabled
+
     if gaussian_enabled:
-        return BC_Gaussian, {}
-    if gmm_enabled:
-        return BC_GMM, {}
-    if vae_enabled:
-        return BC_VAE, {}
-    return BC, {}
+        if rnn_enabled:
+            raise NotImplementedError
+        elif transformer_enabled:
+            raise NotImplementedError
+        else:
+            algo_class, algo_kwargs = BC_Gaussian, {}
+    elif gmm_enabled:
+        if rnn_enabled:
+            algo_class, algo_kwargs = BC_RNN_GMM, {}
+        elif transformer_enabled:
+            algo_class, algo_kwargs = BC_Transformer_GMM, {}
+        else:
+            algo_class, algo_kwargs = BC_GMM, {}
+    elif vae_enabled:
+        if rnn_enabled:
+            raise NotImplementedError
+        elif transformer_enabled:
+            raise NotImplementedError
+        else:
+            algo_class, algo_kwargs = BC_VAE, {}
+    else:
+        if rnn_enabled:
+            algo_class, algo_kwargs = BC_RNN, {}
+        elif transformer_enabled:
+            algo_class, algo_kwargs = BC_Transformer, {}
+        else:
+            algo_class, algo_kwargs = BC, {}
+
+    return algo_class, algo_kwargs
 
 
 class BC(PolicyAlgo):
     """
     Normal BC training.
     """
     def _create_networks(self):
@@ -83,15 +105,18 @@
             input_batch (dict): processed and filtered batch that
                 will be used for training 
         """
         input_batch = dict()
         input_batch["obs"] = {k: batch["obs"][k][:, 0, :] for k in batch["obs"]}
         input_batch["goal_obs"] = batch.get("goal_obs", None) # goals may not be present
         input_batch["actions"] = batch["actions"][:, 0, :]
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
+
 
     def train_on_batch(self, batch, epoch, validate=False):
         """
         Training on a single batch of data.
 
         Args:
             batch (dict): dictionary with torch.Tensors sampled
@@ -500,15 +525,17 @@
             # replace the observation sequence with one that only consists of the first observation.
             # This way, all actions are predicted "open-loop" after the first observation, based
             # on the rnn hidden state.
             n_steps = batch["actions"].shape[1]
             obs_seq_start = TensorUtils.index_at_time(batch["obs"], ind=0)
             input_batch["obs"] = TensorUtils.unsqueeze_expand_at(obs_seq_start, size=n_steps, dim=1)
 
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
 
     def get_action(self, obs_dict, goal_dict=None):
         """
         Get policy action outputs.
 
         Args:
             obs_dict (dict): current observation
@@ -639,7 +666,209 @@
         """
         log = PolicyAlgo.log_info(self, info)
         log["Loss"] = info["losses"]["action_loss"].item()
         log["Log_Likelihood"] = info["losses"]["log_probs"].item() 
         if "policy_grad_norms" in info:
             log["Policy_Grad_Norms"] = info["policy_grad_norms"]
         return log
+
+
+class BC_Transformer(BC):
+    """
+    BC training with a Transformer policy.
+    """
+    def _create_networks(self):
+        """
+        Creates networks and places them into @self.nets.
+        """
+        assert self.algo_config.transformer.enabled
+
+        self.nets = nn.ModuleDict()
+        self.nets["policy"] = PolicyNets.TransformerActorNetwork(
+            obs_shapes=self.obs_shapes,
+            goal_shapes=self.goal_shapes,
+            ac_dim=self.ac_dim,
+            encoder_kwargs=ObsUtils.obs_encoder_kwargs_from_config(self.obs_config.encoder),
+            **BaseNets.transformer_args_from_config(self.algo_config.transformer),
+        )
+        self._set_params_from_config()
+        self.nets = self.nets.float().to(self.device)
+        
+    def _set_params_from_config(self):
+        """
+        Read specific config variables we need for training / eval.
+        Called by @_create_networks method
+        """
+        self.context_length = self.algo_config.transformer.context_length
+        self.supervise_all_steps = self.algo_config.transformer.supervise_all_steps
+
+    def process_batch_for_training(self, batch):
+        """
+        Processes input batch from a data loader to filter out
+        relevant information and prepare the batch for training.
+        Args:
+            batch (dict): dictionary with torch.Tensors sampled
+                from a data loader
+        Returns:
+            input_batch (dict): processed and filtered batch that
+                will be used for training
+        """
+        input_batch = dict()
+        h = self.context_length
+        input_batch["obs"] = {k: batch["obs"][k][:, :h, :] for k in batch["obs"]}
+        input_batch["goal_obs"] = batch.get("goal_obs", None) # goals may not be present
+
+        if self.supervise_all_steps:
+            # supervision on entire sequence (instead of just current timestep)
+            input_batch["actions"] = batch["actions"][:, :h, :]
+        else:
+            # just use current timestep
+            input_batch["actions"] = batch["actions"][:, h-1, :]
+
+        input_batch = TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        return input_batch
+
+    def _forward_training(self, batch, epoch=None):
+        """
+        Internal helper function for BC_Transformer algo class. Compute forward pass
+        and return network outputs in @predictions dict.
+
+        Args:
+            batch (dict): dictionary with torch.Tensors sampled
+                from a data loader and filtered by @process_batch_for_training
+
+        Returns:
+            predictions (dict): dictionary containing network outputs
+        """
+        # ensure that transformer context length is consistent with temporal dimension of observations
+        TensorUtils.assert_size_at_dim(
+            batch["obs"], 
+            size=(self.context_length), 
+            dim=1, 
+            msg="Error: expect temporal dimension of obs batch to match transformer context length {}".format(self.context_length),
+        )
+
+        predictions = OrderedDict()
+        predictions["actions"] = self.nets["policy"](obs_dict=batch["obs"], actions=None, goal_dict=batch["goal_obs"])
+        if not self.supervise_all_steps:
+            # only supervise final timestep
+            predictions["actions"] = predictions["actions"][:, -1, :]
+        return predictions
+
+    def get_action(self, obs_dict, goal_dict=None):
+        """
+        Get policy action outputs.
+        Args:
+            obs_dict (dict): current observation
+            goal_dict (dict): (optional) goal
+        Returns:
+            action (torch.Tensor): action tensor
+        """
+        assert not self.nets.training
+
+        return self.nets["policy"](obs_dict, actions=None, goal_dict=goal_dict)[:, -1, :]
+
+
+class BC_Transformer_GMM(BC_Transformer):
+    """
+    BC training with a Transformer GMM policy.
+    """
+    def _create_networks(self):
+        """
+        Creates networks and places them into @self.nets.
+        """
+        assert self.algo_config.gmm.enabled
+        assert self.algo_config.transformer.enabled
+
+        self.nets = nn.ModuleDict()
+        self.nets["policy"] = PolicyNets.TransformerGMMActorNetwork(
+            obs_shapes=self.obs_shapes,
+            goal_shapes=self.goal_shapes,
+            ac_dim=self.ac_dim,
+            num_modes=self.algo_config.gmm.num_modes,
+            min_std=self.algo_config.gmm.min_std,
+            std_activation=self.algo_config.gmm.std_activation,
+            low_noise_eval=self.algo_config.gmm.low_noise_eval,
+            encoder_kwargs=ObsUtils.obs_encoder_kwargs_from_config(self.obs_config.encoder),
+            **BaseNets.transformer_args_from_config(self.algo_config.transformer),
+        )
+        self._set_params_from_config()
+        self.nets = self.nets.float().to(self.device)
+
+    def _forward_training(self, batch, epoch=None):
+        """
+        Modify from super class to support GMM training.
+        """
+        # ensure that transformer context length is consistent with temporal dimension of observations
+        TensorUtils.assert_size_at_dim(
+            batch["obs"], 
+            size=(self.context_length), 
+            dim=1, 
+            msg="Error: expect temporal dimension of obs batch to match transformer context length {}".format(self.context_length),
+        )
+
+        dists = self.nets["policy"].forward_train(
+            obs_dict=batch["obs"], 
+            actions=None,
+            goal_dict=batch["goal_obs"],
+            low_noise_eval=False,
+        )
+
+        # make sure that this is a batch of multivariate action distributions, so that
+        # the log probability computation will be correct
+        assert len(dists.batch_shape) == 2 # [B, T]
+
+        if not self.supervise_all_steps:
+            # only use final timestep prediction by making a new distribution with only final timestep.
+            # This essentially does `dists = dists[:, -1]`
+            component_distribution = D.Normal(
+                loc=dists.component_distribution.base_dist.loc[:, -1],
+                scale=dists.component_distribution.base_dist.scale[:, -1],
+            )
+            component_distribution = D.Independent(component_distribution, 1)
+            mixture_distribution = D.Categorical(logits=dists.mixture_distribution.logits[:, -1])
+            dists = D.MixtureSameFamily(
+                mixture_distribution=mixture_distribution,
+                component_distribution=component_distribution,
+            )
+
+        log_probs = dists.log_prob(batch["actions"])
+
+        predictions = OrderedDict(
+            log_probs=log_probs,
+        )
+        return predictions
+
+    def _compute_losses(self, predictions, batch):
+        """
+        Internal helper function for BC_Transformer_GMM algo class. Compute losses based on
+        network outputs in @predictions dict, using reference labels in @batch.
+        Args:
+            predictions (dict): dictionary containing network outputs, from @_forward_training
+            batch (dict): dictionary with torch.Tensors sampled
+                from a data loader and filtered by @process_batch_for_training
+        Returns:
+            losses (dict): dictionary of losses computed over the batch
+        """
+
+        # loss is just negative log-likelihood of action targets
+        action_loss = -predictions["log_probs"].mean()
+        return OrderedDict(
+            log_probs=-action_loss,
+            action_loss=action_loss,
+        )
+
+    def log_info(self, info):
+        """
+        Process info dictionary from @train_on_batch to summarize
+        information to pass to tensorboard for logging.
+        Args:
+            info (dict): dictionary of info
+        Returns:
+            loss_log (dict): name -> summary statistic
+        """
+        log = PolicyAlgo.log_info(self, info)
+        log["Loss"] = info["losses"]["action_loss"].item()
+        log["Log_Likelihood"] = info["losses"]["log_probs"].item() 
+        if "policy_grad_norms" in info:
+            log["Policy_Grad_Norms"] = info["policy_grad_norms"]
+        return log
```

### Comparing `robomimic-0.2.0/robomimic/algo/bcq.py` & `robomimic-0.3.0/robomimic/algo/bcq.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,17 @@
 
         if self.algo_config.infinite_horizon:
             # scale terminal rewards by 1 / (1 - gamma) for infinite horizon MDPs
             done_inds = input_batch["dones"].round().long().nonzero(as_tuple=False)[:, 0]
             if done_inds.shape[0] > 0:
                 input_batch["rewards"][done_inds] = input_batch["rewards"][done_inds] * (1. / (1. - self.discount))
 
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
 
     def _train_action_sampler_on_batch(self, batch, epoch, no_backprop=False):
         """
         A modular helper function that can be overridden in case
         subclasses would like to modify training behavior for the
         action sampler.
```

### Comparing `robomimic-0.2.0/robomimic/algo/cql.py` & `robomimic-0.3.0/robomimic/algo/cql.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,17 @@
         discounts = torch.pow(self.algo_config.discount, torch.arange(self.n_step).float()).unsqueeze(0)
         input_batch["rewards"] = (reward_seq * discounts).sum(dim=1).unsqueeze(1)
 
         # consider this n-step seqeunce done if any intermediate dones are present
         done_seq = batch["dones"][:, :self.n_step]
         input_batch["dones"] = (done_seq.sum(dim=1) > 0).float().unsqueeze(1)
 
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
 
     def train_on_batch(self, batch, epoch, validate=False):
         """
         Training on a single batch of data.
 
         Args:
             batch (dict): dictionary with torch.Tensors sampled
```

### Comparing `robomimic-0.2.0/robomimic/algo/gl.py` & `robomimic-0.3.0/robomimic/algo/gl.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,17 @@
         # remove temporal batches for all except scalar signals (to be compatible with model outputs)
         input_batch["obs"] = { k: batch["obs"][k][:, 0, :] for k in batch["obs"] }
         # extract multi-horizon subgoal target
         input_batch["subgoals"] = {k: batch["next_obs"][k][:, self._subgoal_horizon - 1, :] for k in batch["next_obs"]}
         input_batch["target_subgoals"] = input_batch["subgoals"]
         input_batch["goal_obs"] = batch.get("goal_obs", None) # goals may not be present
 
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
 
     def get_actor_goal_for_training_from_processed_batch(self, processed_batch, **kwargs):
         """
         Retrieve subgoals from processed batch to use for training the actor. Subclasses
         can modify this function to change the subgoals.
 
         Args:
@@ -574,15 +576,17 @@
                 will be used for training 
         """
         input_batch = dict()
 
         input_batch["planner"] = self.planner.process_batch_for_training(batch)
         input_batch["value_net"] = self.value_net.process_batch_for_training(batch)
 
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
 
     def train_on_batch(self, batch, epoch, validate=False):
         """
         Training on a single batch of data.
 
         Args:
             batch (dict): dictionary with torch.Tensors sampled
```

### Comparing `robomimic-0.2.0/robomimic/algo/hbc.py` & `robomimic-0.3.0/robomimic/algo/hbc.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         input_batch["actor"] = self.actor.process_batch_for_training(batch)
 
         if self.algo_config.actor_use_random_subgoals:
             # optionally use randomly sampled step between [1, seq_length] as policy goal
             policy_subgoal_indices = torch.randint(
                 low=0, high=self.global_config.train.seq_length, size=(batch["actions"].shape[0],))
             goal_obs = TensorUtils.gather_sequence(batch["next_obs"], policy_subgoal_indices)
-            goal_obs = TensorUtils.to_device(TensorUtils.to_float(goal_obs), self.device)
+            goal_obs = TensorUtils.to_float(TensorUtils.to_device(goal_obs, self.device))
             input_batch["actor"]["goal_obs"] = \
                 self.planner.get_actor_goal_for_training_from_processed_batch(
                     goal_obs,
                     use_latent_subgoals=self.algo_config.latent_subgoal.enabled,
                     use_prior_correction=self.algo_config.latent_subgoal.prior_correction.enabled,
                     num_prior_samples=self.algo_config.latent_subgoal.prior_correction.num_samples,
                 )
@@ -163,15 +163,17 @@
                 self.planner.get_actor_goal_for_training_from_processed_batch(
                     input_batch["planner"],
                     use_latent_subgoals=self.algo_config.latent_subgoal.enabled,
                     use_prior_correction=self.algo_config.latent_subgoal.prior_correction.enabled,
                     num_prior_samples=self.algo_config.latent_subgoal.prior_correction.num_samples,
                 )
 
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
 
     def train_on_batch(self, batch, epoch, validate=False):
         """
         Training on a single batch of data.
 
         Args:
             batch (dict): dictionary with torch.Tensors sampled
```

### Comparing `robomimic-0.2.0/robomimic/algo/iris.py` & `robomimic-0.3.0/robomimic/algo/iris.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,21 +141,23 @@
         input_batch["actor"] = self.actor.process_batch_for_training(batch)
 
         if self.algo_config.actor_use_random_subgoals:
             # optionally use randomly sampled step between [1, seq_length] as policy goal
             policy_subgoal_indices = torch.randint(
                 low=0, high=self.global_config.train.seq_length, size=(batch["actions"].shape[0],))
             goal_obs = TensorUtils.gather_sequence(batch["next_obs"], policy_subgoal_indices)
-            goal_obs = TensorUtils.to_device(TensorUtils.to_float(goal_obs), self.device)
+            goal_obs = TensorUtils.to_float(TensorUtils.to_device(goal_obs, self.device))
             input_batch["actor"]["goal_obs"] = goal_obs
         else:
             # otherwise, use planner subgoal target as goal for the policy
             input_batch["actor"]["goal_obs"] = input_batch["planner"]["planner"]["target_subgoals"]
 
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
 
     def get_state_value(self, obs_dict, goal_dict=None):
         """
         Get state value outputs.
 
         Args:
             obs_dict (dict): current observation
```

### Comparing `robomimic-0.2.0/robomimic/algo/td3_bc.py` & `robomimic-0.3.0/robomimic/algo/td3_bc.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,17 @@
 
         if self.algo_config.infinite_horizon:
             # scale terminal rewards by 1 / (1 - gamma) for infinite horizon MDPs
             done_inds = input_batch["dones"].round().long().nonzero(as_tuple=False)[:, 0]
             if done_inds.shape[0] > 0:
                 input_batch["rewards"][done_inds] = input_batch["rewards"][done_inds] * (1. / (1. - self.discount))
 
-        return TensorUtils.to_device(TensorUtils.to_float(input_batch), self.device)
+        # we move to device first before float conversion because image observation modalities will be uint8 -
+        # this minimizes the amount of data transferred to GPU
+        return TensorUtils.to_float(TensorUtils.to_device(input_batch, self.device))
 
     def _train_critic_on_batch(self, batch, epoch, no_backprop=False):
         """
         A modular helper function that can be overridden in case
         subclasses would like to modify training behavior for the
         critics.
```

### Comparing `robomimic-0.2.0/robomimic/config/__init__.py` & `robomimic-0.3.0/robomimic/config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from robomimic.config.config import Config
 from robomimic.config.base_config import config_factory, get_all_registered_configs
 
 # note: these imports are needed to register these classes in the global config registry
 from robomimic.config.bc_config import BCConfig
 from robomimic.config.bcq_config import BCQConfig
 from robomimic.config.cql_config import CQLConfig
+from robomimic.config.iql_config import IQLConfig
 from robomimic.config.gl_config import GLConfig
 from robomimic.config.hbc_config import HBCConfig
 from robomimic.config.iris_config import IRISConfig
 from robomimic.config.td3_bc_config import TD3_BCConfig
```

### Comparing `robomimic-0.2.0/robomimic/config/base_config.py` & `robomimic-0.3.0/robomimic/config/base_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         # store algo name class property in the config (must be implemented by subclasses)
         self.algo_name = type(self).ALGO_NAME
 
         self.experiment_config()
         self.train_config()
         self.algo_config()
         self.observation_config()
+        self.meta_config()
 
         # After Config init, new keys cannot be added to the config, except under nested
         # attributes that have called @do_not_lock_keys
         self.lock_keys()
 
     @property
     @classmethod
@@ -77,17 +78,19 @@
         which has several experiment settings such as the name of the training run, 
         whether to do logging, whether to save models (and how often), whether to render 
         videos, and whether to do rollouts (and how often). This class has a default 
         implementation that usually doesn't need to be overriden.
         """
 
         self.experiment.name = "test"                               # name of experiment used to make log files
-        self.experiment.validate = True                             # whether to do validation or not
+        self.experiment.validate = False                            # whether to do validation or not
         self.experiment.logging.terminal_output_to_txt = True       # whether to log stdout to txt file 
         self.experiment.logging.log_tb = True                       # enable tensorboard logging
+        self.experiment.logging.log_wandb = False                   # enable wandb logging
+        self.experiment.logging.wandb_proj_name = "debug"           # project name if using wandb
 
 
         ## save config - if and when to save model checkpoints ##
         self.experiment.save.enabled = True                         # whether model saving should be enabled or disabled
         self.experiment.save.every_n_seconds = None                 # save model every n seconds (set to None to disable)
         self.experiment.save.every_n_epochs = 50                    # save model every n epochs (set to None to disable)
         self.experiment.save.epochs = []                            # save model on these specific epochs
@@ -148,25 +151,36 @@
         # to None to use no caching - in this case, every batch sample is retrieved via file i/o.
         # You should almost never set this to None, even for large image datasets.
         self.train.hdf5_cache_mode = "all"
 
         # used for parallel data loading
         self.train.hdf5_use_swmr = True
 
+        # whether to load "next_obs" group from hdf5 - only needed for batch / offline RL algorithms
+        self.train.hdf5_load_next_obs = True
+
         # if true, normalize observations at train and test time, using the global mean and standard deviation
         # of each observation in each dimension, computed across the training set. See SequenceDataset.normalize_obs
         # in utils/dataset.py for more information.
         self.train.hdf5_normalize_obs = False
 
         # if provided, use the list of demo keys under the hdf5 group "mask/@hdf5_filter_key" for training, instead 
         # of the full dataset. This provides a convenient way to train on only a subset of the trajectories in a dataset.
         self.train.hdf5_filter_key = None
 
+        # if provided, use the list of demo keys under the hdf5 group "mask/@hdf5_validation_filter_key" for validation.
+        # Must be provided if @experiment.validate is True.
+        self.train.hdf5_validation_filter_key = None
+
         # length of experience sequence to fetch from the dataset
+        # and whether to pad the beginning / end of the sequence at boundaries of trajectory in dataset
         self.train.seq_length = 1
+        self.train.pad_seq_length = True
+        self.train.frame_stack = 1
+        self.train.pad_frame_stack = True
 
         # keys from hdf5 to load into each batch, besides "obs" and "next_obs". If algorithms
         # require additional keys from each trajectory in the hdf5, they should be specified here.
         self.train.dataset_keys = (
             "actions", 
             "rewards", 
             "dones",
@@ -231,55 +245,50 @@
 
         # Low Dim: Obs Randomizer settings
         self.observation.encoder.low_dim.obs_randomizer_class = None
         self.observation.encoder.low_dim.obs_randomizer_kwargs = Config()       # No kwargs by default
         self.observation.encoder.low_dim.obs_randomizer_kwargs.do_not_lock_keys()
 
         # =============== RGB default encoder (ResNet backbone + linear layer output) ===============
-        self.observation.encoder.rgb.core_class = "VisualCore"
-        self.observation.encoder.rgb.core_kwargs.feature_dimension = 64
-        self.observation.encoder.rgb.core_kwargs.flatten = True
-        self.observation.encoder.rgb.core_kwargs.backbone_class = "ResNet18Conv"
-        self.observation.encoder.rgb.core_kwargs.backbone_kwargs.pretrained = False
-        self.observation.encoder.rgb.core_kwargs.backbone_kwargs.input_coord_conv = False
-        self.observation.encoder.rgb.core_kwargs.backbone_kwargs.do_not_lock_keys()
-        self.observation.encoder.rgb.core_kwargs.pool_class = "SpatialSoftmax"                # Alternate options are "SpatialMeanPool" or None (no pooling)
-        self.observation.encoder.rgb.core_kwargs.pool_kwargs.num_kp = 32                      # Default arguments for "SpatialSoftmax"
-        self.observation.encoder.rgb.core_kwargs.pool_kwargs.learnable_temperature = False    # Default arguments for "SpatialSoftmax"
-        self.observation.encoder.rgb.core_kwargs.pool_kwargs.temperature = 1.0                # Default arguments for "SpatialSoftmax"
-        self.observation.encoder.rgb.core_kwargs.pool_kwargs.noise_std = 0.0                  # Default arguments for "SpatialSoftmax"
-        self.observation.encoder.rgb.core_kwargs.pool_kwargs.output_variance = False          # Default arguments for "SpatialSoftmax"
-        self.observation.encoder.rgb.core_kwargs.pool_kwargs.do_not_lock_keys()
+        self.observation.encoder.rgb.core_class = "VisualCore"                  # Default VisualCore class combines backbone (like ResNet-18) with pooling operation (like spatial softmax)
+        self.observation.encoder.rgb.core_kwargs = Config()                     # See models/obs_core.py for important kwargs to set and defaults used
+        self.observation.encoder.rgb.core_kwargs.do_not_lock_keys()
 
         # RGB: Obs Randomizer settings
-        self.observation.encoder.rgb.obs_randomizer_class = None                  # Can set to 'CropRandomizer' to use crop randomization
-        self.observation.encoder.rgb.obs_randomizer_kwargs.crop_height = 76       # Default arguments for "CropRandomizer"
-        self.observation.encoder.rgb.obs_randomizer_kwargs.crop_width = 76        # Default arguments for "CropRandomizer"
-        self.observation.encoder.rgb.obs_randomizer_kwargs.num_crops = 1          # Default arguments for "CropRandomizer"
-        self.observation.encoder.rgb.obs_randomizer_kwargs.pos_enc = False        # Default arguments for "CropRandomizer"
+        self.observation.encoder.rgb.obs_randomizer_class = None                # Can set to 'CropRandomizer' to use crop randomization
+        self.observation.encoder.rgb.obs_randomizer_kwargs = Config()           # See models/obs_core.py for important kwargs to set and defaults used
         self.observation.encoder.rgb.obs_randomizer_kwargs.do_not_lock_keys()
 
         # Allow for other custom modalities to be specified
         self.observation.encoder.do_not_lock_keys()
 
         # =============== Depth default encoder (same as rgb) ===============
         self.observation.encoder.depth = deepcopy(self.observation.encoder.rgb)
 
         # =============== Scan default encoder (Conv1d backbone + linear layer output) ===============
         self.observation.encoder.scan = deepcopy(self.observation.encoder.rgb)
-        self.observation.encoder.scan.core_kwargs.pop("backbone_class")
-        self.observation.encoder.scan.core_kwargs.pop("backbone_kwargs")
 
         # Scan: Modify the core class + kwargs, otherwise, is same as rgb encoder
-        self.observation.encoder.scan.core_class = "ScanCore"
-        self.observation.encoder.scan.core_kwargs.conv_activation = "relu"
-        self.observation.encoder.scan.core_kwargs.conv_kwargs.out_channels = [32, 64, 64]
-        self.observation.encoder.scan.core_kwargs.conv_kwargs.kernel_size = [8, 4, 2]
-        self.observation.encoder.scan.core_kwargs.conv_kwargs.stride = [4, 2, 1]
-
+        self.observation.encoder.scan.core_class = "ScanCore"                   # Default ScanCore class uses Conv1D to process this modality
+        self.observation.encoder.scan.core_kwargs = Config()                    # See models/obs_core.py for important kwargs to set and defaults used
+        self.observation.encoder.scan.core_kwargs.do_not_lock_keys()
+
+    def meta_config(self):
+        """
+        This function populates the `config.meta` attribute of the config. This portion of the config 
+        is used to specify job information primarily for hyperparameter sweeps.
+        It contains hyperparameter keys and values, which are populated automatically
+        by the hyperparameter config generator (see `utils/hyperparam_utils.py`).
+        These values are read by the wandb logger (see `utils/log_utils.py`) to set job tags.
+        """
+        
+        self.meta.hp_base_config_file = None            # base config file in hyperparam sweep
+        self.meta.hp_keys = []                          # relevant keys (swept) in hyperparam sweep
+        self.meta.hp_values = []                        # values corresponding to keys in hyperparam sweep
+    
     @property
     def use_goals(self):
         # whether the agent is goal-conditioned
         return len([obs_key for modality in self.observation.modalities.goal.values() for obs_key in modality]) > 0
 
     @property
     def all_obs_keys(self):
```

### Comparing `robomimic-0.2.0/robomimic/config/bc_config.py` & `robomimic-0.3.0/robomimic/config/gl_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,43 @@
 """
-Config for BC algorithm.
+Config for Goal Learning (sub-algorithm used by hierarchical models like HBC and IRIS).
+This class of model predicts (or samples) subgoal observations given a current observation.
 """
 
 from robomimic.config.base_config import BaseConfig
 
 
-class BCConfig(BaseConfig):
-    ALGO_NAME = "bc"
+class GLConfig(BaseConfig):
+    ALGO_NAME = "gl"
 
     def algo_config(self):
         """
         This function populates the `config.algo` attribute of the config, and is given to the 
         `Algo` subclass (see `algo/algo.py`) for each algorithm through the `algo_config` 
         argument to the constructor. Any parameter that an algorithm needs to determine its 
         training and test-time behavior should be populated here.
         """
 
         # optimization parameters
-        self.algo.optim_params.policy.learning_rate.initial = 1e-4      # policy learning rate
-        self.algo.optim_params.policy.learning_rate.decay_factor = 0.1  # factor to decay LR by (if epoch schedule non-empty)
-        self.algo.optim_params.policy.learning_rate.epoch_schedule = [] # epochs where LR decay occurs
-        self.algo.optim_params.policy.regularization.L2 = 0.00          # L2 regularization strength
-
-        # loss weights
-        self.algo.loss.l2_weight = 1.0      # L2 loss weight
-        self.algo.loss.l1_weight = 0.0      # L1 loss weight
-        self.algo.loss.cos_weight = 0.0     # cosine loss weight
-
-        # MLP network architecture (layers after observation encoder and RNN, if present)
-        self.algo.actor_layer_dims = (1024, 1024)
-
-        # stochastic Gaussian policy settings
-        self.algo.gaussian.enabled = False              # whether to train a Gaussian policy
-        self.algo.gaussian.fixed_std = False            # whether to train std output or keep it constant
-        self.algo.gaussian.init_std = 0.1               # initial standard deviation (or constant)
-        self.algo.gaussian.min_std = 0.01               # minimum std output from network
-        self.algo.gaussian.std_activation = "softplus"  # activation to use for std output from policy net
-        self.algo.gaussian.low_noise_eval = True        # low-std at test-time 
-
-        # stochastic GMM policy settings
-        self.algo.gmm.enabled = False                   # whether to train a GMM policy
-        self.algo.gmm.num_modes = 5                     # number of GMM modes
-        self.algo.gmm.min_std = 0.0001                  # minimum std output from network
-        self.algo.gmm.std_activation = "softplus"       # activation to use for std output from policy net
-        self.algo.gmm.low_noise_eval = True             # low-std at test-time 
-
-        # stochastic VAE policy settings
-        self.algo.vae.enabled = False                   # whether to train a VAE policy
-        self.algo.vae.latent_dim = 14                   # VAE latent dimnsion - set to twice the dimensionality of action space
-        self.algo.vae.latent_clip = None                # clip latent space when decoding (set to None to disable)
-        self.algo.vae.kl_weight = 1.                    # beta-VAE weight to scale KL loss relative to reconstruction loss in ELBO
+        self.algo.optim_params.goal_network.learning_rate.initial = 1e-4        # goal network learning rate
+        self.algo.optim_params.goal_network.learning_rate.decay_factor = 0.1    # factor to decay LR by (if epoch schedule non-empty)
+        self.algo.optim_params.goal_network.learning_rate.epoch_schedule = []   # epochs where LR decay occurs
+        self.algo.optim_params.goal_network.regularization.L2 = 0.00
+
+        # subgoal definition: observation that is @subgoal_horizon number of timesteps in future from current observation
+        self.algo.subgoal_horizon = 10 
+
+        # MLP size for deterministic goal network (unused if VAE is enabled)
+        self.algo.ae.planner_layer_dims = (300, 400)
+
+        # ================== VAE config ==================
+        self.algo.vae.enabled = True                                        # set to true to use VAE network
+        self.algo.vae.latent_dim = 16                                       # VAE latent dimension
+        self.algo.vae.latent_clip = None                                    # clip latent space when decoding (set to None to disable)
+        self.algo.vae.kl_weight = 1.                                        # beta-VAE weight to scale KL loss relative to reconstruction loss in ELBO
 
         # VAE decoder settings
         self.algo.vae.decoder.is_conditioned = True                         # whether decoder should condition on observation
         self.algo.vae.decoder.reconstruction_sum_across_elements = False    # sum instead of mean for reconstruction loss
 
         # VAE prior settings
         self.algo.vae.prior.learn = False                                   # learn Gaussian / GMM prior instead of N(0, 1)
@@ -68,16 +52,38 @@
         self.algo.vae.prior.categorical_temp_anneal_step = 0.001            # linear temp annealing rate
         self.algo.vae.prior.categorical_min_temp = 0.3                      # lowest gumbel-softmax temp
 
         self.algo.vae.encoder_layer_dims = (300, 400)                       # encoder MLP layer dimensions
         self.algo.vae.decoder_layer_dims = (300, 400)                       # decoder MLP layer dimensions
         self.algo.vae.prior_layer_dims = (300, 400)                         # prior MLP layer dimensions (if learning conditioned prior)
 
-        # RNN policy settings
-        self.algo.rnn.enabled = False       # whether to train RNN policy
-        self.algo.rnn.horizon = 10          # unroll length for RNN - should usually match train.seq_length
-        self.algo.rnn.hidden_dim = 400      # hidden dimension size    
-        self.algo.rnn.rnn_type = "LSTM"     # rnn type - one of "LSTM" or "GRU"
-        self.algo.rnn.num_layers = 2        # number of RNN layers that are stacked
-        self.algo.rnn.open_loop = False     # if True, action predictions are only based on a single observation (not sequence)
-        self.algo.rnn.kwargs.bidirectional = False            # rnn kwargs
-        self.algo.rnn.kwargs.do_not_lock_keys()
+    def observation_config(self):
+        """
+        Update from superclass to specify subgoal modalities.
+        """
+        super(GLConfig, self).observation_config()
+        self.observation.modalities.subgoal.low_dim = [                     # specify low-dim subgoal observations for agent to predict
+            "robot0_eef_pos", 
+            "robot0_eef_quat", 
+            "robot0_gripper_qpos", 
+            "object",
+        ]
+        self.observation.modalities.subgoal.rgb = []                      # specify rgb image subgoal observations for agent to predict
+        self.observation.modalities.subgoal.depth = []
+        self.observation.modalities.subgoal.scan = []
+        self.observation.modalities.subgoal.do_not_lock_keys()
+
+    @property
+    def all_obs_keys(self):
+        """
+        Update from superclass to include subgoals.
+        """
+        # pool all modalities
+        return sorted(tuple(set([
+            obs_key for group in [
+                self.observation.modalities.obs.values(),
+                self.observation.modalities.goal.values(),
+                self.observation.modalities.subgoal.values(),
+            ]
+            for modality in group
+            for obs_key in modality
+        ])))
```

### Comparing `robomimic-0.2.0/robomimic/config/bcq_config.py` & `robomimic-0.3.0/robomimic/config/bcq_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         # use VAE by default
         self.algo.action_sampler.vae.enabled = True
         # remove unused parts of BCConfig algo config
         del self.algo.action_sampler.optim_params           # since action sampler optim params specified at top-level
         del self.algo.action_sampler.loss
         del self.algo.action_sampler.gaussian
         del self.algo.action_sampler.rnn
+        del self.algo.action_sampler.transformer
 
         # Number of epochs before freezing encoder (-1 for no freezing). Only applies to cVAE-based action samplers.
         with self.algo.action_sampler.unlocked():
             self.algo.action_sampler.freeze_encoder_epoch = -1
 
         # ================== Actor Network Config ===================
         self.algo.actor.enabled = False                     # whether to use the actor perturbation network
```

### Comparing `robomimic-0.2.0/robomimic/config/config.py` & `robomimic-0.3.0/robomimic/config/config.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/config/cql_config.py` & `robomimic-0.3.0/robomimic/config/cql_config.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/config/hbc_config.py` & `robomimic-0.3.0/robomimic/config/hbc_config.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/config/iris_config.py` & `robomimic-0.3.0/robomimic/config/iris_config.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/config/td3_bc_config.py` & `robomimic-0.3.0/robomimic/config/td3_bc_config.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/envs/env_base.py` & `robomimic-0.3.0/robomimic/envs/env_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,22 @@
     def type(self):
         """
         Returns environment type (int) for this kind of environment.
         This helps identify this env class.
         """
         return
 
+    @property
+    def version(self):
+        """
+        Returns version of environment (str).
+        This is not an abstract method, some subclasses do not implement it
+        """
+        return None
+
     @abc.abstractmethod
     def serialize(self):
         """
         Save all information needed to re-instantiate this environment in a dictionary.
         This is the same as @env_meta - environment metadata stored in hdf5 datasets,
         and used in utils/env_utils.py.
         """
```

### Comparing `robomimic-0.2.0/robomimic/envs/env_gym.py` & `robomimic-0.3.0/robomimic/envs/env_gym.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/envs/env_ig_momart.py` & `robomimic-0.3.0/robomimic/envs/env_ig_momart.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/envs/env_robosuite.py` & `robomimic-0.3.0/robomimic/envs/env_robosuite.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 import json
 import numpy as np
 from copy import deepcopy
 
 import mujoco_py
 import robosuite
-from robosuite.utils.mjcf_utils import postprocess_model_xml
 
 import robomimic.utils.obs_utils as ObsUtils
 import robomimic.envs.env_base as EB
 
 
 class EnvRobosuite(EB.EnvBase):
     """Wrapper class for robosuite environments (https://github.com/ARISE-Initiative/robosuite)"""
@@ -127,15 +126,21 @@
         Returns:
             observation (dict): observation dictionary after setting the simulator state (only
                 if "states" is in @state)
         """
         should_ret = False
         if "model" in state:
             self.reset()
-            xml = postprocess_model_xml(state["model"])
+            robosuite_version_id = int(robosuite.__version__.split(".")[1])
+            if robosuite_version_id <= 3:
+                from robosuite.utils.mjcf_utils import postprocess_model_xml
+                xml = postprocess_model_xml(state["model"])
+            else:
+                # v1.4 and above use the class-based edit_model_xml function
+                xml = self.env.edit_model_xml(state["model"])
             self.env.reset_from_xml_string(xml)
             self.env.sim.reset()
             if not self._is_v1:
                 # hide teleop visualization after restoring from model
                 self.env.sim.model.site_rgba[self.env.eef_site_id] = np.array([0., 0., 0., 0.])
                 self.env.sim.model.site_rgba[self.env.eef_cylinder_id] = np.array([0., 0., 0., 0.])
         if "states" in state:
@@ -192,15 +197,15 @@
         if self._is_v1:
             for robot in self.env.robots:
                 # add all robot-arm-specific observations. Note the (k not in ret) check
                 # ensures that we don't accidentally add robot wrist images a second time
                 pf = robot.robot_model.naming_prefix
                 for k in di:
                     if k.startswith(pf) and (k not in ret) and \
-                            (not k.endswith("proprio-state")) and (k in ObsUtils.OBS_KEYS_TO_MODALITIES):
+                            (not k.endswith("proprio-state")):
                         ret[k] = np.array(di[k])
         else:
             # minimal proprioception for older versions of robosuite
             ret["proprio"] = np.array(di["robot-state"])
             ret["eef_pos"] = np.array(di["eef_pos"])
             ret["eef_quat"] = np.array(di["eef_quat"])
             ret["gripper_qpos"] = np.array(di["gripper_qpos"])
@@ -270,21 +275,33 @@
     def type(self):
         """
         Returns environment type (int) for this kind of environment.
         This helps identify this env class.
         """
         return EB.EnvType.ROBOSUITE_TYPE
 
+    @property
+    def version(self):
+        """
+        Returns version of robosuite used for this environment, eg. 1.2.0
+        """
+        return robosuite.__version__
+
     def serialize(self):
         """
         Save all information needed to re-instantiate this environment in a dictionary.
         This is the same as @env_meta - environment metadata stored in hdf5 datasets,
         and used in utils/env_utils.py.
         """
-        return dict(env_name=self.name, type=self.type, env_kwargs=deepcopy(self._init_kwargs))
+        return dict(
+            env_name=self.name,
+            env_version=self.version,
+            type=self.type,
+            env_kwargs=deepcopy(self._init_kwargs)
+        )
 
     @classmethod
     def create_for_data_processing(
         cls, 
         env_name, 
         camera_names, 
         camera_height,
```

### Comparing `robomimic-0.2.0/robomimic/exps/templates/bc.json` & `robomimic-0.3.0/robomimic/exps/templates/hbc.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5522098515519568%*

 * *Differences: {"'algo'": "{replace: OrderedDict([('mode', 'separate'), ('actor_use_random_subgoals', False), "*

 * *           "('subgoal_update_interval', 10), ('latent_subgoal', OrderedDict([('enabled', False), "*

 * *           "('prior_correction', OrderedDict([('enabled', False), ('num_samples', 100)]))])), "*

 * *           "('planner', OrderedDict([('optim_params', OrderedDict([('goal_network', "*

 * *           "OrderedDict([('learning_rate', OrderedDict([('initial', 0.0001), ('decay_factor', "*

 * *           "0.1), ('epoch_schedule', [ […]*

```diff
@@ -1,101 +1,137 @@
 {
     "algo": {
-        "actor_layer_dims": [
-            1024,
-            1024
-        ],
-        "gaussian": {
-            "enabled": false,
-            "fixed_std": false,
-            "init_std": 0.1,
-            "low_noise_eval": true,
-            "min_std": 0.01,
-            "std_activation": "softplus"
-        },
-        "gmm": {
-            "enabled": false,
-            "low_noise_eval": true,
-            "min_std": 0.0001,
-            "num_modes": 5,
-            "std_activation": "softplus"
-        },
-        "loss": {
-            "cos_weight": 0.0,
-            "l1_weight": 0.0,
-            "l2_weight": 1.0
-        },
-        "optim_params": {
-            "policy": {
-                "learning_rate": {
-                    "decay_factor": 0.1,
-                    "epoch_schedule": [],
-                    "initial": 0.0001
-                },
-                "regularization": {
-                    "L2": 0.0
+        "actor": {
+            "actor_layer_dims": [
+                1024,
+                1024
+            ],
+            "loss": {
+                "cos_weight": 0.0,
+                "l1_weight": 0.0,
+                "l2_weight": 1.0
+            },
+            "optim_params": {
+                "policy": {
+                    "learning_rate": {
+                        "decay_factor": 0.1,
+                        "epoch_schedule": [],
+                        "initial": 0.0001,
+                        "scheduler_type": "multistep"
+                    },
+                    "optimizer_type": "adam",
+                    "regularization": {
+                        "L2": 0.0
+                    }
                 }
+            },
+            "rnn": {
+                "enabled": true,
+                "hidden_dim": 400,
+                "horizon": 10,
+                "kwargs": {
+                    "bidirectional": false
+                },
+                "num_layers": 2,
+                "open_loop": false,
+                "rnn_type": "LSTM"
+            },
+            "transformer": {
+                "activation": "gelu",
+                "attn_dropout": 0.1,
+                "block_output_dropout": 0.1,
+                "context_length": 10,
+                "emb_dropout": 0.1,
+                "embed_dim": 512,
+                "enabled": false,
+                "nn_parameter_for_timesteps": true,
+                "num_heads": 8,
+                "num_layers": 6,
+                "sinusoidal_embedding": false,
+                "supervise_all_steps": false
             }
         },
-        "rnn": {
+        "actor_use_random_subgoals": false,
+        "latent_subgoal": {
             "enabled": false,
-            "hidden_dim": 400,
-            "horizon": 10,
-            "kwargs": {
-                "bidirectional": false
-            },
-            "num_layers": 2,
-            "open_loop": false,
-            "rnn_type": "LSTM"
+            "prior_correction": {
+                "enabled": false,
+                "num_samples": 100
+            }
         },
-        "vae": {
-            "decoder": {
-                "is_conditioned": true,
-                "reconstruction_sum_across_elements": false
+        "mode": "separate",
+        "planner": {
+            "ae": {
+                "planner_layer_dims": [
+                    300,
+                    400
+                ]
             },
-            "decoder_layer_dims": [
-                300,
-                400
-            ],
-            "enabled": false,
-            "encoder_layer_dims": [
-                300,
-                400
-            ],
-            "kl_weight": 1.0,
-            "latent_clip": null,
-            "latent_dim": 14,
-            "prior": {
-                "categorical_dim": 10,
-                "categorical_gumbel_softmax_hard": false,
-                "categorical_init_temp": 1.0,
-                "categorical_min_temp": 0.3,
-                "categorical_temp_anneal_step": 0.001,
-                "gmm_learn_weights": false,
-                "gmm_num_modes": 10,
-                "is_conditioned": false,
-                "learn": false,
-                "use_categorical": false,
-                "use_gmm": false
+            "optim_params": {
+                "goal_network": {
+                    "learning_rate": {
+                        "decay_factor": 0.1,
+                        "epoch_schedule": [],
+                        "initial": 0.0001
+                    },
+                    "regularization": {
+                        "L2": 0.0
+                    }
+                }
             },
-            "prior_layer_dims": [
-                300,
-                400
-            ]
-        }
+            "subgoal_horizon": 10,
+            "vae": {
+                "decoder": {
+                    "is_conditioned": true,
+                    "reconstruction_sum_across_elements": false
+                },
+                "decoder_layer_dims": [
+                    300,
+                    400
+                ],
+                "enabled": true,
+                "encoder_layer_dims": [
+                    300,
+                    400
+                ],
+                "kl_weight": 1.0,
+                "latent_clip": null,
+                "latent_dim": 16,
+                "prior": {
+                    "categorical_dim": 10,
+                    "categorical_gumbel_softmax_hard": false,
+                    "categorical_init_temp": 1.0,
+                    "categorical_min_temp": 0.3,
+                    "categorical_temp_anneal_step": 0.001,
+                    "gmm_learn_weights": false,
+                    "gmm_num_modes": 10,
+                    "is_conditioned": false,
+                    "learn": false,
+                    "use_categorical": false,
+                    "use_gmm": false
+                },
+                "prior_layer_dims": [
+                    300,
+                    400
+                ]
+            }
+        },
+        "subgoal_update_interval": 10
     },
-    "algo_name": "bc",
+    "algo_name": "hbc",
     "experiment": {
         "additional_envs": null,
         "env": null,
         "epoch_every_n_steps": 100,
         "keep_all_videos": false,
         "logging": {
             "log_tb": true,
-            "terminal_output_to_txt": true
+            "log_wandb": false,
+            "terminal_output_to_txt": true,
+            "wandb_proj_name": "debug"
         },
         "name": "test",
         "render": false,
         "render_video": true,
         "rollout": {
             "enabled": true,
             "horizon": 400,
@@ -109,154 +145,149 @@
             "epochs": [],
             "every_n_epochs": 50,
             "every_n_seconds": null,
             "on_best_rollout_return": false,
             "on_best_rollout_success_rate": true,
             "on_best_validation": false
         },
-        "validate": true,
+        "validate": false,
         "validation_epoch_every_n_steps": 10,
         "video_skip": 5
     },
+    "meta": {
+        "hp_base_config_file": null,
+        "hp_keys": [],
+        "hp_values": []
+    },
     "observation": {
-        "encoder": {
-            "depth": {
-                "core_class": "VisualCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    }
+        "actor": {
+            "encoder": {
+                "depth": {
+                    "core_class": "VisualCore",
+                    "core_kwargs": {},
+                    "obs_randomizer_class": null,
+                    "obs_randomizer_kwargs": {}
                 },
-                "feature_dimension": 64,
-                "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
-            },
-            "low_dim": {
-                "core_class": null,
-                "core_kwargs": {},
-                "feature_dimension": null,
-                "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {}
-            },
-            "rgb": {
-                "core_class": "VisualCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    }
+                "low_dim": {
+                    "core_class": null,
+                    "core_kwargs": {},
+                    "obs_randomizer_class": null,
+                    "obs_randomizer_kwargs": {}
                 },
-                "feature_dimension": 64,
-                "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
+                "rgb": {
+                    "core_class": "VisualCore",
+                    "core_kwargs": {},
+                    "obs_randomizer_class": null,
+                    "obs_randomizer_kwargs": {}
+                },
+                "scan": {
+                    "core_class": "ScanCore",
+                    "core_kwargs": {},
+                    "obs_randomizer_class": null,
+                    "obs_randomizer_kwargs": {}
                 }
             },
-            "scan": {
-                "core_class": "ScanCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    },
-                    "conv_kwargs": {
-                        "kernel_size": [
-                            8,
-                            4,
-                            2
-                        ],
-                        "out_channels": [
-                            32,
-                            64,
-                            64
-                        ],
-                        "stride": [
-                            4,
-                            2,
-                            1
-                        ]
-                    }
+            "modalities": {
+                "goal": {
+                    "depth": [],
+                    "low_dim": [],
+                    "rgb": [],
+                    "scan": []
                 },
-                "feature_dimension": 64,
-                "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
+                "obs": {
+                    "depth": [],
+                    "low_dim": [
+                        "robot0_eef_pos",
+                        "robot0_eef_quat",
+                        "robot0_gripper_qpos",
+                        "object"
+                    ],
+                    "rgb": [],
+                    "scan": []
                 }
             }
         },
-        "modalities": {
-            "goal": {
-                "depth": [],
-                "low_dim": [],
-                "rgb": [],
-                "scan": []
+        "planner": {
+            "encoder": {
+                "depth": {
+                    "core_class": "VisualCore",
+                    "core_kwargs": {},
+                    "obs_randomizer_class": null,
+                    "obs_randomizer_kwargs": {}
+                },
+                "low_dim": {
+                    "core_class": null,
+                    "core_kwargs": {},
+                    "obs_randomizer_class": null,
+                    "obs_randomizer_kwargs": {}
+                },
+                "rgb": {
+                    "core_class": "VisualCore",
+                    "core_kwargs": {},
+                    "obs_randomizer_class": null,
+                    "obs_randomizer_kwargs": {}
+                },
+                "scan": {
+                    "core_class": "ScanCore",
+                    "core_kwargs": {},
+                    "obs_randomizer_class": null,
+                    "obs_randomizer_kwargs": {}
+                }
             },
-            "obs": {
-                "depth": [],
-                "low_dim": [
-                    "robot0_eef_pos",
-                    "robot0_eef_quat",
-                    "robot0_gripper_qpos",
-                    "object"
-                ],
-                "rgb": [],
-                "scan": []
+            "modalities": {
+                "goal": {
+                    "depth": [],
+                    "low_dim": [],
+                    "rgb": [],
+                    "scan": []
+                },
+                "obs": {
+                    "depth": [],
+                    "low_dim": [
+                        "robot0_eef_pos",
+                        "robot0_eef_quat",
+                        "robot0_gripper_qpos",
+                        "object"
+                    ],
+                    "rgb": [],
+                    "scan": []
+                },
+                "subgoal": {
+                    "depth": [],
+                    "low_dim": [
+                        "robot0_eef_pos",
+                        "robot0_eef_quat",
+                        "robot0_gripper_qpos",
+                        "object"
+                    ],
+                    "rgb": [],
+                    "scan": []
+                }
             }
         }
     },
     "train": {
         "batch_size": 100,
         "cuda": true,
         "data": null,
         "dataset_keys": [
             "actions",
             "rewards",
             "dones"
         ],
+        "frame_stack": 1,
         "goal_mode": null,
         "hdf5_cache_mode": "all",
         "hdf5_filter_key": null,
+        "hdf5_load_next_obs": true,
         "hdf5_normalize_obs": false,
         "hdf5_use_swmr": true,
+        "hdf5_validation_filter_key": null,
         "num_data_workers": 0,
         "num_epochs": 2000,
-        "output_dir": "../bc_trained_models",
+        "output_dir": "../hbc_trained_models",
+        "pad_frame_stack": true,
+        "pad_seq_length": true,
         "seed": 1,
-        "seq_length": 1
+        "seq_length": 10
     }
 }
```

### Comparing `robomimic-0.2.0/robomimic/exps/templates/bcq.json` & `robomimic-0.3.0/robomimic/exps/templates/bcq.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8016106974166185%*

 * *Differences: {"'experiment'": "{'validate': False, 'logging': {'log_wandb': False, 'wandb_proj_name': 'debug'}}",*

 * * "'meta'": "OrderedDict([('hp_base_config_file', None), ('hp_keys', []), ('hp_values', [])])",*

 * * "'observation'": "{'encoder': {'low_dim': {delete: ['feature_dimension']}, 'rgb': {'core_kwargs': "*

 * *                  "{replace: OrderedDict()}, 'obs_randomizer_kwargs': {replace: OrderedDict()}, "*

 * *                  "delete: ['feature_dimension', 'pool_class', 'pool_kwargs']}, 'depth': "*

 * *                  "{'core_ […]*

```diff
@@ -123,15 +123,17 @@
     "experiment": {
         "additional_envs": null,
         "env": null,
         "epoch_every_n_steps": 100,
         "keep_all_videos": false,
         "logging": {
             "log_tb": true,
-            "terminal_output_to_txt": true
+            "log_wandb": false,
+            "terminal_output_to_txt": true,
+            "wandb_proj_name": "debug"
         },
         "name": "test",
         "render": false,
         "render_video": true,
         "rollout": {
             "enabled": true,
             "horizon": 400,
@@ -145,118 +147,48 @@
             "epochs": [],
             "every_n_epochs": 50,
             "every_n_seconds": null,
             "on_best_rollout_return": false,
             "on_best_rollout_success_rate": true,
             "on_best_validation": false
         },
-        "validate": true,
+        "validate": false,
         "validation_epoch_every_n_steps": 10,
         "video_skip": 5
     },
+    "meta": {
+        "hp_base_config_file": null,
+        "hp_keys": [],
+        "hp_values": []
+    },
     "observation": {
         "encoder": {
             "depth": {
                 "core_class": "VisualCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             },
             "low_dim": {
                 "core_class": null,
                 "core_kwargs": {},
-                "feature_dimension": null,
                 "obs_randomizer_class": null,
                 "obs_randomizer_kwargs": {}
             },
             "rgb": {
                 "core_class": "VisualCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             },
             "scan": {
                 "core_class": "ScanCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    },
-                    "conv_kwargs": {
-                        "kernel_size": [
-                            8,
-                            4,
-                            2
-                        ],
-                        "out_channels": [
-                            32,
-                            64,
-                            64
-                        ],
-                        "stride": [
-                            4,
-                            2,
-                            1
-                        ]
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             }
         },
         "modalities": {
             "goal": {
                 "depth": [],
                 "low_dim": [],
                 "rgb": [],
@@ -280,19 +212,24 @@
         "cuda": true,
         "data": null,
         "dataset_keys": [
             "actions",
             "rewards",
             "dones"
         ],
+        "frame_stack": 1,
         "goal_mode": null,
         "hdf5_cache_mode": "all",
         "hdf5_filter_key": null,
+        "hdf5_load_next_obs": true,
         "hdf5_normalize_obs": false,
         "hdf5_use_swmr": true,
+        "hdf5_validation_filter_key": null,
         "num_data_workers": 0,
         "num_epochs": 2000,
         "output_dir": "../bcq_trained_models",
+        "pad_frame_stack": true,
+        "pad_seq_length": true,
         "seed": 1,
         "seq_length": 1
     }
 }
```

### Comparing `robomimic-0.2.0/robomimic/exps/templates/cql.json` & `robomimic-0.3.0/robomimic/exps/templates/iql.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6700749797686475%*

 * *Differences: {"'algo'": "{'optim_params': {'critic': {'learning_rate': {'initial': 0.0001}}, 'actor': "*

 * *           "{'learning_rate': {'initial': 0.0001}}, 'vf': OrderedDict([('learning_rate', "*

 * *           "OrderedDict([('initial', 0.0001), ('decay_factor', 0.0), ('epoch_schedule', [])])), "*

 * *           "('regularization', OrderedDict([('L2', 0.0)]))])}, 'target_tau': 0.01, 'actor': "*

 * *           "{'net': {'common': {'std_activation': 'softplus', 'use_tanh': False}, 'gmm': "*

 * *           "OrderedDict([('num_modes', 5), ('mi […]*

```diff
@@ -1,84 +1,96 @@
 {
     "algo": {
         "actor": {
-            "bc_start_steps": 0,
             "layer_dims": [
                 300,
                 400
             ],
             "max_gradient_norm": null,
             "net": {
                 "common": {
                     "low_noise_eval": true,
-                    "std_activation": "exp",
-                    "use_tanh": true
+                    "std_activation": "softplus",
+                    "use_tanh": false
                 },
                 "gaussian": {
                     "fixed_std": false,
                     "init_last_fc_weight": 0.001,
                     "init_std": 0.3
                 },
+                "gmm": {
+                    "min_std": 0.0001,
+                    "num_modes": 5
+                },
                 "type": "gaussian"
-            },
-            "target_entropy": "default"
+            }
+        },
+        "adv": {
+            "beta": 1.0,
+            "clip_adv_value": null,
+            "use_final_clip": true
         },
         "critic": {
-            "cql_weight": 1.0,
-            "deterministic_backup": true,
             "ensemble": {
                 "n": 2
             },
             "layer_dims": [
                 300,
                 400
             ],
             "max_gradient_norm": null,
-            "min_q_weight": 1.0,
-            "num_action_samples": 1,
-            "num_random_actions": 10,
-            "target_q_gap": 5.0,
-            "use_huber": false,
-            "value_bounds": null
+            "use_huber": false
         },
         "discount": 0.99,
-        "n_step": 1,
         "optim_params": {
             "actor": {
                 "learning_rate": {
                     "decay_factor": 0.0,
                     "epoch_schedule": [],
-                    "initial": 0.0003
+                    "initial": 0.0001
                 },
                 "regularization": {
                     "L2": 0.0
                 }
             },
             "critic": {
                 "learning_rate": {
                     "decay_factor": 0.0,
                     "epoch_schedule": [],
-                    "initial": 0.001
+                    "initial": 0.0001
+                },
+                "regularization": {
+                    "L2": 0.0
+                }
+            },
+            "vf": {
+                "learning_rate": {
+                    "decay_factor": 0.0,
+                    "epoch_schedule": [],
+                    "initial": 0.0001
                 },
                 "regularization": {
                     "L2": 0.0
                 }
             }
         },
-        "target_tau": 0.005
+        "target_tau": 0.01,
+        "vf_quantile": 0.9
     },
-    "algo_name": "cql",
+    "algo_name": "iql",
     "experiment": {
         "additional_envs": null,
         "env": null,
         "epoch_every_n_steps": 100,
         "keep_all_videos": false,
         "logging": {
             "log_tb": true,
-            "terminal_output_to_txt": true
+            "log_wandb": false,
+            "terminal_output_to_txt": true,
+            "wandb_proj_name": "debug"
         },
         "name": "test",
         "render": false,
         "render_video": true,
         "rollout": {
             "enabled": true,
             "horizon": 400,
@@ -92,118 +104,48 @@
             "epochs": [],
             "every_n_epochs": 50,
             "every_n_seconds": null,
             "on_best_rollout_return": false,
             "on_best_rollout_success_rate": true,
             "on_best_validation": false
         },
-        "validate": true,
+        "validate": false,
         "validation_epoch_every_n_steps": 10,
         "video_skip": 5
     },
+    "meta": {
+        "hp_base_config_file": null,
+        "hp_keys": [],
+        "hp_values": []
+    },
     "observation": {
         "encoder": {
             "depth": {
                 "core_class": "VisualCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             },
             "low_dim": {
                 "core_class": null,
                 "core_kwargs": {},
-                "feature_dimension": null,
                 "obs_randomizer_class": null,
                 "obs_randomizer_kwargs": {}
             },
             "rgb": {
                 "core_class": "VisualCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             },
             "scan": {
                 "core_class": "ScanCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    },
-                    "conv_kwargs": {
-                        "kernel_size": [
-                            8,
-                            4,
-                            2
-                        ],
-                        "out_channels": [
-                            32,
-                            64,
-                            64
-                        ],
-                        "stride": [
-                            4,
-                            2,
-                            1
-                        ]
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             }
         },
         "modalities": {
             "goal": {
                 "depth": [],
                 "low_dim": [],
                 "rgb": [],
@@ -219,27 +161,32 @@
                 ],
                 "rgb": [],
                 "scan": []
             }
         }
     },
     "train": {
-        "batch_size": 1024,
+        "batch_size": 100,
         "cuda": true,
         "data": null,
         "dataset_keys": [
             "actions",
             "rewards",
             "dones"
         ],
+        "frame_stack": 1,
         "goal_mode": null,
         "hdf5_cache_mode": "all",
         "hdf5_filter_key": null,
+        "hdf5_load_next_obs": true,
         "hdf5_normalize_obs": false,
         "hdf5_use_swmr": true,
+        "hdf5_validation_filter_key": null,
         "num_data_workers": 0,
         "num_epochs": 2000,
-        "output_dir": "../cql_trained_models",
+        "output_dir": "../iql_trained_models",
+        "pad_frame_stack": true,
+        "pad_seq_length": true,
         "seed": 1,
         "seq_length": 1
     }
 }
```

### Comparing `robomimic-0.2.0/robomimic/exps/templates/gl.json` & `robomimic-0.3.0/robomimic/exps/templates/cql.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6282432510228563%*

 * *Differences: {"'algo'": "{'optim_params': {replace: OrderedDict([('critic', OrderedDict([('learning_rate', "*

 * *           "OrderedDict([('initial', 0.001), ('decay_factor', 0.0), ('epoch_schedule', [])])), "*

 * *           "('regularization', OrderedDict([('L2', 0.0)]))])), ('actor', "*

 * *           "OrderedDict([('learning_rate', OrderedDict([('initial', 0.0003), ('decay_factor', "*

 * *           "0.0), ('epoch_schedule', [])])), ('regularization', OrderedDict([('L2', 0.0)]))]))])}, "*

 * *           "'discount': 0.99, 'n_step': 1, 'tar […]*

```diff
@@ -1,73 +1,86 @@
 {
     "algo": {
-        "ae": {
-            "planner_layer_dims": [
+        "actor": {
+            "bc_start_steps": 0,
+            "layer_dims": [
                 300,
                 400
-            ]
+            ],
+            "max_gradient_norm": null,
+            "net": {
+                "common": {
+                    "low_noise_eval": true,
+                    "std_activation": "exp",
+                    "use_tanh": true
+                },
+                "gaussian": {
+                    "fixed_std": false,
+                    "init_last_fc_weight": 0.001,
+                    "init_std": 0.3
+                },
+                "type": "gaussian"
+            },
+            "target_entropy": "default"
+        },
+        "critic": {
+            "cql_weight": 1.0,
+            "deterministic_backup": true,
+            "ensemble": {
+                "n": 2
+            },
+            "layer_dims": [
+                300,
+                400
+            ],
+            "max_gradient_norm": null,
+            "min_q_weight": 1.0,
+            "num_action_samples": 1,
+            "num_random_actions": 10,
+            "target_q_gap": 5.0,
+            "use_huber": false,
+            "value_bounds": null
         },
+        "discount": 0.99,
+        "n_step": 1,
         "optim_params": {
-            "goal_network": {
+            "actor": {
                 "learning_rate": {
-                    "decay_factor": 0.1,
+                    "decay_factor": 0.0,
                     "epoch_schedule": [],
-                    "initial": 0.0001
+                    "initial": 0.0003
+                },
+                "regularization": {
+                    "L2": 0.0
+                }
+            },
+            "critic": {
+                "learning_rate": {
+                    "decay_factor": 0.0,
+                    "epoch_schedule": [],
+                    "initial": 0.001
                 },
                 "regularization": {
                     "L2": 0.0
                 }
             }
         },
-        "subgoal_horizon": 10,
-        "vae": {
-            "decoder": {
-                "is_conditioned": true,
-                "reconstruction_sum_across_elements": false
-            },
-            "decoder_layer_dims": [
-                300,
-                400
-            ],
-            "enabled": true,
-            "encoder_layer_dims": [
-                300,
-                400
-            ],
-            "kl_weight": 1.0,
-            "latent_clip": null,
-            "latent_dim": 16,
-            "prior": {
-                "categorical_dim": 10,
-                "categorical_gumbel_softmax_hard": false,
-                "categorical_init_temp": 1.0,
-                "categorical_min_temp": 0.3,
-                "categorical_temp_anneal_step": 0.001,
-                "gmm_learn_weights": false,
-                "gmm_num_modes": 10,
-                "is_conditioned": false,
-                "learn": false,
-                "use_categorical": false,
-                "use_gmm": false
-            },
-            "prior_layer_dims": [
-                300,
-                400
-            ]
-        }
+        "target_tau": 0.005
     },
-    "algo_name": "gl",
+    "algo_name": "cql",
     "experiment": {
         "additional_envs": null,
         "env": null,
         "epoch_every_n_steps": 100,
         "keep_all_videos": false,
         "logging": {
             "log_tb": true,
-            "terminal_output_to_txt": true
+            "log_wandb": false,
+            "terminal_output_to_txt": true,
+            "wandb_proj_name": "debug"
         },
         "name": "test",
         "render": false,
         "render_video": true,
         "rollout": {
             "enabled": true,
             "horizon": 400,
@@ -81,118 +94,48 @@
             "epochs": [],
             "every_n_epochs": 50,
             "every_n_seconds": null,
             "on_best_rollout_return": false,
             "on_best_rollout_success_rate": true,
             "on_best_validation": false
         },
-        "validate": true,
+        "validate": false,
         "validation_epoch_every_n_steps": 10,
         "video_skip": 5
     },
+    "meta": {
+        "hp_base_config_file": null,
+        "hp_keys": [],
+        "hp_values": []
+    },
     "observation": {
         "encoder": {
             "depth": {
                 "core_class": "VisualCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             },
             "low_dim": {
                 "core_class": null,
                 "core_kwargs": {},
-                "feature_dimension": null,
                 "obs_randomizer_class": null,
                 "obs_randomizer_kwargs": {}
             },
             "rgb": {
                 "core_class": "VisualCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             },
             "scan": {
                 "core_class": "ScanCore",
-                "core_kwargs": {
-                    "backbone_class": "ResNet18Conv",
-                    "backbone_kwargs": {
-                        "input_coord_conv": false,
-                        "pretrained": false
-                    },
-                    "conv_kwargs": {
-                        "kernel_size": [
-                            8,
-                            4,
-                            2
-                        ],
-                        "out_channels": [
-                            32,
-                            64,
-                            64
-                        ],
-                        "stride": [
-                            4,
-                            2,
-                            1
-                        ]
-                    }
-                },
-                "feature_dimension": 64,
+                "core_kwargs": {},
                 "obs_randomizer_class": null,
-                "obs_randomizer_kwargs": {
-                    "crop_height": 76,
-                    "crop_width": 76,
-                    "num_crops": 1,
-                    "pos_enc": false
-                },
-                "pool_class": "SpatialSoftmax",
-                "pool_kwargs": {
-                    "learnable_temperature": false,
-                    "noise_std": 0.0,
-                    "num_kp": 32,
-                    "temperature": 1.0
-                }
+                "obs_randomizer_kwargs": {}
             }
         },
         "modalities": {
             "goal": {
                 "depth": [],
                 "low_dim": [],
                 "rgb": [],
@@ -204,42 +147,36 @@
                     "robot0_eef_pos",
                     "robot0_eef_quat",
                     "robot0_gripper_qpos",
                     "object"
                 ],
                 "rgb": [],
                 "scan": []
-            },
-            "subgoal": {
-                "depth": [],
-                "low_dim": [
-                    "robot0_eef_pos",
-                    "robot0_eef_quat",
-                    "robot0_gripper_qpos",
-                    "object"
-                ],
-                "rgb": [],
-                "scan": []
             }
         }
     },
     "train": {
-        "batch_size": 100,
+        "batch_size": 1024,
         "cuda": true,
         "data": null,
         "dataset_keys": [
             "actions",
             "rewards",
             "dones"
         ],
+        "frame_stack": 1,
         "goal_mode": null,
         "hdf5_cache_mode": "all",
         "hdf5_filter_key": null,
+        "hdf5_load_next_obs": true,
         "hdf5_normalize_obs": false,
         "hdf5_use_swmr": true,
+        "hdf5_validation_filter_key": null,
         "num_data_workers": 0,
         "num_epochs": 2000,
-        "output_dir": "../gl_trained_models",
+        "output_dir": "../cql_trained_models",
+        "pad_frame_stack": true,
+        "pad_seq_length": true,
         "seed": 1,
         "seq_length": 1
     }
 }
```

### Comparing `robomimic-0.2.0/robomimic/exps/templates/hbc.json` & `robomimic-0.3.0/robomimic/exps/templates/iris.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.639571484801748%*

 * *Differences: {"'algo'": "{'actor': {'optim_params': {'policy': {'learning_rate': {'scheduler_type': "*

 * *           "'multistep'}, 'optimizer_type': 'adam'}}, 'transformer': OrderedDict([('enabled', "*

 * *           "False), ('context_length', 10), ('embed_dim', 512), ('num_layers', 6), ('num_heads', "*

 * *           "8), ('emb_dropout', 0.1), ('attn_dropout', 0.1), ('block_output_dropout', 0.1), "*

 * *           "('sinusoidal_embedding', False), ('activation', 'gelu'), ('supervise_all_steps', "*

 * *           "False), ('nn_parameter_for_ […]*

```diff
@@ -11,16 +11,18 @@
                 "l2_weight": 1.0
             },
             "optim_params": {
                 "policy": {
                     "learning_rate": {
                         "decay_factor": 0.1,
                         "epoch_schedule": [],
-                        "initial": 0.0001
+                        "initial": 0.0001,
+                        "scheduler_type": "multistep"
                     },
+                    "optimizer_type": "adam",
                     "regularization": {
                         "L2": 0.0
                     }
                 }
             },
             "rnn": {
                 "enabled": true,
@@ -28,92 +30,231 @@
                 "horizon": 10,
                 "kwargs": {
                     "bidirectional": false
                 },
                 "num_layers": 2,
                 "open_loop": false,
                 "rnn_type": "LSTM"
+            },
+            "transformer": {
+                "activation": "gelu",
+                "attn_dropout": 0.1,
+                "block_output_dropout": 0.1,
+                "context_length": 10,
+                "emb_dropout": 0.1,
+                "embed_dim": 512,
+                "enabled": false,
+                "nn_parameter_for_timesteps": true,
+                "num_heads": 8,
+                "num_layers": 6,
+                "sinusoidal_embedding": false,
+                "supervise_all_steps": false
             }
         },
         "actor_use_random_subgoals": false,
         "latent_subgoal": {
             "enabled": false,
             "prior_correction": {
                 "enabled": false,
                 "num_samples": 100
             }
         },
         "mode": "separate",
-        "planner": {
-            "ae": {
-                "planner_layer_dims": [
-                    300,
-                    400
-                ]
-            },
-            "optim_params": {
-                "goal_network": {
-                    "learning_rate": {
-                        "decay_factor": 0.1,
-                        "epoch_schedule": [],
-                        "initial": 0.0001
-                    },
-                    "regularization": {
-                        "L2": 0.0
+        "subgoal_update_interval": 10,
+        "value_planner": {
+            "num_samples": 100,
+            "planner": {
+                "ae": {
+                    "planner_layer_dims": [
+                        300,
+                        400
+                    ]
+                },
+                "optim_params": {
+                    "goal_network": {
+                        "learning_rate": {
+                            "decay_factor": 0.1,
+                            "epoch_schedule": [],
+                            "initial": 0.0001
+                        },
+                        "regularization": {
+                            "L2": 0.0
+                        }
                     }
+                },
+                "subgoal_horizon": 10,
+                "vae": {
+                    "decoder": {
+                        "is_conditioned": true,
+                        "reconstruction_sum_across_elements": false
+                    },
+                    "decoder_layer_dims": [
+                        300,
+                        400
+                    ],
+                    "enabled": true,
+                    "encoder_layer_dims": [
+                        300,
+                        400
+                    ],
+                    "kl_weight": 1.0,
+                    "latent_clip": null,
+                    "latent_dim": 16,
+                    "prior": {
+                        "categorical_dim": 10,
+                        "categorical_gumbel_softmax_hard": false,
+                        "categorical_init_temp": 1.0,
+                        "categorical_min_temp": 0.3,
+                        "categorical_temp_anneal_step": 0.001,
+                        "gmm_learn_weights": false,
+                        "gmm_num_modes": 10,
+                        "is_conditioned": false,
+                        "learn": false,
+                        "use_categorical": false,
+                        "use_gmm": false
+                    },
+                    "prior_layer_dims": [
+                        300,
+                        400
+                    ]
                 }
             },
-            "subgoal_horizon": 10,
-            "vae": {
-                "decoder": {
-                    "is_conditioned": true,
-                    "reconstruction_sum_across_elements": false
-                },
-                "decoder_layer_dims": [
-                    300,
-                    400
-                ],
-                "enabled": true,
-                "encoder_layer_dims": [
-                    300,
-                    400
-                ],
-                "kl_weight": 1.0,
-                "latent_clip": null,
-                "latent_dim": 16,
-                "prior": {
-                    "categorical_dim": 10,
-                    "categorical_gumbel_softmax_hard": false,
-                    "categorical_init_temp": 1.0,
-                    "categorical_min_temp": 0.3,
-                    "categorical_temp_anneal_step": 0.001,
-                    "gmm_learn_weights": false,
-                    "gmm_num_modes": 10,
-                    "is_conditioned": false,
-                    "learn": false,
-                    "use_categorical": false,
-                    "use_gmm": false
-                },
-                "prior_layer_dims": [
-                    300,
-                    400
-                ]
+            "value": {
+                "action_sampler": {
+                    "actor_layer_dims": [
+                        1024,
+                        1024
+                    ],
+                    "freeze_encoder_epoch": -1,
+                    "gmm": {
+                        "enabled": false,
+                        "low_noise_eval": true,
+                        "min_std": 0.0001,
+                        "num_modes": 5,
+                        "std_activation": "softplus"
+                    },
+                    "vae": {
+                        "decoder": {
+                            "is_conditioned": true,
+                            "reconstruction_sum_across_elements": false
+                        },
+                        "decoder_layer_dims": [
+                            300,
+                            400
+                        ],
+                        "enabled": true,
+                        "encoder_layer_dims": [
+                            300,
+                            400
+                        ],
+                        "kl_weight": 1.0,
+                        "latent_clip": null,
+                        "latent_dim": 14,
+                        "prior": {
+                            "categorical_dim": 10,
+                            "categorical_gumbel_softmax_hard": false,
+                            "categorical_init_temp": 1.0,
+                            "categorical_min_temp": 0.3,
+                            "categorical_temp_anneal_step": 0.001,
+                            "gmm_learn_weights": false,
+                            "gmm_num_modes": 10,
+                            "is_conditioned": false,
+                            "learn": false,
+                            "use_categorical": false,
+                            "use_gmm": false
+                        },
+                        "prior_layer_dims": [
+                            300,
+                            400
+                        ]
+                    }
+                },
+                "actor": {
+                    "enabled": false,
+                    "layer_dims": [
+                        300,
+                        400
+                    ],
+                    "perturbation_scale": 0.05
+                },
+                "critic": {
+                    "distributional": {
+                        "enabled": false,
+                        "num_atoms": 51
+                    },
+                    "ensemble": {
+                        "n": 2,
+                        "weight": 0.75
+                    },
+                    "layer_dims": [
+                        300,
+                        400
+                    ],
+                    "max_gradient_norm": null,
+                    "num_action_samples": 10,
+                    "num_action_samples_rollout": 100,
+                    "use_huber": false,
+                    "value_bounds": null
+                },
+                "discount": 0.99,
+                "infinite_horizon": false,
+                "n_step": 1,
+                "optim_params": {
+                    "action_sampler": {
+                        "end_epoch": -1,
+                        "learning_rate": {
+                            "decay_factor": 0.1,
+                            "epoch_schedule": [],
+                            "initial": 0.001
+                        },
+                        "regularization": {
+                            "L2": 0.0
+                        },
+                        "start_epoch": -1
+                    },
+                    "actor": {
+                        "end_epoch": -1,
+                        "learning_rate": {
+                            "decay_factor": 0.1,
+                            "epoch_schedule": [],
+                            "initial": 0.001
+                        },
+                        "regularization": {
+                            "L2": 0.0
+                        },
+                        "start_epoch": -1
+                    },
+                    "critic": {
+                        "end_epoch": -1,
+                        "learning_rate": {
+                            "decay_factor": 0.1,
+                            "epoch_schedule": [],
+                            "initial": 0.001
+                        },
+                        "regularization": {
+                            "L2": 0.0
+                        },
+                        "start_epoch": -1
+                    }
+                },
+                "target_tau": 0.005
             }
-        },
-        "subgoal_update_interval": 10
+        }
     },
-    "algo_name": "hbc",
+    "algo_name": "iris",
     "experiment": {
         "additional_envs": null,
         "env": null,
         "epoch_every_n_steps": 100,
         "keep_all_videos": false,
         "logging": {
             "log_tb": true,
-            "terminal_output_to_txt": true
+            "log_wandb": false,
+            "terminal_output_to_txt": true,
+            "wandb_proj_name": "debug"
         },
         "name": "test",
         "render": false,
         "render_video": true,
         "rollout": {
             "enabled": true,
             "horizon": 400,
@@ -127,119 +268,49 @@
             "epochs": [],
             "every_n_epochs": 50,
             "every_n_seconds": null,
             "on_best_rollout_return": false,
             "on_best_rollout_success_rate": true,
             "on_best_validation": false
         },
-        "validate": true,
+        "validate": false,
         "validation_epoch_every_n_steps": 10,
         "video_skip": 5
     },
+    "meta": {
+        "hp_base_config_file": null,
+        "hp_keys": [],
+        "hp_values": []
+    },
     "observation": {
         "actor": {
             "encoder": {
                 "depth": {
                     "core_class": "VisualCore",
-                    "core_kwargs": {
-                        "backbone_class": "ResNet18Conv",
-                        "backbone_kwargs": {
-                            "input_coord_conv": false,
-                            "pretrained": false
-                        }
-                    },
-                    "feature_dimension": 64,
+                    "core_kwargs": {},
                     "obs_randomizer_class": null,
-                    "obs_randomizer_kwargs": {
-                        "crop_height": 76,
-                        "crop_width": 76,
-                        "num_crops": 1,
-                        "pos_enc": false
-                    },
-                    "pool_class": "SpatialSoftmax",
-                    "pool_kwargs": {
-                        "learnable_temperature": false,
-                        "noise_std": 0.0,
-                        "num_kp": 32,
-                        "temperature": 1.0
-                    }
+                    "obs_randomizer_kwargs": {}
                 },
                 "low_dim": {
                     "core_class": null,
                     "core_kwargs": {},
-                    "feature_dimension": null,
                     "obs_randomizer_class": null,
                     "obs_randomizer_kwargs": {}
                 },
                 "rgb": {
                     "core_class": "VisualCore",
-                    "core_kwargs": {
-                        "backbone_class": "ResNet18Conv",
-                        "backbone_kwargs": {
-                            "input_coord_conv": false,
-                            "pretrained": false
-                        }
-                    },
-                    "feature_dimension": 64,
+                    "core_kwargs": {},
                     "obs_randomizer_class": null,
-                    "obs_randomizer_kwargs": {
-                        "crop_height": 76,
-                        "crop_width": 76,
-                        "num_crops": 1,
-                        "pos_enc": false
-                    },
-                    "pool_class": "SpatialSoftmax",
-                    "pool_kwargs": {
-                        "learnable_temperature": false,
-                        "noise_std": 0.0,
-                        "num_kp": 32,
-                        "temperature": 1.0
-                    }
+                    "obs_randomizer_kwargs": {}
                 },
                 "scan": {
                     "core_class": "ScanCore",
-                    "core_kwargs": {
-                        "backbone_class": "ResNet18Conv",
-                        "backbone_kwargs": {
-                            "input_coord_conv": false,
-                            "pretrained": false
-                        },
-                        "conv_kwargs": {
-                            "kernel_size": [
-                                8,
-                                4,
-                                2
-                            ],
-                            "out_channels": [
-                                32,
-                                64,
-                                64
-                            ],
-                            "stride": [
-                                4,
-                                2,
-                                1
-                            ]
-                        }
-                    },
-                    "feature_dimension": 64,
+                    "core_kwargs": {},
                     "obs_randomizer_class": null,
-                    "obs_randomizer_kwargs": {
-                        "crop_height": 76,
-                        "crop_width": 76,
-                        "num_crops": 1,
-                        "pos_enc": false
-                    },
-                    "pool_class": "SpatialSoftmax",
-                    "pool_kwargs": {
-                        "learnable_temperature": false,
-                        "noise_std": 0.0,
-                        "num_kp": 32,
-                        "temperature": 1.0
-                    }
+                    "obs_randomizer_kwargs": {}
                 }
             },
             "modalities": {
                 "goal": {
                     "depth": [],
                     "low_dim": [],
                     "rgb": [],
@@ -254,162 +325,141 @@
                         "object"
                     ],
                     "rgb": [],
                     "scan": []
                 }
             }
         },
-        "planner": {
-            "encoder": {
-                "depth": {
-                    "core_class": "VisualCore",
-                    "core_kwargs": {
-                        "backbone_class": "ResNet18Conv",
-                        "backbone_kwargs": {
-                            "input_coord_conv": false,
-                            "pretrained": false
-                        }
-                    },
-                    "feature_dimension": 64,
-                    "obs_randomizer_class": null,
-                    "obs_randomizer_kwargs": {
-                        "crop_height": 76,
-                        "crop_width": 76,
-                        "num_crops": 1,
-                        "pos_enc": false
-                    },
-                    "pool_class": "SpatialSoftmax",
-                    "pool_kwargs": {
-                        "learnable_temperature": false,
-                        "noise_std": 0.0,
-                        "num_kp": 32,
-                        "temperature": 1.0
+        "value_planner": {
+            "planner": {
+                "encoder": {
+                    "depth": {
+                        "core_class": "VisualCore",
+                        "core_kwargs": {},
+                        "obs_randomizer_class": null,
+                        "obs_randomizer_kwargs": {}
+                    },
+                    "low_dim": {
+                        "core_class": null,
+                        "core_kwargs": {},
+                        "obs_randomizer_class": null,
+                        "obs_randomizer_kwargs": {}
+                    },
+                    "rgb": {
+                        "core_class": "VisualCore",
+                        "core_kwargs": {},
+                        "obs_randomizer_class": null,
+                        "obs_randomizer_kwargs": {}
+                    },
+                    "scan": {
+                        "core_class": "ScanCore",
+                        "core_kwargs": {},
+                        "obs_randomizer_class": null,
+                        "obs_randomizer_kwargs": {}
                     }
                 },
-                "low_dim": {
-                    "core_class": null,
-                    "core_kwargs": {},
-                    "feature_dimension": null,
-                    "obs_randomizer_class": null,
-                    "obs_randomizer_kwargs": {}
-                },
-                "rgb": {
-                    "core_class": "VisualCore",
-                    "core_kwargs": {
-                        "backbone_class": "ResNet18Conv",
-                        "backbone_kwargs": {
-                            "input_coord_conv": false,
-                            "pretrained": false
-                        }
-                    },
-                    "feature_dimension": 64,
-                    "obs_randomizer_class": null,
-                    "obs_randomizer_kwargs": {
-                        "crop_height": 76,
-                        "crop_width": 76,
-                        "num_crops": 1,
-                        "pos_enc": false
-                    },
-                    "pool_class": "SpatialSoftmax",
-                    "pool_kwargs": {
-                        "learnable_temperature": false,
-                        "noise_std": 0.0,
-                        "num_kp": 32,
-                        "temperature": 1.0
-                    }
-                },
-                "scan": {
-                    "core_class": "ScanCore",
-                    "core_kwargs": {
-                        "backbone_class": "ResNet18Conv",
-                        "backbone_kwargs": {
-                            "input_coord_conv": false,
-                            "pretrained": false
-                        },
-                        "conv_kwargs": {
-                            "kernel_size": [
-                                8,
-                                4,
-                                2
-                            ],
-                            "out_channels": [
-                                32,
-                                64,
-                                64
-                            ],
-                            "stride": [
-                                4,
-                                2,
-                                1
-                            ]
-                        }
-                    },
-                    "feature_dimension": 64,
-                    "obs_randomizer_class": null,
-                    "obs_randomizer_kwargs": {
-                        "crop_height": 76,
-                        "crop_width": 76,
-                        "num_crops": 1,
-                        "pos_enc": false
-                    },
-                    "pool_class": "SpatialSoftmax",
-                    "pool_kwargs": {
-                        "learnable_temperature": false,
-                        "noise_std": 0.0,
-                        "num_kp": 32,
-                        "temperature": 1.0
+                "modalities": {
+                    "goal": {
+                        "depth": [],
+                        "low_dim": [],
+                        "rgb": [],
+                        "scan": []
+                    },
+                    "obs": {
+                        "depth": [],
+                        "low_dim": [
+                            "robot0_eef_pos",
+                            "robot0_eef_quat",
+                            "robot0_gripper_qpos",
+                            "object"
+                        ],
+                        "rgb": [],
+                        "scan": []
+                    },
+                    "subgoal": {
+                        "depth": [],
+                        "low_dim": [
+                            "robot0_eef_pos",
+                            "robot0_eef_quat",
+                            "robot0_gripper_qpos",
+                            "object"
+                        ],
+                        "rgb": [],
+                        "scan": []
                     }
                 }
             },
-            "modalities": {
-                "goal": {
-                    "depth": [],
-                    "low_dim": [],
-                    "rgb": [],
-                    "scan": []
-                },
-                "obs": {
-                    "depth": [],
-                    "low_dim": [
-                        "robot0_eef_pos",
-                        "robot0_eef_quat",
-                        "robot0_gripper_qpos",
-                        "object"
-                    ],
-                    "rgb": [],
-                    "scan": []
+            "value": {
+                "encoder": {
+                    "depth": {
+                        "core_class": "VisualCore",
+                        "core_kwargs": {},
+                        "obs_randomizer_class": null,
+                        "obs_randomizer_kwargs": {}
+                    },
+                    "low_dim": {
+                        "core_class": null,
+                        "core_kwargs": {},
+                        "obs_randomizer_class": null,
+                        "obs_randomizer_kwargs": {}
+                    },
+                    "rgb": {
+                        "core_class": "VisualCore",
+                        "core_kwargs": {},
+                        "obs_randomizer_class": null,
+                        "obs_randomizer_kwargs": {}
+                    },
+                    "scan": {
+                        "core_class": "ScanCore",
+                        "core_kwargs": {},
+                        "obs_randomizer_class": null,
+                        "obs_randomizer_kwargs": {}
+                    }
                 },
-                "subgoal": {
-                    "depth": [],
-                    "low_dim": [
-                        "robot0_eef_pos",
-                        "robot0_eef_quat",
-                        "robot0_gripper_qpos",
-                        "object"
-                    ],
-                    "rgb": [],
-                    "scan": []
+                "modalities": {
+                    "goal": {
+                        "depth": [],
+                        "low_dim": [],
+                        "rgb": [],
+                        "scan": []
+                    },
+                    "obs": {
+                        "depth": [],
+                        "low_dim": [
+                            "robot0_eef_pos",
+                            "robot0_eef_quat",
+                            "robot0_gripper_qpos",
+                            "object"
+                        ],
+                        "rgb": [],
+                        "scan": []
+                    }
                 }
             }
         }
     },
     "train": {
         "batch_size": 100,
         "cuda": true,
         "data": null,
         "dataset_keys": [
             "actions",
             "rewards",
             "dones"
         ],
+        "frame_stack": 1,
         "goal_mode": null,
         "hdf5_cache_mode": "all",
         "hdf5_filter_key": null,
+        "hdf5_load_next_obs": true,
         "hdf5_normalize_obs": false,
         "hdf5_use_swmr": true,
+        "hdf5_validation_filter_key": null,
         "num_data_workers": 0,
         "num_epochs": 2000,
-        "output_dir": "../hbc_trained_models",
+        "output_dir": "../iris_trained_models",
+        "pad_frame_stack": true,
+        "pad_seq_length": true,
         "seed": 1,
         "seq_length": 10
     }
 }
```

### Comparing `robomimic-0.2.0/robomimic/models/base_nets.py` & `robomimic-0.3.0/robomimic/models/base_nets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
 Contains torch Modules that correspond to basic network building blocks, like 
 MLP, RNN, and CNN backbones.
 """
 
-import sys
 import math
 import abc
 import numpy as np
 import textwrap
-from copy import deepcopy
 from collections import OrderedDict
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+from torchvision import transforms
 from torchvision import models as vision_models
 
 import robomimic.utils.tensor_utils as TensorUtils
-import robomimic.utils.obs_utils as ObsUtils
-from robomimic.utils.python_utils import extract_class_init_kwargs_from_dict
 
 
 CONV_ACTIVATIONS = {
     "relu": nn.ReLU,
     "None": None,
     None: None,
 }
@@ -38,14 +35,38 @@
         rnn_hidden_dim=rnn_config.hidden_dim,
         rnn_num_layers=rnn_config.num_layers,
         rnn_type=rnn_config.rnn_type,
         rnn_kwargs=dict(rnn_config.kwargs),
     )
 
 
+def transformer_args_from_config(transformer_config):
+    """
+    Takes a Config object corresponding to Transformer settings
+    (for example `config.algo.transformer` in BCConfig) and extracts
+    transformer kwargs for instantiating transformer networks.
+    """
+    transformer_args = dict(
+        transformer_context_length=transformer_config.context_length,
+        transformer_embed_dim=transformer_config.embed_dim,
+        transformer_num_heads=transformer_config.num_heads,
+        transformer_emb_dropout=transformer_config.emb_dropout,
+        transformer_attn_dropout=transformer_config.attn_dropout,
+        transformer_block_output_dropout=transformer_config.block_output_dropout,
+        transformer_sinusoidal_embedding=transformer_config.sinusoidal_embedding,
+        transformer_activation=transformer_config.activation,
+        transformer_nn_parameter_for_timesteps=transformer_config.nn_parameter_for_timesteps,
+    )
+    
+    if "num_layers" in transformer_config:
+        transformer_args["transformer_num_layers"] = transformer_config.num_layers
+
+    return transformer_args
+
+
 class Module(torch.nn.Module):
     """
     Base class for networks. The only difference from torch.nn.Module is that it
     requires implementing @output_shape.
     """
     @abc.abstractmethod
     def output_shape(self, input_shape=None):
@@ -63,36 +84,57 @@
         raise NotImplementedError
 
 
 class Sequential(torch.nn.Sequential, Module):
     """
     Compose multiple Modules together (defined above).
     """
-    def __init__(self, *args):
+    def __init__(self, *args, has_output_shape = True):
+        """
+        Args:
+            has_output_shape (bool, optional): indicates whether output_shape can be called on the Sequential module.
+                torch.nn modules do not have an output_shape, but Modules (defined above) do. Defaults to True.
+        """
         for arg in args:
-            assert isinstance(arg, Module)
+            if has_output_shape:
+                assert isinstance(arg, Module)
+            else:
+                assert isinstance(arg, nn.Module)
         torch.nn.Sequential.__init__(self, *args)
+        self.fixed = False
+        self.has_output_shape = has_output_shape
 
     def output_shape(self, input_shape=None):
         """
         Function to compute output shape from inputs to this module. 
 
         Args:
             input_shape (iterable of int): shape of input. Does not include batch dimension.
                 Some modules may not need this argument, if their output does not depend 
                 on the size of the input, or if they assume fixed size input.
 
         Returns:
             out_shape ([int]): list of integers corresponding to output shape
         """
+        if not self.has_output_shape:
+            raise NotImplementedError("Output shape is not defined for this module")
         out_shape = input_shape
         for module in self:
             out_shape = module.output_shape(out_shape)
         return out_shape
 
+    def freeze(self):
+        self.fixed = True
+
+    def train(self, mode):
+        if self.fixed:
+            super().train(False)
+        else:
+            super().train(mode)
+
 
 class Parameter(Module):
     """
     A class that is a thin wrapper around a torch.nn.Parameter to make for easy saving
     and optimization.
     """
     def __init__(self, init_tensor):
@@ -496,14 +538,174 @@
 
     def __repr__(self):
         """Pretty print network."""
         header = '{}'.format(str(self.__class__.__name__))
         return header + '(input_channel={}, input_coord_conv={})'.format(self._input_channel, self._input_coord_conv)
 
 
+class R3MConv(ConvBase):
+    """
+    Base class for ConvNets pretrained with R3M (https://arxiv.org/abs/2203.12601)
+    """
+    def __init__(
+        self,
+        input_channel=3,
+        r3m_model_class='resnet18',
+        freeze=True,
+    ):
+        """
+        Using R3M pretrained observation encoder network proposed by https://arxiv.org/abs/2203.12601
+        Args:
+            input_channel (int): number of input channels for input images to the network.
+                If not equal to 3, modifies first conv layer in ResNet to handle the number
+                of input channels.
+            r3m_model_class (str): select one of the r3m pretrained model "resnet18", "resnet34" or "resnet50"
+            freeze (bool): if True, use a frozen R3M pretrained model.
+        """
+        super(R3MConv, self).__init__()
+
+        try:
+            from r3m import load_r3m
+        except ImportError:
+            print("WARNING: could not load r3m library! Please follow https://github.com/facebookresearch/r3m to install R3M")
+
+        net = load_r3m(r3m_model_class)
+
+        assert input_channel == 3 # R3M only support input image with channel size 3
+        assert r3m_model_class in ["resnet18", "resnet34", "resnet50"] # make sure the selected r3m model do exist
+
+        # cut the last fc layer
+        self._input_channel = input_channel
+        self._r3m_model_class = r3m_model_class
+        self._freeze = freeze
+        self._input_coord_conv = False
+        self._pretrained = True
+
+        preprocess = nn.Sequential(
+            transforms.Resize(256),
+            transforms.CenterCrop(224),
+            transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+        )
+        self.nets = Sequential(*([preprocess] + list(net.module.convnet.children())), has_output_shape = False)
+        if freeze:
+            self.nets.freeze()
+
+        self.weight_sum = np.sum([param.cpu().data.numpy().sum() for param in self.nets.parameters()])
+        if freeze:
+            for param in self.nets.parameters():
+                param.requires_grad = False
+
+        self.nets.eval()
+
+    def output_shape(self, input_shape):
+        """
+        Function to compute output shape from inputs to this module.
+        Args:
+            input_shape (iterable of int): shape of input. Does not include batch dimension.
+                Some modules may not need this argument, if their output does not depend
+                on the size of the input, or if they assume fixed size input.
+        Returns:
+            out_shape ([int]): list of integers corresponding to output shape
+        """
+        assert(len(input_shape) == 3)
+
+        if self._r3m_model_class == 'resnet50':
+            out_dim = 2048
+        else:
+            out_dim = 512
+
+        return [out_dim, 1, 1]
+
+    def __repr__(self):
+        """Pretty print network."""
+        header = '{}'.format(str(self.__class__.__name__))
+        return header + '(input_channel={}, input_coord_conv={}, pretrained={}, freeze={})'.format(self._input_channel, self._input_coord_conv, self._pretrained, self._freeze)
+
+
+class MVPConv(ConvBase):
+    """
+    Base class for ConvNets pretrained with MVP (https://arxiv.org/abs/2203.06173)
+    """
+    def __init__(
+        self,
+        input_channel=3,
+        mvp_model_class='vitb-mae-egosoup',
+        freeze=True,
+    ):
+        """
+        Using MVP pretrained observation encoder network proposed by https://arxiv.org/abs/2203.06173
+        Args:
+            input_channel (int): number of input channels for input images to the network.
+                If not equal to 3, modifies first conv layer in ResNet to handle the number
+                of input channels.
+            mvp_model_class (str): select one of the mvp pretrained model "vits-mae-hoi", "vits-mae-in", "vits-sup-in", "vitb-mae-egosoup" or "vitl-256-mae-egosoup"
+            freeze (bool): if True, use a frozen MVP pretrained model.
+        """
+        super(MVPConv, self).__init__()
+
+        try:
+            import mvp
+        except ImportError:
+            print("WARNING: could not load mvp library! Please follow https://github.com/ir413/mvp to install MVP.")
+
+        self.nets = mvp.load(mvp_model_class)
+        if freeze:
+            self.nets.freeze()
+
+        assert input_channel == 3 # MVP only support input image with channel size 3
+        assert mvp_model_class in ["vits-mae-hoi", "vits-mae-in", "vits-sup-in", "vitb-mae-egosoup", "vitl-256-mae-egosoup"] # make sure the selected r3m model do exist
+
+        self._input_channel = input_channel
+        self._freeze = freeze
+        self._mvp_model_class = mvp_model_class
+        self._input_coord_conv = False
+        self._pretrained = True
+
+        if '256' in mvp_model_class:
+            input_img_size = 256
+        else:
+            input_img_size = 224
+        self.preprocess = nn.Sequential(
+            transforms.Resize(input_img_size)
+        )
+
+    def forward(self, inputs):
+        x = self.preprocess(inputs)
+        x = self.nets(x)
+        if list(self.output_shape(list(inputs.shape)[1:])) != list(x.shape)[1:]:
+            raise ValueError('Size mismatch: expect size %s, but got size %s' % (
+                str(self.output_shape(list(inputs.shape)[1:])), str(list(x.shape)[1:]))
+            )
+        return x
+
+    def output_shape(self, input_shape):
+        """
+        Function to compute output shape from inputs to this module.
+        Args:
+            input_shape (iterable of int): shape of input. Does not include batch dimension.
+                Some modules may not need this argument, if their output does not depend
+                on the size of the input, or if they assume fixed size input.
+        Returns:
+            out_shape ([int]): list of integers corresponding to output shape
+        """
+        assert(len(input_shape) == 3)
+        if 'vitb' in self._mvp_model_class:
+            output_shape = [768]
+        elif 'vitl' in self._mvp_model_class:
+            output_shape = [1024]
+        else:
+            output_shape = [384]
+        return output_shape
+
+    def __repr__(self):
+        """Pretty print network."""
+        header = '{}'.format(str(self.__class__.__name__))
+        return header + '(input_channel={}, input_coord_conv={}, pretrained={}, freeze={})'.format(self._input_channel, self._input_coord_conv, self._pretrained, self._freeze)
+
+
 class CoordConv2d(nn.Conv2d, Module):
     """
     2D Coordinate Convolution
 
     Source: An Intriguing Failing of Convolutional Neural Networks and the CoordConv Solution
     https://arxiv.org/abs/1807.03247
     (e.g. adds 2 channels per input feature map corresponding to (x, y) location on map)
@@ -625,40 +827,37 @@
     """
     Base class for stacked Conv1d layers.
 
     Args:
         input_channel (int): Number of channels for inputs to this network
         activation (None or str): Per-layer activation to use. Defaults to "relu". Valid options are
             currently {relu, None} for no activation
-        conv_kwargs (dict): Specific nn.Conv1D args to use, in list form, where the ith element corresponds to the
+        out_channels (list of int): Output channel size for each sequential Conv1d layer
+        kernel_size (list of int): Kernel sizes for each sequential Conv1d layer
+        stride (list of int): Stride sizes for each sequential Conv1d layer
+        conv_kwargs (dict): additional nn.Conv1D args to use, in list form, where the ith element corresponds to the
             argument to be passed to the ith Conv1D layer.
             See https://pytorch.org/docs/stable/generated/torch.nn.Conv1d.html for specific possible arguments.
-
-            e.g.: common values to use:
-                out_channels (list of int): Output channel size for each sequential Conv1d layer
-                kernel_size (list of int): Kernel sizes for each sequential Conv1d layer
-                stride (list of int): Stride sizes for each sequential Conv1d layer
     """
     def __init__(
         self,
         input_channel=1,
         activation="relu",
+        out_channels=(32, 64, 64),
+        kernel_size=(8, 4, 2),
+        stride=(4, 2, 1),
         **conv_kwargs,
     ):
         super(Conv1dBase, self).__init__()
 
         # Get activation requested
         activation = CONV_ACTIVATIONS[activation]
 
-        # Make sure out_channels and kernel_size are specified
-        for kwarg in ("out_channels", "kernel_size"):
-            assert kwarg in conv_kwargs, f"{kwarg} must be specified in Conv1dBase kwargs!"
-
         # Generate network
-        self.n_layers = len(conv_kwargs["out_channels"])
+        self.n_layers = len(out_channels)
         layers = OrderedDict()
         for i in range(self.n_layers):
             layer_kwargs = {k: v[i] for k, v in conv_kwargs.items()}
             layers[f'conv{i}'] = nn.Conv1d(
                 in_channels=input_channel,
                 **layer_kwargs,
             )
@@ -708,24 +907,24 @@
 
     Based on Deep Spatial Autoencoders for Visuomotor Learning by Finn et al.
     https://rll.berkeley.edu/dsae/dsae.pdf
     """
     def __init__(
         self,
         input_shape,
-        num_kp=None,
+        num_kp=32,
         temperature=1.,
         learnable_temperature=False,
         output_variance=False,
         noise_std=0.0,
     ):
         """
         Args:
             input_shape (list): shape of the input feature (C, H, W)
-            num_kp (int): number of keypoints (None for not use spatialsoftmax)
+            num_kp (int): number of keypoints (None for not using spatialsoftmax)
             temperature (float): temperature term for the softmax.
             learnable_temperature (bool): whether to learn the temperature
             output_variance (bool): treat attention as a distribution, and compute second-order statistics to return
             noise_std (float): add random spatial noise to the predicted keypoints
         """
         super(SpatialSoftmax, self).__init__()
         assert len(input_shape) == 3
@@ -906,478 +1105,7 @@
         if self.agg_type == "avg":
             # mean-pooling
             return torch.mean(x, dim=1)
         if self.agg_type == "w_avg":
             # weighted mean-pooling
             return torch.sum(x * self.agg_weight, dim=1)
         raise Exception("unexpected agg type: {}".forward(self.agg_type))
-
-
-"""
-================================================
-Encoder Core Networks (Abstract class)
-================================================
-"""
-class EncoderCore(Module):
-    """
-    Abstract class used to categorize all cores used to encode observations
-    """
-    def __init__(self, input_shape):
-        self.input_shape = input_shape
-        super(EncoderCore, self).__init__()
-
-    def __init_subclass__(cls, **kwargs):
-        """
-        Hook method to automatically register all valid subclasses so we can keep track of valid observation encoders
-        in a global dict.
-
-        This global dict stores mapping from observation encoder network name to class.
-        We keep track of these registries to enable automated class inference at runtime, allowing
-        users to simply extend our base encoder class and refer to that class in string form
-        in their config, without having to manually register their class internally.
-        This also future-proofs us for any additional encoder classes we would
-        like to add ourselves.
-        """
-        ObsUtils.register_encoder_core(cls)
-
-
-"""
-================================================
-Visual Core Networks (Backbone + Pool)
-================================================
-"""
-class VisualCore(EncoderCore, ConvBase):
-    """
-    A network block that combines a visual backbone network with optional pooling
-    and linear layers.
-    """
-    def __init__(
-        self,
-        input_shape,
-        backbone_class,
-        backbone_kwargs,
-        pool_class=None,
-        pool_kwargs=None,
-        flatten=True,
-        feature_dimension=None,
-    ):
-        """
-        Args:
-            input_shape (tuple): shape of input (not including batch dimension)
-            backbone_class (str): class name for the visual backbone network (e.g.: ResNet18)
-            backbone_kwargs (dict): kwargs for the visual backbone network
-            pool_class (str): class name for the visual feature pooler (optional)
-                Common options are "SpatialSoftmax" and "SpatialMeanPool"
-            pool_kwargs (dict): kwargs for the visual feature pooler (optional)
-            flatten (bool): whether to flatten the visual feature
-            feature_dimension (int): if not None, add a Linear layer to
-                project output into a desired feature dimension
-        """
-        super(VisualCore, self).__init__(input_shape=input_shape)
-        self.flatten = flatten
-
-        # add input channel dimension to visual core inputs
-        backbone_kwargs["input_channel"] = input_shape[0]
-
-        # extract only relevant kwargs for this specific backbone
-        backbone_kwargs = extract_class_init_kwargs_from_dict(cls=eval(backbone_class), dic=backbone_kwargs, copy=True)
-
-        # visual backbone
-        assert isinstance(backbone_class, str)
-        self.backbone = eval(backbone_class)(**backbone_kwargs)
-
-        assert isinstance(self.backbone, ConvBase)
-
-        feat_shape = self.backbone.output_shape(input_shape)
-        net_list = [self.backbone]
-
-        # maybe make pool net
-        if pool_class is not None:
-            assert isinstance(pool_class, str)
-            # feed output shape of backbone to pool net
-            if pool_kwargs is None:
-                pool_kwargs = dict()
-            # extract only relevant kwargs for this specific backbone
-            pool_kwargs["input_shape"] = feat_shape
-            pool_kwargs = extract_class_init_kwargs_from_dict(cls=eval(pool_class), dic=pool_kwargs, copy=True)
-            self.pool = eval(pool_class)(**pool_kwargs)
-            assert isinstance(self.pool, Module)
-
-            feat_shape = self.pool.output_shape(feat_shape)
-            net_list.append(self.pool)
-        else:
-            self.pool = None
-
-        # flatten layer
-        if self.flatten:
-            net_list.append(torch.nn.Flatten(start_dim=1, end_dim=-1))
-
-        # maybe linear layer
-        self.feature_dimension = feature_dimension
-        if feature_dimension is not None:
-            assert self.flatten
-            linear = torch.nn.Linear(int(np.prod(feat_shape)), feature_dimension)
-            net_list.append(linear)
-
-        self.nets = nn.Sequential(*net_list)
-
-    def output_shape(self, input_shape):
-        """
-        Function to compute output shape from inputs to this module. 
-
-        Args:
-            input_shape (iterable of int): shape of input. Does not include batch dimension.
-                Some modules may not need this argument, if their output does not depend 
-                on the size of the input, or if they assume fixed size input.
-
-        Returns:
-            out_shape ([int]): list of integers corresponding to output shape
-        """
-        if self.feature_dimension is not None:
-            # linear output
-            return [self.feature_dimension]
-        feat_shape = self.backbone.output_shape(input_shape)
-        if self.pool is not None:
-            # pool output
-            feat_shape = self.pool.output_shape(feat_shape)
-        # backbone + flat output
-        if self.flatten:
-            return [np.prod(feat_shape)]
-        else:
-            return feat_shape
-
-    def forward(self, inputs):
-        """
-        Forward pass through visual core.
-        """
-        ndim = len(self.input_shape)
-        assert tuple(inputs.shape)[-ndim:] == tuple(self.input_shape)
-        return super(VisualCore, self).forward(inputs)
-
-    def __repr__(self):
-        """Pretty print network."""
-        header = '{}'.format(str(self.__class__.__name__))
-        msg = ''
-        indent = ' ' * 2
-        msg += textwrap.indent(
-            "\ninput_shape={}\noutput_shape={}".format(self.input_shape, self.output_shape(self.input_shape)), indent)
-        msg += textwrap.indent("\nbackbone_net={}".format(self.backbone), indent)
-        msg += textwrap.indent("\npool_net={}".format(self.pool), indent)
-        msg = header + '(' + msg + '\n)'
-        return msg
-
-
-"""
-================================================
-Scan Core Networks (Conv1D Sequential + Pool)
-================================================
-"""
-class ScanCore(EncoderCore, ConvBase):
-    """
-    A network block that combines a Conv1D backbone network with optional pooling
-    and linear layers.
-    """
-    def __init__(
-        self,
-        input_shape,
-        conv_kwargs,
-        conv_activation="relu",
-        pool_class=None,
-        pool_kwargs=None,
-        flatten=True,
-        feature_dimension=None,
-    ):
-        """
-        Args:
-            input_shape (tuple): shape of input (not including batch dimension)
-            conv_kwargs (dict): kwargs for the conv1d backbone network. Should contain lists for the following values:
-                out_channels (int)
-                kernel_size (int)
-                stride (int)
-                ...
-            conv_activation (str or None): Activation to use between conv layers. Default is relu.
-                Currently, valid options are {relu}
-            pool_class (str): class name for the visual feature pooler (optional)
-                Common options are "SpatialSoftmax" and "SpatialMeanPool"
-            pool_kwargs (dict): kwargs for the visual feature pooler (optional)
-            flatten (bool): whether to flatten the network output
-            feature_dimension (int): if not None, add a Linear layer to
-                project output into a desired feature dimension (note: flatten must be set to True!)
-        """
-        super(ScanCore, self).__init__(input_shape=input_shape)
-        self.flatten = flatten
-        self.feature_dimension = feature_dimension
-
-        # Generate backbone network
-        self.backbone = Conv1dBase(
-            input_channel=1,
-            activation=conv_activation,
-            **conv_kwargs,
-        )
-        feat_shape = self.backbone.output_shape(input_shape=input_shape)
-
-        # Create netlist of all generated networks
-        net_list = [self.backbone]
-
-        # Possibly add pooling network
-        if pool_class is not None:
-            # Add an unsqueeze network so that the shape is correct to pass to pooling network
-            self.unsqueeze = Unsqueeze(dim=-1)
-            net_list.append(self.unsqueeze)
-            # Get output shape
-            feat_shape = self.unsqueeze.output_shape(feat_shape)
-            # Create pooling network
-            self.pool = eval(pool_class)(input_shape=feat_shape, **pool_kwargs)
-            net_list.append(self.pool)
-            feat_shape = self.pool.output_shape(feat_shape)
-        else:
-            self.unsqueeze, self.pool = None, None
-
-        # flatten layer
-        if self.flatten:
-            net_list.append(torch.nn.Flatten(start_dim=1, end_dim=-1))
-
-        # maybe linear layer
-        if self.feature_dimension is not None:
-            assert self.flatten
-            linear = torch.nn.Linear(int(np.prod(feat_shape)), self.feature_dimension)
-            net_list.append(linear)
-
-        # Generate final network
-        self.nets = nn.Sequential(*net_list)
-
-    def output_shape(self, input_shape):
-        """
-        Function to compute output shape from inputs to this module.
-
-        Args:
-            input_shape (iterable of int): shape of input. Does not include batch dimension.
-                Some modules may not need this argument, if their output does not depend
-                on the size of the input, or if they assume fixed size input.
-
-        Returns:
-            out_shape ([int]): list of integers corresponding to output shape
-        """
-        if self.feature_dimension is not None:
-            # linear output
-            return [self.feature_dimension]
-        feat_shape = self.backbone.output_shape(input_shape)
-        if self.pool is not None:
-            # pool output
-            feat_shape = self.pool.output_shape(self.unsqueeze.output_shape(feat_shape))
-        # backbone + flat output
-        return [np.prod(feat_shape)] if self.flatten else feat_shape
-
-    def forward(self, inputs):
-        """
-        Forward pass through visual core.
-        """
-        ndim = len(self.input_shape)
-        assert tuple(inputs.shape)[-ndim:] == tuple(self.input_shape)
-        return super(ScanCore, self).forward(inputs)
-
-    def __repr__(self):
-        """Pretty print network."""
-        header = '{}'.format(str(self.__class__.__name__))
-        msg = ''
-        indent = ' ' * 2
-        msg += textwrap.indent(
-            "\ninput_shape={}\noutput_shape={}".format(self.input_shape, self.output_shape(self.input_shape)), indent)
-        msg += textwrap.indent("\nbackbone_net={}".format(self.backbone), indent)
-        msg += textwrap.indent("\npool_net={}".format(self.pool), indent)
-        msg = header + '(' + msg + '\n)'
-        return msg
-
-
-
-"""
-================================================
-Observation Randomizer Networks
-================================================
-"""
-class Randomizer(Module):
-    """
-    Base class for randomizer networks. Each randomizer should implement the @output_shape_in,
-    @output_shape_out, @forward_in, and @forward_out methods. The randomizer's @forward_in
-    method is invoked on raw inputs, and @forward_out is invoked on processed inputs
-    (usually processed by a @VisualCore instance). Note that the self.training property
-    can be used to change the randomizer's behavior at train vs. test time.
-    """
-    def __init__(self):
-        super(Randomizer, self).__init__()
-
-    def __init_subclass__(cls, **kwargs):
-        """
-        Hook method to automatically register all valid subclasses so we can keep track of valid observation randomizers
-        in a global dict.
-
-        This global dict stores mapping from observation randomizer network name to class.
-        We keep track of these registries to enable automated class inference at runtime, allowing
-        users to simply extend our base randomizer class and refer to that class in string form
-        in their config, without having to manually register their class internally.
-        This also future-proofs us for any additional randomizer classes we would
-        like to add ourselves.
-        """
-        ObsUtils.register_randomizer(cls)
-
-    def output_shape(self, input_shape=None):
-        """
-        This function is unused. See @output_shape_in and @output_shape_out.
-        """
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def output_shape_in(self, input_shape=None):
-        """
-        Function to compute output shape from inputs to this module. Corresponds to
-        the @forward_in operation, where raw inputs (usually observation modalities)
-        are passed in.
-
-        Args:
-            input_shape (iterable of int): shape of input. Does not include batch dimension.
-                Some modules may not need this argument, if their output does not depend 
-                on the size of the input, or if they assume fixed size input.
-
-        Returns:
-            out_shape ([int]): list of integers corresponding to output shape
-        """
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def output_shape_out(self, input_shape=None):
-        """
-        Function to compute output shape from inputs to this module. Corresponds to
-        the @forward_out operation, where processed inputs (usually encoded observation
-        modalities) are passed in.
-
-        Args:
-            input_shape (iterable of int): shape of input. Does not include batch dimension.
-                Some modules may not need this argument, if their output does not depend 
-                on the size of the input, or if they assume fixed size input.
-
-        Returns:
-            out_shape ([int]): list of integers corresponding to output shape
-        """
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def forward_in(self, inputs):
-        """
-        Randomize raw inputs.
-        """
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def forward_out(self, inputs):
-        """
-        Processing for network outputs.
-        """
-        return inputs
-
-
-class CropRandomizer(Randomizer):
-    """
-    Randomly sample crops at input, and then average across crop features at output.
-    """
-    def __init__(
-        self,
-        input_shape,
-        crop_height, 
-        crop_width, 
-        num_crops=1,
-        pos_enc=False,
-    ):
-        """
-        Args:
-            input_shape (tuple, list): shape of input (not including batch dimension)
-            crop_height (int): crop height
-            crop_width (int): crop width
-            num_crops (int): number of random crops to take
-            pos_enc (bool): if True, add 2 channels to the output to encode the spatial
-                location of the cropped pixels in the source image
-        """
-        super(CropRandomizer, self).__init__()
-
-        assert len(input_shape) == 3 # (C, H, W)
-        assert crop_height < input_shape[1]
-        assert crop_width < input_shape[2]
-
-        self.input_shape = input_shape
-        self.crop_height = crop_height
-        self.crop_width = crop_width
-        self.num_crops = num_crops
-        self.pos_enc = pos_enc
-
-    def output_shape_in(self, input_shape=None):
-        """
-        Function to compute output shape from inputs to this module. Corresponds to
-        the @forward_in operation, where raw inputs (usually observation modalities)
-        are passed in.
-
-        Args:
-            input_shape (iterable of int): shape of input. Does not include batch dimension.
-                Some modules may not need this argument, if their output does not depend 
-                on the size of the input, or if they assume fixed size input.
-
-        Returns:
-            out_shape ([int]): list of integers corresponding to output shape
-        """
-
-        # outputs are shape (C, CH, CW), or maybe C + 2 if using position encoding, because
-        # the number of crops are reshaped into the batch dimension, increasing the batch
-        # size from B to B * N
-        out_c = self.input_shape[0] + 2 if self.pos_enc else self.input_shape[0]
-        return [out_c, self.crop_height, self.crop_width]
-
-    def output_shape_out(self, input_shape=None):
-        """
-        Function to compute output shape from inputs to this module. Corresponds to
-        the @forward_out operation, where processed inputs (usually encoded observation
-        modalities) are passed in.
-
-        Args:
-            input_shape (iterable of int): shape of input. Does not include batch dimension.
-                Some modules may not need this argument, if their output does not depend 
-                on the size of the input, or if they assume fixed size input.
-
-        Returns:
-            out_shape ([int]): list of integers corresponding to output shape
-        """
-        
-        # since the forward_out operation splits [B * N, ...] -> [B, N, ...]
-        # and then pools to result in [B, ...], only the batch dimension changes,
-        # and so the other dimensions retain their shape.
-        return list(input_shape)
-
-    def forward_in(self, inputs):
-        """
-        Samples N random crops for each input in the batch, and then reshapes
-        inputs to [B * N, ...].
-        """
-        assert len(inputs.shape) >= 3 # must have at least (C, H, W) dimensions
-        out, _ = ObsUtils.sample_random_image_crops(
-            images=inputs,
-            crop_height=self.crop_height, 
-            crop_width=self.crop_width, 
-            num_crops=self.num_crops,
-            pos_enc=self.pos_enc,
-        )
-        # [B, N, ...] -> [B * N, ...]
-        return TensorUtils.join_dimensions(out, 0, 1)
-
-    def forward_out(self, inputs):
-        """
-        Splits the outputs from shape [B * N, ...] -> [B, N, ...] and then average across N
-        to result in shape [B, ...] to make sure the network output is consistent with
-        what would have happened if there were no randomization.
-        """
-        batch_size = (inputs.shape[0] // self.num_crops)
-        out = TensorUtils.reshape_dimensions(inputs, begin_axis=0, end_axis=0, 
-            target_dims=(batch_size, self.num_crops))
-        return out.mean(dim=1)
-
-    def __repr__(self):
-        """Pretty print network."""
-        header = '{}'.format(str(self.__class__.__name__))
-        msg = header + "(input_shape={}, crop_size=[{}, {}], num_crops={})".format(
-            self.input_shape, self.crop_height, self.crop_width, self.num_crops)
-        return msg
```

### Comparing `robomimic-0.2.0/robomimic/models/distributions.py` & `robomimic-0.3.0/robomimic/models/distributions.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/models/obs_nets.py` & `robomimic-0.3.0/robomimic/models/obs_nets.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 import torch.nn.functional as F
 import torch.distributions as D
 
 from robomimic.utils.python_utils import extract_class_init_kwargs_from_dict
 import robomimic.utils.tensor_utils as TensorUtils
 import robomimic.utils.obs_utils as ObsUtils
 from robomimic.models.base_nets import Module, Sequential, MLP, RNN_Base, ResNet18Conv, SpatialSoftmax, \
-    FeatureAggregator, VisualCore, Randomizer
+    FeatureAggregator
+from robomimic.models.obs_core import VisualCore, Randomizer
+from robomimic.models.transformers import PositionalEncoding, GPT_Backbone
 
 
 def obs_encoder_factory(
         obs_shapes,
         feature_activation=nn.ReLU,
         encoder_kwargs=None,
     ):
@@ -792,15 +794,15 @@
         # apply MLP + decoder to last RNN output
         outputs = self.nets["rnn"].forward(inputs=rnn_inputs, rnn_init_state=rnn_init_state, return_state=return_state)
         if return_state:
             outputs, rnn_state = outputs
 
         assert outputs.ndim == 3 # [B, T, D]
         if self._has_mlp:
-            outputs = self.nets["decoder"](self.mlp(outputs[:, -1]))
+            outputs = self.nets["decoder"](self.nets["mlp"](outputs[:, -1]))
         else:
             outputs = self.nets["decoder"](outputs[:, -1])
 
         if return_state:
             return outputs, rnn_state
         return outputs
 
@@ -847,7 +849,251 @@
         msg = ''
         indent = ' ' * 4
         msg += textwrap.indent("\n" + self._to_string(), indent)
         msg += textwrap.indent("\n\nencoder={}".format(self.nets["encoder"]), indent)
         msg += textwrap.indent("\n\nrnn={}".format(self.nets["rnn"]), indent)
         msg = header + '(' + msg + '\n)'
         return msg
+
+
+class MIMO_Transformer(Module):
+    """
+    Extension to Transformer (based on GPT architecture) to accept multiple observation 
+    dictionaries as input and to output dictionaries of tensors. Inputs are specified as 
+    a dictionary of observation dictionaries, with each key corresponding to an observation group.
+    This module utilizes @ObservationGroupEncoder to process the multiple input dictionaries and
+    @ObservationDecoder to generate tensor dictionaries. The default behavior
+    for encoding the inputs is to process visual inputs with a learned CNN and concatenating
+    the flat encodings with the other flat inputs. The default behavior for generating 
+    outputs is to use a linear layer branch to produce each modality separately
+    (including visual outputs).
+    """
+    def __init__(
+        self,
+        input_obs_group_shapes,
+        output_shapes,
+        transformer_embed_dim,
+        transformer_num_layers,
+        transformer_num_heads,
+        transformer_context_length,
+        transformer_emb_dropout=0.1,
+        transformer_attn_dropout=0.1,
+        transformer_block_output_dropout=0.1,
+        transformer_sinusoidal_embedding=False,
+        transformer_activation="gelu",
+        transformer_nn_parameter_for_timesteps=False,
+        encoder_kwargs=None,
+    ):
+        """
+        Args:
+            input_obs_group_shapes (OrderedDict): a dictionary of dictionaries.
+                Each key in this dictionary should specify an observation group, and
+                the value should be an OrderedDict that maps modalities to
+                expected shapes.
+            output_shapes (OrderedDict): a dictionary that maps modality to
+                expected shapes for outputs.
+            transformer_embed_dim (int): dimension for embeddings used by transformer
+            transformer_num_layers (int): number of transformer blocks to stack
+            transformer_num_heads (int): number of attention heads for each
+                transformer block - must divide @transformer_embed_dim evenly. Self-attention is 
+                computed over this many partitions of the embedding dimension separately.
+            transformer_context_length (int): expected length of input sequences
+            transformer_activation: non-linearity for input and output layers used in transformer
+            transformer_emb_dropout (float): dropout probability for embedding inputs in transformer
+            transformer_attn_dropout (float): dropout probability for attention outputs for each transformer block
+            transformer_block_output_dropout (float): dropout probability for final outputs for each transformer block
+            encoder_kwargs (dict): observation encoder config
+        """
+        super(MIMO_Transformer, self).__init__()
+        
+        assert isinstance(input_obs_group_shapes, OrderedDict)
+        assert np.all([isinstance(input_obs_group_shapes[k], OrderedDict) for k in input_obs_group_shapes])
+        assert isinstance(output_shapes, OrderedDict)
+
+        self.input_obs_group_shapes = input_obs_group_shapes
+        self.output_shapes = output_shapes
+
+        self.nets = nn.ModuleDict()
+        self.params = nn.ParameterDict()
+
+        # Encoder for all observation groups.
+        self.nets["encoder"] = ObservationGroupEncoder(
+            observation_group_shapes=input_obs_group_shapes,
+            encoder_kwargs=encoder_kwargs,
+            feature_activation=None,
+        )
+
+        # flat encoder output dimension
+        transformer_input_dim = self.nets["encoder"].output_shape()[0]
+
+        self.nets["embed_encoder"] = nn.Linear(
+            transformer_input_dim, transformer_embed_dim
+        )
+
+        max_timestep = transformer_context_length
+
+        if transformer_sinusoidal_embedding:
+            self.nets["embed_timestep"] = PositionalEncoding(transformer_embed_dim)
+        elif transformer_nn_parameter_for_timesteps:
+            assert (
+                not transformer_sinusoidal_embedding
+            ), "nn.Parameter only works with learned embeddings"
+            self.params["embed_timestep"] = nn.Parameter(
+                torch.zeros(1, max_timestep, transformer_embed_dim)
+            )
+        else:
+            self.nets["embed_timestep"] = nn.Embedding(max_timestep, transformer_embed_dim)
+
+        # layer norm for embeddings
+        self.nets["embed_ln"] = nn.LayerNorm(transformer_embed_dim)
+        
+        # dropout for input embeddings
+        self.nets["embed_drop"] = nn.Dropout(transformer_emb_dropout)
+
+        # GPT transformer
+        self.nets["transformer"] = GPT_Backbone(
+            embed_dim=transformer_embed_dim,
+            num_layers=transformer_num_layers,
+            num_heads=transformer_num_heads,
+            context_length=transformer_context_length,
+            attn_dropout=transformer_attn_dropout,
+            block_output_dropout=transformer_block_output_dropout,
+            activation=transformer_activation,
+        )
+
+        # decoder for output modalities
+        self.nets["decoder"] = ObservationDecoder(
+            decode_shapes=self.output_shapes,
+            input_feat_dim=transformer_embed_dim,
+        )
+
+        self.transformer_context_length = transformer_context_length
+        self.transformer_embed_dim = transformer_embed_dim
+        self.transformer_sinusoidal_embedding = transformer_sinusoidal_embedding
+        self.transformer_nn_parameter_for_timesteps = transformer_nn_parameter_for_timesteps
+
+    def output_shape(self, input_shape=None):
+        """
+        Returns output shape for this module, which is a dictionary instead
+        of a list since outputs are dictionaries.
+        """
+        return { k : list(self.output_shapes[k]) for k in self.output_shapes }
+
+    def embed_timesteps(self, embeddings):
+        """
+        Computes timestep-based embeddings (aka positional embeddings) to add to embeddings.
+        Args:
+            embeddings (torch.Tensor): embeddings prior to positional embeddings are computed
+        Returns:
+            time_embeddings (torch.Tensor): positional embeddings to add to embeddings
+        """
+        timesteps = (
+            torch.arange(
+                0,
+                embeddings.shape[1],
+                dtype=embeddings.dtype,
+                device=embeddings.device,
+            )
+            .unsqueeze(0)
+            .repeat(embeddings.shape[0], 1)
+        )
+        assert (timesteps >= 0.0).all(), "timesteps must be positive!"
+        if self.transformer_sinusoidal_embedding:
+            assert torch.is_floating_point(timesteps), timesteps.dtype
+        else:
+            timesteps = timesteps.long()
+
+        if self.transformer_nn_parameter_for_timesteps:
+            time_embeddings = self.params["embed_timestep"]
+        else:
+            time_embeddings = self.nets["embed_timestep"](
+                timesteps
+            )  # these are NOT fed into transformer, only added to the inputs.
+            # compute how many modalities were combined into embeddings, replicate time embeddings that many times
+            num_replicates = embeddings.shape[-1] // self.transformer_embed_dim
+            time_embeddings = torch.cat([time_embeddings for _ in range(num_replicates)], -1)
+            assert (
+                embeddings.shape == time_embeddings.shape
+            ), f"{embeddings.shape}, {time_embeddings.shape}"
+        return time_embeddings
+
+    def input_embedding(
+        self,
+        inputs,
+    ):
+        """
+        Process encoded observations into embeddings to pass to transformer,
+        Adds timestep-based embeddings (aka positional embeddings) to inputs.
+        Args:
+            inputs (torch.Tensor): outputs from observation encoder
+        Returns:
+            embeddings (torch.Tensor): input embeddings to pass to transformer backbone.
+        """
+        embeddings = self.nets["embed_encoder"](inputs)
+        time_embeddings = self.embed_timesteps(embeddings)
+        embeddings = embeddings + time_embeddings
+        embeddings = self.nets["embed_ln"](embeddings)
+        embeddings = self.nets["embed_drop"](embeddings)
+
+        return embeddings
+
+    
+    def forward(self, **inputs):
+        """
+        Process each set of inputs in its own observation group.
+        Args:
+            inputs (dict): a dictionary of dictionaries with one dictionary per
+                observation group. Each observation group's dictionary should map
+                modality to torch.Tensor batches. Should be consistent with
+                @self.input_obs_group_shapes. First two leading dimensions should
+                be batch and time [B, T, ...] for each tensor.
+        Returns:
+            outputs (dict): dictionary of output torch.Tensors, that corresponds
+                to @self.output_shapes. Leading dimensions will be batch and time [B, T, ...]
+                for each tensor.
+        """
+        for obs_group in self.input_obs_group_shapes:
+            for k in self.input_obs_group_shapes[obs_group]:
+                # first two dimensions should be [B, T] for inputs
+                if inputs[obs_group][k] is None:
+                    continue
+                assert inputs[obs_group][k].ndim - 2 == len(self.input_obs_group_shapes[obs_group][k])
+
+        inputs = inputs.copy()
+
+        transformer_encoder_outputs = None
+        transformer_inputs = TensorUtils.time_distributed(
+            inputs, self.nets["encoder"], inputs_as_kwargs=True
+        )
+        assert transformer_inputs.ndim == 3  # [B, T, D]
+
+        if transformer_encoder_outputs is None:
+            transformer_embeddings = self.input_embedding(transformer_inputs)
+            # pass encoded sequences through transformer
+            transformer_encoder_outputs = self.nets["transformer"].forward(transformer_embeddings)
+
+        transformer_outputs = transformer_encoder_outputs
+        # apply decoder to each timestep of sequence to get a dictionary of outputs
+        transformer_outputs = TensorUtils.time_distributed(
+            transformer_outputs, self.nets["decoder"]
+        )
+        transformer_outputs["transformer_encoder_outputs"] = transformer_encoder_outputs
+        return transformer_outputs
+
+    def _to_string(self):
+        """
+        Subclasses should override this method to print out info about network / policy.
+        """
+        return ''
+
+    def __repr__(self):
+        """Pretty print network."""
+        header = '{}'.format(str(self.__class__.__name__))
+        msg = ''
+        indent = ' ' * 4
+        if self._to_string() != '':
+            msg += textwrap.indent("\n" + self._to_string() + "\n", indent)
+        msg += textwrap.indent("\nencoder={}".format(self.nets["encoder"]), indent)
+        msg += textwrap.indent("\n\ntransformer={}".format(self.nets["transformer"]), indent)
+        msg += textwrap.indent("\n\ndecoder={}".format(self.nets["decoder"]), indent)
+        msg = header + '(' + msg + '\n)'
+        return msg
```

### Comparing `robomimic-0.2.0/robomimic/models/policy_nets.py` & `robomimic-0.3.0/robomimic/models/policy_nets.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.distributions as D
 
 import robomimic.utils.tensor_utils as TensorUtils
 from robomimic.models.base_nets import Module
-from robomimic.models.obs_nets import MIMO_MLP, RNN_MIMO_MLP
+from robomimic.models.transformers import GPT_Backbone
+from robomimic.models.obs_nets import MIMO_MLP, RNN_MIMO_MLP, MIMO_Transformer, ObservationDecoder
 from robomimic.models.vae_nets import VAE
 from robomimic.models.distributions import TanhWrappedDistribution
 
 
 class ActorNetwork(MIMO_MLP):
     """
     A basic policy network that predicts actions from observations.
@@ -969,14 +970,372 @@
 
     def _to_string(self):
         """Info to pretty print."""
         msg = "action_dim={}, std_activation={}, low_noise_eval={}, num_nodes={}, min_std={}".format(
             self.ac_dim, self.std_activation, self.low_noise_eval, self.num_modes, self.min_std)
         return msg
 
+
+class TransformerActorNetwork(MIMO_Transformer):
+    """
+    An Transformer policy network that predicts actions from observation sequences (assumed to be frame stacked
+    from previous observations) and possible from previous actions as well (in an autoregressive manner).
+    """
+    def __init__(
+        self,
+        obs_shapes,
+        ac_dim,
+        transformer_embed_dim,
+        transformer_num_layers,
+        transformer_num_heads,
+        transformer_context_length,
+        transformer_emb_dropout=0.1,
+        transformer_attn_dropout=0.1,
+        transformer_block_output_dropout=0.1,
+        transformer_sinusoidal_embedding=False,
+        transformer_activation="gelu",
+        transformer_nn_parameter_for_timesteps=False,
+        goal_shapes=None,
+        encoder_kwargs=None,
+    ):
+        """
+        Args:
+
+            obs_shapes (OrderedDict): a dictionary that maps modality to
+                expected shapes for observations.
+            
+            ac_dim (int): dimension of action space.
+
+            transformer_embed_dim (int): dimension for embeddings used by transformer
+
+            transformer_num_layers (int): number of transformer blocks to stack
+
+            transformer_num_heads (int): number of attention heads for each
+                transformer block - must divide @transformer_embed_dim evenly. Self-attention is 
+                computed over this many partitions of the embedding dimension separately.
+            
+            transformer_context_length (int): expected length of input sequences
+
+            transformer_embedding_dropout (float): dropout probability for embedding inputs in transformer
+
+            transformer_attn_dropout (float): dropout probability for attention outputs for each transformer block
+
+            transformer_block_output_dropout (float): dropout probability for final outputs for each transformer block
+            
+            goal_shapes (OrderedDict): a dictionary that maps modality to
+                expected shapes for goal observations.
+            
+            encoder_kwargs (dict or None): If None, results in default encoder_kwargs being applied. Otherwise, should
+                be nested dictionary containing relevant per-modality information for encoder networks.
+                Should be of form:
+
+                obs_modality1: dict
+                    feature_dimension: int
+                    core_class: str
+                    core_kwargs: dict
+                        ...
+                        ...
+                    obs_randomizer_class: str
+                    obs_randomizer_kwargs: dict
+                        ...
+                        ...
+                obs_modality2: dict
+                    ...
+        """
+        self.ac_dim = ac_dim
+
+        assert isinstance(obs_shapes, OrderedDict)
+        self.obs_shapes = obs_shapes
+
+        self.transformer_nn_parameter_for_timesteps = transformer_nn_parameter_for_timesteps
+
+        # set up different observation groups for @RNN_MIMO_MLP
+        observation_group_shapes = OrderedDict()
+        observation_group_shapes["obs"] = OrderedDict(self.obs_shapes)
+
+        self._is_goal_conditioned = False
+        if goal_shapes is not None and len(goal_shapes) > 0:
+            assert isinstance(goal_shapes, OrderedDict)
+            self._is_goal_conditioned = True
+            self.goal_shapes = OrderedDict(goal_shapes)
+            observation_group_shapes["goal"] = OrderedDict(self.goal_shapes)
+        else:
+            self.goal_shapes = OrderedDict()
+
+        output_shapes = self._get_output_shapes()
+        super(TransformerActorNetwork, self).__init__(
+            input_obs_group_shapes=observation_group_shapes,
+            output_shapes=output_shapes,
+            transformer_embed_dim=transformer_embed_dim,
+            transformer_num_layers=transformer_num_layers,
+            transformer_num_heads=transformer_num_heads,
+            transformer_context_length=transformer_context_length,
+            transformer_emb_dropout=transformer_emb_dropout,
+            transformer_attn_dropout=transformer_attn_dropout,
+            transformer_block_output_dropout=transformer_block_output_dropout,
+            transformer_sinusoidal_embedding=transformer_sinusoidal_embedding,
+            transformer_activation=transformer_activation,
+            transformer_nn_parameter_for_timesteps=transformer_nn_parameter_for_timesteps,
+
+            encoder_kwargs=encoder_kwargs,
+        )
+
+    def _get_output_shapes(self):
+        """
+        Allow subclasses to re-define outputs from @MIMO_Transformer, since we won't
+        always directly predict actions, but may instead predict the parameters
+        of a action distribution.
+        """
+        output_shapes = OrderedDict(action=(self.ac_dim,))
+        return output_shapes
+
+    def output_shape(self, input_shape):
+        # note: @input_shape should be dictionary (key: mod)
+        # infers temporal dimension from input shape
+        mod = list(self.obs_shapes.keys())[0]
+        T = input_shape[mod][0]
+        TensorUtils.assert_size_at_dim(input_shape, size=T, dim=0, 
+                msg="TransformerActorNetwork: input_shape inconsistent in temporal dimension")
+        return [T, self.ac_dim]
+
+    def forward(self, obs_dict, actions=None, goal_dict=None):
+        """
+        Forward a sequence of inputs through the Transformer.
+        Args:
+            obs_dict (dict): batch of observations - each tensor in the dictionary
+                should have leading dimensions batch and time [B, T, ...]
+            actions (torch.Tensor): batch of actions of shape [B, T, D]
+            goal_dict (dict): if not None, batch of goal observations
+        Returns:
+            outputs (torch.Tensor or dict): contains predicted action sequence, or dictionary
+                with predicted action sequence and predicted observation sequences
+        """
+        if self._is_goal_conditioned:
+            assert goal_dict is not None
+            # repeat the goal observation in time to match dimension with obs_dict
+            mod = list(obs_dict.keys())[0]
+            goal_dict = TensorUtils.unsqueeze_expand_at(goal_dict, size=obs_dict[mod].shape[1], dim=1)
+
+        forward_kwargs = dict(obs=obs_dict, goal=goal_dict)
+        outputs = super(TransformerActorNetwork, self).forward(**forward_kwargs)
+
+        # apply tanh squashing to ensure actions are in [-1, 1]
+        outputs["action"] = torch.tanh(outputs["action"])
+
+        return outputs["action"] # only action sequences
+
+    def _to_string(self):
+        """Info to pretty print."""
+        return "action_dim={}".format(self.ac_dim)
+
+
+class TransformerGMMActorNetwork(TransformerActorNetwork):
+    """
+    A Transformer GMM policy network that predicts sequences of action distributions from observation 
+    sequences (assumed to be frame stacked from previous observations).
+    """
+    def __init__(
+        self,
+        obs_shapes,
+        ac_dim,
+        transformer_embed_dim,
+        transformer_num_layers,
+        transformer_num_heads,
+        transformer_context_length,
+        transformer_emb_dropout=0.1,
+        transformer_attn_dropout=0.1,
+        transformer_block_output_dropout=0.1,
+        transformer_sinusoidal_embedding=False,
+        transformer_activation="gelu",
+        transformer_nn_parameter_for_timesteps=False,
+        num_modes=5,
+        min_std=0.01,
+        std_activation="softplus",
+        low_noise_eval=True,
+        use_tanh=False,
+        goal_shapes=None,
+        encoder_kwargs=None,
+    ):
+        """
+        Args:
+
+            obs_shapes (OrderedDict): a dictionary that maps modality to
+                expected shapes for observations.
+            
+            ac_dim (int): dimension of action space.
+
+            transformer_embed_dim (int): dimension for embeddings used by transformer
+
+            transformer_num_layers (int): number of transformer blocks to stack
+
+            transformer_num_heads (int): number of attention heads for each
+                transformer block - must divide @transformer_embed_dim evenly. Self-attention is 
+                computed over this many partitions of the embedding dimension separately.
+            
+            transformer_context_length (int): expected length of input sequences
+
+            transformer_embedding_dropout (float): dropout probability for embedding inputs in transformer
+
+            transformer_attn_dropout (float): dropout probability for attention outputs for each transformer block
+
+            transformer_block_output_dropout (float): dropout probability for final outputs for each transformer block
+
+            num_modes (int): number of GMM modes
+
+            min_std (float): minimum std output from network
+
+            std_activation (None or str): type of activation to use for std deviation. Options are:
+
+                `'softplus'`: Softplus activation applied
+
+                `'exp'`: Exp applied; this corresponds to network output being interpreted as log_std instead of std
+
+            low_noise_eval (float): if True, model will sample from GMM with low std, so that
+                one of the GMM modes will be sampled (approximately)
+
+            use_tanh (bool): if True, use a tanh-Gaussian distribution
+
+            encoder_kwargs (dict or None): If None, results in default encoder_kwargs being applied. Otherwise, should
+                be nested dictionary containing relevant per-modality information for encoder networks.
+                Should be of form:
+
+                obs_modality1: dict
+                    feature_dimension: int
+                    core_class: str
+                    core_kwargs: dict
+                        ...
+                        ...
+                    obs_randomizer_class: str
+                    obs_randomizer_kwargs: dict
+                        ...
+                        ...
+                obs_modality2: dict
+                    ...
+        """
+        
+        # parameters specific to GMM actor
+        self.num_modes = num_modes
+        self.min_std = min_std
+        self.low_noise_eval = low_noise_eval
+        self.use_tanh = use_tanh
+
+        # Define activations to use
+        self.activations = {
+            "softplus": F.softplus,
+            "exp": torch.exp,
+        }
+        assert std_activation in self.activations, \
+            "std_activation must be one of: {}; instead got: {}".format(self.activations.keys(), std_activation)
+        self.std_activation = std_activation
+
+        super(TransformerGMMActorNetwork, self).__init__(
+            obs_shapes=obs_shapes,
+            ac_dim=ac_dim,
+            transformer_embed_dim=transformer_embed_dim,
+            transformer_num_layers=transformer_num_layers,
+            transformer_num_heads=transformer_num_heads,
+            transformer_context_length=transformer_context_length,
+            transformer_emb_dropout=transformer_emb_dropout,
+            transformer_attn_dropout=transformer_attn_dropout,
+            transformer_block_output_dropout=transformer_block_output_dropout,
+            transformer_sinusoidal_embedding=transformer_sinusoidal_embedding,
+            transformer_activation=transformer_activation,
+            transformer_nn_parameter_for_timesteps=transformer_nn_parameter_for_timesteps,            
+            encoder_kwargs=encoder_kwargs,
+            goal_shapes=goal_shapes,
+        )
+
+    def _get_output_shapes(self):
+        """
+        Tells @MIMO_Transformer superclass about the output dictionary that should be generated
+        at the last layer. Network outputs parameters of GMM distribution.
+        """
+        return OrderedDict(
+            mean=(self.num_modes, self.ac_dim), 
+            scale=(self.num_modes, self.ac_dim), 
+            logits=(self.num_modes,),
+        )
+
+    def forward_train(self, obs_dict, actions=None, goal_dict=None, low_noise_eval=None):
+        """
+        Return full GMM distribution, which is useful for computing
+        quantities necessary at train-time, like log-likelihood, KL 
+        divergence, etc.
+        Args:
+            obs_dict (dict): batch of observations
+            actions (torch.Tensor): batch of actions
+            goal_dict (dict): if not None, batch of goal observations
+        Returns:
+            dists (Distribution): sequence of GMM distributions over the timesteps
+        """
+        if self._is_goal_conditioned:
+            assert goal_dict is not None
+            # repeat the goal observation in time to match dimension with obs_dict
+            mod = list(obs_dict.keys())[0]
+            goal_dict = TensorUtils.unsqueeze_expand_at(goal_dict, size=obs_dict[mod].shape[1], dim=1)
+
+        forward_kwargs = dict(obs=obs_dict, goal=goal_dict)
+
+        outputs = MIMO_Transformer.forward(self, **forward_kwargs)
+        
+        means = outputs["mean"]
+        scales = outputs["scale"]
+        logits = outputs["logits"]
+
+        # apply tanh squashing to mean if not using tanh-GMM to ensure means are in [-1, 1]
+        if not self.use_tanh:
+            means = torch.tanh(means)
+
+        if low_noise_eval is None:
+            low_noise_eval = self.low_noise_eval
+        if low_noise_eval and (not self.training):
+            # low-noise for all Gaussian dists
+            scales = torch.ones_like(means) * 1e-4
+        else:
+            # post-process the scale accordingly
+            scales = self.activations[self.std_activation](scales) + self.min_std
+
+        # mixture components - make sure that `batch_shape` for the distribution is equal
+        # to (batch_size, timesteps, num_modes) since MixtureSameFamily expects this shape
+        component_distribution = D.Normal(loc=means, scale=scales)
+        component_distribution = D.Independent(component_distribution, 1) # shift action dim to event shape
+
+        # unnormalized logits to categorical distribution for mixing the modes
+        mixture_distribution = D.Categorical(logits=logits)
+
+        dists = D.MixtureSameFamily(
+            mixture_distribution=mixture_distribution,
+            component_distribution=component_distribution,
+        )
+
+        if self.use_tanh:
+            # Wrap distribution with Tanh
+            dists = TanhWrappedDistribution(base_dist=dists, scale=1.)
+
+        return dists
+
+    def forward(self, obs_dict, actions=None, goal_dict=None):
+        """
+        Samples actions from the policy distribution.
+        Args:
+            obs_dict (dict): batch of observations
+            actions (torch.Tensor): batch of actions
+            goal_dict (dict): if not None, batch of goal observations
+        Returns:
+            action (torch.Tensor): batch of actions from policy distribution
+        """
+        out = self.forward_train(obs_dict=obs_dict, actions=actions, goal_dict=goal_dict)
+        return out.sample()
+
+    def _to_string(self):
+        """Info to pretty print."""
+        msg = "action_dim={}, std_activation={}, low_noise_eval={}, num_nodes={}, min_std={}".format(
+            self.ac_dim, self.std_activation, self.low_noise_eval, self.num_modes, self.min_std)
+        return msg
+
 
 class VAEActor(Module):
     """
     A VAE that models a distribution of actions conditioned on observations.
     The VAE prior and decoder are used at test-time as the policy.
     """
     def __init__(
```

### Comparing `robomimic-0.2.0/robomimic/models/vae_nets.py` & `robomimic-0.3.0/robomimic/models/vae_nets.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             obs_shapes = net_kwargs["obs_shapes"]
             goal_shapes = net_kwargs["goal_shapes"]
             obs_group_shapes = OrderedDict()
             assert isinstance(obs_shapes, OrderedDict)
             obs_group_shapes["obs"] = OrderedDict(obs_shapes)
             if goal_shapes is not None and len(goal_shapes) > 0:
                 assert isinstance(goal_shapes, OrderedDict)
-                obs_group_shapes["goal"] = OrderedDict(self.goal_shapes)
+                obs_group_shapes["goal"] = OrderedDict(goal_shapes)
             self.prior_module = MIMO_MLP(
                 input_obs_group_shapes=obs_group_shapes,
                 output_shapes=mlp_output_shapes,
                 layer_dims=net_kwargs["mlp_layer_dims"],
                 encoder_kwargs=net_kwargs["encoder_kwargs"],
             )
```

### Comparing `robomimic-0.2.0/robomimic/models/value_nets.py` & `robomimic-0.3.0/robomimic/models/value_nets.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/conversion/convert_d4rl.py` & `robomimic-0.3.0/robomimic/scripts/conversion/convert_d4rl.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         a `d4rl/converted` subfolder will be created in this folder with the converted
         datasets (if they do not already exist). Defaults to the datasets folder at
         the top-level of the repository.
 
 Example usage:
 
     # downloads to default path at robomimic/datasets/d4rl
-    python convert_d4rl.py --env walker2d-medium-expert-v0
+    python convert_d4rl.py --env walker2d-medium-expert-v2
 
     # download to custom path
-    python convert_d4rl.py --env walker2d-medium-expert-v0 --folder /path/to/folder
+    python convert_d4rl.py --env walker2d-medium-expert-v2 --folder /path/to/folder
 """
 
 import os
 import h5py
 import json
 import argparse
 import numpy as np
```

### Comparing `robomimic-0.2.0/robomimic/scripts/conversion/convert_robosuite.py` & `robomimic-0.3.0/robomimic/scripts/conversion/convert_robosuite.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
     # store env meta
     env_name = f["data"].attrs["env"]
     env_info = json.loads(f["data"].attrs["env_info"])
     env_meta = dict(
         type=EB.EnvType.ROBOSUITE_TYPE,
         env_name=env_name,
+        env_version=f["data"].attrs["repository_version"],
         env_kwargs=env_info,
     )
     if "env_args" in f["data"].attrs:
         del f["data"].attrs["env_args"]
     f["data"].attrs["env_args"] = json.dumps(env_meta, indent=4)
 
     print("====== Stored env meta ======")
```

### Comparing `robomimic-0.2.0/robomimic/scripts/conversion/convert_roboturk_pilot.py` & `robomimic-0.3.0/robomimic/scripts/conversion/convert_roboturk_pilot.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/dataset_states_to_obs.py` & `robomimic-0.3.0/robomimic/scripts/dataset_states_to_obs.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,20 @@
     # extract low-dimensional observations
     python dataset_states_to_obs.py --dataset /path/to/demo.hdf5 --output_name low_dim.hdf5 --done_mode 2
     
     # extract 84x84 image observations
     python dataset_states_to_obs.py --dataset /path/to/demo.hdf5 --output_name image.hdf5 \
         --done_mode 2 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
+    # (space saving option) extract 84x84 image observations with compression and without 
+    # extracting next obs (not needed for pure imitation learning algos)
+    python dataset_states_to_obs.py --dataset /path/to/demo.hdf5 --output_name image.hdf5 \
+        --done_mode 2 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84 \
+        --compress --exclude-next-obs
+
     # use dense rewards, and only annotate the end of trajectories with done signal
     python dataset_states_to_obs.py --dataset /path/to/demo.hdf5 --output_name image_dense_done_1.hdf5 \
         --done_mode 1 --dense --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 """
 import os
 import json
 import h5py
@@ -206,16 +212,23 @@
         #            consistent as well
         ep_data_grp = data_grp.create_group(ep)
         ep_data_grp.create_dataset("actions", data=np.array(traj["actions"]))
         ep_data_grp.create_dataset("states", data=np.array(traj["states"]))
         ep_data_grp.create_dataset("rewards", data=np.array(traj["rewards"]))
         ep_data_grp.create_dataset("dones", data=np.array(traj["dones"]))
         for k in traj["obs"]:
-            ep_data_grp.create_dataset("obs/{}".format(k), data=np.array(traj["obs"][k]))
-            ep_data_grp.create_dataset("next_obs/{}".format(k), data=np.array(traj["next_obs"][k]))
+            if args.compress:
+                ep_data_grp.create_dataset("obs/{}".format(k), data=np.array(traj["obs"][k]), compression="gzip")
+            else:
+                ep_data_grp.create_dataset("obs/{}".format(k), data=np.array(traj["obs"][k]))
+            if not args.exclude_next_obs:
+                if args.compress:
+                    ep_data_grp.create_dataset("next_obs/{}".format(k), data=np.array(traj["next_obs"][k]), compression="gzip")
+                else:
+                    ep_data_grp.create_dataset("next_obs/{}".format(k), data=np.array(traj["next_obs"][k]))
 
         # episode metadata
         if is_robosuite_env:
             ep_data_grp.attrs["model_file"] = traj["initial_state_dict"]["model"] # model xml for this episode
         ep_data_grp.attrs["num_samples"] = traj["actions"].shape[0] # number of transitions in this episode
         total_samples += traj["actions"].shape[0]
         print("ep {}: wrote {} transitions to group {}".format(ind, ep_data_grp.attrs["num_samples"], ep))
@@ -311,9 +324,23 @@
     # flag for copying dones from source file instead of re-writing them
     parser.add_argument(
         "--copy_dones", 
         action='store_true',
         help="(optional) copy dones from source file instead of inferring them",
     )
 
+    # flag to exclude next obs in dataset
+    parser.add_argument(
+        "--exclude-next-obs", 
+        action='store_true',
+        help="(optional) exclude next obs in dataset",
+    )
+
+    # flag to compress observations with gzip option in hdf5
+    parser.add_argument(
+        "--compress", 
+        action='store_true',
+        help="(optional) compress observations with gzip option in hdf5",
+    )
+
     args = parser.parse_args()
     dataset_states_to_obs(args)
```

### Comparing `robomimic-0.2.0/robomimic/scripts/download_datasets.py` & `robomimic-0.3.0/robomimic/scripts/download_datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     # hdf5 types to download datasets for
     parser.add_argument(
         "--hdf5_types",
         type=str,
         nargs='+',
         default=["low_dim"],
-        help="hdf5 types to download datasets for (e.g. raw, low_dim, image). Defaults to low_dim. Pass 'all' \
+        help="hdf5 types to download datasets for (e.g. raw, low_dim, image). Defaults to raw. Pass 'all' \
             to download datasets for all available hdf5 types per task and dataset, or directly specify the list\
             of hdf5 types.",
     )
 
     # dry run - don't actually download datasets, but print which datasets would be downloaded
     parser.add_argument(
         "--dry_run",
@@ -140,14 +140,21 @@
             for dataset_type in DATASET_REGISTRY[task]:
                 if dataset_type in download_dataset_types:
                     for hdf5_type in DATASET_REGISTRY[task][dataset_type]:
                         if hdf5_type in download_hdf5_types:
                             download_dir = os.path.abspath(os.path.join(default_base_dir, task, dataset_type))
                             print("\nDownloading dataset:\n    task: {}\n    dataset type: {}\n    hdf5 type: {}\n    download path: {}"
                                 .format(task, dataset_type, hdf5_type, download_dir))
+                            url = DATASET_REGISTRY[task][dataset_type][hdf5_type]["url"]
+                            if url is None:
+                                print(
+                                    "Skipping {}-{}-{}, no url for dataset exists.".format(task, dataset_type, hdf5_type)
+                                    + " Create this dataset locally by running the appropriate command from robomimic/scripts/extract_obs_from_raw_datasets.sh."
+                                )
+                                continue
                             if args.dry_run:
                                 print("\ndry run: skip download")
                             else:
                                 # Make sure path exists and create if it doesn't
                                 os.makedirs(download_dir, exist_ok=True)
                                 FileUtils.download_url(
                                     url=DATASET_REGISTRY[task][dataset_type][hdf5_type]["url"],
```

### Comparing `robomimic-0.2.0/robomimic/scripts/download_momart_datasets.py` & `robomimic-0.3.0/robomimic/scripts/download_momart_datasets.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/extract_obs_from_raw_datasets.sh` & `robomimic-0.3.0/robomimic/scripts/extract_obs_from_raw_datasets.sh`

 * *Files 21% similar despite different names*

```diff
@@ -11,130 +11,130 @@
 
 
 ### mg ###
 
 
 # lift - mg, sparse
 python dataset_states_to_obs.py --done_mode 0 \
---dataset $BASE_DATASET_DIR/lift/mg/demo.hdf5 \
---output_name low_dim_sparse.hdf5
+--dataset $BASE_DATASET_DIR/lift/mg/demo_v141.hdf5 \
+--output_name low_dim_sparse_v141.hdf5
 python dataset_states_to_obs.py --done_mode 0 \
---dataset $BASE_DATASET_DIR/lift/mg/demo.hdf5 \
---output_name image_sparse.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/lift/mg/demo_v141.hdf5 \
+--output_name image_sparse_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # lift - mg, dense
 python dataset_states_to_obs.py --done_mode 0 --shaped \
---dataset $BASE_DATASET_DIR/lift/mg/demo.hdf5 \
---output_name low_dim_dense.hdf5
+--dataset $BASE_DATASET_DIR/lift/mg/demo_v141.hdf5 \
+--output_name low_dim_dense_v141.hdf5
 python dataset_states_to_obs.py --done_mode 0 --shaped \
---dataset $BASE_DATASET_DIR/lift/mg/demo.hdf5 \
---output_name image_dense.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/lift/mg/demo_v141.hdf5 \
+--output_name image_dense_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # can - mg, sparse
 python dataset_states_to_obs.py --done_mode 0 \
---dataset $BASE_DATASET_DIR/can/mg/demo.hdf5 \
---output_name low_dim_sparse.hdf5
+--dataset $BASE_DATASET_DIR/can/mg/demo_v141.hdf5 \
+--output_name low_dim_sparse_v141.hdf5
 python dataset_states_to_obs.py --done_mode 0 \
---dataset $BASE_DATASET_DIR/can/mg/demo.hdf5 \
---output_name image_sparse.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/can/mg/demo_v141.hdf5 \
+--output_name image_sparse_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # can - mg, dense
 python dataset_states_to_obs.py --done_mode 0 --shaped \
---dataset $BASE_DATASET_DIR/can/mg/demo.hdf5 \
---output_name low_dim_dense.hdf5
+--dataset $BASE_DATASET_DIR/can/mg/demo_v141.hdf5 \
+--output_name low_dim_dense_v141.hdf5
 python dataset_states_to_obs.py --done_mode 0 --shaped \
---dataset $BASE_DATASET_DIR/can/mg/demo.hdf5 \
---output_name image_dense.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/can/mg/demo_v141.hdf5 \
+--output_name image_dense_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 
 ### NOTE: we use done-mode 2 for PH / MH (dones on task success and end of trajectory) ###
 
 
 ### ph ###
 
 
 # lift - ph
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/lift/ph/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/lift/ph/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/lift/ph/demo.hdf5 \
---output_name image.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/lift/ph/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # can - ph
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/can/ph/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/can/ph/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/can/ph/demo.hdf5 \
---output_name image.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/can/ph/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # square - ph
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/square/ph/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/square/ph/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/square/ph/demo.hdf5 \
---output_name image.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/square/ph/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # transport - ph
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/transport/ph/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/transport/ph/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/transport/ph/demo.hdf5 \
---output_name image.hdf5 --camera_names shouldercamera0 shouldercamera1 robot0_eye_in_hand robot1_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/transport/ph/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names shouldercamera0 shouldercamera1 robot0_eye_in_hand robot1_eye_in_hand --camera_height 84 --camera_width 84
 
 # tool hang - ph
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/tool_hang/ph/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/tool_hang/ph/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/tool_hang/ph/demo.hdf5 \
---output_name image.hdf5 --camera_names sideview robot0_eye_in_hand --camera_height 240 --camera_width 240
+--dataset $BASE_DATASET_DIR/tool_hang/ph/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names sideview robot0_eye_in_hand --camera_height 240 --camera_width 240
 
 
 ### mh ###
 
 
 # lift - mh
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/lift/mh/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/lift/mh/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/lift/mh/demo.hdf5 \
---output_name image.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/lift/mh/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # can - mh
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/can/mh/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/can/mh/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/can/mh/demo.hdf5 \
---output_name image.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/can/mh/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # square - mh
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/square/mh/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/square/mh/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/square/mh/demo.hdf5 \
---output_name image.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/square/mh/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
 
 # transport - mh
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/transport/mh/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/transport/mh/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/transport/mh/demo.hdf5 \
---output_name image.hdf5 --camera_names shouldercamera0 shouldercamera1 robot0_eye_in_hand robot1_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/transport/mh/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names shouldercamera0 shouldercamera1 robot0_eye_in_hand robot1_eye_in_hand --camera_height 84 --camera_width 84
 
 
 ### can-paired ###
 
 
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/can/paired/demo.hdf5 \
---output_name low_dim.hdf5
+--dataset $BASE_DATASET_DIR/can/paired/demo_v141.hdf5 \
+--output_name low_dim_v141.hdf5
 python dataset_states_to_obs.py --done_mode 2 \
---dataset $BASE_DATASET_DIR/can/paired/demo.hdf5 \
---output_name image.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
+--dataset $BASE_DATASET_DIR/can/paired/demo_v141.hdf5 \
+--output_name image_v141.hdf5 --camera_names agentview robot0_eye_in_hand --camera_height 84 --camera_width 84
```

### Comparing `robomimic-0.2.0/robomimic/scripts/generate_config_templates.py` & `robomimic-0.3.0/robomimic/scripts/generate_config_templates.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/generate_paper_configs.py` & `robomimic-0.3.0/robomimic/scripts/generate_paper_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,25 +211,42 @@
 
         # look up rollout evaluation horizon in registry and set it
         config.experiment.rollout.horizon = DATASET_REGISTRY[task_name][dataset_type][hdf5_type]["horizon"]
 
         if dataset_type == "mg":
             # machine-generated datasets did not use validation
             config.experiment.validate = False
+        else:
+            # all other datasets used validation
+            config.experiment.validate = True
 
         if is_real_dataset:
             # no evaluation rollouts for real robot training
             config.experiment.rollout.enabled = False
 
     with config.train.values_unlocked():
-        # set dataset path and possibly filter key
-        file_name = DATASET_REGISTRY[task_name][dataset_type][hdf5_type]["url"].split("/")[-1]
+        # set dataset path and possibly filter keys
+        url = DATASET_REGISTRY[task_name][dataset_type][hdf5_type]["url"]
+        if url is None:
+            # infer file_name
+            if task_name in ["lift", "can", "square", "tool_hang", "transport"]:
+                file_name = "{}_v141.hdf5".format(hdf5_type)
+            elif task_name in ["lift_real", "can_real", "tool_hang_real"]:
+                file_name = "{}.hdf5".format(hdf5_type)
+            else:
+                raise ValueError("Unknown dataset type")
+        else:
+            file_name = url.split("/")[-1]
         config.train.data = os.path.join(base_dataset_dir, task_name, dataset_type, file_name)
-        if filter_key is not None:
-            config.train.hdf5_filter_key = filter_key
+        config.train.hdf5_filter_key = None if filter_key is None else filter_key
+        config.train.hdf5_validation_filter_key = None
+        if config.experiment.validate:
+            # set train and valid keys for validation
+            config.train.hdf5_filter_key = "train" if filter_key is None else "{}_train".format(filter_key)
+            config.train.hdf5_validation_filter_key = "valid" if filter_key is None else "{}_valid".format(filter_key)
 
     with config.observation.values_unlocked():
         # maybe modify observation names and randomization sizes (since image size might be different)
 
         if is_real_dataset:
             # modify observation names for real robot datasets
             config.observation.modalities.obs.low_dim = [
@@ -1164,46 +1181,59 @@
             config.algo.optim_params.actor.learning_rate.initial = 1e-3
             config.algo.actor.enabled = True
             config.algo.action_sampler.vae.kl_weight = 0.5
         return config
 
     def cql_algo_config_modifier(config):
         with config.algo.values_unlocked():
-            # taken from TD3-BC settings describe in their paper
+            # taken from TD3-BC settings described in their paper
             config.algo.optim_params.critic.learning_rate.initial = 3e-4
             config.algo.optim_params.actor.learning_rate.initial = 3e-5
             config.algo.actor.bc_start_steps = 40000                        # pre-training steps for actor
             config.algo.critic.target_q_gap = None                          # no Lagrange, and fixed weight of 10.0
             config.algo.critic.cql_weight = 10.0
             config.algo.critic.min_q_weight = 1.0 
             config.algo.critic.deterministic_backup = True                  # deterministic backup (no entropy in Q-target)
             config.algo.actor.layer_dims = (256, 256, 256)                  # MLP sizes
             config.algo.critic.layer_dims = (256, 256, 256)
         return config
+    
+    def iql_algo_config_modifier(config):
+        with config.algo.values_unlocked():
+            # taken from IQL settings described in their paper
+            config.algo.target_tau = 0.005
+            config.algo.vf_quantile = 0.7
+            config.algo.adv.beta = 3.0
+            config.algo.optim_params.critic.learning_rate.initial = 3e-4
+            config.algo.optim_params.vf.learning_rate.initial = 3e-4
+            config.algo.optim_params.actor.learning_rate.initial = 3e-4
+            config.algo.actor.layer_dims = (256, 256, 256)                  # MLP sizes
+            config.algo.critic.layer_dims = (256, 256, 256)
+        return config
 
     d4rl_tasks = [
-        # "halfcheetah-random-v0",
-        # "hopper-random-v0",
-        # "walker2d-random-v0",
-        "halfcheetah-medium-v0",
-        "hopper-medium-v0",
-        "walker2d-medium-v0",
-        "halfcheetah-expert-v0",
-        "hopper-expert-v0",
-        "walker2d-expert-v0",
-        "halfcheetah-medium-expert-v0",
-        "hopper-medium-expert-v0",
-        "walker2d-medium-expert-v0",
-        # "halfcheetah-medium-replay-v0",
-        # "hopper-medium-replay-v0",
-        # "walker2d-medium-replay-v0",
+        # "halfcheetah-random-v2",
+        # "hopper-random-v2",
+        # "walker2d-random-v2",
+        "halfcheetah-medium-v2",
+        "hopper-medium-v2",
+        "walker2d-medium-v2",
+        "halfcheetah-expert-v2",
+        "hopper-expert-v2",
+        "walker2d-expert-v2",
+        "halfcheetah-medium-expert-v2",
+        "hopper-medium-expert-v2",
+        "walker2d-medium-expert-v2",
+        # "halfcheetah-medium-replay-v2",
+        # "hopper-medium-replay-v2",
+        # "walker2d-medium-replay-v2",
     ]
     d4rl_json_paths = Config() # use for convenient nested dict
     for task_name in d4rl_tasks:
-        for algo_name in ["bcq", "cql", "td3_bc"]:
+        for algo_name in ["bcq", "cql", "td3_bc", "iql"]:
             config = config_factory(algo_name=algo_name)
 
             # hack: copy experiment and train sections from td3-bc, since that has defaults for training with D4RL
             if algo_name != "td3_bc":
                 ref_config = config_factory(algo_name="td3_bc")
                 with config.values_unlocked():
                     config.experiment = ref_config.experiment
@@ -1212,23 +1242,27 @@
                     config.train.hdf5_normalize_obs = False # only TD3-BC uses observation normalization
 
             # modify algo section for d4rl defaults
             if algo_name == "bcq":
                 config = bcq_algo_config_modifier(config)
             elif algo_name == "cql":
                 config = cql_algo_config_modifier(config)
+            elif algo_name == "iql":
+                config = iql_algo_config_modifier(config)
 
             # set experiment name
             with config.experiment.values_unlocked():
                 config.experiment.name = "{}_{}_{}".format("d4rl", algo_name, task_name)
             # set output folder and dataset
             with config.train.values_unlocked():
                 if base_output_dir is None:
-                    base_output_dir = "../{}_trained_models".format(algo_name)
-                config.train.output_dir = os.path.join(base_output_dir, "d4rl", algo_name, task_name, "trained_models")
+                    base_output_dir_for_algo = "../{}_trained_models".format(algo_name)
+                else:
+                    base_output_dir_for_algo = base_output_dir
+                config.train.output_dir = os.path.join(base_output_dir_for_algo, "d4rl", algo_name, task_name, "trained_models")
                 config.train.data = os.path.join(base_dataset_dir, "d4rl", "converted", 
                     "{}.hdf5".format(task_name.replace("-", "_")))
 
             # save config to json file
             dir_to_save = os.path.join(base_config_dir, "d4rl", task_name)
             os.makedirs(dir_to_save, exist_ok=True)
             json_path = os.path.join(dir_to_save, "{}.json".format(algo_name))
```

### Comparing `robomimic-0.2.0/robomimic/scripts/get_dataset_info.py` & `robomimic-0.3.0/robomimic/scripts/get_dataset_info.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/hyperparam_helper.py` & `robomimic-0.3.0/robomimic/scripts/hyperparam_helper.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/playback_dataset.py` & `robomimic-0.3.0/robomimic/scripts/playback_dataset.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/run_trained_agent.py` & `robomimic-0.3.0/robomimic/scripts/run_trained_agent.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/split_train_val.py` & `robomimic-0.3.0/robomimic/scripts/split_train_val.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/scripts/train.py` & `robomimic-0.3.0/robomimic/scripts/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,26 +35,28 @@
 import robomimic.utils.train_utils as TrainUtils
 import robomimic.utils.torch_utils as TorchUtils
 import robomimic.utils.obs_utils as ObsUtils
 import robomimic.utils.env_utils as EnvUtils
 import robomimic.utils.file_utils as FileUtils
 from robomimic.config import config_factory
 from robomimic.algo import algo_factory, RolloutPolicy
-from robomimic.utils.log_utils import PrintLogger, DataLogger
+from robomimic.utils.log_utils import PrintLogger, DataLogger, flush_warnings
 
 
 def train(config, device):
     """
     Train a model using the algorithm.
     """
 
     # first set seeds
     np.random.seed(config.train.seed)
     torch.manual_seed(config.train.seed)
 
+    torch.set_num_threads(2)
+
     print("\n============= New Training Run with Config =============")
     print(config)
     print("")
     log_dir, ckpt_dir, video_dir = TrainUtils.get_exp_dir(config)
 
     if config.experiment.logging.terminal_output_to_txt:
         # log stdout and stderr to a text file
@@ -97,43 +99,54 @@
             env = EnvUtils.create_env_from_metadata(
                 env_meta=env_meta,
                 env_name=env_name, 
                 render=False, 
                 render_offscreen=config.experiment.render_video,
                 use_image_obs=shape_meta["use_images"], 
             )
+            env = EnvUtils.wrap_env_from_config(env, config=config) # apply environment warpper, if applicable
             envs[env.name] = env
             print(envs[env.name])
 
     print("")
 
     # setup for a new training run
     data_logger = DataLogger(
         log_dir,
+        config,
         log_tb=config.experiment.logging.log_tb,
+        log_wandb=config.experiment.logging.log_wandb,
     )
     model = algo_factory(
         algo_name=config.algo_name,
         config=config,
         obs_key_shapes=shape_meta["all_shapes"],
         ac_dim=shape_meta["ac_dim"],
         device=device,
     )
+    
+    # save the config as a json file
+    with open(os.path.join(log_dir, '..', 'config.json'), 'w') as outfile:
+        json.dump(config, outfile, indent=4)
 
     print("\n============= Model Summary =============")
     print(model)  # print model summary
     print("")
 
     # load training data
     trainset, validset = TrainUtils.load_data_for_training(
         config, obs_keys=shape_meta["all_obs_keys"])
     train_sampler = trainset.get_dataset_sampler()
     print("\n============= Training Dataset =============")
     print(trainset)
     print("")
+    if validset is not None:
+        print("\n============= Validation Dataset =============")
+        print(validset)
+        print("")
 
     # maybe retreve statistics for normalizing observations
     obs_normalization_stats = None
     if config.train.hdf5_normalize_obs:
         obs_normalization_stats = trainset.get_obs_normalization_stats()
 
     # initialize data loaders
@@ -157,26 +170,39 @@
             shuffle=(valid_sampler is None),
             num_workers=num_workers,
             drop_last=True
         )
     else:
         valid_loader = None
 
+    # print all warnings before training begins
+    print("*" * 50)
+    print("Warnings generated by robomimic have been duplicated here (from above) for convenience. Please check them carefully.")
+    flush_warnings()
+    print("*" * 50)
+    print("")
+
     # main training loop
     best_valid_loss = None
     best_return = {k: -np.inf for k in envs} if config.experiment.rollout.enabled else None
     best_success_rate = {k: -1. for k in envs} if config.experiment.rollout.enabled else None
     last_ckpt_time = time.time()
 
     # number of learning steps per epoch (defaults to a full dataset pass)
     train_num_steps = config.experiment.epoch_every_n_steps
     valid_num_steps = config.experiment.validation_epoch_every_n_steps
 
     for epoch in range(1, config.train.num_epochs + 1): # epoch numbers start at 1
-        step_log = TrainUtils.run_epoch(model=model, data_loader=train_loader, epoch=epoch, num_steps=train_num_steps)
+        step_log = TrainUtils.run_epoch(
+            model=model,
+            data_loader=train_loader,
+            epoch=epoch,
+            num_steps=train_num_steps,
+            obs_normalization_stats=obs_normalization_stats,
+        )
         model.on_epoch_end(epoch)
 
         # setup checkpoint path
         epoch_ckpt_name = "model_epoch_{}".format(epoch)
 
         # check for recurring checkpoint saving conditions
         should_save_ckpt = False
```

### Comparing `robomimic-0.2.0/robomimic/utils/dataset.py` & `robomimic-0.3.0/robomimic/utils/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,17 +280,17 @@
         all_data = dict()
         print("SequenceDataset: loading dataset into memory...")
         for ep in LogUtils.custom_tqdm(demo_list):
             all_data[ep] = {}
             all_data[ep]["attrs"] = {}
             all_data[ep]["attrs"]["num_samples"] = hdf5_file["data/{}".format(ep)].attrs["num_samples"]
             # get obs
-            all_data[ep]["obs"] = {k: hdf5_file["data/{}/obs/{}".format(ep, k)][()].astype('float32') for k in obs_keys}
+            all_data[ep]["obs"] = {k: hdf5_file["data/{}/obs/{}".format(ep, k)][()] for k in obs_keys}
             if load_next_obs:
-                all_data[ep]["next_obs"] = {k: hdf5_file["data/{}/next_obs/{}".format(ep, k)][()].astype('float32') for k in obs_keys}
+                all_data[ep]["next_obs"] = {k: hdf5_file["data/{}/next_obs/{}".format(ep, k)][()] for k in obs_keys}
             # get other dataset keys
             for k in dataset_keys:
                 if k in hdf5_file["data/{}".format(ep)]:
                     all_data[ep][k] = hdf5_file["data/{}/{}".format(ep, k)][()].astype('float32')
                 else:
                     all_data[ep][k] = np.zeros((all_data[ep]["attrs"]["num_samples"], 1), dtype=np.float32)
 
@@ -421,14 +421,15 @@
         demo_length_offset = 0 if self.pad_seq_length else (self.seq_length - 1)
         end_index_in_demo = demo_length - demo_length_offset
 
         meta = self.get_dataset_sequence_from_demo(
             demo_id,
             index_in_demo=index_in_demo,
             keys=self.dataset_keys,
+            num_frames_to_stack=self.n_frame_stack - 1, # note: need to decrement self.n_frame_stack by one
             seq_length=self.seq_length
         )
 
         # determine goal index
         goal_index = None
         if self.goal_mode == "last":
             goal_index = end_index_in_demo - 1
@@ -505,19 +506,19 @@
         if not self.pad_seq_length:
             assert seq_end_pad == 0
 
         # fetch observation from the dataset file
         seq = dict()
         for k in keys:
             data = self.get_dataset_for_ep(demo_id, k)
-            seq[k] = data[seq_begin_index: seq_end_index].astype("float32")
+            seq[k] = data[seq_begin_index: seq_end_index]
 
         seq = TensorUtils.pad_sequence(seq, padding=(seq_begin_pad, seq_end_pad), pad_same=True)
         pad_mask = np.array([0] * seq_begin_pad + [1] * (seq_end_index - seq_begin_index) + [0] * seq_end_pad)
-        pad_mask = pad_mask[:, None].astype(np.bool)
+        pad_mask = pad_mask[:, None].astype(bool)
 
         return seq, pad_mask
 
     def get_obs_sequence_from_demo(self, demo_id, index_in_demo, keys, num_frames_to_stack=0, seq_length=1, prefix="obs"):
         """
         Extract a (sub)sequence of observation items from a demo given the @keys of the items.
 
@@ -539,35 +540,35 @@
             num_frames_to_stack=num_frames_to_stack,
             seq_length=seq_length,
         )
         obs = {k.split('/')[1]: obs[k] for k in obs}  # strip the prefix
         if self.get_pad_mask:
             obs["pad_mask"] = pad_mask
 
-        # prepare image observations from dataset
-        return ObsUtils.process_obs_dict(obs)
+        return obs
 
-    def get_dataset_sequence_from_demo(self, demo_id, index_in_demo, keys, seq_length=1):
+    def get_dataset_sequence_from_demo(self, demo_id, index_in_demo, keys, num_frames_to_stack=0, seq_length=1):
         """
         Extract a (sub)sequence of dataset items from a demo given the @keys of the items (e.g., states, actions).
         
         Args:
             demo_id (str): id of the demo, e.g., demo_0
             index_in_demo (int): beginning index of the sequence wrt the demo
             keys (tuple): list of keys to extract
+            num_frames_to_stack (int): numbers of frame to stack. Seq gets prepended with repeated items if out of range
             seq_length (int): sequence length to extract. Seq gets post-pended with repeated items if out of range
 
         Returns:
             a dictionary of extracted items.
         """
         data, pad_mask = self.get_sequence_from_demo(
             demo_id,
             index_in_demo=index_in_demo,
             keys=keys,
-            num_frames_to_stack=0,  # don't frame stack for meta keys
+            num_frames_to_stack=num_frames_to_stack,
             seq_length=seq_length,
         )
         if self.get_pad_mask:
             data["pad_mask"] = pad_mask
         return data
 
     def get_trajectory_at_index(self, index):
@@ -578,14 +579,15 @@
         demo_id = self.demos[index]
         demo_length = self._demo_id_to_demo_length[demo_id]
 
         meta = self.get_dataset_sequence_from_demo(
             demo_id,
             index_in_demo=0,
             keys=self.dataset_keys,
+            num_frames_to_stack=self.n_frame_stack - 1, # note: need to decrement self.n_frame_stack by one
             seq_length=demo_length
         )
         meta["obs"] = self.get_obs_sequence_from_demo(
             demo_id,
             index_in_demo=0,
             keys=self.obs_keys,
             seq_length=demo_length
```

### Comparing `robomimic-0.2.0/robomimic/utils/env_utils.py` & `robomimic-0.3.0/robomimic/utils/env_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This file contains several utility functions for working with environment
 wrappers provided by the repository, and with environment metadata saved
 in dataset files.
 """
 from copy import deepcopy
 import robomimic.envs.env_base as EB
+from robomimic.utils.log_utils import log_warning
 
 
 def get_env_class(env_meta=None, env_type=None, env=None):
     """
     Return env class from either env_meta, env_type, or env.
     Note the use of lazy imports - this ensures that modules are only
     imported when the corresponding env type is requested. This can
@@ -91,14 +92,47 @@
 
         env (instance of EB.EnvBase): environment instance
     """
     env_type = get_env_type(env_meta=env_meta, env_type=env_type, env=env)
     return (env_type == type_to_check)
 
 
+def check_env_version(env, env_meta):
+    """
+    Checks whether the passed env and env_meta dictionary having matching environment versions.
+    Logs warning if cannot find version or versions do not match.
+
+    Args:
+        env (instance of EB.EnvBase): environment instance
+
+        env_meta (dict): environment metadata, which should be loaded from demonstration
+            hdf5 with @FileUtils.get_env_metadata_from_dataset or from checkpoint (see
+            @FileUtils.env_from_checkpoint). Contains following key:
+
+                :`'env_version'`: environment version, type str
+    """
+    env_system_version = env.version
+    env_meta_version = env_meta.get("env_version", None)
+
+    if env_meta_version is None:
+        log_warning(
+            "No environment version found in dataset!"\
+            "\nCannot verify if dataset and installed environment versions match"\
+        )
+    elif env_system_version != env_meta_version:
+        log_warning(
+            "Dataset and installed environment version mismatch!"\
+            "\nDataset environment version: {meta}"\
+            "\nInstalled environment version: {sys}".format(
+                sys=env_system_version,
+                meta=env_meta_version,
+            )
+        )
+
+
 def is_robosuite_env(env_meta=None, env_type=None, env=None):
     """
     Determines whether the environment is a robosuite environment. Accepts
     either env_meta, env_type, or env.
     """
     return check_env_type(type_to_check=EB.EnvType.ROBOSUITE_TYPE, env_meta=env_meta, env_type=env_type, env=env)
 
@@ -185,14 +219,15 @@
         env_type=env_type,
         env_name=env_name,  
         render=render, 
         render_offscreen=render_offscreen, 
         use_image_obs=use_image_obs, 
         **env_kwargs,
     )
+    check_env_version(env, env_meta)
     return env
 
 
 def create_env_for_data_processing(
     env_meta,
     camera_names, 
     camera_height, 
@@ -228,15 +263,29 @@
     env_kwargs = deepcopy(env_kwargs)
     env_kwargs.pop("env_name", None)
     env_kwargs.pop("camera_names", None)
     env_kwargs.pop("camera_height", None)
     env_kwargs.pop("camera_width", None)
     env_kwargs.pop("reward_shaping", None)
 
-    return env_class.create_for_data_processing(
+    env = env_class.create_for_data_processing(
         env_name=env_name, 
         camera_names=camera_names, 
         camera_height=camera_height, 
         camera_width=camera_width, 
         reward_shaping=reward_shaping, 
         **env_kwargs,
     )
+    check_env_version(env, env_meta)
+    return env
+
+
+def wrap_env_from_config(env, config):
+    """
+    Wraps environment using the provided Config object to determine which wrappers
+    to use (if any).
+    """
+    if config.train.frame_stack > 1:
+        from robomimic.envs.wrappers import FrameStackWrapper
+        env = FrameStackWrapper(env, num_frames=config.train.frame_stack)
+
+    return env
```

### Comparing `robomimic-0.2.0/robomimic/utils/file_utils.py` & `robomimic-0.3.0/robomimic/utils/file_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,14 +59,33 @@
         del f[k]
     f[k] = np.array(demo_keys, dtype='S')
 
     f.close()
     return ep_lengths
 
 
+def get_demos_for_filter_key(hdf5_path, filter_key):
+    """
+    Gets demo keys that correspond to a particular filter key.
+
+    Args:
+        hdf5_path (str): path to hdf5 file
+        filter_key (str): name of filter key
+
+    Returns:
+        demo_keys ([str]): list of demonstration keys that
+            correspond to this filter key. For example, ["demo_0", 
+            "demo_1"].
+    """
+    f = h5py.File(hdf5_path, "r")
+    demo_keys = [elem.decode("utf-8") for elem in np.array(f["mask/{}".format(filter_key)][:])]
+    f.close()
+    return demo_keys
+
+
 def get_env_metadata_from_dataset(dataset_path):
     """
     Retrieves env metadata from dataset.
 
     Args:
         dataset_path (str): path to dataset
 
@@ -195,14 +214,101 @@
             re-loading checkpoint from disk multiple times)
     """
     ckpt_dict = maybe_dict_from_checkpoint(ckpt_path=ckpt_path, ckpt_dict=ckpt_dict)
     algo_name = ckpt_dict["algo_name"]
     return algo_name, ckpt_dict
 
 
+def update_config(cfg):
+    """
+    Updates the config for backwards-compatibility if it uses outdated configurations.
+
+    See https://github.com/ARISE-Initiative/robomimic/releases/tag/v0.2.0 for more info.
+
+    Args:
+        cfg (dict): Raw dictionary of config values
+    """
+    # Check if image modality is defined -- this means we're using an outdated config
+    # Note: There may be a nested hierarchy, so we possibly check all the nested obs cfgs which can include
+    # e.g. a planner and actor for HBC
+
+    def find_obs_dicts_recursively(dic):
+        dics = []
+        if "modalities" in dic:
+            dics.append(dic)
+        else:
+            for child_dic in dic.values():
+                dics += find_obs_dicts_recursively(child_dic)
+        return dics
+
+    obs_cfgs = find_obs_dicts_recursively(cfg["observation"])
+    for obs_cfg in obs_cfgs:
+        modalities = obs_cfg["modalities"]
+
+        found_img = False
+        for modality_group in ("obs", "subgoal", "goal"):
+            if modality_group in modalities:
+                img_modality = modalities[modality_group].pop("image", None)
+                if img_modality is not None:
+                    found_img = True
+                    modalities[modality_group]["rgb"] = img_modality
+
+        if found_img:
+            # Also need to map encoder kwargs correctly
+            old_encoder_cfg = obs_cfg.pop("encoder")
+
+            # Create new encoder entry for RGB
+            rgb_encoder_cfg = {
+                "core_class": "VisualCore",
+                "core_kwargs": {
+                    "backbone_kwargs": dict(),
+                    "pool_kwargs": dict(),
+                },
+                "obs_randomizer_class": None,
+                "obs_randomizer_kwargs": dict(),
+            }
+
+            if "visual_feature_dimension" in old_encoder_cfg:
+                rgb_encoder_cfg["core_kwargs"]["feature_dimension"] = old_encoder_cfg["visual_feature_dimension"]
+
+            if "visual_core" in old_encoder_cfg:
+                rgb_encoder_cfg["core_kwargs"]["backbone_class"] = old_encoder_cfg["visual_core"]
+
+            for kwarg in ("pretrained", "input_coord_conv"):
+                if "visual_core_kwargs" in old_encoder_cfg and kwarg in old_encoder_cfg["visual_core_kwargs"]:
+                    rgb_encoder_cfg["core_kwargs"]["backbone_kwargs"][kwarg] = old_encoder_cfg["visual_core_kwargs"][kwarg]
+
+            # Optionally add pooling info too
+            if old_encoder_cfg.get("use_spatial_softmax", True):
+                rgb_encoder_cfg["core_kwargs"]["pool_class"] = "SpatialSoftmax"
+
+            for kwarg in ("num_kp", "learnable_temperature", "temperature", "noise_std"):
+                if "spatial_softmax_kwargs" in old_encoder_cfg and kwarg in old_encoder_cfg["spatial_softmax_kwargs"]:
+                    rgb_encoder_cfg["core_kwargs"]["pool_kwargs"][kwarg] = old_encoder_cfg["spatial_softmax_kwargs"][kwarg]
+
+            # Update obs randomizer as well
+            for kwarg in ("obs_randomizer_class", "obs_randomizer_kwargs"):
+                if kwarg in old_encoder_cfg:
+                    rgb_encoder_cfg[kwarg] = old_encoder_cfg[kwarg]
+
+            # Store rgb config
+            obs_cfg["encoder"] = {"rgb": rgb_encoder_cfg}
+
+            # Also add defaults for low dim
+            obs_cfg["encoder"]["low_dim"] = {
+                "core_class": None,
+                "core_kwargs": {
+                    "backbone_kwargs": dict(),
+                    "pool_kwargs": dict(),
+                },
+                "obs_randomizer_class": None,
+                "obs_randomizer_kwargs": dict(),
+            }
+
+
 def config_from_checkpoint(algo_name=None, ckpt_path=None, ckpt_dict=None, verbose=False):
     """
     Helper function to restore config from a checkpoint file or loaded model dictionary.
 
     Args:
         algo_name (str): Algorithm name.
 
@@ -218,21 +324,23 @@
         ckpt_dict (dict): loaded checkpoint dictionary (convenient to avoid
             re-loading checkpoint from disk multiple times)
     """
     ckpt_dict = maybe_dict_from_checkpoint(ckpt_path=ckpt_path, ckpt_dict=ckpt_dict)
     if algo_name is None:
         algo_name, _ = algo_name_from_checkpoint(ckpt_dict=ckpt_dict)
 
+    # restore config from loaded model dictionary
+    config_dict = json.loads(ckpt_dict['config'])
+    update_config(cfg=config_dict)
+
     if verbose:
         print("============= Loaded Config =============")
-        print(ckpt_dict['config'])
+        print(json.dumps(config_dict, indent=4))
 
-    # restore config from loaded model dictionary
-    config_json = ckpt_dict['config']
-    config = config_factory(algo_name, dic=json.loads(config_json))
+    config = config_factory(algo_name, dic=config_dict)
 
     # lock config to prevent further modifications and ensure missing keys raise errors
     config.lock()
 
     return config, ckpt_dict
 
 
@@ -263,16 +371,15 @@
     # algo name and config from model dict
     algo_name, _ = algo_name_from_checkpoint(ckpt_dict=ckpt_dict)
     config, _ = config_from_checkpoint(algo_name=algo_name, ckpt_dict=ckpt_dict, verbose=verbose)
 
     # read config to set up metadata for observation modalities (e.g. detecting rgb observations)
     ObsUtils.initialize_obs_utils_with_config(config)
 
-    # env meta from model dict to get info needed to create model
-    env_meta = ckpt_dict["env_metadata"]
+    # shape meta from model dict to get info needed to create model
     shape_meta = ckpt_dict["shape_metadata"]
 
     # maybe restore observation normalization stats
     obs_normalization_stats = ckpt_dict.get("obs_normalization_stats", None)
     if obs_normalization_stats is not None:
         assert config.train.hdf5_normalize_obs
         for m in obs_normalization_stats:
@@ -331,14 +438,16 @@
     # create env from saved metadata
     env = EnvUtils.create_env_from_metadata(
         env_meta=env_meta, 
         render=render, 
         render_offscreen=render_offscreen,
         use_image_obs=shape_meta["use_images"],
     )
+    config, _ = config_from_checkpoint(algo_name=ckpt_dict["algo_name"], ckpt_dict=ckpt_dict, verbose=False)
+    env = EnvUtils.wrap_env_from_config(env, config=config) # apply environment warpper, if applicable
     if verbose:
         print("============= Loaded Environment =============")
         print(env)
     return env, ckpt_dict
 
 
 class DownloadProgressBar(tqdm):
```

### Comparing `robomimic-0.2.0/robomimic/utils/hyperparam_utils.py` & `robomimic-0.3.0/robomimic/utils/hyperparam_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,28 +12,39 @@
 
 
 class ConfigGenerator(object):
     """
     Useful class to keep track of hyperparameters to sweep, and to generate
     the json configs for each experiment run.
     """
-    def __init__(self, base_config_file, script_file):
+    def __init__(self, base_config_file, wandb_proj_name="debug", script_file=None, generated_config_dir=None):
         """
         Args:
             base_config_file (str): path to a base json config to use as a starting point
                 for the parameter sweep.
 
             script_file (str): script filename to write as output
         """
         assert isinstance(base_config_file, str)
         self.base_config_file = base_config_file
-        assert isinstance(script_file, str)
-        self.script_file = script_file
+        assert generated_config_dir is None or isinstance(generated_config_dir, str)
+        if generated_config_dir is not None:
+            generated_config_dir = os.path.expanduser(generated_config_dir)
+        self.generated_config_dir = generated_config_dir
+        assert script_file is None or isinstance(script_file, str)
+        if script_file is None:
+            self.script_file = os.path.join('~', 'tmp/tmpp.sh')
+        else:
+            self.script_file = script_file
+        self.script_file = os.path.expanduser(self.script_file)
         self.parameters = OrderedDict()
 
+        assert isinstance(wandb_proj_name, str)
+        self.wandb_proj_name = wandb_proj_name
+
     def add_param(self, key, name, group, values, value_names=None):
         """
         Add parameter to the hyperparameter sweep.
 
         Args:
             key (str): location of parameter in the config, using hierarchical key format
                 (ex. train/data = config.train.data)
@@ -185,18 +196,23 @@
         @self.base_config_file.
 
         Returns:
             json_paths (list): list of paths to created json files, one per experiment
         """
 
         # base directory for saving jsons
-        base_dir = os.path.abspath(os.path.dirname(self.base_config_file))
+        if self.generated_config_dir:
+            base_dir = self.generated_config_dir
+            if not os.path.exists(base_dir):
+                os.makedirs(base_dir)
+        else:
+            base_dir = os.path.abspath(os.path.dirname(self.base_config_file))
 
         # read base json
-        base_config = load_json(self.base_config_file)
+        base_config = load_json(self.base_config_file, verbose=False)
 
         # base exp name from this base config
         base_exp_name = base_config['experiment']['name']
 
         # use base json to determine the parameter ranges
         parameter_ranges, parameter_names = self._get_parameter_ranges()
 
@@ -225,31 +241,58 @@
 
             # copy old json, but override name, and parameter values
             json_dict = deepcopy(base_config)
             json_dict['experiment']['name'] = exp_name
             for k in parameter_ranges:
                 set_value_for_key(json_dict, k, v=parameter_ranges[k][i])
 
+            # populate list of identifying meta for logger;
+            # see meta_config method in base_config.py for more info
+            json_dict["experiment"]["logging"]["wandb_proj_name"] = self.wandb_proj_name
+            if "meta" not in json_dict:
+                json_dict["meta"] = dict()
+            json_dict["meta"].update(
+                hp_base_config_file=self.base_config_file,
+                hp_keys=list(),
+                hp_values=list(),
+            )
+            # logging: keep track of hyp param names and values as meta info
+            for k in parameter_ranges.keys():
+                key_name = self.parameters[k].name
+                if key_name is not None and len(key_name) > 0:
+                    if maybe_parameter_names[k] is not None:
+                        value_name = maybe_parameter_names[k]
+                    else:
+                        value_name = setting[k]
+            
+                    json_dict["meta"]["hp_keys"].append(key_name)
+                    json_dict["meta"]["hp_values"].append(value_name)
+
             # save file in same directory as old json
             json_path = os.path.join(base_dir, "{}.json".format(exp_name))
             save_json(json_dict, json_path)
             json_paths.append(json_path)
 
+        print("Num exps:", len(json_paths))
+
         return json_paths
 
     def _script_from_jsons(self, json_paths):
         """
         Generates a bash script to run the experiments that correspond to
         the input jsons.
         """
         with open(self.script_file, 'w') as f:
             f.write("#!/bin/bash\n\n")
             for path in json_paths:
                 # write python command to file
                 cmd = "python train.py --config {}\n".format(path)
+                
+                print()
+                print(cmd)
                 f.write(cmd)
 
 
 def load_json(json_file, verbose=True):
     """
     Simple utility function to load a json file as a dict.
```

### Comparing `robomimic-0.2.0/robomimic/utils/loss_utils.py` & `robomimic-0.3.0/robomimic/utils/loss_utils.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/robomimic/utils/obs_utils.py` & `robomimic-0.3.0/robomimic/utils/obs_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -922,15 +922,15 @@
         Args:
             obs (np.array or torch.Tensor): depth array
 
         Returns:
             unprocessed_obs (np.array or torch.Tensor): depth passed through
                 inverse operation of @process_depth
         """
-        return TU.to_uint8(unprocess_frame(frame=obs, channel_dim=1, scale=1.))
+        return unprocess_frame(frame=obs, channel_dim=1, scale=1.)
 
 
 class ScanModality(Modality):
     """
     Modality for scan observations
     """
     name = "scan"
```

### Comparing `robomimic-0.2.0/robomimic/utils/python_utils.py` & `robomimic-0.3.0/robomimic/utils/python_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Set of general purpose utility functions for easier interfacing with Python API
 """
 import inspect
 from copy import deepcopy
-import robomimic.utils.macros as Macros
+import robomimic.macros as Macros
 
 
 def get_class_init_kwargs(cls):
     """
     Helper function to return a list of all valid keyword arguments (excluding "self") for the given @cls class.
 
     Args:
```

### Comparing `robomimic-0.2.0/robomimic/utils/tensor_utils.py` & `robomimic-0.3.0/robomimic/utils/tensor_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,15 @@
 def reshape_dimensions_single(x, begin_axis, end_axis, target_dims):
     """
     Reshape selected dimensions in a tensor to a target dimension.
 
     Args:
         x (torch.Tensor): tensor to reshape
         begin_axis (int): begin dimension
-        end_axis (int): end dimension
+        end_axis (int): end dimension (inclusive)
         target_dims (tuple or list): target shape for the range of dimensions
             (@begin_axis, @end_axis)
 
     Returns:
         y (torch.Tensor): reshaped tensor
     """
     assert(begin_axis <= end_axis)
@@ -507,15 +507,15 @@
     """
     Reshape selected dimensions for all tensors in nested dictionary or list or tuple 
     to a target dimension.
     
     Args:
         x (dict or list or tuple): a possibly nested dictionary or list or tuple
         begin_axis (int): begin dimension
-        end_axis (int): end dimension
+        end_axis (int): end dimension (inclusive)
         target_dims (tuple or list): target shape for the range of dimensions
             (@begin_axis, @end_axis)
 
     Returns:
         y (dict or list or tuple): new nested dict-list-tuple
     """
     return recursive_dict_list_tuple_apply(
```

### Comparing `robomimic-0.2.0/robomimic/utils/test_utils.py` & `robomimic-0.3.0/robomimic/utils/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 def example_dataset_path():
     """
     Path to dataset to use for testing and example purposes. It should
     exist under the tests/assets directory, and will be downloaded 
     from a server if it does not exist.
     """
     dataset_folder = os.path.join(robomimic.__path__[0], "../tests/assets/")
-    dataset_path = os.path.join(dataset_folder, "test.hdf5")
+    dataset_path = os.path.join(dataset_folder, "test_v141.hdf5")
     if not os.path.exists(dataset_path):
         print("\nWARNING: test hdf5 does not exist! Downloading from server...")
         os.makedirs(dataset_folder, exist_ok=True)
         FileUtils.download_url(
-            url="http://downloads.cs.stanford.edu/downloads/rt_benchmark/test.hdf5", 
+            url="http://downloads.cs.stanford.edu/downloads/rt_benchmark/test_v141.hdf5", 
             download_dir=dataset_folder,
         )
     return dataset_path
 
 
 def example_momart_dataset_path():
     """
@@ -126,14 +126,18 @@
     # train and validate for 3 gradient steps
     config.experiment.name = "test"
     config.experiment.validate = True
     config.experiment.epoch_every_n_steps = 3
     config.experiment.validation_epoch_every_n_steps = 3
     config.train.num_epochs = 1
 
+    # default train and validation filter keys
+    config.train.hdf5_filter_key = "train"
+    config.train.hdf5_validation_filter_key = "valid"
+
     # ensure model saving, rollout, and offscreen video rendering are tested too
     config.experiment.save.enabled = True
     config.experiment.save.every_n_epochs = 1
     config.experiment.rollout.enabled = True
     config.experiment.rollout.rate = 1
     config.experiment.rollout.n = 1
     config.experiment.rollout.horizon = 10
```

### Comparing `robomimic-0.2.0/robomimic/utils/torch_utils.py` & `robomimic-0.3.0/robomimic/utils/torch_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,19 +97,29 @@
 
         net (torch.nn.Module): module whose parameters this optimizer will be
             responsible
 
     Returns:
         optimizer (torch.optim.Optimizer): optimizer
     """
-    return optim.Adam(
-        params=net.parameters(),
-        lr=net_optim_params["learning_rate"]["initial"],
-        weight_decay=net_optim_params["regularization"]["L2"],
-    )
+    optimizer_type = net_optim_params.get("optimizer_type", "adam")
+    lr = net_optim_params["learning_rate"]["initial"]
+
+    if optimizer_type == "adam":
+        return optim.Adam(
+            params=net.parameters(),
+            lr=lr,
+            weight_decay=net_optim_params["regularization"]["L2"],
+        )
+    elif optimizer_type == "adamw":
+        return optim.AdamW(
+            params=net.parameters(),
+            lr=lr,
+            weight_decay=net_optim_params["regularization"]["L2"],
+        )
 
 
 def lr_scheduler_from_optim_params(net_optim_params, net, optimizer):
     """
     Helper function to return a LRScheduler from the optim_params 
     section of the config for a particular network. Returns None
     if a scheduler is not needed.
@@ -122,22 +132,38 @@
             responsible
 
         optimizer (torch.optim.Optimizer): optimizer for this net
 
     Returns:
         lr_scheduler (torch.optim.lr_scheduler or None): learning rate scheduler
     """
+    lr_scheduler_type = net_optim_params["learning_rate"].get("scheduler_type", "multistep")
+    epoch_schedule = net_optim_params["learning_rate"]["epoch_schedule"]
+
     lr_scheduler = None
-    if len(net_optim_params["learning_rate"]["epoch_schedule"]) > 0:
-        # decay LR according to the epoch schedule
-        lr_scheduler = optim.lr_scheduler.MultiStepLR(
-            optimizer=optimizer,
-            milestones=net_optim_params["learning_rate"]["epoch_schedule"],
-            gamma=net_optim_params["learning_rate"]["decay_factor"],
-        )
+    if len(epoch_schedule) > 0:
+        if lr_scheduler_type == "linear":
+            assert len(epoch_schedule) == 1
+            end_epoch = epoch_schedule[0]
+            
+            return optim.lr_scheduler.LinearLR(
+                optimizer,
+                start_factor=1.0,
+                end_factor=net_optim_params["learning_rate"]["decay_factor"],
+                total_iters=end_epoch,
+            )
+        elif lr_scheduler_type == "multistep":
+            return optim.lr_scheduler.MultiStepLR(
+                optimizer=optimizer,
+                milestones=epoch_schedule,
+                gamma=net_optim_params["learning_rate"]["decay_factor"],
+            )
+        else:
+            raise ValueError("Invalid LR scheduler type: {}".format(lr_scheduler_type))
+        
     return lr_scheduler
 
 
 def backprop_for_loss(net, optim, loss, max_grad_norm=None, retain_graph=False):
     """
     Backpropagate loss and update parameters for network with
     name @name.
```

### Comparing `robomimic-0.2.0/robomimic/utils/train_utils.py` & `robomimic-0.3.0/robomimic/utils/train_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 from collections import OrderedDict
 
 import torch
 
 import robomimic
 import robomimic.utils.tensor_utils as TensorUtils
 import robomimic.utils.log_utils as LogUtils
+import robomimic.utils.file_utils as FileUtils
 
 from robomimic.utils.dataset import SequenceDataset
 from robomimic.envs.env_base import EnvBase
+from robomimic.envs.wrappers import EnvWrapper
 from robomimic.algo import RolloutPolicy
 
 
 def get_exp_dir(config, auto_remove_exp_dir=False):
     """
     Create experiment directory from config. If an identical experiment directory
     exists and @auto_remove_exp_dir is False (default), the function will prompt 
@@ -44,15 +46,15 @@
             to store rollout videos
     """
     # timestamp for directory names
     t_now = time.time()
     time_str = datetime.datetime.fromtimestamp(t_now).strftime('%Y%m%d%H%M%S')
 
     # create directory for where to dump model parameters, tensorboard logs, and videos
-    base_output_dir = config.train.output_dir
+    base_output_dir = os.path.expanduser(config.train.output_dir)
     if not os.path.isabs(base_output_dir):
         # relative paths are specified relative to robomimic module location
         base_output_dir = os.path.join(robomimic.__path__[0], base_output_dir)
     base_output_dir = os.path.join(base_output_dir, config.experiment.name)
     if os.path.exists(base_output_dir):
         if not auto_remove_exp_dir:
             ans = input("WARNING: model directory ({}) already exists! \noverwrite? (y/n)\n".format(base_output_dir))
@@ -89,28 +91,39 @@
 
     Returns:
         train_dataset (SequenceDataset instance): train dataset object
         valid_dataset (SequenceDataset instance): valid dataset object (only if using validation)
     """
 
     # config can contain an attribute to filter on
-    filter_by_attribute = config.train.hdf5_filter_key
+    train_filter_by_attribute = config.train.hdf5_filter_key
+    valid_filter_by_attribute = config.train.hdf5_validation_filter_key
+    if valid_filter_by_attribute is not None:
+        assert config.experiment.validate, "specified validation filter key {}, but config.experiment.validate is not set".format(valid_filter_by_attribute)
 
     # load the dataset into memory
     if config.experiment.validate:
         assert not config.train.hdf5_normalize_obs, "no support for observation normalization with validation data yet"
-        train_filter_by_attribute = "train"
-        valid_filter_by_attribute = "valid"
-        if filter_by_attribute is not None:
-            train_filter_by_attribute = "{}_{}".format(filter_by_attribute, train_filter_by_attribute)
-            valid_filter_by_attribute = "{}_{}".format(filter_by_attribute, valid_filter_by_attribute)
+        assert (train_filter_by_attribute is not None) and (valid_filter_by_attribute is not None), \
+            "did not specify filter keys corresponding to train and valid split in dataset" \
+            " - please fill config.train.hdf5_filter_key and config.train.hdf5_validation_filter_key"
+        train_demo_keys = FileUtils.get_demos_for_filter_key(
+            hdf5_path=os.path.expanduser(config.train.data),
+            filter_key=train_filter_by_attribute,
+        )
+        valid_demo_keys = FileUtils.get_demos_for_filter_key(
+            hdf5_path=os.path.expanduser(config.train.data),
+            filter_key=valid_filter_by_attribute,
+        )
+        assert set(train_demo_keys).isdisjoint(set(valid_demo_keys)), "training demonstrations overlap with " \
+            "validation demonstrations!"
         train_dataset = dataset_factory(config, obs_keys, filter_by_attribute=train_filter_by_attribute)
         valid_dataset = dataset_factory(config, obs_keys, filter_by_attribute=valid_filter_by_attribute)
     else:
-        train_dataset = dataset_factory(config, obs_keys, filter_by_attribute=filter_by_attribute)
+        train_dataset = dataset_factory(config, obs_keys, filter_by_attribute=train_filter_by_attribute)
         valid_dataset = None
 
     return train_dataset, valid_dataset
 
 
 def dataset_factory(config, obs_keys, filter_by_attribute=None, dataset_path=None):
     """
@@ -134,19 +147,19 @@
     if dataset_path is None:
         dataset_path = config.train.data
 
     ds_kwargs = dict(
         hdf5_path=dataset_path,
         obs_keys=obs_keys,
         dataset_keys=config.train.dataset_keys,
-        load_next_obs=True, # make sure dataset returns s'
-        frame_stack=1, # no frame stacking
+        load_next_obs=config.train.hdf5_load_next_obs, # whether to load next observations (s') from dataset
+        frame_stack=config.train.frame_stack,
         seq_length=config.train.seq_length,
-        pad_frame_stack=True,
-        pad_seq_length=True, # pad last obs per trajectory to ensure all sequences are sampled
+        pad_frame_stack=config.train.pad_frame_stack,
+        pad_seq_length=config.train.pad_seq_length,
         get_pad_mask=False,
         goal_mode=config.train.goal_mode,
         hdf5_cache_mode=config.train.hdf5_cache_mode,
         hdf5_use_swmr=config.train.hdf5_use_swmr,
         hdf5_normalize_obs=config.train.hdf5_normalize_obs,
         filter_by_attribute=filter_by_attribute
     )
@@ -186,15 +199,15 @@
 
         terminate_on_success (bool): if True, terminate episode early as soon as a success is encountered
 
     Returns:
         results (dict): dictionary containing return, success rate, etc.
     """
     assert isinstance(policy, RolloutPolicy)
-    assert isinstance(env, EnvBase)
+    assert isinstance(env, EnvBase) or isinstance(env, EnvWrapper)
 
     policy.start_episode()
 
     ob_dict = env.reset()
     goal_dict = None
     if use_goals:
         # retrieve goal from the environment
@@ -480,15 +493,15 @@
         assert config.train.hdf5_normalize_obs
         obs_normalization_stats = deepcopy(obs_normalization_stats)
         params["obs_normalization_stats"] = TensorUtils.to_list(obs_normalization_stats)
     torch.save(params, ckpt_path)
     print("save checkpoint to {}".format(ckpt_path))
 
 
-def run_epoch(model, data_loader, epoch, validate=False, num_steps=None):
+def run_epoch(model, data_loader, epoch, validate=False, num_steps=None, obs_normalization_stats=None):
     """
     Run an epoch of training or validation.
 
     Args:
         model (Algo instance): model to train
 
         data_loader (DataLoader instance): data loader that will be used to serve batches of data
@@ -498,14 +511,18 @@
 
         validate (bool): whether this is a training epoch or validation epoch. This tells the model
             whether to do gradient steps or purely do forward passes.
 
         num_steps (int): if provided, this epoch lasts for a fixed number of batches (gradient steps),
             otherwise the epoch is a complete pass through the training dataset
 
+        obs_normalization_stats (dict or None): if provided, this should map observation keys to dicts
+            with a "mean" and "std" of shape (1, ...) where ... is the default
+            shape for the observation.
+
     Returns:
         step_log_all (dict): dictionary of logged training metrics averaged across all batches
     """
     epoch_timestamp = time.time()
     if validate:
         model.set_eval()
     else:
@@ -530,14 +547,15 @@
             t = time.time()
             batch = next(data_loader_iter)
         timing_stats["Data_Loading"].append(time.time() - t)
 
         # process batch for training
         t = time.time()
         input_batch = model.process_batch_for_training(batch)
+        input_batch = model.postprocess_batch_for_training(input_batch, obs_normalization_stats=obs_normalization_stats)
         timing_stats["Process_Batch"].append(time.time() - t)
 
         # forward and backward pass
         t = time.time()
         info = model.train_on_batch(input_batch, epoch, validate=validate)
         timing_stats["Train_Batch"].append(time.time() - t)
```

### Comparing `robomimic-0.2.0/robomimic.egg-info/SOURCES.txt` & `robomimic-0.3.0/robomimic.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,89 +4,97 @@
 setup.py
 examples/add_new_modality.py
 examples/simple_config.py
 examples/simple_obs_nets.py
 examples/simple_train_loop.py
 examples/train_bc_rnn.py
 robomimic/__init__.py
+robomimic/macros.py
 robomimic.egg-info/PKG-INFO
 robomimic.egg-info/SOURCES.txt
 robomimic.egg-info/dependency_links.txt
 robomimic.egg-info/eager_resources.txt
 robomimic.egg-info/requires.txt
 robomimic.egg-info/top_level.txt
 robomimic/algo/__init__.py
 robomimic/algo/algo.py
 robomimic/algo/bc.py
 robomimic/algo/bcq.py
 robomimic/algo/cql.py
 robomimic/algo/gl.py
 robomimic/algo/hbc.py
+robomimic/algo/iql.py
 robomimic/algo/iris.py
 robomimic/algo/td3_bc.py
 robomimic/config/__init__.py
 robomimic/config/base_config.py
 robomimic/config/bc_config.py
 robomimic/config/bcq_config.py
 robomimic/config/config.py
 robomimic/config/cql_config.py
 robomimic/config/gl_config.py
 robomimic/config/hbc_config.py
+robomimic/config/iql_config.py
 robomimic/config/iris_config.py
 robomimic/config/td3_bc_config.py
 robomimic/envs/__init__.py
 robomimic/envs/env_base.py
 robomimic/envs/env_gym.py
 robomimic/envs/env_ig_momart.py
 robomimic/envs/env_robosuite.py
+robomimic/envs/wrappers.py
 robomimic/exps/templates/bc.json
 robomimic/exps/templates/bcq.json
 robomimic/exps/templates/cql.json
 robomimic/exps/templates/gl.json
 robomimic/exps/templates/hbc.json
+robomimic/exps/templates/iql.json
 robomimic/exps/templates/iris.json
 robomimic/exps/templates/td3_bc.json
 robomimic/models/__init__.py
 robomimic/models/base_nets.py
 robomimic/models/distributions.py
+robomimic/models/obs_core.py
 robomimic/models/obs_nets.py
 robomimic/models/policy_nets.py
+robomimic/models/transformers.py
 robomimic/models/vae_nets.py
 robomimic/models/value_nets.py
 robomimic/scripts/dataset_states_to_obs.py
 robomimic/scripts/download_datasets.py
 robomimic/scripts/download_momart_datasets.py
 robomimic/scripts/extract_obs_from_raw_datasets.sh
 robomimic/scripts/generate_config_templates.py
 robomimic/scripts/generate_paper_configs.py
 robomimic/scripts/get_dataset_info.py
 robomimic/scripts/hyperparam_helper.py
 robomimic/scripts/playback_dataset.py
 robomimic/scripts/run_trained_agent.py
+robomimic/scripts/setup_macros.py
 robomimic/scripts/split_train_val.py
 robomimic/scripts/train.py
 robomimic/scripts/conversion/convert_d4rl.py
 robomimic/scripts/conversion/convert_robosuite.py
 robomimic/scripts/conversion/convert_roboturk_pilot.py
 robomimic/utils/__init__.py
 robomimic/utils/dataset.py
 robomimic/utils/env_utils.py
 robomimic/utils/file_utils.py
 robomimic/utils/hyperparam_utils.py
 robomimic/utils/log_utils.py
 robomimic/utils/loss_utils.py
-robomimic/utils/macros.py
 robomimic/utils/obs_utils.py
 robomimic/utils/python_utils.py
 robomimic/utils/tensor_utils.py
 robomimic/utils/test_utils.py
 robomimic/utils/torch_utils.py
 robomimic/utils/train_utils.py
 robomimic/utils/vis_utils.py
 tests/test.sh
 tests/test_bc.py
 tests/test_bcq.py
 tests/test_cql.py
 tests/test_examples.py
 tests/test_hbc.py
+tests/test_iql.py
 tests/test_iris.py
 tests/test_scripts.py
```

### Comparing `robomimic-0.2.0/setup.py` & `robomimic-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,22 +21,23 @@
         "psutil",
         "tqdm",
         "termcolor",
         "tensorboard",
         "tensorboardX",
         "imageio",
         "imageio-ffmpeg",
+        "matplotlib",
         "egl_probe>=1.0.1",
         "torch",
         "torchvision",
     ],
     eager_resources=['*'],
     include_package_data=True,
     python_requires='>=3',
     description="robomimic: A Modular Framework for Robot Learning from Demonstration",
-    author="Ajay Mandlekar, Danfei Xu, Josiah Wong, Soroush Nasiriany, Chen Wang",
+    author="Ajay Mandlekar, Danfei Xu, Josiah Wong, Soroush Nasiriany, Chen Wang, Matthew Bronars",
     url="https://github.com/ARISE-Initiative/robomimic",
     author_email="amandlek@cs.stanford.edu",
-    version="0.2.0",
+    version="0.3.0",
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `robomimic-0.2.0/tests/test_bc.py` & `robomimic-0.3.0/tests/test_bc.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,31 @@
     config.algo.gmm.enabled = True
     config.algo.rnn.enabled = True
     config.algo.rnn.horizon = 10
     config.train.seq_length = 10
     return config
 
 
+@register_mod("bc-transformer")
+def bc_transformer_modifier(config):
+    config.algo.transformer.enabled = True
+    config.train.frame_stack = 10
+    config.train.seq_length = 1
+    return config
+
+
+@register_mod("bc-transformer-gmm")
+def bc_transformer_gmm_modifier(config):
+    config.algo.gmm.enabled = True
+    config.algo.transformer.enabled = True
+    config.train.frame_stack = 10
+    config.train.seq_length = 1
+    return config
+
+
 # add image version of all tests
 image_modifiers = OrderedDict()
 for test_name in MODIFIERS:
     lst = test_name.split("-")
     name = "-".join(lst[:1] + ["rgb"] + lst[1:])
     image_modifiers[name] = make_image_modifier(MODIFIERS[test_name])
 MODIFIERS.update(image_modifiers)
```

### Comparing `robomimic-0.2.0/tests/test_bcq.py` & `robomimic-0.3.0/tests/test_bcq.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/tests/test_cql.py` & `robomimic-0.3.0/tests/test_cql.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/tests/test_examples.py` & `robomimic-0.3.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/tests/test_hbc.py` & `robomimic-0.3.0/tests/test_hbc.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/tests/test_iris.py` & `robomimic-0.3.0/tests/test_iris.py`

 * *Files identical despite different names*

### Comparing `robomimic-0.2.0/tests/test_scripts.py` & `robomimic-0.3.0/tests/test_scripts.py`

 * *Files identical despite different names*

