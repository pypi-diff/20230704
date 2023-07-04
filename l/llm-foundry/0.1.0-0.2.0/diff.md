# Comparing `tmp/llm-foundry-0.1.0.tar.gz` & `tmp/llm-foundry-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-foundry-0.1.0.tar", last modified: Wed May 10 20:23:36 2023, max compression
+gzip compressed data, was "llm-foundry-0.2.0.tar", last modified: Tue Jul  4 05:35:49 2023, max compression
```

## Comparing `llm-foundry-0.1.0.tar` & `llm-foundry-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.424291 llm-foundry-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-05-10 20:23:36.424291 llm-foundry-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.416288 llm-foundry-0.1.0/llm_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-05-10 20:23:36.000000 llm-foundry-0.1.0/llm_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-10 20:23:36.000000 llm-foundry-0.1.0/llm_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:23:36.000000 llm-foundry-0.1.0/llm_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-10 20:23:36.000000 llm-foundry-0.1.0/llm_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 20:23:36.000000 llm-foundry-0.1.0/llm_foundry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.416288 llm-foundry-0.1.0/llmfoundry/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.416288 llm-foundry-0.1.0/llmfoundry/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/callbacks/fdiff_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/callbacks/generate_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/callbacks/monolithic_ckpt_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/callbacks/resumption_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/callbacks/scheduled_gc_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.416288 llm-foundry-0.1.0/llmfoundry/data/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    42791 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/denoising.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.416288 llm-foundry-0.1.0/llmfoundry/data/finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/finetuning/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/finetuning/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/finetuning/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/data/text_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.416288 llm-foundry-0.1.0/llmfoundry/models/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.420290 llm-foundry-0.1.0/llmfoundry/models/hf/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/hf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/hf/hf_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/hf/hf_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/hf/hf_prefix_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/hf/hf_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/hf/model_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.420290 llm-foundry-0.1.0/llmfoundry/models/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20632 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/layers/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/layers/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/model_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.420290 llm-foundry-0.1.0/llmfoundry/models/mpt/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/mpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/mpt/configuration_mpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    28795 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/mpt/modeling_mpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.420290 llm-foundry-0.1.0/llmfoundry/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/utils/adapt_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    38878 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/utils/hf_prefixlm_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/utils/meta_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/models/utils/param_init_fns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.424291 llm-foundry-0.1.0/llmfoundry/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19592 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/optim/adaptive_lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/optim/outlier_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.424291 llm-foundry-0.1.0/llmfoundry/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10805 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/utils/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/llmfoundry/utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:23:36.424291 llm-foundry-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-10 20:23:16.000000 llm-foundry-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:23:36.424291 llm-foundry-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_data_prep_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_flash_triton_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_hf_v_mpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_icl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_init_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    44042 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-10 20:23:15.000000 llm-foundry-0.1.0/tests/test_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.389423 llm-foundry-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-04 05:35:49.389423 llm-foundry-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.377421 llm-foundry-0.2.0/llm_foundry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-04 05:35:49.000000 llm-foundry-0.2.0/llm_foundry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-04 05:35:49.000000 llm-foundry-0.2.0/llm_foundry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:35:49.000000 llm-foundry-0.2.0/llm_foundry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-04 05:35:49.000000 llm-foundry-0.2.0/llm_foundry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 05:35:49.000000 llm-foundry-0.2.0/llm_foundry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.377421 llm-foundry-0.2.0/llmfoundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.377421 llm-foundry-0.2.0/llmfoundry/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/callbacks/fdiff_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/callbacks/generate_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/callbacks/model_gauntlet_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/callbacks/monolithic_ckpt_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/callbacks/resumption_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/callbacks/scheduled_gc_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.381422 llm-foundry-0.2.0/llmfoundry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42800 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/denoising.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.381422 llm-foundry-0.2.0/llmfoundry/data/finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/finetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/finetuning/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/finetuning/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/finetuning/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/data/text_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.381422 llm-foundry-0.2.0/llmfoundry/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.381422 llm-foundry-0.2.0/llmfoundry/models/hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/hf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/hf/hf_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/hf/hf_fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/hf/hf_prefix_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/hf/hf_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/hf/model_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.385422 llm-foundry-0.2.0/llmfoundry/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/layers/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/layers/custom_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38355 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/layers/flash_attn_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/layers/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/model_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.385422 llm-foundry-0.2.0/llmfoundry/models/mpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/mpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/mpt/configuration_mpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31099 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/mpt/modeling_mpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.385422 llm-foundry-0.2.0/llmfoundry/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/utils/adapt_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38878 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/utils/hf_prefixlm_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/utils/meta_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/models/utils/param_init_fns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.385422 llm-foundry-0.2.0/llmfoundry/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19592 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/optim/adaptive_lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/optim/outlier_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.385422 llm-foundry-0.2.0/llmfoundry/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/utils/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/llmfoundry/utils/huggingface_hub_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15361 2023-07-04 05:35:32.000000 llm-foundry-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 05:35:49.389423 llm-foundry-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:49.389423 llm-foundry-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_data_prep_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_flash_triton_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_hf_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_hf_conversion_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_hf_mpt_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_hf_v_mpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_icl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_init_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52269 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-04 05:35:33.000000 llm-foundry-0.2.0/tests/test_training.py
```

### Comparing `llm-foundry-0.1.0/LICENSE` & `llm-foundry-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llm_foundry.egg-info/SOURCES.txt` & `llm-foundry-0.2.0/llm_foundry.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 llm_foundry.egg-info/dependency_links.txt
 llm_foundry.egg-info/requires.txt
 llm_foundry.egg-info/top_level.txt
 llmfoundry/__init__.py
 llmfoundry/callbacks/__init__.py
 llmfoundry/callbacks/fdiff_callback.py
 llmfoundry/callbacks/generate_callback.py
+llmfoundry/callbacks/model_gauntlet_callback.py
 llmfoundry/callbacks/monolithic_ckpt_callback.py
 llmfoundry/callbacks/resumption_callbacks.py
 llmfoundry/callbacks/scheduled_gc_callback.py
 llmfoundry/data/__init__.py
-llmfoundry/data/datasets.py
+llmfoundry/data/data.py
 llmfoundry/data/denoising.py
 llmfoundry/data/packing.py
 llmfoundry/data/text_data.py
 llmfoundry/data/finetuning/__init__.py
 llmfoundry/data/finetuning/collator.py
 llmfoundry/data/finetuning/dataloader.py
 llmfoundry/data/finetuning/tasks.py
@@ -30,14 +31,16 @@
 llmfoundry/models/hf/hf_fsdp.py
 llmfoundry/models/hf/hf_prefix_lm.py
 llmfoundry/models/hf/hf_t5.py
 llmfoundry/models/hf/model_wrapper.py
 llmfoundry/models/layers/__init__.py
 llmfoundry/models/layers/attention.py
 llmfoundry/models/layers/blocks.py
+llmfoundry/models/layers/custom_embedding.py
+llmfoundry/models/layers/flash_attn_triton.py
 llmfoundry/models/layers/norm.py
 llmfoundry/models/mpt/__init__.py
 llmfoundry/models/mpt/configuration_mpt.py
 llmfoundry/models/mpt/modeling_mpt.py
 llmfoundry/models/utils/__init__.py
 llmfoundry/models/utils/adapt_tokenizer.py
 llmfoundry/models/utils/hf_prefixlm_converter.py
@@ -46,17 +49,21 @@
 llmfoundry/optim/__init__.py
 llmfoundry/optim/adaptive_lion.py
 llmfoundry/optim/lion.py
 llmfoundry/optim/outlier_detection.py
 llmfoundry/utils/__init__.py
 llmfoundry/utils/builders.py
 llmfoundry/utils/config_utils.py
+llmfoundry/utils/huggingface_hub_utils.py
 tests/test_data_prep_scripts.py
 tests/test_dataloader.py
 tests/test_flash_triton_torch.py
+tests/test_hf_config.py
+tests/test_hf_conversion_script.py
+tests/test_hf_mpt_gen.py
 tests/test_hf_v_mpt.py
 tests/test_icl_datasets.py
 tests/test_init_fn.py
 tests/test_model.py
 tests/test_onnx.py
 tests/test_tokenizer.py
 tests/test_training.py
```

### Comparing `llm-foundry-0.1.0/llmfoundry/__init__.py` & `llm-foundry-0.2.0/llmfoundry/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
-try:
-    import torch
+import torch
 
+try:
     from llmfoundry import optim, utils
     from llmfoundry.data import (ConcatTokensDataset,
                                  MixtureOfDenoisersCollator, NoConcatDataset,
                                  Seq2SeqFinetuningCollator,
                                  build_finetuning_dataloader,
                                  build_text_denoising_dataloader)
     from llmfoundry.models.hf import (ComposerHFCausalLM, ComposerHFPrefixLM,
@@ -20,15 +20,15 @@
     from llmfoundry.models.model_registry import COMPOSER_MODEL_REGISTRY
     from llmfoundry.models.mpt import (ComposerMPTCausalLM, MPTConfig,
                                        MPTForCausalLM, MPTModel,
                                        MPTPreTrainedModel)
 
 except ImportError as e:
     try:
-        is_cuda_available = torch.cuda.is_available()  # type: ignore
+        is_cuda_available = torch.cuda.is_available()
     except:
         is_cuda_available = False
 
     extras = '.[gpu]' if is_cuda_available else '.'
     raise ImportError(
         f'Please make sure to pip install {extras} to get the requirements for the LLM example.'
     ) from e
@@ -58,8 +58,8 @@
     'attn_bias_shape',
     'build_attn_bias',
     'build_alibi_bias',
     'optim',
     'utils',
 ]
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

### Comparing `llm-foundry-0.1.0/llmfoundry/callbacks/__init__.py` & `llm-foundry-0.2.0/llmfoundry/callbacks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 try:
     from llmfoundry.callbacks.fdiff_callback import FDiffMetrics
     from llmfoundry.callbacks.generate_callback import Generate
+    from llmfoundry.callbacks.model_gauntlet_callback import ModelGauntlet
     from llmfoundry.callbacks.monolithic_ckpt_callback import \
         MonolithicCheckpointSaver
     from llmfoundry.callbacks.resumption_callbacks import (GlobalLRScaling,
                                                            LayerFreezing)
     from llmfoundry.callbacks.scheduled_gc_callback import \
         ScheduledGarbageCollector
 except ImportError as e:
@@ -18,8 +19,9 @@
 __all__ = [
     'FDiffMetrics',
     'Generate',
     'MonolithicCheckpointSaver',
     'GlobalLRScaling',
     'LayerFreezing',
     'ScheduledGarbageCollector',
+    'ModelGauntlet',
 ]
```

### Comparing `llm-foundry-0.1.0/llmfoundry/callbacks/fdiff_callback.py` & `llm-foundry-0.2.0/llmfoundry/callbacks/fdiff_callback.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,21 +43,23 @@
             for k in state.train_metric_values.keys():
                 value = state.train_metric_values[k]
                 self.train_prev_metric[k] = value
 
     def eval_end(self, state: State, logger: Logger):
         if self.diff_eval_metrics:
             evaluator = state.dataloader_label
-            metrics = list(state.eval_metrics[evaluator].keys())  # type: ignore
+            assert evaluator is not None, 'dataloader should have been set'
+
+            metrics = list(state.eval_metrics[evaluator].keys())
 
             for k in metrics:
-                mkey = '/'.join(['metrics', evaluator, k])  # type: ignore
+                mkey = '/'.join(['metrics', evaluator, k])
                 if mkey in self.eval_prev_metric.keys():
                     logger.log_metrics({
                         f'{mkey}_fdiff':
                             state.eval_metric_values[k] -
                             self.eval_prev_metric[mkey]
                     })
 
             for k in metrics:
-                mkey = '/'.join(['metrics', evaluator, k])  # type: ignore
+                mkey = '/'.join(['metrics', evaluator, k])
                 self.eval_prev_metric[mkey] = state.eval_metric_values[k]
```

### Comparing `llm-foundry-0.1.0/llmfoundry/callbacks/generate_callback.py` & `llm-foundry-0.2.0/llmfoundry/callbacks/generate_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Periodically log generations to wandb from a set of prompts."""
 from typing import List, Union, cast
 
 import torch
 import wandb
-from composer.core import Callback, State
+from composer.core import Callback, State, get_precision_context
 from composer.loggers import Logger, WandBLogger
 from composer.utils import dist, ensure_tuple
 from transformers import PreTrainedTokenizer, PreTrainedTokenizerFast
 
 Tokenizer = Union[PreTrainedTokenizer, PreTrainedTokenizerFast]
 
 
@@ -68,29 +68,32 @@
 
         for k, v in tokenized_input.items():
             tokenized_input[k] = device.tensor_to_device(v)
 
         # dummy forward call needed for FSDP to work consistently
         dummy_input = torch.tensor([[0]], dtype=torch.long)
         dummy_input = device.tensor_to_device(dummy_input)
-        with torch.no_grad():
-            _ = model.model(input_ids=dummy_input)  # type: ignore
-
-        output_token_ids = model.model.generate(  # type: ignore
-            input_ids=tokenized_input['input_ids'],
-            attention_mask=tokenized_input['attention_mask'],
-            synced_gpus=True,
-            **self.generate_kwargs,
-        )
+        with get_precision_context(state.precision):
+            with torch.no_grad():
+                _ = model.model(input_ids=dummy_input)
+
+            output_token_ids = model.model.generate(
+                input_ids=tokenized_input['input_ids'],
+                attention_mask=tokenized_input['attention_mask'],
+                synced_gpus=True,
+                **self.generate_kwargs,
+            )
 
         if dist.get_global_rank() == 0:
             if self.wandb_logger is not None:
-                artifact = wandb.Artifact(
-                    'generate_samples_' + str(wandb.run.id),  # type: ignore
-                    type='predictions')
+                assert wandb.run is not None, 'wandb should have started run'
+
+                artifact = wandb.Artifact('generate_samples_' +
+                                          str(wandb.run.id),
+                                          type='predictions')
 
                 rows = []
                 for i in range(len(self.prompts)):
                     prompt = self.prompts[i]
                     output_tokens = output_token_ids[i][
                         tokenized_input['input_ids'].shape[1]:]
                     output_text = tokenizer.decode(output_tokens,
```

### Comparing `llm-foundry-0.1.0/llmfoundry/callbacks/monolithic_ckpt_callback.py` & `llm-foundry-0.2.0/llmfoundry/callbacks/monolithic_ckpt_callback.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import contextlib
 import os
 import tempfile
 from pathlib import Path
 
 import torch
 from composer.core import Callback, State
-from composer.core.state import fsdp_state_dict_type_context
+from composer.core.state import (fsdp_get_optim_state_dict,
+                                 fsdp_state_dict_type_context)
 from composer.loggers import Logger
 from composer.loggers.remote_uploader_downloader import RemoteUploaderDownloader
 from composer.utils import (dist, format_name_with_dist_and_time, parse_uri,
                             reproducibility)
 
 
 class MonolithicCheckpointSaver(Callback):
@@ -75,21 +76,35 @@
             dirname = os.path.dirname(save_path)
             if dirname:
                 os.makedirs(dirname, exist_ok=True)
             state_dict = {
                 'state': state.state_dict(),
                 'rng': reproducibility.get_rng_state()
             }
-            if not self.keep_optimizers:
-                state_dict['state'].pop('optimizers')
+            # Remove sharded model and optimizer state dicts
+            state_dict['state'].pop('optimizers')
+            state_dict['state'].pop('model')
+
+            # Add in unsharded model params.
             with fsdp_state_dict_type_context(state.model,
                                               state_dict_type='full'):
                 state_dict['state']['model'] = state.model.state_dict()
-                if dist.get_global_rank() == 0:
-                    torch.save(state_dict, save_path)
+
+            # Add in unsharded optimizer state dict.
+            if self.keep_optimizers:
+                optimizer = state.optimizers[0]
+                state_dict['state']['optimizers'] = {
+                    type(optimizer).__qualname__:
+                        fsdp_get_optim_state_dict(state.model,
+                                                  optimizer,
+                                                  state_dict_type='full')
+                }
+            if dist.get_global_rank() == 0:
+                torch.save(state_dict, save_path)
+
             if self.upload_to_object_store and self.remote_ud is not None and dist.get_global_rank(
             ) == 0:
                 remote_file_name = str(Path(save_dir) / Path(filename))
                 self.remote_ud.upload_file(state=state,
                                            remote_file_name=remote_file_name,
                                            file_path=Path(save_path),
                                            overwrite=self.overwrite)
```

### Comparing `llm-foundry-0.1.0/llmfoundry/callbacks/resumption_callbacks.py` & `llm-foundry-0.2.0/llmfoundry/callbacks/resumption_callbacks.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/callbacks/scheduled_gc_callback.py` & `llm-foundry-0.2.0/llmfoundry/callbacks/scheduled_gc_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/data/__init__.py` & `llm-foundry-0.2.0/llmfoundry/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
-from llmfoundry.data.datasets import ConcatTokensDataset, NoConcatDataset
+from llmfoundry.data.data import ConcatTokensDataset, NoConcatDataset
 from llmfoundry.data.denoising import (MixtureOfDenoisersCollator,
                                        build_text_denoising_dataloader)
 from llmfoundry.data.finetuning import (Seq2SeqFinetuningCollator,
                                         build_finetuning_dataloader)
 from llmfoundry.data.text_data import (StreamingTextDataset,
                                        build_text_dataloader)
```

### Comparing `llm-foundry-0.1.0/llmfoundry/data/datasets.py` & `llm-foundry-0.2.0/llmfoundry/data/data.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/data/denoising.py` & `llm-foundry-0.2.0/llmfoundry/data/denoising.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         return batch
 
 
 def build_text_denoising_dataloader(
     cfg: DictConfig,
     tokenizer: Tokenizer,
     device_batch_size: int,
-) -> DataLoader:
+) -> DataLoader[Dict]:
     """Constructor function for a Mixture of Denoisers dataloader.
 
     This function constructs a dataloader that can be used to train an
     encoder-decoder model or a (prefix LM) decoder-only model on a text
     denoising task mixture (e.g. span corruption, or UL2).
 
     The underlying dataset is a :class:`StreamingTextDataset`, allowing you to
@@ -476,15 +476,15 @@
         download_timeout=cfg.dataset.get('download_timeout', 60),
         validate_hash=cfg.dataset.get('validate_hash'),
         shuffle_seed=cfg.dataset.get('shuffle_seed', 9176),
         num_canonical_nodes=cfg.dataset.get('num_canonical_nodes', 128),
         batch_size=device_batch_size,
     )
 
-    if dataset.tokenizer.pad_token is None:  # type: ignore
+    if dataset.tokenizer.pad_token is None:
         dataset.tokenizer.pad_token = dataset.tokenizer.eos_token
 
     if cfg.dataset.get('packing_ratio'):
         n_examples_to_pack = int(device_batch_size * cfg.dataset.packing_ratio)
         if n_examples_to_pack < device_batch_size:
             raise ValueError('packing_ratio must be >= 1, if supplied')
         if not cfg.mixture_of_denoisers.decoder_only_format:
@@ -560,15 +560,15 @@
         # trimming to max_seq_length won't cut off any <EOS> token.
         # In the decoder-only case, this won't insert new tokens.
         if mask_ratio <= 0.5:
             u = np.random.uniform(low=0.0, high=mask_ratio * 2)
         else:
             u = np.random.uniform(low=(mask_ratio * 2) - 1, high=1.0)
         mean_span_length = float(np.round(1 + u * (length - 1)))
-        mask_ratio = mean_span_length / length  # type: ignore
+        mask_ratio = mean_span_length / length
         use_sentinels = False
     else:
         use_sentinels = True
 
     # Generate the mask
     # Note: this function can be used for all the UL2 noising functions
     mask = _sample_mask_array(length, mask_ratio, mean_span_length)
@@ -867,17 +867,17 @@
         'kwargs': {}
     }
     tokenizer_cfg['kwargs'] = {'model_max_length': cfg.dataset.max_seq_len}
     tokenizer_cfg = om.create(tokenizer_cfg)
     tokenizer = build_tokenizer(tokenizer_cfg)
 
     loader = build_text_denoising_dataloader(cfg, tokenizer, device_batch_size)
+    assert isinstance(loader.dataset, StreamingTextDataset)
 
-    print(
-        f'\n\nTRUNCATING TO: {loader.dataset.max_seq_len}\n\n')  # type: ignore
+    print(f'\n\nTRUNCATING TO: {loader.dataset.max_seq_len}\n\n')
 
     packing = cfg.dataset.get('packing_ratio') is not None
     if packing:
         tokenizer = loader.collate_fn.base_collator.tokenizer
     else:
         tokenizer = loader.collate_fn.tokenizer
     batch_ix = 0
```

### Comparing `llm-foundry-0.1.0/llmfoundry/data/finetuning/collator.py` & `llm-foundry-0.2.0/llmfoundry/data/finetuning/collator.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/data/finetuning/dataloader.py` & `llm-foundry-0.2.0/llmfoundry/data/finetuning/dataloader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 import logging
+import os
+import tempfile
 from typing import Union
 
 import torch
-from composer.utils import dist
+from composer.utils import dist, get_file, parse_uri
 from omegaconf import DictConfig
 from torch.utils.data import DataLoader
 from transformers import PreTrainedTokenizer, PreTrainedTokenizerFast
 
 from llmfoundry.data.finetuning.collator import Seq2SeqFinetuningCollator
 from llmfoundry.data.finetuning.tasks import dataset_constructor
 from llmfoundry.data.packing import BinPackWrapper
@@ -34,15 +36,17 @@
 
     Args:
         cfg (DictConfig): An omegaconf dictionary used to configure the loader:
             cfg.name (str): The type of dataloader to build. Must = "finetuning".
             ---
             *** HuggingFace dataset config fields ***
             cfg.dataset.hf_name (str, optional): The name of the HuggingFace dataset
-                to use.
+                to use. Can also be a remote http(s) directory or object store bucket
+                containing the file {split}.jsonl in the format (prompt, response),
+                in which case the builder will create a HuggingFace dataset.
             cfg.dataset.hf_kwargs (DictConfig, optional): Additional kwargs to
                 pass to `datasets.load_dataset`, which can be used to load
                 a dataset from local files.
             cfg.dataset.preprocessing_fn (str, optional): The name/import path of
                 the preprocessing function to use for formatting the data examples.
                 If ``None`` (default), the builder will use the preprocessing function
                     registered under `hf_name` (see `tasks.py`), if one exists,
@@ -82,15 +86,15 @@
                     packing.
                     Select `packing_ratio` **carefully** based on the dataset
                     statistics, `max_seq_len`, and tolerance for discarding samples!
                     The packing code in `../packing.py` provides a script that can help
                     you choose the best `packing_ratio`.
             cfg.dataset.shuffle (bool): Whether to shuffle the dataset.
             ___
-            See :class:`StreamingTextDataset` for info on other standard config
+            See :class:`StreamingFinetuningDataset` for info on other standard config
                 options within `cfg.dataset` that will be passed as kwargs if
                 using the streaming codepath.
             ---
             See :class:`DataLoader` for standard argument options to the pytorch
                 dataloader, such as `cfg.drop_last`, `cfg.num_workers`, etc.
         tokenizer (transformers.PreTrainedTokenizer): The tokenizer used to
             prepare the data from raw text. Any missing sentinel tokens will
@@ -116,15 +120,15 @@
         dataset = dataset_constructor.build_from_streaming(
             tokenizer=tokenizer,
             local=cfg.dataset.local,
             remote=cfg.dataset.get('remote', None),
             split=cfg.dataset.get('split'),
             shuffle=cfg.dataset.get('shuffle', False),
             predownload=cfg.dataset.get('predownload', 100_000),
-            keep_zip=cfg.dataset.get('keep_zip', None),
+            keep_zip=cfg.dataset.get('keep_zip', False),
             download_retry=cfg.dataset.get('download_retry', 2),
             download_timeout=cfg.dataset.get('download_timeout', 60),
             validate_hash=cfg.dataset.get('validate_hash', None),
             shuffle_seed=cfg.dataset.get('shuffle_seed', 9176),
             num_canonical_nodes=cfg.dataset.get('num_canonical_nodes', 128),
             batch_size=device_batch_size,
         )
@@ -141,15 +145,61 @@
             pin_memory=cfg.get('pin_memory', True),
             prefetch_factor=cfg.get('prefetch_factor', 2),
             persistent_workers=cfg.get('persistent_workers', True),
             timeout=cfg.get('timeout', 0),
         )
 
     else:
-        dataset = dataset_constructor.build_from_hf(cfg.dataset, tokenizer)
+        backend, _, _ = parse_uri(cfg.dataset.hf_name)
+        if backend not in ['', None]:
+            if cfg.dataset.get('split') is None:
+                raise ValueError(
+                    'When using a HuggingFace dataset from a URL, you must set the ' + \
+                    '`split` key in the dataset config.'
+                )
+            supported_extensions = ['jsonl', 'csv', 'parquet']
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                for extension in supported_extensions:
+                    name = f'{cfg.dataset.hf_name.strip("/")}/{cfg.dataset.split}.{extension}'
+                    destination = str(
+                        os.path.abspath(
+                            f'{tmp_dir}/{cfg.dataset.split}.{extension}'))
+                    try:
+                        with dist.run_local_rank_zero_first():
+                            get_file(name, destination, overwrite=True)
+                    except FileNotFoundError as e:
+                        if extension == supported_extensions[-1]:
+                            raise FileNotFoundError(
+                                f'Could not find a {cfg.dataset.split} file with any of ' + \
+                                f'the supported extensions: {supported_extensions}\n' + \
+                                f'at {cfg.dataset.hf_name}/{cfg.dataset.split}'
+                            ) from e
+                        else:
+                            print(
+                                f'Could not find {name}, looking for another extension'
+                            )
+                        continue
+                    # 'json' causes special behavior in the dataset constructor
+                    cfg.dataset.hf_name = extension if extension != 'jsonl' else 'json'
+                    kwargs = cfg.dataset.get('hf_kwargs', {})
+                    kwargs['data_files'] = destination
+                    cfg.dataset['hf_kwargs'] = kwargs
+                    print(cfg.dataset)
+                    dataset = dataset_constructor.build_from_hf(
+                        cfg.dataset,
+                        max_seq_len=cfg.dataset.max_seq_len,
+                        tokenizer=tokenizer,
+                    )
+                    break
+        else:
+            dataset = dataset_constructor.build_from_hf(
+                cfg.dataset,
+                max_seq_len=cfg.dataset.max_seq_len,
+                tokenizer=tokenizer,
+            )
 
         collate_fn, dataloader_batch_size = _build_collate_fn(
             cfg.dataset, tokenizer, device_batch_size)
 
         return DataLoader(
             dataset,
             collate_fn=collate_fn,
@@ -202,15 +252,15 @@
         if discovered_illegal_keys:
             raise ValueError(
                 'The dataset config sets a value for `remote` as well as the ' +\
                 f'following keys: {", ".join(discovered_illegal_keys)}.\n' +\
                 'Those keys are used when building from a HuggingFace dataset, but ' +\
                 'setting `remote` instructs the dataset to build from a streaming dataset.'
             )
-        if dataset_cfg.get('local') is not None:
+        if dataset_cfg.get('local') is None:
             raise ValueError(
                 'Using a streaming dataset requires setting both `remote` and `local`, ' +\
                 'but dataset.local is None.'
             )
     else:
         raise ValueError(
             'In the dataset config, you must set either `hf_name` to use a ' +\
```

### Comparing `llm-foundry-0.1.0/llmfoundry/data/finetuning/tasks.py` & `llm-foundry-0.2.0/llmfoundry/data/finetuning/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,17 +29,18 @@
 The key requirement of these functions is that they return a dictionary
 with "prompt" and "response" keys, and that the values associated with
 those keys are strings (i.e. text).
 """
 
 import importlib
 import os
+import warnings
 from typing import Any, Callable, Dict, Optional, Union
 
-import datasets
+import datasets as hf_datasets
 from omegaconf import DictConfig
 from streaming import StreamingDataset
 from transformers import PreTrainedTokenizer, PreTrainedTokenizerFast
 
 __all__ = ['dataset_constructor']
 
 Tokenizer = Union[PreTrainedTokenizer, PreTrainedTokenizerFast]
@@ -86,26 +87,26 @@
     def __init__(self,
                  local: str,
                  tokenizer: Tokenizer,
                  remote: Optional[str] = None,
                  split: Optional[str] = None,
                  shuffle: bool = False,
                  predownload: Optional[int] = 100_000,
-                 keep_zip: Optional[bool] = None,
+                 keep_zip: bool = False,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  shuffle_seed: int = 9176,
                  num_canonical_nodes: Optional[int] = 128,
                  batch_size: Optional[int] = None,
                  **kwargs: Any):
 
         if len(kwargs) > 0:
             raise ValueError(
-                f'StreamingTextDataset() got an unexpected keyword argument: {kwargs}'
+                f'StreamingFinetuningDataset() got an unexpected keyword argument: {kwargs}'
             )
 
         if remote is None or (local == remote):
             if os.path.isdir(local):
                 contents = set(os.listdir(local))
                 if split not in contents:
                     raise ValueError(
@@ -157,14 +158,48 @@
 
         return wrapper
 
     def print_registered_tasks(self):
         tasks = sorted(self._task_preprocessing_registry.keys())
         print('\n'.join(tasks))
 
+    def get_preprocessing_fn_from_dict(self, mapping: dict):
+        """Get a preprocessing function from a dictionary.
+
+        The dictionary maps column names in the dataset to "prompt" and "response".
+        For example,
+            ```yaml
+            preprocessing_fn:
+                prompt: text
+                response: summary
+            ```
+        would map the `text` column as to prompt and the `summary` column as the response.
+
+        Args:
+            mapping (dict): A dictionary mapping column names to "prompt" and "response".
+
+        Returns:
+            Callable: The preprocessing function.
+
+        Raises:
+            ValueError: If the mapping does not have keys "prompt" and "response".
+        """
+
+        def _preprocessor(example: Dict[str, Any]) -> Dict[str, str]:
+            if list(mapping.keys()) != ['prompt', 'response']:
+                raise ValueError(
+                    f'Expected {mapping=} to have keys "prompt" and "response".'
+                )
+            return {
+                'prompt': example[mapping['prompt']],
+                'response': example[mapping['response']]
+            }
+
+        return _preprocessor
+
     def get_preprocessing_fn_from_str(self,
                                       preprocessor: Optional[str],
                                       dataset_name: Optional[str] = None,
                                       verbose: bool = False):
         """Get a preprocessing function from a string.
 
         String can be either a registered function or an import path.
@@ -216,45 +251,64 @@
         except Exception as e:
             raise ValueError(
                 f'Failed to import preprocessing function from string = {preprocessor}.'
             ) from e
 
         return preprocessing_fn
 
-    def build_from_hf(self, cfg: DictConfig, tokenizer: Tokenizer):
+    def build_from_hf(self, cfg: DictConfig, max_seq_len: int,
+                      tokenizer: Tokenizer):
         """Load a HuggingFace Datasets, preprocess, and tokenize.
 
+        Note: This function will drop examples where the prompt is longer than the max_seq_len
+
         Args:
             cfg (DictConfig): The dataset configuration.
+            max_seq_len (int): The maximum sequence length. Examples with prompts longer than this will be dropped.
             tokenizer (Tokenizer): The tokenizer to be used for tokenizing the dataset.
 
         Returns:
             Dataset: The tokenized dataset.
         """
         dataset_name = cfg.hf_name
         split = cfg.split
         kwargs = cfg.get('hf_kwargs', {})
-        preprocessing_fn = self.get_preprocessing_fn_from_str(
-            cfg.get('preprocessing_fn'), dataset_name, verbose=True)
+        proto_preprocessing_fn = cfg.get('preprocessing_fn')
+        if isinstance(proto_preprocessing_fn, dict) or isinstance(
+                proto_preprocessing_fn, DictConfig):
+            preprocessing_fn = self.get_preprocessing_fn_from_dict(
+                proto_preprocessing_fn)
+        else:
+            preprocessing_fn = self.get_preprocessing_fn_from_str(
+                proto_preprocessing_fn, dataset_name, verbose=True)
 
-        dataset = datasets.load_dataset(dataset_name, split=split, **kwargs)
+        dataset = hf_datasets.load_dataset(dataset_name, split=split, **kwargs)
 
         def dataset_mapper(example: Dict):
             if preprocessing_fn is not None:
                 example = preprocessing_fn(example)
             return _tokenize_formatted_example(example, tokenizer)
 
         columns_to_remove = list(dataset[0].keys())
         tokenized_dataset = dataset.map(
             dataset_mapper,
             batched=False,
             remove_columns=columns_to_remove,
         )
+        prompt_length_filtered_dataset = tokenized_dataset.filter(
+            lambda example: len(example['input_ids']) < max_seq_len)
+
+        examples_removed = len(tokenized_dataset) - len(
+            prompt_length_filtered_dataset)
+        if examples_removed > 0:
+            warnings.warn(
+                f'Dropped {examples_removed} examples where the prompt was longer than {max_seq_len}.'
+            )
 
-        return tokenized_dataset
+        return prompt_length_filtered_dataset
 
     def build_from_streaming(self, *args: Any, **kwargs: Any):
         return StreamingFinetuningDataset(*args, **kwargs)
 
 
 dataset_constructor = DatasetConstructor()
```

### Comparing `llm-foundry-0.1.0/llmfoundry/data/packing.py` & `llm-foundry-0.2.0/llmfoundry/data/packing.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/data/text_data.py` & `llm-foundry-0.2.0/llmfoundry/data/text_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,53 +41,59 @@
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
             `False``.
-        keep_raw (bool): Whether to keep or delete the decompressed form (or only form)
-            of shards after all their samples have been yielded this epoch. If ``False``, keep iff
-            remote is local or no remote and no compression. Defaults to ``True``.
-        samples_per_epoch (int, optional): Provide this field iff you are weighting sub-datasets
-            proportionally. Defaults to ``None``.
+        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+            streams. If ``None``, takes its value from the total number of underlying samples.
+            Provide this field if you are weighting streams relatively to target a larger or
+            smaller epoch size. Defaults to ``None``.
         predownload (int, optional): Target number of samples ahead to download the shards of while
             iterating. Defaults to ``100_000``.
+        cache_limit (Union[int, str], optional) - Maximum size in bytes of this StreamingDataset's
+            shard cache. Before downloading a shard, the least recently used resident shard(s) may
+            be evicted (deleted from the local cache) in order to stay under the limit. Set to None
+            to disable shard eviction. Supports integer bytes as well as string human-readable
+            bytes (e.g., 100b, 64kb, 77mb, and so on). Defaults to None.
         partition_algo (str): Which partitioning algorithm to use. Defaults to ``orig``.
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
     """
 
     def __init__(self,
                  tokenizer: Tokenizer,
                  max_seq_len: int,
                  streams: Optional[Sequence[Stream]] = None,
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 keep_raw: bool = True,
-                 samples_per_epoch: Optional[int] = None,
+                 epoch_size: Optional[int] = None,
                  predownload: int = 100_000,
+                 cache_limit: Optional[Union[int, str]] = None,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
+                 shuffle_algo: str = 'py1b',
                  shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18,
                  **kwargs: Dict[str, Any]):
 
         group_method = kwargs.pop('group_method', None)
         if group_method is not None:
             raise NotImplementedError(
                 'group_method is deprecated and has been removed.\nTo ' +
                 'concatenate, use the --concat_tokens ' +
@@ -112,17 +118,17 @@
             remote=remote,
             local=local,
             split=split,
             download_retry=download_retry,
             download_timeout=download_timeout,
             validate_hash=validate_hash,
             keep_zip=keep_zip,
-            keep_raw=keep_raw,
-            samples_per_epoch=samples_per_epoch,
+            epoch_size=epoch_size,
             predownload=predownload,
+            cache_limit=cache_limit,
             partition_algo=partition_algo,
             num_canonical_nodes=num_canonical_nodes,
             batch_size=batch_size,
             shuffle=shuffle,
             shuffle_algo=shuffle_algo,
             shuffle_seed=shuffle_seed,
         )
@@ -216,74 +222,41 @@
     if cfg.dataset.get('group_method', None) is not None:
         raise NotImplementedError(
             'group_method is deprecated and has been removed.\nTo ' +
             'concatenate, use the --concat_tokens ' +
             'argument when creating your MDS dataset with convert_dataset_hf.py'
         )
 
+    # get kwargs
+    streams_dict = cfg.dataset.pop('streams', None)
+    mlm_probability = cfg.dataset.pop('mlm_probability', None)
+    eos_token_id = cfg.dataset.pop('eos_token_id', None)
+    bos_token_id = cfg.dataset.pop('bos_token_id', None)
+
     # build streams
-    streams_dict = cfg.dataset.get('streams', None)
     streams = None
     if streams_dict is not None:
         streams = []
         for _, stream in streams_dict.items():
-            streams.append(
-                Stream(
-                    remote=stream.get('remote', None) or
-                    cfg.dataset.get('remote', None),
-                    local=stream.get('local', None) or
-                    cfg.dataset.get('local', None),
-                    split=stream.get('split', None) or
-                    cfg.dataset.get('split', None),
-                    proportion=stream.get('proportion', None),
-                    repeat=stream.get('repeat', None),
-                    samples=stream.get('samples', None),
-                    download_retry=stream.get('download_retry', None) or
-                    cfg.dataset.get('download_retry', 2),
-                    download_timeout=stream.get('download_timeout', None) or
-                    cfg.dataset.get('download_timeout', 60),
-                    validate_hash=stream.get('validate_hash', None) or
-                    cfg.dataset.get('validate_hash', None),
-                    keep_zip=stream.get('keep_zip', None) or
-                    cfg.dataset.get('keep_zip', False),
-                    keep_raw=stream.get('keep_raw', None) or
-                    cfg.dataset.get('keep_raw', True),
-                ))
+            # stream is the streams kwargs
+            # fwd all kwargs with **stream allows streaming to check args
+            streams.append(Stream(**stream))
 
     # build dataset potentially with streams
     dataset = StreamingTextDataset(
         tokenizer=tokenizer,
-        max_seq_len=cfg.dataset.max_seq_len,
         streams=streams,
-        remote=cfg.dataset.get('remote', None),
-        local=cfg.dataset.get('local', None),
-        split=cfg.dataset.get('split', None),
-        download_retry=cfg.dataset.get('download_retry', 2),
-        download_timeout=cfg.dataset.get('download_timeout', 60),
-        validate_hash=cfg.dataset.get('validate_hash', None),
-        keep_zip=cfg.dataset.get('keep_zip', False),
-        keep_raw=cfg.dataset.get('keep_raw', True),
-        samples_per_epoch=cfg.dataset.get('samples_per_epoch', None),
-        predownload=cfg.dataset.get('predownload', 100_000),
-        partition_algo=cfg.dataset.get('partition_algo', 'orig'),
-        num_canonical_nodes=cfg.dataset.get('num_canonical_nodes', 128),
-        batch_size=device_batch_size,
-        shuffle=cfg.dataset.get('shuffle', False),
-        shuffle_algo=cfg.dataset.get('shuffle_algo', 'py1s'),
-        shuffle_seed=cfg.dataset.get('shuffle_seed', 9176),
+        **cfg.dataset,
     )
 
-    mlm_probability = cfg.dataset.get('mlm_probability', None)
     collate_fn = transformers.DataCollatorForLanguageModeling(
         tokenizer=dataset.tokenizer,
         mlm=mlm_probability is not None,
         mlm_probability=mlm_probability)
 
-    eos_token_id = cfg.dataset.get('eos_token_id')
-    bos_token_id = cfg.dataset.get('bos_token_id')
     if (eos_token_id is not None) or (bos_token_id is not None):
         # Note: Will raise an error if both are non-None
         collate_fn = ConcatenatedSequenceCollatorWrapper(
             base_collator=collate_fn,
             eos_token_id=eos_token_id,
             bos_token_id=bos_token_id)
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/__init__.py` & `llm-foundry-0.2.0/llmfoundry/models/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/models/hf/__init__.py` & `llm-foundry-0.2.0/llmfoundry/models/hf/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/models/hf/hf_fsdp.py` & `llm-foundry-0.2.0/llmfoundry/models/hf/hf_fsdp.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 # helper functions from https://github.com/CarperAI/trlx/blob/main/trlx/utils/modeling.py
 # which is MIT licensed
 
 import functools
 from typing import Any, Iterable, List
 
+import torch
 from transformers import PreTrainedModel
 from transformers.models.opt.modeling_opt import OPTDecoder
 
-# helper functions
-
 
+# helper functions
 def rhasattr(obj: Any, attr: str):
     """A chain-able attribute version of hasattr.
 
     For example, to check if
     `obj` has the attribute `foo.bar.baz`, you can use:
         `rhasattr(obj, "foo.bar.baz")`
     Reference: https://stackoverflow.com/a/67303315
@@ -88,31 +88,42 @@
         'layers',  # ProphetNet, Marian (from encoder)
         'model.layers',  # LLaMa
         'transformer.blocks',  # MPT
     )
     return findattr(model, hidden_layers_attrs)
 
 
+def hf_get_init_device(init_device: str):
+    """Returns the appropriate device to initialize models."""
+    from composer.utils import dist
+    if init_device == 'mixed':
+        if dist.get_local_rank() == 0:
+            return 'cpu'
+        return 'meta'
+    return init_device
+
+
 # /end helper functions
 
 
-def prepare_hf_model_for_fsdp(model: PreTrainedModel) -> None:
+def prepare_hf_model_for_fsdp(model: PreTrainedModel, init_device: str) -> None:
     """FSDP wrap a HuggingFace model.
 
     Call specific functions
     """
     if model.config.is_encoder_decoder:
-        prepare_hf_enc_dec_model_for_fsdp(model)
+        prepare_hf_enc_dec_model_for_fsdp(model, init_device)
     else:
         # many common decoder-only model do not set the flag
         # model.config.is_decoder, so we can't trust it
-        prepare_hf_causal_lm_model_for_fsdp(model)
+        prepare_hf_causal_lm_model_for_fsdp(model, init_device)
 
 
-def prepare_hf_causal_lm_model_for_fsdp(model: PreTrainedModel) -> None:
+def prepare_hf_causal_lm_model_for_fsdp(model: PreTrainedModel,
+                                        init_device: str) -> None:
     """FSDP wrap a HuggingFace decoder.
 
     Wrap any model for FSDP which follows one of the 3 existing conventions from
     HuggingFace for decoder-only LLMs.
     """
     causal_base_model = hf_get_causal_base_model(model)
     # OPT has an extra layer of wrapping, so special case here
@@ -132,32 +143,57 @@
 
     for mod_name, module in modules.items():
         if module is None:
             raise ValueError(
                 f'Unable to FSDP-wrap this model! `{mod_name}` does not ' +
                 'follow common layer/weight naming conventions.')
     block_type = type(model_block[0])  # type: ignore
-    # When using the HF LM models,
-    # the weights of the self.lm_head and self.transformer.wte are tied.
-    # This tying occurs inside the `self.post_init()` function.
-    # This is a hurdle for FSDP because they need to be in the same FSDP block
-    # These lines ensures that both modules stay together in the top-most block when
-    # the model has this tying enabled (almost all do; this property defaults to True)
-    if model.config.tie_word_embeddings:
-        causal_base_model._fsdp_wrap = False  # type: ignore
-        tied_embeddings._fsdp_wrap = False  # type: ignore
-        lm_head._fsdp_wrap = False  # type: ignore
+    if init_device == 'mixed':
+        # For FSDP with models with different device intiailizations, `mixed`, which
+        # initializes the model on rank 0 on `cpu` and on all other ranks on `meta,``
+        # we need to tag all child modules that are torch.nn.Modules with `_fsdp_wrap`.
+        for child in model.children():
+            if isinstance(child, type(causal_base_model)):
+                continue
+            if isinstance(child, torch.nn.Module):
+                child._fsdp_wrap = True
+
+        for child in causal_base_model.children():
+            if isinstance(child, torch.nn.ModuleList):
+                continue
+            if isinstance(child, torch.nn.Module):
+                child._fsdp_wrap = True
+
+        if model.config.tie_word_embeddings and not model.config.model_type == 'mpt':
+            raise ValueError(
+                'The passed in HuggingFaceModel has tied word embeddings '
+                'and the passed in initialization device is `mixed.` '
+                'In order to support this initialization scheme, we would need to break '
+                'the weight tying. As a result, either use a different initialization scheme '
+                'or in the model config set `tie_word_embeddings=False.`')
+    else:
+        # When using the HF LM models,
+        # the weights of the self.lm_head and self.transformer.wte are tied.
+        # This tying occurs inside the `self.post_init()` function.
+        # This is a hurdle for FSDP because they need to be in the same FSDP block
+        # These lines ensures that both modules stay together in the top-most block when
+        # the model has this tying enabled (almost all do; this property defaults to True)
+        if model.config.tie_word_embeddings:
+            causal_base_model._fsdp_wrap = False  # type: ignore
+            tied_embeddings._fsdp_wrap = False  # type: ignore
+            lm_head._fsdp_wrap = False  # type: ignore
 
     # FSDP Wrap and Activation Checkpoint every model block
     model.fsdp_wrap_fn = lambda module: isinstance(module, block_type)
     model.activation_checkpointing_fn = lambda module: isinstance(
         module, block_type)
 
 
-def prepare_hf_enc_dec_model_for_fsdp(model: PreTrainedModel) -> None:
+def prepare_hf_enc_dec_model_for_fsdp(model: PreTrainedModel,
+                                      init_device: str) -> None:
     """Wrap an encoder/decoder HF model.
 
     This works for T5, BART, Pegasus, PegasusX, but not all enc/dec (ProphetNet)
     You have model.shared, model.encoder, model.decoder and model.lm_head, where
     model.shared are the embeddings which are tied to model.lm_head, and
     model.shared == model.encoder.embed_tokens and model.shared ==
     model.decoder.embed_tokens
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/hf/hf_prefix_lm.py` & `llm-foundry-0.2.0/llmfoundry/models/hf/hf_prefix_lm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Implements a Hugging Prefix LM wrapped inside a :class:`.ComposerModel`."""
 
 from __future__ import annotations
 
-from typing import Union
+from typing import Mapping, Union
 
 from composer.metrics.nlp import LanguageCrossEntropy, MaskedAccuracy
+from composer.utils import dist
 from omegaconf import DictConfig
 from transformers import (AutoConfig, AutoModelForCausalLM, PreTrainedTokenizer,
                           PreTrainedTokenizerFast)
 
+from llmfoundry.models.hf.hf_fsdp import hf_get_init_device
 from llmfoundry.models.hf.model_wrapper import HuggingFaceModelWithZLoss
 from llmfoundry.models.utils import (adapt_tokenizer_for_denoising,
                                      add_bidirectional_mask_if_missing,
                                      convert_hf_causal_lm_to_prefix_lm,
                                      init_empty_weights)
 
 __all__ = ['ComposerHFPrefixLM']
@@ -65,55 +67,85 @@
                 the weights. Default: ``False``.
         tokenizer (PreTrainedTokenizer): The tokenizer that the model will use.
     """
 
     def __init__(self, om_model_config: DictConfig, tokenizer: Tokenizer):
         config = AutoConfig.from_pretrained(
             om_model_config.pretrained_model_name_or_path,
-            **om_model_config.get('config_overrides', {}))
+            trust_remote_code=om_model_config.get('trust_remote_code', True),
+            use_auth_token=om_model_config.get('use_auth_token', False),
+        )
+
+        # set config overrides
+        for k, v in om_model_config.get('config_overrides', {}).items():
+            if not hasattr(config, k):
+                raise ValueError(
+                    f'config does not have attribute "{k}" to override ({k}: {v}).'
+                )
+
+            attr = getattr(config, k)
+            if isinstance(attr, Mapping):
+                extra_keys = [_k for _k in v.keys() if _k not in attr.keys()]
+                if extra_keys:
+                    raise ValueError(
+                        f'Config dict override got unknown keys. '
+                        f'Extra keys: {extra_keys}. '
+                        f'Expected (a subset of) keys: {list(attr.keys())}.')
+                getattr(config, k).update(v)
+            else:
+                setattr(config, k, v)
 
         # Set up the tokenizer (add tokens for denoising sentinels if needed)
         if om_model_config.get('adapt_vocab_for_denoising', False):
             adapt_tokenizer_for_denoising(tokenizer)
 
-        vocab_size = len(tokenizer)
-
         init_device = om_model_config.get('init_device', 'cpu')
-        if init_device == 'cpu':
+
+        # Get the device we want to initialize, and use the
+        # reolved version to initialize the HF model
+        resolved_init_device = hf_get_init_device(init_device)
+
+        # We need to have all non-zero local ranks be not-pretrained
+        # Rank 0 will still be pretrained, and distribute the weights appropriately
+        if dist.get_local_rank() != 0 and init_device == 'mixed':
+            om_model_config.pretrained = False
+
+        if resolved_init_device == 'cpu':
             if om_model_config.pretrained:
                 model = AutoModelForCausalLM.from_pretrained(
                     om_model_config.pretrained_model_name_or_path,
                     config=config)
             else:
                 model = AutoModelForCausalLM.from_config(config)
-        elif init_device == 'meta':
+        elif resolved_init_device == 'meta':
             if om_model_config.pretrained:
                 raise ValueError(
                     'Setting cfg.pretrained=True is not supported when init_device="meta".'
                 )
             with init_empty_weights(include_buffers=False):
                 model = AutoModelForCausalLM.from_config(config)
         else:
             raise ValueError(
                 f'init_device="{init_device}" must be either "cpu" or "meta".')
 
         # Convert the Causal LM into a Prefix LM via our custom wrapper
         model = convert_hf_causal_lm_to_prefix_lm(model)
 
         metrics = [
-            LanguageCrossEntropy(vocab_size=vocab_size,
-                                 ignore_index=_HF_IGNORE_INDEX),
+            LanguageCrossEntropy(ignore_index=_HF_IGNORE_INDEX),
             MaskedAccuracy(ignore_index=_HF_IGNORE_INDEX)
         ]
 
         composer_model = super().__init__(model=model,
+                                          shift_labels=True,
                                           tokenizer=tokenizer,
                                           metrics=metrics,
                                           z_loss=om_model_config.get(
-                                              'z_loss', 0.0))
+                                              'z_loss', 0.0),
+                                          init_device=init_device)
 
         return composer_model
 
     def forward(self, batch):
         # Add bidirectional_mask if it is missing and can be constructed
         add_bidirectional_mask_if_missing(batch)
         return super().forward(batch)
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/hf/hf_t5.py` & `llm-foundry-0.2.0/llmfoundry/models/hf/hf_t5.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Implements a Hugging Face T5 wrapped inside a :class:`.ComposerModel`."""
 
 from __future__ import annotations
 
-from typing import Union
+from typing import Mapping, Union
 
 from composer.metrics.nlp import LanguageCrossEntropy, MaskedAccuracy
+from composer.utils import dist
 from omegaconf import DictConfig
 from transformers import (AutoConfig, PreTrainedTokenizer,
                           PreTrainedTokenizerFast, T5ForConditionalGeneration)
 
+from llmfoundry.models.hf.hf_fsdp import hf_get_init_device
 from llmfoundry.models.hf.model_wrapper import HuggingFaceModelWithZLoss
 from llmfoundry.models.utils import (adapt_tokenizer_for_denoising,
                                      init_empty_weights)
 
 __all__ = ['ComposerHFT5']
 
 Tokenizer = Union[PreTrainedTokenizer, PreTrainedTokenizerFast]
@@ -54,51 +56,80 @@
                 the weights. Default: ``False``.
         tokenizer (PreTrainedTokenizer): The tokenizer that the model will use.
     """
 
     def __init__(self, om_model_config: DictConfig, tokenizer: Tokenizer):
         config = AutoConfig.from_pretrained(
             om_model_config.pretrained_model_name_or_path,
-            **om_model_config.get('config_overrides', {}))
+            trust_remote_code=om_model_config.get('trust_remote_code', True),
+            use_auth_token=om_model_config.get('use_auth_token', False),
+        )
+
+        # set config overrides
+        for k, v in om_model_config.get('config_overrides', {}).items():
+            if not hasattr(config, k):
+                raise ValueError(
+                    f'config does not have attribute "{k}" to override ({k}: {v}).'
+                )
+
+            attr = getattr(config, k)
+            if isinstance(attr, Mapping):
+                extra_keys = [_k for _k in v.keys() if _k not in attr.keys()]
+                if extra_keys:
+                    raise ValueError(
+                        f'Config dict override got unknown keys. '
+                        f'Extra keys: {extra_keys}. '
+                        f'Expected (a subset of) keys: {list(attr.keys())}.')
+                getattr(config, k).update(v)
+            else:
+                setattr(config, k, v)
 
         if not config.is_encoder_decoder:
             raise ValueError(f'Model type "hf_t5" currently only supports T5 models ' +\
                              f'using configs where `is_encoder_decoder` is ``True``.')
 
         # Set up the tokenizer (add tokens for denoising sentinels if needed)
         if om_model_config.get('adapt_vocab_for_denoising', False):
             adapt_tokenizer_for_denoising(tokenizer)
 
-        vocab_size = len(tokenizer)
-
         init_device = om_model_config.get('init_device', 'cpu')
-        if init_device == 'cpu':
+
+        # Get the device we want to initialize, and use the
+        # reolved version to initialize the HF model
+        resolved_init_device = hf_get_init_device(init_device)
+
+        # We need to have all non-zero local ranks be not-pretrained
+        # Rank 0 will still be pretrained, and distribute the weights appropriately
+        if dist.get_local_rank() != 0 and init_device == 'mixed':
+            om_model_config.pretrained = False
+
+        if resolved_init_device == 'cpu':
             if om_model_config.pretrained:
                 model = T5ForConditionalGeneration.from_pretrained(
                     om_model_config.pretrained_model_name_or_path,
                     config=config)
             else:
                 model = T5ForConditionalGeneration(config)
-        elif init_device == 'meta':
+        elif resolved_init_device == 'meta':
             if om_model_config.pretrained:
                 raise ValueError(
                     'Setting cfg.pretrained=True is not supported when init_device="meta".'
                 )
             with init_empty_weights(include_buffers=False):
                 model = T5ForConditionalGeneration(config)
         else:
             raise ValueError(
                 f'init_device="{init_device}" must be either "cpu" or "meta".')
 
         metrics = [
-            LanguageCrossEntropy(vocab_size=vocab_size,
-                                 ignore_index=_HF_IGNORE_INDEX),
+            LanguageCrossEntropy(ignore_index=_HF_IGNORE_INDEX),
             MaskedAccuracy(ignore_index=_HF_IGNORE_INDEX)
         ]
 
         composer_model = super().__init__(model=model,
                                           tokenizer=tokenizer,
                                           metrics=metrics,
                                           z_loss=om_model_config.get(
-                                              'z_loss', 0.0))
+                                              'z_loss', 0.0),
+                                          init_device=init_device)
 
         return composer_model
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/hf/model_wrapper.py` & `llm-foundry-0.2.0/llmfoundry/models/hf/model_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,30 +40,33 @@
     """
 
     def __init__(self,
                  model: transformers.PreTrainedModel,
                  tokenizer: Optional[Tokenizer] = None,
                  metrics: Optional[List[Metric]] = None,
                  eval_metrics: Optional[List[Metric]] = None,
-                 z_loss: float = 0.0):
+                 z_loss: float = 0.0,
+                 shift_labels: bool = False,
+                 init_device: Optional[str] = None):
         super().__init__(model,
                          tokenizer,
                          use_logits=True,
                          metrics=metrics,
-                         eval_metrics=eval_metrics)
+                         eval_metrics=eval_metrics,
+                         shift_labels=shift_labels)
         self.z_loss = float(z_loss)
         if self.z_loss < 0.0:
             raise ValueError(f'z_loss(={z_loss}) cannot be negative.')
 
         self.model_forward_args = inspect.getfullargspec(
             self.model.forward).args
 
         # Note: We need to add the FSDP related attributes to the model AFTER the super init,
         # so that the (possible) embedding resizing doesn't destroy them
-        prepare_hf_model_for_fsdp(self.model)
+        prepare_hf_model_for_fsdp(self.model, init_device)
 
         # This provides support for meta initialization when using FSDP
         self.model.param_init_fn = lambda module: self.model._init_weights(
             module)
 
     def forward(self, batch):
         if isinstance(batch, dict) or isinstance(batch, UserDict):
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/layers/__init__.py` & `llm-foundry-0.2.0/llmfoundry/models/layers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from llmfoundry.models.layers.attention import (
     ATTN_CLASS_REGISTRY, MultiheadAttention, MultiQueryAttention,
     attn_bias_shape, build_alibi_bias, build_attn_bias, flash_attn_fn,
     scaled_multihead_dot_product_attention, triton_flash_attn_fn)
 from llmfoundry.models.layers.blocks import MPTMLP, MPTBlock
+from llmfoundry.models.layers.custom_embedding import SharedEmbedding
 from llmfoundry.models.layers.norm import NORM_CLASS_REGISTRY, LPLayerNorm
 
 __all__ = [
     'scaled_multihead_dot_product_attention',
     'flash_attn_fn',
     'triton_flash_attn_fn',
     'MultiheadAttention',
@@ -18,8 +19,9 @@
     'build_attn_bias',
     'build_alibi_bias',
     'ATTN_CLASS_REGISTRY',
     'MPTMLP',
     'MPTBlock',
     'NORM_CLASS_REGISTRY',
     'LPLayerNorm',
+    'SharedEmbedding',
 ]
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/layers/attention.py` & `llm-foundry-0.2.0/llmfoundry/models/layers/attention.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 import math
 import warnings
 from typing import Optional
 
 import torch
 import torch.nn as nn
 from einops import rearrange
+from packaging import version
 from torch import nn
 
 from llmfoundry.models.layers.norm import LPLayerNorm
 
 
 def _reset_is_causal(num_query_tokens: int, num_key_tokens: int,
                      original_is_causal: bool):
+    # disable causal when it is not needed
+    # necessary for flash & triton for generation with kv_cache
     if original_is_causal and num_query_tokens != num_key_tokens:
         if num_query_tokens != 1:
             raise NotImplementedError(
                 'MPT does not support query and key with different number of tokens, unless number of query tokens is 1.'
             )
         else:
             return False
@@ -28,63 +31,81 @@
 
 
 def scaled_multihead_dot_product_attention(
     query,
     key,
     value,
     n_heads,
+    past_key_value=None,
     softmax_scale=None,
     attn_bias=None,
     key_padding_mask=None,
     is_causal=False,
     dropout_p=0.0,
     training=False,
     needs_weights=False,
     multiquery=False,
 ):
-
     q = rearrange(query, 'b s (h d) -> b h s d', h=n_heads)
-    k = rearrange(key, 'b s (h d) -> b h d s',
-                  h=1 if multiquery else n_heads)  # includes key.t()
-    v = rearrange(value, 'b s (h d) -> b h s d', h=1 if multiquery else n_heads)
+    kv_n_heads = 1 if multiquery else n_heads
+    k = rearrange(key, 'b s (h d) -> b h d s', h=kv_n_heads)
+    v = rearrange(value, 'b s (h d) -> b h s d', h=kv_n_heads)
+
+    if past_key_value is not None:
+        # attn_impl: flash & triton use kernels which expect input shape [b, s, h, d_head].
+        # kv_cache is therefore stored using that shape.
+        # attn_impl: torch stores the kv_cache in the ordering which is most advantageous
+        # for its attn computation ie
+        # keys are stored as tensors with shape [b, h, d_head, s] and
+        # values are stored as tensors with shape [b, h, s, d_head]
+        if len(past_key_value) != 0:
+            k = torch.cat([past_key_value[0], k], dim=3)
+            v = torch.cat([past_key_value[1], v], dim=2)
 
-    min_val = torch.finfo(q.dtype).min
+        past_key_value = (k, v)
 
     b, _, s_q, d = q.shape
     s_k = k.size(-1)
 
     if softmax_scale is None:
         softmax_scale = 1 / math.sqrt(d)
 
     attn_weight = q.matmul(k) * softmax_scale
 
     if attn_bias is not None:
+        # clamp to 0 necessary for torch 2.0 compile()
+        _s_q = max(0, attn_bias.size(2) - s_q)
+        _s_k = max(0, attn_bias.size(3) - s_k)
+        attn_bias = attn_bias[:, :, _s_q:, _s_k:]
+
         if (attn_bias.size(-1) != 1 and
                 attn_bias.size(-1) != s_k) or (attn_bias.size(-2) != 1 and
                                                attn_bias.size(-2) != s_q):
             raise RuntimeError(
                 f'attn_bias (shape: {attn_bias.shape}) is expected to broadcast to shape: {attn_weight.shape}.'
             )
         attn_weight = attn_weight + attn_bias
 
+    min_val = torch.finfo(q.dtype).min
+
     if key_padding_mask is not None:
         if attn_bias is not None:
             warnings.warn(
                 'Propogating key_padding_mask to the attention module ' +\
                 'and applying it within the attention module can cause ' +\
                 'unneccessary computation/memory usage. Consider integrating ' +\
                 'into attn_bias once and passing that to each attention ' +\
                 'module instead.'
             )
         attn_weight = attn_weight.masked_fill(
             ~key_padding_mask.view((b, 1, 1, s_k)), min_val)
 
-    if is_causal:
+    if is_causal and (not q.size(2) == 1):
         s = max(s_q, s_k)
-        causal_mask = attn_weight.new_ones(s, s, dtype=torch.float16)
+        causal_mask = attn_weight.new_ones(s, s, dtype=torch.float32)
         causal_mask = causal_mask.tril()
         causal_mask = causal_mask.to(torch.bool)
         causal_mask = ~causal_mask
         causal_mask = causal_mask[-s_q:, -s_k:]
         attn_weight = attn_weight.masked_fill(causal_mask.view(1, 1, s_q, s_k),
                                               min_val)
 
@@ -92,20 +113,20 @@
 
     if dropout_p:
         attn_weight = torch.nn.functional.dropout(attn_weight,
                                                   p=dropout_p,
                                                   training=training,
                                                   inplace=True)
 
-    out = attn_weight.matmul(v)
+    out = attn_weight.to(v.dtype).matmul(v)
     out = rearrange(out, 'b h s d -> b s (h d)')
 
     if needs_weights:
-        return out, attn_weight
-    return out, None
+        return out, attn_weight, past_key_value
+    return out, None, past_key_value
 
 
 def check_valid_inputs(*tensors, valid_dtypes=[torch.float16, torch.bfloat16]):
     for tensor in tensors:
         if tensor.dtype not in valid_dtypes:
             raise TypeError(f'{tensor.dtype=} must be in {valid_dtypes=}.')
         if not tensor.is_cuda:
@@ -113,14 +134,15 @@
 
 
 def flash_attn_fn(
     query,
     key,
     value,
     n_heads,
+    past_key_value=None,
     softmax_scale=None,
     attn_bias=None,
     key_padding_mask=None,
     is_causal=False,
     dropout_p=0.0,
     training=False,
     needs_weights=False,
@@ -129,14 +151,27 @@
     try:
         from flash_attn import bert_padding, flash_attn_interface  # type: ignore # yapf: disable # isort: skip
     except:
         raise RuntimeError('Please install flash-attn==1.0.3.post0')
 
     check_valid_inputs(query, key, value)
 
+    if past_key_value is not None:
+        if len(past_key_value) != 0:
+            key = torch.cat([past_key_value[0], key], dim=1)
+            value = torch.cat([past_key_value[1], value], dim=1)
+
+        past_key_value = (key, value)
+
+    if attn_bias is not None:
+        # clamp to 0 necessary for torch 2.0 compile()
+        _s_q = max(0, attn_bias.size(2) - query.size(1))
+        _s_k = max(0, attn_bias.size(3) - key.size(1))
+        attn_bias = attn_bias[:, :, _s_q:, _s_k:]
+
     if attn_bias is not None:
         raise NotImplementedError(f'attn_bias not implemented for flash attn.')
 
     batch_size, seqlen = query.shape[:2]
 
     if key_padding_mask is None:
         key_padding_mask = torch.ones_like(key[:, :, 0], dtype=torch.bool)
@@ -185,40 +220,70 @@
         softmax_scale=softmax_scale,
         causal=reset_is_causal,
         return_attn_probs=needs_weights)
 
     output = bert_padding.pad_input(
         rearrange(output_unpad, 'nnz h d -> nnz (h d)'), indices_q, batch_size,
         seqlen)
-    return output, None
+    return output, None, past_key_value
 
 
 def triton_flash_attn_fn(
     query,
     key,
     value,
     n_heads,
+    past_key_value=None,
     softmax_scale=None,
     attn_bias=None,
     key_padding_mask=None,
     is_causal=False,
     dropout_p=0.0,
     training=False,
     needs_weights=False,
     multiquery=False,
 ):
     try:
-        from flash_attn import flash_attn_triton  # type: ignore
+        from llmfoundry.models.layers.flash_attn_triton import flash_attn_func
     except:
-        raise RuntimeError(
-            'Please install flash-attn==1.0.3.post0 and triton==2.0.0.dev20221202'
-        )
+        _installed = False
+        if version.parse(torch.__version__) < version.parse('2.0.0'):
+            _installed = True
+            # if torch1.13.1 revert to using triton flash attn from HazyResearch
+            # with flash-attn==1.0.3.post0 and triton==2.0.0.dev20221202
+            try:
+                from flash_attn.flash_attn_triton import flash_attn_func
+            except:
+                _installed = False
+        if not _installed:
+            # installing triton-pre-mlir works for both torch1.13.1 and torch2.0+
+            # default recommendation is to install this variant
+            raise RuntimeError(
+                'Requirements for `attn_impl: triton` not installed. Either (1) have a CUDA-compatible GPU '
+                'and `pip install .[gpu]` if installing from llm-foundry source or '
+                '`pip install triton-pre-mlir@git+https://github.com/vchiley/triton.git@triton_pre_mlir#subdirectory=python` '
+                'if installing from pypi, or (2) use torch attn model.attn_config.attn_impl=torch (torch attn_impl will be slow). '
+                'Note: (1) requires you have CMake and PyTorch already installed.'
+            )
 
     check_valid_inputs(query, key, value)
 
+    if past_key_value is not None:
+        if len(past_key_value) != 0:
+            key = torch.cat([past_key_value[0], key], dim=1)
+            value = torch.cat([past_key_value[1], value], dim=1)
+
+        past_key_value = (key, value)
+
+    if attn_bias is not None:
+        # clamp to 0 necessary for torch 2.0 compile()
+        _s_q = max(0, attn_bias.size(2) - query.size(1))
+        _s_k = max(0, attn_bias.size(3) - key.size(1))
+        attn_bias = attn_bias[:, :, _s_q:, _s_k:]
+
     if dropout_p:
         raise NotImplementedError(
             f'Dropout not implemented for attn_impl: triton.')
 
     if needs_weights:
         raise NotImplementedError(
             f'attn_impl: triton cannot return attn weights.')
@@ -253,21 +318,20 @@
         # - pytorch docs
         #
         # hopefully the kernels can utilize this and we're jot just wasting BW here
         key = key.expand(*key.shape[:2], n_heads, key.size(-1))
         value = value.expand(*value.shape[:2], n_heads, value.size(-1))
 
     reset_is_causal = _reset_is_causal(query.size(1), key.size(1), is_causal)
-    attn_output = flash_attn_triton.flash_attn_func(query, key, value,
-                                                    attn_bias, reset_is_causal,
-                                                    softmax_scale)
+    attn_output = flash_attn_func(query, key, value, attn_bias, reset_is_causal,
+                                  softmax_scale)
 
     output = attn_output.view(*attn_output.shape[:2], -1)
 
-    return output, None
+    return output, None, past_key_value
 
 
 class MultiheadAttention(nn.Module):
     """Multi-head self attention.
 
     Using torch or triton attention implemetation enables user to also use
     additive bias.
@@ -330,21 +394,23 @@
                 )
         else:
             raise ValueError(f'{attn_impl=} is an invalid setting.')
 
         self.out_proj = nn.Linear(self.d_model, self.d_model, device=device)
         self.out_proj._is_residual = True  # type: ignore
 
-    def forward(self,
-                x,
-                past_key_value=None,
-                attn_bias=None,
-                attention_mask=None,
-                is_causal=True,
-                needs_weights=False):
+    def forward(
+        self,
+        x,
+        past_key_value=None,
+        attn_bias=None,
+        attention_mask=None,
+        is_causal=True,
+        needs_weights=False,
+    ):
         qkv = self.Wqkv(x)
 
         if self.clip_qkv:
             qkv.clamp_(min=-self.clip_qkv, max=self.clip_qkv)
 
         query, key, value = qkv.chunk(3, dim=2)
 
@@ -352,29 +418,20 @@
 
         if self.qk_ln:
             # Applying layernorm to qk
             dtype = query.dtype
             query = self.q_ln(query).to(dtype)
             key = self.k_ln(key).to(dtype)
 
-        if past_key_value is not None:
-            if len(past_key_value) != 0:
-                key = torch.cat([past_key_value[0], key], dim=1)
-                value = torch.cat([past_key_value[1], value], dim=1)
-
-            past_key_value = (key, value)
-
-        if attn_bias is not None:
-            attn_bias = attn_bias[:, :, -query.size(1):, -key.size(1):]
-
-        context, attn_weights = self.attn_fn(
+        context, attn_weights, past_key_value = self.attn_fn(
             query,
             key,
             value,
             self.n_heads,
+            past_key_value=past_key_value,
             softmax_scale=self.softmax_scale,
             attn_bias=attn_bias,
             key_padding_mask=key_padding_mask,
             is_causal=is_causal,
             dropout_p=self.attn_dropout_p,
             training=self.training,
             needs_weights=needs_weights,
@@ -417,17 +474,19 @@
             self.softmax_scale = 1 / math.sqrt(self.head_dim)
         self.attn_dropout_p = attn_pdrop
 
         # NOTE: if we ever want to make attn TensorParallel, I'm pretty sure we'll
         # want to split Wqkv into Wq and Wkv where Wq can be TensorParallel but
         # Wkv shouldn't be TensorParallel
         # - vchiley
-        self.Wqkv = nn.Linear(d_model,
-                              d_model + 2 * self.head_dim,
-                              device=device)
+        self.Wqkv = nn.Linear(
+            d_model,
+            d_model + 2 * self.head_dim,
+            device=device,
+        )
         # for param init fn; enables shape based init of fused layers
         fuse_splits = (d_model, d_model + self.head_dim)
         self.Wqkv._fused = (0, fuse_splits)  # type: ignore
 
         if self.qk_ln:
             layernorm_class = LPLayerNorm if low_precision_layernorm else nn.LayerNorm
             self.q_ln = layernorm_class(d_model, device=device)
@@ -454,21 +513,23 @@
                 )
         else:
             raise ValueError(f'{attn_impl=} is an invalid setting.')
 
         self.out_proj = nn.Linear(self.d_model, self.d_model, device=device)
         self.out_proj._is_residual = True  # type: ignore
 
-    def forward(self,
-                x,
-                past_key_value=None,
-                attn_bias=None,
-                attention_mask=None,
-                is_causal=True,
-                needs_weights=False):
+    def forward(
+        self,
+        x,
+        past_key_value=None,
+        attn_bias=None,
+        attention_mask=None,
+        is_causal=True,
+        needs_weights=False,
+    ):
         qkv = self.Wqkv(x)
 
         if self.clip_qkv:
             qkv.clamp_(min=-self.clip_qkv, max=self.clip_qkv)
 
         query, key, value = qkv.split(
             [self.d_model, self.head_dim, self.head_dim], dim=2)
@@ -477,29 +538,20 @@
 
         if self.qk_ln:
             # Applying layernorm to qk
             dtype = query.dtype
             query = self.q_ln(query).to(dtype)
             key = self.k_ln(key).to(dtype)
 
-        if past_key_value is not None:
-            if len(past_key_value) != 0:
-                key = torch.cat([past_key_value[0], key], dim=1)
-                value = torch.cat([past_key_value[1], value], dim=1)
-
-            past_key_value = (key, value)
-
-        if attn_bias is not None:
-            attn_bias = attn_bias[:, :, -query.size(1):, -key.size(1):]
-
-        context, attn_weights = self.attn_fn(
+        context, attn_weights, past_key_value = self.attn_fn(
             query,
             key,
             value,
             self.n_heads,
+            past_key_value=past_key_value,
             softmax_scale=self.softmax_scale,
             attn_bias=attn_bias,
             key_padding_mask=key_padding_mask,
             is_causal=is_causal,
             dropout_p=self.attn_dropout_p,
             training=self.training,
             needs_weights=needs_weights,
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/layers/blocks.py` & `llm-foundry-0.2.0/llmfoundry/models/layers/blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,17 +88,19 @@
         x: torch.Tensor,
         past_key_value: Optional[Tuple[torch.Tensor]] = None,
         attn_bias: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.ByteTensor] = None,
         is_causal: bool = True,
     ) -> Tuple[torch.Tensor, Optional[Tuple[torch.Tensor]]]:
         a = self.norm_1(x)
-        b, _, past_key_value = self.attn(a,
-                                         past_key_value=past_key_value,
-                                         attn_bias=attn_bias,
-                                         attention_mask=attention_mask,
-                                         is_causal=is_causal)
+        b, attn_weights, past_key_value = self.attn(
+            a,
+            past_key_value=past_key_value,
+            attn_bias=attn_bias,
+            attention_mask=attention_mask,
+            is_causal=is_causal,
+        )
         x = x + self.resid_attn_dropout(b)
         m = self.norm_2(x)
         n = self.ffn(m)
         x = x + self.resid_ffn_dropout(n)
-        return x, past_key_value
+        return x, attn_weights, past_key_value
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/layers/norm.py` & `llm-foundry-0.2.0/llmfoundry/models/layers/norm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
+from typing import Dict, Type
+
 import torch
 
 
 def _cast_if_autocast_enabled(tensor):
     if torch.is_autocast_enabled():
         if tensor.device.type == 'cuda':
             dtype = torch.get_autocast_gpu_dtype()
@@ -48,15 +50,15 @@
                 downcast_weight,
                 downcast_bias,
                 self.eps,
             )
 
 
 def rms_norm(x, weight=None, eps=1e-5):
-    output = x / torch.rsqrt(x.pow(2).mean(-1, keepdim=True) + eps)
+    output = x * torch.rsqrt(x.pow(2).mean(-1, keepdim=True) + eps)
     if weight is not None:
         return output * weight
     return output
 
 
 class RMSNorm(torch.nn.Module):
 
@@ -103,13 +105,13 @@
         downcast_weight = _cast_if_autocast_enabled(
             self.weight) if self.weight is not None else self.weight
         with torch.autocast(enabled=False, device_type=x.device.type):
             return rms_norm(downcast_x, downcast_weight,
                             self.eps).to(dtype=x.dtype)
 
 
-NORM_CLASS_REGISTRY = {
+NORM_CLASS_REGISTRY: Dict[str, Type[torch.nn.Module]] = {
     'layernorm': torch.nn.LayerNorm,
     'low_precision_layernorm': LPLayerNorm,
     'rmsnorm': RMSNorm,
     'low_precision_rmsnorm': LPRMSNorm,
 }
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/mpt/configuration_mpt.py` & `llm-foundry-0.2.0/llmfoundry/models/mpt/configuration_mpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,19 @@
     'alibi_bias_max': 8,
 }
 
 init_config_defaults: Dict = {
     'name': 'kaiming_normal_',
     'fan_mode': 'fan_in',
     'init_nonlinearity': 'relu',
+    'init_div_is_residual': True,
+    'emb_init_std': None,
+    'emb_init_uniform_lim': None,
+    'init_std': None,
+    'init_gain': 0.0,
 }
 
 
 class MPTConfig(PretrainedConfig):
     model_type = 'mpt'
 
     def __init__(
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/mpt/modeling_mpt.py` & `llm-foundry-0.2.0/llmfoundry/models/mpt/modeling_mpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,74 +16,98 @@
 from composer.metrics import (InContextLearningLMAccuracy,
                               InContextLearningLMExpectedCalibrationError,
                               InContextLearningMCExpectedCalibrationError,
                               InContextLearningMultipleChoiceAccuracy,
                               InContextLearningQAAccuracy)
 from composer.metrics.nlp import LanguageCrossEntropy, LanguagePerplexity
 from composer.models import HuggingFaceModel
+from composer.utils import dist
 from omegaconf import DictConfig
 from omegaconf import OmegaConf as om
 from transformers import (PreTrainedModel, PreTrainedTokenizer,
                           PreTrainedTokenizerFast)
 from transformers.modeling_outputs import (BaseModelOutputWithPast,
                                            CausalLMOutputWithPast)
 
 from llmfoundry.models.layers.attention import attn_bias_shape, build_attn_bias
 from llmfoundry.models.layers.blocks import MPTBlock
+from llmfoundry.models.layers.custom_embedding import SharedEmbedding
 from llmfoundry.models.layers.norm import NORM_CLASS_REGISTRY
 from llmfoundry.models.mpt.configuration_mpt import MPTConfig
-# NOTE: We import all the utils directly just so that HuggingFace will detect
-# all the files that it needs to copy into its modules folder. Otherwise it misses
-# the ones imported in the submodule
+
+# NOTE: All utils are imported directly even if unused so that
+# HuggingFace can detect all the needed files to copy into its modules folder.
+# Otherwise, certain modules are missing.
+# isort: off
 from llmfoundry.models.utils.adapt_tokenizer import (
-    AutoTokenizerForMOD, adapt_tokenizer_for_denoising)
+    AutoTokenizerForMOD,  # type: ignore (see note),
+    adapt_tokenizer_for_denoising,  # type: ignore (see note)
+)
 from llmfoundry.models.utils.hf_prefixlm_converter import (
-    add_bidirectional_mask_if_missing, convert_hf_causal_lm_to_prefix_lm)
-from llmfoundry.models.utils.meta_init_context import init_empty_weights
-from llmfoundry.models.utils.param_init_fns import (  # type: ignore
-    MODEL_INIT_REGISTRY, generic_param_init_fn_)
+    add_bidirectional_mask_if_missing,  # type: ignore (see note)
+    convert_hf_causal_lm_to_prefix_lm,  # type: ignore (see note)
+)
+from llmfoundry.models.utils.meta_init_context import \
+    init_empty_weights  # type: ignore (see note)
+from llmfoundry.models.utils.param_init_fns import (
+    generic_param_init_fn_,  # type: ignore (see note)
+    MODEL_INIT_REGISTRY,
+)
+
+try:
+    from llmfoundry.models.layers.flash_attn_triton import flash_attn_func
+except:
+    pass
+# isort: on
 
 Tokenizer = Union[PreTrainedTokenizer, PreTrainedTokenizerFast]
 
 
 class MPTPreTrainedModel(PreTrainedModel):
     config_class = MPTConfig
     base_model_prefix = 'model'
+    _no_split_modules = ['MPTBlock']
 
 
 class MPTModel(MPTPreTrainedModel):
 
     def __init__(self, config: MPTConfig):
         config._validate_config()
         super().__init__(config)
 
         self.attn_impl = config.attn_config['attn_impl']
         self.prefix_lm = config.attn_config['prefix_lm']
         self.attn_uses_sequence_id = config.attn_config['attn_uses_sequence_id']
         self.alibi = config.attn_config['alibi']
         self.alibi_bias_max = config.attn_config['alibi_bias_max']
 
+        if config.init_device == 'mixed':
+            if dist.get_local_rank() == 0:
+                config.init_device = 'cpu'
+            else:
+                config.init_device = 'meta'
+
         if config.norm_type.lower() not in NORM_CLASS_REGISTRY.keys():
             norm_options = ' | '.join(NORM_CLASS_REGISTRY.keys())
             raise NotImplementedError(
                 f'Requested norm type ({config.norm_type}) is not implemented within this repo (Options: {norm_options}).'
             )
         norm_class = NORM_CLASS_REGISTRY[config.norm_type.lower()]
 
         # CogView (https://arxiv.org/abs/2105.13290) and GLM-130B (https://arxiv.org/abs/2210.02414)
         # both report this helping with stabilizing training
         self.embedding_fraction = config.embedding_fraction
 
-        self.wte = nn.Embedding(config.vocab_size,
-                                config.d_model,
-                                device=config.init_device)
+        self.wte = SharedEmbedding(config.vocab_size,
+                                   config.d_model,
+                                   device=config.init_device)
         if not self.alibi:
-            self.wpe = nn.Embedding(config.max_seq_len,
-                                    config.d_model,
-                                    device=config.init_device)
+            self.wpe = torch.nn.Embedding(config.max_seq_len,
+                                          config.d_model,
+                                          device=config.init_device)
         self.emb_drop = nn.Dropout(config.emb_pdrop)
         self.blocks = nn.ModuleList([
             MPTBlock(
                 device=config.init_device,
                 **config.to_dict(),
             ) for _ in range(config.n_layers)
         ])
@@ -103,15 +127,16 @@
         self.attn_bias_shape = attn_bias_shape(
             self.attn_impl,
             config.n_heads,
             config.max_seq_len,
             self.alibi,
             prefix_lm=self.prefix_lm,
             causal=self.is_causal,
-            use_sequence_id=self.attn_uses_sequence_id)
+            use_sequence_id=self.attn_uses_sequence_id,
+        )
 
         if config.no_bias:
             for module in self.modules():
                 if hasattr(module, 'bias') and isinstance(
                         module.bias, nn.Parameter):
                     if config.verbose:
                         warnings.warn(
@@ -126,24 +151,26 @@
         if self.config.init_config['verbose'] > 1:
             init_fn_name = self.config.init_config['name']
             warnings.warn(f'Using {init_fn_name} initialization.')
 
     def get_input_embeddings(self):
         return self.wte
 
-    def set_input_embeddings(self, value):
+    def set_input_embeddings(self, value: nn.Embedding):
         self.wte = value
 
     @torch.no_grad()
-    def _attn_bias(self,
-                   device,
-                   dtype,
-                   attention_mask: Optional[torch.ByteTensor] = None,
-                   prefix_mask: Optional[torch.ByteTensor] = None,
-                   sequence_id: Optional[torch.LongTensor] = None):
+    def _attn_bias(
+        self,
+        device,
+        dtype,
+        attention_mask: Optional[torch.ByteTensor] = None,
+        prefix_mask: Optional[torch.ByteTensor] = None,
+        sequence_id: Optional[torch.LongTensor] = None,
+    ):
         if not self._attn_bias_initialized:
             if self.attn_bias_shape:
                 self.attn_bias = torch.zeros(self.attn_bias_shape,
                                              device=device,
                                              dtype=dtype)
                 self.attn_bias = build_attn_bias(
                     self.attn_impl,
@@ -185,36 +212,36 @@
         if attention_mask is not None:
             s_k = attention_mask.shape[-1]
             if attn_bias is None:
                 attn_bias = torch.zeros((1, 1, 1, s_k),
                                         device=device,
                                         dtype=dtype)
             else:
-                attn_bias = attn_bias[:, :, :, -s_k:]
+                # clamp to 0 necessary for torch 2.0 compile()
+                _s_k = max(0, attn_bias.size(-1) - s_k)
+                attn_bias = attn_bias[:, :, :, _s_k:]
             if prefix_mask is not None and (attention_mask.shape !=
                                             prefix_mask.shape):
                 raise ValueError(
-                    f'attention_mask shape={attention_mask.shape} ' +\
-                    f'and prefix_mask shape={prefix_mask.shape} are not equal.'
-                )
+                    f'attention_mask shape={attention_mask.shape} ' +
+                    f'and prefix_mask shape={prefix_mask.shape} are not equal.')
             min_val = torch.finfo(attn_bias.dtype).min
             attn_bias = attn_bias.masked_fill(
                 ~attention_mask.view(-1, 1, 1, s_k), min_val)
 
         return attn_bias, None
 
     def _apply_prefix_mask(self, attn_bias: torch.Tensor,
                            prefix_mask: torch.Tensor):
         s_k, s_q = attn_bias.shape[-2:]
         if (s_k != self.config.max_seq_len) or (s_q != self.config.max_seq_len):
             raise ValueError(
-                'attn_bias does not match the expected shape. ' +\
-                f'The last two dimensions should both be {self.config.max_length} ' +\
-                f'but are {s_k} and {s_q}.'
-            )
+                'attn_bias does not match the expected shape. ' +
+                f'The last two dimensions should both be {self.config.max_length} '
+                + f'but are {s_k} and {s_q}.')
         seq_len = prefix_mask.shape[-1]
         if seq_len > self.config.max_seq_len:
             raise ValueError(
                 f'prefix_mask sequence length cannot exceed max_seq_len={self.config.max_seq_len}'
             )
 
         # select seq_len subset of attn mask
@@ -244,70 +271,85 @@
 
         # select seq_len subset of attn mask
         attn_bias = attn_bias[..., :seq_len, :seq_len]
 
         # Restrict attention to tokens that share the same value
         # in sequence_id
         cannot_attend = torch.logical_not(
-            torch.eq(sequence_id.view(-1, seq_len, 1),
-                     sequence_id.view(-1, 1, seq_len))).unsqueeze(1)
+            torch.eq(
+                sequence_id.view(-1, seq_len, 1),
+                sequence_id.view(-1, 1, seq_len),
+            )).unsqueeze(1)
         min_val = torch.finfo(attn_bias.dtype).min
         attn_bias = attn_bias.masked_fill(cannot_attend, min_val)
 
         return attn_bias
 
     def forward(
-            self,
-            input_ids: torch.LongTensor,
-            past_key_values: Optional[List[Tuple[torch.FloatTensor]]] = None,
-            attention_mask: Optional[torch.ByteTensor] = None,
-            prefix_mask: Optional[torch.ByteTensor] = None,
-            sequence_id: Optional[torch.LongTensor] = None,
-            return_dict: Optional[bool] = None,
-            output_attentions: Optional[bool] = None,
-            output_hidden_states: Optional[bool] = None,
-            use_cache: Optional[bool] = None):
-        return_dict = return_dict if return_dict is not None else self.config.return_dict
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
+        self,
+        input_ids: torch.LongTensor,
+        past_key_values: Optional[List[Tuple[torch.FloatTensor]]] = None,
+        attention_mask: Optional[torch.ByteTensor] = None,
+        prefix_mask: Optional[torch.ByteTensor] = None,
+        sequence_id: Optional[torch.LongTensor] = None,
+        return_dict: Optional[bool] = None,
+        output_attentions: Optional[bool] = None,
+        output_hidden_states: Optional[bool] = None,
+        use_cache: Optional[bool] = None,
+        inputs_embeds: Optional[torch.Tensor] = None,
+    ):
+        return_dict = (return_dict
+                       if return_dict is not None else self.config.return_dict)
+        use_cache = (use_cache
+                     if use_cache is not None else self.config.use_cache)
 
         if attention_mask is not None:
             attention_mask = attention_mask.bool()
+
         if prefix_mask is not None:
             prefix_mask = prefix_mask.bool()
 
         # These args are passed in by keyword in huggingface's generate function
         # https://github.com/huggingface/transformers/blob/68287689f2f0d8b7063c400230b3766987abf18d/src/transformers/generation/utils.py#L2201-L2206
         # but have not yet been fully implemented in MPTModel
         if not return_dict:
             raise NotImplementedError(
                 'return_dict False is not implemented yet for MPT')
         if output_attentions:
-            raise NotImplementedError(
-                'output_attentions is not implemented yet for MPT')
+            if self.attn_impl != 'torch':
+                raise NotImplementedError(
+                    'output_attentions is not implemented for MPT when using attn_impl `flash` or `triton`.'
+                )
 
-        if attention_mask is not None and attention_mask[:, 0].sum(
-        ) != attention_mask.shape[0] and self.training:
+        if (attention_mask is not None and
+                attention_mask[:, 0].sum() != attention_mask.shape[0] and
+                self.training):
             raise NotImplementedError(
                 'MPT does not support training with left padding.')
 
         if self.prefix_lm and prefix_mask is None:
             raise ValueError(
                 'prefix_mask is a required argument when MPT is configured with prefix_lm=True.'
             )
 
+        # Raise a not implemented error if input_embeds is not None (this is an arg in huggingface transformers and we need to support it for PEFT)
+        if inputs_embeds is not None:
+            raise NotImplementedError(
+                'inputs_embeds is not implemented for MPT.')
+
         if self.training:
             if self.attn_uses_sequence_id and sequence_id is None:
                 raise ValueError(
-                    'sequence_id is a required argument when MPT is configured with attn_uses_sequence_id=True ' +\
-                    'and the model is in train mode.'
-                )
+                    'sequence_id is a required argument when MPT is configured with attn_uses_sequence_id=True '
+                    + 'and the model is in train mode.')
             elif (self.attn_uses_sequence_id is False) and (sequence_id
                                                             is not None):
                 warnings.warn(
-                    'MPT received non-None input for `sequence_id` but is configured with attn_uses_sequence_id=False. ' +\
+                    'MPT received non-None input for `sequence_id` but is configured with attn_uses_sequence_id=False. '
+                    +
                     'This input will be ignored. If you want the model to use `sequence_id`, set attn_uses_sequence_id to True.'
                 )
 
         S = input_ids.size(1)
 
         assert (
             S <= self.config.max_seq_len
@@ -317,36 +359,43 @@
         if self.alibi:
             x = tok_emb
         else:
             past_position = 0
             if past_key_values is not None:
                 if len(past_key_values) != self.config.n_layers:
                     raise ValueError(
-                        f'past_key_values must provide a past_key_value for each attention ' +\
+                        f'past_key_values must provide a past_key_value for each attention '
+                        +
                         f'layer in the network ({len(past_key_values)=}; {self.config.n_layers=}).'
                     )
-                # get the key tensor whose spec should be (batch, seq, dim), and
-                # collect the `seq`, so that the position embedding is shifted
+                # For attn_impl: triton and flash the past key tensor spec is (batch, seq, dim).
+                # For attn_impl: torch the past key tensor spec is (batch, heads, head_dim, seq).
+                # Here we shift position embedding using the `seq` dim of the past key
                 past_position = past_key_values[0][0].size(1)
+                if self.attn_impl == 'torch':
+                    past_position = past_key_values[0][0].size(3)
 
             if S + past_position > self.config.max_seq_len:
                 raise ValueError(
                     f'Cannot forward input with past sequence length {past_position} and current sequence length '
                     f'{S + 1}, this model only supports total sequence length <= {self.config.max_seq_len}.'
                 )
-            pos = torch.arange(past_position,
-                               S + past_position,
-                               dtype=torch.long,
-                               device=input_ids.device).unsqueeze(0)
+            pos = torch.arange(
+                past_position,
+                S + past_position,
+                dtype=torch.long,
+                device=input_ids.device,
+            ).unsqueeze(0)
             if attention_mask is not None:
                 # adjust the position indices to account for padding tokens
-                pos = torch.clamp(pos - torch.cumsum(
-                    (~attention_mask).to(torch.int32), dim=1)[:,
-                                                              past_position:],
-                                  min=0)
+                pos = torch.clamp(
+                    pos - torch.cumsum((~attention_mask).to(torch.int32),
+                                       dim=1)[:, past_position:],
+                    min=0,
+                )
 
             pos_emb = self.wpe(pos)  # type: ignore
             x = tok_emb + pos_emb
 
         if self.embedding_fraction == 1:
             x = self.emb_drop(x)  # type: ignore
         else:
@@ -354,54 +403,70 @@
             x_shrunk = (x * self.embedding_fraction) + (
                 x.detach() * (1 - self.embedding_fraction))
             assert isinstance(self.emb_drop, nn.Module)  # pyright
             x = self.emb_drop(x_shrunk)
 
         attn_bias, attention_mask = self._attn_bias(
             device=x.device,
-            dtype=x.dtype,
+            dtype=torch.float32,
             attention_mask=attention_mask,
             prefix_mask=prefix_mask,
-            sequence_id=sequence_id)
+            sequence_id=sequence_id,
+        )
 
         # initialize the past key values cache if it should be used
         if use_cache and past_key_values is None:
             past_key_values = [() for _ in range(self.config.n_layers)
                               ]  # type: ignore
 
         all_hidden_states = () if output_hidden_states else None
+        all_self_attns = () if output_attentions else None
         for b_idx, block in enumerate(self.blocks):  # type: ignore
             if output_hidden_states:
                 assert all_hidden_states is not None  # pyright
                 all_hidden_states = all_hidden_states + (x,)
-            past_key_value = past_key_values[
-                b_idx] if past_key_values is not None else None
-            x, past_key_value = block(x,
-                                      past_key_value=past_key_value,
-                                      attn_bias=attn_bias,
-                                      attention_mask=attention_mask,
-                                      is_causal=self.is_causal)
+            past_key_value = (past_key_values[b_idx]
+                              if past_key_values is not None else None)
+            x, attn_weights, past_key_value = block(
+                x,
+                past_key_value=past_key_value,
+                attn_bias=attn_bias,
+                attention_mask=attention_mask,
+                is_causal=self.is_causal,
+            )
             if past_key_values is not None:
                 past_key_values[b_idx] = past_key_value
 
+            if output_attentions:
+                assert all_self_attns is not None  # pyright
+                all_self_attns = all_self_attns + (attn_weights,)
+
         x = self.norm_f(x)  # type: ignore
 
+        # add hidden states from the last decoder layer
+        if output_hidden_states:
+            assert all_hidden_states is not None  # pyright
+            all_hidden_states = all_hidden_states + (x,)
+
         return BaseModelOutputWithPast(
             last_hidden_state=x,
             past_key_values=past_key_values,
             hidden_states=all_hidden_states,
+            attentions=all_self_attns,
         )
 
     # Param Initialization, needed for device='meta' fast initialization
     def param_init_fn(self, module):
         init_fn_name = self.config.init_config['name']
-        MODEL_INIT_REGISTRY[init_fn_name](module=module,
-                                          n_layers=self.config.n_layers,
-                                          d_model=self.config.d_model,
-                                          **self.config.init_config)
+        MODEL_INIT_REGISTRY[init_fn_name](
+            module=module,
+            n_layers=self.config.n_layers,
+            d_model=self.config.d_model,
+            **self.config.init_config,
+        )
 
     # FSDP Wrap function
     def fsdp_wrap_fn(self, module):
         return isinstance(module, MPTBlock)
 
     # Activation Checkpointing
     def activation_checkpointing_fn(self, module):
@@ -412,15 +477,23 @@
 
     def __init__(self, config: MPTConfig):
         super().__init__(config)
         if not config.tie_word_embeddings:
             raise ValueError(
                 'MPTForCausalLM only supports tied word embeddings')
 
-        self.transformer = MPTModel(config)
+        print(f'Instantiating an MPTForCausalLM model from {__file__}')
+
+        self.transformer: MPTModel = MPTModel(config)
+
+        for child in self.transformer.children():
+            if isinstance(child, torch.nn.ModuleList):
+                continue
+            if isinstance(child, torch.nn.Module):
+                child._fsdp_wrap = True
 
         # enables scaling output logits; similar to a softmax "temperature"
         # PaLM paper uses scale 1/sqrt(config.d_model)
         self.logit_scale = None
         if config.logit_scale is not None:
             logit_scale = config.logit_scale
             if isinstance(logit_scale, str):
@@ -458,74 +531,94 @@
         prefix_mask: Optional[torch.ByteTensor] = None,
         sequence_id: Optional[torch.LongTensor] = None,
         labels: Optional[torch.LongTensor] = None,
         return_dict: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         use_cache: Optional[bool] = None,
+        inputs_embeds: Optional[torch.FloatTensor] = None,
     ):
-        return_dict = return_dict if return_dict is not None else self.config.return_dict
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
+        return_dict = (return_dict
+                       if return_dict is not None else self.config.return_dict)
+        use_cache = (use_cache
+                     if use_cache is not None else self.config.use_cache)
 
+        # if input_embeds is not none, raise a not implemented error
+        if inputs_embeds is not None:
+            raise NotImplementedError(
+                'inputs_embeds has to be None (for hf/peft support).')
         # decoder outputs consists of (dec_features, layer_state, dec_hidden, dec_attn)
-        outputs = self.transformer(input_ids=input_ids,
-                                   past_key_values=past_key_values,
-                                   attention_mask=attention_mask,
-                                   prefix_mask=prefix_mask,
-                                   sequence_id=sequence_id,
-                                   return_dict=return_dict,
-                                   output_attentions=output_attentions,
-                                   output_hidden_states=output_hidden_states,
-                                   use_cache=use_cache)
+        outputs = self.transformer(
+            input_ids=input_ids,
+            past_key_values=past_key_values,
+            attention_mask=attention_mask,
+            prefix_mask=prefix_mask,
+            sequence_id=sequence_id,
+            return_dict=return_dict,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            use_cache=use_cache,
+        )
 
-        logits = F.linear(outputs.last_hidden_state,
-                          self.transformer.wte.weight)
+        # move outputs to same device as weights for token embedding
+        # needed to support HF `device_map`
+        logits = self.transformer.wte(
+            outputs.last_hidden_state.to(self.transformer.wte.weight.device),
+            True,
+        )
 
         if self.logit_scale is not None:
             if self.logit_scale == 0:
                 warnings.warn(
                     f'Multiplying logits by {self.logit_scale=}. This will produce uniform (uninformative) outputs.'
                 )
             logits *= self.logit_scale
 
         loss = None
         if labels is not None:
-            labels = torch.roll(labels, shifts=-1)
-            labels[:, -1] = -100
-            loss = F.cross_entropy(logits.view(-1, logits.size(-1)),
-                                   labels.to(logits.device).view(-1))
+            _labels = torch.roll(labels, shifts=-1)
+            _labels[:, -1] = -100
+            loss = F.cross_entropy(
+                logits.view(-1, logits.size(-1)),
+                _labels.to(logits.device).view(-1),
+            )
 
         return CausalLMOutputWithPast(
             loss=loss,
             logits=logits,
             past_key_values=outputs.past_key_values,
             hidden_states=outputs.hidden_states,
+            attentions=outputs.attentions,
         )
 
     # Param Initialization, needed for device='meta' fast initialization
     def param_init_fn(self, module):
         init_fn_name = self.config.init_config['name']
-        MODEL_INIT_REGISTRY[init_fn_name](module=module,
-                                          n_layers=self.config.n_layers,
-                                          d_model=self.config.d_model,
-                                          **self.config.init_config)
+        MODEL_INIT_REGISTRY[init_fn_name](
+            module=module,
+            n_layers=self.config.n_layers,
+            d_model=self.config.d_model,
+            **self.config.init_config,
+        )
 
     # FSDP Wrap function
     def fsdp_wrap_fn(self, module):
         return isinstance(module, MPTBlock)
 
     # Activation Checkpointing
     def activation_checkpointing_fn(self, module):
         return isinstance(module, MPTBlock)
 
-    def prepare_inputs_for_generation(self,
-                                      input_ids,
-                                      past_key_values=None,
-                                      inputs_embeds=None,
-                                      **kwargs):
+    def prepare_inputs_for_generation(
+        self,
+        input_ids,
+        past_key_values=None,
+        inputs_embeds=None,
+        **kwargs,
+    ):
         if inputs_embeds is not None:
             raise NotImplementedError(
                 'inputs_embeds is not implemented for MPT yet')
 
         attention_mask = kwargs['attention_mask'].bool()
         if attention_mask[:, -1].sum() != attention_mask.shape[0]:
             raise NotImplementedError(
@@ -583,26 +676,23 @@
         tokenizer: Optional[Tokenizer] = None,
     ):
         resolved_om_model_config = om.to_container(om_model_config,
                                                    resolve=True)
         hf_config = MPTConfig.from_dict(resolved_om_model_config)
         model = MPTForCausalLM(hf_config)
 
-        train_metrics = [
-            LanguageCrossEntropy(hf_config.vocab_size),
-            LanguagePerplexity(hf_config.vocab_size)
-        ]
+        train_metrics = [LanguageCrossEntropy(), LanguagePerplexity()]
         eval_metrics = [
-            LanguageCrossEntropy(hf_config.vocab_size),
-            LanguagePerplexity(hf_config.vocab_size),
+            LanguageCrossEntropy(),
+            LanguagePerplexity(),
             InContextLearningLMAccuracy(),
             InContextLearningMultipleChoiceAccuracy(),
             InContextLearningQAAccuracy(),
             InContextLearningLMExpectedCalibrationError(),
-            InContextLearningMCExpectedCalibrationError()
+            InContextLearningMCExpectedCalibrationError(),
         ]
 
         super().__init__(
             model=model,
             tokenizer=tokenizer,
             use_logits=True,
             metrics=train_metrics,
@@ -613,21 +703,22 @@
 
         self.n_active_params = sum(p.numel() for p in self.parameters())
 
         loss_fn_config = om_model_config.get('loss_fn', 'fused_crossentropy')
         if loss_fn_config == 'fused_crossentropy':
             try:
                 from flash_attn.losses.cross_entropy import CrossEntropyLoss as FusedCrossEntropyLoss  # type: ignore # isort: skip
+
                 if hf_config.verbose > 1:
                     warnings.warn('Using Fused Cross Entropy Loss.')
                 self.loss_fn = FusedCrossEntropyLoss(ignore_index=-100)
             except:
                 raise ValueError(
                     'Fused Cross Entropy is not installed. Either (1) have a CUDA-compatible GPU '
-                    'and `pip install .[gpu]` if installing from source or `pip install xentropy-cuda-lib@git+https://github.com/HazyResearch/flash-attention.git@v0.2.8#subdirectory=csrc/xentropy` '
+                    'and `pip install .[gpu]` if installing from source or `pip install xentropy-cuda-lib@git+https://github.com/HazyResearch/flash-attention.git@v1.0.3#subdirectory=csrc/xentropy` '
                     'if installing from pypi, or (2) set your config model.loss_fn=torch_crossentropy.'
                 )
         elif loss_fn_config == 'torch_crossentropy':
             self.loss_fn = nn.CrossEntropyLoss(ignore_index=-100)
         else:
             raise ValueError(
                 f'Specified loss_fn={self.loss_fn} not recognized. `loss_fn` must be one of [`fused_crossentropy`, `torch_crossentropy`].'
@@ -643,14 +734,15 @@
             add_bidirectional_mask_if_missing(batch)
         # Note: prefix_mask is only used if model.prefix_lm is True
         return self.model(
             input_ids=batch['input_ids'],
             attention_mask=batch.get('attention_mask', None),
             prefix_mask=batch.get('bidirectional_mask', None),
             sequence_id=batch.get('sequence_id', None),
+            inputs_embeds=batch.get('inputs_embeds', None),
         )
 
     def loss(self, outputs, batch):
         targets = self.get_targets(batch)
         return self.loss_fn(outputs.logits.view(-1, outputs.logits.size(-1)),
                             targets.view(-1))
 
@@ -658,11 +750,11 @@
         # Note: this computation does not take into account padding, and assumes
         # that the dataset has been constructed without padding. Additionally, we
         # assume the backward pass is approximately 2x the forward pass
 
         bs, msl = batch['input_ids'].shape[0:2]
         params_flops_per_token = 2 * self.n_active_params
         params_flops_per_seq = params_flops_per_token * msl
-        attn_flops_per_seq = self.model.config.n_layers * 2 * 2 * (
-            self.model.config.d_model * (msl**2))
+        attn_flops_per_seq = (self.model.config.n_layers * 2 * 2 *
+                              (self.model.config.d_model * (msl**2)))
 
         return (params_flops_per_seq + attn_flops_per_seq) * 3 * bs
```

### Comparing `llm-foundry-0.1.0/llmfoundry/models/utils/__init__.py` & `llm-foundry-0.2.0/llmfoundry/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/models/utils/adapt_tokenizer.py` & `llm-foundry-0.2.0/llmfoundry/models/utils/adapt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/models/utils/hf_prefixlm_converter.py` & `llm-foundry-0.2.0/llmfoundry/models/utils/hf_prefixlm_converter.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/models/utils/meta_init_context.py` & `llm-foundry-0.2.0/llmfoundry/models/utils/meta_init_context.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/models/utils/param_init_fns.py` & `llm-foundry-0.2.0/llmfoundry/models/utils/param_init_fns.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/optim/adaptive_lion.py` & `llm-foundry-0.2.0/llmfoundry/optim/adaptive_lion.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/optim/lion.py` & `llm-foundry-0.2.0/llmfoundry/optim/lion.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/optim/outlier_detection.py` & `llm-foundry-0.2.0/llmfoundry/optim/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/utils/__init__.py` & `llm-foundry-0.2.0/llmfoundry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/llmfoundry/utils/builders.py` & `llm-foundry-0.2.0/llmfoundry/utils/builders.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 from typing import Union
 
 from composer import algorithms
-from composer.callbacks import (HealthChecker, LRMonitor, MemoryMonitor,
-                                OptimizerMonitor, RuntimeEstimator,
-                                SpeedMonitor)
+from composer.callbacks import (LRMonitor, MemoryMonitor, OptimizerMonitor,
+                                RuntimeEstimator, SpeedMonitor)
 from composer.core import Evaluator
 from composer.datasets.in_context_learning_evaluation import \
     get_icl_task_dataloader
-from composer.loggers import WandBLogger
+from composer.loggers import TensorboardLogger, WandBLogger
 from composer.optim import DecoupledAdamW
 from composer.optim.scheduler import (ConstantWithWarmupScheduler,
                                       CosineAnnealingWithWarmupScheduler,
                                       LinearWithWarmupScheduler)
 from composer.utils import dist
 from omegaconf import DictConfig
 from omegaconf import OmegaConf as om
@@ -43,16 +42,14 @@
     elif name == 'fdiff':
         return FDiffMetrics(**kwargs)
     elif name == 'runtime_estimator':
         return RuntimeEstimator()
     elif name == 'optimizer_monitor':
         return OptimizerMonitor(log_optimizer_metrics=kwargs.get(
             'log_optimizer_metrics', True),)
-    elif name == 'health_checker':
-        return HealthChecker(**kwargs)
     elif name == 'generate_callback':
         prompts = kwargs.pop('prompts')
         return Generate(prompts=list(prompts), **kwargs)
     elif name == 'global_lr_scaling':
         return GlobalLRScaling(**kwargs)
     elif name == 'layer_freezing':
         return LayerFreezing(**kwargs)
@@ -63,14 +60,16 @@
     else:
         raise ValueError(f'Not sure how to build callback: {name}')
 
 
 def build_logger(name, kwargs):
     if name == 'wandb':
         return WandBLogger(**kwargs)
+    elif name == 'tensorboard':
+        return TensorboardLogger(**kwargs)
     else:
         raise ValueError(f'Not sure how to build logger: {name}')
 
 
 def build_algorithm(name, kwargs):
     if name == 'gradient_clipping':
         return algorithms.GradientClipping(**kwargs)
@@ -209,17 +208,18 @@
                 pad_tok_id = tokenizer.eos_token_id
             else:
                 pad_tok_id = tokenizer.pad_token_id
             label = f'{icl_cfg.label}/{num_fewshot}-shot'
             metric_names = list(icl_cfg.metric_names)
             # TODO: fix Composer bug when copying local paths and destination exists
             destination_path = f'{destination_dir}/{icl_cfg.label}-{num_fewshot}.jsonl'
-            with dist.run_local_rank_zero_first():
-                if os.path.exists(destination_path):
-                    os.remove(destination_path)
+            if dist.get_local_rank() == 0 and os.path.exists(destination_path):
+                os.remove(destination_path)
+            dist.barrier()
+
             dataloaders = get_icl_task_dataloader(
                 icl_cfg.icl_task_type,
                 icl_cfg.dataset_uri,
                 tokenizer,
                 batch_size=icl_cfg.batch_size,
                 max_seq_len=icl_cfg.max_seq_len,
                 pad_tok_id=pad_tok_id,
```

### Comparing `llm-foundry-0.1.0/llmfoundry/utils/config_utils.py` & `llm-foundry-0.2.0/llmfoundry/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/pyproject.toml` & `llm-foundry-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 concurrency = ["thread"]
 include = [
     "llmfoundry/*"
 ]
 
 # Pyright
 [tool.pyright]
-exclude = ['env-**']
+exclude = ['env-**', 'venv*']
+ignore = ['llmfoundry/models/layers/flash_attn_triton.py']
 stubPath = ""  # suppress useless 'stubPath is not a valid directory' errors
 
 reportUnnecessaryIsInstance = "warning"
 reportMissingTypeStubs = "none"
 reportIncompatibleMethodOverride = "none"
 reportIncompatibleVariableOverride = "error"
 reportUnusedImport = "error"
```

### Comparing `llm-foundry-0.1.0/setup.py` & `llm-foundry-0.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,42 +43,56 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 ]
 
 install_requires = [
-    'mosaicml[nlp,streaming,wandb]>=0.14.1,<0.15',
-    'torch==1.13.1',
+    'composer[libcloud,nlp,wandb]>=0.15.0,<0.16',
+    'accelerate>=0.19,<0.20',  # for HF inference `device_map`
+    'mosaicml-streaming>=0.5.1,<0.6',
+    'torch>=1.13.1,<=2.0.1',
     'datasets==2.10.1',
     'sentencepiece==0.1.97',
     'einops==0.5.0',
     'omegaconf>=2.2.3,<3',
-    'pynvml<12',
     'slack-sdk<4',
     'mosaicml-cli>=0.3,<1',
-    'onnx==1.13.1',
-    'onnxruntime==1.14.1',
+    'onnx==1.14.0',
+    'onnxruntime==1.15.1',
+    'cmake>=3.25.0,<=3.26.3',  # required for triton-pre-mlir below
+    # PyPI does not support direct dependencies, so we remove this line before uploading from PyPI
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
     'pre-commit>=2.18.1,<3',
     'pytest>=7.2.1,<8',
     'pytest_codeblocks>=0.16.1,<0.17',
     'pytest-cov>=4,<5',
     'pyright==1.1.296',
     'toml>=0.10.2,<0.11',
     'packaging>=21,<23',
 ]
 
+extra_deps['tensorboard'] = [
+    'composer[tensorboard]>=0.15.0,<0.16',
+]
+
 extra_deps['gpu'] = [
     'flash-attn==v1.0.3.post0',
-    'triton==2.0.0.dev20221202',
+    # PyPI does not support direct dependencies, so we remove this line before uploading from PyPI
+]
+
+extra_deps['peft'] = [
+    'loralib==0.1.1',  # lora core
+    'bitsandbytes==0.39.1',  # 8bit
+    'scipy>=1.10.0,<=1.11.0',  # bitsandbytes dependency; TODO: eliminate when incorporated to bitsandbytes
+    # TODO: pin peft when it stabilizes.
     # PyPI does not support direct dependencies, so we remove this line before uploading from PyPI
 ]
 
 extra_deps['all'] = set(dep for deps in extra_deps.values() for dep in deps)
 
 setup(
     name=_PACKAGE_NAME,
```

### Comparing `llm-foundry-0.1.0/tests/test_data_prep_scripts.py` & `llm-foundry-0.2.0/tests/test_data_prep_scripts.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,16 @@
                 'data_subset': 'en',
                 'splits': ['val_xsmall'],
                 'out_root': './my-copy-c4-1',
                 'compression': None,
                 'concat_tokens': None,
                 'bos_text': None,
                 'eos_text': None,
-                'no_wrap': False
+                'no_wrap': False,
+                'num_workers': None
             }))
     assert os.path.exists(path)
     shutil.rmtree(path, ignore_errors=False)
 
 
 def test_json_script_from_api():
     # test calling it directly
@@ -44,11 +45,12 @@
                 'path': 'scripts/data_prep/example_data/arxiv.jsonl',
                 'out_root': './my-copy-c4-3',
                 'compression': None,
                 'split': 'train',
                 'concat_tokens': None,
                 'bos_text': None,
                 'eos_text': None,
-                'no_wrap': False
+                'no_wrap': False,
+                'num_workers': None
             }))
     assert os.path.exists(path)
     shutil.rmtree(path, ignore_errors=False)
```

### Comparing `llm-foundry-0.1.0/tests/test_dataloader.py` & `llm-foundry-0.2.0/tests/test_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,35 +64,38 @@
                     'splits': [split],
                     'out_root': path,
                     'compression': None,
                     'concat_tokens': 2048,
                     'tokenizer': tokenizer_name,
                     'bos_text': bos_text,
                     'eos_text': eos_text,
-                    'no_wrap': False
+                    'no_wrap': False,
+                    'num_workers': None
                 }))
     else:
         main_hf(
             Namespace(
                 **{
                     'dataset': 'c4',
                     'data_subset': 'en',
                     'splits': [split],
                     'out_root': path,
                     'compression': None,
                     'concat_tokens': None,
                     'tokenizer': tokenizer_name,
                     'bos_text': bos_text,
                     'eos_text': eos_text,
-                    'no_wrap': False
+                    'no_wrap': False,
+                    'num_workers': None,
                 }))
     if not os.path.isdir(path):
         raise RuntimeError(f'c4 dataset at {path} not set up as expected')
 
-    test_cfg = get_config(conf_path='scripts/train/yamls/mpt/125m.yaml')
+    test_cfg = get_config(
+        conf_path='scripts/train/yamls/pretrain/mpt-125m.yaml')
     test_cfg.data_local = data_local
     test_cfg.eval_loader.dataset.split = split
     test_cfg.dataset = om.create({
         'num_canonical_nodes': 1,
         'predownload': 3000,
     })
 
@@ -165,22 +168,23 @@
                 'remote': path,
                 'split': 'val_xsmall',
                 'shuffle': False,
                 'max_seq_len': max_seq_len,
                 'packing_ratio': packing_ratio,
                 'predownload': 1000,
                 'keep_zip': False,
+                'num_workers': None
             },
             'mixture_of_denoisers': {
                 'decoder_only_format': decoder_only_format,
                 'span_mean_lengths_and_ratios': [[3, .15], [8, .5]],
                 'sequence_mask_ratios': 0.25,
             },
             'drop_last': False,
-            'num_workers': 0,
+            'num_workers': 4,
         }
         cfg = om.create(cfg)
         device_batch_size = 2
 
         expected_keys = ['input_ids', 'attention_mask', 'labels']
         if decoder_only_format:
             expected_keys += ['bidirectional_mask']
@@ -232,15 +236,15 @@
             'max_seq_len': max_seq_len,
             'decoder_only_format': decoder_only_format,
             'allow_pad_trimming': allow_pad_trimming,
             'packing_ratio': packing_ratio,
             'shuffle': True,
         },
         'drop_last': False,
-        'num_workers': 0,
+        'num_workers': 4,
         'pin_memory': False,
         'prefetch_factor': 2,
         'persistent_workers': False,
         'timeout': 0
     }
 
     cfg = om.create(cfg)
```

### Comparing `llm-foundry-0.1.0/tests/test_flash_triton_torch.py` & `llm-foundry-0.2.0/tests/test_flash_triton_torch.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/tests/test_hf_v_mpt.py` & `llm-foundry-0.2.0/tests/test_hf_v_mpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def test_compare_hf_v_mpt(attn_impl, dropout, alibi, mask_val, no_attn_mask):
     warnings.filterwarnings(
         action='ignore',
         message='Torchmetrics v0.9 introduced a new argument class property')
     warnings.filterwarnings(action='ignore',
                             message='Using Fused Cross Entropy Loss.')
 
-    conf_path = 'scripts/train/yamls/mpt/125m.yaml'  # set cfg path
+    conf_path = 'scripts/train/yamls/pretrain/mpt-125m.yaml'  # set cfg path
     batch_size = 2  # set batch size
     device = 'cuda'  # set decive
 
     # ensure reproducibility
     seed = 17
     reproducibility.seed_all(seed)  # set seed
```

### Comparing `llm-foundry-0.1.0/tests/test_icl_datasets.py` & `llm-foundry-0.2.0/tests/test_icl_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
                 start_idx = (
                     inputs == tokenizer.pad_token_id).tolist().index(False)
             else:
                 start_idx = (
                     inputs == tokenizer.eos_token_id).tolist().index(False)
             full_example = tokenizer.decode(inputs[start_idx:])
             answer = batch['labels'][0][0]
+
         if e.label == 'jeopardy/0-shot/american_history':
             assert full_example == bos_tok + 'AMERICAN HISTORY: On May 29, 1765 Patrick Henrys Stamp Act protest was interrupted with this one word\nAnswer: Treason'
             assert answer == ' Treason'
         elif e.label == 'jeopardy/1-shot/american_history':
             assert full_example == bos_tok + 'AMERICAN HISTORY: Witchcraft trials held in this town in 1692 led to the hangings of 19 people\nAnswer: Salem\nAMERICAN HISTORY: On May 29, 1765 Patrick Henrys Stamp Act protest was interrupted with this one word\nAnswer: Treason'
             assert answer == ' Treason'
         elif e.label == 'triviaqa/0-shot':
```

### Comparing `llm-foundry-0.1.0/tests/test_init_fn.py` & `llm-foundry-0.2.0/tests/test_init_fn.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.1.0/tests/test_model.py` & `llm-foundry-0.2.0/tests/test_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
+import contextlib
 import copy
+import gc
 import os
 import warnings
 from typing import cast
 from unittest import mock
 
 import pytest
 import torch
 import torch.nn as nn
-from composer.core.precision import get_precision_context
+from accelerate import init_empty_weights
+from composer.core.precision import Precision, get_precision_context
 from composer.optim import DecoupledAdamW
-from composer.utils import get_device, reproducibility
+from composer.trainer.dist_strategy import prepare_fsdp_module
+from composer.utils import dist, get_device, reproducibility
 from omegaconf import DictConfig
 from omegaconf import OmegaConf as om
-from transformers import PreTrainedTokenizer, PreTrainedTokenizerFast
+from transformers import (AutoConfig, AutoModelForCausalLM, AutoTokenizer,
+                          PreTrainedTokenizer, PreTrainedTokenizerFast,
+                          pipeline)
 from transformers.modeling_outputs import CausalLMOutputWithPast
 from transformers.models.bloom.modeling_bloom import build_alibi_tensor
 
 from llmfoundry import (COMPOSER_MODEL_REGISTRY, ComposerHFCausalLM,
                         ComposerHFPrefixLM)
+from llmfoundry.models.hf.model_wrapper import HuggingFaceModelWithZLoss
 from llmfoundry.models.layers import NORM_CLASS_REGISTRY, build_alibi_bias
+from llmfoundry.models.layers.blocks import MPTBlock
 from llmfoundry.models.mpt import MPTConfig, MPTForCausalLM
 from llmfoundry.utils import build_tokenizer
 
 
-def get_config(conf_path='scripts/train/yamls/mpt/testing.yaml') -> DictConfig:
+def get_config(
+        conf_path='scripts/train/yamls/pretrain/testing.yaml') -> DictConfig:
     os.environ['TOKENIZERS_PARALLELISM'] = 'false'
     print(conf_path)
     with open(conf_path) as f:
         test_cfg = om.load(f)
     return cast(DictConfig, test_cfg)
 
 
-def get_objs(conf_path='scripts/train/yamls/mpt/testing.yaml'):
+def get_objs(conf_path='scripts/train/yamls/pretrain/testing.yaml'):
     warnings.filterwarnings(
         action='ignore',
         message='Torchmetrics v0.9 introduced a new argument class property')
     test_cfg = get_config(conf_path=conf_path)
 
     reproducibility.seed_all(test_cfg.seed)
 
@@ -60,16 +69,18 @@
     test_cfg.model.init_device = device
     test_cfg.device = device
 
     test_cfg.global_train_batch_size = 2
     test_cfg.device_eval_batch_size = 2
     test_cfg.device_train_microbatch_size = 2
 
+    tokenizer = build_tokenizer(test_cfg.tokenizer)
+
     model = COMPOSER_MODEL_REGISTRY[test_cfg.model.name](test_cfg.model,
-                                                         test_cfg.tokenizer)
+                                                         tokenizer)
     # Optimizer
     assert test_cfg.optimizer.name == 'decoupled_adamw'
     optimizer = DecoupledAdamW(model.parameters(),
                                lr=test_cfg.optimizer.lr,
                                betas=test_cfg.optimizer.betas,
                                eps=test_cfg.optimizer.eps,
                                weight_decay=test_cfg.optimizer.weight_decay)
@@ -112,15 +123,15 @@
                                          dtype=torch.int64).to(device)
     batch['decoder_attention_mask'] = batch['attention_mask'].clone()
     return batch
 
 
 def test_full_forward_and_backward(batch_size=2):
     test_cfg, model, optimizer = get_objs(
-        conf_path='scripts/train/yamls/mpt/testing.yaml')
+        conf_path='scripts/train/yamls/pretrain/testing.yaml')
 
     batch = gen_random_batch(batch_size, test_cfg)
 
     assert batch['input_ids'].shape == torch.Size(
         [batch_size, test_cfg.max_seq_len])
     model.train()
     original_params = next(model.parameters()).clone().data
@@ -130,15 +141,15 @@
     optimizer.step()
     updated_params = next(model.parameters()).clone().data
     assert not torch.equal(original_params, updated_params)
 
 
 def test_attention_mechanism(batch_size=2):
     test_cfg, model, _ = get_objs(
-        conf_path='scripts/train/yamls/mpt/testing.yaml')
+        conf_path='scripts/train/yamls/pretrain/testing.yaml')
 
     batch = gen_random_batch(batch_size, test_cfg)
 
     model.eval()
     # run a partial forward where we explicitly inspect the attention_mask from the causal_attn block
     input_ids, attention_mask = batch['input_ids'], batch[
         'attention_mask'].bool()
@@ -190,15 +201,15 @@
 
 
 @pytest.mark.parametrize('prefixlm', [False, True])
 def test_full_forward_and_backward_gpt2_small(prefixlm, batch_size=2):
     warnings.filterwarnings(
         action='ignore',
         message='Torchmetrics v0.9 introduced a new argument class property')
-    conf_path = 'scripts/train/yamls/hf_causal_lm/gpt2-small.yaml'
+    conf_path = 'scripts/train/yamls/pretrain/gpt2-small.yaml'
     with open(conf_path) as f:
         neo_cfg = om.load(f)
 
     device = 'cpu'
     neo_cfg.device = device
     neo_cfg.max_seq_len = 256
 
@@ -238,15 +249,15 @@
     assert not torch.equal(original_params, updated_params)
 
 
 def test_full_forward_and_backward_t5_small(batch_size=2):
     warnings.filterwarnings(
         action='ignore',
         message='Torchmetrics v0.9 introduced a new argument class property')
-    conf_path = 'scripts/train/yamls/hf_t5/t5-small_dolly_sft.yaml'
+    conf_path = 'scripts/train/yamls/finetune/t5-small_dolly_sft.yaml'
     with open(conf_path) as f:
         t5_cfg = om.load(f)
 
     device = 'cpu'
     t5_cfg.device = device
     t5_cfg.max_seq_len = 16
 
@@ -288,26 +299,28 @@
 def test_determinism(attn_impl: str, precision):
     if not torch.cuda.is_available():
         pytest.skip(
             'This test requires CUDA to be available in order to run with bfloat16 precision.'
         )
     reproducibility.seed_all(1111)
 
-    conf_path = 'scripts/train/yamls/mpt/testing.yaml'
+    conf_path = 'scripts/train/yamls/pretrain/testing.yaml'
     with open(conf_path) as f:
         test_cfg = om.load(f)
 
     test_cfg.model.attn_config = {
         'attn_impl': attn_impl,
     }
     test_cfg.model.init_device = 'cuda:0'
     test_cfg.device = 'cuda:0'
 
+    tokenizer = build_tokenizer(test_cfg.tokenizer)
+
     model_1 = COMPOSER_MODEL_REGISTRY[test_cfg.model.name](test_cfg.model,
-                                                           test_cfg.tokenizer)
+                                                           tokenizer)
     model_2 = copy.deepcopy(model_1)
 
     optimizer_1 = DecoupledAdamW(model_1.parameters(),
                                  lr=test_cfg.optimizer.lr,
                                  betas=test_cfg.optimizer.betas,
                                  eps=test_cfg.optimizer.eps,
                                  weight_decay=test_cfg.optimizer.weight_decay)
@@ -342,29 +355,37 @@
     between the two loss implementations.
     """
     try:
         from flash_attn.losses.cross_entropy import CrossEntropyLoss as FusedCrossEntropyLoss  # type: ignore # isort: skip
     except:
         pytest.skip('Fused cross entropy was not installed')
 
-    reproducibility.seed_all(1111)
+    # run numerical test in pure fp32
+    torch.backends.cuda.matmul.allow_tf32 = False  # type: ignore (third-party)
+    torch.backends.cudnn.allow_tf32 = False  # type: ignore (third-party)
 
-    conf_path = 'scripts/train/yamls/mpt/testing.yaml'
+    conf_path = 'scripts/train/yamls/pretrain/testing.yaml'
     with open(conf_path) as f:
         test_cfg = om.load(f)
 
+    assert isinstance(test_cfg, DictConfig)
+
     test_cfg.device = 'cuda:0'
     test_cfg.model.init_device = 'cuda:0'
     test_cfg.model.init_config = {
         'name': 'baseline_',
         'init_std': 0.02,
     }
 
+    reproducibility.seed_all(test_cfg.get('global_seed', 42))
+
+    tokenizer = build_tokenizer(test_cfg.tokenizer)
+
     model_1 = COMPOSER_MODEL_REGISTRY[test_cfg.model.name](test_cfg.model,
-                                                           test_cfg.tokenizer)
+                                                           tokenizer)
     model_2 = copy.deepcopy(model_1)
     assert isinstance(model_1.loss_fn, torch.nn.CrossEntropyLoss)
     model_2.loss_fn = FusedCrossEntropyLoss(ignore_index=-100)
 
     optimizer_1 = DecoupledAdamW(model_1.parameters(),
                                  lr=test_cfg.optimizer.lr,
                                  betas=test_cfg.optimizer.betas,
@@ -372,15 +393,15 @@
                                  weight_decay=test_cfg.optimizer.weight_decay)
     optimizer_2 = DecoupledAdamW(model_2.parameters(),
                                  lr=test_cfg.optimizer.lr,
                                  betas=test_cfg.optimizer.betas,
                                  eps=test_cfg.optimizer.eps,
                                  weight_decay=test_cfg.optimizer.weight_decay)
 
-    for i in range(25):
+    for i in range(15):
         batch = gen_random_batch(2, test_cfg)
         output_1 = model_1(batch)
         output_2 = model_2(batch)
         assert output_1.logits.allclose(output_2.logits, rtol=1e-4,
                                         atol=1e-4), f'differed at step {i}'
 
         loss_1 = model_1.loss(output_1, batch)
@@ -408,18 +429,20 @@
         },
         'tokenizer': {
             'name': 'facebook/opt-125m'
         }
     }
     config = DictConfig(conf)
 
+    tokenizer = build_tokenizer(config.tokenizer)
+
     if prefixlm:
-        model = ComposerHFPrefixLM(config.model, config.tokenizer)
+        model = ComposerHFPrefixLM(config.model, tokenizer)
     else:
-        model = ComposerHFCausalLM(config.model, config.tokenizer)
+        model = ComposerHFCausalLM(config.model, tokenizer)
 
     # check that all the modules we except are blocked from FSDP wrapping
     assert not model.model.model._fsdp_wrap
     assert not model.model.model.decoder._fsdp_wrap
     assert not model.model.model.decoder.embed_tokens._fsdp_wrap
     assert not model.model.lm_head._fsdp_wrap
 
@@ -447,33 +470,32 @@
 
     assert mpt.config.d_model == 128
     assert mpt.config.n_heads == 4
     assert mpt.config.n_layers == 2
     assert mpt.config.expansion_ratio == 2
     assert mpt.config.max_seq_len == 2048
 
-    assert mpt.transformer.wte.weight.shape == torch.Size(  # type: ignore
+    assert mpt.transformer.wte.weight.shape == torch.Size(
         [hf_config.vocab_size, hf_config.d_model])
-    assert mpt.transformer.wpe.weight.shape == torch.Size(  # type: ignore
+    assert mpt.transformer.wpe.weight.shape == torch.Size(
         [hf_config.max_seq_len, hf_config.d_model])
-    assert mpt.transformer.emb_drop.p == 0.1  # type: ignore
-    assert len(mpt.transformer.blocks) == 2  # type: ignore
+    assert mpt.transformer.emb_drop.p == 0.1
+    assert len(mpt.transformer.blocks) == 2
 
     d_model = hf_config.d_model
-    for block in mpt.transformer.blocks:  # type: ignore
-        assert block.norm_1.weight.shape == torch.Size([d_model
-                                                       ])  # type: ignore
-        assert block.norm_2.weight.shape == torch.Size([d_model
-                                                       ])  # type: ignore
-        assert block.ffn.up_proj.weight.shape == torch.Size(  # type: ignore
+    for block in mpt.transformer.blocks:
+        assert isinstance(block, MPTBlock)
+        assert block.norm_1.weight.shape == torch.Size([d_model])
+        assert block.norm_2.weight.shape == torch.Size([d_model])
+        assert block.ffn.up_proj.weight.shape == torch.Size(
             [hf_config.d_model * hf_config.expansion_ratio, hf_config.d_model])
-        assert block.ffn.down_proj.weight.shape == torch.Size(  # type: ignore
+        assert block.ffn.down_proj.weight.shape == torch.Size(
             [hf_config.d_model, hf_config.d_model * hf_config.expansion_ratio])
-        assert block.resid_attn_dropout.p == 0.2  # type: ignore
-        assert block.resid_ffn_dropout.p == 0.2  # type: ignore
+        assert block.resid_attn_dropout.p == 0.2
+        assert block.resid_ffn_dropout.p == 0.2
 
 
 @pytest.mark.parametrize('attention_impl,device', [('torch', 'cpu'),
                                                    ('flash', 'gpu'),
                                                    ('triton', 'gpu'),
                                                    ('torch', 'gpu')])
 @pytest.mark.parametrize('alibi', [True, False])
@@ -734,14 +756,70 @@
         assert generation_with_no_padding.shape == (2, 3 + 5)
 
         # check that left padding and no padding produce the same output
         assert generation_with_no_padding[:, 3:].equal(
             generation_with_left_padding[:, 6:])
 
 
+@pytest.mark.gpu
+@pytest.mark.parametrize('world_size', [1, 2])
+@pytest.mark.parametrize('use_cache', [False, True])
+def test_generate_with_device_map(tmp_path, world_size, use_cache):
+    if not torch.cuda.is_available():
+        pytest.skip(f'This test requires CUDA to be available.')
+    if not torch.cuda.device_count() >= world_size:
+        pytest.skip(f'This test requires {world_size} GPUs.')
+
+    save_path = tmp_path / 'test-device-map'
+    hf_config = MPTConfig(
+        init_device='cpu',
+        d_model=128,
+        n_heads=4,
+        n_layers=2,
+        expansion_ratio=2,
+        max_seq_len=2048,
+        emb_pdrop=0.1,
+        resid_pdrop=0.2,
+        attn_config={
+            'attn_impl': 'torch',
+        },
+        use_cache=use_cache,
+    )
+    mpt = MPTForCausalLM(hf_config)
+    mpt.save_pretrained(save_path)
+
+    AutoConfig.register('mpt', MPTConfig)
+    AutoModelForCausalLM.register(MPTConfig, MPTForCausalLM)
+    tokenizer = AutoTokenizer.from_pretrained('EleutherAI/gpt-neox-20b')
+
+    device_map = {
+        'transformer.wte': 0,
+        'transformer.wpe': 0,
+        'transformer.embd_drop': 0,
+        'transformer.blocks.0': 0,
+        'transformer.blocks.1': 1 if world_size == 2 else 0,
+        'transformer.norm_f': 1 if world_size == 2 else 0,
+    }
+
+    pipe = pipeline(
+        'text-generation',
+        model=save_path,
+        tokenizer=tokenizer,
+        torch_dtype=torch.bfloat16,
+        trust_remote_code=True,
+        device_map=device_map,
+    )
+    with torch.autocast('cuda', dtype=torch.bfloat16):
+        out = pipe(
+            'The quick fox jumped over',
+            max_length=10,
+            do_sample=True,
+        )
+
+
 def check_hf_model_equivalence(model1, model2):
     # Checks that two huggingface models are equivalent (config and
     # parameters)
     expected_model_config_dict = model1.config.to_dict()
     new_model_config_dict = model2.config.to_dict()
 
     # this key just says the folder it was loaded from, which is a tmp dir during pytest
@@ -846,97 +924,113 @@
     torch.testing.assert_close(second_output_no_padding.logits,
                                second_output_padding.logits[:,
                                                             -1, :].unsqueeze(1),
                                atol=1e-6,
                                rtol=1e-6)
 
 
-@pytest.mark.parametrize('attention_impl,device', [('torch', 'cpu'),
-                                                   ('flash', 'gpu'),
-                                                   ('triton', 'gpu'),
-                                                   ('torch', 'gpu')])
+@pytest.mark.parametrize('attn_impl,device', [
+    ('torch', 'cpu'),
+    ('flash', 'gpu'),
+    ('triton', 'gpu'),
+    ('torch', 'gpu'),
+])
 @pytest.mark.parametrize('alibi', [True, False])
-def test_forward_with_cache(attention_impl, device, alibi):
+def test_forward_with_cache(attn_impl, device, alibi):
     # Test that model forward with and without the key-value cache produces the
     # same output.
     if not torch.cuda.is_available() and device == 'gpu':
         pytest.skip(
-            f'This test requires CUDA to be available in order to run with {attention_impl} attention.'
+            f'This test requires CUDA to be available in order to run with {attn_impl} attention.'
         )
-    if alibi and attention_impl == 'flash':
+    if alibi and attn_impl == 'flash':
         pytest.skip(f'alibi only implemented with torch and triton attention.')
 
     device = get_device(device)
 
     hf_config = MPTConfig(
         init_device='cpu',
         d_model=128,
         n_heads=4,
         n_layers=2,
         expansion_ratio=2,
         max_seq_len=2048,
         emb_pdrop=0.1,
         resid_pdrop=0.2,
         attn_config={
-            'attn_impl': attention_impl,
+            'attn_impl': attn_impl,
             'alibi': alibi,
         },
-        attn_impl=attention_impl,
+        attn_impl=attn_impl,
         alibi=alibi,
         use_cache=True,
         init_config={
             'name': 'baseline_',
             'init_std': 0.02,
         },
     )
     reproducibility.seed_all(1234)
     mpt = MPTForCausalLM(hf_config)
-    mpt.eval()
     mpt = device.module_to_device(mpt)
+    mpt.eval()
 
     with get_precision_context('amp_bf16' if device.name == 'gpu' else 'fp32'):
         reproducibility.seed_all(1234)
         first_input_ids = torch.tensor([[11274, 16390, 11]])
         first_input_ids = device.tensor_to_device(first_input_ids)
         first_attention_mask = torch.tensor([[1, 1, 1]]).bool()
         first_attention_mask = device.tensor_to_device(first_attention_mask)
 
         # start with passing the first three tokens through
         first_output = mpt(first_input_ids, attention_mask=first_attention_mask)
 
         assert first_output.logits.shape == (1, 3, hf_config.vocab_size)
-        assert len(first_output.past_key_values) == 2
+        assert len(first_output.past_key_values) == hf_config.n_layers
         assert all(
             len(past_key_value) == 2
             for past_key_value in first_output.past_key_values)
-        assert all(past_key_value[0].shape == (1, 3, 128)
-                   for past_key_value in first_output.past_key_values)
-        assert all(past_key_value[1].shape == (1, 3, 128)
-                   for past_key_value in first_output.past_key_values)
+        if attn_impl == 'torch':
+            assert all(past_key_value[0].shape == (1, 4, 32, 3)
+                       for past_key_value in first_output.past_key_values)
+            assert all(past_key_value[1].shape == (1, 4, 3, 32)
+                       for past_key_value in first_output.past_key_values)
+        else:
+            assert all(past_key_value[0].shape == (1, 3, 128)
+                       for past_key_value in first_output.past_key_values)
+            assert all(past_key_value[1].shape == (1, 3, 128)
+                       for past_key_value in first_output.past_key_values)
 
         reproducibility.seed_all(1234)
         second_input_ids = torch.tensor([[11274, 16390, 11, 11274]])
         second_input_ids = device.tensor_to_device(second_input_ids)
         second_attention_mask = torch.tensor([[1, 1, 1, 1]]).bool()
         second_attention_mask = device.tensor_to_device(second_attention_mask)
 
         # pass through the fourth token by itself, using the key-value cache
-        second_output = mpt(second_input_ids[:, -1].unsqueeze(-1),
-                            attention_mask=second_attention_mask,
-                            past_key_values=first_output.past_key_values)
+        second_output = mpt(
+            second_input_ids[:, -1].unsqueeze(-1),
+            past_key_values=first_output.past_key_values,
+            attention_mask=second_attention_mask,
+        )
 
         assert second_output.logits.shape == (1, 1, hf_config.vocab_size)
-        assert len(second_output.past_key_values) == 2
+        assert len(second_output.past_key_values) == hf_config.n_layers
         assert all(
             len(past_key_value) == 2
             for past_key_value in second_output.past_key_values)
-        assert all(past_key_value[0].shape == (1, 4, 128)
-                   for past_key_value in second_output.past_key_values)
-        assert all(past_key_value[1].shape == (1, 4, 128)
-                   for past_key_value in second_output.past_key_values)
+        if attn_impl == 'torch':
+            assert all(past_key_value[0].shape == (1, 4, 32, 4)
+                       for past_key_value in second_output.past_key_values)
+            assert all(past_key_value[1].shape == (1, 4, 4, 32)
+                       for past_key_value in second_output.past_key_values)
+        else:
+            assert all(past_key_value[0].shape == (1, 4, 128)
+                       for past_key_value in second_output.past_key_values)
+            assert all(past_key_value[1].shape == (1, 4, 128)
+                       for past_key_value in second_output.past_key_values)
 
         reproducibility.seed_all(1234)
         # pass through the first four tokens without the key-value cache
         full_output = mpt(second_input_ids,
                           attention_mask=second_attention_mask)
 
         # check that the output is the same whether using the key-value cache or not
@@ -1074,42 +1168,49 @@
     mpt = mpt.to('cuda')
     mpt.eval()
 
     # gen input data
     input_ids = torch.tensor([[11274, 16390, 11]]).to('cuda')
     attention_mask = torch.tensor([[1, 1, 1]]).bool().to('cuda')
 
+    # with get_precision_context('amp_bf16'):
     _ = mpt(input_ids, attention_mask=attention_mask)
 
     # move the model around using different methods
+    mpt = mpt.bfloat16()
     mpt = mpt.to('cpu')
 
     # verify the model still works
     if attention_impl == 'torch':
-        _ = mpt(input_ids.to('cpu'), attention_mask=attention_mask.to('cpu'))
+        with torch.autocast('cpu', dtype=torch.bfloat16, enabled=True):
+            _ = mpt(input_ids.to('cpu'),
+                    attention_mask=attention_mask.to('cpu'))
 
     mpt = mpt.cuda()
+    mpt = mpt.bfloat16()
 
     # verify the model still works
     if attention_impl == 'torch':
-        _ = mpt(input_ids, attention_mask=attention_mask)
+        with torch.autocast('cuda', dtype=torch.bfloat16, enabled=True):
+            _ = mpt(input_ids, attention_mask=attention_mask)
 
     mpt = mpt.to('cpu')
     mpt = mpt.float()
 
     # verify the model still works
     if attention_impl == 'torch':
         _ = mpt(input_ids.to('cpu'), attention_mask=attention_mask.to('cpu'))
 
     mpt = mpt.half()
     mpt = mpt.to(0)  # move to rank0
     mpt = mpt.bfloat16()
 
     # verify the model still works
-    _ = mpt(input_ids, attention_mask=attention_mask)
+    with torch.autocast('cuda', dtype=torch.bfloat16, enabled=True):
+        _ = mpt(input_ids, attention_mask=attention_mask)
 
 
 def test_alibi_vs_hf():
     # compare alibi-bias generation vs HF Bloom model alibi-bias for diff seq len and n_heads
     for n_heads in range(1, 64):
         for seq_len in [1, 2, 8, 13, 64, 195, 256]:
             # hf bloom alibi bais
@@ -1121,7 +1222,166 @@
             # mosaicml alibi bais
             alibi_bias_m = build_alibi_bias(n_heads,
                                             seq_len,
                                             dtype=torch.float32)
             alibi_bias_m = alibi_bias_m[0]
 
             torch.testing.assert_close(alibi_bias_hf, alibi_bias_m)
+
+
+@pytest.mark.parametrize('attn_impl,device', [
+    ('torch', 'cpu'),
+    ('flash', 'gpu'),
+    ('triton', 'gpu'),
+    ('torch', 'gpu'),
+])
+@pytest.mark.parametrize('alibi', [True, False])
+@pytest.mark.parametrize('output_attentions', [True, False])
+@pytest.mark.parametrize('output_hidden_states', [True, False])
+def test_forward_with_output_attentions_and_output_hidden_states(
+        attn_impl, device, alibi, output_attentions, output_hidden_states):
+    # Test that model forward with output_attentions_and_output_hidden_states
+    if not torch.cuda.is_available() and device == 'gpu':
+        pytest.skip(
+            f'This test requires CUDA to be available in order to run with {attn_impl} attention.'
+        )
+    if alibi and attn_impl == 'flash':
+        pytest.skip(f'alibi only implemented with torch and triton attention.')
+    if output_attentions and attn_impl in ['flash', 'triton']:
+        pytest.skip(f'output_attentions only implemented with torch attention.')
+
+    device = get_device(device)
+
+    n_layers = 2
+
+    hf_config = MPTConfig(
+        init_device='cpu',
+        d_model=128,
+        n_heads=4,
+        n_layers=n_layers,
+        expansion_ratio=2,
+        max_seq_len=2048,
+        emb_pdrop=0.1,
+        resid_pdrop=0.2,
+        attn_config={
+            'attn_impl': attn_impl,
+            'alibi': alibi,
+        },
+        attn_impl=attn_impl,
+        alibi=alibi,
+        use_cache=True,
+        init_config={
+            'name': 'baseline_',
+            'init_std': 0.02,
+        },
+    )
+    reproducibility.seed_all(1234)
+    mpt = MPTForCausalLM(hf_config)
+    mpt = device.module_to_device(mpt)
+    mpt.eval()
+
+    with get_precision_context('amp_bf16' if device.name == 'gpu' else 'fp32'):
+        reproducibility.seed_all(1234)
+        input_ids = torch.tensor([[11274, 16390, 11]])
+        input_ids = device.tensor_to_device(input_ids)
+        attention_mask = torch.tensor([[1, 1, 1]]).bool()
+        attention_mask = device.tensor_to_device(attention_mask)
+
+        # start with passing the first three tokens through
+        outputs = mpt(
+            input_ids,
+            attention_mask=attention_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+        )
+
+        if output_attentions:
+            assert len(outputs.attentions) == n_layers
+        if output_hidden_states:
+            assert len(outputs.hidden_states) == n_layers + 1
+
+
+@pytest.mark.gpu
+@pytest.mark.parametrize('init_device', ['cpu', 'meta', 'mixed'])
+@pytest.mark.parametrize('world_size', [2])
+def test_hf_init(tmp_path,
+                 init_device: str,
+                 world_size: int,
+                 batch_size: int = 1):
+    if not torch.cuda.is_available():
+        pytest.skip(f'This test requires CUDA to be available.')
+    if not torch.cuda.device_count() >= world_size:
+        pytest.skip(f'This test requires {world_size} GPUs.')
+
+    torch.cuda.empty_cache()
+    gc.collect()  #just in case
+    torch.cuda.synchronize()
+
+    test_cfg = get_config(conf_path='scripts/train/yamls/pretrain/testing.yaml')
+    test_cfg.device = torch.cuda.current_device()
+
+    device = get_device(None)
+    dist.initialize_dist(device, timeout=30)
+
+    fsdp_config = {
+        'sharding_strategy': 'FULL_SHARD',
+    }
+
+    save_path = tmp_path / 'test-hf-device-init'
+
+    if init_device == 'mixed':
+        if dist.get_local_rank() != 0:
+            init_device = 'meta'
+        else:
+            init_device = 'cpu'
+
+    precision = Precision('amp_bf16')
+
+    hf_config = MPTConfig(
+        init_device=init_device,
+        d_model=32,
+        n_heads=4,
+        n_layers=1,
+        expansion_ratio=2,
+        max_seq_len=128,
+        emb_pdrop=0.1,
+        resid_pdrop=0.2,
+        attn_config={
+            'attn_impl': 'torch',
+        },
+    )
+
+    mpt = MPTForCausalLM(hf_config)
+    mpt.save_pretrained(save_path)
+
+    AutoConfig.register('mpt', MPTConfig)
+    AutoModelForCausalLM.register(MPTConfig, MPTForCausalLM)
+
+    context = contextlib.nullcontext()
+    if init_device == 'meta':
+        context = init_empty_weights(include_buffers=False)
+
+    # Load in a pretrained model with a given context
+    with context:
+        model = AutoModelForCausalLM.from_pretrained(save_path,
+                                                     trust_remote_code=True)
+
+    tokenizer = build_tokenizer(test_cfg.tokenizer)
+    optimizer = DecoupledAdamW(model.parameters(), lr=1e-5, betas=[0.9, 0.99])
+
+    prepare_fsdp_module(model, optimizer, fsdp_config, precision, device, False)
+
+    model = HuggingFaceModelWithZLoss(model, tokenizer)
+
+    batch = gen_random_batch(batch_size, test_cfg)
+
+    original_params = next(model.parameters()).clone().data
+
+    with torch.autocast('cuda', dtype=torch.bfloat16, enabled=True):
+        outputs = model(batch)
+    loss = model.loss(outputs, batch)
+    loss.backward()
+    optimizer.step()
+
+    updated_params = next(model.parameters()).clone().data
+
+    assert not torch.equal(original_params, updated_params)
```

### Comparing `llm-foundry-0.1.0/tests/test_onnx.py` & `llm-foundry-0.2.0/tests/test_onnx.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,40 +25,38 @@
 
 
 def test_onnx_export(tmp_path):
     reproducibility.seed_all(42)
     AutoConfig.register('mpt', MPTConfig)
     AutoModelForCausalLM.register(MPTConfig, MPTForCausalLM)
 
+    batch_size, vocab_size, max_seq_len = 1, 50368, 128
+
     hf_config = MPTConfig(
         init_device='cpu',
-        d_model=128,
+        d_model=64,
         n_heads=4,
         n_layers=2,
         expansion_ratio=2,
-        max_seq_len=2048,
+        max_seq_len=max_seq_len,
         emb_pdrop=0.0,
         resid_pdrop=0.0,
         attn_config={
             'attn_impl': 'torch',
             'alibi': True,
         },
         use_cache=True,
-        vocab_size=50368,
+        vocab_size=vocab_size,
         norm_type='layernorm',
     )
     mpt = MPTForCausalLM(hf_config)
     mpt.eval()
 
     print('Creating random batch...')
-    sample_input = gen_random_batch(
-        1,
-        50368,
-        2048,
-    )
+    sample_input = gen_random_batch(batch_size, vocab_size, max_seq_len)
 
     with torch.no_grad():
         mpt(**sample_input)
 
     torch.onnx.export(
         mpt,
         (sample_input,),
```

### Comparing `llm-foundry-0.1.0/tests/test_tokenizer.py` & `llm-foundry-0.2.0/tests/test_tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 from omegaconf import OmegaConf as om
 from transformers import AutoTokenizer
 
 
-def get_config(conf_path='scripts/train/yamls/mpt/125m.yaml'):
+def get_config(conf_path='scripts/train/yamls/pretrain/mpt-125m.yaml'):
     with open(conf_path) as f:
         test_cfg = om.load(f)
     return test_cfg
 
 
 def test_load_tokenizer():
-    test_cfg = get_config(conf_path='scripts/train/yamls/mpt/125m.yaml')
+    test_cfg = get_config(
+        conf_path='scripts/train/yamls/pretrain/mpt-125m.yaml')
     truncation = True
     padding = 'max_length'
 
     resolved_om_tokenizer_config = om.to_container(test_cfg.tokenizer,
                                                    resolve=True)
     tokenizer_kwargs = resolved_om_tokenizer_config.get(  # type: ignore
         'kwargs', {})
```

### Comparing `llm-foundry-0.1.0/tests/test_training.py` & `llm-foundry-0.2.0/tests/test_training.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Add repo root to path so we can import scripts and test it
 repo_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 sys.path.append(repo_dir)
 from scripts.train.train import main
 
 
-def gpt_tiny_cfg(conf_path='scripts/train/yamls/mpt/125m.yaml'):
+def gpt_tiny_cfg(conf_path='scripts/train/yamls/pretrain/mpt-125m.yaml'):
     """Create gpt tiny cfg."""
     with open(conf_path) as f:
         test_cfg = om.load(f)
     # removes requirement to download / process train set
     test_cfg.train_loader.dataset = test_cfg.eval_loader.dataset
 
     test_cfg.global_train_batch_size = 8
@@ -58,15 +58,16 @@
     warnings.filterwarnings(
         action='ignore',
         category=DeprecationWarning,
         message=
         "Using the 'grad_clip_norm' field in Trainer is deprecated. Please usethe GradientClipping Algorithm in composer.algorithms.gradient_clipping."
     )
 
-    test_cfg = gpt_tiny_cfg(conf_path='scripts/train/yamls/mpt/125m.yaml')
+    test_cfg = gpt_tiny_cfg(
+        conf_path='scripts/train/yamls/pretrain/mpt-125m.yaml')
     test_cfg.eval_subset_num_batches = 2
     if logit_scale:
         test_cfg.model.logit_scale = logit_scale
 
     if device == 'cpu':
         pytest.xfail(
             'FSDP in PyTorch 1.13 does not support precision `Precision.FP32` with sharding_strategy `FULL_SHARD.`'
```

