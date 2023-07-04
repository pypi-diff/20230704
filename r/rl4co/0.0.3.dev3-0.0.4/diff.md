# Comparing `tmp/rl4co-0.0.3.dev3.tar.gz` & `tmp/rl4co-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl4co-0.0.3.dev3.tar", last modified: Wed Jun 21 19:57:20 2023, max compression
+gzip compressed data, was "rl4co-0.0.4.tar", last modified: Tue Jul  4 17:10:46 2023, max compression
```

## Comparing `rl4co-0.0.3.dev3.tar` & `rl4co-0.0.4.tar`

### file list

```diff
@@ -1,125 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.060481 rl4co-0.0.3.dev3/rl4co/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.064481 rl4co-0.0.3.dev3/rl4co/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/data/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/atsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/cvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/dpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/ffsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/mdpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/mtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/op.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/pctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/pdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/sdvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/envs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/nn/
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/env_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/env_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/flash_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/nn/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/graph/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/graph/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/graph/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.060481 rl4co-0.0.3.dev3/rl4co/models/rl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/rl/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/ppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/ppo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.068481 rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.060481 rl4co-0.0.3.dev3/rl4co/models/zoo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/am/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/am/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/am/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/am/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/am/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ham/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.072481 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.076481 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.076481 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.076481 rl4co-0.0.3.dev3/rl4co/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/tasks/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/tasks/rl4co.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/rl4co/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/rl4co/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/callbacks/speed_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/rl4co/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/download/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/download/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/download/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/instantiators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/param_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/pylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/rl4co/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.064481 rl4co-0.0.3.dev3/rl4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 19:57:20.000000 rl4co-0.0.3.dev3/rl4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:57:20.080481 rl4co-0.0.3.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 19:57:07.000000 rl4co-0.0.3.dev3/tests/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.976010 rl4co-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-04 17:10:36.000000 rl4co-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-04 17:10:46.976010 rl4co-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-04 17:10:36.000000 rl4co-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-04 17:10:36.000000 rl4co-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/data/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/atsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/envs/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15278 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/cvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/dpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/ffsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/mdpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/mtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/pctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/sdvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/spctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/env_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/env_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/flash_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/nn/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/graph/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/graph/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/graph/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.960010 rl4co-0.0.4/rl4co/models/rl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/rl/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/ppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/ppo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/rl/reinforce/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/reinforce/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/reinforce/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/reinforce/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.960010 rl4co-0.0.4/rl4co/models/zoo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/am/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/am/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/am/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/am/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/am/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/amppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/amppo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/amppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/amppo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/ham/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/mdam/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/pomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/models/zoo/ptrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/models/zoo/symnco/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/tasks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/tasks/rl4co.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/callbacks/speed_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/download/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/download/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/download/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/param_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/pylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:10:46.976010 rl4co-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.976010 rl4co-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-04 17:10:36.000000 rl4co-0.0.4/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-04 17:10:36.000000 rl4co-0.0.4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-04 17:10:36.000000 rl4co-0.0.4/tests/test_ops.py
```

### Comparing `rl4co-0.0.3.dev3/LICENSE` & `rl4co-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/PKG-INFO` & `rl4co-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.3.dev3
+Version: 0.0.4
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/kaist-silab/rl4co
 Project-URL: Bug Tracker, https://github.com/kaist-silab/rl4co/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: graph
@@ -221,26 +221,32 @@
 Provides-Extra: linting
 License-File: LICENSE
 
 <div align="center">
 
 # RL4CO
 
-An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
 
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
-<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
 [![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
+[**Documentation**](https://rl4co.readthedocs.io/) |  [**Getting Started**](#getting-started) | [**Usage**](#usage) | [**Contributing**](#contributing) | [**Paper**](https://arxiv.org/abs/2306.17100) | [**Citation**](#cite-us)
+
 </div>
 
+---
+
+
+An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
+
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
 - [TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily handle heterogeneous data such as states, actions and rewards
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
@@ -366,13 +372,32 @@
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
 
 ## Contributing
-Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO!
+[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls).
+If you would like to contribute, please check out our contribution guidelines   [here](.github/CONTRIBUTING.md). We welcome and look forward to all contributions to RL4CO!
+
+We are also on [Slack](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) if you have any questions or would like to discuss RL4CO with us. We are open to collaborations and would love to hear from you 🚀
+
 
 ### Contributors
 <a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
 </a>
+
+## Cite us
+If you find RL4CO valuable for your research or applied projects:
+
+```bibtex
+@article{berto2023rl4co,
+    title = {{RL4CO}: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark},
+    author={Federico Berto and Chuanbo Hua and Junyoung Park and Minsu Kim and Hyeonah Kim and Jiwoo Son and Haeyeon Kim and Joungho Kim and Jinkyoo Park},
+    journal={arXiv preprint arXiv:2306.17100},
+    year={2023},
+    url = {https://github.com/kaist-silab/rl4co}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rl4co-0.0.3.dev3/README.md` & `rl4co-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 <div align="center">
 
 # RL4CO
 
-An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
 
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
-<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
 [![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
+[**Documentation**](https://rl4co.readthedocs.io/) |  [**Getting Started**](#getting-started) | [**Usage**](#usage) | [**Contributing**](#contributing) | [**Paper**](https://arxiv.org/abs/2306.17100) | [**Citation**](#cite-us)
+
 </div>
 
+---
+
+
+An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
+
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
 - [TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily handle heterogeneous data such as states, actions and rewards
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
@@ -143,13 +149,32 @@
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
 
 ## Contributing
-Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO!
+[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls).
+If you would like to contribute, please check out our contribution guidelines   [here](.github/CONTRIBUTING.md). We welcome and look forward to all contributions to RL4CO!
+
+We are also on [Slack](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) if you have any questions or would like to discuss RL4CO with us. We are open to collaborations and would love to hear from you 🚀
+
 
 ### Contributors
 <a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
-</a>
+</a>
+
+## Cite us
+If you find RL4CO valuable for your research or applied projects:
+
+```bibtex
+@article{berto2023rl4co,
+    title = {{RL4CO}: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark},
+    author={Federico Berto and Chuanbo Hua and Junyoung Park and Minsu Kim and Hyeonah Kim and Jiwoo Son and Haeyeon Kim and Joungho Kim and Jinkyoo Park},
+    journal={arXiv preprint arXiv:2306.17100},
+    year={2023},
+    url = {https://github.com/kaist-silab/rl4co}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,44 +1,49 @@
-# RL4CO An extensive Reinforcement Learning (RL) for Combinatorial Optimization
-  (CO) benchmark. Our goal is to provide a unified framework for RL-based CO
- algorithms, and to facilitate reproducible research in this field, decoupling
-   the science from the engineering. [PyTorch] [Lightning] [base:_TorchRL]_
-      [config:_Hydra]_[![Code_style:_black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black)_![license](https:
-   //img.shields.io/badge/license-Apache%202.0-green.svg?)[![PyPI](https://
-  img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)_[!
-   [Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/
-badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)_
-RL4CO is built upon: - [TorchRL](https://github.com/pytorch/rl): official
-PyTorch framework for RL algorithms and vectorized environments on GPUs -
-[TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily
-handle heterogeneous data such as states, actions and rewards - [PyTorch
-Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch
-wrapper for high-performance AI research - [Hydra](https://github.com/
-facebookresearch/hydra): a framework for elegantly configuring complex
-applications ![image](https://github.com/kaist-silab/rl4co/assets/48984123/
-0db4efdd-1c93-4991-8f09-f3c6c1f35d60) ## Getting started [Open_In_Colab] RL4CO
-is now available for installation on `pip`! ```bash pip install rl4co ``` ###
-Local install and development If you want to develop RL4CO or access the latest
-builds, we recommend you to install it locally with `pip` in editable mode:
-```bash git clone https://github.com/kaist-silab/rl4co && cd rl4co pip install
--e . ```  [Optional] Automatically install PyTorch with correct CUDA version
-These commands will [automatically install](https://github.com/pmeier/light-
-the-torch) PyTorch with the right GPU version for your system: ```bash pip
-install light-the-torch python3 -m light_the_torch install -r --upgrade torch
-``` > Note: `conda` is also a good candidate for hassle-free installation of
-PyTorch: check out the [PyTorch website](https://pytorch.org/get-started/
-locally/) for more details.  To get started, we recommend checking out our
-[quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic
-example](#minimalistic-example) below. ## Usage Train model with default
-configuration (AM on TSP environment): ```bash python run.py ```  Change
-experiment Train model with chosen experiment configuration from [configs/
-experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
-```bash python run.py experiment=tsp/am env.num_loc=42 ```   Disable logging
-```bash python run.py experiment=test/am logger=none
+ # RL4CO [PyTorch] [Lightning] [base:_TorchRL]_[config:_Hydra]_[![Code_style:
+ black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://
+    github.com/psf/black)[![Slack](https://img.shields.io/badge/slack-chat-
+   611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-
+  1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)_![license](https://img.shields.io/badge/
+license-Apache%202.0-green.svg?)[Open_In_Colab][![PyPI](https://img.shields.io/
+  pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)_[![Test](https://
+ github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://
+github.com/kaist-silab/rl4co/actions/workflows/tests.yml)__[**Documentation**]
+ (https://rl4co.readthedocs.io/)_|_[**Getting_Started**](#getting-started)_|_
+[**Usage**](#usage)_|_[**Contributing**](#contributing)_|_[**Paper**](https://
+             arxiv.org/abs/2306.17100)_|_[**Citation**](#cite-us)
+--- An extensive Reinforcement Learning (RL) for Combinatorial Optimization
+(CO) benchmark. Our goal is to provide a unified framework for RL-based CO
+algorithms, and to facilitate reproducible research in this field, decoupling
+the science from the engineering. RL4CO is built upon: - [TorchRL](https://
+github.com/pytorch/rl): official PyTorch framework for RL algorithms and
+vectorized environments on GPUs - [TensorDict](https://github.com/pytorch-labs/
+tensordict): a library to easily handle heterogeneous data such as states,
+actions and rewards - [PyTorch Lightning](https://github.com/Lightning-AI/
+lightning): a lightweight PyTorch wrapper for high-performance AI research -
+[Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly
+configuring complex applications ![image](https://github.com/kaist-silab/rl4co/
+assets/48984123/0db4efdd-1c93-4991-8f09-f3c6c1f35d60) ## Getting started [Open
+In_Colab] RL4CO is now available for installation on `pip`! ```bash pip install
+rl4co ``` ### Local install and development If you want to develop RL4CO or
+access the latest builds, we recommend you to install it locally with `pip` in
+editable mode: ```bash git clone https://github.com/kaist-silab/rl4co && cd
+rl4co pip install -e . ```  [Optional] Automatically install PyTorch with
+correct CUDA version These commands will [automatically install](https://
+github.com/pmeier/light-the-torch) PyTorch with the right GPU version for your
+system: ```bash pip install light-the-torch python3 -m light_the_torch install
+-r --upgrade torch ``` > Note: `conda` is also a good candidate for hassle-free
+installation of PyTorch: check out the [PyTorch website](https://pytorch.org/
+get-started/locally/) for more details.  To get started, we recommend checking
+out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the
+[minimalistic example](#minimalistic-example) below. ## Usage Train model with
+default configuration (AM on TSP environment): ```bash python run.py ```
+Change experiment Train model with chosen experiment configuration from
+[configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with
+42 cities) ```bash python run.py experiment=tsp/am env.num_loc=42 ```   Disable
+logging ```bash python run.py experiment=test/am logger=none
 '~callbacks.learning_rate_monitor' ``` Note that `~` is used to disable a
 callback that would need a logger.   Create a sweep over hyperparameters (-
 m for multirun) ```bash python run.py -m experiment=tsp/am
 train.optimizer.lr=1e-3,1e-4,1e-5 ```  ### Minimalistic Example Here is a
 minimalistic example training the Attention Model with greedy rollout baseline
 on TSP in less than 50 lines of code: ```python from omegaconf import
 DictConfig import lightning as L from rl4co.envs import TSPEnv from
@@ -50,12 +55,25 @@
 trainer = L.Trainer( max_epochs=3, # only few epochs accelerator="gpu", # use
 GPU if available, else you can use others as "cpu" logger=None, # can replace
 with WandbLogger, TensorBoardLogger, etc. precision="16-mixed", # Lightning
 will handle faster training with mixed precision gradient_clip_val=1.0, # clip
 gradients to avoid exploding gradients reload_dataloaders_every_n_epochs=1, #
 necessary for sampling new data ) # Fit the model trainer.fit(lit_module) ```
 ### Testing Run tests with `pytest` from the root directory: ```bash pytest
-tests ``` ## Contributing Have a suggestion, request, or found a bug? Feel free
-to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a
-pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome
-contributions to RL4CO! ### Contributors [https://contrib.rocks/
-image?repo=kaist-silab/rl4co]
+tests ``` ## Contributing [![Slack](https://img.shields.io/badge/slack-chat-
+611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-
+1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) Have a suggestion, request, or found a bug?
+Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or
+[submit a pull request](https://github.com/kaist-silab/rl4co/pulls). If you
+would like to contribute, please check out our contribution guidelines [here]
+(.github/CONTRIBUTING.md). We welcome and look forward to all contributions to
+RL4CO! We are also on [Slack](https://join.slack.com/t/rl4co/shared_invite/zt-
+1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) if you have any questions or would like to
+discuss RL4CO with us. We are open to collaborations and would love to hear
+from you ð ### Contributors [https://contrib.rocks/image?repo=kaist-silab/
+rl4co] ## Cite us If you find RL4CO valuable for your research or applied
+projects: ```bibtex @article{berto2023rl4co, title = {{RL4CO}: an Extensive
+Reinforcement Learning for Combinatorial Optimization Benchmark}, author=
+{Federico Berto and Chuanbo Hua and Junyoung Park and Minsu Kim and Hyeonah Kim
+and Jiwoo Son and Haeyeon Kim and Joungho Kim and Jinkyoo Park}, journal={arXiv
+preprint arXiv:2306.17100}, year={2023}, url = {https://github.com/kaist-silab/
+rl4co} } ```
```

### Comparing `rl4co-0.0.3.dev3/pyproject.toml` & `rl4co-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 dynamic = ["version"]
 
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python"
 ]
 
 dependencies = [
```

### Comparing `rl4co-0.0.3.dev3/rl4co/data/dataset.py` & `rl4co-0.0.4/rl4co/data/dataset.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/data/generate_data.py` & `rl4co-0.0.4/rl4co/data/generate_data.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/data/utils.py` & `rl4co-0.0.4/rl4co/data/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/atsp.py` & `rl4co-0.0.4/rl4co/envs/atsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
-from rl4co.envs.base import RL4COEnvBase
-from rl4co.envs.utils import batch_to_scalar
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.envs.common.utils import batch_to_scalar
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class ATSPEnv(RL4COEnvBase):
     """
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/base.py` & `rl4co-0.0.4/rl4co/envs/common/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,36 +17,39 @@
     """Base class for RL4CO environments based on TorchRL EnvBase
 
     Args:
         data_dir (str): Root directory for the dataset
         train_file (str): Name of the training file
         val_file (str): Name of the validation file
         test_file (str): Name of the test file
+        check_solution (bool): Whether to check the validity of the solution at the end of the episode
         seed (int): Seed for the environment
         device (str): Device to use. Generally, no need to set as tensors are updated on the fly
     """
 
     batch_locked = False
 
     def __init__(
         self,
         *,
         data_dir: str = "data/",
         train_file: str = None,
         val_file: str = None,
         test_file: str = None,
+        check_solution: bool = True,
         seed: int = None,
         device: str = "cpu",
         **kwargs,
     ):
         super().__init__(device=device, batch_size=[])
         self.data_dir = data_dir
         self.train_file = pjoin(data_dir, train_file) if train_file is not None else None
         self.val_file = pjoin(data_dir, val_file) if val_file is not None else None
         self.test_file = pjoin(data_dir, test_file) if test_file is not None else None
+        self.check_solution = check_solution
         if seed is None:
             seed = torch.empty((), dtype=torch.int64).random_().item()
         self.set_seed(seed)
 
     def _step(self, td: TensorDict) -> TensorDict:
         """Step function to call at each step of the episode containing an action.
         Gives the next observation, reward, done
@@ -63,14 +66,26 @@
 
     def get_reward(self, td, actions) -> TensorDict:
         """Function to compute the reward. Can be called by the agent to compute the reward of the current state
         This is faster than calling step() and getting the reward from the returned TensorDict at each time for CO tasks
         """
         raise NotImplementedError
 
+    def get_action_mask(self, td: TensorDict) -> torch.Tensor:
+        """Function to compute the action mask (feasible actions) for the current state
+        Action mask is 1 if the action is feasible, 0 otherwise
+        """
+        raise NotImplementedError
+
+    def check_solution_validity(self, td, actions) -> TensorDict:
+        """Function to check whether the solution is valid. Can be called by the agent to check the validity of the current state
+        This is called with the full solution (i.e. all actions) at the end of the episode
+        """
+        raise NotImplementedError
+
     def dataset(self, batch_size=[], phase="train", filename=None):
         """Return a dataset of observations
         Generates the dataset if it does not exist, otherwise loads it from file
         """
         if filename is not None:
             log.info(f"Overriding dataset filename from {filename}")
         f = getattr(self, f"{phase}_file") if filename is None else filename
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/cvrp.py` & `rl4co-0.0.4/rl4co/envs/cvrp.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.data.utils import load_npz_to_tensordict
-from rl4co.envs import RL4COEnvBase
-from rl4co.utils.ops import gather_by_index
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.utils.ops import gather_by_index, get_tour_length
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 # From Kool et al. 2019, Hottung et al. 2022, Kim et al. 2023
 CAPACITIES = {
@@ -79,17 +79,15 @@
         if self.capacity is None:
             raise ValueError(
                 f"Capacity for {num_loc} locations is not defined. Please provide a capacity manually."
             )
         self.vehicle_capacity = vehicle_capacity
         self._make_spec(td_params)
 
-    @staticmethod
-    def _step(td: TensorDict) -> TensorDict:
-        # Update the state
+    def _step(self, td: TensorDict) -> TensorDict:
         current_node = td["action"][:, None]  # Add dimension for step
         n_loc = td["demand"].size(-1)  # Excludes depot
 
         # Not selected_demand is demand of first node (by clamp) so incorrect for nodes that visit depot!
         selected_demand = gather_by_index(
             td["demand"], torch.clamp(current_node - 1, 0, n_loc - 1), squeeze=False
         )
@@ -99,140 +97,89 @@
             current_node != 0
         ).float()
 
         # Note: here we do not subtract one as we have to scatter so the first column allows scattering depot
         # Add one dimension since we write a single value
         visited = td["visited"].scatter(-1, current_node[..., None], 1)
 
-        # SECTION: get mask
-        visited_loc = visited[..., 1:]
-
-        # For demand steps_dim is inserted by indexing with id, for used_capacity insert node dim for broadcasting
-        exceeds_cap = td["demand"][:, None, :] + used_capacity[..., None] > 1.0
-
-        # Nodes that cannot be visited are already visited or too much demand to be served now
-        mask_loc = visited_loc.to(exceeds_cap.dtype) | exceeds_cap
-
-        # Cannot visit the depot if just visited and still unserved nodes
-        mask_depot = (current_node == 0) & ((mask_loc == 0).int().sum(-1) > 0)
-
-        # Action mask will be inverse of unfeasible actions
-        feasible_actions = ~torch.cat((mask_depot[..., None], mask_loc), -1).squeeze(-2)
-
         # SECTION: get done
         done = visited.sum(-1) == visited.size(-1)
         reward = torch.ones_like(done) * float("-inf")
 
-        return TensorDict(
+        td_step = TensorDict(
             {
                 "next": {
                     "locs": td["locs"],
                     "demand": td["demand"],
                     "current_node": current_node,
                     "used_capacity": used_capacity,
                     "vehicle_capacity": td["vehicle_capacity"],
                     "visited": visited,
-                    "action_mask": feasible_actions,
                     "reward": reward,
                     "done": done,
                 }
             },
             td.shape,
         )
+        td_step["next"].set("action_mask", self.get_action_mask(td_step["next"]))
+        return td_step     
 
     def _reset(
         self,
         td: Optional[TensorDict] = None,
         batch_size: Optional[list] = None,
     ) -> TensorDict:
         if batch_size is None:
             batch_size = self.batch_size if td is None else td["locs"].shape[:-2]
 
         if td is None or td.is_empty():
             td = self.generate_data(batch_size=batch_size)
 
         self.device = td.device
 
-        locs = torch.cat((td["depot"][:, None, :], td["locs"]), -2)
-        current_node = torch.zeros(*batch_size, 1, dtype=torch.long, device=self.device)
-        used_capacity = torch.zeros((*batch_size, 1), device=self.device)
-
-        _, n_loc, _ = td["locs"].size()
-        visited = torch.zeros(
-            (*batch_size, 1, n_loc + 1), dtype=torch.uint8, device=self.device
+        # Create reset TensorDict
+        td_reset = TensorDict(
+            {
+                "locs": torch.cat((td["depot"][:, None, :], td["locs"]), -2),
+                "demand": td["demand"],
+                "current_node": torch.zeros(*batch_size, 1, dtype=torch.long, device=self.device),
+                "used_capacity":  torch.zeros((*batch_size, 1), device=self.device),
+                "vehicle_capacity": torch.full((*batch_size, 1), self.vehicle_capacity, device=self.device),
+                "visited": torch.zeros((*batch_size, 1, td["locs"].shape[-2] + 1), dtype=torch.uint8, device=self.device),
+            },
+            batch_size=batch_size,
         )
-
-        # SECTION: get mask
-        visited_loc = visited[..., 1:]
-
+        td_reset.set("action_mask", self.get_action_mask(td_reset))
+        return td_reset
+    
+    @staticmethod
+    def get_action_mask(td: TensorDict) -> torch.Tensor:
         # For demand steps_dim is inserted by indexing with id, for used_capacity insert node dim for broadcasting
-        exceeds_cap = td["demand"][:, None, :] + used_capacity[..., None] > 1.0
+        exceeds_cap = td["demand"][:, None, :] + td["used_capacity"][..., None] > 1.0
 
         # Nodes that cannot be visited are already visited or too much demand to be served now
-        mask_loc = visited_loc.to(exceeds_cap.dtype) | exceeds_cap
+        mask_loc = td["visited"][..., 1:].to(exceeds_cap.dtype) | exceeds_cap
 
         # Cannot visit the depot if just visited and still unserved nodes
-        mask_depot = (current_node == 0) & ((mask_loc == 0).int().sum(-1) > 0)
-        feasible_actions = ~torch.cat((mask_depot[..., None], mask_loc), -1).squeeze(-2)
-
-        # Vehicle capacity as a feature
-        vehicle_capacity = torch.full(
-            (*batch_size, 1), self.vehicle_capacity, device=self.device
-        )
+        mask_depot = (td["current_node"] == 0) & ((mask_loc == 0).int().sum(-1) > 0)
+        return ~torch.cat((mask_depot[..., None], mask_loc), -1).squeeze(-2)
 
-        return TensorDict(
-            {
-                "locs": locs,
-                "demand": td["demand"],
-                "current_node": current_node,
-                "used_capacity": used_capacity,
-                "vehicle_capacity": vehicle_capacity,
-                "visited": visited,
-                "action_mask": feasible_actions,
-            },
-            batch_size=batch_size,
-        )
+    def get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict:        
+        # Check that the solution is valid
+        if self.check_solution:
+            self.check_solution_validity(td, actions)
 
-    def _make_spec(self, td_params: TensorDict):
-        """Make the observation and action specs from the parameters."""
-        self.observation_spec = CompositeSpec(
-            locs=BoundedTensorSpec(
-                minimum=self.min_loc,
-                maximum=self.max_loc,
-                shape=(self.num_loc + 1, 2),
-                dtype=torch.float32,
-            ),
-            current_node=UnboundedDiscreteTensorSpec(
-                shape=(1),
-                dtype=torch.int64,
-            ),
-            demand=BoundedTensorSpec(
-                minimum=-self.capacity,
-                maximum=self.max_demand,
-                shape=(self.num_loc, 1),  # demand is only for customers
-                dtype=torch.float32,
-            ),
-            action_mask=UnboundedDiscreteTensorSpec(
-                shape=(self.num_loc + 1, 1),
-                dtype=torch.bool,
-            ),
-            shape=(),
-        )
-        self.input_spec = self.observation_spec.clone()
-        self.action_spec = BoundedTensorSpec(
-            shape=(1,),
-            dtype=torch.int64,
-            minimum=0,
-            maximum=self.num_loc + 1,
-        )
-        self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
-        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
+        # Gather dataset in order of tour
+        depot = td["locs"][..., 0:1, :]
+        locs_ordered = torch.cat([depot, gather_by_index(td["locs"], actions)], dim=1)
+        return -get_tour_length(locs_ordered)
 
     @staticmethod
-    def get_reward(td, actions) -> TensorDict:
+    def check_solution_validity(td: TensorDict, actions: torch.Tensor):
+        """Check that solution is valid: nodes are not visited twice except depot and capacity is not exceeded"""
         # Check if tour is valid, i.e. contain 0 to n-1
         batch_size, graph_size = td["demand"].size()
         sorted_pi = actions.data.sort(1)[0]
 
         # Sorting it should give all zeros at front and then 1...n
         assert (
             torch.arange(1, graph_size + 1, out=sorted_pi.data.new())
@@ -252,21 +199,14 @@
             ]  # This will reset/make capacity negative if i == 0, e.g. depot visited
             # Cannot use less than 0
             used_cap[used_cap < 0] = 0
             assert (
                 used_cap <= td["vehicle_capacity"] + 1e-5
             ).all(), "Used more than capacity"
 
-        # Calculate the reward: - distance from all locations.
-        # We add the depot as first so we calculate also depot-first and depot-last tours with roll
-        depot = td["locs"][..., 0:1, :]
-        loc_gathered = torch.cat([depot, gather_by_index(td["locs"], actions)], dim=1)
-        loc_gathered_next = torch.roll(loc_gathered, 1, dims=1)
-        return -((loc_gathered_next - loc_gathered).norm(p=2, dim=2).sum(1))
-
     def generate_data(self, batch_size) -> TensorDict:
         # Batch size input check
         batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
 
         # Initialize the locations (including the depot which is always the first node)
         locs_with_depot = (
             torch.FloatTensor(*batch_size, self.num_loc + 1, 2)
@@ -309,41 +249,81 @@
         """Dataset loading from file
         Normalize demand by capacity to be in [0, 1]
         """
         td_load = load_npz_to_tensordict(fpath)
         td_load.set_("demand", td_load["demand"] / td_load["capacity"][:, None])
         return td_load
 
+    def _make_spec(self, td_params: TensorDict):
+        """Make the observation and action specs from the parameters."""
+        self.observation_spec = CompositeSpec(
+            locs=BoundedTensorSpec(
+                minimum=self.min_loc,
+                maximum=self.max_loc,
+                shape=(self.num_loc + 1, 2),
+                dtype=torch.float32,
+            ),
+            current_node=UnboundedDiscreteTensorSpec(
+                shape=(1),
+                dtype=torch.int64,
+            ),
+            demand=BoundedTensorSpec(
+                minimum=-self.capacity,
+                maximum=self.max_demand,
+                shape=(self.num_loc, 1),  # demand is only for customers
+                dtype=torch.float32,
+            ),
+            action_mask=UnboundedDiscreteTensorSpec(
+                shape=(self.num_loc + 1, 1),
+                dtype=torch.bool,
+            ),
+            shape=(),
+        )
+        self.input_spec = self.observation_spec.clone()
+        self.action_spec = BoundedTensorSpec(
+            shape=(1,),
+            dtype=torch.int64,
+            minimum=0,
+            maximum=self.num_loc + 1,
+        )
+        self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
+        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
+
     @staticmethod
     def render(td: TensorDict, actions=None, ax=None):
         import matplotlib.pyplot as plt
         import numpy as np
 
         from matplotlib import cm, colormaps
 
-        base = colormaps["rainbow"]
-        color_list = base(np.linspace(0, 1, 6))
-        cmap_name = base.name + str(6)
-        out = base.from_list(cmap_name, color_list, 6)
+        num_routine = (actions == 0).sum().item() + 2
+        base = colormaps["nipy_spectral"]
+        color_list = base(np.linspace(0, 1, num_routine))
+        cmap_name = base.name + str(num_routine)
+        out = base.from_list(cmap_name, color_list, num_routine)
 
         if ax is None:
             # Create a plot of the nodes
             _, ax = plt.subplots()
 
         td = td.detach().cpu()
         # if batch_size greater than 0 , we need to select the first batch element
         if td.batch_size != torch.Size([]):
             td = td[0]
 
         locs = td["locs"]
-        demands = td["demand"]
+        scale = CAPACITIES.get(td['locs'].size(-2)-1, 1)
+        demands = td["demand"] * scale
 
         if actions is None:
             actions = td.get("action", None)
 
+        # add the depot at the first action and the end action
+        actions = torch.cat([torch.tensor([0]), actions, torch.tensor([0])])
+
         # gather locs in order of action if available
         if actions is None:
             log.warning("No action in TensorDict, rendering unsorted locs")
         else:
             locs = locs
 
         # Cat the first node to the end to complete the tour
@@ -363,27 +343,27 @@
 
         # plot visited nodes
         ax.scatter(
             x[1:],
             y[1:],
             edgecolors=cm.Set2(0),
             facecolors="none",
-            s=100,
+            s=50,
             linewidths=2,
             marker="o",
             alpha=1,
         )
 
         # plot demand bars
         for node_idx in range(1, len(locs)):
             ax.add_patch(
                 plt.Rectangle(
-                    (locs[node_idx, 0] - 0.005, locs[node_idx, 1] + 0.025),
+                    (locs[node_idx, 0] - 0.005, locs[node_idx, 1] + 0.015),
                     0.01,
-                    demands[node_idx - 1] * 0.1,
+                    demands[node_idx - 1]/(scale * 10),
                     edgecolor=cm.Set2(0),
                     facecolor=cm.Set2(0),
                     fill=True,
                 )
             )
 
         # text demand
@@ -416,27 +396,28 @@
                 color_idx += 1
             from_loc = locs[actions[action_idx]]
             to_loc = locs[actions[action_idx + 1]]
             ax.plot(
                 [from_loc[0], to_loc[0]],
                 [from_loc[1], to_loc[1]],
                 color=out(color_idx),
+                lw=1,
             )
             ax.annotate(
                 "",
                 xy=(to_loc[0], to_loc[1]),
                 xytext=(from_loc[0], from_loc[1]),
-                arrowprops=dict(arrowstyle="->", color=out(color_idx)),
+                arrowprops=dict(arrowstyle="-|>", color=out(color_idx)),
+                size=15,
                 annotation_clip=False,
             )
 
         # setup
         ax.set_xlim(-0.05, 1.05)
         ax.set_ylim(-0.05, 1.05)
-        ax.grid(axis="both", color="black", ls="--", alpha=0.1)
 
         # Set plot title and axis labels
         title_font = {"fontsize": 14}
         label_font = {"fontsize": 12}
         ax.set_title("CVRP Solution", fontdict=title_font)
         ax.set_xlabel("X Coordinate", fontdict=label_font)
         ax.set_ylabel("Y Coordinate", fontdict=label_font)
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/dpp.py` & `rl4co-0.0.4/rl4co/envs/dpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.data.utils import load_npz_to_tensordict
-from rl4co.envs.base import RL4COEnvBase
+from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.utils.download.downloader import download_url
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class DPPEnv(RL4COEnvBase):
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/ffsp.py` & `rl4co-0.0.4/rl4co/envs/ffsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
-from rl4co.envs import RL4COEnvBase
+from rl4co.envs.common.base import RL4COEnvBase
 
 
 class FFSPEnv(RL4COEnvBase):
     """Flexible Flow Shop Problem (FFSP) Environment
     Args:
 
     Note:
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/mdpp.py` & `rl4co-0.0.4/rl4co/envs/mdpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/mtsp.py` & `rl4co-0.0.4/rl4co/envs/mtsp.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
-from rl4co.envs.base import RL4COEnvBase
-from rl4co.envs.utils import batch_to_scalar
-from rl4co.utils.ops import distance, gather_by_index
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.envs.common.utils import batch_to_scalar
+from rl4co.utils.ops import get_distance, gather_by_index, get_tour_length
 
 
 class MTSPEnv(RL4COEnvBase):
     """Multiple Traveling Salesman Problem environment
     At each step, an agent chooses to visit a city. A maximum of `num_agents` agents can be employed to visit the cities.
     The cost can be defined in two ways:
         - `minmax`: (default) the reward is the maximum of the path lengths of all the agents
@@ -81,20 +81,20 @@
         # If done is True, then we make the depot available again, so that it will be selected as the next node with prob 1
         available[..., 0] = torch.logical_or(done, available[..., 0])
 
         # If current agent is different from previous agent, then we have a new subtour and reset the length, otherwise we add the new distance
         current_length = torch.where(
             cur_agent_idx != td["agent_idx"],
             torch.zeros_like(td["current_length"]),
-            td["current_length"] + distance(cur_loc, prev_loc),
+            td["current_length"] + get_distance(cur_loc, prev_loc),
         )
 
         # If done, we add the distance from the current_node to the depot as well
         current_length = torch.where(
-            done, current_length + distance(cur_loc, depot_loc), current_length
+            done, current_length + get_distance(cur_loc, depot_loc), current_length
         )
 
         # We update the max_subtour_length and reset the current_length
         max_subtour_length = torch.where(
             current_length > td["max_subtour_length"],
             current_length,
             td["max_subtour_length"],
@@ -219,19 +219,17 @@
         # With minmax, get the maximum distance among subtours, calculated in the model
         if self.cost_type == "minmax":
             return td["reward"].squeeze(-1)
 
         # With distance, same as TSP
         elif self.cost_type == "distance":
             locs = td["locs"]
-            locs = locs.gather(1, actions.unsqueeze(-1).expand_as(locs))
-            locs_next = torch.roll(
-                locs, 1, dims=1
-            )  # roll will also consider last node to depot
-            return -((locs_next - locs).norm(p=2, dim=2).sum(1))
+            locs_ordered = locs.gather(1, actions.unsqueeze(-1).expand_as(locs))
+            return -get_tour_length(locs_ordered)
+
         else:
             raise ValueError(f"Cost type {self.cost_type} not supported")
 
     def generate_data(self, batch_size) -> TensorDict:
         batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
 
         # Initialize the locations (including the depot which is always the first node)
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/op.py` & `rl4co-0.0.4/rl4co/envs/pdp.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,299 +6,299 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
-from rl4co.envs.base import RL4COEnvBase
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.utils.ops import gather_by_index, get_tour_length
 
-MAX_LENGTHS = {20: 2.0, 50: 3.0, 100: 4.0}
 
-
-class OPEnv(RL4COEnvBase):
-    """Orienteering Problem (OP) environment
-    At each step, the agent chooses a city to visit. The reward is the -infinite unless the agent visits all the cities.
+class PDPEnv(RL4COEnvBase):
+    """Pickup and Delivery Problem (PDP) environment
+    The environment is made of num_loc + 1 locations (cities):
+    - 1 depot
+    - num_loc / 2 pickup locations
+    - num_loc / 2 delivery locations
+    The goal is to visit all the pickup and delivery locations in the shortest path possible starting from the depot
+    The conditions is that the agent must visit a pickup location before visiting its corresponding delivery location
 
     Args:
-        - num_loc <int>: number of locations (cities) in the VRP. NOTE: the depot is included
-        - min_loc <float>: minimum value for the location coordinates
-        - max_loc <float>: maximum value for the location coordinates
-        - length_capacity <float>: capacity of the vehicle of length, i.e. the maximum length the vehicle can travel
-        - td_params <TensorDict>: parameters of the environment
-        - seed <int>: seed for the environment
-        - device <str>: 'cpu' or 'cuda:0', device to use.  Generally, no need to set as tensors are updated on the fly
-    Note:
-        - in our setting, the vehicle has to come back to the depot at the end
+        num_loc: number of locations (cities) in the TSP
+        td_params: parameters of the environment
+        seed: seed for the environment
+        device: device to use.  Generally, no need to set as tensors are updated on the fly
     """
 
-    name = "op"
+    name = "pdp"
 
     def __init__(
         self,
-        num_loc: int = 10,
+        num_loc: int = 20,
         min_loc: float = 0,
         max_loc: float = 1,
-        min_prize: float = 0.01,
-        max_prize: float = 1.01,
         td_params: TensorDict = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.num_loc = num_loc
         self.min_loc = min_loc
         self.max_loc = max_loc
-        self.min_prize = min_prize
-        self.max_prize = max_prize
-        self.length_capacity = MAX_LENGTHS[num_loc]
         self._make_spec(td_params)
 
-    def _step(self, td: TensorDict) -> TensorDict:
-        """Update the states of the environment
-        Args:
-            - td <TensorDict>: tensor dictionary containing with the action
-                - action <int> [batch_size, 1]: action to take
-        NOTE:
-            - the first node in de prize is larger than 0 or less than 0?
-            - this design is important. For now the design is LESS than 0
-        """
-        current_node = td["action"][..., None]
-        current_node_expand = current_node[..., None].repeat_interleave(2, dim=-1)
-        length_capacity = td["length_capacity"]
-        prize = td["prize"]
-        prize_collect = td["prize_collect"]
-
-        # Collect prize
-        prize_collect += torch.gather(prize, -1, current_node)
-
-        # Set the visited node prize to -1
-        prize.scatter_(-1, current_node, 0)
-
-        # Update the used length capacity
-        length_capacity -= (
-            torch.gather(td["locs"], -2, current_node_expand)
-            - torch.gather(
-                td["locs"],
-                -2,
-                td["current_node"][..., None].repeat_interleave(2, dim=-1),
-            )
-        ).norm(p=2, dim=-1)
+    @staticmethod
+    def _step(td: TensorDict) -> TensorDict:
+        current_node = td["action"].unsqueeze(-1)
+
+        num_loc = td["locs"].shape[-2] - 1  # except depot
+
+        # Pickup and delivery node pair of selected node
+        new_to_deliver = (current_node + num_loc // 2) % (num_loc + 1)
 
-        # Get the action mask, no zero prize nodes can be visited
-        action_mask = prize > 0
+        # Set available to 0 (i.e., we visited the node)
+        available = td["available"].scatter(
+            -1, current_node.expand_as(td["action_mask"]), 0
+        )
 
-        # Nodes distance exceeding length capacity cannot be visited
-        length_to_next_node = (
-            td["locs"] - torch.gather(td["locs"], -2, current_node_expand)
-        ).norm(p=2, dim=-1)
-        length_to_next_node_and_return = length_to_next_node + td["length_to_depot"]
-        action_mask = torch.logical_and(
-            action_mask, length_to_next_node_and_return <= length_capacity
+        to_deliver = td["to_deliver"].scatter(
+            -1, new_to_deliver.expand_as(td["to_deliver"]), 1
         )
 
-        # We are done if run out the lenght capacity, i.e. no available node to visit
-        done = torch.count_nonzero(action_mask.float(), dim=-1) <= 1e-5
+        # Action is feasible if the node is not visited and is to deliver
+        # action_mask = torch.logical_and(available, to_deliver)
+        action_mask = available & to_deliver
 
-        # If done, then set the depot be always available
-        action_mask[..., 0] = torch.logical_or(action_mask[..., 0], done)
+        # We are done there are no unvisited locations
+        done = torch.count_nonzero(available, dim=-1) == 0
 
-        # Calculate reward (minus length of path, since we want to maximize the reward -> minimize the path length)
-        # Note: reward is calculated outside for now via the get_reward function
-        # to calculate here need to pass action sequence or save it as state
+        # The reward is calculated outside via get_reward for efficiency, so we set it to -inf here
         reward = torch.ones_like(done) * float("-inf")
 
         # The output must be written in a ``"next"`` entry
         return TensorDict(
             {
                 "next": {
                     "locs": td["locs"],
-                    "length_capacity": td["length_capacity"],
-                    "length_to_depot": td["length_to_depot"],
                     "current_node": current_node,
-                    "prize": prize,
-                    "prize_collect": prize_collect,
+                    "available": available,
+                    "to_deliver": to_deliver,
+                    "i": td["i"] + 1,
                     "action_mask": action_mask,
                     "reward": reward,
                     "done": done,
                 }
             },
             td.shape,
         )
 
     def _reset(self, td: Optional[TensorDict] = None, batch_size=None) -> TensorDict:
-        """
-        Args:
-            - td (Optional) <TensorDict>: tensor dictionary containing the initial state
-        """
         if batch_size is None:
-            batch_size = self.batch_size if td is None else td["prize"].shape[:-1]
+            batch_size = self.batch_size if td is None else td.batch_size
+
         if td is None or td.is_empty():
             td = self.generate_data(batch_size=batch_size)
-        device = td.device
 
-        observation = torch.cat([td["depot"][..., None, :], td["locs"]], dim=-2)
-        prize_depot = torch.zeros((*batch_size, 1), device=device)
-        prize = torch.cat([prize_depot, td["prize"]], dim=-1)
+        self.device = td.device
 
-        # Initialize the current node
-        current_node = torch.zeros((*batch_size, 1), dtype=torch.int64, device=device)
+        locs = torch.cat((td["depot"][:, None, :], td["locs"]), -2)
 
-        # Initialize the capacity
-        length_capacity = torch.full(
-            (*batch_size, 1), self.length_capacity, dtype=torch.float32, device=device
-        )
-
-        # Calculate the lenght of each node back to the depot
-        length_to_depot = (observation - td["depot"][..., None, :]).norm(p=2, dim=-1)
-
-        # Init the action mask
-        action_mask = prize > 1e-5
-
-        # Calculate the distance of each node at this moment
-        current_node_loccation = torch.gather(
-            observation, -2, current_node[..., None].repeat_interleave(2, dim=-1)
-        )
-        length_to_next_node = (observation - current_node_loccation).norm(p=2, dim=-1)
-        length_to_next_node_and_return = length_to_next_node + length_to_depot
-        action_mask = torch.logical_and(
-            action_mask, length_to_next_node_and_return <= length_capacity
+        # Pick is 1, deliver is 0 [batch_size, graph_size+1], [1,1...1, 0...0]
+        to_deliver = torch.cat(
+            [
+                torch.ones(
+                    *batch_size,
+                    self.num_loc // 2 + 1,
+                    dtype=torch.bool,
+                    device=self.device,
+                ),
+                torch.zeros(
+                    *batch_size, self.num_loc // 2, dtype=torch.bool, device=self.device
+                ),
+            ],
+            dim=-1,
+        )
+
+        # Cannot visit depot at first step # [0,1...1] so set not available
+        available = torch.ones(
+            (*batch_size, self.num_loc + 1), dtype=torch.bool, device=self.device
+        )
+        action_mask = ~available.contiguous()  # [batch_size, graph_size+1]
+        action_mask[..., 0] = 1  # First step is always the depot
+
+        # Other variables
+        current_node = torch.zeros(
+            (*batch_size, 1), dtype=torch.int64, device=self.device
         )
+        i = torch.zeros((*batch_size, 1), dtype=torch.int64, device=self.device)
 
         return TensorDict(
             {
-                "locs": observation,
-                "length_capacity": length_capacity,
-                "length_to_depot": length_to_depot,
+                "locs": locs,
                 "current_node": current_node,
-                "prize": prize,
-                "prize_collect": torch.zeros_like(length_capacity),
+                "to_deliver": to_deliver,
+                "available": available,
+                "i": i,
                 "action_mask": action_mask,
             },
             batch_size=batch_size,
         )
 
-    def _make_spec(self, td_params: TensorDict = None):
+    def _make_spec(self, td_params: TensorDict):
         """Make the observation and action specs from the parameters."""
         self.observation_spec = CompositeSpec(
             locs=BoundedTensorSpec(
                 minimum=self.min_loc,
                 maximum=self.max_loc,
-                shape=(self.num_loc, 2),
+                shape=(self.num_loc + 1, 2),
                 dtype=torch.float32,
             ),
-            length_capacity=BoundedTensorSpec(
-                minimum=0,
-                maximum=self.length_capacity,
+            current_node=UnboundedDiscreteTensorSpec(
                 shape=(1),
-                dtype=torch.float32,
+                dtype=torch.int64,
             ),
-            length_to_depot=BoundedTensorSpec(
-                minimum=0,
-                maximum=self.length_capacity,
+            to_deliver=UnboundedDiscreteTensorSpec(
                 shape=(1),
-                dtype=torch.float32,
+                dtype=torch.int64,
             ),
-            current_node=UnboundedDiscreteTensorSpec(
+            i=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
-            prize=BoundedTensorSpec(
-                minimum=-1,
-                maximum=self.max_prize,
-                shape=(self.num_loc),
-                dtype=torch.float32,
-            ),
-            prize_collect=UnboundedContinuousTensorSpec(
-                shape=(self.num_loc),
-                dtype=torch.float32,
-            ),
             action_mask=UnboundedDiscreteTensorSpec(
-                shape=(self.num_loc),
+                shape=(self.num_loc + 1),
                 dtype=torch.bool,
             ),
             shape=(),
         )
         self.input_spec = self.observation_spec.clone()
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             minimum=0,
-            maximum=self.num_loc,
+            maximum=self.num_loc + 1,
         )
-        self.reward_spec = UnboundedContinuousTensorSpec()
-        self.done_spec = UnboundedDiscreteTensorSpec(dtype=torch.bool)
+        self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
+        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
 
-    def get_reward(self, td, actions) -> TensorDict:
-        """Function to compute the reward. Can be called by the agent to compute the reward of the current state
-        This is faster than calling step() and getting the reward from the returned TensorDict at each time for CO tasks
-        """
-        # Check that tours are valid, i.e. contain 0 to n -1
-        sorted_actions = actions.data.sort(1)[0]
-        # Make sure each node visited once at most (except for depot)
+    @staticmethod
+    def get_reward(td, actions) -> TensorDict:
+        # assert (actions[:, 0] == 0).all(), "Not starting at depot"
         assert (
-            (sorted_actions[:, 1:] == 0)
-            | (sorted_actions[:, 1:] > sorted_actions[:, :-1])
-        ).all(), "Duplicates"
-
-        d = td["locs"].gather(
-            1, actions[..., None].expand(*actions.size(), td["locs"].size(-1))
-        )
-        length = (
-            (d[:, 1:] - d[:, :-1]).norm(p=2, dim=-1).sum(1)  # Prevent error if len 1 seq
-            + (d[:, 0] - td["locs"][..., 0, :]).norm(p=2, dim=-1)  # Depot to first
-            + (d[:, -1] - td["locs"][..., 0, :]).norm(
-                p=2, dim=-1
-            )  # Last to depot, will be 0 if depot is last
-        )
+            torch.arange(actions.size(1), out=actions.data.new())
+            .view(1, -1)
+            .expand_as(actions)
+            == actions.data.sort(1)[0]
+        ).all(), "Not visiting all nodes"
+
+        visited_time = torch.argsort(
+            actions, 1
+        )  # index of pickup less than index of delivery
         assert (
-            length <= self.length_capacity + 1e-5
-        ).all(), "Max length exceeded by {}".format(
-            (length - td["length_capacity"]).max()
-        )
-
-        return td["prize_collect"].squeeze(-1)
-
-    def generate_data(self, batch_size):
-        """
-        Args:
-            - batch_size <int> or <list>: batch size
-        Returns:
-            - td <TensorDict>: tensor dictionary containing the initial state
-                - locs <Tensor> [batch_size, num_loc, 2]: locations of the nodes
-                - prize <Tensor> [batch_size, num_loc]: prize of the nodes
-                - capacity <Tensor> [batch_size, 1]: capacity of the vehicle
-                - current_node <Tensor> [batch_size, 1]: current node
-                - i <Tensor> [batch_size, 1]: number of visited nodes
-        NOTE:
-            - the locs includes the depot as the first node
-            - the prize includes the used capacity at the first value
-            - the unvisited variable can be replaced by prize > 0
-        """
-        # Batch size input check
+            visited_time[:, 1 : actions.size(1) // 2 + 1]
+            < visited_time[:, actions.size(1) // 2 + 1 :]
+        ).all(), "Deliverying without pick-up"
+
+        # Gather locations in the order of actions and get reward = -(total distance)
+        locs_ordered = gather_by_index(td["locs"], actions)  # [batch, graph_size+1, 2]
+        return -get_tour_length(locs_ordered)
+
+    def generate_data(self, batch_size) -> TensorDict:
         batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
 
         # Initialize the locations (including the depot which is always the first node)
-        locs = (
+        locs_with_depot = (
             torch.FloatTensor(*batch_size, self.num_loc + 1, 2)
             .uniform_(self.min_loc, self.max_loc)
             .to(self.device)
         )
 
-        # Initialize the prize
-        prize_ = (locs[..., :1, :] - locs[..., 1:, :]).norm(p=2, dim=-1)
-        prize = (
-            1 + (prize_ / prize_.max(dim=-1, keepdim=True)[0] * 99).int()
-        ).float() / 100.0
-
         return TensorDict(
             {
-                "locs": locs[..., 1:, :],
-                "depot": locs[..., 0, :],
-                "prize": prize,
+                "locs": locs_with_depot[..., 1:, :],
+                "depot": locs_with_depot[..., 0, :],
             },
             batch_size=batch_size,
         )
 
-    def render(self, td):
-        # TODO
-        """Render the environment"""
-        raise NotImplementedError
+    @staticmethod
+    def render(td, actions=None):
+        import matplotlib.pyplot as plt
+
+        markersize = 8
+
+        td = td.detach().cpu()
+        # if batch_size greater than 0 , we need to select the first batch element
+        if td.batch_size != torch.Size([]):
+            td = td[0]
+            if actions is not None:
+                actions = actions[0]
+
+        # Variables
+        init_deliveries = td["to_deliver"][1:]
+        delivery_locs = td["locs"][1:][~init_deliveries.bool()]
+        pickup_locs = td["locs"][1:][init_deliveries.bool()]
+        depot_loc = td["locs"][0]
+        actions = actions if actions is not None else td["action"]
+
+        fig, ax = plt.subplots()
+
+        # Plot the actions in order
+        for i in range(len(actions)):
+            from_node = actions[i]
+            to_node = (
+                actions[i + 1] if i < len(actions) - 1 else actions[0]
+            )  # last goes back to depot
+            from_loc = td["locs"][from_node]
+            to_loc = td["locs"][to_node]
+            ax.plot([from_loc[0], to_loc[0]], [from_loc[1], to_loc[1]], "k-")
+            ax.annotate(
+                "",
+                xy=(to_loc[0], to_loc[1]),
+                xytext=(from_loc[0], from_loc[1]),
+                arrowprops=dict(arrowstyle="->", color="black"),
+                annotation_clip=False,
+            )
+
+        # Plot the depot location
+        ax.plot(
+            depot_loc[0],
+            depot_loc[1],
+            "g",
+            marker="s",
+            markersize=markersize,
+            label="Depot",
+        )
+
+        # Plot the pickup locations
+        for i, pickup_loc in enumerate(pickup_locs):
+            ax.plot(
+                pickup_loc[0],
+                pickup_loc[1],
+                "r",
+                marker="^",
+                markersize=markersize,
+                label="Pickup" if i == 0 else None,
+            )
+
+        # Plot the delivery locations
+        for i, delivery_loc in enumerate(delivery_locs):
+            ax.plot(
+                delivery_loc[0],
+                delivery_loc[1],
+                "b",
+                marker="v",
+                markersize=markersize,
+                label="Delivery" if i == 0 else None,
+            )
+
+        # Legend
+        # plt.legend(['Actions', 'Depot', 'Delivery', 'Pickup'])
+        # get handles
+        handles, labels = ax.get_legend_handles_labels()
+
+        # plot legend
+        ax.legend(handles, labels)
+        ax.set_title("Pickup and Delivery Problem Solution")
+        ax.set_xlabel("x-coordinate")
+        ax.set_ylabel("y-coordinate")
+        plt.show()
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/pctsp.py` & `rl4co-0.0.4/rl4co/envs/pctsp.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
-from rl4co.envs import RL4COEnvBase
-from rl4co.utils.ops import gather_by_index
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.utils.ops import gather_by_index, get_tour_length
+from rl4co.utils.pylogger import get_pylogger
+
+
+log = get_pylogger(__name__)
 
 # For the penalty to make sense it should be not too large (in which case all nodes will be visited) nor too small
 # so we want the objective term to be approximately equal to the length of the tour, which we estimate with half
 # of the nodes by half of the tour length (which is very rough but similar to op)
 # This means that the sum of penalties for all nodes will be approximately equal to the tour length (on average)
 # The expected total (uniform) penalty of half of the nodes (since approx half will be visited by the constraint)
 # is (n / 2) / 2 = n / 4 so divide by this means multiply by 4 / n,
@@ -31,98 +35,92 @@
 
     Args:
         num_loc (int): Number of locations
         min_loc (float): Minimum location value
         max_loc (float): Maximum location value
         penalty_factor (float): Penalty factor
         prize_required (float): Minimum prize required to visit a node
-        stochastic (bool): Whether the environment is stochastic
+        check_solution (bool): Set to False by default for small bug happening around 0.01% of the time (TODO: fix)
         td_params (TensorDict): Parameters of the environment
     """
-
+    
     name = "pctsp"
+    _stochastic = False
 
     def __init__(
         self,
         num_loc: int = 10,
         min_loc: float = 0,
         max_loc: float = 1,
         penalty_factor: float = 3,
         prize_required: float = 1,
-        stochastic: bool = False,
+        check_solution: bool = False,
         td_params: TensorDict = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.num_loc = num_loc
         self.min_loc = min_loc
         self.max_loc = max_loc
         self.penalty_factor = penalty_factor
         self.prize_required = prize_required
-        self.stochastic = stochastic
+        self.check_solution = check_solution
 
-    @staticmethod
-    def _step(td: TensorDict) -> TensorDict:
+    def _step(self, td: TensorDict) -> TensorDict:
         current_node = td["action"]
 
         # Get current coordinates, prize, and penalty
         cur_total_prize = td["cur_total_prize"] + gather_by_index(
             td["real_prize"], current_node
         )
         cur_total_penalty = td["cur_total_penalty"] + gather_by_index(
             td["penalty"], current_node
         )
-
-        # Update masks
+        
+        # Update visited
         visited = td["visited"].scatter(-1, current_node[..., None], 1)
-        mask = visited | visited[..., 0:1]
-
-        # Cannot visit depot if not yet collected 1 total prize and there are unvisited nodes
-        mask[..., 0] = (cur_total_prize < 1.0) & (
-            visited[..., 1:].int().sum(-1) < visited[..., 1:].size(-1)
-        )
-        action_mask = ~(mask > 0)  # Invert mask
 
         # Done and reward. Calculation is done outside hence set -inf
         done = (td["i"] > 0) & (current_node == 0)
         reward = torch.ones_like(cur_total_prize) * float("-inf")
 
-        return TensorDict(
+        td_step = TensorDict(
             {
                 "next": {
                     "locs": td["locs"],
                     "current_node": current_node,
                     "expected_prize": td["expected_prize"],
                     "real_prize": td["real_prize"],
                     "penalty": td["penalty"],
                     "cur_total_prize": cur_total_prize,
                     "cur_total_penalty": cur_total_penalty,
                     "visited": visited,
                     "prize_required": td["prize_required"],
                     "i": td["i"] + 1,
-                    "action_mask": action_mask,
                     "reward": reward,
                     "done": done,
                 },
             },
             batch_size=td.batch_size,
         )
+        td_step["next"].set("action_mask", self.get_action_mask(td_step["next"]))
+        return td_step 
 
     def _reset(
         self, td: Optional[TensorDict] = None, batch_size: Optional[list] = None
     ) -> TensorDict:
         if batch_size is None:
             batch_size = self.batch_size if td is None else td["locs"].shape[:-2]
         if td is None or td.is_empty():
             td = self.generate_data(batch_size=batch_size)
         self.device = td.device
 
         locs = torch.cat([td["depot"][..., None, :], td["locs"]], dim=-2)
         expected_prize = td["deterministic_prize"]
-        real_prize = td["stochastic_prize"] if self.stochastic else expected_prize
+        real_prize = td["stochastic_prize"] if self.stochastic else td["deterministic_prize"]
         penalty = td["penalty"]
 
         # Concatenate depots
         real_prize_with_depot = torch.cat(
             [torch.zeros_like(real_prize[..., :1]), real_prize], dim=-1
         )
         penalty_with_depot = F.pad(penalty, (1, 0), mode="constant", value=0)
@@ -139,38 +137,136 @@
             (*batch_size, self.num_loc + 1), dtype=torch.bool, device=self.device
         )
         i = torch.zeros((*batch_size,), dtype=torch.int64, device=self.device)
         prize_required = torch.full(
             (*batch_size,), self.prize_required, device=self.device
         )
 
-        # Cannot visit depot if not yet collected 1 total prize and there are unvisited nodes
-        mask = visited | visited[..., 0:1]
-        mask[..., 0] = (cur_total_prize < 1.0) & (
-            visited[..., 1:].int().sum(-1) < visited[..., 1:].size(-1)
-        )
-        action_mask = ~(mask > 0)  # Invert mask
-
-        return TensorDict(
+        td_reset = TensorDict(
             {
                 "locs": locs,
                 "current_node": current_node,
                 "expected_prize": expected_prize,
                 "real_prize": real_prize_with_depot,
                 "penalty": penalty_with_depot,
                 "cur_total_prize": cur_total_prize,
                 "cur_total_penalty": cur_total_penalty,
                 "visited": visited,
                 "prize_required": prize_required,
                 "i": i,
-                "action_mask": action_mask,
+            },
+            batch_size=batch_size,
+        )
+        td_reset.set("action_mask", self.get_action_mask(td_reset))
+        return td_reset
+    
+    @staticmethod
+    def get_action_mask(td: TensorDict) -> torch.Tensor:
+        """Cannot visit depot if not yet collected 1 total prize and there are unvisited nodes"""
+        mask = td["visited"] | td["visited"][..., 0:1]
+        mask[..., 0] = (td["cur_total_prize"] < 1.0) & (
+            td["visited"][..., 1:].int().sum(-1) < td["visited"][..., 1:].size(-1)
+        )
+        return ~(mask > 0)  # Invert mask, since 1 means feasible action
+
+    def get_reward(self, td: TensorDict, actions: torch.Tensor) -> torch.Tensor:
+        """Reward is `saved penalties - (total length + penalty)`"""
+
+        # In case all tours directly return to depot, prevent further problems
+        if actions.size(-1) == 1:  
+            assert (actions == 0).all(), "If all length 1 tours, they should be zero"
+            return torch.zeros(actions.size(0), dtype=torch.float, device=actions.device)
+        
+        # Check that the solution is valid
+        if self.check_solution:
+            self.check_solution_validity(td, actions)
+
+        # Gather locations in order of tour and get the length of tours
+        locs_ordered = gather_by_index(td["locs"], actions)
+        length = get_tour_length(locs_ordered)
+        
+        # Reward is saved penalties - (total length + penalty)
+        saved_penalty = td["penalty"].gather(1, actions)
+        return saved_penalty.sum(-1) - (length + td["penalty"][..., 1:].sum(-1))
+
+    @staticmethod
+    def check_solution_validity(td: TensorDict, actions: torch.Tensor):
+        """Check that the solution is valid, i.e. contains all nodes once at most, and either prize constraint is met or all nodes are visited"""
+
+        # Check that tours are valid, i.e. contain 0 to n -1
+        sorted_actions = actions.data.sort(1)[0]
+
+        # Make sure each node visited once at most (except for depot)
+        assert ((sorted_actions[..., 1:] == 0) | (sorted_actions[..., 1:] > sorted_actions[..., :-1])).all(), "Duplicates"
+
+        prize = td["real_prize"][..., 1:]  # Remove depot
+        prize_with_depot = torch.cat((torch.zeros_like(prize[:, :1]), prize), 1)
+        p = prize_with_depot.gather(1, actions)
+
+        # Either prize constraint should be satisfied or all prizes should be visited
+        assert (
+            (p.sum(-1) >= 1 - 1e-5) |
+            (sorted_actions.size(-1) - (sorted_actions == 0).int().sum(-1) == (td["locs"].size(-2) - 1)) # no depot
+        ).all(), "Total prize does not satisfy min total prize"
+
+    def generate_data(self, batch_size) -> TensorDict:
+        # Batch size input check
+        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
+
+        depot = torch.rand((*batch_size, 2))
+        locs = torch.rand((*batch_size, self.num_loc, 2))
+
+        penalty_max = (
+            MAX_LENGTHS[self.num_loc] * (self.penalty_factor) / float(self.num_loc)
+        )
+        penalty = torch.rand((*batch_size, self.num_loc)) * penalty_max
+
+        # Take uniform prizes
+        # Now expectation is 0.5 so expected total prize is n / 2, we want to force to visit approximately half of the nodes
+        # so the constraint will be that total prize >= (n / 2) / 2 = n / 4
+        # equivalently, we divide all prizes by n / 4 and the total prize should be >= 1
+        deterministic_prize = (
+            torch.rand((*batch_size, self.num_loc)) * 4 / float(self.num_loc)
+        )
+
+        # In the deterministic setting, the stochastic_prize is not used and the deterministic prize is known
+        # In the stochastic setting, the deterministic prize is the expected prize and is known up front but the
+        # stochastic prize is only revealed once the node is visited
+        # Stochastic prize is between (0, 2 * expected_prize) such that E(stochastic prize) = E(deterministic_prize)
+        stochastic_prize = (
+            torch.rand((*batch_size, self.num_loc)) * deterministic_prize * 2
+        )
+        # In the deterministic setting, the stochastic_prize is not used and the deterministic prize is known
+        # In the stochastic setting, the deterministic prize is the expected prize and is known up front but the
+        # stochastic prize is only revealed once the node is visited
+        # Stochastic prize is between (0, 2 * expected_prize) such that E(stochastic prize) = E(deterministic_prize)
+        stochastic_prize = (
+            torch.rand((*batch_size, self.num_loc)) * deterministic_prize * 2
+        )
+
+        return TensorDict(
+            {
+                "locs": locs,
+                "depot": depot,
+                "penalty": penalty,
+                "deterministic_prize": deterministic_prize,
+                "stochastic_prize": stochastic_prize,
             },
             batch_size=batch_size,
         )
 
+    @property
+    def stochastic(self):
+        return self._stochastic
+    
+    @stochastic.setter
+    def stochastic(self, state: bool):
+        if state == True:
+            log.warning('Stochastic mode should not be used for PCTSP. Use SPCTSP instead.')
+            
     def _make_spec(self, td_params: TensorDict):
         """Make the locs and action specs from the parameters."""
         self.observation_spec = CompositeSpec(
             locs=BoundedTensorSpec(
                 minimum=self.min_loc,
                 maximum=self.max_loc,
                 shape=(self.num_loc, 2),
@@ -224,95 +320,10 @@
             dtype=torch.int64,
             minimum=0,
             maximum=self.num_loc,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
         self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
 
-    def get_reward(self, td, actions):
-        # if actions.size(-1) == 1:  # In case all tours directly return to depot, prevent further problems
-        #     assert (actions == 0).all(), "If all length 1 tours, they should be zero"
-        #     return torch.zeros(actions.size(0), dtype=torch.float, device=actions.device)
-
-        # Check that tours are valid, i.e. contain 0 to n -1
-        # sorted_actions = actions.data.sort(1)[0]
-        # Make sure each node visited once at most (except for depot)
-        # assert ((sorted_actions[..., 1:] == 0) | (sorted_actions[..., 1:] > sorted_actions[..., :-1])).all(), "Duplicates"
-
-        prize = td["real_prize"][..., 1:]  # Remove depot
-        prize_with_depot = torch.cat((torch.zeros_like(prize[:, :1]), prize), 1)
-        prize_with_depot.gather(1, actions)
-
-        locs_with_depot = td["locs"]
-        depot = locs_with_depot[..., 0, :]
-        td["locs"][..., 1:]  # Remove depot
-
-        # Either prize constraint should be satisfied or all prizes should be visited
-        # assert (
-        #     (p.sum(-1) >= 1 - 1e-5) |
-        #     (sorted_actions.size(-1) - (sorted_actions == 0).int().sum(-1) == locs.size(-2)) # no depot
-        # ).all(), "Total prize does not satisfy min total prize"
-
-        pen = td["penalty"].gather(1, actions)
-
-        # Gather td in order of tour. We consider locs already have depot concatenated
-        d = gather_by_index(locs_with_depot, actions)
-
-        length = (
-            (d[:, 1:] - d[:, :-1]).norm(p=2, dim=-1).sum(1)  # Prevent error if len 1 seq
-            + (d[:, 0] - depot).norm(p=2, dim=-1)  # Depot to first
-            + (d[:, -1] - depot).norm(
-                p=2, dim=-1
-            )  # Last to depot, will be 0 if depot is last
-        )
-        # We want to maximize total prize
-        # Incurred penalty cost is total penalty cost - saved penalty costs of nodes visited
-        return -(length + td["penalty"][..., 1:].sum(-1) - pen.sum(-1))
-
-    def generate_data(self, batch_size) -> TensorDict:
-        # Batch size input check
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-
-        depot = torch.rand((*batch_size, 2))
-        locs = torch.rand((*batch_size, self.num_loc, 2))
-
-        penalty_max = (
-            MAX_LENGTHS[self.num_loc] * (self.penalty_factor) / float(self.num_loc)
-        )
-        penalty = torch.rand((*batch_size, self.num_loc)) * penalty_max
-
-        # Take uniform prizes
-        # Now expectation is 0.5 so expected total prize is n / 2, we want to force to visit approximately half of the nodes
-        # so the constraint will be that total prize >= (n / 2) / 2 = n / 4
-        # equivalently, we divide all prizes by n / 4 and the total prize should be >= 1
-        deterministic_prize = (
-            torch.rand((*batch_size, self.num_loc)) * 4 / float(self.num_loc)
-        )
-
-        # In the deterministic setting, the stochastic_prize is not used and the deterministic prize is known
-        # In the stochastic setting, the deterministic prize is the expected prize and is known up front but the
-        # stochastic prize is only revealed once the node is visited
-        # Stochastic prize is between (0, 2 * expected_prize) such that E(stochastic prize) = E(deterministic_prize)
-        stochastic_prize = (
-            torch.rand((*batch_size, self.num_loc)) * deterministic_prize * 2
-        )
-        # In the deterministic setting, the stochastic_prize is not used and the deterministic prize is known
-        # In the stochastic setting, the deterministic prize is the expected prize and is known up front but the
-        # stochastic prize is only revealed once the node is visited
-        # Stochastic prize is between (0, 2 * expected_prize) such that E(stochastic prize) = E(deterministic_prize)
-        stochastic_prize = (
-            torch.rand((*batch_size, self.num_loc)) * deterministic_prize * 2
-        )
-
-        return TensorDict(
-            {
-                "locs": locs,
-                "depot": depot,
-                "penalty": penalty,
-                "deterministic_prize": deterministic_prize,
-                "stochastic_prize": stochastic_prize,
-            },
-            batch_size=batch_size,
-        )
-
-    def render(self, td: TensorDict):
+    @staticmethod
+    def render(td: TensorDict, actions=None, ax=None):
         raise NotImplementedError("TODO: render is not implemented yet")
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/pdp.py` & `rl4co-0.0.4/rl4co/envs/tsp.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,35 +6,36 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
-from rl4co.envs.base import RL4COEnvBase
-from rl4co.utils.ops import gather_by_index
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.envs.common.utils import batch_to_scalar
+from rl4co.utils.ops import gather_by_index, get_tour_length
+from rl4co.utils.pylogger import get_pylogger
 
+log = get_pylogger(__name__)
 
-class PDPEnv(RL4COEnvBase):
-    """Pickup and Delivery Problem (PDP) environment
-    The environment is made of num_loc + 1 locations (cities):
-    - 1 depot
-    - num_loc / 2 pickup locations
-    - num_loc / 2 delivery locations
-    The goal is to visit all the pickup and delivery locations in the shortest path possible starting from the depot
-    The conditions is that the agent must visit a pickup location before visiting its corresponding delivery location
+
+class TSPEnv(RL4COEnvBase):
+    """
+    Traveling Salesman Problem environment
+    At each step, the agent chooses a city to visit. The reward is the -infinite unless the agent visits all the cities.
+    In that case, the reward is (-)length of the path: maximizing the reward is equivalent to minimizing the path length.
 
     Args:
         num_loc: number of locations (cities) in the TSP
         td_params: parameters of the environment
         seed: seed for the environment
         device: device to use.  Generally, no need to set as tensors are updated on the fly
     """
 
-    name = "pdp"
+    name = "tsp"
 
     def __init__(
         self,
         num_loc: int = 20,
         min_loc: float = 0,
         max_loc: float = 1,
         td_params: TensorDict = None,
@@ -44,262 +45,170 @@
         self.num_loc = num_loc
         self.min_loc = min_loc
         self.max_loc = max_loc
         self._make_spec(td_params)
 
     @staticmethod
     def _step(td: TensorDict) -> TensorDict:
-        current_node = td["action"].unsqueeze(-1)
-
-        num_loc = td["locs"].shape[-2] - 1  # except depot
-
-        # Pickup and delivery node pair of selected node
-        new_to_deliver = (current_node + num_loc // 2) % (num_loc + 1)
+        current_node = td["action"]
+        first_node = current_node if batch_to_scalar(td["i"]) == 0 else td["first_node"]
 
-        # Set available to 0 (i.e., we visited the node)
-        available = td["available"].scatter(
-            -1, current_node.expand_as(td["action_mask"]), 0
+        # Set not visited to 0 (i.e., we visited the node)
+        available = td["action_mask"].scatter(
+            -1, current_node.unsqueeze(-1).expand_as(td["action_mask"]), 0
         )
 
-        to_deliver = td["to_deliver"].scatter(
-            -1, new_to_deliver.expand_as(td["to_deliver"]), 1
-        )
-
-        # Action is feasible if the node is not visited and is to deliver
-        # action_mask = torch.logical_and(available, to_deliver)
-        action_mask = available & to_deliver
-
         # We are done there are no unvisited locations
-        done = torch.count_nonzero(available, dim=-1) == 0
+        done = torch.count_nonzero(available, dim=-1) <= 0
 
         # The reward is calculated outside via get_reward for efficiency, so we set it to -inf here
         reward = torch.ones_like(done) * float("-inf")
 
         # The output must be written in a ``"next"`` entry
         return TensorDict(
             {
                 "next": {
                     "locs": td["locs"],
+                    "first_node": first_node,
                     "current_node": current_node,
-                    "available": available,
-                    "to_deliver": to_deliver,
                     "i": td["i"] + 1,
-                    "action_mask": action_mask,
+                    "action_mask": available,
                     "reward": reward,
                     "done": done,
                 }
             },
             td.shape,
         )
 
     def _reset(self, td: Optional[TensorDict] = None, batch_size=None) -> TensorDict:
+        # Initialize locations
+        init_locs = td["locs"] if td is not None else None
         if batch_size is None:
-            batch_size = self.batch_size if td is None else td.batch_size
-
-        if td is None or td.is_empty():
-            td = self.generate_data(batch_size=batch_size)
+            batch_size = self.batch_size if init_locs is None else init_locs.shape[:-2]
+        self.device = device = init_locs.device if init_locs is not None else self.device
+        if init_locs is None:
+            init_locs = self.generate_data(batch_size=batch_size).to(device)["locs"]
 
-        self.device = td.device
-
-        locs = torch.cat((td["depot"][:, None, :], td["locs"]), -2)
-
-        # Pick is 1, deliver is 0 [batch_size, graph_size+1], [1,1...1, 0...0]
-        to_deliver = torch.cat(
-            [
-                torch.ones(
-                    *batch_size,
-                    self.num_loc // 2 + 1,
-                    dtype=torch.bool,
-                    device=self.device,
-                ),
-                torch.zeros(
-                    *batch_size, self.num_loc // 2, dtype=torch.bool, device=self.device
-                ),
-            ],
-            dim=-1,
-        )
-
-        # Cannot visit depot at first step # [0,1...1] so set not available
-        available = torch.ones(
-            (*batch_size, self.num_loc + 1), dtype=torch.bool, device=self.device
-        )
-        action_mask = ~available.contiguous()  # [batch_size, graph_size+1]
-        action_mask[..., 0] = 1  # First step is always the depot
+        # We do not enforce loading from self for flexibility
+        num_loc = init_locs.shape[-2]
 
         # Other variables
-        current_node = torch.zeros(
-            (*batch_size, 1), dtype=torch.int64, device=self.device
-        )
-        i = torch.zeros((*batch_size, 1), dtype=torch.int64, device=self.device)
+        current_node = torch.zeros((batch_size), dtype=torch.int64, device=device)
+        available = torch.ones(
+            (*batch_size, num_loc), dtype=torch.bool, device=device
+        )  # 1 means not visited, i.e. action is allowed
+        i = torch.zeros((*batch_size, 1), dtype=torch.int64, device=device)
 
         return TensorDict(
             {
-                "locs": locs,
+                "locs": init_locs,
+                "first_node": current_node,
                 "current_node": current_node,
-                "to_deliver": to_deliver,
-                "available": available,
                 "i": i,
-                "action_mask": action_mask,
+                "action_mask": available,
             },
             batch_size=batch_size,
         )
 
-    def _make_spec(self, td_params: TensorDict):
-        """Make the observation and action specs from the parameters."""
+    def _make_spec(self, td_params):
+        """Make the observation and action specs from the parameters"""
         self.observation_spec = CompositeSpec(
             locs=BoundedTensorSpec(
                 minimum=self.min_loc,
                 maximum=self.max_loc,
-                shape=(self.num_loc + 1, 2),
+                shape=(self.num_loc, 2),
                 dtype=torch.float32,
             ),
-            current_node=UnboundedDiscreteTensorSpec(
+            first_node=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
-            to_deliver=UnboundedDiscreteTensorSpec(
+            current_node=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
             i=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
             action_mask=UnboundedDiscreteTensorSpec(
-                shape=(self.num_loc + 1),
+                shape=(self.num_loc),
                 dtype=torch.bool,
             ),
             shape=(),
         )
         self.input_spec = self.observation_spec.clone()
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             minimum=0,
-            maximum=self.num_loc + 1,
+            maximum=self.num_loc,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
         self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
 
     @staticmethod
     def get_reward(td, actions) -> TensorDict:
-        # assert (actions[:, 0] == 0).all(), "Not starting at depot"
+        locs = td["locs"]
         assert (
             torch.arange(actions.size(1), out=actions.data.new())
             .view(1, -1)
             .expand_as(actions)
             == actions.data.sort(1)[0]
-        ).all(), "Not visiting all nodes"
+        ).all(), "Invalid tour"
 
-        visited_time = torch.argsort(
-            actions, 1
-        )  # index of pickup less than index of delivery
-        assert (
-            visited_time[:, 1 : actions.size(1) // 2 + 1]
-            < visited_time[:, actions.size(1) // 2 + 1 :]
-        ).all(), "Deliverying without pick-up"
-
-        # Gather locations in the order of actions and get reward = -(total distance)
-        locs = gather_by_index(td["locs"], actions)  # [batch, graph_size+1, 2]
-        locs_next = torch.roll(locs, 1, dims=1)
-        return -(locs_next - locs).norm(p=2, dim=2).sum(1)
+        # Gather locations in order of tour and return distance between them (i.e., -reward)
+        locs_ordered = gather_by_index(locs, actions)
+        return -get_tour_length(locs_ordered)
 
     def generate_data(self, batch_size) -> TensorDict:
         batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-
-        # Initialize the locations (including the depot which is always the first node)
-        locs_with_depot = (
-            torch.FloatTensor(*batch_size, self.num_loc + 1, 2)
-            .uniform_(self.min_loc, self.max_loc)
-            .to(self.device)
-        )
-
-        return TensorDict(
-            {
-                "locs": locs_with_depot[..., 1:, :],
-                "depot": locs_with_depot[..., 0, :],
-            },
-            batch_size=batch_size,
+        locs = (
+            torch.rand((*batch_size, self.num_loc, 2), generator=self.rng)
+            * (self.max_loc - self.min_loc)
+            + self.min_loc
         )
+        return TensorDict({"locs": locs}, batch_size=batch_size)
 
     @staticmethod
-    def render(td, actions=None):
+    def render(td, actions=None, ax=None):
         import matplotlib.pyplot as plt
+        import numpy as np
 
-        markersize = 8
+        if ax is None:
+            # Create a plot of the nodes
+            _, ax = plt.subplots()
 
         td = td.detach().cpu()
         # if batch_size greater than 0 , we need to select the first batch element
         if td.batch_size != torch.Size([]):
             td = td[0]
-            if actions is not None:
-                actions = actions[0]
 
-        # Variables
-        init_deliveries = td["to_deliver"][1:]
-        delivery_locs = td["locs"][1:][~init_deliveries.bool()]
-        pickup_locs = td["locs"][1:][init_deliveries.bool()]
-        depot_loc = td["locs"][0]
-        actions = actions if actions is not None else td["action"]
-
-        fig, ax = plt.subplots()
-
-        # Plot the actions in order
-        for i in range(len(actions)):
-            from_node = actions[i]
-            to_node = (
-                actions[i + 1] if i < len(actions) - 1 else actions[0]
-            )  # last goes back to depot
-            from_loc = td["locs"][from_node]
-            to_loc = td["locs"][to_node]
-            ax.plot([from_loc[0], to_loc[0]], [from_loc[1], to_loc[1]], "k-")
-            ax.annotate(
-                "",
-                xy=(to_loc[0], to_loc[1]),
-                xytext=(from_loc[0], from_loc[1]),
-                arrowprops=dict(arrowstyle="->", color="black"),
-                annotation_clip=False,
-            )
-
-        # Plot the depot location
-        ax.plot(
-            depot_loc[0],
-            depot_loc[1],
-            "g",
-            marker="s",
-            markersize=markersize,
-            label="Depot",
+        locs = td["locs"]
+
+        if actions is None:
+            actions = td.get("action", None)
+
+        # gather locs in order of action if available
+        if actions is None:
+            log.warning("No action in TensorDict, rendering unsorted locs")
+        else:
+            locs = gather_by_index(locs, actions, dim=0)
+
+        # Cat the first node to the end to complete the tour
+        locs = torch.cat((locs, locs[0:1]))
+        x, y = locs[:, 0], locs[:, 1]
+
+        # Plot the visited nodes
+        ax.scatter(x, y, color="tab:blue")
+
+        # Add arrows between visited nodes as a quiver plot
+        dx, dy = np.diff(x), np.diff(y)
+        ax.quiver(
+            x[:-1], y[:-1], dx, dy, scale_units="xy", angles="xy", scale=1, color="k"
         )
 
-        # Plot the pickup locations
-        for i, pickup_loc in enumerate(pickup_locs):
-            ax.plot(
-                pickup_loc[0],
-                pickup_loc[1],
-                "r",
-                marker="^",
-                markersize=markersize,
-                label="Pickup" if i == 0 else None,
-            )
-
-        # Plot the delivery locations
-        for i, delivery_loc in enumerate(delivery_locs):
-            ax.plot(
-                delivery_loc[0],
-                delivery_loc[1],
-                "b",
-                marker="v",
-                markersize=markersize,
-                label="Delivery" if i == 0 else None,
-            )
-
-        # Legend
-        # plt.legend(['Actions', 'Depot', 'Delivery', 'Pickup'])
-        # get handles
-        handles, labels = ax.get_legend_handles_labels()
-
-        # plot legend
-        ax.legend(handles, labels)
-        ax.set_title("Pickup and Delivery Problem Solution")
+        # Set plot title and axis labels
+        ax.set_title("TSP Solution")
         ax.set_xlabel("x-coordinate")
         ax.set_ylabel("y-coordinate")
         plt.show()
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/sdvrp.py` & `rl4co-0.0.4/rl4co/envs/sdvrp.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,154 +6,166 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
-from rl4co.envs import RL4COEnvBase
+from rl4co.envs.cvrp import CVRPEnv, CAPACITIES
 from rl4co.utils.ops import gather_by_index
+from rl4co.utils.pylogger import get_pylogger
 
+log = get_pylogger(__name__)
 
-class SDVRPEnv(RL4COEnvBase):
-    """
-    Split Dilivery Vehicle Routing Problem (SDVRP) environment
-    At each step, the agent chooses a city to visit. The reward is the -infinite unless the agent visits all the cities.
+
+class SDVRPEnv(CVRPEnv):
+    """Split Delivery Vehicle Routing Problem (SDVRP) environment.
+    SDVRP is a generalization of CVRP, where nodes can be visited multiple times and a fraction of the demand can be met.
+    At each step, the agent chooses a customer to visit depending on the current location and the remaining capacity.
+    When the agent visits a customer, the remaining capacity is updated. If the remaining capacity is not enough to
+    visit any customer, the agent must go back to the depot. The reward is the -infinite unless the agent visits all the cities.
     In that case, the reward is (-)length of the path: maximizing the reward is equivalent to minimizing the path length.
 
     Args:
-        - num_loc <int>: number of locations (cities) in the VRP, without the depot. (e.g. 10 means 10 locs + 1 depot)
-        - min_loc <float>: minimum value for the location coordinates
-        - max_loc <float>: maximum value for the location coordinates
-        - capacity <float>: capacity of the vehicle
-        - td_params <TensorDict>: parameters of the environment
-        - seed <int>: seed for the environment
-        - device <str>: 'cpu' or 'cuda:0', device to use.  Generally, no need to set as tensors are updated on the fly
+        num_loc (int): number of locations (cities) in the VRP, without the depot. (e.g. 10 means 10 locs + 1 depot)
+        min_loc (float): minimum value for the location coordinates
+        max_loc (float): maximum value for the location coordinates
+        min_demand (float): minimum value for the demand of each customer
+        max_demand (float): maximum value for the demand of each customer
+        vehicle_capacity (float): capacity of the vehicle
+        capacity (float): capacity of the vehicle
+        td_params (TensorDict): parameters of the environment
     """
 
     name = "sdvrp"
 
     def __init__(
         self,
         num_loc: int = 20,
         min_loc: float = 0,
         max_loc: float = 1,
-        min_demand: float = 0.1,
-        max_demand: float = 0.5,
-        capacity: float = 1,
-        batch_size: list = [],
+        min_demand: float = 1,
+        max_demand: float = 10,
+        vehicle_capacity: float = 1.0,
+        capacity: float = None,
         td_params: TensorDict = None,
         **kwargs,
     ):
-        super().__init__(**kwargs)
-        self.num_loc = num_loc
-        self.min_loc = min_loc
-        self.max_loc = max_loc
-        self.min_demand = min_demand
-        self.max_demand = max_demand
-        self.capacity = capacity
-        self.batch_size = batch_size
-        self._make_spec(td_params)
+        super().__init__(
+            num_loc=num_loc,
+            min_loc=min_loc,
+            max_loc=max_loc,
+            min_demand=min_demand,
+            max_demand=max_demand,
+            vehicle_capacity=vehicle_capacity,
+            capacity=capacity,
+            td_params=td_params,
+            **kwargs,
+        )
+    
+    def _step(self, td: TensorDict) -> TensorDict:
+        # Update the state
+        current_node = td["action"][:, None]  # Add dimension for step
+
+        # Not selected_demand is demand of first node (by clamp) so incorrect for nodes that visit depot!
+        selected_demand = gather_by_index(
+            td["demand_with_depot"], current_node, dim=-1, squeeze=False
+        )[..., :1]
+        delivered_demand = torch.min(selected_demand, td["vehicle_capacity"] - td["used_capacity"])
 
-    @staticmethod
-    def _step(td: TensorDict) -> TensorDict:
-        """Update the states of the environment
-        Args:
-            - td <TensorDict>: tensor dictionary containing with the action
-                - action <int> [batch_size, 1]: action to take
-        NOTE:
-            - the first node in de demand is larger than 1 or less than 0?
-            - this design is important. For now the design is LESS than 0
-        """
-        current_node = td["action"].unsqueeze(-1)
-        demand = td["demand"]
-
-        # Calculate the available capacity
-        available_capacity = td["capacity"] + demand[..., :1]
-
-        # Calculate the capacity to use, if the demand is larger than the available capacity, use the capacity
-        current_demand = torch.gather(demand, 1, current_node)
-        use_capacity = torch.min(current_demand, available_capacity)
-
-        # Update the used capacity
-        demand[..., 0] -= use_capacity.squeeze()
-
-        # Update visited node capacity
-        demand[..., 1:] = demand.scatter(-1, current_node, -use_capacity, reduce="add")[
-            ..., 1:
-        ]
-
-        # Get the action mask, no zero demand nodes can be visited
-        action_mask = torch.abs(demand) > 0
-
-        # Nodes exceeding capacity cannot be visited
-        available_capacity = td["capacity"] + demand[..., :1]
-        action_mask = torch.logical_and(action_mask, demand <= available_capacity)
-
-        # We are done there are no unvisited locations
-        done = torch.count_nonzero(demand, dim=-1) <= 0
-
-        # If all nodes are visited, then set the depot be always available
-        action_mask[..., 0] = torch.logical_or(action_mask[..., 0], done)
-
-        # Calculate reward (minus length of path, since we want to maximize the reward -> minimize the path length)
-        # Note: reward is calculated outside for now via the get_reward function
-        # to calculate here need to pass action sequence or save it as state
+        # Increase capacity if depot is not visited, otherwise set to 0
+        used_capacity = (td["used_capacity"] + delivered_demand) * (current_node != 0).float()
+
+        # Update demand
+        demand_with_depot = td["demand_with_depot"].scatter_add(-1, current_node, -delivered_demand)
+
+        # Get done and reward (-inf since we get it outside)
+        done = ~(demand_with_depot > 0).any(-1)
         reward = torch.ones_like(done) * float("-inf")
 
-        # The output must be written in a ``"next"`` entry
-        return TensorDict(
+        td_step = TensorDict(
             {
                 "next": {
                     "locs": td["locs"],
-                    "capacity": td["capacity"],
+                    "demand": td["demand"],
+                    "demand_with_depot": demand_with_depot,
                     "current_node": current_node,
-                    "demand": demand,
-                    "action_mask": action_mask,
+                    "used_capacity": used_capacity,
+                    "vehicle_capacity": td["vehicle_capacity"],
                     "reward": reward,
                     "done": done,
                 }
             },
             td.shape,
         )
+        td_step["next"].set("action_mask", self.get_action_mask(td_step["next"]))
+        return td_step
 
     def _reset(
-        self, td: Optional[TensorDict] = None, batch_size: Optional[list] = None
+        self,
+        td: Optional[TensorDict] = None,
+        batch_size: Optional[list] = None,
     ) -> TensorDict:
-        """
-        Args:
-            - td (Optional) <TensorDict>: tensor dictionary containing the initial state
-        """
         if batch_size is None:
             batch_size = self.batch_size if td is None else td["locs"].shape[:-2]
 
         if td is None or td.is_empty():
             td = self.generate_data(batch_size=batch_size)
 
-        # Initialize the current node
-        current_node = torch.zeros(
-            (*batch_size, 1), dtype=torch.int64, device=self.device
-        )
-
-        # Initialize the capacity
-        capacity = torch.full((*batch_size, 1), self.capacity)
+        self.device = td.device
 
-        # Init the action mask
-        action_mask = td["demand"] > 0
-
-        return TensorDict(
+        # Create reset TensorDict
+        reset_td = TensorDict(
             {
-                "locs": td["locs"],
-                "capacity": capacity,
-                "current_node": current_node,
+                "locs": torch.cat((td["depot"][..., None, :], td["locs"]), -2),
                 "demand": td["demand"],
-                "action_mask": action_mask,
+                "demand_with_depot": torch.cat((torch.zeros_like(td["demand"][..., 0:1]), td["demand"]), -1),
+                "current_node": torch.zeros(*batch_size, 1, dtype=torch.long, device=self.device),
+                "used_capacity": torch.zeros((*batch_size, 1), device=self.device),
+                "vehicle_capacity": torch.full((*batch_size, 1), self.vehicle_capacity, device=self.device),
             },
             batch_size=batch_size,
         )
+        reset_td.set("action_mask", self.get_action_mask(reset_td))
+        return reset_td
+    
+    @staticmethod
+    def get_action_mask(td: TensorDict) -> torch.Tensor:
+        mask_loc = (td["demand_with_depot"][..., 1:] == 0) | (td["used_capacity"] >= td["vehicle_capacity"])
+        mask_depot = (td["current_node"] == 0).squeeze(-1) & ((mask_loc == 0).int().sum(-1) > 0)
+        return ~torch.cat((mask_depot[..., None], mask_loc), -1)
+
+    @staticmethod
+    def check_solution_validity(td: TensorDict, actions: torch.Tensor):
+        """Check that the solution is valid (all demand is satisfied)"""
+        
+        batch_size, graph_size = td["demand"].size()
+
+        # Each node can be visited multiple times, but we always deliver as much demand as possible
+        # We check that at the end all demand has been satisfied
+        demands = torch.cat(
+            (
+                -td["vehicle_capacity"],
+                td['demand']
+            ),
+            1
+        )
+
+        rng = torch.arange(batch_size, out=demands.data.new().long())
+        used_cap = torch.zeros_like(td['demand'][..., 0])
+        a_prev = None
+        for a in actions.transpose(0, 1):
+            assert a_prev is None or (demands[((a_prev == 0) & (a == 0)), :] == 0).all(), \
+                "Cannot visit depot twice if any nonzero demand"
+            d = torch.min(demands[rng, a], td["vehicle_capacity"].squeeze(-1) - used_cap)
+            demands[rng, a] -= d
+            used_cap += d
+            used_cap[a == 0] = 0
+            a_prev = a
+        assert (demands == 0).all(), "All demand must be satisfied"
 
     def _make_spec(self, td_params: TensorDict):
         """Make the observation and action specs from the parameters."""
         self.observation_spec = CompositeSpec(
             locs=BoundedTensorSpec(
                 minimum=self.min_loc,
                 maximum=self.max_loc,
@@ -161,91 +173,39 @@
                 dtype=torch.float32,
             ),
             current_node=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
             demand=BoundedTensorSpec(
-                minimum=-self.capacity,
+                minimum=self.min_demand,
+                maximum=self.max_demand,
+                shape=(self.num_loc, 1),  # demand is only for customers
+                dtype=torch.float32,
+            ),
+            demand_with_depot=BoundedTensorSpec(
+                minimum=self.min_demand, 
                 maximum=self.max_demand,
                 shape=(self.num_loc + 1, 1),
                 dtype=torch.float32,
             ),
+            used_capacity=BoundedTensorSpec(
+                minimum=0,
+                maximum=self.vehicle_capacity,
+                shape=(1,),
+                dtype=torch.float32,
+            ),
             action_mask=UnboundedDiscreteTensorSpec(
                 shape=(self.num_loc + 1, 1),
                 dtype=torch.bool,
             ),
             shape=(),
         )
         self.input_spec = self.observation_spec.clone()
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             minimum=0,
             maximum=self.num_loc + 1,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
-        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
-
-    @staticmethod
-    def get_reward(td, actions) -> TensorDict:
-        """
-        Args:
-            - td: <tensor_dict>: tensor dictionary containing the state
-            - actions: [batch_size, TODO] num_loc means a sequence of actions till the task is done
-        NOTE:
-            - about the length of the actions
-        """
-        locs = td["locs"]
-
-        # Gather locations in order of tour and return distance between them (i.e., -reward)
-        locs = gather_by_index(locs, actions)
-        locs_next = torch.roll(locs, 1, dims=1)
-        return -((locs_next - locs).norm(p=2, dim=2).sum(1))
-
-    def generate_data(self, batch_size) -> TensorDict:
-        """
-        Args:
-            - batch_size <int> or <list>: batch size
-        Returns:
-            - td <TensorDict>: tensor dictionary containing the initial state
-                - locs <Tensor> [batch_size, num_loc+1, 2]: locations of the nodes
-                - demand <Tensor> [batch_size, num_loc+1]: demand of the nodes
-                - capacity <Tensor> [batch_size, 1]: capacity of the vehicle
-                - current_node <Tensor> [batch_size, 1]: current node
-                - i <Tensor> [batch_size, 1]: number of visited nodes
-        NOTE:
-            - the locs includes the depot as the first node
-            - the demand includes the used capacity at the first value
-            - the unvisited variable can be replaced by demand > 0
-        """
-        # Batch size input check
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-
-        # Initialize the locations (including the depot which is always the first node)
-        locs = (
-            torch.FloatTensor(*batch_size, self.num_loc + 1, 2)
-            .uniform_(self.min_loc, self.max_loc)
-            .to(self.device)
-        )
-
-        # Initialize the demand
-        demand = (
-            torch.FloatTensor(*batch_size, self.num_loc + 1)
-            .uniform_(self.min_demand, self.max_demand)
-            .to(self.device)
-        )
-
-        # The first demand is the used capacity
-        demand[..., 0] = 0
-
-        return TensorDict(
-            {
-                "locs": locs,
-                "depot": locs[..., 0, :],
-                "demand": demand,
-            },
-            batch_size=batch_size,
-        )
-
-    def render(self, td: TensorDict):
-        raise NotImplementedError("TODO: render is not implemented yet")
+        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
```

### Comparing `rl4co-0.0.3.dev3/rl4co/envs/utils.py` & `rl4co-0.0.4/rl4co/envs/common/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/attention.py` & `rl4co-0.0.4/rl4co/models/nn/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/env_context.py` & `rl4co-0.0.4/rl4co/models/nn/env_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     """Get context object for given environment name"""
     context_classes = {
         "tsp": TSPContext,
         "atsp": TSPContext,
         "cvrp": VRPContext,
         "sdvrp": VRPContext,
         "pctsp": PCTSPContext,
+        "spctsp": PCTSPContext,
         "op": OPContext,
         "dpp": DPPContext,
         "mdpp": DPPContext,
         "pdp": PDPContext,
         "mtsp": MTSPContext,
     }
 
@@ -104,32 +105,33 @@
 
 
 class OPContext(EnvContext):
     def __init__(self, embedding_dim):
         super(OPContext, self).__init__(embedding_dim, embedding_dim + 1)
 
     def _state_embedding(self, embeddings, td):
-        state_embedding = td["length_capacity"]
-        return state_embedding
+        state_embedding = td["max_length"][..., 0] - td["tour_length"]
+        return state_embedding[..., None]
 
 
 class DPPContext(EnvContext):
     def __init__(self, embedding_dim):
         super(DPPContext, self).__init__(embedding_dim)
 
     def forward(self, embeddings, td):
         """Context cannot be defined by a single node embedding for DPP, hence 0.
         We modify the dynamic embedding instead to capture placed items
         """
         return embeddings.new_zeros(embeddings.size(0), self.embedding_dim)
 
 
 class PDPContext(EnvContext):
+    """From https://arxiv.org/abs/2110.02634"""
+
     def __init__(self, embedding_dim):
-        """From https://arxiv.org/abs/2110.02634"""
         super(PDPContext, self).__init__(embedding_dim, embedding_dim)
 
     def forward(self, embeddings, td):
         cur_node_embedding = self._cur_node_embedding(embeddings, td).squeeze()
         return self.project_context(cur_node_embedding)
```

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/env_embedding.py` & `rl4co-0.0.4/rl4co/models/nn/env_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,18 @@
             "init": VRPInitEmbedding,
             "dynamic": SDVRPDynamicEmbedding,
         },
         "pctsp": {
             "init": PCTSPInitEmbedding,
             "dynamic": StaticEmbedding,
         },
+        "spctsp": {
+            "init": PCTSPInitEmbedding,
+            "dynamic": StaticEmbedding,
+        },
         "op": {
             "init": OPInitEmbedding,
             "dynamic": StaticEmbedding,
         },
         "dpp": {
             "init": DPPInitEmbedding,
             "dynamic": StaticEmbedding,
```

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/flash_attention.py` & `rl4co-0.0.4/rl4co/models/nn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/graph/gat.py` & `rl4co-0.0.4/rl4co/models/nn/graph/gat.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/graph/gcn.py` & `rl4co-0.0.4/rl4co/models/nn/graph/gcn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/graph/mpnn.py` & `rl4co-0.0.4/rl4co/models/nn/graph/mpnn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/mlp.py` & `rl4co-0.0.4/rl4co/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/ops.py` & `rl4co-0.0.4/rl4co/models/nn/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/nn/utils.py` & `rl4co-0.0.4/rl4co/models/nn/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/rl/ppo/model.py` & `rl4co-0.0.4/rl4co/models/rl/ppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/rl/ppo/task.py` & `rl4co-0.0.4/rl4co/models/rl/ppo/task.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/base.py` & `rl4co-0.0.4/rl4co/models/rl/reinforce/base.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/baselines.py` & `rl4co-0.0.4/rl4co/models/rl/reinforce/baselines.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/rl/reinforce/critic.py` & `rl4co-0.0.4/rl4co/models/rl/reinforce/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/am/decoder.py` & `rl4co-0.0.4/rl4co/models/zoo/am/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/am/model.py` & `rl4co-0.0.4/rl4co/models/zoo/am/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/am/policy.py` & `rl4co-0.0.4/rl4co/models/zoo/am/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/decoder.py` & `rl4co-0.0.4/rl4co/models/zoo/amppo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/model.py` & `rl4co-0.0.4/rl4co/models/zoo/amppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/amppo/policy.py` & `rl4co-0.0.4/rl4co/models/zoo/amppo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ham/attention.py` & `rl4co-0.0.4/rl4co/models/zoo/ham/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ham/encoder.py` & `rl4co-0.0.4/rl4co/models/zoo/ham/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ham/model.py` & `rl4co-0.0.4/rl4co/models/zoo/ham/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ham/policy.py` & `rl4co-0.0.4/rl4co/models/zoo/ham/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/decoder.py` & `rl4co-0.0.4/rl4co/models/zoo/mdam/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/encoder.py` & `rl4co-0.0.4/rl4co/models/zoo/mdam/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/model.py` & `rl4co-0.0.4/rl4co/models/zoo/mdam/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/mdam/policy.py` & `rl4co-0.0.4/rl4co/models/zoo/mdam/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/augmentations.py` & `rl4co-0.0.4/rl4co/models/zoo/pomo/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/decoder.py` & `rl4co-0.0.4/rl4co/models/zoo/pomo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/model.py` & `rl4co-0.0.4/rl4co/models/zoo/pomo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/pomo/policy.py` & `rl4co-0.0.4/rl4co/models/zoo/pomo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/critic.py` & `rl4co-0.0.4/rl4co/models/zoo/ptrnet/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/decoder.py` & `rl4co-0.0.4/rl4co/models/zoo/ptrnet/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/encoder.py` & `rl4co-0.0.4/rl4co/models/zoo/ptrnet/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/model.py` & `rl4co-0.0.4/rl4co/models/zoo/ptrnet/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/ptrnet/policy.py` & `rl4co-0.0.4/rl4co/models/zoo/ptrnet/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/augmentations.py` & `rl4co-0.0.4/rl4co/models/zoo/symnco/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/decoder.py` & `rl4co-0.0.4/rl4co/models/zoo/symnco/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/losses.py` & `rl4co-0.0.4/rl4co/models/zoo/symnco/losses.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/model.py` & `rl4co-0.0.4/rl4co/models/zoo/symnco/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/models/zoo/symnco/policy.py` & `rl4co-0.0.4/rl4co/models/zoo/symnco/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/tasks/eval.py` & `rl4co-0.0.4/rl4co/tasks/eval.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/tasks/rl4co.py` & `rl4co-0.0.4/rl4co/tasks/rl4co.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from hydra.utils import instantiate
 from lightning import LightningModule
 from omegaconf import DictConfig
 from torch.utils.data import DataLoader
 
 from rl4co.data.dataset import tensordict_collate_fn
 from rl4co.data.generate_data import generate_default_datasets
-from rl4co.envs.base import EnvBase
+from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class RL4COLitModule(LightningModule):
     """
     Base LightningModule for Neural Combinatorial Optimization
     Args:
         cfg: Hydra config
         env: Environment to use overridding the config. If None, instantiate from config
         model: Model to use overridding the config. If None, instantiate from config
     """
 
-    def __init__(self, cfg: DictConfig, env: EnvBase = None, model: nn.Module = None):
+    def __init__(self, cfg: DictConfig, env: RL4COEnvBase = None, model: nn.Module = None):
         if cfg.get("train", {}).get("disable_profiling", True):
             # Disable profiling executor. This reduces memory and increases speed.
             # https://github.com/HazyResearch/safari/blob/111d2726e7e2b8d57726b7a8b932ad8a4b2ad660/train.py#LL124-L129C17
             try:
                 torch._C._jit_set_profiling_executor(False)
                 torch._C._jit_set_profiling_mode(False)
             except AttributeError:
```

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/callbacks/speed_monitor.py` & `rl4co-0.0.4/rl4co/utils/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/download/downloader.py` & `rl4co-0.0.4/rl4co/utils/download/downloader.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/download/gdrive.py` & `rl4co-0.0.4/rl4co/utils/download/gdrive.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/download/s3.py` & `rl4co-0.0.4/rl4co/utils/download/s3.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/helpers.py` & `rl4co-0.0.4/rl4co/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/instantiators.py` & `rl4co-0.0.4/rl4co/utils/instantiators.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/lightning.py` & `rl4co-0.0.4/rl4co/utils/lightning.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/logging_utils.py` & `rl4co-0.0.4/rl4co/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/ops.py` & `rl4co-0.0.4/rl4co/utils/ops.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     s = x.shape
     return x.expand(repeats, *s).contiguous().view(s[0] * repeats, *s[1:])
 
 
 def batchify(
     x: Union[Tensor, TensorDict], shape: Union[tuple, int]
 ) -> Union[Tensor, TensorDict]:
-    """Same as `einops.repeat(x, 'b ... -> (b r) ...', r=repeats)` but ~1.5x faster and supports TensorDicts
-    Repeats batchify operation `n` times as specified by each shape element
+    """Same as `einops.repeat(x, 'b ... -> (b r) ...', r=repeats)` but ~1.5x faster and supports TensorDicts.
+    Repeats batchify operation `n` times as specified by each shape element.
     If shape is a tuple, iterates over each element and repeats that many times to match the tuple shape.
 
     Example:
     >>> x.shape: [a, b, c, ...]
     >>> shape: [a, b, c]
     >>> out.shape: [a*b*c, ...]
     """
@@ -72,17 +72,30 @@
     """
     expanded_shape = list(src.shape)
     expanded_shape[dim] = -1
     idx = idx.view(idx.shape + (1,) * (src.dim() - idx.dim())).expand(expanded_shape)
     return src.gather(dim, idx).squeeze() if squeeze else src.gather(dim, idx)
 
 
-def distance(x, y):
+# @torch.jit.script
+def get_distance(x: Tensor, y: Tensor):
     """Euclidean distance between two tensors of shape `[..., n, dim]`"""
-    return torch.norm(x - y, p=2, dim=-1)
+    return (x - y).norm(p=2, dim=-1)
+
+
+# @torch.jit.script
+def get_tour_length(ordered_locs):
+    """Compute the total tour distance for a batch of ordered tours.
+    Computes the L2 norm between each pair of consecutive nodes in the tour and sums them up.
+
+    Args:
+        ordered_locs: Tensor of shape [batch_size, num_nodes, 2] containing the ordered locations of the tour
+    """
+    ordered_locs_next = torch.roll(ordered_locs, 1, dims=-2)
+    return get_distance(ordered_locs_next, ordered_locs).sum(-1)
 
 
 def select_start_nodes(td, num_nodes, env=None):
     """Node selection strategy as proposed in POMO (Kwon et al. 2020)
     and extended in SymNCO (Kim et al. 2022).
     Selects different start nodes for each batch element
```

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/param_grouping.py` & `rl4co-0.0.4/rl4co/utils/param_grouping.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/pylogger.py` & `rl4co-0.0.4/rl4co/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/rich_utils.py` & `rl4co-0.0.4/rl4co/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/test_utils.py` & `rl4co-0.0.4/rl4co/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/transfer.py` & `rl4co-0.0.4/rl4co/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co/utils/utils.py` & `rl4co-0.0.4/rl4co/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/rl4co.egg-info/PKG-INFO` & `rl4co-0.0.4/rl4co.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.3.dev3
+Version: 0.0.4
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/kaist-silab/rl4co
 Project-URL: Bug Tracker, https://github.com/kaist-silab/rl4co/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: graph
@@ -221,26 +221,32 @@
 Provides-Extra: linting
 License-File: LICENSE
 
 <div align="center">
 
 # RL4CO
 
-An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
 
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
-<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
 [![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
+[**Documentation**](https://rl4co.readthedocs.io/) |  [**Getting Started**](#getting-started) | [**Usage**](#usage) | [**Contributing**](#contributing) | [**Paper**](https://arxiv.org/abs/2306.17100) | [**Citation**](#cite-us)
+
 </div>
 
+---
+
+
+An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering.
+
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
 - [TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily handle heterogeneous data such as states, actions and rewards
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
@@ -366,13 +372,32 @@
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
 
 ## Contributing
-Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO!
+[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls).
+If you would like to contribute, please check out our contribution guidelines   [here](.github/CONTRIBUTING.md). We welcome and look forward to all contributions to RL4CO!
+
+We are also on [Slack](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) if you have any questions or would like to discuss RL4CO with us. We are open to collaborations and would love to hear from you 🚀
+
 
 ### Contributors
 <a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
 </a>
+
+## Cite us
+If you find RL4CO valuable for your research or applied projects:
+
+```bibtex
+@article{berto2023rl4co,
+    title = {{RL4CO}: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark},
+    author={Federico Berto and Chuanbo Hua and Junyoung Park and Minsu Kim and Hyeonah Kim and Jiwoo Son and Haeyeon Kim and Joungho Kim and Jinkyoo Park},
+    journal={arXiv preprint arXiv:2306.17100},
+    year={2023},
+    url = {https://github.com/kaist-silab/rl4co}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rl4co-0.0.3.dev3/rl4co.egg-info/SOURCES.txt` & `rl4co-0.0.4/rl4co.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 rl4co.egg-info/top_level.txt
 rl4co/data/__init__.py
 rl4co/data/dataset.py
 rl4co/data/generate_data.py
 rl4co/data/utils.py
 rl4co/envs/__init__.py
 rl4co/envs/atsp.py
-rl4co/envs/base.py
 rl4co/envs/cvrp.py
 rl4co/envs/dpp.py
 rl4co/envs/ffsp.py
 rl4co/envs/mdpp.py
 rl4co/envs/mtsp.py
 rl4co/envs/op.py
 rl4co/envs/pctsp.py
 rl4co/envs/pdp.py
 rl4co/envs/sdvrp.py
+rl4co/envs/spctsp.py
 rl4co/envs/tsp.py
-rl4co/envs/utils.py
+rl4co/envs/common/base.py
+rl4co/envs/common/utils.py
 rl4co/models/__init__.py
 rl4co/models/nn/attention.py
 rl4co/models/nn/env_context.py
 rl4co/models/nn/env_embedding.py
 rl4co/models/nn/flash_attention.py
 rl4co/models/nn/mlp.py
 rl4co/models/nn/ops.py
```

### Comparing `rl4co-0.0.3.dev3/tests/test_envs.py` & `rl4co-0.0.4/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/tests/test_models.py` & `rl4co-0.0.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.3.dev3/tests/test_ops.py` & `rl4co-0.0.4/tests/test_ops.py`

 * *Files identical despite different names*

